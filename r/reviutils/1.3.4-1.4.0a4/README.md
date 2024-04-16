# Comparing `tmp/reviutils-1.3.4.tar.gz` & `tmp/reviutils-1.4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviutils-1.3.4.tar", last modified: Thu Apr 11 08:53:25 2024, max compression
+gzip compressed data, was "reviutils-1.4.0a4.tar", last modified: Tue Apr 16 08:17:44 2024, max compression
```

## Comparing `reviutils-1.3.4.tar` & `reviutils-1.4.0a4.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.709816 reviutils-1.3.4/
--rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.3.4/LICENSE
--rw-rw-rw-   0        0        0     2870 2024-04-11 08:53:25.708817 reviutils-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.677816 reviutils-1.3.4/reviutils/
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.690816 reviutils-1.3.4/reviutils/api/
--rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.3.4/reviutils/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.692815 reviutils-1.3.4/reviutils/api/amap/
--rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.3.4/reviutils/api/amap/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.3.4/reviutils/api/amap/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.696816 reviutils-1.3.4/reviutils/audio/
--rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.3.4/reviutils/audio/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.3.4/reviutils/audio/clipper.py
--rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.3.4/reviutils/audio/reader.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.697816 reviutils-1.3.4/reviutils/common/
--rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.3.4/reviutils/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.701816 reviutils-1.3.4/reviutils/gis/
--rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.3.4/reviutils/gis/__init__.py
--rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.3.4/reviutils/gis/convertor.py
--rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.3.4/reviutils/gis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.707815 reviutils-1.3.4/reviutils/noisepollution/
--rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.3.4/reviutils/noisepollution/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.3.4/reviutils/noisepollution/evaluation.py
--rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.3.4/reviutils/noisepollution/funcarea.py
--rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.3.4/reviutils/noisepollution/hourhelper.py
--rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.3.4/reviutils/noisepollution/splhelper.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:53:25.688816 reviutils-1.3.4/reviutils.egg-info/
--rw-rw-rw-   0        0        0     2870 2024-04-11 08:53:25.000000 reviutils-1.3.4/reviutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2024-04-11 08:53:25.000000 reviutils-1.3.4/reviutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 08:53:25.000000 reviutils-1.3.4/reviutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-11 08:53:25.000000 reviutils-1.3.4/reviutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2024-04-11 08:53:25.000000 reviutils-1.3.4/reviutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 08:53:25.000000 reviutils-1.3.4/reviutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 08:53:25.709816 reviutils-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1485 2024-04-11 08:52:49.000000 reviutils-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.691166 reviutils-1.4.0a4/
+-rw-rw-rw-   0        0        0    11558 2024-03-14 03:50:07.000000 reviutils-1.4.0a4/LICENSE
+-rw-rw-rw-   0        0        0     2872 2024-04-16 08:17:44.691166 reviutils-1.4.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2024-04-11 07:45:45.000000 reviutils-1.4.0a4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.650165 reviutils-1.4.0a4/reviutils/
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.664165 reviutils-1.4.0a4/reviutils/api/
+-rw-rw-rw-   0        0        0       57 2024-03-27 06:31:11.000000 reviutils-1.4.0a4/reviutils/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.666166 reviutils-1.4.0a4/reviutils/api/amap/
+-rw-rw-rw-   0        0        0     2497 2024-04-11 08:50:46.000000 reviutils-1.4.0a4/reviutils/api/amap/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-11 08:36:43.000000 reviutils-1.4.0a4/reviutils/api/amap/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.669167 reviutils-1.4.0a4/reviutils/audio/
+-rw-rw-rw-   0        0        0      116 2024-03-20 03:20:30.000000 reviutils-1.4.0a4/reviutils/audio/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-03-18 03:19:04.000000 reviutils-1.4.0a4/reviutils/audio/clipper.py
+-rw-rw-rw-   0        0        0     1534 2024-03-20 03:42:36.000000 reviutils-1.4.0a4/reviutils/audio/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.671166 reviutils-1.4.0a4/reviutils/common/
+-rw-rw-rw-   0        0        0     3467 2024-03-15 02:38:48.000000 reviutils-1.4.0a4/reviutils/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.674166 reviutils-1.4.0a4/reviutils/gis/
+-rw-rw-rw-   0        0        0      106 2024-04-11 06:29:44.000000 reviutils-1.4.0a4/reviutils/gis/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-04-11 08:35:09.000000 reviutils-1.4.0a4/reviutils/gis/convertor.py
+-rw-rw-rw-   0        0        0      558 2024-04-11 06:29:44.000000 reviutils-1.4.0a4/reviutils/gis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.682166 reviutils-1.4.0a4/reviutils/noisepollution/
+-rw-rw-rw-   0        0        0      314 2024-03-20 03:21:45.000000 reviutils-1.4.0a4/reviutils/noisepollution/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-03-14 08:34:09.000000 reviutils-1.4.0a4/reviutils/noisepollution/evaluation.py
+-rw-rw-rw-   0        0        0     4114 2024-03-19 08:00:42.000000 reviutils-1.4.0a4/reviutils/noisepollution/funcarea.py
+-rw-rw-rw-   0        0        0     1043 2024-03-20 03:33:29.000000 reviutils-1.4.0a4/reviutils/noisepollution/hourhelper.py
+-rw-rw-rw-   0        0        0     7313 2024-03-15 02:38:48.000000 reviutils-1.4.0a4/reviutils/noisepollution/splhelper.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.684166 reviutils-1.4.0a4/reviutils/omap/
+-rw-rw-rw-   0        0        0       22 2024-04-16 08:13:41.000000 reviutils-1.4.0a4/reviutils/omap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.685167 reviutils-1.4.0a4/reviutils/omap/constants/
+-rw-rw-rw-   0        0        0     3723 2024-04-16 01:26:46.000000 reviutils-1.4.0a4/reviutils/omap/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.689165 reviutils-1.4.0a4/reviutils/omap/samples/
+-rw-rw-rw-   0        0        0     1131 2024-04-16 02:18:53.000000 reviutils-1.4.0a4/reviutils/omap/samples/Base.py
+-rw-rw-rw-   0        0        0       19 2024-04-16 08:13:29.000000 reviutils-1.4.0a4/reviutils/omap/samples/__init__.py
+-rw-rw-rw-   0        0        0    12530 2024-04-16 08:00:15.000000 reviutils-1.4.0a4/reviutils/omap/samples/main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:17:44.662165 reviutils-1.4.0a4/reviutils.egg-info/
+-rw-rw-rw-   0        0        0     2872 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 08:17:44.000000 reviutils-1.4.0a4/reviutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:17:44.692165 reviutils-1.4.0a4/setup.cfg
+-rw-rw-rw-   0        0        0     1688 2024-04-16 08:17:24.000000 reviutils-1.4.0a4/setup.py
```

### Comparing `reviutils-1.3.4/LICENSE` & `reviutils-1.4.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/PKG-INFO` & `reviutils-1.4.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.3.4
+Version: 1.4.0a4
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
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.3.4 Summary: A common library
-frequently used on python Home-page: https://github.com/Viyyy/viutils Author:
-Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a4 Summary: A common
+library frequently used on python Home-page: https://github.com/Viyyy/viutils
+Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_g_i_t_h_u_b_-_r_e_v_i_u_t_i_l_s_-_r_e_d_?_l_o_g_o_=_g_i_t_h_u_b_]Â Â  _[_h_t_t_p_s_:_/_/
       _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_a_s_t_a_p_i_-_d_e_m_o_-_g_r_e_e_n_?_l_o_g_o_=_f_a_s_t_a_p_i_]Â Â  _[_h_t_t_p_s_:_/_/
```

### Comparing `reviutils-1.3.4/README.md` & `reviutils-1.4.0a4/README.md`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/api/amap/__init__.py` & `reviutils-1.4.0a4/reviutils/api/amap/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/audio/clipper.py` & `reviutils-1.4.0a4/reviutils/audio/clipper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/audio/reader.py` & `reviutils-1.4.0a4/reviutils/audio/reader.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/common/__init__.py` & `reviutils-1.4.0a4/reviutils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/gis/convertor.py` & `reviutils-1.4.0a4/reviutils/gis/convertor.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/gis/main.py` & `reviutils-1.4.0a4/reviutils/gis/main.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/noisepollution/evaluation.py` & `reviutils-1.4.0a4/reviutils/noisepollution/evaluation.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/noisepollution/funcarea.py` & `reviutils-1.4.0a4/reviutils/noisepollution/funcarea.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/noisepollution/hourhelper.py` & `reviutils-1.4.0a4/reviutils/noisepollution/hourhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils/noisepollution/splhelper.py` & `reviutils-1.4.0a4/reviutils/noisepollution/splhelper.py`

 * *Files identical despite different names*

### Comparing `reviutils-1.3.4/reviutils.egg-info/PKG-INFO` & `reviutils-1.4.0a4/reviutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviutils
-Version: 1.3.4
+Version: 1.4.0a4
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
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: reviutils Version: 1.3.4 Summary: A common library
-frequently used on python Home-page: https://github.com/Viyyy/viutils Author:
-Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
+Metadata-Version: 2.1 Name: reviutils Version: 1.4.0a4 Summary: A common
+library frequently used on python Home-page: https://github.com/Viyyy/viutils
+Author: Re.VI Author-email: reviy-top@outlook.com License: Apache License 2.0
 Description-Content-Type: text/markdown Provides-Extra: audio License-File:
 LICENSE
                             ************ rreevviiuuttiillss ************
                            ä¸ä¸ªå¸¸ç¨çPythonåº
                             _ç_®__ä_½__ä_¸_­_æ__ï½ _E_n_g_l_i_s_h
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_g_i_t_h_u_b_-_r_e_v_i_u_t_i_l_s_-_r_e_d_?_l_o_g_o_=_g_i_t_h_u_b_]Â Â  _[_h_t_t_p_s_:_/_/
       _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_a_s_t_a_p_i_-_d_e_m_o_-_g_r_e_e_n_?_l_o_g_o_=_f_a_s_t_a_p_i_]Â Â  _[_h_t_t_p_s_:_/_/
```

### Comparing `reviutils-1.3.4/reviutils.egg-info/SOURCES.txt` & `reviutils-1.4.0a4/reviutils.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,13 @@
 reviutils/gis/__init__.py
 reviutils/gis/convertor.py
 reviutils/gis/main.py
 reviutils/noisepollution/__init__.py
 reviutils/noisepollution/evaluation.py
 reviutils/noisepollution/funcarea.py
 reviutils/noisepollution/hourhelper.py
-reviutils/noisepollution/splhelper.py
+reviutils/noisepollution/splhelper.py
+reviutils/omap/__init__.py
+reviutils/omap/constants/__init__.py
+reviutils/omap/samples/Base.py
+reviutils/omap/samples/__init__.py
+reviutils/omap/samples/main.py
```

### Comparing `reviutils-1.3.4/setup.py` & `reviutils-1.4.0a4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,62 @@
-'''
+"""
 # 打包命令
 python setup.py sdist bdist_wheel
 # 上传命令
 twine upload dist/* --verbose
-'''
+"""
 
+import rm_setup
 from setuptools import setup
-    
-with open('requirements.txt','r',encoding='utf-8') as f:
-    packages = [l for l in f.read().splitlines() if not l.startswith('#') and l.strip()!='']
 
-with open('README.md','r',encoding='utf-8') as f:
+with open("requirements.txt", "r", encoding="utf-8") as f:
+    packages = [
+        l for l in f.read().splitlines() if not l.startswith("#") and l.strip() != ""
+    ]
+
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
-    
+
 
 import os
 import shutil
 
+
 # 递归删除每个子文件夹的__pycache__
 def del_pycache(path):
     for root, dirs, files in os.walk(path):
         for dir in dirs:
-            if dir == '__pycache__':
+            if dir == "__pycache__":
                 shutil.rmtree(os.path.join(root, dir))
             else:
                 del_pycache(os.path.join(root, dir))
 
-del_pycache('reviutils') # 删除reviutils下的每个子文件夹的__pycache__文件夹
+
+del_pycache("reviutils")  # 删除reviutils下的每个子文件夹的__pycache__文件夹
 
 setup(
-    name='reviutils',
-    version='1.3.4',
+    name="reviutils",
+    version="1.4.0a4",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    description='A common library frequently used on python',
-    url='https://github.com/Viyyy/viutils',
-    author='Re.VI',
-    author_email='reviy-top@outlook.com',
-    license='Apache License 2.0',
-    packages=['reviutils.common','reviutils.noisepollution','reviutils.audio','reviutils.api','reviutils.api.amap','reviutils.gis'],
+    long_description_content_type="text/markdown",
+    description="A common library frequently used on python",
+    url="https://github.com/Viyyy/viutils",
+    author="Re.VI",
+    author_email="reviy-top@outlook.com",
+    license="Apache License 2.0",
+    packages=[
+        "reviutils.common",
+        "reviutils.noisepollution",
+        "reviutils.audio",
+        "reviutils.api",
+        "reviutils.api.amap",
+        "reviutils.gis",
+        "reviutils.omap",
+        "reviutils.omap.samples",
+        "reviutils.omap.constants"
+    ],
     install_requires=packages,
     extras_require={
-        'audio': ['librosa', 'soundfile','torch', 'torchaudio','pydub','starlette']
+        "audio": ["librosa", "soundfile", "torch", "torchaudio", "pydub", "starlette"]
     },
-    zip_safe=False
+    zip_safe=False,
 )
-
-
```

