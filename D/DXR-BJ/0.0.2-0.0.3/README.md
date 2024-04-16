# Comparing `tmp/DXR_BJ-0.0.2.tar.gz` & `tmp/DXR_BJ-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR_BJ-0.0.2.tar", last modified: Tue Apr 16 01:04:03 2024, max compression
+gzip compressed data, was "DXR_BJ-0.0.3.tar", last modified: Tue Apr 16 01:18:07 2024, max compression
```

## Comparing `DXR_BJ-0.0.2.tar` & `DXR_BJ-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.854834 DXR_BJ-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.836705 DXR_BJ-0.0.2/DXR_BJ/
--rw-rw-rw-   0        0        0       56 2024-04-15 05:55:54.000000 DXR_BJ-0.0.2/DXR_BJ/__init__.py
--rw-rw-rw-   0        0        0      142 2024-04-15 09:31:33.000000 DXR_BJ-0.0.2/DXR_BJ/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.851663 DXR_BJ-0.0.2/DXR_BJ.egg-info/
--rw-rw-rw-   0        0        0      150 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 01:04:02.000000 DXR_BJ-0.0.2/DXR_BJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       59 2024-04-16 01:03:37.000000 DXR_BJ-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      150 2024-04-16 01:04:03.853658 DXR_BJ-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 01:04:03.854834 DXR_BJ-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1702 2024-04-16 01:02:35.000000 DXR_BJ-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 01:04:03.852660 DXR_BJ-0.0.2/tests/
--rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-0.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:18:07.872118 DXR_BJ-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-16 01:18:07.665913 DXR_BJ-0.0.3/DXR_BJ/
+-rw-rw-rw-   0        0        0       56 2024-04-15 05:55:54.000000 DXR_BJ-0.0.3/DXR_BJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:18:07.662921 DXR_BJ-0.0.3/DXR_BJ/common/
+drwxrwxrwx   0        0        0        0 2024-04-16 01:18:07.836207 DXR_BJ-0.0.3/DXR_BJ/common/dependency/
+-rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-0.0.3/DXR_BJ/common/dependency/simsun.ttc
+-rw-rw-rw-   0        0        0      142 2024-04-15 09:31:33.000000 DXR_BJ-0.0.3/DXR_BJ/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:18:07.675887 DXR_BJ-0.0.3/DXR_BJ.egg-info/
+-rw-rw-rw-   0        0        0      150 2024-04-16 01:18:07.000000 DXR_BJ-0.0.3/DXR_BJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-04-16 01:18:07.000000 DXR_BJ-0.0.3/DXR_BJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:18:07.000000 DXR_BJ-0.0.3/DXR_BJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 01:18:07.000000 DXR_BJ-0.0.3/DXR_BJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      150 2024-04-16 01:18:07.871121 DXR_BJ-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 01:18:07.872118 DXR_BJ-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2024-04-16 01:17:02.000000 DXR_BJ-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:18:07.870124 DXR_BJ-0.0.3/tests/
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-0.0.3/tests/test.py
```

### Comparing `DXR_BJ-0.0.2/setup.py` & `DXR_BJ-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 
 from setuptools import setup,find_packages
 setup(
     name='DXR_BJ',
-      version='0.0.2',
-      description='打印测试下功能',
-      author='zx',
-      author_email='450125770@qq.com',
-      requires= [], # 定义依赖哪些模块
-      packages=find_packages(),  # 系统自动从当前目录开始找包
-      # 如果有的文件不用打包，则只能指定需要打包的文件
-      #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
-      license="apache 3.0"
-      )
+    version='0.0.3',
+    description='打印测试下功能',
+    author='zx',
+    author_email='450125770@qq.com',
+    requires= [], # 定义依赖哪些模块
+    packages=find_packages(),  # 系统自动从当前目录开始找包
+    include_package_data=True,
+    # 如果有的文件不用打包，则只能指定需要打包的文件
+    #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
+    license="apache 3.0"
+    )
 
 '''
 name : 打包后包的文件名
 version : 版本号
 author : 作者
 author_email : 作者的邮箱
 py_modules : 要打包的.py文件
```

