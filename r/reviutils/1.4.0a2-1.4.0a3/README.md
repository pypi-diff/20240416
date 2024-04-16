# Comparing `tmp/reviutils-1.4.0a2.tar.gz` & `tmp/reviutils-1.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviutils-1.4.0a2.tar", last modified: Tue Apr 16 08:08:38 2024, max compression
+gzip compressed data, was "reviutils-1.4.0a3.tar", last modified: Tue Apr 16 08:14:55 2024, max compression
```

## Comparing `reviutils-1.4.0a2.tar` & `reviutils-1.4.0a3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.704021 reviutils-1.4.0a2/
--rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0a2/LICENSE
--rw-rw-rw-   0        0        0     2872 2024-04-16 08:08:38.704021 reviutils-1.4.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.4.0a2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.669766 reviutils-1.4.0a2/reviutils/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.684020 reviutils-1.4.0a2/reviutils/api/
--rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0a2/reviutils/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.687021 reviutils-1.4.0a2/reviutils/api/amap/
--rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0a2/reviutils/api/amap/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0a2/reviutils/api/amap/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.690022 reviutils-1.4.0a2/reviutils/audio/
--rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0a2/reviutils/audio/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0a2/reviutils/audio/clipper.py
--rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0a2/reviutils/audio/reader.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.691023 reviutils-1.4.0a2/reviutils/common/
--rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0a2/reviutils/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.695021 reviutils-1.4.0a2/reviutils/gis/
--rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0a2/reviutils/gis/__init__.py
--rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0a2/reviutils/gis/convertor.py
--rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0a2/reviutils/gis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.701021 reviutils-1.4.0a2/reviutils/noisepollution/
--rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0a2/reviutils/noisepollution/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0a2/reviutils/noisepollution/evaluation.py
--rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0a2/reviutils/noisepollution/funcarea.py
--rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0a2/reviutils/noisepollution/hourhelper.py
--rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0a2/reviutils/noisepollution/splhelper.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.702020 reviutils-1.4.0a2/reviutils/omap/
--rw-rw-rw-   0        0        0       55 2024-04-16 07:52:06.000000 reviutils-1.4.0a2/reviutils/omap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:08:38.683021 reviutils-1.4.0a2/reviutils.egg-info/
--rw-rw-rw-   0        0        0     2872 2024-04-16 08:08:38.000000 reviutils-1.4.0a2/reviutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      709 2024-04-16 08:08:38.000000 reviutils-1.4.0a2/reviutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:08:38.000000 reviutils-1.4.0a2/reviutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-11 08:53:25.000000 reviutils-1.4.0a2/reviutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2024-04-16 08:08:38.000000 reviutils-1.4.0a2/reviutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 08:08:38.000000 reviutils-1.4.0a2/reviutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 08:08:38.705020 reviutils-1.4.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1504 2024-04-16 08:08:34.000000 reviutils-1.4.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.335328 reviutils-1.4.0a3/
+-rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0a3/LICENSE
+-rw-rw-rw-   0        0        0     2872 2024-04-16 08:14:55.335328 reviutils-1.4.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.4.0a3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.299852 reviutils-1.4.0a3/reviutils/
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.313755 reviutils-1.4.0a3/reviutils/api/
+-rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0a3/reviutils/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.317323 reviutils-1.4.0a3/reviutils/api/amap/
+-rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0a3/reviutils/api/amap/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0a3/reviutils/api/amap/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.321328 reviutils-1.4.0a3/reviutils/audio/
+-rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0a3/reviutils/audio/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0a3/reviutils/audio/clipper.py
+-rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0a3/reviutils/audio/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.322327 reviutils-1.4.0a3/reviutils/common/
+-rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0a3/reviutils/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.325327 reviutils-1.4.0a3/reviutils/gis/
+-rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0a3/reviutils/gis/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0a3/reviutils/gis/convertor.py
+-rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0a3/reviutils/gis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.332328 reviutils-1.4.0a3/reviutils/noisepollution/
+-rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0a3/reviutils/noisepollution/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0a3/reviutils/noisepollution/evaluation.py
+-rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0a3/reviutils/noisepollution/funcarea.py
+-rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0a3/reviutils/noisepollution/hourhelper.py
+-rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0a3/reviutils/noisepollution/splhelper.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.333328 reviutils-1.4.0a3/reviutils/omap/
+-rw-rw-rw-   0        0        0       22 2024-04-16 08:13:41.000000 reviutils-1.4.0a3/reviutils/omap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:14:55.312755 reviutils-1.4.0a3/reviutils.egg-info/
+-rw-rw-rw-   0        0        0     2872 2024-04-16 08:14:55.000000 reviutils-1.4.0a3/reviutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2024-04-16 08:14:55.000000 reviutils-1.4.0a3/reviutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:14:55.000000 reviutils-1.4.0a3/reviutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 08:14:55.000000 reviutils-1.4.0a3/reviutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-04-16 08:14:55.000000 reviutils-1.4.0a3/reviutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 08:14:55.000000 reviutils-1.4.0a3/reviutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:14:55.336327 reviutils-1.4.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2024-04-16 08:14:49.000000 reviutils-1.4.0a3/setup.py
```

### Comparing `reviutils-1.4.0a2/LICENSE` & `reviutils-1.4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/PKG-INFO` & `reviutils-1.4.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0a2
+Version: 1.4.0a3
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a2 Summary: A common
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a3 Summary: A common
 library frequently used on python Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
