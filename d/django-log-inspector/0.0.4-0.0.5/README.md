# Comparing `tmp/django_log_inspector-0.0.4.tar.gz` & `tmp/django_log_inspector-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_log_inspector-0.0.4.tar", last modified: Mon Apr 15 13:33:19 2024, max compression
+gzip compressed data, was "django_log_inspector-0.0.5.tar", last modified: Tue Apr 16 13:18:06 2024, max compression
```

## Comparing `django_log_inspector-0.0.4.tar` & `django_log_inspector-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.006750 django_log_inspector-0.0.4/
--rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.4/LICENSE
--rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.4/MANIFEST.in
--rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-15 13:33:19.006567 django_log_inspector-0.0.4/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     1838 2024-04-15 13:01:55.000000 django_log_inspector-0.0.4/README.md
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.006385 django_log_inspector-0.0.4/django_log_inspector.egg-info/
--rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-15 13:33:18.000000 django_log_inspector-0.0.4/django_log_inspector.egg-info/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)      997 2024-04-15 13:33:18.000000 django_log_inspector-0.0.4/django_log_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-15 13:33:18.000000 django_log_inspector-0.0.4/django_log_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-15 13:33:18.000000 django_log_inspector-0.0.4/django_log_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.000393 django_log_inspector-0.0.4/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.4/log_inspector/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.4/log_inspector/admin.py
--rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.4/log_inspector/apps.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.000783 django_log_inspector-0.0.4/log_inspector/migrations/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.4/log_inspector/migrations/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.4/log_inspector/models.py
--rw-r--r--   0 peyman627   (501) staff       (20)      985 2024-01-23 10:07:05.000000 django_log_inspector-0.0.4/log_inspector/settings.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:18.997197 django_log_inspector-0.0.4/log_inspector/static/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:18.997317 django_log_inspector-0.0.4/log_inspector/static/log_inspector/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.001373 django_log_inspector-0.0.4/log_inspector/static/log_inspector/css/
--rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-03-17 11:00:14.000000 django_log_inspector-0.0.4/log_inspector/static/log_inspector/css/input.css
--rw-r--r--   0 peyman627   (501) staff       (20)     8487 2024-04-15 12:53:30.000000 django_log_inspector-0.0.4/log_inspector/static/log_inspector/css/output.css
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.002982 django_log_inspector-0.0.4/log_inspector/static/log_inspector/js/
--rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.4/log_inspector/static/log_inspector/js/alpinejs.min.js
--rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.4/log_inspector/static/log_inspector/js/htmx.min.js
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:18.997434 django_log_inspector-0.0.4/log_inspector/templates/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 13:33:19.006043 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)     9729 2024-04-15 12:17:56.000000 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/home.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2000 2024-04-15 11:56:43.000000 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/log_entries.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2599 2024-04-15 12:53:05.000000 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/log_entries_table.html
--rw-r--r--   0 peyman627   (501) staff       (20)      978 2024-02-15 09:07:48.000000 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/log_files.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/pagination.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1010 2024-04-15 12:21:39.000000 django_log_inspector-0.0.4/log_inspector/templates/log_inspector/start_live.html
--rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.4/log_inspector/tests.py
--rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.4/log_inspector/urls.py
--rw-r--r--   0 peyman627   (501) staff       (20)     2664 2024-03-17 09:58:30.000000 django_log_inspector-0.0.4/log_inspector/utils.py
--rw-r--r--   0 peyman627   (501) staff       (20)     3622 2024-04-15 12:22:26.000000 django_log_inspector-0.0.4/log_inspector/views.py
--rw-r--r--   0 peyman627   (501) staff       (20)      388 2024-04-15 13:01:55.000000 django_log_inspector-0.0.4/pyproject.toml
--rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-15 13:33:19.006788 django_log_inspector-0.0.4/setup.cfg
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.383461 django_log_inspector-0.0.5/
+-rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.5/LICENSE
+-rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.5/MANIFEST.in
+-rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-16 13:18:06.383265 django_log_inspector-0.0.5/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1838 2024-04-16 13:17:59.000000 django_log_inspector-0.0.5/README.md
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.383080 django_log_inspector-0.0.5/django_log_inspector.egg-info/
+-rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-16 13:18:06.000000 django_log_inspector-0.0.5/django_log_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.378677 django_log_inspector-0.0.5/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/admin.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.5/log_inspector/apps.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.378905 django_log_inspector-0.0.5/log_inspector/migrations/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/migrations/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/models.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      985 2024-01-23 10:07:05.000000 django_log_inspector-0.0.5/log_inspector/settings.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.375085 django_log_inspector-0.0.5/log_inspector/static/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.375210 django_log_inspector-0.0.5/log_inspector/static/log_inspector/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.379220 django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/
+-rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/input.css
+-rw-r--r--   0 peyman627   (501) staff       (20)    10025 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/output.css
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.380267 django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/
+-rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/alpinejs.min.js
+-rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/htmx.min.js
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.375334 django_log_inspector-0.0.5/log_inspector/templates/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-16 13:18:06.382711 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)     9719 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/home.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_data.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_table.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_files.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/pagination.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.5/log_inspector/templates/log_inspector/start_live.html
+-rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.5/log_inspector/tests.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.5/log_inspector/urls.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.5/log_inspector/utils.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.5/log_inspector/views.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      388 2024-04-16 13:17:59.000000 django_log_inspector-0.0.5/pyproject.toml
+-rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-16 13:18:06.383499 django_log_inspector-0.0.5/setup.cfg
```

### Comparing `django_log_inspector-0.0.4/LICENSE` & `django_log_inspector-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/PKG-INFO` & `django_log_inspector-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.4
+Version: 0.0.5
 Summary: Read and Download log files
 Author-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Peyman Hassani
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.4-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.5-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.4 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.5 Summary: Read
 and Download log files Author-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
 gmail.com> License: MIT License Copyright (c) 2024 Peyman Hassani Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -14,15 +14,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/peyzor/
 django-log-inspector Description-Content-Type: text/markdown License-File:
 LICENSE # Django Log Inspector ## _Fast and Live view to your log files_ !
