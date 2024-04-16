# Comparing `tmp/r3f-2.0.2.tar.gz` & `tmp/r3f-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3f-2.0.2.tar", last modified: Thu Dec 14 19:27:08 2023, max compression
+gzip compressed data, was "r3f-2.0.3.tar", last modified: Tue Apr 16 02:54:55 2024, max compression
```

## Comparing `r3f-2.0.2.tar` & `r3f-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 19:27:08.285064 r3f-2.0.2/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2022-05-06 23:09:16.000000 r3f-2.0.2/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2023-12-14 19:27:08.285015 r3f-2.0.2/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4320 2023-10-19 22:37:17.000000 r3f-2.0.2/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 r3f-2.0.2/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      607 2023-12-14 19:27:08.285283 r3f-2.0.2/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 19:27:08.281915 r3f-2.0.2/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 19:27:08.283802 r3f-2.0.2/src/r3f/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2022-05-27 17:40:46.000000 r3f-2.0.2/src/r3f/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)   101927 2023-12-14 19:25:42.000000 r3f-2.0.2/src/r3f/r3f.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19785 2023-12-14 19:22:14.000000 r3f-2.0.2/src/r3f/test_r3f.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-14 19:27:08.284845 r3f-2.0.2/src/r3f.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2023-12-14 19:27:08.000000 r3f-2.0.2/src/r3f.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2023-12-14 19:27:08.000000 r3f-2.0.2/src/r3f.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2023-12-14 19:27:08.000000 r3f-2.0.2/src/r3f.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2023-12-14 19:27:08.000000 r3f-2.0.2/src/r3f.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2023-12-14 19:27:08.000000 r3f-2.0.2/src/r3f.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.713215 r3f-2.0.3/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2022-05-06 23:09:16.000000 r3f-2.0.3/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-04-16 02:54:55.713159 r3f-2.0.3/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4320 2023-10-19 22:37:17.000000 r3f-2.0.3/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 r3f-2.0.3/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      607 2024-04-16 02:54:55.713438 r3f-2.0.3/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.710770 r3f-2.0.3/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.711910 r3f-2.0.3/src/r3f/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2022-05-27 17:40:46.000000 r3f-2.0.3/src/r3f/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)   101759 2024-04-12 15:53:17.000000 r3f-2.0.3/src/r3f/r3f.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19785 2023-12-14 19:22:14.000000 r3f-2.0.3/src/r3f/test_r3f.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-16 02:54:55.713000 r3f-2.0.3/src/r3f.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-16 02:54:55.000000 r3f-2.0.3/src/r3f.egg-info/top_level.txt
```

### Comparing `r3f-2.0.2/LICENSE.txt` & `r3f-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `r3f-2.0.2/PKG-INFO` & `r3f-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3f
-Version: 2.0.2
+Version: 2.0.3
 Summary: A library for three-dimensional, reference-frame conversions
 Home-page: https://gitlab.com/davidwoodburn/r3f
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `r3f-2.0.2/README.md` & `r3f-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `r3f-2.0.2/setup.cfg` & `r3f-2.0.3/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = r3f
-version = 2.0.2
+version = 2.0.3
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for three-dimensional, reference-frame conversions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/r3f
 classifiers =
```

### Comparing `r3f-2.0.2/src/r3f/r3f.py` & `r3f-2.0.3/src/r3f/r3f.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Cleared for public release: 88ABW-2023-0793
+Distribution Statement A. Approved for public release: distribution unlimited.
 --------------------------------------------------------------------------------
 
 Functions
 ---------
-This library includes four sets of functions: general array checks,
-attitude-representation conversions, reference-frame conversions, and rotation
-matrix (direction cosine matrix) utilities.
+This library includes four sets of functions: general array checks, attitude-
+representation conversions, reference-frame conversions, and rotation matrix
+(direction cosine matrix) utilities.
 
 All twenty possible conversions among the following five attitude
 representations are provided: rotation vector, rotation axis and angle, roll and
 pitch and yaw (RPY) Euler angles, direction cosine matrix (DCM), and quaternion.
 However, some of the conversions are built using other conversions. In the
 following table, the low-level conversions are marked with an `x` and the
 conversions build using the other conversions are marked with an `o`:
