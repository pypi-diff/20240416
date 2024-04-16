# Comparing `tmp/django_tailwindcss_automated-0.6.tar.gz` & `tmp/django_tailwindcss_automated-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwindcss_automated-0.6.tar", last modified: Tue Apr 16 18:39:37 2024, max compression
+gzip compressed data, was "django_tailwindcss_automated-0.7.tar", last modified: Tue Apr 16 19:57:49 2024, max compression
```

## Comparing `django_tailwindcss_automated-0.6.tar` & `django_tailwindcss_automated-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1243 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      996 2024-04-16 18:34:52.000000 django_tailwindcss_automated-0.6/README.md
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/django_tailwindcss_automated/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated/__init__.py
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated/main.py
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1243 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/SOURCES.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/dependency_links.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/entry_points.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/top_level.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/setup.cfg
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      620 2024-04-16 18:39:33.000000 django_tailwindcss_automated-0.6/setup.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1227 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      980 2024-04-16 19:54:24.000000 django_tailwindcss_automated-0.7/README.md
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 19:57:49.420735 django_tailwindcss_automated-0.7/django_tailwindcss_automated/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated/__init__.py
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated/main.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1227 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/SOURCES.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/dependency_links.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       64 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/entry_points.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/top_level.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/setup.cfg
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      604 2024-04-16 19:54:18.000000 django_tailwindcss_automated-0.7/setup.py
```

### Comparing `django_tailwindcss_automated-0.6/PKG-INFO` & `django_tailwindcss_automated-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tailwindcss_automated
-Version: 0.6
+Version: 0.7
 Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -29,15 +29,15 @@
 pip install django_tailwindcss_automated
 ```
 
 ## Run the Script
 
 In your terminal, run the following script to automate the setup:
 ```bash
-automate-django-tailwind
+automate
 ```
 
 ## Start the Development Server
 
 Open another terminal and navigate to the 'project_name' directory within your project folder:
 ```bash
 cd app
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.6 Summary:
+Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.7 Summary:
 Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
 Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
 markdown Automated Project Initialization ððð --- An automated setup
 for Django project with Tailwind. Handles all setup and configuration
 automatically.â¨
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
 Node.js, Git, and Python installed on your computer. - Create a folder for your
 Django project. ## Install the Package Open your terminal and install the
 package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
 the Script In your terminal, run the following script to automate the setup:
-```bash automate-django-tailwind ``` ## Start the Development Server Open
-another terminal and navigate to the 'project_name' directory within your
-project folder: ```bash cd app ``` ## Then start the development server ```bash
-python manage.py runserver ``` ![Alt Text](img.png) ## Happy Coding!!
+```bash automate ``` ## Start the Development Server Open another terminal and
+navigate to the 'project_name' directory within your project folder: ```bash cd
+app ``` ## Then start the development server ```bash python manage.py runserver
+``` ![Alt Text](img.png) ## Happy Coding!!
```

### Comparing `django_tailwindcss_automated-0.6/README.md` & `django_tailwindcss_automated-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 pip install django_tailwindcss_automated
 ```
 
 ## Run the Script
 
 In your terminal, run the following script to automate the setup:
 ```bash
-automate-django-tailwind
+automate
 ```
 
 ## Start the Development Server
 
 Open another terminal and navigate to the 'project_name' directory within your project folder:
 ```bash
 cd app
```

#### html2text {}

```diff
@@ -2,11 +2,11 @@
 project with Tailwind. Handles all setup and configuration automatically.â¨
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
 Node.js, Git, and Python installed on your computer. - Create a folder for your
 Django project. ## Install the Package Open your terminal and install the
 package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
 the Script In your terminal, run the following script to automate the setup:
-```bash automate-django-tailwind ``` ## Start the Development Server Open
-another terminal and navigate to the 'project_name' directory within your
-project folder: ```bash cd app ``` ## Then start the development server ```bash
-python manage.py runserver ``` ![Alt Text](img.png) ## Happy Coding!!
+```bash automate ``` ## Start the Development Server Open another terminal and
+navigate to the 'project_name' directory within your project folder: ```bash cd
+app ``` ## Then start the development server ```bash python manage.py runserver
+``` ![Alt Text](img.png) ## Happy Coding!!
```

### Comparing `django_tailwindcss_automated-0.6/django_tailwindcss_automated/main.py` & `django_tailwindcss_automated-0.7/django_tailwindcss_automated/main.py`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/PKG-INFO` & `django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwindcss-automated
-Version: 0.6
+Version: 0.7
 Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -29,15 +29,15 @@
 pip install django_tailwindcss_automated
 ```
 
 ## Run the Script
 
 In your terminal, run the following script to automate the setup:
 ```bash
-automate-django-tailwind
+automate
 ```
 
 ## Start the Development Server
 
 Open another terminal and navigate to the 'project_name' directory within your project folder:
 ```bash
 cd app
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.6 Summary:
+Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.7 Summary:
 Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
 Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
 markdown Automated Project Initialization ððð --- An automated setup
 for Django project with Tailwind. Handles all setup and configuration
 automatically.â¨
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
 Node.js, Git, and Python installed on your computer. - Create a folder for your
 Django project. ## Install the Package Open your terminal and install the
 package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
 the Script In your terminal, run the following script to automate the setup:
-```bash automate-django-tailwind ``` ## Start the Development Server Open
-another terminal and navigate to the 'project_name' directory within your
-project folder: ```bash cd app ``` ## Then start the development server ```bash
-python manage.py runserver ``` ![Alt Text](img.png) ## Happy Coding!!
+```bash automate ``` ## Start the Development Server Open another terminal and
+navigate to the 'project_name' directory within your project folder: ```bash cd
+app ``` ## Then start the development server ```bash python manage.py runserver
+``` ![Alt Text](img.png) ## Happy Coding!!
```

### Comparing `django_tailwindcss_automated-0.6/setup.py` & `django_tailwindcss_automated-0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='django_tailwindcss_automated',
     description="Handles all setup and configuration automatically.",
-    version='0.6',
+    version='0.7',
     author='Jan Leander',
     packages=find_packages(),
     install_requires=[
         # add dependencies here.
         # e.g 'num>=1.11.1'
     ],
     entry_points={
         "console_scripts": [
-            "automate-django-tailwind = django_tailwindcss_automated:main",
+            "automate = django_tailwindcss_automated:main",
         ],
     },
     long_description=description,
     long_description_content_type="text/markdown",
 )
```

