# Comparing `tmp/python-sscma-0.5.0.tar.gz` & `tmp/python-sscma-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscma-0.5.0.tar", last modified: Tue Apr 16 07:00:47 2024, max compression
+gzip compressed data, was "python-sscma-0.5.1.tar", last modified: Tue Apr 16 08:12:26 2024, max compression
```

## Comparing `python-sscma-0.5.0.tar` & `python-sscma-0.5.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.044881 python-sscma-0.5.0/
--rw-rw-rw-   0        0        0     2914 2024-04-16 07:00:47.044881 python-sscma-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2396 2024-04-16 06:53:08.000000 python-sscma-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.014584 python-sscma-0.5.0/python_sscma.egg-info/
--rw-rw-rw-   0        0        0     2914 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 07:00:46.000000 python-sscma-0.5.0/python_sscma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 07:00:47.044881 python-sscma-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1148 2024-04-16 06:56:43.000000 python-sscma-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.015585 python-sscma-0.5.0/sscma/
--rw-rw-rw-   0        0        0       42 2024-04-16 06:59:44.000000 python-sscma-0.5.0/sscma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.019587 python-sscma-0.5.0/sscma/cli/
--rw-rw-rw-   0        0        0        0 2024-04-16 06:11:20.000000 python-sscma-0.5.0/sscma/cli/__init__.py
--rw-rw-rw-   0        0        0      253 2024-04-16 06:30:55.000000 python-sscma-0.5.0/sscma/cli/cli.py
--rw-rw-rw-   0        0        0     4773 2024-04-16 06:49:24.000000 python-sscma-0.5.0/sscma/cli/client.py
--rw-rw-rw-   0        0        0     2367 2024-04-16 06:12:54.000000 python-sscma-0.5.0/sscma/cli/flahser.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.023586 python-sscma-0.5.0/sscma/flashers/
--rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.0/sscma/flashers/__init__.py
--rw-rw-rw-   0        0        0      768 2024-04-16 06:01:44.000000 python-sscma-0.5.0/sscma/flashers/base.py
--rw-rw-rw-   0        0        0     5161 2024-04-16 06:09:27.000000 python-sscma-0.5.0/sscma/flashers/core.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.025586 python-sscma-0.5.0/sscma/fonts/
--rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/fonts/Arial.ttf
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.033878 python-sscma-0.5.0/sscma/micro/
--rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/__init__.py
--rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/client.py
--rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/const.py
--rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.0/sscma/micro/device.py
--rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/exceptions.py
--rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.0/sscma/micro/info.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.036879 python-sscma-0.5.0/sscma/utils/
--rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.0/sscma/utils/__init__.py
--rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.0/sscma/utils/image.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:00:47.043877 python-sscma-0.5.0/tests/
--rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_mqtt.py
--rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_mqttclient.py
--rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_serial.py
--rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.0/tests/test_serialclient.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.447260 python-sscma-0.5.1/
+-rw-rw-rw-   0        0        0     2914 2024-04-16 08:12:26.446323 python-sscma-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2396 2024-04-16 08:12:13.000000 python-sscma-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.419643 python-sscma-0.5.1/python_sscma.egg-info/
+-rw-rw-rw-   0        0        0     2914 2024-04-16 08:12:26.000000 python-sscma-0.5.1/python_sscma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2024-04-16 08:12:26.000000 python-sscma-0.5.1/python_sscma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:12:26.000000 python-sscma-0.5.1/python_sscma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-16 08:12:26.000000 python-sscma-0.5.1/python_sscma.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-16 08:12:26.000000 python-sscma-0.5.1/python_sscma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 08:12:26.000000 python-sscma-0.5.1/python_sscma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:12:26.447260 python-sscma-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1270 2024-04-16 08:12:13.000000 python-sscma-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.420655 python-sscma-0.5.1/sscma/
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:12:13.000000 python-sscma-0.5.1/sscma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.425307 python-sscma-0.5.1/sscma/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-16 06:11:20.000000 python-sscma-0.5.1/sscma/cli/__init__.py
+-rw-rw-rw-   0        0        0      253 2024-04-16 06:30:55.000000 python-sscma-0.5.1/sscma/cli/cli.py
+-rw-rw-rw-   0        0        0     4773 2024-04-16 06:49:24.000000 python-sscma-0.5.1/sscma/cli/client.py
+-rw-rw-rw-   0        0        0     2367 2024-04-16 06:12:54.000000 python-sscma-0.5.1/sscma/cli/flahser.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.428319 python-sscma-0.5.1/sscma/flashers/
+-rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.1/sscma/flashers/__init__.py
+-rw-rw-rw-   0        0        0      768 2024-04-16 06:01:44.000000 python-sscma-0.5.1/sscma/flashers/base.py
+-rw-rw-rw-   0        0        0     5161 2024-04-16 06:09:27.000000 python-sscma-0.5.1/sscma/flashers/core.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.429319 python-sscma-0.5.1/sscma/fonts/
+-rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.1/sscma/fonts/Arial.ttf
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.437319 python-sscma-0.5.1/sscma/micro/
+-rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.1/sscma/micro/__init__.py
+-rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.1/sscma/micro/client.py
+-rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.1/sscma/micro/const.py
+-rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.1/sscma/micro/device.py
+-rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.1/sscma/micro/exceptions.py
+-rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.1/sscma/micro/info.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.439321 python-sscma-0.5.1/sscma/utils/
+-rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.1/sscma/utils/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.1/sscma/utils/image.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:12:26.445324 python-sscma-0.5.1/tests/
+-rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.1/tests/test_mqtt.py
+-rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.1/tests/test_mqttclient.py
+-rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.1/tests/test_serial.py
+-rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.1/tests/test_serialclient.py
```

### Comparing `python-sscma-0.5.0/PKG-INFO` & `python-sscma-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sscma
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python library for sscma
 Home-page: https://github.com/Seeed-Studio/python-sscma
 Author: Seeed Studio
 Author-email: lht856@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-sscma-0.5.0/README.md` & `python-sscma-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/python_sscma.egg-info/PKG-INFO` & `python-sscma-0.5.1/python_sscma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sscma
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python library for sscma
 Home-page: https://github.com/Seeed-Studio/python-sscma
 Author: Seeed Studio
 Author-email: lht856@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-sscma-0.5.0/python_sscma.egg-info/SOURCES.txt` & `python-sscma-0.5.1/python_sscma.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 python_sscma.egg-info/PKG-INFO
 python_sscma.egg-info/SOURCES.txt
 python_sscma.egg-info/dependency_links.txt
 python_sscma.egg-info/entry_points.txt
