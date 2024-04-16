# Comparing `tmp/pyees-1.9.1.tar.gz` & `tmp/pyees-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.9.1.tar", last modified: Sun Mar 24 16:39:16 2024, max compression
+gzip compressed data, was "pyees-1.9.2.tar", last modified: Tue Apr 16 07:43:37 2024, max compression
```

## Comparing `pyees-1.9.1.tar` & `pyees-1.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 16:39:16.665794 pyees-1.9.1/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2024-03-24 16:39:16.667790 pyees-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-11-16 13:49:16.000000 pyees-1.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 16:39:16.565064 pyees-1.9.1/pyees/
--rw-rw-rw-   0        0        0      323 2023-11-15 09:47:38.000000 pyees-1.9.1/pyees/__init__.py
--rw-rw-rw-   0        0        0    20037 2024-03-23 12:45:30.000000 pyees-1.9.1/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.9.1/pyees/profileFit.py
--rw-rw-rw-   0        0        0      826 2024-03-09 09:00:50.000000 pyees-1.9.1/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    12238 2024-03-24 16:28:20.000000 pyees-1.9.1/pyees/prop.py
--rw-rw-rw-   0        0        0    20428 2024-03-20 14:17:49.000000 pyees-1.9.1/pyees/sheet.py
--rw-rw-rw-   0        0        0    15635 2024-03-16 17:14:51.000000 pyees-1.9.1/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.9.1/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0    16664 2024-03-23 12:35:23.000000 pyees-1.9.1/pyees/testFit.py
--rw-rw-rw-   0        0        0    19641 2024-03-24 16:39:07.000000 pyees-1.9.1/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2024-03-20 14:24:28.000000 pyees-1.9.1/pyees/testPyees.py
--rw-rw-rw-   0        0        0    19971 2024-03-18 06:28:49.000000 pyees-1.9.1/pyees/testSheet.py
--rw-rw-rw-   0        0        0    25381 2024-03-16 17:00:14.000000 pyees-1.9.1/pyees/testSolve.py
--rw-rw-rw-   0        0        0    15349 2024-03-21 13:07:42.000000 pyees-1.9.1/pyees/testUnit.py
--rw-rw-rw-   0        0        0    98903 2024-03-21 13:17:19.000000 pyees-1.9.1/pyees/testVariable.py
--rw-rw-rw-   0        0        0    47370 2024-03-23 12:56:29.000000 pyees-1.9.1/pyees/unit.py
--rw-rw-rw-   0        0        0    37537 2024-03-21 14:05:30.000000 pyees-1.9.1/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2024-03-24 16:39:16.653827 pyees-1.9.1/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2024-03-24 16:39:15.000000 pyees-1.9.1/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-03-24 16:39:15.000000 pyees-1.9.1/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 16:39:15.000000 pyees-1.9.1/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-03-24 16:39:15.000000 pyees-1.9.1/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-24 16:39:15.000000 pyees-1.9.1/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-24 16:39:16.676766 pyees-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1240 2024-03-24 16:39:13.000000 pyees-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:43:36.947712 pyees-1.9.2/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2024-04-16 07:43:36.963337 pyees-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-11-16 13:49:16.000000 pyees-1.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:43:35.932045 pyees-1.9.2/pyees/
+-rw-rw-rw-   0        0        0      323 2023-11-15 09:47:38.000000 pyees-1.9.2/pyees/__init__.py
+-rw-rw-rw-   0        0        0    19427 2024-04-16 06:56:58.000000 pyees-1.9.2/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.9.2/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      826 2024-03-09 09:00:50.000000 pyees-1.9.2/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    12238 2024-03-24 16:28:20.000000 pyees-1.9.2/pyees/prop.py
+-rw-rw-rw-   0        0        0    20428 2024-03-20 14:17:49.000000 pyees-1.9.2/pyees/sheet.py
+-rw-rw-rw-   0        0        0    15635 2024-03-16 17:14:51.000000 pyees-1.9.2/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.9.2/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0    16674 2024-04-16 06:59:08.000000 pyees-1.9.2/pyees/testFit.py
+-rw-rw-rw-   0        0        0    19641 2024-03-24 16:39:07.000000 pyees-1.9.2/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2024-04-16 07:19:32.000000 pyees-1.9.2/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    19971 2024-03-18 06:28:49.000000 pyees-1.9.2/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    25381 2024-03-16 17:00:14.000000 pyees-1.9.2/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    15347 2024-04-16 06:53:53.000000 pyees-1.9.2/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    99106 2024-04-16 06:59:36.000000 pyees-1.9.2/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    47786 2024-04-16 06:58:48.000000 pyees-1.9.2/pyees/unit.py
+-rw-rw-rw-   0        0        0    37564 2024-04-16 07:43:04.000000 pyees-1.9.2/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:43:36.713327 pyees-1.9.2/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2024-04-16 07:43:30.000000 pyees-1.9.2/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-16 07:43:31.000000 pyees-1.9.2/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:43:30.000000 pyees-1.9.2/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-16 07:43:30.000000 pyees-1.9.2/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 07:43:30.000000 pyees-1.9.2/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-16 07:43:37.072716 pyees-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2024-04-16 07:43:25.000000 pyees-1.9.2/setup.py
```

### Comparing `pyees-1.9.1/LICENSE.txt` & `pyees-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/PKG-INFO` & `pyees-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.9.1
+Version: 1.9.2
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.9.1/README.md` & `pyees-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/fit.py` & `pyees-1.9.2/pyees/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,19 +533,7 @@
         def getVariableUnits(self):
             return self.getVariableUnitsFunc(self.xUnit, self.yUnit)
 
     return newFit
 
 
 
