# Comparing `tmp/vs-colabi-1.1.5.tar.gz` & `tmp/vs-colabi-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vs-colabi-1.1.5.tar", last modified: Sun Apr 14 06:43:00 2024, max compression
+gzip compressed data, was "vs-colabi-1.1.6.tar", last modified: Tue Apr 16 04:48:27 2024, max compression
```

## Comparing `vs-colabi-1.1.5.tar` & `vs-colabi-1.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 06:43:00.354414 vs-colabi-1.1.5/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-14 06:43:00.354414 vs-colabi-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-14 06:42:51.000000 vs-colabi-1.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 06:43:00.354414 vs-colabi-1.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-14 06:42:51.000000 vs-colabi-1.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 06:43:00.354414 vs-colabi-1.1.5/vs_colabi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-14 06:43:00.000000 vs-colabi-1.1.5/vs_colabi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2024-04-14 06:43:00.000000 vs-colabi-1.1.5/vs_colabi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 06:43:00.000000 vs-colabi-1.1.5/vs_colabi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 06:43:00.000000 vs-colabi-1.1.5/vs_colabi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-14 06:43:00.000000 vs-colabi-1.1.5/vs_colabi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 06:43:00.353414 vs-colabi-1.1.5/vscolabi/
--rw-rw-rw-   0 root         (0) root         (0)     3422 2024-04-14 06:42:51.000000 vs-colabi-1.1.5/vscolabi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:48:27.478948 vs-colabi-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-16 04:48:27.478948 vs-colabi-1.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-16 04:48:18.000000 vs-colabi-1.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 04:48:27.478948 vs-colabi-1.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-16 04:48:18.000000 vs-colabi-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:48:27.478948 vs-colabi-1.1.6/vs_colabi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-16 04:48:27.000000 vs-colabi-1.1.6/vs_colabi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2024-04-16 04:48:27.000000 vs-colabi-1.1.6/vs_colabi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 04:48:27.000000 vs-colabi-1.1.6/vs_colabi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 04:48:27.000000 vs-colabi-1.1.6/vs_colabi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-16 04:48:27.000000 vs-colabi-1.1.6/vs_colabi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 04:48:27.477948 vs-colabi-1.1.6/vscolabi/
+-rw-rw-rw-   0 root         (0) root         (0)     3427 2024-04-16 04:48:18.000000 vs-colabi-1.1.6/vscolabi/__init__.py
```

### Comparing `vs-colabi-1.1.5/PKG-INFO` & `vs-colabi-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vs-colabi
-Version: 1.1.5
+Version: 1.1.6
 Summary: Run vs code tunnel inside colab notebook
 Home-page: https://gitlab.com/isampypi/vs-colabi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vs-colabi-1.1.5/README.md` & `vs-colabi-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vs-colabi-1.1.5/setup.py` & `vs-colabi-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `vs-colabi-1.1.5/vs_colabi.egg-info/PKG-INFO` & `vs-colabi-1.1.6/vs_colabi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vs-colabi
-Version: 1.1.5
+Version: 1.1.6
 Summary: Run vs code tunnel inside colab notebook
 Home-page: https://gitlab.com/isampypi/vs-colabi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vs-colabi-1.1.5/vscolabi/__init__.py` & `vs-colabi-1.1.6/vscolabi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def configure(clear = True, mount = False  , tab = False ,folder = "/content" ) : 
     if clear : clear_output()
     if mount : drive.mount('/content/drive')
     singletab = "" if tab else ",'width=500,height=400,scrollbars=yes'"
     html_code = """
     <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>Section with Button</title> <style> body {{margin: 0; padding: 0; font-family: Arial, sans-serif; }} .section {{background-color: #fff; padding: 50px; text-align: center; }} .button {{display: inline-block; padding: 20px 40px; /* Adjust padding to make the button bigger */ font-size: 25px; /* Increase font size */ background-color: #007bff; color: #fff; border: none; border-radius: 5px; cursor: pointer; width: 80%; font-weight: 400; letter-spacing: 2px ; }} </style> </head> <body> <section class="section"> <button onclick="navigator.clipboard.writeText('{code_to_authenticate}').then(function() {{window.open('https://microsoft.com/devicelogin', '_blank', 'width=500,height=400,scrollbars=yes');}} );" class = "button">Open https://microsoft.com/devicelogin and Paste code </button> </section> </body> </html>    """
-    openpath = urljoin("https://vscode.dev/tunnel/colab",os.abspath(folder))
+    openpath = urljoin("https://vscode.dev/tunnel/colab",os.path.abspath(folder))
     vs_code_btn  = """
       <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>Section with Button</title> <style> body {{ margin: 0; padding: 0; font-family: Arial, sans-serif; }} .section {{background-color: #fff; padding: 50px; text-align: center; }} .button {{display: inline-block; padding: 20px 40px; /* Adjust padding to make the button bigger */ font-size: 25px; /* Increase font size */ background-color: #007bff; color: #fff; border: none; border-radius: 5px; cursor: pointer; width: 80%; font-weight: 400; letter-spacing: 2px ; }} </style> </head> <body> <section class="section"> <button onclick="window.open('{openpath}', '_blank' {singletab});" class = "button" >Open vs-code .</button> </section> </body> </html>    
     """.format(openpath = openpath, singletab = singletab )
     if not os.path.exists("./code") : 
         assert b.bash('''
         curl -Lk 'https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64' --output vscode_cli.tar.gz && tar -xf vscode_cli.tar.gz && rm vscode_cli.tar.gz
         ''').ok
```

