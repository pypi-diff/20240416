# Comparing `tmp/healpix-2023.4.tar.gz` & `tmp/healpix-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healpix-2023.4.tar", last modified: Tue Feb  6 11:23:02 2024, max compression
+gzip compressed data, was "healpix-2024.1.tar", last modified: Tue Apr 16 08:15:19 2024, max compression
```

## Comparing `healpix-2023.4.tar` & `healpix-2024.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:23:02.802382 healpix-2023.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-06 11:22:53.000000 healpix-2023.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 11:22:53.000000 healpix-2023.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-06 11:23:02.802382 healpix-2023.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-06 11:22:53.000000 healpix-2023.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-06 11:22:53.000000 healpix-2023.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:23:02.798382 healpix-2023.4/python/
--rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-02-06 11:22:53.000000 healpix-2023.4/python/chealpix.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:23:02.798382 healpix-2023.4/python/healpix/
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-02-06 11:22:53.000000 healpix-2023.4/python/healpix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:23:02.802382 healpix-2023.4/python/healpix/test/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-06 11:22:53.000000 healpix-2023.4/python/healpix/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-06 11:22:53.000000 healpix-2023.4/python/healpix/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-02-06 11:22:53.000000 healpix-2023.4/python/healpix/test/test_chealpix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-02-06 11:22:53.000000 healpix-2023.4/python/healpix/test/test_healpix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:23:02.802382 healpix-2023.4/python/healpix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-06 11:23:02.000000 healpix-2023.4/python/healpix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-06 11:23:02.000000 healpix-2023.4/python/healpix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 11:23:02.000000 healpix-2023.4/python/healpix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-06 11:23:02.000000 healpix-2023.4/python/healpix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 11:23:02.000000 healpix-2023.4/python/healpix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-06 11:23:02.802382 healpix-2023.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-06 11:22:53.000000 healpix-2023.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:23:02.802382 healpix-2023.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-02-06 11:22:53.000000 healpix-2023.4/src/healpix.c
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-02-06 11:22:53.000000 healpix-2023.4/src/healpix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:15:19.416199 healpix-2024.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-16 08:15:15.000000 healpix-2024.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 08:15:15.000000 healpix-2024.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-16 08:15:19.416199 healpix-2024.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-16 08:15:15.000000 healpix-2024.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-16 08:15:15.000000 healpix-2024.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:15:19.412199 healpix-2024.1/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    30451 2024-04-16 08:15:15.000000 healpix-2024.1/python/chealpix.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:15:19.412199 healpix-2024.1/python/healpix/
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-16 08:15:15.000000 healpix-2024.1/python/healpix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:15:19.416199 healpix-2024.1/python/healpix/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 08:15:15.000000 healpix-2024.1/python/healpix/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-16 08:15:15.000000 healpix-2024.1/python/healpix/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-16 08:15:15.000000 healpix-2024.1/python/healpix/test/test_chealpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-16 08:15:15.000000 healpix-2024.1/python/healpix/test/test_healpix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:15:19.416199 healpix-2024.1/python/healpix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-16 08:15:19.000000 healpix-2024.1/python/healpix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 08:15:19.000000 healpix-2024.1/python/healpix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:15:19.000000 healpix-2024.1/python/healpix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 08:15:19.000000 healpix-2024.1/python/healpix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 08:15:19.000000 healpix-2024.1/python/healpix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:15:19.416199 healpix-2024.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 08:15:15.000000 healpix-2024.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:15:19.416199 healpix-2024.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-04-16 08:15:15.000000 healpix-2024.1/src/healpix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-16 08:15:15.000000 healpix-2024.1/src/healpix.h
```

### Comparing `healpix-2023.4/LICENSE.md` & `healpix-2024.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `healpix-2023.4/PKG-INFO` & `healpix-2024.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: healpix
-Version: 2023.4
+Version: 2024.1
 Summary: Python package for HEALPix discretisation of the sphere
-Home-page: https://github.com/ntessore/healpix
-Maintainer: Nicolas Tessore
-Maintainer-email: n.tessore@ucl.ac.uk
+Maintainer-email: Nicolas Tessore <n.tessore@ucl.ac.uk>
 License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/ntessore/healpix
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 healpix
 =======
 
 **Python and C package for HEALPix discretisation of the sphere**
 
 This package implements a lean set of routines for working with the HEALPix
```

