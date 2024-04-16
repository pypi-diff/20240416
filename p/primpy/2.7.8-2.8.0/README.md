# Comparing `tmp/primpy-2.7.8.tar.gz` & `tmp/primpy-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primpy-2.7.8.tar", last modified: Wed Apr 10 08:35:08 2024, max compression
+gzip compressed data, was "primpy-2.8.0.tar", last modified: Tue Apr 16 20:26:01 2024, max compression
```

## Comparing `primpy-2.7.8.tar` & `primpy-2.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.564746 primpy-2.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 08:35:02.000000 primpy-2.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 08:35:08.564746 primpy-2.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-10 08:35:02.000000 primpy-2.7.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.556746 primpy-2.7.8/primpy/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/bigbang.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.560746 primpy-2.7.8/primpy/efolds/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/efolds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/efolds/inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/efolds/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/equations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/exceptionhandling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/initialconditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/oscode_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.560746 primpy-2.7.8/primpy/time/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/time/inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/time/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.564746 primpy-2.7.8/primpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:35:08.564746 primpy-2.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-10 08:35:02.000000 primpy-2.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.560746 primpy-2.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_bigbang.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_efolds_inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_equations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_exceptionhandling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_initialconditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_time_inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:26:01.582383 primpy-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 20:25:54.000000 primpy-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-16 20:26:01.582383 primpy-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-16 20:25:54.000000 primpy-2.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:26:01.578383 primpy-2.8.0/primpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/bigbang.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:26:01.578383 primpy-2.8.0/primpy/efolds/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/efolds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/efolds/inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/efolds/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/exceptionhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23613 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/initialconditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/oscode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:26:01.578383 primpy-2.8.0/primpy/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/time/inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/time/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 20:25:54.000000 primpy-2.8.0/primpy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:26:01.582383 primpy-2.8.0/primpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-16 20:26:01.000000 primpy-2.8.0/primpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-16 20:26:01.000000 primpy-2.8.0/primpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:26:01.000000 primpy-2.8.0/primpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 20:26:01.000000 primpy-2.8.0/primpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 20:26:01.000000 primpy-2.8.0/primpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:26:01.582383 primpy-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-16 20:25:54.000000 primpy-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:26:01.582383 primpy-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_bigbang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_efolds_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_exceptionhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_initialconditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_time_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 20:25:54.000000 primpy-2.8.0/tests/test_version.py
```

### Comparing `primpy-2.7.8/LICENSE` & `primpy-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/PKG-INFO` & `primpy-2.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primpy
-Version: 2.7.8
+Version: 2.8.0
 Summary: primpy: Calculations for the primordial Universe.
 Author: Lukas Hergt
 Author-email: lh561@mrao.cam.ac.uk
 License: MIT
 Keywords: PPS,cosmic inflation,initial conditions for inflation,kinetic dominance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 Requires-Dist: pyoscode
 
 ================================================
 primpy: calculations for the primordial Universe
 ================================================
 :primpy: calculations for the primordial Universe
 :Author: Lukas Hergt
-:Version: 2.7.8
+:Version: 2.8.0
 :Homepage: https://github.com/lukashergt/primpy
 :Documentation: https://primpy.readthedocs.io
 
 .. image:: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml/badge.svg?branch=master
     :target: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml
     :alt: Build Status
 .. image:: https://codecov.io/gh/lukashergt/primpy/branch/master/graph/badge.svg?token=USS4K53PY0
```

### Comparing `primpy-2.7.8/README.rst` & `primpy-2.8.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ================================================
 primpy: calculations for the primordial Universe
 ================================================
 :primpy: calculations for the primordial Universe
 :Author: Lukas Hergt
-:Version: 2.7.8
+:Version: 2.8.0
 :Homepage: https://github.com/lukashergt/primpy
 :Documentation: https://primpy.readthedocs.io
 
 .. image:: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml/badge.svg?branch=master
     :target: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml
     :alt: Build Status
 .. image:: https://codecov.io/gh/lukashergt/primpy/branch/master/graph/badge.svg?token=USS4K53PY0
```

### Comparing `primpy-2.7.8/primpy/bigbang.py` & `primpy-2.8.0/primpy/bigbang.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 """:mod:`primpy.bigbang`: general setup for equations for standard Big Bang cosmology."""
 import warnings
 import numpy as np
 from scipy import integrate
 from primpy.exceptionhandling import BigBangWarning, BigBangError
-from primpy.units import pi, G, tp_s, lp_m, Mpc_m
+from primpy.units import pi, c, G, tp_s, lp_m, Mpc_m
 from primpy.parameters import rho_r0_kg_im3, z_BBN
 
 
 def get_H0(h, units='planck'):
     """Get present-day Hubble parameter from little Hubble `h`."""
     if units == 'planck':
-        return h * 100e3 / Mpc_m * tp_s  # in reduced Planck units
+        return h * 100e3 / Mpc_m * tp_s  # in reduced Planck units, i.e. tp^-1
     elif units == 'H0':
-        return h * 100  # in conventional Hubble parameter units
+        return h * 100  # in conventional Hubble parameter units, i.e. km/s/Mpc
     elif units == 'SI':
         return h * 100e3 / Mpc_m  # in SI units, i.e. s^-1
     else:
         raise NotImplementedError("%s not implemented for H0 units, please choose "
                                   "one of {'planck', 'H0', 'SI'}." % units)
 
 
@@ -40,19 +40,20 @@
 
 
 def get_N_BBN(h, Omega_K0):
     """Get the epoch of Big Bang nucleosynthesis in terms of e-folds (in Planck units)."""
     return np.log(get_a0(h=h, Omega_K0=Omega_K0, units='planck') / (1 + z_BBN))
 
 
-def get_w_reh(N1, N2, log_cHH1, log_cHH2):
+def get_w_delta_reh(N_end, N_reh, log_cHH_end, log_cHH_reh):
     """Get the e.o.s. parameter for reheating `w_reh` from e-folds and comoving Hubble horizon."""
-    delta_N = N2 - N1
-    delta_cHH = log_cHH2 - log_cHH1
-    return (2 * delta_cHH / delta_N - 1) / 3
+    delta_reh = N_reh - N_end
+    delta_cHH = log_cHH_reh - log_cHH_end
+    w_reh = (2 * delta_cHH / delta_reh - 1) / 3
+    return w_reh, delta_reh
 
 
 def get_rho_crit_kg_im3(h):
     """Get present-day critical density from little Hubble `h`."""
     H0_is = get_H0(h=h, units='SI')
     rho_crit_kg_im3 = 3 * H0_is**2 / (8 * pi * G)
     return rho_crit_kg_im3
@@ -61,41 +62,44 @@
 def get_Omega_r0(h):
     """Get present-day radiation density parameter from little Hubble `h`."""
     rho_crit_kg_im3 = get_rho_crit_kg_im3(h=h)
     Omega_r0 = rho_r0_kg_im3 / rho_crit_kg_im3
     return Omega_r0
 
 
-def Hubble_parameter(N, Omega_m0, Omega_K0, h):
+def Hubble_parameter(N, Omega_m0, Omega_K0, h, units='planck'):
     """Hubble parameter (in reduced Planck units) at `N=ln(a)` during standard Big Bang.
 
     Parameters
     ----------
         N : float, np.ndarray
             e-folds of the scale factor N=ln(a) during standard Big Bang
             evolution, where the scale factor would be given in reduced Planck
             units (same as output from primpy).
         Omega_m0 : float
             matter density parameter today
         Omega_K0 : float
             curvature density parameter today
         h : float
             dimensionless Hubble parameter today, "little h"
+        units : str
+            Output units, can be any of {'planck', 'H0', 'SI'} returning
+            units of `1/tp`, `km/s/Mpc` or `1/s` respectively.
 
     `Omega_r0` is derived from the Hubble parameter using Planck's law.
     `Omega_L0` is derived from the other density parameters to sum to one.
 
     Returns
     -------
         H : float
             Hubble parameter during standard Big Bang evolution of the Universe.
             In reduced Planck units [tp^-1].
 
     """
-    H0 = get_H0(h=h, units='planck')  # in reduced Planck units
+    H0 = get_H0(h=h, units=units)
     Omega_r0 = get_Omega_r0(h=h)
     Omega_L0 = 1 - Omega_r0 - Omega_m0 - Omega_K0
     if Omega_L0 > no_Big_Bang_line(Omega_m0=Omega_m0):
         raise BigBangError("no Big Bang for Omega_m0=%g, Omega_L0=%g" % (Omega_m0, Omega_L0))
     elif Omega_L0 < expand_recollapse_line(Omega_m0=Omega_m0):
         warnings.warn(BigBangWarning("Universe recollapses for Omega_m0=%g, Omega_L0=%g"
                                      % (Omega_m0, Omega_L0)))
@@ -171,29 +175,35 @@
             matter density parameter today
         Omega_K0 : float
             curvature density parameter today
         h : float
             dimensionless Hubble parameter today, "little h"
         units : str
             Output units, can be any of {'planck', 'Mpc', 'SI'} returning
-            units of `lp`, `Mpc` or `m` respectively.
+            units of `lp`, `Mpc`, or `m` respectively.
 
     `Omega_r0` is derived from the Hubble parameter using Planck's law.
     `Omega_L0` is derived from the other density parameters to sum to one.
 
     Returns
     -------
         cHH : float
             Comoving Hubble horizon during standard Big Bang evolution of the Universe.
 
     """
-    a0 = get_a0(h=h, Omega_K0=Omega_K0, units=units)
+    a0 = get_a0(h=h, Omega_K0=Omega_K0, units='planck')
     a = np.exp(N)
-    H = Hubble_parameter(N=N, Omega_m0=Omega_m0, Omega_K0=Omega_K0, h=h)
-    return a0 / (a * H)
+    units = 'H0' if units == 'Mpc' else units
+    H = Hubble_parameter(N=N, Omega_m0=Omega_m0, Omega_K0=Omega_K0, h=h, units=units)
+    if units == 'planck':
+        return a0 / (a * H)
+    elif units == 'H0':  # actually Mpc
+        return a0 * c / (a * H * 1e3)
+    elif units == 'SI':
+        return a0 * c / (a * H)
 
 
 def conformal_time(N_start, N, Omega_m0, Omega_K0, h):
     """Conformal time during standard Big Bang evolution from `N_start` to `N`.
 
     Parameters
     ----------
@@ -271,14 +281,14 @@
         eta_beg = b_forward.eta[0]
     else:
         eta_beg = b_backward.eta[-1]
     eta_end = b_forward.eta[-1]
     conformal_time_before = eta_end - eta_beg
 
     # after (from the end of inflation until today)