-
-if __name__ == "__main__":
-
-    flow = variable([660.09423012, 632.43569693, 585.42024242, 522.76300061, 503.14430082, 447.93713197, 400.01585758], '1', [40.16979867, 39.40731403, 32.88129504, 25.96587423, 28.57373576, 20.87486404, 21.3429122])
-    dp = variable([227.49190451, 201.72024508, 171.5431791, 140.95368402, 125.08148975, 101.49530656, 82.13967787], '1', [2.60904033, 2.31367366, 2.39738832, 2.1452602, 1.83369048, 1.48646204, 1.33872491])
-
-    fit_dp1_2 = pol_fit(flow, dp)
-    print(*fit_dp1_2.coefficients)
-    x = variable(10)
-    out = fit_dp1_2.predict(x)
-    print(out)
-    exit()
```

### Comparing `pyees-1.9.1/pyees/profileFit.py` & `pyees-1.9.2/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/profilePyees.py` & `pyees-1.9.2/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/prop.py` & `pyees-1.9.2/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/sheet.py` & `pyees-1.9.2/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/solve.py` & `pyees-1.9.2/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/stackOverflowODR.py` & `pyees-1.9.2/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/testFit.py` & `pyees-1.9.2/pyees/testFit.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 
         F = pol_fit(x, y, deg=3)
         Fa = F.coefficients[0]
         Fb = F.coefficients[1]
         Fc = F.coefficients[2]
         Fd = F.coefficients[3]
         
+        
         self.assertAlmostEqual(Fa.value, 2)
         self.assertEqual(str(Fa.unit), 'DELTAC/m3')
 
         self.assertAlmostEqual(Fb.value, 10)
         self.assertEqual(str(Fb.unit), 'DELTAC/m2')
 
         self.assertAlmostEqual(Fc.value, 15)
```

### Comparing `pyees-1.9.1/pyees/testProp.py` & `pyees-1.9.2/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/testPyees.py` & `pyees-1.9.2/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/testSheet.py` & `pyees-1.9.2/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/testSolve.py` & `pyees-1.9.2/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.9.1/pyees/testUnit.py` & `pyees-1.9.2/pyees/testUnit.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,12 +404,11 @@
         converter = unit('Ra').getConverter('Rø')
         A = variable(83.1,'',1)
         converter(A)
         self.assertAlmostEqual(A.value, -111.66625)
         self.assertAlmostEqual(A.uncert,  0.29166666666666666666667)
         self.assertAlmostEqual(A._uncertSI, 1)
         
-
     
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyees-1.9.1/pyees/testVariable.py` & `pyees-1.9.2/pyees/testVariable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1200,27 +1200,31 @@
             (2**0.34 * np.log(2) * 0.01)**2 + (0.34 * 2**(0.34 - 1) * 0)**2))
 
     def testPrettyPrint(self):
         a = variable(12.3, 'm')
         b = variable(12.3, 'm', 2.5)
         c = variable([12.3, 56.2], 'm')
         d = variable([12.3, 56.2], 'm', [2.5, 7.3])
-
+        e = variable(12.3, 'DELTAC')
+        
         self.assertEqual(a.__str__(pretty=False), '12.3 [m]')
         self.assertEqual(b.__str__(pretty=False), '12 +/- 2 [m]')
         self.assertEqual(c.__str__(pretty=False), '[12.3, 56.2] [m]')
         self.assertEqual(d.__str__(pretty=False), '[12, 56] +/- [2, 7] [m]')