### Comparing `healpix-2023.4/README.md` & `healpix-2024.1/README.md`

 * *Files identical despite different names*

### Comparing `healpix-2023.4/python/healpix/__init__.py` & `healpix-2024.1/python/healpix/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # author: Nicolas Tessore <n.tessore@ucl.ac.uk>
 # license: BSD-3-Clause
 '''Python package for HEALPix discretisation of the sphere'''
 
-__version__ = '2023.4'
+__version__ = '2024.1'
 
 
 import numpy as np
 import chealpix as _chp
 
 
 NSIDE_MAX = _chp.NSIDE_MAX
 '''Maximum admissible value for the NSIDE parameter.
 
 If nside > NSIDE_MAX is used, the resulting pixel indices can overflow their
 underlying integer type in the C library functions.
 
 '''
 
+
 def is_power_of_two(n):
     '''Return True if n is a power of two, or False otherwise.'''
     return (n & (n-1)) == 0
 
 
 def check_nside(nside, nest=False):
     '''Check whether nside is a valid resolution parameter.'''
     if nside < 1 or nside > NSIDE_MAX:
         raise ValueError('nside must be a positive integer 1 <= nside <= '
                          f'2^{np.log2(NSIDE_MAX):.0f}')
     if nest and (nside & (nside-1)) != 0:
-        raise ValueError('nside must be power of two in the NEST scheme');
+        raise ValueError('nside must be power of two in the NEST scheme')
 
 
 def thetaphi_from_lonlat(lon, lat, theta=None, phi=None):
     '''convert longitude and latitude in degree to theta and phi in radian'''
     theta, phi = np.deg2rad(lat, out=theta), np.deg2rad(lon, out=phi)
     theta *= -1
     theta += np.pi/2
@@ -114,14 +115,24 @@
     return _chp.nside2npix(nside)
 
 
 def npix2nside(npix):
     return _chp.npix2nside(npix)
 
 
+def nside2order(nside):
+    """Return the HEALPix order for a given NSIDE parameter."""
+    return _chp.nside2order(nside)
+
+
+def order2nside(order):
+    """Return the NSIDE parameter for a given HEALPix order."""
+    return _chp.order2nside(order)
+
+
 def randang(nside, ipix, nest=False, lonlat=False, rng=None):
     '''Sample random spherical coordinates from the given HEALPix pixels.
 
     This function produces one pair of random spherical coordinates from each
     HEALPix pixel listed in `ipix`, which can be scalar or array-like.  The
     indices use the `nside` resolution parameter and either the RING scheme
     (if `nest` is false, the default) or the NEST scheme (if `nest` is true).
@@ -187,33 +198,32 @@
 def ring2nest(nside, ipix):
     return _chp.ring2nest(nside, ipix)
 
 
 def uniq2pix(uniq, nest=False):
     '''Convert from UNIQ to RING or NEST pixel scheme.
 
-    Returns a tuple `nside, ipix` of resolution parameters and pixel
-    indices in the RING scheme (if `nest` is false, the default) or the
-    NEST scheme (if `nest` is true).
+    Returns a tuple `order, ipix` of HEALPix orders and pixel indices in
+    the RING scheme (if `nest` is false, the default) or the NEST scheme
+    (if `nest` is true).
 
     '''
     if nest:
-        nside, ipix = _chp.uniq2nest(uniq)
+        order, ipix = _chp.uniq2nest(uniq)
     else:
-        nside, ipix = _chp.uniq2ring(uniq)
-    return nside, ipix
+        order, ipix = _chp.uniq2ring(uniq)
+    return order, ipix
 
 
-def pix2uniq(nside, ipix, nest=False):
+def pix2uniq(order, ipix, nest=False):
     '''Convert RING or NEST to UNIQ pixel scheme.
 