```

### Comparing `reviutils-1.4.0a2/README.md` & `reviutils-1.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/api/amap/__init__.py` & `reviutils-1.4.0a3/reviutils/api/amap/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/audio/clipper.py` & `reviutils-1.4.0a3/reviutils/audio/clipper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/audio/reader.py` & `reviutils-1.4.0a3/reviutils/audio/reader.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/common/__init__.py` & `reviutils-1.4.0a3/reviutils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/gis/convertor.py` & `reviutils-1.4.0a3/reviutils/gis/convertor.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/gis/main.py` & `reviutils-1.4.0a3/reviutils/gis/main.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/noisepollution/evaluation.py` & `reviutils-1.4.0a3/reviutils/noisepollution/evaluation.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/noisepollution/funcarea.py` & `reviutils-1.4.0a3/reviutils/noisepollution/funcarea.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/noisepollution/hourhelper.py` & `reviutils-1.4.0a3/reviutils/noisepollution/hourhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils/noisepollution/splhelper.py` & `reviutils-1.4.0a3/reviutils/noisepollution/splhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/reviutils.egg-info/PKG-INFO` & `reviutils-1.4.0a3/reviutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.4.0a2
+Version: 1.4.0a3
 Summary: A common library frequently used on python
 Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI
 Author-email: reviy-top@outlook.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a2 Summary: A common
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a3 Summary: A common
 library frequently used on python Home-page: https://github.com/Viyyy/viutils
 Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
```

### Comparing `reviutils-1.4.0a2/reviutils.egg-info/SOURCES.txt` & `reviutils-1.4.0a3/reviutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reviutils-1.4.0a2/setup.py` & `reviutils-1.4.0a3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 # 打包命令
 python setup.py sdist bdist_wheel
 # 上传命令
 twine upload dist/* --verbose
 '''
-
+import rm_setup
 from setuptools import setup
     
 with open('requirements.txt','r',encoding='utf-8') as f:
     packages = [l for l in f.read().splitlines() if not l.startswith('#') and l.strip()!='']
 
 with open('README.md','r',encoding='utf-8') as f:
     long_description = f.read()
@@ -26,15 +26,15 @@
             else:
                 del_pycache(os.path.join(root, dir))
 
 del_pycache('reviutils') # 删除reviutils下的每个子文件夹的__pycache__文件夹
 
 setup(
     name='reviutils',
-    version='1.4.0a2',
+    version='1.4.0a3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='A common library frequently used on python',
     url='https://github.com/Viyyy/viutils',
     author='Re.VI',
     author_email='reviy-top@outlook.com',
     license='Apache License 2.0',
```