-    conformal_time_after = conformal_time(N_start=b_forward.N_end,
-                                          N=np.log(b_forward.a0_lp),
+    conformal_time_after = conformal_time(N_start=b_forward._N_end,
+                                          N=np.log(b_forward.a0),
                                           Omega_m0=Omega_m0,
                                           Omega_K0=Omega_K0,
                                           h=h)[0]
 
     return conformal_time_before / conformal_time_after
```

### Comparing `primpy-2.7.8/primpy/efolds/inflation.py` & `primpy-2.8.0/primpy/efolds/inflation.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,28 @@
     """Background equations during inflation w.r.t. e-folds `N`.
 
     Solves background variables with e-folds `N` of the scale factor as
     independent variable for curved and flat universes using the Klein-Gordon
     and Friedmann equations.
 
     Independent variable:
-        N: e-folds of the scale-factor
+        _N: e-folds of the scale-factor
+        (the underscore here means that this is the as of yet uncalibrated scale factor)
 
     Dependent variables:
         phi: inflaton field
         dphidN: `d(phi)/dN`
         t: time (optional)
         eta: conformal time (optional)
 
     """
 
     def __init__(self, K, potential, track_time=False, track_eta=False, verbose=False):
         super(InflationEquationsN, self).__init__(K=K, potential=potential, verbose=verbose)
-        self._set_independent_variable('N')
+        self._set_independent_variable('_N')
         self.add_variable('phi', 'dphidN')
         self.track_time = track_time
         self.track_eta = track_eta
         if track_time:
             self.add_variable('t')
         if track_eta:
             self.add_variable('eta')
```

### Comparing `primpy-2.7.8/primpy/efolds/perturbations.py` & `primpy-2.8.0/primpy/efolds/perturbations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
-""":mod:`primpy.efolds.perturbations`: curvature perturbations with respect to e-folds `N`."""
+""":mod:`primpy.efolds.perturbations`: curvature perturbations with respect to e-folds `_N`."""
 import numpy as np
 from primpy.perturbations import Perturbation, ScalarMode, TensorMode
 
 
 class PerturbationN(Perturbation):
-    """Curvature perturbation for wavenumber `k` with respect to e-folds `N=ln(a)`.
+    """Curvature perturbation for wavenumber `k` with respect to e-folds `_N=ln(a)`.
 
-    Solves the Mukhanov--Sasaki equations w.r.t. number of e-folds `N` of the
+    Solves the Mukhanov--Sasaki equations w.r.t. number of e-folds `_N` of the
     scale factor `a` for curved universes.
 
     Input Parameters
     ----------------
         background : Bunch object
             Background solution as returned by
             :func:`primpy.efolds.inflation.InflationEquationsN.sol`.
@@ -29,30 +29,30 @@
 
 
 class ScalarModeN(ScalarMode):
     """Template for scalar modes."""
 
     def __init__(self, background, k, **kwargs):
         super(ScalarModeN, self).__init__(background=background, k=k, **kwargs)
-        self._set_independent_variable('N')
+        self._set_independent_variable('_N')
 
     def __call__(self, x, y):
         """Vector of derivatives."""
         raise NotImplementedError("Equations class must define __call__.")
 
     def mukhanov_sasaki_frequency_damping(self):
         """Frequency and damping term of the Mukhanov-Sasaki equations for scalar modes.
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
-        comoving curvature perturbations `R` w.r.t. e-folds `N`, where the e.o.m. is
+        comoving curvature perturbations `R` w.r.t. e-folds `_N`, where the e.o.m. is
         written as `ddR + 2 * damping * dR + frequency**2 R = 0`.
 
         """
         K = self.background.K
-        a2 = np.exp(2 * self.background.N[self.idx_beg:self.idx_end+1])
+        a2 = np.exp(2 * self.background._N[self.idx_beg:self.idx_end+1])
         H = self.background.H[self.idx_beg:self.idx_end+1]
         dphidN = self.background.dphidN[self.idx_beg:self.idx_end+1]
         H2 = H**2
         dV = self.background.potential.dV(self.background.phi[self.idx_beg:self.idx_end+1])
         Omega_K = self.background.Omega_K[self.idx_beg:self.idx_end+1]
 
         kappa2 = self.k**2 + self.k * K * (K + 1) - 3 * K
@@ -63,53 +63,53 @@
         frequency2 = kappa2 / (a2 * H2) + (damping2 + xi + 1) * Omega_K
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping2 / 2
         else:
             return np.sqrt(frequency2 + 0j), damping2 / 2
 
     def get_vacuum_ic_RST(self):
-        """Get initial conditions for scalar modes for RST vacuum w.r.t. e-folds `N`."""
-        a_i = np.exp(self.background.N[self.idx_beg])
+        """Get initial conditions for scalar modes for RST vacuum w.r.t. e-folds `_N`."""
+        a_i = np.exp(self.background._N[self.idx_beg])
         H_i = self.background.H[self.idx_beg]
         z_i = a_i * self.background.dphidN[self.idx_beg]
         Rk_i = 1 / np.sqrt(2 * self.k) / z_i
         dRk_i = -1j * self.k / (a_i * H_i) * Rk_i
         return Rk_i, dRk_i
 
 
 class TensorModeN(TensorMode):
     """Template for tensor modes."""
 
     def __init__(self, background, k, **kwargs):
         super(TensorModeN, self).__init__(background=background, k=k, **kwargs)
-        self._set_independent_variable('N')
+        self._set_independent_variable('_N')
 
     def __call__(self, x, y):
         """Vector of derivatives."""
         raise NotImplementedError("Equations class must define __call__.")
 
     def mukhanov_sasaki_frequency_damping(self):
         """Frequency and damping term of the Mukhanov-Sasaki equations for tensor modes.
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
-        tensor perturbations `h` w.r.t. e-folds `N`, where the e.o.m. is
+        tensor perturbations `h` w.r.t. e-folds `_N`, where the e.o.m. is
         written as `ddh + 2 * damping * dh + frequency**2 h = 0`.
 
         """
         K = self.background.K
-        N = self.background.N[self.idx_beg:self.idx_end+1]
+        N = self.background._N[self.idx_beg:self.idx_end+1]
         H2 = self.background.H[self.idx_beg:self.idx_end+1]**2
         dphidN = self.background.dphidN[self.idx_beg:self.idx_end+1]
         frequency2 = (self.k**2 + self.k * K * (K + 1) + 2 * K) * np.exp(-2 * N) / H2
         damping2 = 3 - dphidN**2 / 2 + K * np.exp(-2 * N) / H2
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping2 / 2
         else:
             return np.sqrt(frequency2 + 0j), damping2 / 2
 
     def get_vacuum_ic_RST(self):
-        """Get initial conditions for tensor modes for RST vacuum w.r.t. e-folds `N`."""
-        a_i = np.exp(self.background.N[self.idx_beg])
+        """Get initial conditions for tensor modes for RST vacuum w.r.t. e-folds `_N`."""
+        a_i = np.exp(self.background._N[self.idx_beg])
         H_i = self.background.H[self.idx_beg]
         hk_i = 2 / np.sqrt(2 * self.k) / a_i
         dhk_i = -1j * self.k / (a_i * H_i) * hk_i
         return hk_i, dhk_i
```

### Comparing `primpy-2.7.8/primpy/equations.py` & `primpy-2.8.0/primpy/equations.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/primpy/events.py` & `primpy-2.8.0/primpy/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,23 @@
 
     def __call__(self, x, y):
         """Root of `t - value`."""
         return self.equations.t(x, y) - self.value
 
 
 class UntilNEvent(Event):
-    """Stop after a given number of e-folds `N`."""
+    """Stop after a given number of e-folds `_N`."""
 
     def __init__(self, equations, value, direction=0, terminal=True):
         super(UntilNEvent, self).__init__(equations, direction, terminal, value)
         self.name = 'UntilN'
 
     def __call__(self, x, y):
-        """Root of `N - value`."""
-        return self.equations.N(x, y) - self.value
+        """Root of `_N - value`."""
+        return self.equations._N(x, y) - self.value
 
 
 class InflationEvent(Event):
     """Track inflation start/end."""
 
     def __init__(self, equations, direction=0, terminal=False, value=0, **kwargs):
         super(InflationEvent, self).__init__(equations, direction, terminal, value)
@@ -131,10 +131,10 @@
     """Track when mode exits the horizon aH."""
 
     def __init__(self, equations, value, direction=0, terminal=True):
         super(ModeExitEvent, self).__init__(equations, direction, terminal, value)
         self.name = 'ModeExit_dir%d_term%d_%e' % (self.direction, self.terminal, self.value)
 
     def __call__(self, x, y):
-        """Root of `logaH - log(value)`."""
+        """Root of `_logaH - log(value)`."""
         logH = np.log(np.abs(self.equations.H2(x, y))) / 2
-        return logH + self.equations.N(x, y) - np.log(self.value)
+        return logH + self.equations._N(x, y) - np.log(self.value)
```

### Comparing `primpy-2.7.8/primpy/exceptionhandling.py` & `primpy-2.8.0/primpy/exceptionhandling.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,28 @@
     """
 
     def __init__(self, message, *args):
         self.message = message
         super(StepSizeError, self).__init__(message, *args)
 
 
+class InsufficientInflationError(PrimpyError):
+    """Exception when there are insufficient number of e-folds for inflation.
+
+    Attributes
+    ----------
+        message : str
+            Explanation of the error.
+    """
+
+    def __init__(self, message, *args):
+        self.message = message
+        super(InsufficientInflationError, self).__init__(self.message, *args)
+
+
 class BigBangError(PrimpyError):
     """Exceptions for the standard Big Bang evolution.
 
     Attributes
     ----------
         message : str
             Explanation of the error.
@@ -108,17 +122,17 @@
     def __init__(self, message, *args, **kwargs):
         self.header = "Inflation start not determined."
         events = kwargs.pop('events', None)
         if events is None:
             self.message = "%s. %s" % (self.header, message)
         elif 'Inflation_dir+1_term1' not in events and 'Inflation_dir+1_term0' not in events:
             extra_info = ("Not tracking `InflationEvent`. Events tracked are %s. In order to "
-                          "determine the start of inflation `N_beg`, make sure to track the event "
-                          "`InflationEvent(equations, direction=+1)` defined in `primpy.events`"
-                          % events)
+                          "determine the start of inflation `_N_beg`, make sure to track the "
+                          "event `InflationEvent(equations, direction=+1)` defined in "
+                          "`primpy.events`" % events)
             self.message = "%s: %s. %s" % (self.header, extra_info, message)
         else:
             self.message = "%s. %s" % (self.header, message)
         super(InflationStartWarning, self).__init__(self.message, *args)
 
 
 class InflationEndWarning(InflationWarning):