+        self.assertEqual(e.__str__(pretty=False), '12.3 [DELTAC]')
 
         self.assertEqual(a.__str__(pretty=True), '12.3\\ \\left [m\\right ]')
         self.assertEqual(b.__str__(pretty=True),
                          '12 \pm 2\\ \\left [m\\right ]')
         self.assertEqual(c.__str__(pretty=True),
                          '[12.3, 56.2]\\ \\left [m\\right ]')
         self.assertEqual(d.__str__(pretty=True),
                          '[12, 56] \pm [2, 7]\\ \\left [m\\right ]')
+        self.assertEqual(e.__str__(pretty=True), '12.3\\ \\left [\\Delta C\\right ]')
+
 
     def testMax(self):
 
         A = variable(10, 'm', 2.3)
         A = np.max(A)
         self.assertEqual(A.value, 10)
         self.assertEqual(A.unit, 'm')
```

### Comparing `pyees-1.9.1/pyees/unit.py` & `pyees-1.9.2/pyees/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -879,18 +879,30 @@
         
         # update unitStr
         unitStrPretty = unitStrPretty[0:currentParensPretty[0]] + _unitStrPretty + unitStrPretty[currentParensPretty[1]+1:]
         return unit._formatUnitStrPretty(unitStrPretty)
 
     @staticmethod
     def _unitStrPrettyPostProcessing(unitStrPretty):
+        ## replace 'left' with '\left'
         unitStrPretty = resub(r'(?<!\\)\\right', r'\\right)', unitStrPretty)
+        
+        ## replace 'right' with '\right'
         unitStrPretty = resub(r'(?<!\\)\\left', r'\\left(', unitStrPretty)
+        
+        ## replace '%' with '\%'
         unitStrPretty = resub(r'(?<!\\)%', r'\%', unitStrPretty)
-        return resub(r'(?<!\{)(?<!\\{)(\d+)(?=\}|\D|$)', r'^{\1}', unitStrPretty)
+        
+        ## replace 'exp' with '^{exp}' if the exponent is not 1. Else remove the exponent
+        unitStrPretty = resub(r'(?<!\{)(?<!\\{)(\d+)(?=\}|\D|$)', r'^{\1}', unitStrPretty)
+     
+        ## replace 'DELTA' with '\DELTA '
+        unitStrPretty = resub(r'(?<!/)DELTA', r'\\Delta ', unitStrPretty)
+        
+        return unitStrPretty
      
     @ staticmethod
     def _removeExponentFromUnit(u):
 
         integerIndexes = [i for i, char in enumerate(u) if char in integers]
 
         if not integerIndexes:
@@ -1262,9 +1274,9 @@
         if u == 'dec':
             return _bellConversion()
 
         raise ValueError(f'The logarithmic conversion of {u} is not knwon')
 
 
 if __name__ == "__main__":
-    a = unit('%')
+    a = unit('DELTAK')
     print(a.unitStrPretty)
```

### Comparing `pyees-1.9.1/pyees/variable.py` & `pyees-1.9.2/pyees/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,18 +827,20 @@
     def __len__(self):
         return len(self.scalarVariables)
 
     def __getitem__(self, index):
 
         if isinstance(index, int) or isinstance(index, np.integer):
             return self.scalarVariables[index]
-        elif isinstance(index, slice):
+        if isinstance(index, slice):
             return arrayVariable(scalarVariables=self.scalarVariables[index])
         if isinstance(index, list):
             return arrayVariable(scalarVariables=[self.scalarVariables[elem] for elem in index])
+        if isinstance(index, np.ndarray):
+            return arrayVariable(scalarVariables=[self.scalarVariables[elem] for elem in index])            
         else:
             raise NotImplementedError()
 
     @property
     def value(self):
         return np.array([elem.value for elem in self.scalarVariables])
 
@@ -1115,12 +1117,7 @@
                     'The lenght of the value has to be equal to the lenght of the uncertanty')
 
     if isinstance(value, np.ndarray):
         return arrayVariable(value=value, unitStr=unit, uncert=uncert)
     else:
         return scalarVariable(value, unit, uncert)
 
-if __name__ == "__main__":
-    a = variable(10, 'C', 1.2)
-    b = variable(100, 'muC', 3.9)
-    c = a - b
-    print(c)
```

### Comparing `pyees-1.9.1/pyees.egg-info/PKG-INFO` & `pyees-1.9.2/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.9.1
+Version: 1.9.2
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.9.1/setup.py` & `pyees-1.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.9.1',
+    version='1.9.2',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

