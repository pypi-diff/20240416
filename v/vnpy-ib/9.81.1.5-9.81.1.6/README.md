# Comparing `tmp/vnpy_ib-9.81.1.5.tar.gz` & `tmp/vnpy_ib-9.81.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_ib-9.81.1.5.tar", last modified: Tue Dec 13 07:49:42 2022, max compression
+gzip compressed data, was "vnpy_ib-9.81.1.6.tar", last modified: Wed Feb 15 14:09:26 2023, max compression
```

## Comparing `vnpy_ib-9.81.1.5.tar` & `vnpy_ib-9.81.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 07:49:42.281826 vnpy_ib-9.81.1.5/
--rw-rw-rw-   0        0        0     1109 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.5/LICENSE
--rw-rw-rw-   0        0        0     3020 2022-12-13 07:49:42.282864 vnpy_ib-9.81.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2040 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.5/README.md
--rw-rw-rw-   0        0        0     1021 2022-12-13 07:49:42.283903 vnpy_ib-9.81.1.5/setup.cfg
--rw-rw-rw-   0        0        0       43 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-13 07:49:42.248973 vnpy_ib-9.81.1.5/vnpy_ib/
--rw-rw-rw-   0        0        0     1352 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.5/vnpy_ib/__init__.py
--rw-rw-rw-   0        0        0    27313 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.5/vnpy_ib/ib_gateway.py
-drwxrwxrwx   0        0        0        0 2022-12-13 07:49:42.280248 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/
--rw-rw-rw-   0        0        0     3020 2022-12-13 07:49:42.000000 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-12-13 07:49:42.000000 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-13 07:49:42.000000 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-13 07:49:42.000000 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2022-12-13 07:49:42.000000 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-13 07:49:42.000000 vnpy_ib-9.81.1.5/vnpy_ib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-15 14:09:26.326276 vnpy_ib-9.81.1.6/
+-rw-rw-rw-   0        0        0     1109 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3020 2023-02-15 14:09:26.326276 vnpy_ib-9.81.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2040 2023-02-15 14:08:07.000000 vnpy_ib-9.81.1.6/README.md
+-rw-rw-rw-   0        0        0     1021 2023-02-15 14:09:26.329890 vnpy_ib-9.81.1.6/setup.cfg
+-rw-rw-rw-   0        0        0       43 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-15 14:09:26.279191 vnpy_ib-9.81.1.6/vnpy_ib/
+-rw-rw-rw-   0        0        0     1352 2022-12-13 07:48:57.000000 vnpy_ib-9.81.1.6/vnpy_ib/__init__.py
+-rw-rw-rw-   0        0        0    27412 2023-02-15 14:07:26.000000 vnpy_ib-9.81.1.6/vnpy_ib/ib_gateway.py
+drwxrwxrwx   0        0        0        0 2023-02-15 14:09:26.324229 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/
+-rw-rw-rw-   0        0        0     3020 2023-02-15 14:09:26.000000 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-02-15 14:09:26.000000 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-15 14:09:26.000000 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 14:09:26.000000 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-02-15 14:09:26.000000 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-02-15 14:09:26.000000 vnpy_ib-9.81.1.6/vnpy_ib.egg-info/top_level.txt
```

### Comparing `vnpy_ib-9.81.1.5/LICENSE` & `vnpy_ib-9.81.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_ib-9.81.1.5/PKG-INFO` & `vnpy_ib-9.81.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_ib
-Version: 9.81.1.5
+Version: 9.81.1.6
 Summary: IB gateway for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的InteractiveBrokers交易接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-9.81.1.5-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-9.81.1.6-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ib-9.81.1.5/README.md` & `vnpy_ib-9.81.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的InteractiveBrokers交易接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-9.81.1.5-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-9.81.1.6-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ib-9.81.1.5/setup.cfg` & `vnpy_ib-9.81.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6962 0d0a 7665 7273   = vnpy_ib..vers
-00000020: 696f 6e20 3d20 392e 3831 2e31 2e35 0d0a  ion = 9.81.1.5..
+00000020: 696f 6e20 3d20 392e 3831 2e31 2e36 0d0a  ion = 9.81.1.6..
 00000030: 7572 6c20 3d20 6874 7470 733a 2f2f 7777  url = https://ww
 00000040: 772e 766e 7079 2e63 6f6d 0d0a 6c69 6365  w.vnpy.com..lice
 00000050: 6e73 6520 3d20 4d49 540d 0a61 7574 686f  nse = MIT..autho
 00000060: 7220 3d20 5869 616f 796f 7520 4368 656e  r = Xiaoyou Chen
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2078 6961 6f79 6f75 2e63 6865 6e40 6d61   xiaoyou.chen@ma
 00000090: 696c 2e76 6e70 792e 636f 6d0d 0a64 6573  il.vnpy.com..des
```

### Comparing `vnpy_ib-9.81.1.5/vnpy_ib/__init__.py` & `vnpy_ib-9.81.1.6/vnpy_ib/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_ib-9.81.1.5/vnpy_ib/ib_gateway.py` & `vnpy_ib-9.81.1.6/vnpy_ib/ib_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,17 @@
 
         msg: str = f"服务器时间: {time_string}"
         self.gateway.write_log(msg)
 
     def error(self, reqId: TickerId, errorCode: int, errorString: str) -> None:
         """具体错误请求回报"""
         super().error(reqId, errorCode, errorString)
-        if reqId == self.history_reqid:
+    
+        # 2000-2999信息通知不属于报错信息
+        if reqId == self.history_reqid and errorCode not in range(2000, 3000):
             self.history_condition.acquire()
             self.history_condition.notify()
             self.history_condition.release()
 
         msg: str = f"信息通知，代码：{errorCode}，内容: {errorString}"
         self.gateway.write_log(msg)
```

### Comparing `vnpy_ib-9.81.1.5/vnpy_ib.egg-info/PKG-INFO` & `vnpy_ib-9.81.1.6/vnpy_ib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-ib
-Version: 9.81.1.5
+Version: 9.81.1.6
 Summary: IB gateway for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的InteractiveBrokers交易接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-9.81.1.5-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-9.81.1.6-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