-    Returns a pixel index in the UNIQ scheme for each pair of resolution
-    parameter `nside` and pixel index `ipix` in the RING scheme (if
-    `nest` is false, the default) or the NEST scheme (if `nest` is
-    true).
+    Returns a pixel index in the UNIQ scheme for each pair of HEALPix
+    order `order` and pixel index `ipix` in the RING scheme (if `nest`
+    is false, the default) or the NEST scheme (if `nest` is true).
 
     '''
     if nest:
-        uniq = _chp.nest2uniq(nside, ipix)
+        uniq = _chp.nest2uniq(order, ipix)
     else:
-        uniq = _chp.ring2uniq(nside, ipix)
+        uniq = _chp.ring2uniq(order, ipix)
     return uniq
```

### Comparing `healpix-2023.4/python/healpix/test/conftest.py` & `healpix-2024.1/python/healpix/test/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import pytest
 import numpy as np
 
-np.random.seed(12345)
-
-
-def is_power_of_two(n):
-    return (n & (n-1)) == 0
-
 
 def fixture_get(request, name, default):
     if name in request.fixturenames:
         return request.getfixturevalue(name)
     else:
         return default
 
 
-@pytest.fixture(params=[1, 15, 16, 128])
+@pytest.fixture(params=[1, 4, 16, 64])
 def nside(request):
     nside = request.param
-    if (fixture_get(request, 'nest', False) or request.node.get_closest_marker('nest')) \
-            and not is_power_of_two(nside):
-        pytest.skip(reason='nside is not power of two')
     return nside
 
 
+@pytest.fixture(params=[1, 3, 4, 15, 16, 63, 64])
+def nside_dirty(request):
+    nside = request.param
+    return nside
+
+
+@pytest.fixture
+def order(nside):
+    return nside.bit_length() - 1
+
+
 @pytest.fixture(params=[True, False])
 def nest(request):
     return request.param
 
 
 @pytest.fixture(params=[True, False])
 def lonlat(request):
@@ -55,10 +57,10 @@
     a, b = (5/18)**0.5, 2/3
     x = np.array([a, -a, -a, a, 1, 0, -1, 0, a, -a, -a, a])
     y = np.array([a, a, -a, -a, 0, 1, 0, -1, a, a, -a, -a])
     z = np.array([b, b, b, b, 0, 0, 0, 0, -b, -b, -b, -b])
     return x, y, z
 
 
-def pytest_configure(config):
-    config.addinivalue_line(
-            'markers', 'nest: mark test as using the NEST scheme')
+@pytest.fixture(scope="session")
+def rng():
+    return np.random.default_rng(12345)
```

### Comparing `healpix-2023.4/python/healpix/test/test_chealpix.py` & `healpix-2024.1/python/healpix/test/test_chealpix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pytest
 import numpy as np
 import numpy.testing as npt
 
 
 def test_ang2vec():
     from chealpix import ang2vec
     theta = np.arccos(np.random.uniform(-1, 1, size=100))
@@ -17,115 +16,129 @@
     from chealpix import vec2ang
     x, y, z = np.random.randn(3, 100)
     theta, phi = vec2ang(x, y, z)
     npt.assert_allclose(theta, np.arctan2(np.hypot(x, y), z))
     npt.assert_allclose(phi, np.arctan2(y, x))
 
 
-@pytest.mark.nest
 def test_ang_nest(nside):
     from chealpix import ang2nest, nest2ang
     ipix = np.arange(12*nside**2)
     npt.assert_array_equal(ang2nest(nside, *nest2ang(nside, ipix)), ipix)
 
 
-def test_ang_ring(nside):
+def test_ang_ring(nside_dirty):
     from chealpix import ang2ring, ring2ang
-    ipix = np.arange(12*nside**2)
-    npt.assert_array_equal(ang2ring(nside, *ring2ang(nside, ipix)), ipix)
+    ipix = np.arange(12*nside_dirty**2)
+    npt.assert_array_equal(ang2ring(nside_dirty, *ring2ang(nside_dirty, ipix)), ipix)
 
 
-@pytest.mark.nest
 def test_vec_nest(nside):
     from chealpix import vec2nest, nest2vec
     ipix = np.arange(12*nside**2)
     npt.assert_array_equal(vec2nest(nside, *nest2vec(nside, ipix)), ipix)
 
 
-def test_vec_ring(nside):
+def test_vec_ring(nside_dirty):
     from chealpix import vec2ring, ring2vec
-    ipix = np.arange(12*nside**2)
-    npt.assert_array_equal(vec2ring(nside, *ring2vec(nside, ipix)), ipix)
+    ipix = np.arange(12*nside_dirty**2)
+    npt.assert_array_equal(vec2ring(nside_dirty, *ring2vec(nside_dirty, ipix)), ipix)
 
 
-@pytest.mark.nest
 def test_ang_nest_uv(nside):
     from chealpix import ang2nest_uv, nest2ang_uv
     ipix = np.arange(12*nside**2)
     u, v = np.random.rand(2, ipix.size)
     result = ang2nest_uv(nside, *nest2ang_uv(nside, ipix, u, v))
     npt.assert_array_equal(result[0], ipix)
-    npt.assert_allclose(result[1], u)
-    npt.assert_allclose(result[2], v)
+    npt.assert_allclose(result[1], u, rtol=1e-6)
+    npt.assert_allclose(result[2], v, rtol=1e-6)
 
 
-def test_ang_ring_uv(nside):
+def test_ang_ring_uv(nside_dirty):
     from chealpix import ang2ring_uv, ring2ang_uv
-    ipix = np.arange(12*nside**2)
+    ipix = np.arange(12*nside_dirty**2)
     u, v = np.random.rand(2, ipix.size)
-    result = ang2ring_uv(nside, *ring2ang_uv(nside, ipix, u, v))
+    result = ang2ring_uv(nside_dirty, *ring2ang_uv(nside_dirty, ipix, u, v))
     npt.assert_array_equal(result[0], ipix)
-    npt.assert_allclose(result[1], u)
-    npt.assert_allclose(result[2], v)
+    npt.assert_allclose(result[1], u, rtol=1e-6)
+    npt.assert_allclose(result[2], v, rtol=1e-6)
 
 
-@pytest.mark.nest
 def test_vec_nest_uv(nside):
     from chealpix import vec2nest_uv, nest2vec_uv
     ipix = np.arange(12*nside**2)
     u, v = np.random.rand(2, ipix.size)
     result = vec2nest_uv(nside, *nest2vec_uv(nside, ipix, u, v))
     npt.assert_array_equal(result[0], ipix)
-    npt.assert_allclose(result[1], u)
-    npt.assert_allclose(result[2], v)
+    npt.assert_allclose(result[1], u, rtol=1e-6)
+    npt.assert_allclose(result[2], v, rtol=1e-6)
 
 
-def test_vec_ring_uv(nside):
+def test_vec_ring_uv(nside_dirty):
     from chealpix import vec2ring_uv, ring2vec_uv
-    ipix = np.arange(12*nside**2)
+    ipix = np.arange(12*nside_dirty**2)
     u, v = np.random.rand(2, ipix.size)
-    result = vec2ring_uv(nside, *ring2vec_uv(nside, ipix, u, v))
+    result = vec2ring_uv(nside_dirty, *ring2vec_uv(nside_dirty, ipix, u, v))
     npt.assert_array_equal(result[0], ipix)
-    npt.assert_allclose(result[1], u)
-    npt.assert_allclose(result[2], v)
+    npt.assert_allclose(result[1], u, rtol=1e-6)
+    npt.assert_allclose(result[2], v, rtol=1e-6)
 
 
-@pytest.mark.nest
 def test_nest_ring(nside):
     from chealpix import nest2ring, ring2nest
     ipix = np.arange(12*nside**2)
     npt.assert_array_equal(nest2ring(nside, ring2nest(nside, ipix)), ipix)
     npt.assert_array_equal(ring2nest(nside, nest2ring(nside, ipix)), ipix)
 
 
-def test_nside2npix(nside):
+def test_nside2npix(nside_dirty):
     from chealpix import nside2npix
-    assert nside2npix(nside) == 12*nside**2
+    assert nside2npix(nside_dirty) == 12*nside_dirty**2
 
 
-def test_npix2nside(nside):
+def test_npix2nside(nside_dirty):
     from chealpix import npix2nside
-    assert npix2nside(12*nside**2) == nside
+    assert npix2nside(12*nside_dirty**2) == nside_dirty
 
 
 def test_npix2nside_invalid():
     from chealpix import npix2nside
     assert npix2nside(7) == -1
     assert npix2nside(49) == -1
 
 
-@pytest.mark.nest
-def test_uniq_nest(nside):
+def test_nside2order(nside, order):
+    from chealpix import nside2order
+    assert nside2order(nside) == order
+
+
+def test_nside2order_invalid():
+    from chealpix import nside2order
+    assert nside2order(-1) == -1
+    assert nside2order(3) == -1
+
+
+def test_order2nside(nside, order):
+    from chealpix import order2nside
+    assert order2nside(order) == nside
+
+
+def test_order2nside_invalid():
+    from chealpix import order2nside
+    assert order2nside(-1) == -1
+
+
+def test_uniq_nest(order):
     from chealpix import uniq2nest, nest2uniq
-    ipix = np.arange(12*nside**2)
-    nside_out, ipix_out = uniq2nest(nest2uniq(nside, ipix))
-    npt.assert_array_equal(nside_out, nside)
+    ipix = np.arange(12 * (1 << 2*order))
+    order_out, ipix_out = uniq2nest(nest2uniq(order, ipix))
+    npt.assert_array_equal(order_out, order)
     npt.assert_array_equal(ipix_out, ipix)
 
 
-@pytest.mark.nest
-def test_uniq_ring(nside):
+def test_uniq_ring(order):
     from chealpix import uniq2ring, ring2uniq
-    ipix = np.arange(12*nside**2)
-    nside_out, ipix_out = uniq2ring(ring2uniq(nside, ipix))
-    npt.assert_array_equal(nside_out, nside)
+    ipix = np.arange(12 * (1 << 2*order))
+    order_out, ipix_out = uniq2ring(ring2uniq(order, ipix))
+    npt.assert_array_equal(order_out, order)
     npt.assert_array_equal(ipix_out, ipix)
```

### Comparing `healpix-2023.4/python/healpix/test/test_healpix.py` & `healpix-2024.1/python/healpix/test/test_healpix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-import pytest
 import numpy as np
 import numpy.testing as npt
 
 from . import assert_shape
 
 
-def test_ang2vec(lonlat, size):
+def test_ang2vec(lonlat, size, rng):
     from healpix import ang2vec
     if lonlat:
-        theta_lon = np.random.uniform(0, 360, size=size)
-        phi_lat = np.random.uniform(-90, 90, size=size)
+        theta_lon = rng.uniform(0, 360, size=size)
+        phi_lat = rng.uniform(-90, 90, size=size)
         x_ = np.cos(np.deg2rad(phi_lat))*np.cos(np.deg2rad(theta_lon))
         y_ = np.cos(np.deg2rad(phi_lat))*np.sin(np.deg2rad(theta_lon))
         z_ = np.sin(np.deg2rad(phi_lat))
     else:
-        theta_lon = np.random.uniform(0, np.pi, size=size)
-        phi_lat = np.random.uniform(0, 2*np.pi, size=size)
+        theta_lon = rng.uniform(0, np.pi, size=size)
+        phi_lat = rng.uniform(0, 2*np.pi, size=size)
         x_ = np.sin(theta_lon)*np.cos(phi_lat)
         y_ = np.sin(theta_lon)*np.sin(phi_lat)
         z_ = np.cos(theta_lon)
     x, y, z = ang2vec(theta_lon, phi_lat, lonlat=lonlat)
     npt.assert_allclose(x, x_)
     npt.assert_allclose(y, y_)
     npt.assert_allclose(z, z_)
     assert_shape(x, size)
     assert_shape(y, size)
     assert_shape(z, size)
 
 
-def test_vec2ang(lonlat, size):
+def test_vec2ang(lonlat, size, rng):
     from healpix import vec2ang
-    x = np.random.standard_normal(size)
-    y = np.random.standard_normal(size)
-    z = np.random.standard_normal(size)
+    x = rng.standard_normal(size)
+    y = rng.standard_normal(size)
+    z = rng.standard_normal(size)
     theta_, phi_ = np.arctan2(np.hypot(x, y), z), np.arctan2(y, x)
     if lonlat:
         theta_, phi_ = np.rad2deg(phi_), np.rad2deg(np.pi/2-theta_)
     theta, phi = vec2ang(x, y, z, lonlat=lonlat)
     npt.assert_allclose(theta, theta_)
     npt.assert_allclose(phi, phi_)
     assert_shape(theta, size)
@@ -71,17 +70,18 @@
 
 def test_vec_pix(nside, nest):
     from healpix import vec2pix, pix2vec
     ipix = np.arange(12*nside**2)
     npt.assert_array_equal(vec2pix(nside, *pix2vec(nside, ipix, nest), nest), ipix)
 
 
-def test_uniq_pix(nest):
+def test_uniq_pix(nest, rng):
     from healpix import uniq2pix, pix2uniq, ring2nest
-    nside = 2**np.random.randint(0, 30, 1000)
-    ipix = np.random.randint(0, 12*nside**2)
+    order = rng.integers(0, 30, 1000)
+    nside = 1 << order
+    ipix = rng.integers(0, 12*nside**2)
     ipnest = ipix if nest else [ring2nest(ns, ip) for ns, ip in zip(nside, ipix)]
-    uniq = pix2uniq(nside, ipix, nest)
+    uniq = pix2uniq(order, ipix, nest)
     npt.assert_array_equal(uniq, 4*nside**2 + ipnest)
-    nside_out, ipix_out = uniq2pix(uniq, nest)
-    npt.assert_array_equal(nside_out, nside)
+    order_out, ipix_out = uniq2pix(uniq, nest)
+    npt.assert_array_equal(order_out, order)
     npt.assert_array_equal(ipix_out, ipix)
```

### Comparing `healpix-2023.4/python/healpix.egg-info/PKG-INFO` & `healpix-2024.1/python/healpix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: healpix
-Version: 2023.4
+Version: 2024.1
 Summary: Python package for HEALPix discretisation of the sphere
-Home-page: https://github.com/ntessore/healpix
-Maintainer: Nicolas Tessore
-Maintainer-email: n.tessore@ucl.ac.uk
+Maintainer-email: Nicolas Tessore <n.tessore@ucl.ac.uk>
 License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/ntessore/healpix
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 healpix
 =======
 
 **Python and C package for HEALPix discretisation of the sphere**
 
 This package implements a lean set of routines for working with the HEALPix
```

### Comparing `healpix-2023.4/src/healpix.c` & `healpix-2024.1/src/healpix.c`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 #ifdef _MSC_VER
 #include <intrin.h>  // for _BitScanReverse64
 #endif
 
 
 // count leading zeros
-static inline int clz(uint64_t x) {
+static inline uint8_t clz(uint64_t x) {
 #if defined(__GNUC__) || defined(__clang__)
     return __builtin_clzll(x);
 #elif defined(_MSC_VER) && (defined(_M_AMD64) || defined(_M_X64))
     unsigned long bsr;
     return _BitScanReverse64(&bsr, x) ? 63 - bsr : 64;
 #else
     // taken from https://stackoverflow.com/a/70550680 under CC BY-SA 4.0
@@ -47,16 +47,16 @@
     x |= x >> 16;
     x |= x >> 32;
     return clz64_tab[(uint64_t)(x * 0x03f6eaf2cd271461u) >> 58];
 #endif
 }
 
 // fast integer log2
-int ilog2(uint64_t x) {
-    return x == 0 ? -1 : 63 - clz(x);
+int8_t ilog2(uint64_t x) {
+    return x > 0 ? 63 - clz(x) : -1;
 }
 
 
 // fast integer square root
 // taken from https://stackoverflow.com/a/70550680 under CC BY-SA 4.0
 uint32_t isqrt(uint64_t x) {
     // isqrt64_tab[k] = isqrt(256*(k+65)-1) for 0 <= k < 192
@@ -365,14 +365,27 @@
 
 
 int64_t nside2npix(int64_t nside) {
     return 12*nside*nside;
 }
 
 
+int8_t nside2order(int64_t nside) {
+    // power of two check
+    if ((nside & (nside-1)) != 0)
+        return -1;
+    return ilog2(nside);
+}
+
+
+int64_t order2nside(int8_t order) {
+    return order >= 0 ? (int64_t)1 << order : -1;
+}
+
+
 double vec_angle(t_vec v1, t_vec v2) {
     t_vec cross = {
         v1.y*v2.z - v1.z*v2.y,
         v1.z*v2.x - v1.x*v2.z,
         v1.x*v2.y - v1.y*v2.x
     };
     double len = sqrt(cross.x*cross.x + cross.y*cross.y + cross.z*cross.z);
@@ -467,32 +480,41 @@
 // conversions from or to UNIQ pixel scheme
 
 
 t_pix uniq2nest(int64_t uniq) {
     if (uniq < 4) {
         return (t_pix){-1, -1};
     } else {
-        int order = ilog2(uniq)/2 - 1;
-        return (t_pix){1ll << order, uniq - 4*(1ll << 2*order)};
+        int8_t order = ilog2(uniq)/2 - 1;
+        return (t_pix){order, uniq - ((int64_t)1 << 2*(order+1))};
     }
 }
 
 
 t_pix uniq2ring(int64_t uniq) {
-    t_pix pix = uniq2nest(uniq);
-    pix.ipix = nest2ring(pix.nside, pix.ipix);
-    return pix;
+    if (uniq < 4) {
+        return (t_pix){-1, -1};
+    } else {
+        t_pix pix = uniq2nest(uniq);
+        pix.ipix = nest2ring(order2nside(pix.order), pix.ipix);
+        return pix;
+    }
 }
 
 
-int64_t nest2uniq(int64_t nside, int64_t ipix) {
-    if (nside < 0 || ipix < 0) {
+int64_t nest2uniq(int8_t order, int64_t ipix) {
+    if (order < 0 || ipix < 0) {
         return -1;
     } else {
-        return 4*nside*nside + ipix;
+        return ((int64_t)1 << 2*(order+1)) + ipix;
     }
 }
 
 
-int64_t ring2uniq(int64_t nside, int64_t ipix) {
-    return nest2uniq(nside, ring2nest(nside, ipix));
+int64_t ring2uniq(int8_t order, int64_t ipix) {
+    if (order < 0 || ipix < 0) {
+        return -1;
+    } else {
+        int64_t nside = order2nside(order);
+        return 4*nside*nside + ring2nest(nside, ipix);
+    }
 }
```

### Comparing `healpix-2023.4/src/healpix.h` & `healpix-2024.1/src/healpix.h`

 * *Files 5% similar despite different names*

```diff
@@ -117,14 +117,22 @@
 int64_t nside2npix(int64_t nside);
 
 
 // Returns sqrt(npix/12) if this is an integer number, otherwise -1.
 int64_t npix2nside(int64_t npix);
 
 
+// Returns log2(nside).
+int8_t nside2order(int64_t nside);
+
+
+// Returns log2(npix).
+int64_t order2nside(int8_t order);
+
+
 // Returns the angle (in radians) between the vectors v1 and v2.
 // The result is accurate even for angles close to 0 and pi.
 double vec_angle(t_vec v1, t_vec v2);
 
 
 // conversions with sub-pixel positions
 
@@ -160,35 +168,35 @@
 // Variant of ring2vec that also takes the sub-pixel position in u and v.
 t_vec ring2vec_uv(int64_t nside, int64_t ipix, double u, double v);
 
 
 // Conversions to UNIQ pixel index scheme
 
 
-// Describe a pixel index in RING or NEST scheme and its nside parameter
+// Describe a pixel index in RING or NEST scheme and its order parameter
 typedef struct {
-    int64_t nside;
+    int8_t order;
     int64_t ipix;
 } t_pix;
 
 
 // Convert from UNIQ to NEST scheme and nside parameter
 t_pix uniq2nest(int64_t uniq);
 
 
 // Convert from UNIQ to RING scheme and nside parameter
 t_pix uniq2ring(int64_t uniq);
 
 
-// Convert from NEST scheme and nside parameter to UNIQ
-int64_t nest2uniq(int64_t nside, int64_t ipix);
+// Convert from NEST scheme and order parameter to UNIQ
+int64_t nest2uniq(int8_t order, int64_t ipix);
 
 
-// Convert from RING scheme and nside parameter to UNIQ
-int64_t ring2uniq(int64_t nside, int64_t ipix);
+// Convert from RING scheme and order parameter to UNIQ
+int64_t ring2uniq(int8_t order, int64_t ipix);
 
 
 #ifdef __cplusplus
 } // extern "C"
 #endif
 
 #endif  // HEALPIX_H_
```