@@ -109,15 +109,15 @@
 not conform to the ideal type and shape. Generally, the allowed types are int,
 float, list, and np.ndarray.
 --------------------------------------------------------------------------------
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2023-12-14"
+__date__ = "2024-04-12"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import numpy as np
 
 # WGS84 constants (IS-GPS-200M and NIMA TR8350.2)
@@ -525,18 +525,18 @@
         x y (1 - cos(ang)) - z sin(ang)
 
     Through these simplifications the `C` can be redefined as
 
             .-         2                                     -.
             |    co + x cc     x y cc + z si   x z cc - y si  |
             |                                                 |
-            |                           2                     |
+            |                          2                      |
         C = |  x y cc - z si     co + y cc     y z cc + x si  |
             |                                                 |
-            |                                            2    |
+            |                                          2      |
             |  x z cc + y si   y z cc - x si     co + z cc    |
             '-                                               -'
 
     where `co` is the cosine of the angle, `si` is the sine of the angle, and
     `cc` is the compelement of the cosine: `(1 - co)`.
 
     Before the algorithm described above is applied, the `ax` input is first
@@ -576,15 +576,15 @@
     that we might use when the input is actually a DCM.
 
     Putting this together, the `ax` vector is normalized and its norm applied to
     the angle:
 
                 .-----------------
                /   2      2      2
-        nm = |/ ax1  + ax2  + ax3
+        nm = `/ ax1  + ax2  + ax3
 
              ax1             ax2
         x = -----       y = -----
              nm              nm
 
              ax3
         z = -----       ang = ang nm .
@@ -696,22 +696,22 @@
         q = a + b i + c j + d k
 
     where `q` is the quaternion and `ax` is the rotation axis vector. Then, the
     norm of [b, c, d] will be
 
            .-----------       .---------------------------
           / 2    2    2      /  2    2    2     2.- ang -.       .- ang -.
-        |/ b  + c  + d  =   / (x  + y  + z ) sin | ----- | = sin | ----- | .
-                          |/                     '-  2  -'       '-  2  -'
+        `/ b  + c  + d  =   / (x  + y  + z ) sin | ----- | = sin | ----- | .
+                          `/                     '-  2  -'       '-  2  -'
 
     Since a = cos(ang/2), with the above value, we can calculate the angle by
 
                             .-   .-----------    -.
                             |   / 2    2    2     |
-        ang = 2 sgn arctan2 | |/ b  + c  + d  , a | ,
+        ang = 2 sgn arctan2 | `/ b  + c  + d  , a | ,
                             '-                   -'
 
     where `sgn` is the sign of the angle based on whether the dot product of the
     vector [b, c, d] with [1, 1, 1] is positive:
 
         sgn = sign( b + c + d ) .
 
@@ -897,22 +897,22 @@
                                             c = y sin( ang/2 )
                                             d = z sin( ang/2 ) .
 
     The norm of [b, c, d]' would be
 
            .-----------       .---------------------------
           / 2    2    2      /  2    2    2     2
-        |/ b  + c  + d  =  |/ (x  + y  + z ) sin ( ang/2 ) = sin( ang/2 ) ,
+        `/ b  + c  + d  =  `/ (x  + y  + z ) sin ( ang/2 ) = sin( ang/2 ) ,
 
     where [x, y, z]' is a unit vector by design. Since a = cos(ang/2), with the
     above value we can calculate the angle by
 
                             .-   .-----------   -.
                             |   / 2    2    2    |
