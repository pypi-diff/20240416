# Comparing `tmp/DXR_BJ-0.0.1.tar.gz` & `tmp/DXR_BJ-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR_BJ-0.0.1.tar", last modified: Mon Apr 15 09:06:14 2024, max compression
+gzip compressed data, was "DXR_BJ-0.0.2.tar", last modified: Tue Apr 16 01:04:03 2024, max compression
```

## Comparing `DXR_BJ-0.0.1.tar` & `DXR_BJ-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:06:14.031522 DXR_BJ-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-15 09:06:14.026535 DXR_BJ-0.0.1/DXR_BJ.egg-info/
--rw-rw-rw-   0        0        0      150 2024-04-15 09:06:13.000000 DXR_BJ-0.0.1/DXR_BJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-04-15 09:06:13.000000 DXR_BJ-0.0.1/DXR_BJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:06:13.000000 DXR_BJ-0.0.1/DXR_BJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 09:06:13.000000 DXR_BJ-0.0.1/DXR_BJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      150 2024-04-15 09:06:14.030526 DXR_BJ-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 09:06:14.028529 DXR_BJ-0.0.1/dxr_bj/
--rw-rw-rw-   0        0        0      142 2024-04-15 09:00:34.000000 DXR_BJ-0.0.1/dxr_bj/DXR_BJ.py
--rw-rw-rw-   0        0        0       56 2024-04-15 05:55:54.000000 DXR_BJ-0.0.1/dxr_bj/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-15 09:06:14.031522 DXR_BJ-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1702 2024-04-15 09:03:39.000000 DXR_BJ-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:06:14.029528 DXR_BJ-0.0.1/tests/
--rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.854834 DXR_BJ-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.836705 DXR_BJ-0.0.2/DXR_BJ/
+-rw-rw-rw-   0        0        0       56 2024-04-15 05:55:54.000000 DXR_BJ-0.0.2/DXR_BJ/__init__.py
+-rw-rw-rw-   0        0        0      142 2024-04-15 09:31:33.000000 DXR_BJ-0.0.2/DXR_BJ/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.851663 DXR_BJ-0.0.2/DXR_BJ.egg-info/
+-rw-rw-rw-   0        0        0      150 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       59 2024-04-16 01:03:37.000000 DXR_BJ-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      150 2024-04-16 01:04:03.853658 DXR_BJ-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 01:04:03.854834 DXR_BJ-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1702 2024-04-16 01:02:35.000000 DXR_BJ-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.852660 DXR_BJ-0.0.2/tests/
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-0.0.2/tests/test.py
```

### Comparing `DXR_BJ-0.0.1/setup.py` & `DXR_BJ-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup,find_packages
 setup(
     name='DXR_BJ',
-      version='0.0.1',
+      version='0.0.2',
       description='打印测试下功能',
       author='zx',
       author_email='450125770@qq.com',
       requires= [], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

