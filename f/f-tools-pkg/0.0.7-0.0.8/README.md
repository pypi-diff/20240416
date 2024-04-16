# Comparing `tmp/f_tools_pkg-0.0.7.tar.gz` & `tmp/f_tools_pkg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\f_tools_pkg-0.0.7.tar", last modified: Wed Apr 10 12:48:46 2024, max compression
+gzip compressed data, was "dist\f_tools_pkg-0.0.8.tar", last modified: Mon Apr 15 11:08:41 2024, max compression
```

## Comparing `f_tools_pkg-0.0.7.tar` & `f_tools_pkg-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/
--rw-rw-rw-   0        0        0      584 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-04-10 12:48:00.000000 f_tools_pkg-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg/
--rw-rw-rw-   0        0        0      108 2022-07-20 05:57:19.000000 f_tools_pkg-0.0.7/f_tools_pkg/__init__.py
--rw-rw-rw-   0        0        0     5610 2022-07-20 05:56:17.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_bmp.py
--rw-rw-rw-   0        0        0     5667 2024-04-10 12:46:32.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_crypt.py
--rw-rw-rw-   0        0        0     3393 2024-03-27 06:54:20.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_e.py
--rw-rw-rw-   0        0        0        0 2023-11-25 09:04:03.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_ecc.py
--rw-rw-rw-   0        0        0     1621 2022-04-14 06:45:04.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_excel.py
--rw-rw-rw-   0        0        0     1588 2022-03-11 02:30:39.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_log.py
--rw-rw-rw-   0        0        0     2250 2022-07-20 03:22:56.000000 f_tools_pkg-0.0.7/f_tools_pkg/f_serial.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/
--rw-rw-rw-   0        0        0      584 2024-04-10 12:48:45.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:48:45.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/f_tools_pkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 12:48:46.000000 f_tools_pkg-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-04-10 12:48:06.000000 f_tools_pkg-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/
+-rw-rw-rw-   0        0        0      625 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-04-15 11:08:01.000000 f_tools_pkg-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/f_tools_pkg/
+-rw-rw-rw-   0        0        0      108 2022-07-20 05:57:19.000000 f_tools_pkg-0.0.8/f_tools_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5610 2022-07-20 05:56:17.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_bmp.py
+-rw-rw-rw-   0        0        0     5667 2024-04-10 12:46:32.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_crypt.py
+-rw-rw-rw-   0        0        0     3981 2024-04-15 11:07:02.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_e.py
+-rw-rw-rw-   0        0        0        0 2023-11-25 09:04:03.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_ecc.py
+-rw-rw-rw-   0        0        0     1621 2022-04-14 06:45:04.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_excel.py
+-rw-rw-rw-   0        0        0     1588 2022-03-11 02:30:39.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_log.py
+-rw-rw-rw-   0        0        0     2250 2022-07-20 03:22:56.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/
+-rw-rw-rw-   0        0        0      625 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-04-15 11:07:15.000000 f_tools_pkg-0.0.8/setup.py
```

### Comparing `f_tools_pkg-0.0.7/PKG-INFO` & `f_tools_pkg-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f_tools_pkg
-Version: 0.0.7
+Version: 0.0.8
 Summary: some common tools(bmp/crypt/excel/log ...)
 Home-page: 
 Author: wushengyan
 Author-email: WUSY1991@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,8 +15,10 @@
 
 2022-7-20 V0.0.4  add bmp_scale function
 
 2024-3-27 V0.06  e bu add "type" parameter
 
 2024-4-10 v0.007 des3 key mast 24 Bytes, and 23:16 must not '0'
 
