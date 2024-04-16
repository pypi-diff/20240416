# Comparing `tmp/All-in-one-chay-2.4.6.tar.gz` & `tmp/all_in_one_chay-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "All-in-one-chay-2.4.6.tar", last modified: Sat Apr  6 13:39:08 2024, max compression
+gzip compressed data, was "all_in_one_chay-2.4.7.tar", last modified: Tue Apr 16 15:21:28 2024, max compression
```

## Comparing `All-in-one-chay-2.4.6.tar` & `all_in_one_chay-2.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.255291 All-in-one-chay-2.4.6/
--rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 All-in-one-chay-2.4.6/LICENSE
--rw-rw-rw-   0        0        0     1857 2024-04-06 13:39:08.254290 All-in-one-chay-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2024-03-29 15:06:20.000000 All-in-one-chay-2.4.6/README.md
--rw-rw-rw-   0        0        0      622 2024-04-06 13:37:57.000000 All-in-one-chay-2.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 13:39:08.255291 All-in-one-chay-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-04-06 13:38:46.000000 All-in-one-chay-2.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.233292 All-in-one-chay-2.4.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.239291 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/
--rw-rw-rw-   0        0        0     9380 2024-04-06 13:37:26.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/Allinone.py
--rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.247291 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/
--rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/book.py
--rw-rw-rw-   0        0        0    10521 2024-04-06 13:34:53.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/calculator.py
--rw-rw-rw-   0        0        0      876 2024-04-05 15:36:03.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
--rw-rw-rw-   0        0        0     1695 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/math_cal_py.py
--rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/student_py.py
--rw-rw-rw-   0        0        0     6957 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/tuxing_cal.py
--rw-rw-rw-   0        0        0     2804 2024-04-06 01:29:46.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/xiaogongju.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.253292 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/
--rw-rw-rw-   0        0        0     1857 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/
+-rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0     4906 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4269 2024-04-16 15:17:42.000000 all_in_one_chay-2.4.7/README.md
+-rw-rw-rw-   0        0        0      622 2024-04-16 15:01:00.000000 all_in_one_chay-2.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-04-16 15:00:52.000000 all_in_one_chay-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.931221 all_in_one_chay-2.4.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.931221 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/
+-rw-rw-rw-   0        0        0     9572 2024-04-16 15:12:54.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/Allinone.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/
+-rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/book.py
+-rw-rw-rw-   0        0        0    11629 2024-04-16 15:07:24.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/calculator.py
+-rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+-rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/math_cal_py.py
+-rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/student_py.py
+-rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/tuxing_cal.py
+-rw-rw-rw-   0        0        0     2804 2024-04-16 15:08:27.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/xiaogongju.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/
+-rw-rw-rw-   0        0        0     4906 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/top_level.txt
```

### Comparing `All-in-one-chay-2.4.6/LICENSE` & `all_in_one_chay-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.6/pyproject.toml` & `all_in_one_chay-2.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "All-in-one-chay"
-version = "2.4.6"
+version = "2.4.7"
 authors = [
   { name="chay", email="lichenyi_2020@qq.com" },
 ]
 description = "多功能一体机（All-in-one）"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6"
+Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7"
 Issues = "https://github.com/lichenyichay/All-in-one/issues"
