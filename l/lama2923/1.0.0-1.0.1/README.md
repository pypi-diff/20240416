# Comparing `tmp/lama2923-1.0.0.tar.gz` & `tmp/lama2923-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.0.0.tar", last modified: Sun Apr 14 02:17:50 2024, max compression
+gzip compressed data, was "lama2923-1.0.1.tar", last modified: Tue Apr 16 14:25:54 2024, max compression
```

## Comparing `lama2923-1.0.0.tar` & `lama2923-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 02:17:50.045637 lama2923-1.0.0/
--rw-rw-rw-   0        0        0      956 2024-04-14 02:17:50.044135 lama2923-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 02:17:50.026034 lama2923-1.0.0/lama2923/
--rw-rw-rw-   0        0        0    26157 2024-04-14 02:17:30.000000 lama2923-1.0.0/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 02:17:50.041133 lama2923-1.0.0/lama2923.egg-info/
--rw-rw-rw-   0        0        0      956 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 02:17:50.045637 lama2923-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1294 2024-04-14 02:17:22.000000 lama2923-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:25:54.122052 lama2923-1.0.1/
+-rw-rw-rw-   0        0        0      956 2024-04-16 14:25:54.120535 lama2923-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 14:25:54.080013 lama2923-1.0.1/lama2923/
+-rw-rw-rw-   0        0        0    26640 2024-04-16 14:25:41.000000 lama2923-1.0.1/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:25:54.097511 lama2923-1.0.1/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-04-16 14:25:53.000000 lama2923-1.0.1/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-16 14:25:53.000000 lama2923-1.0.1/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 14:25:53.000000 lama2923-1.0.1/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 14:25:53.000000 lama2923-1.0.1/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 14:25:53.000000 lama2923-1.0.1/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 14:25:54.122052 lama2923-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-04-16 14:25:22.000000 lama2923-1.0.1/setup.py
```

### Comparing `lama2923-1.0.0/PKG-INFO` & `lama2923-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.0/lama2923/__init__.py` & `lama2923-1.0.1/lama2923/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,28 +346,43 @@
             if INDEX % 3 == 0 and len(str(Numbers)) != INDEX:
                 
                 edited_Numbers += f"{number}."
             else:
                 edited_Numbers += number
         return edited_Numbers[::-1]
                 
-            
+class CustomDecodeError(Exception):
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)   
             
 def terskurallı_sayı(Numbers=0):
     if not isinstance(Numbers, str):
         raise TypeError("Değerin String olması zorunludur!")
     Numbers = str(Numbers).replace(".", "")
     Numbers = Numbers.replace(",", ".")
     return Numbers
 
+
+class _TokenIsNotWork(Exception):
+    pass
+
+
 class Discord:
     class User:
+        
         def __init__(self, token):
             self.token = str(token)
-            
+            response = requests.get('https://discord.com/api/v9/users/@me', headers={'Authorization': str(self.token)})
+            if response.status_code == 200:
+                pass
+            else:
+                raise _TokenIsNotWork('Token IS NOT WORK!')
+                
+                
         def send_message(self, Channel_id, Message, files=None):
             payload = {'content': str(Message)}
             headers = {'Authorization': str(self.token)}
             
             if files is not None and isinstance(files, list):
                 files_data = {}
                 for file_name in files:
```

### Comparing `lama2923-1.0.0/lama2923.egg-info/PKG-INFO` & `lama2923-1.0.1/lama2923.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.0/setup.py` & `lama2923-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.0.0',
+    version='1.0.1',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