+python_sscma.egg-info/requires.txt
 python_sscma.egg-info/top_level.txt
 sscma/__init__.py
 sscma/cli/__init__.py
 sscma/cli/cli.py
 sscma/cli/client.py
 sscma/cli/flahser.py
 sscma/flashers/__init__.py
```

### Comparing `python-sscma-0.5.0/setup.py` & `python-sscma-0.5.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 
 with open("./sscma/__init__.py", 'r') as f:
     content = f.read()
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
+    
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+    
+print(requirements)
 
 setuptools.setup(
     name='python-sscma',
     version=version,
     author='Seeed Studio',
     author_email='lht856@foxmail.com',
     description='Python library for sscma',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Seeed-Studio/python-sscma',
     packages=find_packages(),
     package_data={'sscma': ['fonts/*.ttf']},
-    install_requires=[],
+    install_requires=requirements,
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
```

### Comparing `python-sscma-0.5.0/sscma/cli/client.py` & `python-sscma-0.5.1/sscma/cli/client.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/cli/flahser.py` & `python-sscma-0.5.1/sscma/cli/flahser.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/flashers/base.py` & `python-sscma-0.5.1/sscma/flashers/base.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/flashers/core.py` & `python-sscma-0.5.1/sscma/flashers/core.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/fonts/Arial.ttf` & `python-sscma-0.5.1/sscma/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/micro/client.py` & `python-sscma-0.5.1/sscma/micro/client.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/micro/const.py` & `python-sscma-0.5.1/sscma/micro/const.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/micro/device.py` & `python-sscma-0.5.1/sscma/micro/device.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/micro/exceptions.py` & `python-sscma-0.5.1/sscma/micro/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/micro/info.py` & `python-sscma-0.5.1/sscma/micro/info.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/sscma/utils/image.py` & `python-sscma-0.5.1/sscma/utils/image.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/tests/test_mqtt.py` & `python-sscma-0.5.1/tests/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/tests/test_mqttclient.py` & `python-sscma-0.5.1/tests/test_mqttclient.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/tests/test_serial.py` & `python-sscma-0.5.1/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.0/tests/test_serialclient.py` & `python-sscma-0.5.1/tests/test_serialclient.py`

 * *Files identical despite different names*

