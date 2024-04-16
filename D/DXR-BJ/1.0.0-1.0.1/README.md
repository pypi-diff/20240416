# Comparing `tmp/DXR_BJ-1.0.0.tar.gz` & `tmp/DXR_BJ-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR_BJ-1.0.0.tar", last modified: Tue Apr 16 02:09:45 2024, max compression
+gzip compressed data, was "DXR_BJ-1.0.1.tar", last modified: Tue Apr 16 05:08:58 2024, max compression
```

## Comparing `DXR_BJ-1.0.0.tar` & `DXR_BJ-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:09:45.505377 DXR_BJ-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-04-16 02:09:45.447542 DXR_BJ-1.0.0/DXR_BJ/
--rw-rw-rw-   0        0        0      916 2024-04-16 01:46:33.000000 DXR_BJ-1.0.0/DXR_BJ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:09:45.429770 DXR_BJ-1.0.0/DXR_BJ/common/
-drwxrwxrwx   0        0        0        0 2024-04-16 02:09:45.468497 DXR_BJ-1.0.0/DXR_BJ/common/dependency/
--rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.0/DXR_BJ/common/dependency/simsun.ttc
--rw-rw-rw-   0        0        0    34427 2024-04-16 02:03:21.000000 DXR_BJ-1.0.0/DXR_BJ/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:09:45.467478 DXR_BJ-1.0.0/DXR_BJ.egg-info/
--rw-rw-rw-   0        0        0      153 2024-04-16 02:09:45.000000 DXR_BJ-1.0.0/DXR_BJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-16 02:09:45.000000 DXR_BJ-1.0.0/DXR_BJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 02:09:45.000000 DXR_BJ-1.0.0/DXR_BJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-16 02:09:45.000000 DXR_BJ-1.0.0/DXR_BJ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 02:09:45.000000 DXR_BJ-1.0.0/DXR_BJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      153 2024-04-16 02:09:45.504380 DXR_BJ-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 02:09:45.505377 DXR_BJ-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1788 2024-04-16 02:09:43.000000 DXR_BJ-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:09:45.504380 DXR_BJ-1.0.0/tests/
--rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-1.0.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:08:58.173589 DXR_BJ-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-16 05:08:58.121542 DXR_BJ-1.0.1/DXR_BJ/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.1/DXR_BJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:08:58.104152 DXR_BJ-1.0.1/DXR_BJ/common/
+drwxrwxrwx   0        0        0        0 2024-04-16 05:08:58.135689 DXR_BJ-1.0.1/DXR_BJ/common/dependency/
+-rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.1/DXR_BJ/common/dependency/simsun.ttc
+-rw-rw-rw-   0        0        0    34575 2024-04-16 05:08:37.000000 DXR_BJ-1.0.1/DXR_BJ/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:08:58.134692 DXR_BJ-1.0.1/DXR_BJ.egg-info/
+-rw-rw-rw-   0        0        0      153 2024-04-16 05:08:57.000000 DXR_BJ-1.0.1/DXR_BJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-16 05:08:57.000000 DXR_BJ-1.0.1/DXR_BJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 05:08:57.000000 DXR_BJ-1.0.1/DXR_BJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-16 05:08:57.000000 DXR_BJ-1.0.1/DXR_BJ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 05:08:57.000000 DXR_BJ-1.0.1/DXR_BJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      153 2024-04-16 05:08:58.172611 DXR_BJ-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 05:08:58.173589 DXR_BJ-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1788 2024-04-16 04:43:38.000000 DXR_BJ-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:08:58.171594 DXR_BJ-1.0.1/tests/
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-1.0.1/tests/test.py
```

### Comparing `DXR_BJ-1.0.0/DXR_BJ/common/dependency/simsun.ttc` & `DXR_BJ-1.0.1/DXR_BJ/common/dependency/simsun.ttc`

 * *Files identical despite different names*

### Comparing `DXR_BJ-1.0.0/DXR_BJ/drawer.py` & `DXR_BJ-1.0.1/DXR_BJ/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 # @三种标记方式编写成三个类，加上标记类和颜色类一共五个
 # @ Drawer Colors Freetype2ch  Imagefusion  FreetypePy
 # @ 外部调用接口     drawer = Drawer(字体目录)  outimg,_=drawer.draw_frame_box(img,outmessage)
 # @ 暂时只包含画矩形 区域 线
 
 
 import copy
+import os
 import cv2
 import numpy as np
 import math
 import freetype   ## Freetypechinese
 import traceback  ## log
 
-###版本号
-Version_num='1.0.0'
-## 中英对照列表
-alg_name = {
+
+###全局变量
+Version_num='1.0.1'     ###版本号
+py_path=os.path.dirname(os.path.abspath(__file__))   ##字体路径
+                              
+alg_name = { 
     "smoke": "烟雾",
     "fire": "火焰",
     "person": "行人",
     "car": "车",
     "IRPerson": "夜视行人",
     "open": "开启",
     "cover": "关闭",
@@ -53,16 +56,17 @@
     "drip": "滴漏",
     "hat": "戴帽",
     "no_hat": "未戴帽",
     "animal": "动物",
     "face": "人脸",
     "lpr": "车牌",
 }
+## 中英对照列表   
+
 
-## print打印
 class logger():
     def info(message):
         print(message)
         return
 
 ### 定义框颜色类，包含20个颜色
 class Colors:
@@ -212,15 +216,15 @@
 
 
 
 
 ### 定义标记类 
 class Drawer(object):
     ##  初始化接口
-    def __init__(self, import_path="common/dependency"):
+    def __init__(self, import_path=os.path.join(py_path, "common/dependency") ):
         try:
             logger.info(f'标记类的版本号为:{Version_num}')
             self.import_path = import_path
             self.font_path = self.import_path + '/simsun.ttc'
             self.font = cv2.FONT_HERSHEY_SIMPLEX
             ##中英对照表全局标记名字
             self.global_label_name = alg_name
```

### Comparing `DXR_BJ-1.0.0/setup.py` & `DXR_BJ-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup,find_packages
 setup(
   name='DXR_BJ',      ##from 引入的名称
-  version='1.0.0',    ##发布的版本号
+  version='1.0.1',    ##发布的版本号
   description='标记类正常的功能',
   author='zx',
   author_email='450125770@qq.com',
   install_requires= ['opencv-python','numpy',"freetype-py"], # 定义依赖哪些模块
   packages=find_packages(),  # 系统自动从当前目录开始找包
   include_package_data=True,
   # 如果有的文件不用打包，则只能指定需要打包的文件
```