-        ang = 2 sgn arctan2 | |/ b  + c  + d , a | ,
+        ang = 2 sgn arctan2 | `/ b  + c  + d , a | ,
                             '-                  -'
 
     where sgn is the sign of the angle based on whether the dot product of the
     vector [b, c, d]' with [1, 1, 1]' is positive:
 
         sgn = sign( b + c + d ) .
 
@@ -1079,24 +1079,21 @@
           = |  (cy sp sr - sy cr)  (sy sp sr + cy cr)  (cp sr)  |
             |  (sy sr + cy sp sr)  (sy sp cr - cy sr)  (cp cr)  |
             '-                                                 -'
 
     where `c` and `s` mean cosine and sine, respectively, and `r`, `p`, and `y`
     mean roll, pitch, and yaw, respectively, then we can see that
 
-                                        .-       -.
-                                        |  cp sr  |
+                                        .- cp sr -.
         r = arctan2(c23, c33) => arctan | ------- |
-                                        |  cp cr  |
-                                        '-       -'
-                                        .-       -.
-                                        |  sy cp  |
+                                        '- cp cr -'
+
+                                        .- sy cp -.
         y = arctan2(c12, c11) => arctan | ------- |
-                                        |  cy cp  |
-                                        '-       -'
+                                        '- cy cp -'
 
     where the cp values cancel in both cases. The value for pitch could be found
     from c13 alone:
 
         p = arcsin(-c13)
 
     However, this tends to suffer from numerical error around +- pi/2. So,
@@ -1105,15 +1102,15 @@
           2     2               2     2
         cy  + sy  = 1   and   cr  + sr  = 1 .
 
     Therefore, we can use the fact that
 
            .------------------------
           /   2      2      2      2     .--
-        |/ c11  + c12  + c23  + c33  = |/ 2  cos( |p| )
+        `/ c11  + c12  + c23  + c33  = `/ 2  cos( |p| )
 
     to solve for pitch. We can use the negative of the sign of c13 to give the
     proper sign to pitch. The advantage is that in using more values from the
     DCM matrix, we can can get a value which is more accurate. This works well
     until we get close to a pitch value of zero. Then, the simple formula for
     pitch is actually better. So, we will use both and do a weighted average of
     the two, based on pitch.
@@ -1797,26 +1794,26 @@
         re = |  ---- + hae | cos(lat)
              '- klat      -'
 
     where `aE` is the semi-major radius of the earth and
 
                   .---------------
                  /      2   2
-        klat = |/ 1 - eE sin (lat)
+        klat = `/ 1 - eE sin (lat)
 
     The `eE` value is the eccentricity of the earth. Knowing the distance from
     the z axis, we can get the x and y coordinates:
 
         xe = re cos(lon)            ye = re sin(lon) .
 
     The z-axis coordinate is
 
-             .-  aE         2        -.
-        ze = |  ---- (1 - eE ) + hae  | sin(lat) .
-             '- klat                 -'
+             .-  aE         2       -.
+        ze = |  ---- (1 - eE ) + hae | sin(lat) .
+             '- klat                -'
 
     The output vector `pe` is made up of `xe`, `ye`, and `ze`: [xe, ye, ze].
 
     Several of these equations are admittedly not intuitively obvious. The
     interested reader should refer to external texts for insight.
 
     References
@@ -1897,15 +1894,15 @@
 
     First, we want to approximate the values for geodetic latitude, `lat`, and
     height above ellipsoid, `hae`, given the pe = [xe, ye, ze] position in the
     ECEF frame:
 
                                 .--------
          ^                     /  2     2            ^
-        hae = 0         re = |/ xe  + ye            lat = arctan2(ze, re),
+        hae = 0         re = `/ xe  + ye            lat = arctan2(ze, re),
 
     where `re` is the distance from the z axis of the ECEF frame. (While there
     are better approximations for `hae` than zero, the improvement in accuracy
     was not enough to reduce the number of iterations and the additional
     computational burden could not be justified.)  Then, we will iteratively use
     this approximation for `lat` and `hae` to calculate what `re` and `ze` would
     be, get the residuals given the correct `re` and `ze` values in the ECEF
@@ -1915,17 +1912,17 @@
     iterations was sufficient to reach the limit of numerical precision for
     64-bit floating-point numbers.
 
     So, first, let us define the transverse, `Rt`, and meridional, `Rm`, radii
     and the cosine and sine of the latitude:
 
                                                               .---------------
-              aE               aE  .-       2 -.             /      2   2  ^
-        Rt = ----       Rm = ----- |  1 - eE   |    klat = |/ 1 - eE sin (lat) ,
-             klat                3 '-         -'
+              aE               aE  .-      2 -.              /      2   2  ^
+        Rt = ----       Rm = ----- | 1 - eE   |     klat = `/ 1 - eE sin (lat) ,
+             klat                3 '-        -'
                              klat
                   ^                               ^
         co = cos(lat)                   si = sin(lat)
 
     where `eE` is the eccentricity of the Earth, and `aE` is the semi-major
     radius of the Earth. The ECEF-frame `re` and `ze` values given the
     approximations to geodetic latitude and height above ellipsoid are