+2024-4-15 v0.008 command with timeout
+
```

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg/f_bmp.py` & `f_tools_pkg-0.0.8/f_tools_pkg/f_bmp.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg/f_crypt.py` & `f_tools_pkg-0.0.8/f_tools_pkg/f_crypt.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg/f_e.py` & `f_tools_pkg-0.0.8/f_tools_pkg/f_e.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,111 @@
 import os
+import subprocess
 
 class yc_e:
     def __init__(self,timeout):
-        
         for num in range(0,timeout):
             ret = os.popen("e z").readlines()
             if ret[0].find("sync 0 = 02")!=-1:
                 break
         if(num >=timeout):  
             print("can't e command")
             
+    def run(command, timeout_duration=None, default_value="0"):
+        try:
+            command = command.strip().split(" ")
+            print(command)
+            result = subprocess.run(
+                command,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                text=True,
+                timeout=timeout_duration,
+            )
+            return result.stdout  # 返回正确执行时的输出
+        except subprocess.TimeoutExpired:
+            # 进程超时
+            print("Calling '{' '.join(command)}' timed out after {timeout_duration} seconds.")
+            return default_value  # 返回默认值
+            
     def e_k(self):
-        os.system("e k")
+        self.run("e k")
         
     def e_p(self):
         while True:
-            ret = os.popen("e p").readline()
+            ret =  self.run("e p")
             print(ret)
             if ret.find("Stopped") != -1:
                 break
         return int(ret.split(" ")[3].replace(":",""),16)
     
     def e_pu(self):
         while True:
-            ret = os.popen("e pu").readline()
+            ret = self.run("e pu")
             print(ret)
             if ret.find("Stopped") != -1:
                 break
         return int(ret.split(" ")[3].replace(":",""),16)
 
     def e_pr(self):
         while True:
-            ret = os.popen("e pr").readline()
+            ret = self.run("e pr")
             print(ret)
             if ret.find("Stopped") != -1:
                 break
         return int(ret.split(" ")[3].replace(":",""),16)
     
     def e_tu(self):
         addr = -1
-        ret = os.popen("e tu").readline()
+        ret = self.run("e tu")
         print(ret)
         if ret.find("CPU") != -1:
             addr = int(ret.split(" ")[3].replace(":",""),16)
         return addr
     
     def e_nu(self):
         addr = -1
-        ret = os.popen("e nu").readline()
+        ret = self.run("e nu")
         print(ret)
         if ret.find("CPU") != -1:
             addr = int(ret.split(" ")[3].replace(":",""),16)
         return addr
     
     def e_cu(self):
-        ret = os.popen("e cu").readline()
+        ret = self.run("e cu")
         print(ret)
         return self.e_au()
         
     def e_bu(self,addr,type=0):
-        ret = os.popen("e bu " + hex(addr).replace("0x","") + hex(type).replace("0x"," ")).readline()
+        ret = self.run("e bu " + hex(addr).replace("0x","") + hex(type).replace("0x"," "))
         print(ret)
     
     def e_ru(self,reg):
-        ret = os.popen("e ru "+reg).readline()
+        ret = self.run("e ru "+reg)
         print(ret)
         return [int(ret.split(" ")[1],10),ret.split(" ")[3].strip()]
         
     
     def e_au(self):
         isstop = 0
         pc = 0
-        ret = os.popen("e au").readline()
+        ret = self.run("e au")
         if ret.find("Stopped") != -1:
             isstop = 1
         else:
             isstop = 0
         pc = int(ret.split(" ")[3].replace(":",""),16)
         return [isstop,pc]
         
         
     def tohex(self,d):
         return hex(d).replace("0x","")
             
     def get_mem_data(self,addr,len):
-        result = os.popen("e "+self.tohex(addr)+"l"+self.tohex(len)).readlines()
+        result = self.run("e "+self.tohex(addr)+"l"+self.tohex(len))
         odata=[]
         for line in result[1:]:
             for data in line.split(":")[1].strip().split(" "):
                 odata.append(int(data,16))
         return odata
     
     def get_byte(self,addr):
@@ -100,15 +117,15 @@
         return ret[0] + (ret[1] << 8)
 
     def get_dword(self,addr):
         ret = self.get_mem_data(addr,4)
         return ret[0] + (ret[1] << 8) + (ret[2] << 16) + (ret[3] << 24)
     
     def set_data(self,addr,data):
-        os.system("e "+self.tohex(addr)+" "+self.tohex(data))
+        self.run("e "+self.tohex(addr)+" "+self.tohex(data))
 
     def set_byte(self,addr,data):
         self.set_data(addr,("%02x" %data))
 
     def set_word(self,addr,data):
         self.set_data(addr,("%04x" %data))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg/f_excel.py` & `f_tools_pkg-0.0.8/f_tools_pkg/f_excel.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg/f_log.py` & `f_tools_pkg-0.0.8/f_tools_pkg/f_log.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg/f_serial.py` & `f_tools_pkg-0.0.8/f_tools_pkg/f_serial.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.7/f_tools_pkg.egg-info/PKG-INFO` & `f_tools_pkg-0.0.8/f_tools_pkg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f-tools-pkg
-Version: 0.0.7
+Version: 0.0.8
 Summary: some common tools(bmp/crypt/excel/log ...)
 Home-page: 
 Author: wushengyan
 Author-email: WUSY1991@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,8 +15,10 @@
 
 2022-7-20 V0.0.4  add bmp_scale function
 
 2024-3-27 V0.06  e bu add "type" parameter
 
 2024-4-10 v0.007 des3 key mast 24 Bytes, and 23:16 must not '0'
 
+2024-4-15 v0.008 command with timeout
+
```

### Comparing `f_tools_pkg-0.0.7/setup.py` & `f_tools_pkg-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='f_tools_pkg',
-    version='0.0.7',
+    version='0.0.8',
     packages=setuptools.find_packages(),
     url='',
     license='MIT',
     author='wushengyan',
     author_email='WUSY1991@163.com',
     description='some common tools(bmp/crypt/excel/log ...)',
     long_description=long_description,
```