@@ -142,23 +156,23 @@
         self.header = "Inflation end not determined"
         events = kwargs.pop('events', None)
         sol = kwargs.pop('sol', None)
         if events is None:
             self.message = "%s. %s" % (self.header, message)
         elif 'Inflation_dir-1_term1' not in events and 'Inflation_dir-1_term0' not in events:
             extra_info = ("Not tracking `InflationEvent`. Events tracked are %s. In order to "
-                          "determine the end of inflation `N_end`, make sure to track the event "
+                          "determine the end of inflation `_N_end`, make sure to track the event "
                           "`InflationEvent(equations, direction=-1)` defined in `primpy.events`"
                           % events)
             self.message = "%s: %s. %s" % (self.header, extra_info, message)
         elif sol is None:
             self.message = "%s. %s" % (self.header, message)
         elif sol.w[-1] < -1 / 3:
             extra_info = ("Still inflating: N[-1]=%g, phi[-1]=%g, w[-1]=%g"
-                          % (sol.N[-1], sol.phi[-1], sol.w[-1]))
+                          % (sol._N[-1], sol.phi[-1], sol.w[-1]))
             self.message = "%s: %s. %s" % (self.header, extra_info, message)
         else:
             self.message = "%s. %s" % (self.header, message)
         super(InflationEndWarning, self).__init__(self.message, *args)
 
 
 class BigBangWarning(PrimpyWarning):
```

### Comparing `primpy-2.7.8/primpy/initialconditions.py` & `primpy-2.8.0/primpy/initialconditions.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,18 @@
             self.dphidt_i = -self.dV_i / (3 * self.H_i)
         elif isinstance(self.equations, InflationEquationsN):
             self.x_ini = self.N_i
             self.x_end = self.x_end
             self.dphidN_i = -self.dV_i / (3 * self.H_i**2)
 
     def __call__(self, y0, **ivp_kwargs):
-        """Set background equations of inflation for `N`, `phi` and `dphi`."""
+        """Set background equations of inflation for `_N`, `phi` and `dphi`."""
         if isinstance(self.equations, InflationEquationsT):
             y0[self.equations.idx['dphidt']] = self.dphidt_i
-            y0[self.equations.idx['N']] = self.N_i
+            y0[self.equations.idx['_N']] = self.N_i
         elif isinstance(self.equations, InflationEquationsN):
             y0[self.equations.idx['dphidN']] = self.dphidN_i
             if self.equations.track_time:
                 assert self.t_i is not None, ("`track_time=%s`, but `t_i=%s`."
                                               % (self.equations.track_time, self.t_i))
                 y0[self.equations.idx['t']] = self.t_i
         else:
@@ -121,21 +121,21 @@
             self.N_i = np.log(2 * equations.K / self.V_i * (1 - 1 / self.Omega_Ki)) / 2
             self.aH_i = np.sqrt(-equations.K / self.Omega_Ki)
         else:
             raise TypeError("Need to specify either N_i or Omega_Ki.")
         self.H_i = np.sqrt(self.V_i / 2 - equations.K * np.exp(-2 * self.N_i))
 
     def __call__(self, y0, **ivp_kwargs):
-        """Set background equations of inflation for `N`, `phi` and `dphi`."""
+        """Set background equations of inflation for `_N`, `phi` and `dphi`."""
         if isinstance(self.equations, InflationEquationsT):
             self.x_ini = self.t_i
             self.x_end = self.x_end
             self.dphidt_i = -np.sqrt(self.V_i)
             y0[self.equations.idx['dphidt']] = self.dphidt_i
-            y0[self.equations.idx['N']] = self.N_i
+            y0[self.equations.idx['_N']] = self.N_i
         elif isinstance(self.equations, InflationEquationsN):
             self.x_ini = self.N_i
             self.x_end = self.x_end
             self.dphidN_i = -np.sqrt(self.V_i) / self.H_i
             y0[self.equations.idx['dphidN']] = self.dphidN_i
             if self.equations.track_time:
                 assert self.t_i is not None, ("`track_time=%s`, but `t_i=%s`."
@@ -190,19 +190,19 @@
                       CollapseEvent(self.equations)]
             with warnings.catch_warnings():
                 warnings.filterwarnings(action=self.warn_action, category=InflationWarning)
                 sol = solve(ic, events=events, **kwargs)
             if np.isfinite(sol.N_tot):
                 self.vprint("N_tot = %.15g for phi_i = %.15g" % (sol.N_tot, phi_i))
                 return sol.N_tot - self.N_tot
-            elif np.size(sol.N_events['UntilN']) > 0 or sol.N[-1] - ic.N_i >= self.N_tot:
+            elif np.size(sol._N_events['UntilN']) > 0 or sol._N[-1] - ic.N_i >= self.N_tot:
                 self.vprint("N_tot > %g for phi_i = %.15g" % (self.N_tot, phi_i))
-                return sol.N[-1] - ic.N_i
-            elif (np.size(sol.N_events['Collapse']) > 0 or
-                  sol.N_events['Inflation_dir-1_term1'] == sol.N[0]):
+                return sol._N[-1] - ic.N_i
+            elif (np.size(sol._N_events['Collapse']) > 0 or
+                  sol._N_events['Inflation_dir-1_term1'] == sol._N[0]):
                 self.vprint("N_tot = %g for phi_i = %.15g" % (sol.N_tot, phi_i))
                 return 0 - self.N_tot
             elif 'step size' in sol.message:
                 raise StepSizeError(sol.message)
             else:
                 self.vprint("sol = %s" % sol)
                 raise PrimpyError("`solve_ivp` failed with message: %s" % sol.message)
@@ -267,30 +267,30 @@
                       InflationEvent(self.equations, direction=-1, terminal=True),
                       UntilNEvent(self.equations, self.N0),
                       CollapseEvent(self.equations)]
             with warnings.catch_warnings():
                 warnings.filterwarnings(action=self.warn_action, category=InflationWarning)
                 sol = solve(ic, events=events, **kwargs)
             if np.isfinite(sol.N_tot) and sol.N_tot > self.N_star:
-                sol.derive_approx_power(Omega_K0=self.Omega_K0, h=self.h)
+                sol.calibrate_scale_factor(Omega_K0=self.Omega_K0, h=self.h)
                 self.vprint("N_tot = %.15g, N_star = %.15g for phi_i = %.15g"
                             % (sol.N_tot, sol.N_star, phi_i))
                 return sol.N_star - self.N_star
-            elif np.size(sol.N_events['UntilN']) > 0 or sol.N[-1] >= self.N0:
+            elif np.size(sol._N_events['UntilN']) > 0 or sol._N[-1] >= self.N0:
                 self.vprint("N_tot > %g for phi_i = %.15g" % (self.N0, phi_i))
-                return sol.N[-1]
-            elif (np.size(sol.N_events['Collapse']) > 0 or sol.N_tot <= self.N_star or
-                  sol.N_events['Inflation_dir-1_term1'] == sol.N[0]):
+                return sol._N[-1]
+            elif (np.size(sol._N_events['Collapse']) > 0 or sol.N_tot <= self.N_star or
+                  sol._N_events['Inflation_dir-1_term1'] == sol._N[0]):
                 self.vprint("N_tot = %g for phi_i = %.15g" % (sol.N_tot, phi_i))
                 if sol.N_tot <= self.N_star:
                     self.vwarn(InflationWarning("Insufficient inflation: N_tot = %g < %g = N_star"
                                                 % (sol.N_tot, self.N_star)))
-                elif sol.N_events['Inflation_dir-1_term1'] == sol.N[0]:
-                    self.vwarn(InflationWarning("Universe has ended early: N[0]=%g, N_events=%s"
-                                                % (sol.N[0], sol.N_events)))
+                elif sol._N_events['Inflation_dir-1_term1'] == sol._N[0]:
+                    self.vwarn(InflationWarning("Universe has ended early: _N[0]=%g, _N_events=%s"
+                                                % (sol._N[0], sol._N_events)))
                 return 0 - self.N_star
             elif 'step size' in sol.message:
                 raise StepSizeError(sol.message)
             else:
                 self.vprint("sol = %s" % sol)
                 raise PrimpyError("`solve_ivp` failed with message: %s" % sol.message)
```

### Comparing `primpy-2.7.8/primpy/oscode_solver.py` & `primpy-2.8.0/primpy/oscode_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,23 @@
         return_pps = True
     PPS = PrimordialPowerSpectrum(background=b, k=k, **kwargs)
     # stop integration sufficiently after mode has crossed the horizon (lazy for loop):
     for i, ki in enumerate(k):
         if fac_beg == 0:
             idx_beg = 0
         else:
-            idx_beg = np.argwhere(np.log(ki) - b.logaH > np.log(fac_beg)).ravel()
+            idx_beg = np.argwhere(np.log(ki) - b._logaH > np.log(fac_beg)).ravel()
             # set idx_beg to 0 if horizon starts out too small:
             idx_beg = 0 if idx_beg.size == 0 else idx_beg[-1]
-        idx_end = np.argwhere(b.logaH - np.log(ki) > np.log(fac_end)).ravel()[0]
+        idx_end = np.argwhere(b._logaH - np.log(ki) > np.log(fac_end)).ravel()[0]
         # set minimum for idx_end, needed e.g. in KD for superhorizon modes:
-        idx_end = idx_end if idx_end - idx_beg > b.logaH.size//20 else idx_beg + b.logaH.size//20
+        idx_end = idx_end if idx_end - idx_beg > b._logaH.size//20 else idx_beg + b._logaH.size//20
         if b.independent_variable == 't':
             p = PerturbationT(background=b, k=ki, idx_beg=idx_beg, idx_end=idx_end, **kwargs)
