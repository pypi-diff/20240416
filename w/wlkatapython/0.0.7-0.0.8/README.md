# Comparing `tmp/wlkatapython-0.0.7.tar.gz` & `tmp/wlkatapython-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkatapython-0.0.7.tar", last modified: Mon Nov 20 09:13:44 2023, max compression
+gzip compressed data, was "wlkatapython-0.0.8.tar", last modified: Mon Apr 15 11:16:56 2024, max compression
```

## Comparing `wlkatapython-0.0.7.tar` & `wlkatapython-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 09:13:44.586028 wlkatapython-0.0.7/
--rw-rw-rw-   0        0        0      319 2023-11-20 09:13:44.586028 wlkatapython-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-11-20 09:13:44.587251 wlkatapython-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      520 2023-11-20 08:55:46.000000 wlkatapython-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-20 09:13:44.585029 wlkatapython-0.0.7/wlkatapython.egg-info/
--rw-rw-rw-   0        0        0      319 2023-11-20 09:13:44.000000 wlkatapython-0.0.7/wlkatapython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-11-20 09:13:44.000000 wlkatapython-0.0.7/wlkatapython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 09:13:44.000000 wlkatapython-0.0.7/wlkatapython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-20 09:13:44.000000 wlkatapython-0.0.7/wlkatapython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16152 2023-11-20 08:57:41.000000 wlkatapython-0.0.7/wlkatapython.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:16:56.427834 wlkatapython-0.0.8/
+-rw-rw-rw-   0        0        0     1059 2024-04-15 03:18:13.000000 wlkatapython-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      360 2024-04-15 11:16:56.425730 wlkatapython-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2023-11-21 02:22:29.000000 wlkatapython-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:16:56.427834 wlkatapython-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      565 2024-04-15 10:40:39.000000 wlkatapython-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:16:56.425730 wlkatapython-0.0.8/wlkatapython.egg-info/
+-rw-rw-rw-   0        0        0      360 2024-04-15 11:16:56.000000 wlkatapython-0.0.8/wlkatapython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-15 11:16:56.000000 wlkatapython-0.0.8/wlkatapython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:16:56.000000 wlkatapython-0.0.8/wlkatapython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 11:16:56.000000 wlkatapython-0.0.8/wlkatapython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 11:16:56.000000 wlkatapython-0.0.8/wlkatapython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    43088 2024-04-15 11:15:41.000000 wlkatapython-0.0.8/wlkatapython.py
```

### Comparing `wlkatapython-0.0.7/setup.py` & `wlkatapython-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup
 
 setup(
     name='wlkatapython', # 自定义包名
-    version='0.0.7', # 包的版本号
+    version='0.0.8', # 包的版本号
     description='WLKATA-Mirobot/E4 Multiple robotic arm control!', # 描述信息
     long_description='Suitable for controlling single or multiple Mirobot robotic arms, E4 robotic arms, slides, and conveyor belts. Note that a multifunctional controller must be used to use this SDK.',
-    author='dong shuo', # 作者
+    author='DS', # 作者
     py_modules=[
         'wlkatapython'
-    ] # 包中包含的模块
+    ] ,# 包中包含的模块
+    install_requires=[
+        'pyserial'
+    ]
 )
```