-[version](https://img.shields.io/badge/version-0.0.4-blue.svg) [![Open Source]
+[version](https://img.shields.io/badge/version-0.0.5-blue.svg) [![Open Source]
 (https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
 opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and
 analysis of log files in Django projects. It delivers a fast and live view of
 log data, eliminating manual page refreshing. With an intuitive interface and
 live update functionality, it streamlines log file management for easier issue
 tracking and troubleshooting in Django applications. Django Log Inspector is
 available directly from _P_y_P_I: ## Installation ``` pip install django-log-
```

### Comparing `django_log_inspector-0.0.4/README.md` & `django_log_inspector-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.4-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.5-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Django Log Inspector ## _Fast and Live view to your log files_ ![version]
-(https://img.shields.io/badge/version-0.0.4-blue.svg) [![Open Source](https://
+(https://img.shields.io/badge/version-0.0.5-blue.svg) [![Open Source](https://
 badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and analysis of log
 files in Django projects. It delivers a fast and live view of log data,
 eliminating manual page refreshing. With an intuitive interface and live update
 functionality, it streamlines log file management for easier issue tracking and
 troubleshooting in Django applications. Django Log Inspector is available
 directly from _P_y_P_I: ## Installation ``` pip install django-log-inspector ```
```

### Comparing `django_log_inspector-0.0.4/django_log_inspector.egg-info/PKG-INFO` & `django_log_inspector-0.0.5/django_log_inspector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.4
+Version: 0.0.5
 Summary: Read and Download log files
 Author-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Peyman Hassani
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.4-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.5-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.4 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.5 Summary: Read
 and Download log files Author-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
 gmail.com> License: MIT License Copyright (c) 2024 Peyman Hassani Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -14,15 +14,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/peyzor/
 django-log-inspector Description-Content-Type: text/markdown License-File:
 LICENSE # Django Log Inspector ## _Fast and Live view to your log files_ !
-[version](https://img.shields.io/badge/version-0.0.4-blue.svg) [![Open Source]
+[version](https://img.shields.io/badge/version-0.0.5-blue.svg) [![Open Source]
 (https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
 opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and
 analysis of log files in Django projects. It delivers a fast and live view of
 log data, eliminating manual page refreshing. With an intuitive interface and
 live update functionality, it streamlines log file management for easier issue
 tracking and troubleshooting in Django applications. Django Log Inspector is
 available directly from _P_y_P_I: ## Installation ``` pip install django-log-
```

### Comparing `django_log_inspector-0.0.4/django_log_inspector.egg-info/SOURCES.txt` & `django_log_inspector-0.0.5/django_log_inspector.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 log_inspector/views.py
 log_inspector/migrations/__init__.py
 log_inspector/static/log_inspector/css/input.css
 log_inspector/static/log_inspector/css/output.css
 log_inspector/static/log_inspector/js/alpinejs.min.js
 log_inspector/static/log_inspector/js/htmx.min.js
 log_inspector/templates/log_inspector/home.html
-log_inspector/templates/log_inspector/log_entries.html
+log_inspector/templates/log_inspector/log_entries_data.html
 log_inspector/templates/log_inspector/log_entries_table.html
 log_inspector/templates/log_inspector/log_files.html
 log_inspector/templates/log_inspector/pagination.html
 log_inspector/templates/log_inspector/start_live.html
```

### Comparing `django_log_inspector-0.0.4/log_inspector/settings.py` & `django_log_inspector-0.0.5/log_inspector/settings.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/log_inspector/static/log_inspector/css/input.css` & `django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/input.css`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/log_inspector/static/log_inspector/css/output.css` & `django_log_inspector-0.0.5/log_inspector/static/log_inspector/css/output.css`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.4.3 | MIT License | https://tailwindcss.com*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.bottom-3{bottom:.75rem}.right-0{right:0}.right-3{right:.75rem}.top-0{top:0}.z-20{z-index:20}.float-right{float:right}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-auto{margin-left:auto;margin-right:auto}.mb-6{margin-bottom:1.5rem}.ml-6{margin-left:1.5rem}.mr-2{margin-right:.5rem}.mt-1{margin-top:.25rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-6{margin-top:1.5rem}.box-border{box-sizing:border-box}.block{display:block}.flex{display:flex}.table{display:table}.h-10{height:2.5rem}.w-2\/5{width:40%}.w-3\/12{width:25%}.w-9\/12{width:75%}.w-full{width:100%}.min-w-0{min-width:0}.max-w-sm{max-width:24rem}.flex-none{flex:none}.flex-grow{flex-grow:1}.border-collapse{border-collapse:collapse}.cursor-pointer{cursor:pointer}.items-center{align-items:center}.justify-center{justify-content:center}.overflow-hidden{overflow:hidden}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded{border-radius:.25rem}.rounded-md{border-radius:.375rem}.rounded-l{border-top-left-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-r{border-top-right-radius:.25rem;border-bottom-right-radius:.25rem}.border{border-width:1px}.border-2{border-width:2px}.border-gray-300{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.border-green-300{--tw-border-opacity:1;border-color:rgb(134 239 172/var(--tw-border-opacity))}.bg-blue-500{--tw-bg-opacity:1;background-color:rgb(59 130 246/var(--tw-bg-opacity))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231/var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity:1;background-color:rgb(34 197 94/var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity:1;background-color:rgb(239 68 68/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-4{padding-left:1rem;padding-right:1rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.pl-1{padding-left:.25rem}.pr-2{padding-right:.5rem}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.font-bold{font-weight:700}.text-black{--tw-text-opacity:1;color:rgb(0 0 0/var(--tw-text-opacity))}.text-green-600{--tw-text-opacity:1;color:rgb(22 163 74/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.shadow-md{--tw-shadow:0 4px 6px -1px #0000001a,0 2px 4px -2px #0000001a;--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.transition{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.duration-300{transition-duration:.3s}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid #0000;outline-offset:2px}.dark\:border-gray-600:is(.dark *){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.dark\:border-gray-700:is(.dark *){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.dark\:bg-blue-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(29 78 216/var(--tw-bg-opacity))}.dark\:bg-gray-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:bg-green-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(21 128 61/var(--tw-bg-opacity))}.dark\:bg-red-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(185 28 28/var(--tw-bg-opacity))}.dark\:bg-slate-600:is(.dark *){--tw-bg-opacity:1;background-color:rgb(71 85 105/var(--tw-bg-opacity))}.dark\:bg-slate-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(51 65 85/var(--tw-bg-opacity))}.dark\:bg-slate-800:is(.dark *){--tw-bg-opacity:1;background-color:rgb(30 41 59/var(--tw-bg-opacity))}.dark\:text-white:is(.dark *){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.dark\:hover\:bg-gray-500:hover:is(.dark *){--tw-bg-opacity:1;background-color:rgb(107 114 128/var(--tw-bg-opacity))}.dark\:hover\:bg-gray-700:hover:is(.dark *){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}
+/*! tailwindcss v3.4.3 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{-webkit-text-size-adjust:100%;font-feature-settings:normal;-webkit-tap-highlight-color:transparent;font-family:ui-sans-serif,system-ui,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-feature-settings:normal;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{font-feature-settings:inherit;color:inherit;font-family:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;letter-spacing:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.bottom-3{bottom:.75rem}.right-0{right:0}.right-3{right:.75rem}.top-0{top:0}.z-20{z-index:20}.float-right{float:right}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-auto{margin-left:auto;margin-right:auto}.mb-6{margin-bottom:1.5rem}.ml-6{margin-left:1.5rem}.mr-8{margin-right:2rem}.mt-1{margin-top:.25rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-6{margin-top:1.5rem}.box-border{box-sizing:border-box}.block{display:block}.flex{display:flex}.table{display:table}.h-10{height:2.5rem}.w-10{width:2.5rem}.w-2\/5{width:40%}.w-3\/12{width:25%}.w-9\/12{width:75%}.w-full{width:100%}.min-w-0{min-width:0}.max-w-sm{max-width:24rem}.flex-none{flex:none}.flex-grow{flex-grow:1}.table-fixed{table-layout:fixed}.border-collapse{border-collapse:collapse}.cursor-pointer{cursor:pointer}.items-center{align-items:center}.justify-center{justify-content:center}.overflow-hidden{overflow:hidden}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded{border-radius:.25rem}.rounded-md{border-radius:.375rem}.rounded-l{border-bottom-left-radius:.25rem;border-top-left-radius:.25rem}.rounded-r{border-bottom-right-radius:.25rem;border-top-right-radius:.25rem}.border{border-width:1px}.border-2{border-width:2px}.border-gray-300{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.border-green-300{--tw-border-opacity:1;border-color:rgb(134 239 172/var(--tw-border-opacity))}.bg-blue-500{--tw-bg-opacity:1;background-color:rgb(59 130 246/var(--tw-bg-opacity))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231/var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity:1;background-color:rgb(34 197 94/var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity:1;background-color:rgb(239 68 68/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-4{padding-left:1rem;padding-right:1rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.pl-1{padding-left:.25rem}.pr-2{padding-right:.5rem}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.font-bold{font-weight:700}.text-black{--tw-text-opacity:1;color:rgb(0 0 0/var(--tw-text-opacity))}.text-green-600{--tw-text-opacity:1;color:rgb(22 163 74/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.shadow-md{--tw-shadow:0 4px 6px -1px #0000001a,0 2px 4px -2px #0000001a;--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-300{transition-duration:.3s}body{overflow-y:scroll!important}.log-entry-text{white-space:pre-wrap}.lds-roller{display:inline-block;height:80px;position:relative;width:80px}.lds-roller div{animation:lds-roller 1.2s cubic-bezier(.5,0,.5,1) infinite;transform-origin:40px 40px}.lds-roller div:after{background:#fff;border-radius:50%;content:" ";display:block;height:7px;margin:-4px 0 0 -4px;position:absolute;width:7px}.lds-roller div:first-child{animation-delay:-36ms}.lds-roller div:first-child:after{left:63px;top:63px}.lds-roller div:nth-child(2){animation-delay:-72ms}.lds-roller div:nth-child(2):after{left:56px;top:68px}.lds-roller div:nth-child(3){animation-delay:-.108s}.lds-roller div:nth-child(3):after{left:48px;top:71px}.lds-roller div:nth-child(4){animation-delay:-.144s}.lds-roller div:nth-child(4):after{left:40px;top:72px}.lds-roller div:nth-child(5){animation-delay:-.18s}.lds-roller div:nth-child(5):after{left:32px;top:71px}.lds-roller div:nth-child(6){animation-delay:-.216s}.lds-roller div:nth-child(6):after{left:24px;top:68px}.lds-roller div:nth-child(7){animation-delay:-.252s}.lds-roller div:nth-child(7):after{left:17px;top:63px}.lds-roller div:nth-child(8){animation-delay:-.288s}.lds-roller div:nth-child(8):after{left:12px;top:56px}@keyframes lds-roller{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.loading-spinner{align-items:center;background-color:#0009;display:flex;height:100vh;justify-content:center;left:0;position:fixed;top:0;width:100vw;z-index:10000}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid #0000;outline-offset:2px}.dark\:border-gray-100\/50:is(.dark *){border-color:#f3f4f680}.dark\:border-gray-600:is(.dark *){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.dark\:border-gray-700:is(.dark *){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.dark\:border-b-gray-100\/50:is(.dark *){border-bottom-color:#f3f4f680}.dark\:bg-blue-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(29 78 216/var(--tw-bg-opacity))}.dark\:bg-gray-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:bg-green-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(21 128 61/var(--tw-bg-opacity))}.dark\:bg-red-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(185 28 28/var(--tw-bg-opacity))}.dark\:bg-slate-600:is(.dark *){--tw-bg-opacity:1;background-color:rgb(71 85 105/var(--tw-bg-opacity))}.dark\:bg-slate-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(51 65 85/var(--tw-bg-opacity))}.dark\:bg-slate-800:is(.dark *){--tw-bg-opacity:1;background-color:rgb(30 41 59/var(--tw-bg-opacity))}.dark\:text-white:is(.dark *){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.dark\:hover\:bg-gray-500:hover:is(.dark *){--tw-bg-opacity:1;background-color:rgb(107 114 128/var(--tw-bg-opacity))}
```

### Comparing `django_log_inspector-0.0.4/log_inspector/static/log_inspector/js/alpinejs.min.js` & `django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/log_inspector/static/log_inspector/js/htmx.min.js` & `django_log_inspector-0.0.5/log_inspector/static/log_inspector/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/log_inspector/templates/log_inspector/home.html` & `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/home.html`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                        hx-get="{% url 'log_inspector:log_files' %}"
                        hx-trigger="load"
                        hx-target="#log-files-data"
                        hx-swap="outerHTML">
                     <tbody id="log-files-data">
                     <tr>
                         <td colspan="2"
-                            class="border p-2 hover:bg-gray-100 dark:hover:bg-gray-500 dark:bg-slate-700 dark:border-gray-700 dark:text-white">
+                            class="p-2 hover:bg-gray-100 dark:hover:bg-gray-500 dark:bg-slate-700 dark:border-gray-100/50 dark:text-white">
                             {% trans 'No entries!' %}
                         </td>
                     </tr>
                     </tbody>
                 </table>
             </div>
         </div>
@@ -184,15 +184,15 @@
                     document.documentElement.classList.toggle('dark', this.on);
                 }
             })
         })
 
         document.addEventListener('htmx:configRequest', function (event) {
             const spinner = document.getElementById('spinner');
-            if (event.detail.headers['X-LIVE-ACTION'] === 'START') {
+            if (event.detail.headers['X-ACTION'] === 'LIVE') {
                 spinner.style.display = 'none';
             } else {
                 spinner.style.display = 'flex';
             }
         });
 
         document.addEventListener('htmx:afterRequest', function (event) {
```

### Comparing `django_log_inspector-0.0.4/log_inspector/templates/log_inspector/log_entries.html` & `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/log_entries_data.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-{% load static i18n %}
+{% load i18n %}
 
 <tbody id="log-entries-data" x-data="{ copiedValue: '' }">
 {% if log_entries %}
+
     {% for log_entry in log_entries %}
-        <tr class="hover:bg-gray-100 dark:hover:bg-gray-500 dark:bg-slate-700 dark:text-white dark:border-gray-700">
-            <td class="border p-2 dark:border-gray-700">{{ forloop.counter }}</td>
-            <td class="border p-2 relative break-words dark:border-gray-700 dark:text-white">
+        <tr class="hover:bg-gray-100 dark:hover:bg-gray-500 dark:bg-slate-700 dark:text-white">
+            <td class="p-2 dark:border-b-gray-100/50 ">{{ start_index|add:forloop.counter }}</td>
+            <td class="p-2 dark:border-b-gray-100/50 relative break-words dark:text-white">
                 <div class="flex items-center">
-                    <div class="flex-grow min-w-0">
+                    <div class="flex-grow min-w-0 mr-8">
                         <p class="log-entry-text">{{ log_entry }}</p>
                     </div>
                     <div x-data="{ showMsg: false }">
                         <i @click="copyText($event); showMsg = true; setTimeout(() => showMsg = false, 2000)"
-                           class="fa-solid fa-copy copy-icon p-2 focus:outline-none cursor-pointer dark:text-white">
+                           class="fa-solid fa-copy copy-icon p-2 focus:outline-none cursor-pointer absolute top-0 right-0">
                         </i>
                         <div x-show="showMsg" @click.away="showMsg = false"
                              class="message fixed bottom-3 right-3 z-20 max-w-sm overflow-hidden bg-green-100 border
-                                        border-green-300 rounded p-3 flex items-center justify-center text-green-600 dark:bg-green-700"
-                             style="position: fixed; bottom: 20px; right: 20px; display: none;">
+                                    border-green-300 rounded p-3 flex items-center justify-center text-green-600
+                                    dark:bg-gray-700 dark:border-gray-600 dark:text-white fixed bottom-15 right-15">
                             {% trans 'Copied to Clipboard' %}
                         </div>
                     </div>
                 </div>
             </td>
         </tr>
     {% endfor %}
 
 {% else %}
-    <tr class="hover:bg-gray-100 dark:hover:bg-gray-700">
+    <tr class="hover:bg-gray-100 dark:hover:bg-gray-500">
         <td class="border p-2 hover:bg-gray-100 dark:hover:bg-gray-500 dark:bg-slate-700 dark:border-gray-700 dark:text-white"
             colspan="2">
             {% trans 'No entries!' %}
         </td>
     </tr>
-{% endif %}
-
-</tbody>
-
-<tfoot id="log-entries-footer" hx-swap-oob="true" class="dark:bg-slate-800">
-{% include 'log_inspector/pagination.html' %}
-</tfoot>
+{% endif %}
```

### Comparing `django_log_inspector-0.0.4/log_inspector/templates/log_inspector/pagination.html` & `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/pagination.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/log_inspector/templates/log_inspector/start_live.html` & `django_log_inspector-0.0.5/log_inspector/templates/log_inspector/start_live.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% load static i18n %}
 
 <table id="log-entries-table"
-       class="mt-6 w-full border-collapse dark:bg-slate-800"
+       class="mt-6 w-full border-collapse table-fixed dark:bg-slate-800"
        hx-get="{% url 'log_inspector:log_entries' filename=filename %}"
        hx-headers='{"X-ACTION": "LIVE"}'
        hx-trigger="load, every 1s"
        hx-target="#log-entries-data"
        hx-swap="outerHTML">
     <thead>
     <tr>
         <th scope="col"
-            class="border p-2 dark:border-gray-700 dark:bg-slate-700 dark:text-white dark:border-gray-700">
+            class="border p-2 w-10 dark:border-gray-700 dark:bg-slate-700 dark:text-white dark:border-gray-700">
             {% trans 'No.' %}
         </th>
         <th scope="col"
             class="border p-2 dark:border-gray-700 dark:bg-slate-700 dark:text-white dark:border-gray-700">
             {% trans 'Log entries' %}
         </th>
     </tr>
```

### Comparing `django_log_inspector-0.0.4/log_inspector/urls.py` & `django_log_inspector-0.0.5/log_inspector/urls.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.4/log_inspector/utils.py` & `django_log_inspector-0.0.5/log_inspector/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     patterns = settings.LOG_INSPECTOR_PATTERNS
 
     segment = None
     offset = 0
     file.seek(0, os.SEEK_END)
     file_size = remaining_size = file.tell()
 
+    log = []
     while remaining_size > 0:
         offset = min(file_size, offset + buf_size)
         file.seek(file_size - offset)
 
         buffer = file.read(min(remaining_size, buf_size))
 
         # remove the file's last "\n" if it exists, only for the first buffer
@@ -30,15 +31,14 @@
         # append last chunk's segment to this chunk's last line
         if segment is not None:
             lines[-1] += segment
 
         segment = lines[0]
         lines = lines[1:]
 
-        log = []
         for line in reversed(lines):
             log.append(line)
 
             if any([line.startswith(p) for p in patterns]):
                 log_text = '\n'.join(log[::-1])
 
                 if exclude and re.search(exclude, log_text):
```

### Comparing `django_log_inspector-0.0.4/log_inspector/views.py` & `django_log_inspector-0.0.5/log_inspector/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         except PageNotAnInteger:
             log_entries = paginator.page(1)
         except EmptyPage:
             log_entries = paginator.page(paginator.num_pages)
 
         context = {'log_entries': log_entries, 'filename': filename, 'start_index': start_index}
         if is_live_action:
-            return render(request, 'log_inspector/log_entries.html', context)
+            return render(request, 'log_inspector/log_entries_data.html', context)
 
         return render(request, 'log_inspector/log_entries_table.html', context, status=HTMX_STOP_POLLING)
 
 
 class StartLiveView(TemplateView):
     def get(self, request, filename, *args, **kwargs):
         context = {'filename': filename}
```

