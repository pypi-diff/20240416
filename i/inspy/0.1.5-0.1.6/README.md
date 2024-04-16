# Comparing `tmp/inspy-0.1.5.tar.gz` & `tmp/inspy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inspy-0.1.5.tar", last modified: Mon Apr  1 06:21:45 2024, max compression
+gzip compressed data, was "dist\inspy-0.1.6.tar", last modified: Tue Apr 16 07:01:19 2024, max compression
```

## Comparing `inspy-0.1.5.tar` & `inspy-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 06:21:45.000000 inspy-0.1.5/
--rw-rw-rw-   0        0        0     1086 2024-03-29 02:52:46.000000 inspy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       22 2024-03-29 10:16:21.000000 inspy-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1373 2024-04-01 06:21:45.000000 inspy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-01 06:20:14.000000 inspy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 06:21:45.000000 inspy-0.1.5/inspy.egg-info/
--rw-rw-rw-   0        0        0     1373 2024-04-01 06:21:45.000000 inspy-0.1.5/inspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-01 06:21:45.000000 inspy-0.1.5/inspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 06:21:45.000000 inspy-0.1.5/inspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-01 06:21:45.000000 inspy-0.1.5/inspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 06:21:45.000000 inspy-0.1.5/inspy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 06:21:45.000000 inspy-0.1.5/piinspy/
--rw-rw-rw-   0        0        0     2429 2024-03-29 02:56:18.000000 inspy-0.1.5/piinspy/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-12-29 03:22:28.000000 inspy-0.1.5/piinspy/ins.json
--rw-rw-rw-   0        0        0    10166 2024-03-28 09:53:58.000000 inspy-0.1.5/piinspy/ins_class.py
--rw-rw-rw-   0        0        0     1159 2024-03-28 10:09:09.000000 inspy-0.1.5/piinspy/ins_function.py
--rw-rw-rw-   0        0        0      920 2024-03-29 02:36:10.000000 inspy-0.1.5/piinspy/insconst.py
--rw-rw-rw-   0        0        0      904 2024-03-29 02:57:10.000000 inspy-0.1.5/piinspy/log.py
--rw-rw-rw-   0        0        0       77 2023-11-20 02:03:46.000000 inspy-0.1.5/piinspy/package.json
--rw-rw-rw-   0        0        0       42 2024-04-01 06:21:45.000000 inspy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1480 2024-04-01 06:21:26.000000 inspy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:01:19.000000 inspy-0.1.6/
+-rw-rw-rw-   0        0        0     1086 2024-03-29 02:52:46.000000 inspy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       22 2024-03-29 10:16:21.000000 inspy-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1386 2024-04-16 07:01:19.000000 inspy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2024-04-01 06:20:14.000000 inspy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:01:19.000000 inspy-0.1.6/inspy.egg-info/
+-rw-rw-rw-   0        0        0     1386 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 07:01:19.000000 inspy-0.1.6/piinspy/
+-rw-rw-rw-   0        0        0     2429 2024-03-29 02:56:18.000000 inspy-0.1.6/piinspy/__init__.py
+-rw-rw-rw-   0        0        0     2135 2024-04-16 06:49:45.000000 inspy-0.1.6/piinspy/ins.json
+-rw-rw-rw-   0        0        0    10166 2024-03-28 09:53:58.000000 inspy-0.1.6/piinspy/ins_class.py
+-rw-rw-rw-   0        0        0     1159 2024-03-28 10:09:09.000000 inspy-0.1.6/piinspy/ins_function.py
+-rw-rw-rw-   0        0        0      920 2024-03-29 02:36:10.000000 inspy-0.1.6/piinspy/insconst.py
+-rw-rw-rw-   0        0        0      904 2024-03-29 02:57:10.000000 inspy-0.1.6/piinspy/log.py
+-rw-rw-rw-   0        0        0       77 2023-11-20 02:03:46.000000 inspy-0.1.6/piinspy/package.json
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:01:19.000000 inspy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2024-04-16 07:01:07.000000 inspy-0.1.6/setup.py
```

### Comparing `inspy-0.1.5/LICENSE` & `inspy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/PKG-INFO` & `inspy-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inspy
-Version: 0.1.5
-Summary: scan and control for instrument that support SCPI COMMAND
+Version: 0.1.6
+Summary: scan and control for instrument that support SCPI COMMAND added 34461A
 Home-page: https://github.com/AceWalTer/inspy
 Author: Yafei Wang
 Author-email: yafei.wang@pisemi.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inspy-0.1.5/README.md` & `inspy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/inspy.egg-info/PKG-INFO` & `inspy-0.1.6/inspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inspy
-Version: 0.1.5
-Summary: scan and control for instrument that support SCPI COMMAND
+Version: 0.1.6
+Summary: scan and control for instrument that support SCPI COMMAND added 34461A
 Home-page: https://github.com/AceWalTer/inspy
 Author: Yafei Wang
 Author-email: yafei.wang@pisemi.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inspy-0.1.5/piinspy/__init__.py` & `inspy-0.1.6/piinspy/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/piinspy/ins.json` & `inspy-0.1.6/piinspy/ins.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'DMM'": "{'34461': OrderedDict([('register', '*IDN?'), ('reset', '*RST'), ('conf', "*

 * *          "'CONF:{MODE}:{TYPE}'), ('samp', 'SAMP:COUN {COUNT}'), ('trig', 'TRIG:SOUR {TRIG}'), "*

 * *          "('range', 'SENS:{MODE}:{TYPE}:RANG {RANGE}'), ('read', 'READ?')])}"}*

```diff
@@ -1,9 +1,18 @@
 {
     "DMM": {
+        "34461": {
+            "conf": "CONF:{MODE}:{TYPE}",
+            "range": "SENS:{MODE}:{TYPE}:RANG {RANGE}",
+            "read": "READ?",
+            "register": "*IDN?",
+            "reset": "*RST",
+            "samp": "SAMP:COUN {COUNT}",
+            "trig": "TRIG:SOUR {TRIG}"
+        },
         "gd906x": {
             "conf": "CONF:{MODE}:{TYPE}",
             "range": "SENS:{MODE}:{TYPE}:RANG {RANGE}",
             "read": "READ?",
             "register": "*IDN?",
             "reset": "*RST",
             "samp": "SAMP:COUN {COUNT}",
```

### Comparing `inspy-0.1.5/piinspy/ins_class.py` & `inspy-0.1.6/piinspy/ins_class.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/piinspy/ins_function.py` & `inspy-0.1.6/piinspy/ins_function.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/piinspy/insconst.py` & `inspy-0.1.6/piinspy/insconst.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/piinspy/log.py` & `inspy-0.1.6/piinspy/log.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.5/setup.py` & `inspy-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     @Description: None \n
     @Create Time: 2024/3/29 11:16 \n
 """
 from setuptools import setup, find_packages
 
 setup(
     name='inspy',  # 包名
-    version='0.1.5',  # 包的版本
+    version='0.1.6',  # 包的版本
     author='Yafei Wang',  # 作者名字
     author_email='yafei.wang@pisemi.com',  # 作者邮箱
-    description='scan and control for instrument that support SCPI COMMAND',  # 简短描述
+    description='scan and control for instrument that support SCPI COMMAND added 34461A',  # 简短描述
     long_description=open('README.md').read(),  # 长描述，通常是README
     long_description_content_type='text/markdown',  # 长描述的类型，这里是markdown
     url='https://github.com/AceWalTer/inspy',  # 项目主页
     packages=find_packages(),  # 自动找到项目中的所有包
     include_package_data=True,
     install_requires=[
         # 这里列出了项目的依赖
```