-        elif b.independent_variable == 'N':
+        elif b.independent_variable == '_N':
             p = PerturbationN(background=b, k=ki, idx_beg=idx_beg, idx_end=idx_end, **kwargs)
         else:
             raise NotImplementedError()
         oscode_sol = []
         for mode in [p.scalar, p.tensor]:
             for num in range(2):
                 oscode_sol.append(pyoscode.solve(ts=b.x[idx_beg:idx_end+1],
```

### Comparing `primpy-2.7.8/primpy/parameters.py` & `primpy-2.8.0/primpy/parameters.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/primpy/perturbations.py` & `primpy-2.8.0/primpy/perturbations.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class PrimordialPowerSpectrum(object):
     """Primordial Power spectrum of curvature perturbations."""
 
     def __init__(self, background, k, **kwargs):
         self.background = background
         self.k = k
-        self.k_iMpc = k * K_STAR / np.exp(background.logaH_star)
+        self.k_iMpc = k * K_STAR / np.exp(background._logaH_star)
         vacuum = kwargs.pop('vacuum', ('RST',))
         for vac in vacuum:
             setattr(self, 'P_s_%s' % vac, np.full_like(k, np.nan, dtype=float))
             setattr(self, 'P_t_%s' % vac, np.full_like(k, np.nan, dtype=float))
 
 
 class Perturbation(ABC):
```

### Comparing `primpy-2.7.8/primpy/potentials.py` & `primpy-2.8.0/primpy/potentials.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/primpy/solver.py` & `primpy-2.8.0/primpy/solver.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/primpy/time/inflation.py` & `primpy-2.8.0/primpy/time/inflation.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,46 +10,46 @@
     Solves background variables in cosmic time for curved and flat universes
     using the Klein-Gordon and Friedmann equations.
 
     Independent variable:
         t: cosmic time
 
     Dependent variables:
-        N: number of e-folds
+        _N: number of e-folds
         phi: inflaton field
         dphidt: `d(phi)/dt`
 
     """
 
     def __init__(self, K, potential, track_eta=False, verbose=False):
         super(InflationEquationsT, self).__init__(K=K, potential=potential, verbose=verbose)
         self._set_independent_variable('t')
-        self.add_variable('phi', 'dphidt', 'N')
+        self.add_variable('phi', 'dphidt', '_N')
         self.track_eta = track_eta
         if track_eta:
             self.add_variable('eta')
 
     def __call__(self, x, y):
         """System of coupled ODEs for underlying variables."""
-        N = self.N(x, y)
+        N = self._N(x, y)
         H = self.H(x, y)
         dphidt = self.dphidt(x, y)
         dVdphi = self.dVdphi(x, y)
 
         dy = np.zeros_like(y)
         dy[self.idx['phi']] = dphidt
         dy[self.idx['dphidt']] = -3 * H * dphidt - dVdphi
-        dy[self.idx['N']] = H
+        dy[self.idx['_N']] = H
         if self.track_eta:
             dy[self.idx['eta']] = np.exp(-N)
         return dy
 
     def H2(self, x, y):
         """Compute the square of the Hubble parameter using the Friedmann equation."""
-        N = self.N(x, y)
+        N = self._N(x, y)
         V = self.V(x, y)
         dphidt = self.dphidt(x, y)
         return (dphidt**2 / 2 + V) / 3 - self.K * np.exp(-2 * N)
 
     def w(self, x, y):
         """Compute the equation of state parameter."""
         V = self.V(x, y)
```

### Comparing `primpy-2.7.8/primpy/time/perturbations.py` & `primpy-2.8.0/primpy/time/perturbations.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
         comoving curvature perturbations `R` w.r.t. time `t`, where the e.o.m. is
         written as `ddR + 2 * damping * dR + frequency**2 R = 0`.
 
         """
         K = self.background.K
-        N = self.background.N[self.idx_beg:self.idx_end+1]
+        N = self.background._N[self.idx_beg:self.idx_end+1]
         dphidt = self.background.dphidt[self.idx_beg:self.idx_end+1]
         H = self.background.H[self.idx_beg:self.idx_end+1]
         dV = self.background.potential.dV(self.background.phi[self.idx_beg:self.idx_end+1])
 
         kappa2 = self.k**2 + self.k * K * (K + 1) - 3 * K
         shared = 2 * kappa2 / (kappa2 + K * dphidt**2 / (2 * H**2))
         terms = dphidt**2 / (2 * H**2) - 3 - dV / (H * dphidt) - K * np.exp(-2 * N) / H**2
@@ -61,15 +61,15 @@
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping
         else:
             return np.sqrt(frequency2 + 0j), damping
 
     def get_vacuum_ic_RST(self):
         """Get initial conditions for scalar modes for RST vacuum w.r.t. cosmic time `t`."""
-        a_i = np.exp(self.background.N[self.idx_beg])
+        a_i = np.exp(self.background._N[self.idx_beg])
         dphidt_i = self.background.dphidt[self.idx_beg]
         H_i = self.background.H[self.idx_beg]
         z_i = a_i * dphidt_i / H_i
         Rk_i = 1 / np.sqrt(2 * self.k) / z_i
         dRk_i = -1j * self.k / a_i * Rk_i
         return Rk_i, dRk_i
 
@@ -90,21 +90,21 @@
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
         tensor perturbations `h` w.r.t. time `t`, where the e.o.m. is
         written as `ddh + 2 * damping * dh + frequency**2 h = 0`.
 
         """
         K = self.background.K
-        N = self.background.N[self.idx_beg:self.idx_end+1]
+        N = self.background._N[self.idx_beg:self.idx_end+1]
         frequency2 = (self.k**2 + self.k * K * (K + 1) + 2 * K) * np.exp(-2 * N)
         damping2 = 3 * self.background.H[self.idx_beg:self.idx_end+1]
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping2 / 2
         else:
             return np.sqrt(frequency2 + 0j), damping2 / 2
 
     def get_vacuum_ic_RST(self):
         """Get initial conditions for tensor modes for RST vacuum w.r.t. cosmic time `t`."""
-        a_i = np.exp(self.background.N[self.idx_beg])
+        a_i = np.exp(self.background._N[self.idx_beg])
         hk_i = 2 / np.sqrt(2 * self.k) / a_i
         dhk_i = -1j * self.k / a_i * hk_i
         return hk_i, dhk_i
```

### Comparing `primpy-2.7.8/primpy/units.py` & `primpy-2.8.0/primpy/units.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/primpy.egg-info/PKG-INFO` & `primpy-2.8.0/primpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primpy
-Version: 2.7.8
+Version: 2.8.0
 Summary: primpy: Calculations for the primordial Universe.
 Author: Lukas Hergt
 Author-email: lh561@mrao.cam.ac.uk
 License: MIT
 Keywords: PPS,cosmic inflation,initial conditions for inflation,kinetic dominance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 Requires-Dist: pyoscode
 
 ================================================
 primpy: calculations for the primordial Universe
 ================================================
 :primpy: calculations for the primordial Universe
 :Author: Lukas Hergt
-:Version: 2.7.8
+:Version: 2.8.0
 :Homepage: https://github.com/lukashergt/primpy
 :Documentation: https://primpy.readthedocs.io
 
 .. image:: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml/badge.svg?branch=master
     :target: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml
     :alt: Build Status
 .. image:: https://codecov.io/gh/lukashergt/primpy/branch/master/graph/badge.svg?token=USS4K53PY0
```

### Comparing `primpy-2.7.8/primpy.egg-info/SOURCES.txt` & `primpy-2.8.0/primpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/setup.py` & `primpy-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/tests/test_bigbang.py` & `primpy-2.8.0/tests/test_bigbang.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 
 def test_not_implemented_units():
     with pytest.raises(NotImplementedError):
         bb.get_H0(h=0.7, units='Mpc')
     with pytest.raises(NotImplementedError):
         bb.get_a0(h=0.7, Omega_K0=-0.01, units='H0')
+    with pytest.raises(NotImplementedError):
+        bb.Hubble_parameter(N=0, Omega_m0=0.3, Omega_K0=-0.01, h=0.7, units='Mpc')
+    with pytest.raises(NotImplementedError):
+        bb.comoving_Hubble_horizon(N=0, Omega_m0=0.3, Omega_K0=-0.01, h=0.7, units='spam')
 
 
 @pytest.mark.parametrize('h', [0.3, 0.5, 0.7, 0.9])
 def test_get_H0(h):
     """Tests for `get_H0`."""
     H0_km_per_Mpc_per_s = bb.get_H0(h=h, units='H0')
     H0_per_s = bb.get_H0(h=h, units='SI')
@@ -65,22 +69,24 @@
     pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
     t_i = 7e4
     eq = InflationEquationsT(K=K, potential=pot)
     ic = ISIC_Nt(eq, N_tot=N_tot, Omega_Ki=Omega_Ki, phi_i_bracket=(5, 30), t_i=t_i)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=True)]
     bist = solve(ic=ic, events=ev)
-    bist.derive_comoving_hubble_horizon(Omega_K0=Omega_K0, h=h)
-    N_end = bist.N[-1]
-    log_cHH_end = bist.log_cHH_end_lp
+    bist.calibrate_scale_factor(Omega_K0=Omega_K0, h=h)
 
     N_BBN = bb.get_N_BBN(h=h, Omega_K0=Omega_K0)
-    cHH_BBN = bb.comoving_Hubble_horizon(N=N_BBN, Omega_m0=0.3, Omega_K0=Omega_K0, h=h)
+    cHH_BBN_Mpc = bb.comoving_Hubble_horizon(N=N_BBN, Omega_m0=0.3, Omega_K0=Omega_K0, h=h,
+                                             units='Mpc')
 
-    w_reh = bb.get_w_reh(N1=N_end, N2=N_BBN, log_cHH1=log_cHH_end, log_cHH2=np.log(cHH_BBN))
+    w_reh, delta_reh = bb.get_w_delta_reh(N_end=bist.N_end,
+                                          N_reh=N_BBN,
+                                          log_cHH_end=np.log(bist.cHH_end_Mpc),
+                                          log_cHH_reh=np.log(cHH_BBN_Mpc))
     if N_tot < 15:
         assert w_reh < -1 / 3
     elif N_tot < 25:
         assert -1 / 3 < w_reh < 0
     elif N_tot < 65:
         assert 0 < w_reh < 1 / 3
     elif N_tot < 80:
@@ -92,17 +98,18 @@
 @pytest.mark.parametrize('h', [0.3, 0.5, 0.7, 0.9])
 def test_Omega_r0(h):
     assert 0 < bb.get_Omega_r0(h) < 1e-4 / h**2
 
 
 @pytest.mark.parametrize('h', [0.3, 0.5, 0.7, 0.9])
 @pytest.mark.parametrize('Omega_K0', [-0.15, -0.01, 0.01, 0.15])
-def test_Hubble_parameter(h, Omega_K0):
+@pytest.mark.parametrize('units', ['planck', 'H0', 'SI'])
+def test_Hubble_parameter(h, Omega_K0, units):
     N = np.linspace(0, 200, 201)
-    bb.Hubble_parameter(N=N, Omega_m0=0.3, Omega_K0=Omega_K0, h=h)
+    bb.Hubble_parameter(N=N, Omega_m0=0.3, Omega_K0=Omega_K0, h=h, units=units)
 
 
 def test_no_Big_Bang_line():
     assert 1 == bb.no_Big_Bang_line(Omega_m0=0)
     assert 2 == bb.no_Big_Bang_line(Omega_m0=0.5)
     bb.no_Big_Bang_line(Omega_m0=1)
     with pytest.raises(ValueError, match="Matter density can't be negative"):
@@ -113,37 +120,43 @@
     assert 0 == bb.expand_recollapse_line(Omega_m0=0)
     assert 0 == bb.expand_recollapse_line(Omega_m0=0.5)
     assert effequal(0) == bb.expand_recollapse_line(Omega_m0=1)
     with pytest.raises(ValueError, match="Matter density can't be negative"):
         bb.expand_recollapse_line(Omega_m0=-1)
 
 
-def test_Hubble_parameter_exceptions():
+def test_Hubble_parameter_exceptions(recwarn):
     N = np.linspace(0, 200, 201)
     with pytest.raises(BigBangError, match="no Big Bang"):
         bb.Hubble_parameter(N=N, Omega_m0=0, Omega_K0=-0.01, h=0.7)
-    with pytest.warns(BigBangWarning, match="Universe recollapses"):
-        bb.Hubble_parameter(N=N, Omega_m0=1, Omega_K0=0.01, h=0.7)
+    bb.Hubble_parameter(N=N, Omega_m0=1, Omega_K0=0.01, h=0.7)
+    assert recwarn.list[0].category is BigBangWarning
+    assert "Universe recollapses" in str(recwarn.list[0].message)
+    assert recwarn.list[1].category is RuntimeWarning
+    assert "invalid value encountered in sqrt" == str(recwarn.list[1].message)
 
 
 @pytest.mark.parametrize('h', [0.3, 0.5, 0.7, 0.9])
 @pytest.mark.parametrize('Omega_K0', [-0.15, -0.01, 0.01, 0.15])
 @pytest.mark.parametrize('units', ['planck', 'Mpc', 'SI'])
 def test_comoving_Hubble_horizon(h, Omega_K0, units):
     N = np.linspace(0, 200, 201)
     bb.comoving_Hubble_horizon(N=N, Omega_m0=0.3, Omega_K0=Omega_K0, h=h, units=units)
 
 
 @pytest.mark.parametrize('units', ['planck', 'Mpc', 'SI'])
-def test_comoving_Hubble_horizon_exceptions(units):
+def test_comoving_Hubble_horizon_exceptions(units, recwarn):
     N = np.linspace(0, 200, 201)
     with pytest.raises(BigBangError, match="no Big Bang"):
         bb.comoving_Hubble_horizon(N=N, Omega_m0=0, Omega_K0=-0.01, h=0.7, units=units)
-    with pytest.warns(BigBangWarning, match="Universe recollapses"):
-        bb.comoving_Hubble_horizon(N=N, Omega_m0=1, Omega_K0=0.01, h=0.7, units=units)
+    bb.comoving_Hubble_horizon(N=N, Omega_m0=1, Omega_K0=0.01, h=0.7, units=units)
+    assert recwarn.list[0].category is BigBangWarning
+    assert "Universe recollapses" in str(recwarn.list[0].message)
+    assert recwarn.list[1].category is RuntimeWarning
+    assert "invalid value encountered in sqrt" == str(recwarn.list[1].message)
 
 
 @pytest.mark.parametrize('h', [0.3, 0.5, 0.7, 0.9])
 @pytest.mark.parametrize('Omega_K0', [-0.15, -0.01, 0.01, 0.15])
 @pytest.mark.parametrize('N_BB', [60, 100])
 def test_conformal_time(h, Omega_K0, N_BB):
     eta1 = bb.conformal_time(N_start=N_BB, N=200, Omega_m0=0.3, Omega_K0=Omega_K0, h=h)[0]
@@ -151,21 +164,24 @@
     assert eta1 == pytest.approx(eta2)
 
     N = np.linspace(N_BB, 200, (200-N_BB)//10+1)
     etas = bb.conformal_time(N_start=N_BB, N=N, Omega_m0=0.3, Omega_K0=Omega_K0, h=h)
     assert etas[-2] == pytest.approx(etas[-1])
 
 
-def test_conformal_time_exceptions():
+def test_conformal_time_exceptions(recwarn):
     with pytest.raises(BigBangError, match="no Big Bang"):
         bb.conformal_time(N_start=100, N=200, Omega_m0=0, Omega_K0=-0.01, h=0.7)
-    with pytest.warns(BigBangWarning, match="Universe recollapses"):
-        bb.conformal_time(N_start=100, N=200, Omega_m0=1, Omega_K0=0.01, h=0.7)
     with pytest.raises(TypeError, match="`N` needs to be either float or np.ndarray"):
         bb.conformal_time(N_start=100, N=[150, 200], Omega_m0=1, Omega_K0=0.01, h=0.7)
+    bb.conformal_time(N_start=100, N=200, Omega_m0=1, Omega_K0=0.01, h=0.7)
+    assert recwarn.list[0].category is BigBangWarning
+    assert "Universe recollapses" in str(recwarn.list[0].message)
+    assert recwarn.list[1].category is RuntimeWarning
+    assert "invalid value encountered in sqrt" == str(recwarn.list[1].message)
 
 
 @pytest.mark.parametrize('Omega_m0', [0.2, 0.4])
 @pytest.mark.parametrize('h', [0.5, 0.7])
 @pytest.mark.parametrize('Omega_K0', [-0.15, -0.01, 0.01, 0.09])
 @pytest.mark.parametrize('f_i', [1, 10])
 def test_conformal_time_ratio(f_i, Omega_K0, h, Omega_m0):
@@ -178,15 +194,15 @@
 
     eq = InflationEquationsT(K=K, potential=pot, track_eta=True)
     ic_f = InflationStartIC(eq, Omega_Ki=Omega_Ki, phi_i=phi_i, t_i=t_i, eta_i=eta_i)
     ic_b = InflationStartIC(eq, Omega_Ki=Omega_Ki, phi_i=phi_i, t_i=t_i, eta_i=eta_i, x_end=1)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=True)]
     bist_f = solve(ic=ic_f, events=ev)
-    bist_f.derive_a0(Omega_K0=Omega_K0, h=h)
+    bist_f.calibrate_scale_factor(Omega_K0=Omega_K0, h=h)
     bist_b = solve(ic=ic_b, events=[UntilNEvent(eq, 0)])
     assert np.isclose(bist_b.eta[-1], bist_b.eta[-2])
 
     ratio = bb.conformal_time_ratio(Omega_m0=Omega_m0, Omega_K0=Omega_K0, h=h,
                                     b_forward=bist_f, b_backward=bist_b)
     if np.log10(f_i) < 0.5:
         assert ratio < 1
```

### Comparing `primpy-2.7.8/tests/test_efolds_inflation.py` & `primpy-2.8.0/tests/test_efolds_inflation.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/tests/test_equations.py` & `primpy-2.8.0/tests/test_equations.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,32 @@
         ic_forwards = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
         # integration backward in time:
         ic_backward = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i, x_end=1)
 
         # stop at end of inflation:
         ev_forwards = [InflationEvent(ic_forwards.equations, +1, terminal=False),
                        InflationEvent(ic_forwards.equations, -1, terminal=True)]
-        # stop when N = 0:
+        # stop when _N = 0:
         ev_backward = [UntilNEvent(ic_backward.equations, value=1, terminal=True)]
 
         b_forwards = solve(ic=ic_forwards, events=ev_forwards)
         b_backward = solve(ic=ic_backward, events=ev_backward)
 
         # time and e-folds grow monotonically forwards in time
         assert np.all(np.diff(b_forwards.x) > 0)
         assert np.all(np.diff(b_forwards.t) > 0)
-        assert np.all(np.diff(b_forwards.N) > 0)
+        assert np.all(np.diff(b_forwards._N) > 0)
         # phi shrinks monotonically forwards in time (from start to end of inflation)
         assert np.all(np.diff(b_forwards.y[eq.idx['phi']]) < 0)
         assert np.all(np.diff(b_forwards.phi) < 0)
 
         # time and e-folds shrink monotonically backwards in time
         assert np.all(np.diff(b_backward.x) < 0)
         assert np.all(np.diff(b_backward.t) < 0)
-        assert np.all(np.diff(b_backward.N) < 0)
+        assert np.all(np.diff(b_backward._N) < 0)
         # phi grows monotonically backwards in time (before start of inflation)
         assert np.all(np.diff(b_backward.y[eq.idx['phi']]) > 0)
         assert np.all(np.diff(b_backward.phi) > 0)
 
 
 @pytest.mark.filterwarnings("ignore:invalid value encountered in sqrt:RuntimeWarning")
 @pytest.mark.parametrize('K', [-1, 0, +1])
@@ -72,31 +72,31 @@
         ev = [CollapseEvent(ic.equations),
               InflationEvent(ic.equations, +1, terminal=False),
               InflationEvent(ic.equations, -1, terminal=False),
               UntilNEvent(ic.equations, N_end)]
         sol = solve(ic=ic, events=ev)
 
         assert hasattr(sol, 't_events')
-        assert hasattr(sol, 'N_events')
+        assert hasattr(sol, '_N_events')
         assert hasattr(sol, 'phi_events')
 
         for key, value in sol.y_events.items():
             if value.size == 0:
                 assert_equal(sol.t_events[key], value)
-                assert_equal(sol.N_events[key], value)
+                assert_equal(sol._N_events[key], value)
                 assert_equal(sol.phi_events[key], value)
                 if isinstance(eq, InflationEquationsT):
                     assert hasattr(sol, 'dphidt_events')
                     assert_equal(sol.dphidt_events[key], value)
                 elif isinstance(eq, InflationEquationsN):
                     assert hasattr(sol, 'dphidN_events')
                     assert_equal(sol.dphidN_events[key], value)
             else:
                 assert_equal(sol.phi_events[key], value[:, eq.idx['phi']])
                 if isinstance(eq, InflationEquationsT):
-                    assert_equal(sol.N_events[key], value[:, eq.idx['N']])
+                    assert_equal(sol._N_events[key], value[:, eq.idx['_N']])
                     assert hasattr(sol, 'dphidt_events')
                     assert_equal(sol.dphidt_events[key], value[:, eq.idx['dphidt']])
                 elif isinstance(eq, InflationEquationsN):
                     assert_equal(sol.t_events[key], value[:, eq.idx['t']])
                     assert hasattr(sol, 'dphidN_events')
                     assert_equal(sol.dphidN_events[key], value[:, eq.idx['dphidN']])
```

### Comparing `primpy-2.7.8/tests/test_events.py` & `primpy-2.8.0/tests/test_events.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     N_i = 10
     phi_i = 17
     N_end = 73
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [UntilNEvent(eq, N_end)]
     sol = solve(ic=ic, events=ev)
-    assert sol.N[-1] == approx(N_end)
-    assert sol.N_events['UntilN'][-1] == approx(N_end)
+    assert sol._N[-1] == approx(N_end)
+    assert sol._N_events['UntilN'][-1] == approx(N_end)
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Lambda', [1, 0.0025])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_InflationEvent(K, Lambda, Eq):
     t_i = 7e4
@@ -59,16 +59,16 @@
     phi_i = 17
     pot = QuadraticPotential(Lambda=Lambda)
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=True)]
     sol = solve(ic=ic, events=ev)
-    assert np.isfinite(sol.N_beg)
-    assert np.isfinite(sol.N_end)
+    assert np.isfinite(sol._N_beg)
+    assert np.isfinite(sol._N_end)
     assert sol.w[0] == approx(-1 / 3)
     assert sol.w[-1] == approx(-1 / 3)
     assert np.all(sol.w[1:-1] < -1 / 3)
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
@@ -79,21 +79,21 @@
     phi_i = 17
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=False),
           AfterInflationEndEvent(eq)]
     sol = solve(ic=ic, events=ev)
-    assert np.isfinite(sol.N_beg)
-    assert np.isfinite(sol.N_end)
+    assert np.isfinite(sol._N_beg)
+    assert np.isfinite(sol._N_end)
     assert sol.w[-1] == approx(0)
     assert np.all(sol.w[1:-1] < 0)
-    assert sol.N_events['Inflation_dir-1_term0'].size == 1
-    assert (sol.N_events['Inflation_dir-1_term0'][0] <
-            sol.N_events['AfterInflationEnd_dir1_term1'][0])
+    assert sol._N_events['Inflation_dir-1_term0'].size == 1
+    assert (sol._N_events['Inflation_dir-1_term0'][0] <
+            sol._N_events['AfterInflationEnd_dir1_term1'][0])
 
 
 @pytest.mark.filterwarnings("ignore:invalid value encountered in sqrt:RuntimeWarning")
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_Phi0Event(K, Eq):
     pot = QuadraticPotential(Lambda=0.0025)
@@ -102,13 +102,13 @@
     phi_i = 17
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=False),
           Phi0Event(eq)]
     sol = solve(ic=ic, events=ev)
-    assert np.isfinite(sol.N_beg)
-    assert np.isfinite(sol.N_end)
-    assert sol.N_events['Inflation_dir-1_term0'].size == 1
-    assert (sol.N_events['Inflation_dir-1_term0'][0] <
-            sol.N_events['Phi0_dir0_term1'][0])
+    assert np.isfinite(sol._N_beg)
+    assert np.isfinite(sol._N_end)
+    assert sol._N_events['Inflation_dir-1_term0'].size == 1
+    assert (sol._N_events['Inflation_dir-1_term0'][0] <
+            sol._N_events['Phi0_dir0_term1'][0])
     assert sol.phi[-1] == approx(0)
```

### Comparing `primpy-2.7.8/tests/test_exceptionhandling.py` & `primpy-2.8.0/tests/test_exceptionhandling.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/tests/test_inflation.py` & `primpy-2.8.0/tests/test_perturbations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,251 +1,247 @@
 #!/usr/bin/env python
-"""Tests for `primpy.inflation` module."""
+"""Tests for `primpy.perturbation` module."""
 import pytest
 from pytest import approx
-from scipy.interpolate import interp1d
 import numpy as np
 from numpy.testing import assert_allclose
-from primpy.exceptionhandling import InflationEndWarning
-from primpy.units import Mpc_m, lp_m
-from primpy.parameters import K_STAR
-from primpy.potentials import QuadraticPotential
-from primpy.events import InflationEvent, UntilNEvent
-from primpy.inflation import InflationEquations
+from primpy.potentials import QuadraticPotential, StarobinskyPotential
+from primpy.events import InflationEvent, CollapseEvent
 from primpy.time.inflation import InflationEquationsT
 from primpy.efolds.inflation import InflationEquationsN
-from primpy.initialconditions import InflationStartIC, ISIC_NsOk
+from primpy.initialconditions import InflationStartIC, SlowRollIC
+from primpy.time.perturbations import PerturbationT
+from primpy.efolds.perturbations import PerturbationN
 from primpy.solver import solve
+from primpy.oscode_solver import solve_oscode
 
 
-def test_not_implemented_errors():
-    eq = InflationEquations(K=1, potential=QuadraticPotential(Lambda=0.0025))
-    with pytest.raises(NotImplementedError, match="Equations must define H2 method."):
-        eq.H(x=0, y=np.zeros(4))
-    with pytest.raises(NotImplementedError, match="Equations must define H2 method."):
-        eq.H2(x=0, y=np.zeros(4))
-    with pytest.raises(NotImplementedError, match="Equations must define w method."):
-        eq.w(x=0, y=np.zeros(4))
-    with pytest.raises(NotImplementedError, match="Equations must define inflating method."):
-        eq.inflating(x=0, y=np.zeros(4))
-
-
-def test_track_eta():
-    pot = QuadraticPotential(Lambda=1)
-    N_i = 10
-    phi_i = 17
-    eta_i = 0
-    for K in [-1, 0, 1]:
-        for eq in [InflationEquationsT(K=K, potential=pot, track_eta=True),
-                   InflationEquationsN(K=K, potential=pot, track_eta=True)]:
-            assert eq.track_eta
-            assert hasattr(eq, 'phi')
-            assert hasattr(eq, 'N')
-            assert hasattr(eq, 'eta')
-            assert 'eta' in eq.idx
-            ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, eta_i=eta_i)
-            y0 = np.zeros(len(eq.idx))
-            ic(y0=y0)
-            dy0 = eq(x=ic.x_ini, y=y0)
-            if isinstance(eq, InflationEquationsT):
-                assert hasattr(eq, 'dphidt')
-                assert dy0.size == 4
-                assert dy0[eq.idx['eta']] == np.exp(-N_i)
-            elif isinstance(eq, InflationEquationsN):
-                assert hasattr(eq, 'dphidN')
-                assert dy0.size == 3
-                H2 = (2 * pot.V(phi_i) - 6 * K * np.exp(-2 * N_i)) / (6 - dy0[eq.idx['phi']]**2)
-                assert dy0[eq.idx['eta']] == np.exp(-N_i) / np.sqrt(H2)
-
-
-def test_basic_methods_time_vs_efolds():
-    tol = 1e-12
-    t = 1
-    N = 10
-    phi = 20
-    for K in [-1, 0, 1]:
-        for Lambda in [1, 0.0025]:
-            pot = QuadraticPotential(Lambda=Lambda)
-            for dphidt_squared in [100 * pot.V(phi), 2 * pot.V(phi), pot.V(phi), pot.V(phi) / 100]:
-                dphidt = -np.sqrt(dphidt_squared)
-                eq_t = InflationEquationsT(K=K, potential=pot)
-                eq_N = InflationEquationsN(K=K, potential=pot)
-                assert eq_t.idx['phi'] == 0
-                assert eq_t.idx['dphidt'] == 1
-                assert eq_t.idx['N'] == 2
-                assert eq_N.idx['phi'] == 0
-                assert eq_N.idx['dphidN'] == 1
-                y1_t = np.array([phi, dphidt, N])
-                y1_N = np.array([phi, dphidt / eq_t.H(t, y1_t)])
-                assert eq_t.H2(t, y1_t) == approx(eq_N.H2(N, y1_N), rel=tol, abs=tol)
-                assert eq_t.H(t, y1_t) == approx(eq_N.H(N, y1_N), rel=tol, abs=tol)
-                assert eq_t.V(t, y1_t) == approx(eq_N.V(N, y1_N), rel=tol, abs=tol)
-                assert eq_t.dVdphi(t, y1_t) == approx(eq_N.dVdphi(N, y1_N), rel=tol, abs=tol)
-                assert eq_t.d2Vdphi2(t, y1_t) == approx(eq_N.d2Vdphi2(N, y1_N), rel=tol, abs=tol)
-                assert eq_t.w(t, y1_t) == approx(eq_N.w(N, y1_N), rel=tol, abs=tol)
-                assert eq_t.inflating(t, y1_t) == approx(eq_N.inflating(N, y1_N), rel=tol, abs=tol)
-
-
-@pytest.mark.parametrize('K', [-1, 0, +1])
-def test_sol_time_efolds(K):
-    pot = QuadraticPotential(Lambda=0.0025)
-    N_i = 10
-    phi_i = 17
-    t_i = 7e4
-    eta_i = 0
-    h = 0.7
-    k = np.logspace(-3, 1, 4 * 10 + 1)
-    Omega_K0 = -K * 0.01
-
-    eq_t = InflationEquationsT(K=K, potential=pot, track_eta=True)
-    eq_N = InflationEquationsN(K=K, potential=pot, track_eta=True, track_time=True)
-    ic_t = InflationStartIC(eq_t, N_i=N_i, phi_i=phi_i, t_i=t_i, eta_i=eta_i)
-    ic_N = InflationStartIC(eq_N, N_i=N_i, phi_i=phi_i, t_i=t_i, eta_i=eta_i)
+def set_background_SR():
+    pot = StarobinskyPotential(Lambda=3.3e-3)
+    N_i = 0
+    phi_i = 5.6
+    N_star = 55
+
+    eq_t = InflationEquationsT(K=0, potential=pot)
+    eq_n = InflationEquationsN(K=0, potential=pot)
+    t_eval = np.logspace(np.log10(5e4), np.log10(2e7), int(1e5))
+    ic_t = SlowRollIC(eq_t, N_i=N_i, phi_i=phi_i, t_i=t_eval[0])
+    ic_n = SlowRollIC(eq_n, N_i=N_i, phi_i=phi_i, t_i=None)
+    N_eval = np.linspace(ic_n.N_i, 70, int(1e5))
     ev_t = [InflationEvent(eq_t, +1, terminal=False),
-            InflationEvent(eq_t, -1, terminal=True)]
-    ev_N = [InflationEvent(eq_N, +1, terminal=False),
-            InflationEvent(eq_N, -1, terminal=True)]
-    bist = solve(ic=ic_t, events=ev_t, dense_output=True, method='DOP853', rtol=1e-12)
-    bisn = solve(ic=ic_N, events=ev_N, dense_output=True, method='DOP853', rtol=1e-12)
-    assert bist.N_tot == approx(bisn.N_tot, rel=1e-5)
-
-    N2t = interp1d(bisn.N, bisn.t, kind='cubic')
-    N2phi = interp1d(bisn.N, bisn.phi, kind='cubic')
-    N2H = interp1d(bisn.N, bisn.H, kind='cubic')
-    assert_allclose(bist.t[1:-1], N2t(bist.N[1:-1]), rtol=1e-5)
-    assert_allclose(bist.phi[1:-1], N2phi(bist.N[1:-1]), rtol=1e-4)
-    assert_allclose(bist.H[1:-1], N2H(bist.N[1:-1]), rtol=1e-4)
-
-    bist.derive_a0(Omega_K0=Omega_K0, h=h)
-    bisn.derive_a0(Omega_K0=Omega_K0, h=h)
-    assert bist.K == K
-    assert bisn.K == K
-    assert bist.Omega_K0 == Omega_K0
-    assert bisn.Omega_K0 == Omega_K0
-    if K != 0:
-        assert bisn.a0_Mpc * Mpc_m == bisn.a0_lp * lp_m
-        bist.derive_comoving_hubble_horizon(Omega_K0=Omega_K0, h=h)
-        bisn.derive_comoving_hubble_horizon(Omega_K0=Omega_K0, h=h)
-        bist.derive_approx_power(Omega_K0=Omega_K0, h=h)
-        bisn.derive_approx_power(Omega_K0=Omega_K0, h=h)
-    elif K == 0:
-        assert bisn.a0 == 1
-        bist.derive_comoving_hubble_horizon(N_star=55)
-        bisn.derive_comoving_hubble_horizon(N_star=55)
-        bist.derive_approx_power(N_star=55)
-        bisn.derive_approx_power(N_star=55)
-    assert bist.N_star == approx(bisn.N_star, rel=1e-5)
-    assert bist.N_dagg == approx(bisn.N_dagg, rel=1e-5)
-    assert bist.A_s == approx(bisn.A_s, rel=1e-8)
-    assert bist.n_s == approx(bisn.n_s, rel=1e-5)
-    assert bist.n_run == approx(bisn.n_run, rel=1e-3)
-    assert bist.n_runrun == approx(bisn.n_runrun, rel=2e-1, abs=1e-6)
-    assert bist.A_t == approx(bisn.A_t, rel=1e-8)
-    assert bist.r == approx(bisn.r, rel=1e-5)
-    assert bist.n_t == approx(bisn.n_t, rel=1e-5)
-    assert_allclose(bist.logk2logP_s(np.log(k)), bisn.logk2logP_s(np.log(k)), rtol=1e-6)
-    assert_allclose(bist.logk2logP_t(np.log(k)), bisn.logk2logP_t(np.log(k)), rtol=1e-6)
-    assert_allclose(bist.P_s_approx(k) * 1e9, bisn.P_s_approx(k) * 1e9, rtol=1e-4)
-    assert_allclose(bist.P_t_approx(k) * 1e9, bisn.P_t_approx(k) * 1e9, rtol=1e-3)
-
-
-def nan_inflation_end(background_sol):
-    assert not np.isfinite(background_sol.N_end)
-    assert not np.isfinite(background_sol.phi_end)
-    assert not np.isfinite(background_sol.V_end)
-    assert not np.isfinite(background_sol.N_tot)
-    assert not hasattr(background_sol, 'inflation_mask')
-
-
-@pytest.mark.parametrize('K', [-1, 0, +1])
-@pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
-def test_postprocessing_inflation_end_warnings(K, Eq):
-    t_i = 1e4
-    N_i = 10
-    phi_i = 17
-    pot = QuadraticPotential(Lambda=0.0025)
-    eq = Eq(K=K, potential=pot, verbose=True)
-
-    # stop at N=20 to trigger "Inflation has not ended." warning:
-    ic_early_end = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
-    ev = [InflationEvent(ic_early_end.equations, +1, terminal=False),
-          InflationEvent(ic_early_end.equations, -1, terminal=True),
-          UntilNEvent(ic_early_end.equations, 20)]
-    with pytest.warns(InflationEndWarning, match="Still inflating"):
-        bist = solve(ic=ic_early_end, events=ev)
-    nan_inflation_end(background_sol=bist)
-
-    # no passing of InflationEvent(-1), i.e. inflation end not recorded
-    ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
-    ev_no_end = [InflationEvent(ic.equations, +1, terminal=False),
-                 UntilNEvent(ic.equations, N_i + 65)]
-    with pytest.warns(InflationEndWarning, match="Not tracking"):
-        bist = solve(ic=ic, events=ev_no_end)
-    nan_inflation_end(background_sol=bist)
+            InflationEvent(eq_t, -1, terminal=True),
+            CollapseEvent(eq_t)]
+    ev_n = [InflationEvent(eq_n, +1, terminal=False),
+            InflationEvent(eq_n, -1, terminal=True),
+            CollapseEvent(eq_n)]
+    bsrt = solve(ic=ic_t, events=ev_t, t_eval=t_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    bsrn = solve(ic=ic_n, events=ev_n, t_eval=N_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    bsrt.calibrate_scale_factor(N_star=N_star)
+    bsrn.calibrate_scale_factor(N_star=N_star)
+
+    return bsrt, bsrn
+
+
+def test_set_background_SR():
+    bsrt, bsrn = set_background_SR()
+    assert bsrt.independent_variable == 't'
+    assert bsrn.independent_variable == '_N'
+    assert bsrt.N_tot > bsrt.N_star + 10
+    assert bsrt.N_tot == approx(bsrn.N_tot)
+    assert bsrt.N_star == approx(bsrn.N_star)
+    assert bsrt._N_cross == approx(bsrn._N_cross, rel=1e-5)
+
+
+def test_perturbations_SR():
+    bsrt, bsrn = set_background_SR()
+    ks_iMpc = np.logspace(np.log10(5e-4), np.log10(5e0), 4 * 10 + 1)
+    logk_iMpc = np.log(ks_iMpc)
+    ks_cont = ks_iMpc * bsrt.a0_Mpc
+    pps_t = solve_oscode(background=bsrt, k=ks_cont, fac_beg=100, rtol=5e-5)
+    pps_n = solve_oscode(background=bsrn, k=ks_cont, fac_beg=100, rtol=5e-5, even_grid=True)
+    assert np.isfinite(pps_t.P_s_RST).all()
+    assert np.isfinite(pps_t.P_t_RST).all()
+    assert np.isfinite(pps_n.P_s_RST).all()
+    assert np.isfinite(pps_n.P_t_RST).all()
+
+    # time vs efolds
+    assert_allclose(pps_t.P_s_RST * 1e9, pps_n.P_s_RST * 1e9, rtol=1e-3, atol=1e-6)
+    assert_allclose(pps_t.P_t_RST * 1e9, pps_n.P_t_RST * 1e9, rtol=1e-3, atol=1e-6)
+
+    # oscode vs background
+    As_t_oscode = pps_t.P_s_RST[ks_iMpc.size//2]
+    As_n_oscode = pps_n.P_s_RST[ks_iMpc.size//2]
+    assert As_t_oscode == approx(bsrt.A_s, rel=5e-2)
+    assert As_n_oscode == approx(bsrn.A_s, rel=5e-2)
+    offt = bsrt.A_s / As_t_oscode
+    offn = bsrn.A_s / As_n_oscode
+    assert_allclose(np.log(pps_t.P_s_RST*offt), bsrt.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-6)
+    assert_allclose(np.log(pps_n.P_s_RST*offn), bsrn.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-6)
+    assert_allclose(np.log(pps_t.P_t_RST), bsrt.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-6)
+    assert_allclose(np.log(pps_n.P_t_RST), bsrn.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-6)
 
 
-def test_Ncross_nan():
+def set_background_IS(K, f_i, abs_Omega_K0):
     pot = QuadraticPotential(Lambda=0.0025)
-    N_i = 18
-    phi_i = 15
-    t_i = 7e4
-    h = 0.7
-    for K in [-1, +1]:
-        for eq in [InflationEquationsT(K=K, potential=pot),
-                   InflationEquationsN(K=K, potential=pot)]:
-            Omega_K0 = -K * 0.1
-            ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
-            ev = [InflationEvent(eq, +1, terminal=False),
-                  InflationEvent(eq, -1, terminal=True)]
-            b_sol = solve(ic=ic, events=ev)
-            b_sol.derive_approx_power(Omega_K0=Omega_K0, h=h)
-            assert np.log(K_STAR) < np.min(b_sol.logk)
-            assert np.isnan(b_sol.N_cross)
-            assert np.isnan(b_sol.N_star)
-            assert np.isnan(b_sol.N_dagg)
-
-
-@pytest.mark.parametrize('N_star', [30, 90])
-def test_approx_As_ns_nrun_r__with_tolerances_and_slow_roll(N_star):
-    K = +1
-    pot = QuadraticPotential(Lambda=0.0025)
-    t_i = 1e4
-    N_i = 10
-    Omega_K0 = -K * 0.01
+    phi_i = 16
+    Omega_K0 = -K * abs_Omega_K0
+    Omega_Ki = f_i * Omega_K0
     h = 0.7
 
-    rtols = np.array([1e-12, 2.4e-14])
-    As_range = np.zeros(rtols.size)
-    ns_range = np.zeros(rtols.size)
-    nrun_range = np.zeros(rtols.size)
-    r_range = np.zeros(rtols.size)
-
-    ns_slow_roll = 1 - 2 / N_star
-    r_slow_roll = 8 / N_star
-
-    for i, rtol in enumerate(rtols):
-        eq = InflationEquationsT(K=K, potential=pot)
-        ic = ISIC_NsOk(equations=eq, N_i=N_i, N_star=N_star, Omega_K0=Omega_K0, h=h, t_i=t_i,
-                       phi_i_bracket=[12, 30])
-        ev = [InflationEvent(ic.equations, +1, terminal=False),
-              InflationEvent(ic.equations, -1, terminal=True)]
-        bist = solve(ic=ic, events=ev, rtol=rtol)
-        bist.derive_approx_power(Omega_K0=Omega_K0, h=h)
-        n_s = bist.n_s
-        r = bist.r
-        assert np.isclose(bist.N_star, N_star)
-        assert np.isclose(n_s, ns_slow_roll, rtol=0.005)
-        assert np.isclose(r, r_slow_roll, rtol=0.005)
-        As_range[i] = bist.A_s
-        ns_range[i] = bist.n_s
-        nrun_range[i] = bist.n_run
-        r_range[i] = bist.r
-
-    assert_allclose(ns_range[0], ns_slow_roll, rtol=0.005)
-    assert_allclose(ns_range[1], ns_slow_roll, rtol=0.005)
-    assert_allclose(r_range[0], r_slow_roll, rtol=0.005)
-    assert_allclose(r_range[1], r_slow_roll, rtol=0.005)
-
-    assert_allclose(As_range[0], As_range[1], rtol=1e-4, atol=1e-9*1e-3)
-    assert_allclose(ns_range[0], ns_range[1], rtol=1e-4)
-    assert_allclose(nrun_range[0], nrun_range[1], rtol=1e-4, atol=1e-4)
-    assert_allclose(r_range[0], r_range[1], rtol=1e-4)
+    eq_t = InflationEquationsT(K=K, potential=pot)
+    eq_n = InflationEquationsN(K=K, potential=pot)
+    t_eval = np.logspace(np.log10(5e4), np.log10(4e6), int(5e4))
+    ic_t = InflationStartIC(eq_t, phi_i=phi_i, Omega_Ki=Omega_Ki, t_i=t_eval[0])
+    ic_n = InflationStartIC(eq_n, phi_i=phi_i, Omega_Ki=Omega_Ki, t_i=None)
+    N_eval = np.linspace(ic_n.N_i, 70, int(1e5))
+    ev_t = [InflationEvent(eq_t, +1, terminal=False),
+            InflationEvent(eq_t, -1, terminal=True),
+            CollapseEvent(eq_t)]
+    ev_n = [InflationEvent(eq_n, +1, terminal=False),
+            InflationEvent(eq_n, -1, terminal=True),
+            CollapseEvent(eq_n)]
+    bist = solve(ic=ic_t, events=ev_t, t_eval=t_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    bisn = solve(ic=ic_n, events=ev_n, t_eval=N_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    assert bist.independent_variable == 't'
+    assert bisn.independent_variable == '_N'
+    assert bist.N_tot == approx(bisn.N_tot)
+    bist.calibrate_scale_factor(Omega_K0=Omega_K0, h=h)
+    bisn.calibrate_scale_factor(Omega_K0=Omega_K0, h=h)
+    assert bist.a0_Mpc == approx(bisn.a0_Mpc)
+    assert bist.N_star == approx(bisn.N_star)
+
+    return bist, bisn
+
+
+@pytest.mark.parametrize('K', [-1, +1])
+@pytest.mark.parametrize('f_i', [10, 100])
+@pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
+def test_set_background_IS(K, f_i, abs_Omega_K0):
+    if -K * f_i * abs_Omega_K0 >= 1:
+        with pytest.raises(Exception):
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+    else:
+        set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+
+
+# noinspection DuplicatedCode
+@pytest.mark.parametrize('K', [-1, +1])
+@pytest.mark.parametrize('f_i', [10, 100])
+@pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
+@pytest.mark.parametrize('k_iMpc', np.logspace(-5, 0, 5 + 1))
+def test_perturbations_frequency_damping(K, f_i, abs_Omega_K0, k_iMpc):
+    if -K * f_i * abs_Omega_K0 >= 1:
+        with pytest.raises(Exception):
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+    else:
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        k = k_iMpc * bist.a0_Mpc
+        pert_t = PerturbationT(background=bist, k=k)
+        pert_n = PerturbationN(background=bisn, k=k)
+        assert pert_t.scalar.idx['Rk'] == 0
+        assert pert_n.scalar.idx['Rk'] == 0
+        assert pert_t.scalar.idx['dRk'] == 1
+        assert pert_n.scalar.idx['dRk'] == 1
+        assert pert_t.tensor.idx['hk'] == 0
+        assert pert_n.tensor.idx['hk'] == 0
+        assert pert_t.tensor.idx['dhk'] == 1
+        assert pert_n.tensor.idx['dhk'] == 1
+        with pytest.raises(NotImplementedError):
+            pert_t.scalar(bist.x[0], bist.y[0])
+        with pytest.raises(NotImplementedError):
+            pert_t.tensor(bist.x[0], bist.y[0])
+        with pytest.raises(NotImplementedError):
+            pert_n.scalar(bisn.x[0], bisn.y[0])
+        with pytest.raises(NotImplementedError):
+            pert_n.tensor(bisn.x[0], bisn.y[0])
+        freq_t, damp_t = pert_t.scalar.mukhanov_sasaki_frequency_damping()
+        freq_n, damp_n = pert_n.scalar.mukhanov_sasaki_frequency_damping()
+        assert np.all(freq_t > 0)
+        assert np.all(freq_n > 0)
+        assert np.isfinite(damp_t).all()
+        assert np.isfinite(damp_n).all()
+        freq_t, damp_t = pert_t.tensor.mukhanov_sasaki_frequency_damping()
+        freq_n, damp_n = pert_n.tensor.mukhanov_sasaki_frequency_damping()
+        assert np.all(freq_t > 0)
+        assert np.all(freq_n > 0)
+        assert np.isfinite(damp_t).all()
+        assert np.isfinite(damp_n).all()
+
+        pert_t = solve_oscode(background=bist, k=k, rtol=5e-5)
+        pert_n = solve_oscode(background=bisn, k=k, rtol=5e-5, even_grid=True)
+        for sol in ['one', 'two']:
+            assert np.all(np.isfinite(getattr(getattr(pert_t.scalar, sol), 't')))
+            assert np.all(np.isfinite(getattr(getattr(pert_n.scalar, sol), '_N')))
+            assert np.all(np.isfinite(getattr(getattr(pert_t.tensor, sol), 't')))
+            assert np.all(np.isfinite(getattr(getattr(pert_n.tensor, sol), '_N')))
+        assert pert_n.scalar.P_s_RST == approx(pert_t.scalar.P_s_RST, rel=2e-3)
+        assert pert_n.tensor.P_t_RST == approx(pert_t.tensor.P_t_RST, rel=2e-3)
+
+
+@pytest.mark.parametrize('K', [-1, +1])
+@pytest.mark.parametrize('f_i', [10])
+@pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
+def test_perturbations_discrete_time_efolds(K, f_i, abs_Omega_K0):
+    if -K * f_i * abs_Omega_K0 >= 1:
+        with pytest.raises(Exception):
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+    else:
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        ks_disc = np.concatenate((
+            np.arange(1, 10, 1),
+            np.arange(10, 100, 10),
+            np.arange(100, 1000, 100),
+            np.arange(1000, 10000, 1000),
+        ))
+        pps_t = solve_oscode(background=bist, k=ks_disc, rtol=5e-5)
+        pps_n = solve_oscode(background=bisn, k=ks_disc, rtol=5e-5, even_grid=True)
+        assert np.isfinite(pps_t.P_s_RST).all()
+        assert np.isfinite(pps_t.P_t_RST).all()
+        assert np.isfinite(pps_n.P_s_RST).all()
+        assert np.isfinite(pps_n.P_t_RST).all()
+        assert_allclose(np.log(pps_t.P_s_RST), np.log(pps_n.P_s_RST), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_t.P_t_RST), np.log(pps_n.P_t_RST), rtol=1e-3, atol=1e-8)
+
+
+@pytest.mark.parametrize('K', [-1, +1])
+@pytest.mark.parametrize('f_i', [10])
+@pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
+def test_perturbations_continuous_time_vs_efolds(K, f_i, abs_Omega_K0):
+    if -K * f_i * abs_Omega_K0 >= 1:
+        with pytest.raises(Exception):
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+    else:
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        ks_iMpc = np.logspace(-4, 0, 4 * 10 + 1)
+        ks_cont = ks_iMpc * bist.a0_Mpc
+        pps_t = solve_oscode(background=bist, k=ks_cont, rtol=1e-5)
+        pps_n = solve_oscode(background=bisn, k=ks_cont, rtol=1e-5, even_grid=True)
+        assert np.isfinite(pps_t.P_s_RST).all()
+        assert np.isfinite(pps_t.P_t_RST).all()
+        assert np.isfinite(pps_n.P_s_RST).all()
+        assert np.isfinite(pps_n.P_t_RST).all()
+        assert_allclose(pps_t.P_s_RST * 1e9, pps_n.P_s_RST * 1e9, rtol=1e-3, atol=1e-6)
+        assert_allclose(pps_t.P_t_RST * 1e9, pps_n.P_t_RST * 1e9, rtol=1e-3, atol=1e-6)
+
+
+@pytest.mark.parametrize('K', [-1, +1])
+@pytest.mark.parametrize('f_i', [10])
+@pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
+def test_perturbations_large_scales_pyoscode_vs_background(K, f_i, abs_Omega_K0):
+    if -K * f_i * abs_Omega_K0 >= 1:
+        with pytest.raises(Exception):
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+    else:
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        ks_iMpc = np.logspace(-1, 1, 51)
+        logk_iMpc = np.log(ks_iMpc)
+        ks_cont = ks_iMpc * bist.a0_Mpc
+        pps_t = solve_oscode(background=bist, k=ks_cont)
+        pps_n = solve_oscode(background=bisn, k=ks_cont, even_grid=True)
+        assert np.isfinite(pps_t.P_s_RST).all()
+        assert np.isfinite(pps_t.P_t_RST).all()
+        assert np.isfinite(pps_n.P_s_RST).all()
+        assert np.isfinite(pps_n.P_t_RST).all()
+        assert_allclose(np.log(pps_t.P_s_RST), bist.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_t.P_t_RST), bist.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_n.P_s_RST), bisn.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_n.P_t_RST), bisn.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-8)
```

### Comparing `primpy-2.7.8/tests/test_initialconditions.py` & `primpy-2.8.0/tests/test_initialconditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
     assert ic.N_star == N_star
     assert ic.Omega_K0 == Omega_K0
     assert ic.h == h
     ev = [InflationEvent(ic.equations, +1, terminal=False),
           InflationEvent(ic.equations, -1, terminal=True)]
     b = solve(ic=ic, events=ev)
-    b.derive_approx_power(Omega_K0=Omega_K0, h=h)
+    b.calibrate_scale_factor(Omega_K0=Omega_K0, h=h)
     assert b.N_tot > N_star
     assert pytest.approx(b.N_star) == N_star
 
     # for Omega_Ki:
     abs_Omega_Ki = 0.9
     Omega_Ki = -K * abs_Omega_Ki
     Omega_K0 = -K * 0.01
@@ -251,10 +251,10 @@
         assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
     assert ic.N_star == N_star
     assert ic.Omega_K0 == Omega_K0
     assert ic.h == h
     ev = [InflationEvent(ic.equations, +1, terminal=False),
           InflationEvent(ic.equations, -1, terminal=True)]
     b = solve(ic=ic, events=ev)
-    b.derive_approx_power(Omega_K0=Omega_K0, h=h)
+    b.calibrate_scale_factor(Omega_K0=Omega_K0, h=h)
     assert b.N_tot > N_star
     assert pytest.approx(b.N_star) == N_star
```

### Comparing `primpy-2.7.8/tests/test_potentials.py` & `primpy-2.8.0/tests/test_potentials.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/tests/test_time_inflation.py` & `primpy-2.8.0/tests/test_time_inflation.py`

 * *Files identical despite different names*

### Comparing `primpy-2.7.8/tests/test_version.py` & `primpy-2.8.0/tests/test_version.py`

 * *Files identical despite different names*

