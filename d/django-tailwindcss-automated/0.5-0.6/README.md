# Comparing `tmp/django_tailwindcss_automated-0.5.tar.gz` & `tmp/django_tailwindcss_automated-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwindcss_automated-0.5.tar", last modified: Tue Apr 16 18:33:48 2024, max compression
+gzip compressed data, was "django_tailwindcss_automated-0.6.tar", last modified: Tue Apr 16 18:39:37 2024, max compression
```

## Comparing `django_tailwindcss_automated-0.5.tar` & `django_tailwindcss_automated-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:33:48.626666 django_tailwindcss_automated-0.5/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1225 2024-04-16 18:33:48.626666 django_tailwindcss_automated-0.5/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1021 2024-04-16 18:33:19.000000 django_tailwindcss_automated-0.5/README.md
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:33:48.622666 django_tailwindcss_automated-0.5/django_tailwindcss_automated/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated/__init__.py
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated/main.py
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:33:48.622666 django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1225 2024-04-16 18:33:48.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 18:33:48.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/SOURCES.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 18:33:48.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/dependency_links.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 18:33:48.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/entry_points.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 18:33:48.000000 django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/top_level.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 18:33:48.626666 django_tailwindcss_automated-0.5/setup.cfg
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      550 2024-04-16 18:33:41.000000 django_tailwindcss_automated-0.5/setup.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1243 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      996 2024-04-16 18:34:52.000000 django_tailwindcss_automated-0.6/README.md
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/django_tailwindcss_automated/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated/__init__.py
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated/main.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1243 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/SOURCES.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/dependency_links.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/entry_points.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 18:39:36.000000 django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/top_level.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 18:39:37.245013 django_tailwindcss_automated-0.6/setup.cfg
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      620 2024-04-16 18:39:33.000000 django_tailwindcss_automated-0.6/setup.py
```

### Comparing `django_tailwindcss_automated-0.5/PKG-INFO` & `django_tailwindcss_automated-0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-Metadata-Version: 2.1
-Name: django_tailwindcss_automated
-Version: 0.5
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: Jan Leander
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 Automated Project Initialization 🐍💚💙 
 ---
 An automated setup for Django project with Tailwind. Handles all setup and configuration automatically.✨
 
 <p align="left">
   <a href="https://skillicons.dev">
     <img src="https://skillicons.dev/icons?i=django,tailwindcss,python" />
   </a>
 </p>
 
 ## Getting Started 💙
 - 👀 Before you dive in, make sure that you have Node.js, Git, and Python installed on your computer.
-- Create a Project Folder: Create a folder for your Django project.
+- Create a folder for your Django project.
 
 ## Install the Package 
 
 Open your terminal and install the package using pip:
 ```bash
 pip install django_tailwindcss_automated
 ```
@@ -50,9 +40,7 @@
 python manage.py runserver
 ```
 
 ![Alt Text](img.png)
 
 
 ## Happy Coding!!
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,12 @@
-Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.5 Summary:
-UNKNOWN Home-page: UNKNOWN Author: Jan Leander License: UNKNOWN Platform:
-UNKNOWN Description-Content-Type: text/markdown Automated Project
-Initialization ððð --- An automated setup for Django project with
-Tailwind. Handles all setup and configuration automatically.â¨
+Automated Project Initialization ððð --- An automated setup for Django
+project with Tailwind. Handles all setup and configuration automatically.â¨
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
-Node.js, Git, and Python installed on your computer. - Create a Project Folder:
-Create a folder for your Django project. ## Install the Package Open your
-terminal and install the package using pip: ```bash pip install
-django_tailwindcss_automated ``` ## Run the Script In your terminal, run the
-following script to automate the setup: ```bash automate-django-tailwind ``` ##
-Start the Development Server Open another terminal and navigate to the
-'project_name' directory within your project folder: ```bash cd app ``` ## Then
-start the development server ```bash python manage.py runserver ``` ![Alt Text]
-(img.png) ## Happy Coding!!
+Node.js, Git, and Python installed on your computer. - Create a folder for your
+Django project. ## Install the Package Open your terminal and install the
+package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
+the Script In your terminal, run the following script to automate the setup:
+```bash automate-django-tailwind ``` ## Start the Development Server Open
+another terminal and navigate to the 'project_name' directory within your
+project folder: ```bash cd app ``` ## Then start the development server ```bash
+python manage.py runserver ``` ![Alt Text](img.png) ## Happy Coding!!
```

### Comparing `django_tailwindcss_automated-0.5/django_tailwindcss_automated/main.py` & `django_tailwindcss_automated-0.6/django_tailwindcss_automated/main.py`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.5/django_tailwindcss_automated.egg-info/PKG-INFO` & `django_tailwindcss_automated-0.6/django_tailwindcss_automated.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-tailwindcss-automated
-Version: 0.5
-Summary: UNKNOWN
+Version: 0.6
+Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Automated Project Initialization 🐍💚💙 
@@ -16,15 +16,15 @@
   <a href="https://skillicons.dev">
     <img src="https://skillicons.dev/icons?i=django,tailwindcss,python" />
   </a>
 </p>
 
 ## Getting Started 💙
 - 👀 Before you dive in, make sure that you have Node.js, Git, and Python installed on your computer.
-- Create a Project Folder: Create a folder for your Django project.
+- Create a folder for your Django project.
 
 ## Install the Package 
 
 Open your terminal and install the package using pip:
 ```bash
 pip install django_tailwindcss_automated
 ```
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.5 Summary:
-UNKNOWN Home-page: UNKNOWN Author: Jan Leander License: UNKNOWN Platform:
-UNKNOWN Description-Content-Type: text/markdown Automated Project
-Initialization ððð --- An automated setup for Django project with
-Tailwind. Handles all setup and configuration automatically.â¨
+Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.6 Summary:
+Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
+Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
+markdown Automated Project Initialization ððð --- An automated setup
+for Django project with Tailwind. Handles all setup and configuration
+automatically.â¨
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
-Node.js, Git, and Python installed on your computer. - Create a Project Folder:
-Create a folder for your Django project. ## Install the Package Open your
-terminal and install the package using pip: ```bash pip install
-django_tailwindcss_automated ``` ## Run the Script In your terminal, run the
-following script to automate the setup: ```bash automate-django-tailwind ``` ##
-Start the Development Server Open another terminal and navigate to the
-'project_name' directory within your project folder: ```bash cd app ``` ## Then
-start the development server ```bash python manage.py runserver ``` ![Alt Text]
-(img.png) ## Happy Coding!!
+Node.js, Git, and Python installed on your computer. - Create a folder for your
+Django project. ## Install the Package Open your terminal and install the
+package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
+the Script In your terminal, run the following script to automate the setup:
+```bash automate-django-tailwind ``` ## Start the Development Server Open
+another terminal and navigate to the 'project_name' directory within your
+project folder: ```bash cd app ``` ## Then start the development server ```bash
+python manage.py runserver ``` ![Alt Text](img.png) ## Happy Coding!!
```

### Comparing `django_tailwindcss_automated-0.5/setup.py` & `django_tailwindcss_automated-0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='django_tailwindcss_automated',
-    version='0.5',
+    description="Handles all setup and configuration automatically.",
+    version='0.6',
     author='Jan Leander',
     packages=find_packages(),
     install_requires=[
         # add dependencies here.
         # e.g 'num>=1.11.1'
     ],
     entry_points={
```