```

### Comparing `All-in-one-chay-2.4.6/setup.py` & `all_in_one_chay-2.4.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding:UTF-8
 import setuptools
 
 setuptools.setup(
     name="All-in-one-chay",
-    version="2.4.6",
+    version="2.4.7",
     author="Chay",
     author_email="lichenyi_2020@qq.com",
-    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6",
+    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7",
     description="All-in-one",
     long_description="多功能一体机",
     python_requires=">=3.5",
     # packages=setuptools.find_packages("src"),
     packages_dir={"": "src"},
     packages_data={"": ["*.txt", "*.info", "*.properties"], "": ["data/*.*"]},
     exclude=["*.test", "*.test.*", "test.*", "test"],
```

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/Allinone.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/Allinone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding:UTF-8 -*-
 # @Author:Chay
-# @TIME:2024/3/29 22:55
+# @TIME:2024/4/16 23:04
 # @FILE:Allinone.py
-# @version:2.4.4
+# @version:2.4.7
 # @Software:Visual Studio Code
 import math,random
-
 import module.book as book
 import module.calculator as calculator
 import module.erfenchazhao_py  as erfenchazhao_py
 import module.math_cal_py as math_cal
 import module.student_py as student_py
 import module.tuxing_cal as tuxing_cal
 import module.xiaogongju as xiaogongju
@@ -70,14 +69,18 @@
         return calculator.wanquanpingfangshu(args[0])
     elif fuwu=="判断完全平方数":
         return calculator.iswanquanpingfangshu(args[0])
     elif fuwu=="判断斐波那契完全平方数":
         return calculator.isfabwanquanpingfangshu(args[0])
     elif fuwu=="判断泰波那契序列完全平方数":
         return calculator.istribonacciwanquanpingfangshu(args[0])
+    elif fuwu == "进制转换":
+        return calculator.jinzhizhuanhuan(args[0],args[1],args[2])
+    elif fuwu=="math库计算器":
+        return math_cal.math_cal(mode,args[0],args[1])
     elif fuwu == "图形计算器":
         while True:
             huida = args[0]
             try:
                 args2=[]
                 for i in range(1,len(args)):
                     args2.append(args[i])
```

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/book.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/book.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/calculator.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding:UTF-8 -*-
 # @Author:Chay
-# @TIME:2024/3/29 22:55
+# @TIME:2024/4/16 23:07
 # @FILE:calculator.py
 # @Software:Visual Studio Code
 import math
 '''
 函数名：FtemporCtemp
 调用形式：a = FtemporCtemp(mode,FtemporCtemp)
 :param mode 模式 ℃to℉（摄氏度转为华氏度）/℉to℃（华氏度转为摄氏度） 模式不在选择范围内会抛出异常
@@ -358,8 +358,47 @@
 函数名：istribonacciwanquanpingfangshu
 调用形式：a = istribonacciwanquanpingfangshu(d)
 :param x  类型：int
 :return x 是否是泰波那契序列完全平方数（True or False）
 作用：判断泰波那契序列完全平方数
 '''
 def istribonacciwanquanpingfangshu(num:int) -> bool:
-    return istribonacci(num) and iswanquanpingfangshu(num)
+    return istribonacci(num) and iswanquanpingfangshu(num)
+
+'''
+函数名：jinzhizhuanhuan
+调用形式：a =  jinzhizhuanhuan(a,b,c)
+:param a c的进制数 (2<=a<=36)
+:param b 结果的进制数 (2<=a<=36)
+:param c 需转换的数 无需前缀且需符合a进制规则
+:return z 结果
+'''
+def jinzhizhuanhuan(a:int,b:int,c:str) -> str:
+    if a == b:
+        return c
+    elif a == 10  and b != 10:
+        num = int(c)  
+        result = ""  
+        while num > 0:  
+            remainder = num % b  
+            if remainder >= 10:  
+                result += chr(remainder - 10 + ord('A'))  
+            else:  
+                result += str(remainder)  
+            num //= b
+        return result[::-1] 
+    elif a != 10 and b == 10:
+        ans=0
+        tmp=1
+        n=len(c)
+        for i in range(n-1,-1,-1):
+            base = 0
+            if c[i] >= 'A' and c[i] <= 'Z':
+                base = c[i]-'A'+10
+            else:
+                base = ord(c[i])-ord('0')
+            ans += tmp*base
+            tmp *= a
+        return str(ans)
+
+    else:
+        return jinzhizhuanhuan(10,b,jinzhizhuanhuan(a,10,c))
```

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/math_cal_py.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/math_cal_py.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 函数名：math_cal
 调用形式：s = math_cal(mode,float1,float2)
 :param mode 模式 1~19 模式不在此选择范围内会抛出异常
 :param float1 float2 float型参数，根据模式的需求，如参数有空余，则空余参数添0即可，例：mode = 3:math_cal(3,5.2,0);
 例2：mode = 4:math_cal(4,0,0);例3：mode = 1:math_cal(1,5.92,-8)
 :return 结果
 '''
-def math_cal(mode,float1,float2):
+def math_cal(mode:int,float1:float,float2:float):
     if mode == 1:
         return math.copysign(float1,float2)
     elif mode == 2:
         return math.cos(float1)
     elif mode == 3:
         return math.degrees(float1)
     elif mode == 4:
```

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/student_py.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/student_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/tuxing_cal.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/tuxing_cal.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '''
 函数名：tuxing
 调用形式：tuxing(huida)
 :param huida 图形
 :return 0
 作用：进行图形计算
 '''
-from math import pi
+import math
 def tuxing(huida,mode,*args2):
     while True:
         if huida == "长方体":
             huida1 = mode   #体积/面积/表面积/染色问题/容积/棱长总和
             huida2 = args2[0]
             huida3 = args2[1]
             huida4 = args2[2]
```

### Comparing `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/xiaogongju.py` & `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/xiaogongju.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/SOURCES.txt` & `all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

