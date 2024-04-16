# Comparing `tmp/danila-lib-1.0.3.tar.gz` & `tmp/danila-lib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.0.3.tar", last modified: Mon Apr 15 17:16:02 2024, max compression
+gzip compressed data, was "danila-lib-1.0.4.tar", last modified: Mon Apr 15 17:25:42 2024, max compression
```

## Comparing `danila-lib-1.0.3.tar` & `danila-lib-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.756641 danila-lib-1.0.3/
--rw-rw-rw-   0        0        0     4169 2024-04-15 17:16:02.756641 danila-lib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.748677 danila-lib-1.0.3/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.3/danila/__init__.py
--rw-rw-rw-   0        0        0      404 2024-04-15 17:16:00.000000 danila-lib-1.0.3/danila/danila.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.753654 danila-lib-1.0.3/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1881 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 17:16:02.000000 danila-lib-1.0.3/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.753654 danila-lib-1.0.3/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.754649 danila-lib-1.0.3/data/neuro/
--rw-rw-rw-   0        0        0     3830 2024-04-15 17:05:00.000000 danila-lib-1.0.3/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.3/data/neuro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:16:02.755645 danila-lib-1.0.3/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.3/data/result/Class_im.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.3/data/result/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-15 17:16:02.757636 danila-lib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-15 17:09:18.000000 danila-lib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.576403 danila-lib-1.0.4/
+-rw-rw-rw-   0        0        0     4169 2024-04-15 17:25:42.575407 danila-lib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.553505 danila-lib-1.0.4/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.4/danila/__init__.py
+-rw-rw-rw-   0        0        0      402 2024-04-15 17:25:24.000000 danila-lib-1.0.4/danila/danila.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.571425 danila-lib-1.0.4/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1881 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 17:25:42.000000 danila-lib-1.0.4/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.571425 danila-lib-1.0.4/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.4/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.572420 danila-lib-1.0.4/data/neuro/
+-rw-rw-rw-   0        0        0     3808 2024-04-15 17:24:43.000000 danila-lib-1.0.4/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.4/data/neuro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:25:42.573416 danila-lib-1.0.4/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.4/data/result/Class_im.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.4/data/result/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:25:42.580385 danila-lib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-15 17:25:35.000000 danila-lib-1.0.4/setup.py
```

### Comparing `danila-lib-1.0.3/PKG-INFO` & `danila-lib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.0.3/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.0.4/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.0.3/danila_lib.egg-info/requires.txt` & `danila-lib-1.0.4/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.0.3/data/neuro/Rama_classify_class.py` & `danila-lib-1.0.4/data/neuro/Rama_classify_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         response = requests.get(final_url)
         download_url = response.json()['href']
 
         # Загружаем файл и сохраняем его
         download_response = requests.get(download_url)
         # print(download_response.content)
 
-        with open('data/neuro/17_model.zip', 'wb') as f:
+        with open('17_model.zip', 'wb') as f:
             f.write(download_response.content)
 
-        with zipfile.ZipFile('data/neuro/17_model.zip', 'r') as zip_ref:
+        with zipfile.ZipFile('17_model.zip', 'r') as zip_ref:
             zip_ref.extractall()
         self.rama_classify_model = keras.models.load_model('17_model')
     # сделать картинку чб 512-512
     def prepare_img(self, image_initial):
         img_grey = cv2.cvtColor(image_initial, cv2.COLOR_BGR2GRAY)
         img_grey_size = cv2.resize(img_grey, (512, 512))
         data = np.array(img_grey_size, dtype="float") / 255.0
```

### Comparing `danila-lib-1.0.3/setup.py` & `danila-lib-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.0.3',
+  version='1.0.4',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

