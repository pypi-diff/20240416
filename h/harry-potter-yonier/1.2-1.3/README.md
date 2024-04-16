# Comparing `tmp/harry_potter_yonier-1.2.tar.gz` & `tmp/harry_potter_yonier-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harry_potter_yonier-1.2.tar", last modified: Tue Apr 16 04:11:08 2024, max compression
+gzip compressed data, was "harry_potter_yonier-1.3.tar", last modified: Tue Apr 16 04:45:52 2024, max compression
```

## Comparing `harry_potter_yonier-1.2.tar` & `harry_potter_yonier-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:11:08.494230 harry_potter_yonier-1.2/
--rw-r--r--   0 neo       (1000) neo       (1000)     1061 2024-04-16 03:01:09.000000 harry_potter_yonier-1.2/LICENSE.txt
--rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:11:08.494230 harry_potter_yonier-1.2/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)       57 2024-04-16 00:38:48.000000 harry_potter_yonier-1.2/README.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:11:08.493230 harry_potter_yonier-1.2/harry_potter_yonier/
--rw-r--r--   0 neo       (1000) neo       (1000)      115 2024-04-16 03:58:52.000000 harry_potter_yonier-1.2/harry_potter_yonier/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)      818 2024-04-16 03:59:41.000000 harry_potter_yonier-1.2/harry_potter_yonier/__main__.py
--rw-r--r--   0 neo       (1000) neo       (1000)      657 2024-04-16 03:58:30.000000 harry_potter_yonier-1.2/harry_potter_yonier/get_one_person.py
--rw-r--r--   0 neo       (1000) neo       (1000)      508 2024-04-16 03:58:17.000000 harry_potter_yonier-1.2/harry_potter_yonier/get_person.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:11:08.493230 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/
--rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:11:08.000000 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)      426 2024-04-16 04:11:08.000000 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/SOURCES.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        1 2024-04-16 04:11:08.000000 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/dependency_links.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       61 2024-04-16 04:11:08.000000 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/entry_points.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        9 2024-04-16 04:11:08.000000 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/requires.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       20 2024-04-16 04:11:08.000000 harry_potter_yonier-1.2/harry_potter_yonier.egg-info/top_level.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2024-04-16 04:11:08.494230 harry_potter_yonier-1.2/setup.cfg
--rw-r--r--   0 neo       (1000) neo       (1000)     1198 2024-04-16 04:10:44.000000 harry_potter_yonier-1.2/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1061 2024-04-16 03:01:09.000000 harry_potter_yonier-1.3/LICENSE.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)       57 2024-04-16 00:38:48.000000 harry_potter_yonier-1.3/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:45:52.390138 harry_potter_yonier-1.3/harry_potter_yonier/
+-rw-r--r--   0 neo       (1000) neo       (1000)      115 2024-04-16 03:58:52.000000 harry_potter_yonier-1.3/harry_potter_yonier/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      936 2024-04-16 04:29:20.000000 harry_potter_yonier-1.3/harry_potter_yonier/__main__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      885 2024-04-16 04:45:05.000000 harry_potter_yonier-1.3/harry_potter_yonier/get_one_person.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      508 2024-04-16 03:58:17.000000 harry_potter_yonier-1.3/harry_potter_yonier/get_person.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      426 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       62 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/entry_points.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        9 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       20 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)     1199 2024-04-16 04:28:30.000000 harry_potter_yonier-1.3/setup.py
```

### Comparing `harry_potter_yonier-1.2/LICENSE.txt` & `harry_potter_yonier-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `harry_potter_yonier-1.2/PKG-INFO` & `harry_potter_yonier-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harry_potter_yonier
-Version: 1.2
+Version: 1.3
 Summary: Permite consumir el API de Harry Potter para obtener o listar personajes
 Home-page: https://github.com/YonierGomez/harrypotter_python
 Author: Yonier Asprilla
 Author-email: yoonier13@gmail.com
 License: MIT
 Keywords: harrypotter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `harry_potter_yonier-1.2/harry_potter_yonier/__main__.py` & `harry_potter_yonier-1.3/harry_potter_yonier/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import logging
 from harry_potter_yonier import get_one_person, get_person
 
 if __name__ == "__main__":
-    while True:
-        # Mostrar las opciones disponibles
-        print("1. Buscar personaje")
-        print("2. Listar personajes")
-        print("3. Salir")
-        
-        # Capturar la elección del usuario
-        choose = input("Ingrese el número de la opción que desea: ")
-        
-        if choose == "1":
-            get_one_person()
-            break  # Salir del bucle while
-        elif choose == "2":
-            get_person()
-            break  # Salir del bucle while
-        elif choose == "3":
-            logging.warning("Saliendo del programa...")
-            break  # Salir del bucle while
-        else:
-            logging.warning("Opción inválida. Por favor, elija una opción válida.")
+    
+    def call_me():
+        while True:
+            # Mostrar las opciones disponibles
+            print("1. Buscar personaje")
+            print("2. Listar personajes")
+            print("3. Salir")
+            
+            # Capturar la elección del usuario
+            choose = input("Ingrese el número de la opción que desea: ")
+            
+            if choose == "1":
+                get_one_person()
+                break  # Salir del bucle while
+            elif choose == "2":
+                get_person()
+                break  # Salir del bucle while
+            elif choose == "3":
+                logging.warning("Saliendo del programa...")
+                break  # Salir del bucle while
+            else:
+                logging.warning("Opción inválida. Por favor, elija una opción válida.")
+
+    call_me()
```

### Comparing `harry_potter_yonier-1.2/harry_potter_yonier.egg-info/PKG-INFO` & `harry_potter_yonier-1.3/harry_potter_yonier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harry_potter_yonier
-Version: 1.2
+Version: 1.3
 Summary: Permite consumir el API de Harry Potter para obtener o listar personajes
 Home-page: https://github.com/YonierGomez/harrypotter_python
 Author: Yonier Asprilla
 Author-email: yoonier13@gmail.com
 License: MIT
 Keywords: harrypotter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `harry_potter_yonier-1.2/setup.py` & `harry_potter_yonier-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pathlib import Path # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = 'v1.2'
+VERSION = 'v1.3'
 DESCRIPTION = 'Permite consumir el API de Harry Potter para obtener o listar personajes'
 PACKAGE_NAME = 'harry_potter_yonier'
 AUTHOR = 'Yonier Asprilla'
 EMAIL = 'yoonier13@gmail.com'
 GITHUB_URL = 'https://github.com/YonierGomez/harrypotter_python'
 
 setup(
     name = PACKAGE_NAME,
     packages = [PACKAGE_NAME],
     entry_points={
         "console_scripts":
-            ["pycody=harry_potter_yonier.__main__:main"]
+            ["yonierpotter=harry_potter_yonier.__main__"]
     },
     version = VERSION,
     license='MIT',
     description = DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     author = AUTHOR,
```