@@ -2505,17 +2502,17 @@
         | zc |   |           (hae - hae0)           |
         '-  -'   '-                                -'
 
     where
 
                                        2                .---------------
               aE             aE (1 - eE )              /      2   2
-        Rt = ----       Rm = ------------     klat = |/ 1 - eE sin (lat) .
-             klat                  3
-                               klat
+        Rt = ----       Rm = ------------     klat = `/ 1 - eE sin (lat) .
+             klat                    3
+                                 klat
 
     Here, `aE` is the semi-major axis of the Earth, `eE` is the eccentricity of
     the Earth, `Rt` is the transverse radius of curvature of the Earth, and `Rm`
     is the meridional radius of curvature of the Earth. Unfortunately, the
     reverse process to get geodetic coordinates from curvilinear coordinates is
     not as straightforward. So the Newton-Raphson method is used. Using NED as
     an example, with the above equations, we can write the differential relation
@@ -2715,15 +2712,15 @@
         '-  -'   '-                                -'
 
     where
 
 
                                        2                  .---------------
               aE             aE (1 - eE )                /      2   2
-        Rt = ----       Rm = ------------       klat = |/ 1 - eE sin (lat) .
+        Rt = ----       Rm = ------------       klat = `/ 1 - eE sin (lat) .
              klat                  3
                                klat
 
     Here, `aE` is the semi-major axis of the Earth, `eE` is the eccentricity of
     the Earth, `Rt` is the transverse radius of curvature of the Earth, and `Rm`
     is the meridional radius of curvature of the Earth.
 
@@ -3014,24 +3011,22 @@
     --------
     inverse_rodrigues_rotation
 
     Notes
     -----
     The Rodrigues Rotation formula is
 
-                                        sin(l)            1 - cos(l)        2
-        Delta = exp( [ theta ]x ) = I + ------ [theta]x + ---------- [theta]x,
-                                          l                    2
-                                                              l
-
+                                    sin(l)            1 - cos(l)        2
+        Delta = exp([theta] ) = I + ------ [theta]  + ---------- [theta] ,
+                           x          l           x        2            x
+                                                          l
     where
-
                .---------                  .-          -.           .-   -.
               / 2   2   2                  |  0  -z   y |           |  x  |
-        l = |/ x + y + z ,      [theta]x = |  z   0  -x |   theta = |  y  |.
+        l = `/ x + y + z ,      [theta]x = |  z   0  -x |   theta = |  y  |.
                                            | -y   x   0 |           |  z  |
                                            '-          -'           '-   -'
 
     The two trigonometric fractions become indeterminate when `l` is zero. While
     it is unlikely the vector magnitude `l` would ever become exactly zero, as
     the magnitude gets very small, there can be numerical problems. We need the
     limit of these terms as `l` approaches zero:
@@ -3051,24 +3046,24 @@
     the same as the negative of the rotation vector to the same matrix.
     """
 
     # Check the input.
     if isinstance(theta, (list, tuple)):
         theta = np.array(theta)
     trs = (theta.ndim == 2 and theta.shape[0] != 3)
-    s = np.pi/180 if degs else 1.0
+    sgn = np.pi/180 if degs else 1.0
 
     # Transpose input.
     if trs:
         theta = theta.T
 
     # Parse input.
-    x = theta[0]*s
-    y = theta[1]*s
-    z = theta[2]*s
+    x = theta[0]*sgn
+    y = theta[1]*sgn
+    z = theta[2]*sgn
 
     # Get the vector norm.
     x2 = x**2
     y2 = y**2
     z2 = z**2
     nm2 = x2 + y2 + z2
     nm = np.sqrt(nm2)
```

### Comparing `r3f-2.0.2/src/r3f/test_r3f.py` & `r3f-2.0.3/src/r3f/test_r3f.py`

 * *Files identical despite different names*

### Comparing `r3f-2.0.2/src/r3f.egg-info/PKG-INFO` & `r3f-2.0.3/src/r3f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3f
-Version: 2.0.2
+Version: 2.0.3
 Summary: A library for three-dimensional, reference-frame conversions
 Home-page: https://gitlab.com/davidwoodburn/r3f
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

