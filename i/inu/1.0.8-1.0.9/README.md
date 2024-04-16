# Comparing `tmp/inu-1.0.8.tar.gz` & `tmp/inu-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inu-1.0.8.tar", last modified: Wed Nov 22 20:45:49 2023, max compression
+gzip compressed data, was "inu-1.0.9.tar", last modified: Thu Dec 14 20:17:22 2023, max compression
```

## Comparing `inu-1.0.8.tar` & `inu-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-11-22 20:45:49.235972 inu-1.0.8/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2023-09-06 19:38:32.000000 inu-1.0.8/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2283 2023-11-22 20:45:49.235917 inu-1.0.8/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1829 2023-11-22 20:35:05.000000 inu-1.0.8/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 inu-1.0.8/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2023-11-22 20:45:49.236196 inu-1.0.8/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-11-22 20:45:49.233534 inu-1.0.8/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-11-22 20:45:49.234838 inu-1.0.8/src/inu/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-09-06 20:09:43.000000 inu-1.0.8/src/inu/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    24308 2023-11-22 20:45:17.000000 inu-1.0.8/src/inu/inu.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3368 2023-11-22 20:33:09.000000 inu-1.0.8/src/inu/test_inu.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-11-22 20:45:49.235748 inu-1.0.8/src/inu.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2283 2023-11-22 20:45:49.000000 inu-1.0.8/src/inu.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2023-11-22 20:45:49.000000 inu-1.0.8/src/inu.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2023-11-22 20:45:49.000000 inu-1.0.8/src/inu.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2023-11-22 20:45:49.000000 inu-1.0.8/src/inu.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2023-11-22 20:45:49.000000 inu-1.0.8/src/inu.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.792895 inu-1.0.9/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2023-09-06 19:38:32.000000 inu-1.0.9/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     2283 2023-12-14 20:17:22.792842 inu-1.0.9/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1829 2023-11-22 20:35:05.000000 inu-1.0.9/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 inu-1.0.9/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2023-12-14 20:17:22.793103 inu-1.0.9/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.790426 inu-1.0.9/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.791859 inu-1.0.9/src/inu/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-09-06 20:09:43.000000 inu-1.0.9/src/inu/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    24594 2023-12-14 20:16:28.000000 inu-1.0.9/src/inu/inu.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3381 2023-12-14 19:50:22.000000 inu-1.0.9/src/inu/test_inu.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 20:17:22.792660 inu-1.0.9/src/inu.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     2283 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2023-12-14 20:17:22.000000 inu-1.0.9/src/inu.egg-info/top_level.txt
```

### Comparing `inu-1.0.8/LICENSE.txt` & `inu-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inu-1.0.8/PKG-INFO` & `inu-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inu
-Version: 1.0.8
+Version: 1.0.9
 Summary: Inertial Navigation Utilities
 Home-page: https://gitlab.com/davidwoodburn/inu
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inu-1.0.8/README.md` & `inu-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `inu-1.0.8/setup.cfg` & `inu-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inu
-version = 1.0.8
+version = 1.0.9
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Inertial Navigation Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/inu
 classifiers =
```

### Comparing `inu-1.0.8/src/inu/inu.py` & `inu-1.0.9/src/inu/inu.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Cleared for public release: 88ABW-2023-0793
+Distribution Statement A: Approved for public release; distribution unlimited.
 --------------------------------------------------------------------------------
 
 Functions
 ---------
 This library provides forward mechanization of inertial measurement unit sensor
 values (accelerometer and gyroscope readings) to get position, velocity, and
 attitude as well as inverse mechanization to get sensor values from position,
@@ -56,15 +56,15 @@
 vectors, each with 3 elements. If an input matrix does not have 3 rows, it will
 be assumed that the rows of the matrix are vectors.
 --------------------------------------------------------------------------------
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2023-11-22"
+__date__ = "2023-12-14"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import math
 import numpy as np
 
@@ -314,29 +314,35 @@
 
     Returns
     -------
     theta : (3,) np.ndarray
         Three-element vector of angles in radians.
     """
 
-    # Get the trace of the matrix.
+    # Get the trace of the matrix and limit its value.
     q = Delta[0, 0] + Delta[1, 1] + Delta[2, 2]
-    q = q if q <= 3 else 3 # limit
+    q_min = 2*np.cos(3.1415926) + 1
+    q = max(min(q, 3.0), q_min)
 
     # Get the scaling factor of the vector.
     ang = math.acos((q-1)/2)
     s = ang/math.sqrt(3 + 2*q - q**2) if (q <= 2.9996) \
             else (q**2 - 11*q + 54)/60
 
     # Build the vector.
     theta = s*np.array([
         Delta[2, 1] - Delta[1, 2],
         Delta[0, 2] - Delta[2, 0],
         Delta[1, 0] - Delta[0, 1]])
 
+    # Check the output.
+    if q == q_min:
+        raise ValueError("The provided output is incorrectly all zeros \n"
+                + "because the input is very close to a 180 degree rotation.")
+
     return theta
 
 
 def est_wind(vne_t, yaw_t):
     """
     Estimate the time-varying wind by comparing the ground travel velocity to
     the yaw (heading) angle.
```

### Comparing `inu-1.0.8/src/inu/test_inu.py` & `inu-1.0.9/src/inu/test_inu.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,7 +121,9 @@
     hfbbi, hwbbi = inu.inv_mech(llh, vne, rpy, T)
     tllh, tvne, trpy = inu.mech(hfbbi, hwbbi,
         llh[0, :], vne[0, :], rpy[0, :], T)
 
     assert np.allclose(llh, tllh)
     assert np.allclose(vne, tvne)
     assert np.allclose(rpy, trpy)
+
+test_mech()
```

### Comparing `inu-1.0.8/src/inu.egg-info/PKG-INFO` & `inu-1.0.9/src/inu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inu
-Version: 1.0.8
+Version: 1.0.9
 Summary: Inertial Navigation Utilities
 Home-page: https://gitlab.com/davidwoodburn/inu
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

