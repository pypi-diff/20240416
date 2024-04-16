# Comparing `tmp/mpmath-1.3.0.tar.gz` & `tmp/mpmath-1.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpmath-1.3.0.tar", last modified: Tue Mar  7 16:47:06 2023, max compression
+gzip compressed data, was "mpmath-1.4.0a0.tar", last modified: Fri Feb 23 03:26:45 2024, max compression
```

## Comparing `mpmath-1.3.0.tar` & `mpmath-1.4.0a0.tar`

### file list

```diff
@@ -1,105 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.191945 mpmath-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-03-07 16:44:15.000000 mpmath-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8211 2023-03-07 16:47:06.191945 mpmath-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6905 2023-03-07 16:44:15.000000 mpmath-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.179945 mpmath-1.3.0/mpmath/
--rw-r--r--   0 runner    (1001) docker     (122)     8765 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.183945 mpmath-1.3.0/mpmath/calculus/
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8817 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/approximation.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/calculus.py
--rw-r--r--   0 runner    (1001) docker     (122)    20226 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/differentiation.py
--rw-r--r--   0 runner    (1001) docker     (122)    73306 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/extrapolation.py
--rw-r--r--   0 runner    (1001) docker     (122)    36056 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/inverselaplace.py
--rw-r--r--   0 runner    (1001) docker     (122)     9908 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/odes.py
--rw-r--r--   0 runner    (1001) docker     (122)    32856 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)     7877 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/polynomials.py
--rw-r--r--   0 runner    (1001) docker     (122)    42432 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/calculus/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (122)    15985 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/ctx_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/ctx_fp.py
--rw-r--r--   0 runner    (1001) docker     (122)    17211 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/ctx_iv.py
--rw-r--r--   0 runner    (1001) docker     (122)    49452 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/ctx_mp.py
--rw-r--r--   0 runner    (1001) docker     (122)    37815 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/ctx_mp_python.py
--rw-r--r--   0 runner    (1001) docker     (122)   283512 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/function_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.183945 mpmath-1.3.0/mpmath/functions/
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    37938 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/bessel.py
--rw-r--r--   0 runner    (1001) docker     (122)    42237 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/elliptic.py
--rw-r--r--   0 runner    (1001) docker     (122)    11644 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/expintegrals.py
--rw-r--r--   0 runner    (1001) docker     (122)     5273 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/factorials.py
--rw-r--r--   0 runner    (1001) docker     (122)    18100 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    51570 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/hypergeometric.py
--rw-r--r--   0 runner    (1001) docker     (122)    16097 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/orthogonal.py
--rw-r--r--   0 runner    (1001) docker     (122)     7633 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/qfunctions.py
--rw-r--r--   0 runner    (1001) docker     (122)    46184 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/rszeta.py
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)    37320 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/theta.py
--rw-r--r--   0 runner    (1001) docker     (122)    36410 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/zeta.py
--rw-r--r--   0 runner    (1001) docker     (122)    30858 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/functions/zetazeros.py
--rw-r--r--   0 runner    (1001) docker     (122)    29253 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/identification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.183945 mpmath-1.3.0/mpmath/libmp/
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    71469 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/gammazeta.py
--rw-r--r--   0 runner    (1001) docker     (122)    43861 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/libelefun.py
--rw-r--r--   0 runner    (1001) docker     (122)    36624 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/libhyper.py
--rw-r--r--   0 runner    (1001) docker     (122)    16688 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/libintmath.py
--rw-r--r--   0 runner    (1001) docker     (122)    26875 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/libmpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    45021 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/libmpf.py
--rw-r--r--   0 runner    (1001) docker     (122)    27622 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/libmp/libmpi.py
--rw-r--r--   0 runner    (1001) docker     (122)    18561 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/math2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.187945 mpmath-1.3.0/mpmath/matrices/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/matrices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18609 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/matrices/calculus.py
--rw-r--r--   0 runner    (1001) docker     (122)    24394 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/matrices/eigen.py
--rw-r--r--   0 runner    (1001) docker     (122)    58534 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/matrices/eigen_symmetric.py
--rw-r--r--   0 runner    (1001) docker     (122)    26958 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/matrices/linalg.py
--rw-r--r--   0 runner    (1001) docker     (122)    32331 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/matrices/matrices.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/rational.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.191945 mpmath-1.3.0/mpmath/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7228 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/extratest_gamma.py
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/extratest_zeta.py
--rw-r--r--   0 runner    (1001) docker     (122)     5189 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/runtests.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (122)     9187 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_calculus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     8834 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_division.py
--rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_eigen.py
--rw-r--r--   0 runner    (1001) docker     (122)     8778 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_eigen_symmetric.py
--rw-r--r--   0 runner    (1001) docker     (122)    26225 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_elliptic.py
--rw-r--r--   0 runner    (1001) docker     (122)    89997 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (122)    30955 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    96990 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_functions2.py
--rw-r--r--   0 runner    (1001) docker     (122)    27917 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_gammazeta.py
--rw-r--r--   0 runner    (1001) docker     (122)    10461 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_hp.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_identify.py
--rw-r--r--   0 runner    (1001) docker     (122)    17527 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_levin.py
--rw-r--r--   0 runner    (1001) docker     (122)    10440 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_mpmath.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (122)     5227 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (122)     3132 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_rootfinding.py
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_special.py
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_str.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_summation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4799 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_trig.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (122)     7868 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/tests/torture.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/usertools.py
--rw-r--r--   0 runner    (1001) docker     (122)    10627 2023-03-07 16:44:15.000000 mpmath-1.3.0/mpmath/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 16:47:06.179945 mpmath-1.3.0/mpmath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8211 2023-03-07 16:47:06.000000 mpmath-1.3.0/mpmath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-03-07 16:47:06.000000 mpmath-1.3.0/mpmath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 16:47:06.000000 mpmath-1.3.0/mpmath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-07 16:47:06.000000 mpmath-1.3.0/mpmath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-07 16:47:06.000000 mpmath-1.3.0/mpmath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-03-07 16:47:06.191945 mpmath-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-03-07 16:44:15.000000 mpmath-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.045758 mpmath-1.4.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.001758 mpmath-1.4.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.005758 mpmath-1.4.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    45246 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-02-23 03:26:45.045758 mpmath-1.4.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.005758 mpmath-1.4.0a0/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/demo/mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/demo/manydigits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/demo/pidigits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/demo/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/demo/taylor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.005758 mpmath-1.4.0a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/basics.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.009758 mpmath-1.4.0a0/docs/calculus/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/approximation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/differentiation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/inverselaplace.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/odes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/optimization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/polynomials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/calculus/sums_limits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    42543 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/cplot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.009758 mpmath-1.4.0a0/docs/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/bessel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/elliptic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/expintegrals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/gamma.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/hyperbolic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/hypergeometric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/numtheory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/orthogonal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/powers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/qfunctions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/trigonometric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/functions/zeta.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/general.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/identification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/matrices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20614 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.029758 mpmath-1.4.0a0/docs/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)    26596 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ai.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61953 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ai_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ai_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19451 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ber.png
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besseli.png
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besseli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35095 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besseli_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besseli_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23549 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselj.png
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37422 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselj_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselj_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15252 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselk.png
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30483 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselk_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/besselk_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bessely.png
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bessely.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40491 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bessely_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bessely_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25211 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bi.png
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67342 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bi_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/bi_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/buildplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33025 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/chebyt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/chebyt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22495 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/chebyu.png
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/chebyu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34810 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombf.png
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39897 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombf_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombf_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34197 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46092 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombg_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/coulombg_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellipe.png
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellipf.png
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellipf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellipk.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellipk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellippi.png
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ellippi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/gi.png
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/gi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57729 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/gi_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/gi_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26786 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36130 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel1_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel1_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27100 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35840 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel2_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hankel2_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25846 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hermite.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hermite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hi.png
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47358 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hi_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/hi_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ker.png
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/ker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77369 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/kleinj.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/kleinj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61723 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/kleinj2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/kleinj2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/laguerre.png
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/laguerre.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lambertw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lambertw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lambertw_c.png
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lambertw_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28034 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/legendre.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/legendre.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26654 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lommels1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lommels1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lommels2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/lommels2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/pcfd.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/pcfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm40.png
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm40.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37882 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm41.png
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm41.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51314 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm42.png
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm42.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48141 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm43.png
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm43.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41468 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm44.png
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plots/spherharm44.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23750 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/splot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/docs/technical.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.029758 mpmath-1.4.0a0/mpmath/
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.033758 mpmath-1.4.0a0/mpmath/calculus/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20351 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73554 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/extrapolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35967 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/inverselaplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/odes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32821 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42866 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/calculus/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16713 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/ctx_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/ctx_fp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16871 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/ctx_iv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47934 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/ctx_mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41848 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/ctx_mp_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)   290975 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/function_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.037758 mpmath-1.4.0a0/mpmath/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38031 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43324 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/elliptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/expintegrals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/factorials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51781 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/hypergeometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/orthogonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/qfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46176 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/rszeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37320 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36399 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/zeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30982 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/functions/zetazeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29215 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libfp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.037758 mpmath-1.4.0a0/mpmath/libmp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72083 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/gammazeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43349 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/libelefun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36153 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/libhyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/libintmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26664 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/libmpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41264 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/libmpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/libmp/libmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.037758 mpmath-1.4.0a0/mpmath/matrices/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/matrices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18851 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/matrices/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/matrices/eigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58229 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/matrices/eigen_symmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30585 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/matrices/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32091 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/matrices/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.045758 mpmath-1.4.0a0/mpmath/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19543 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_eigen_symmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_elliptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_extra_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_extra_zeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91214 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33698 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98912 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_functions2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_gammazeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_hp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17401 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_levin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_mpmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_rootfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_summation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_torture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_trig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/usertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/mpmath/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 03:26:45.045758 mpmath-1.4.0a0/mpmath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-02-23 03:26:44.000000 mpmath-1.4.0a0/mpmath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-02-23 03:26:44.000000 mpmath-1.4.0a0/mpmath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 03:26:44.000000 mpmath-1.4.0a0/mpmath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-23 03:26:44.000000 mpmath-1.4.0a0/mpmath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-23 03:26:44.000000 mpmath-1.4.0a0/mpmath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 03:21:56.000000 mpmath-1.4.0a0/mpmath.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-02-23 03:21:04.000000 mpmath-1.4.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 03:26:45.045758 mpmath-1.4.0a0/setup.cfg
```

### Comparing `mpmath-1.3.0/LICENSE` & `mpmath-1.4.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2005-2021 Fredrik Johansson and mpmath contributors
+Copyright (c) 2005-2024 Fredrik Johansson and mpmath contributors
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
   a. Redistributions of source code must retain the above copyright notice,
```

### Comparing `mpmath-1.3.0/PKG-INFO` & `mpmath-1.4.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 Metadata-Version: 2.1
 Name: mpmath
-Version: 1.3.0
+Version: 1.4.0a0
 Summary: Python library for arbitrary-precision floating-point arithmetic
-Home-page: http://mpmath.org/
-Author: Fredrik Johansson
-Author-email: fredrik.johansson@gmail.com
+Author-email: Fredrik Johansson <fredrik.johansson@gmail.com>
 License: BSD
-Project-URL: Source, https://github.com/fredrik-johansson/mpmath
-Project-URL: Tracker, https://github.com/fredrik-johansson/mpmath/issues
+Project-URL: Homepage, https://mpmath.org/
+Project-URL: Source Code, https://github.com/mpmath/mpmath
+Project-URL: Bug Tracker, https://github.com/mpmath/mpmath/issues
 Project-URL: Documentation, http://mpmath.org/doc/current/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: tests
+Requires-Dist: pytest>=6; extra == "tests"
+Requires-Dist: numpy<=1.25.2; python_version < "3.12" and extra == "tests"
 Provides-Extra: develop
+Requires-Dist: mpmath[tests]; extra == "develop"
+Requires-Dist: flake518>=1.5; python_version >= "3.9" and extra == "develop"
+Requires-Dist: pytest-cov; extra == "develop"
+Requires-Dist: wheel; extra == "develop"
+Requires-Dist: build; extra == "develop"
 Provides-Extra: gmpy
+Requires-Dist: gmpy2>=2.1.0a4; (platform_python_implementation != "PyPy" and python_version < "3.12") and extra == "gmpy"
+Requires-Dist: gmpy2>=2.2.0a1; (platform_python_implementation != "PyPy" and python_version >= "3.12") and extra == "gmpy"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Provides-Extra: ci
+Requires-Dist: pytest-xdist; extra == "ci"
 
 mpmath
 ======
 
 |pypi version| |Build status| |Code coverage status| |Zenodo Badge|
 
 .. |pypi version| image:: https://img.shields.io/pypi/v/mpmath.svg
    :target: https://pypi.python.org/pypi/mpmath
-.. |Build status| image:: https://github.com/fredrik-johansson/mpmath/workflows/test/badge.svg
-   :target: https://github.com/fredrik-johansson/mpmath/actions?workflow=test
-.. |Code coverage status| image:: https://codecov.io/gh/fredrik-johansson/mpmath/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/fredrik-johansson/mpmath
+.. |Build status| image:: https://github.com/mpmath/mpmath/workflows/test/badge.svg
+   :target: https://github.com/mpmath/mpmath/actions?workflow=test
+.. |Code coverage status| image:: https://codecov.io/gh/mpmath/mpmath/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/mpmath/mpmath
 .. |Zenodo Badge| image:: https://zenodo.org/badge/2934512.svg
    :target: https://zenodo.org/badge/latestdoi/2934512
 
 A Python library for arbitrary-precision floating-point arithmetic.
 
-Website: http://mpmath.org/
+Website: https://mpmath.org/
 Main author: Fredrik Johansson <fredrik.johansson@gmail.com>
 
 Mpmath is free software released under the New BSD License (see the
-LICENSE file for details)
+LICENSE file for details).
 
 0. History and credits
 ----------------------
 
 The following people (among others) have contributed major patches
 or new features to mpmath:
 
@@ -113,14 +125,15 @@
   implementations.
 * George Brandl for developing the Sphinx documentation tool
   used to build mpmath's documentation
 
 Release history:
 
 * Version 1.3.0 released on March 7, 2023
+* Version 1.2.1 released on February 9, 2021
 * Version 1.2.0 released on February 1, 2021
 * Version 1.1.0 released on December 11, 2018
 * Version 1.0.0 released on September 27, 2017
 * Version 0.19 released on June 10, 2014
 * Version 0.18 released on December 31, 2013
 * Version 0.17 released on February 1, 2011
 * Version 0.16 released on September 24, 2010
@@ -139,66 +152,58 @@
 * Version 0.3 released on October 5, 2007
 * Version 0.2 released on October 2, 2007
 * Version 0.1 released on September 27, 2007
 
 1. Download & installation
 --------------------------
 
-Mpmath requires Python 2.7 or 3.5 (or later versions). It has been tested
-with CPython 2.7, 3.5 through 3.7 and for PyPy.
+Mpmath requires Python 3.8 or later versions. It has been tested
+with CPython 3.8 through 3.12 and for PyPy.
 
 The latest release of mpmath can be downloaded from the mpmath
-website and from https://github.com/fredrik-johansson/mpmath/releases
+website and from https://github.com/mpmath/mpmath/releases
 
 It should also be available in the Python Package Index at
 https://pypi.python.org/pypi/mpmath
 
 To install latest release of Mpmath with pip, simply run
 
 ``pip install mpmath``
 
-Or unpack the mpmath archive and run
-
-``python setup.py install``
-
-Mpmath can also be installed using
+or from the source tree
 
-``python -m easy_install mpmath``
+``pip install .``
 
 The latest development code is available from
-https://github.com/fredrik-johansson/mpmath
+https://github.com/mpmath/mpmath
 
 See the main documentation for more detailed instructions.
 
-2. Running tests
+2. Documentation
 ----------------
 
-The unit tests in mpmath/tests/ can be run via the script
-runtests.py, but it is recommended to run them with py.test
-(https://pytest.org/), especially
-to generate more useful reports in case there are failures.
+Documentation in reStructuredText format is available in the
+docs directory included with the source package. These files
+are human-readable, but can be compiled to prettier HTML using
+`Sphinx <https://www.sphinx-doc.org/>`_.
 
-You may also want to check out the demo scripts in the demo
-directory.
+The most recent documentation is also available in HTML format:
 
-The master branch is automatically tested by Travis CI.
+https://mpmath.org/doc/current/
 
-3. Documentation
+3. Running tests
 ----------------
 
-Documentation in reStructuredText format is available in the
-doc directory included with the source package. These files
-are human-readable, but can be compiled to prettier HTML using
-the build.py script (requires Sphinx, http://sphinx.pocoo.org/).
-
-See setup.txt in the documentation for more information.
+The unit tests in mpmath/tests/ can be run with `pytest
+<https://pytest.org/>`_, see the main documentation.
 
-The most recent documentation is also available in HTML format:
+You may also want to check out the demo scripts in the demo
+directory.
 
-http://mpmath.org/doc/current/
+The master branch is automatically tested on the Github Actions.
 
 4. Known problems
 -----------------
 
 Mpmath is a work in progress. Major issues include:
 
 * Some functions may return incorrect values when given extremely
@@ -215,11 +220,11 @@
 * The interface for switching precision and rounding is not finalized.
   The current method is not threadsafe.
 
 5. Help and bug reports
 -----------------------
 
 General questions and comments can be sent to the mpmath mailinglist,
-mpmath@googlegroups.com
+mailto:mpmath@googlegroups.com
 
 You can also report bugs and send patches to the mpmath issue tracker,
-https://github.com/fredrik-johansson/mpmath/issues
+https://github.com/mpmath/mpmath/issues
```

### Comparing `mpmath-1.3.0/README.rst` & `mpmath-1.4.0a0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 mpmath
 ======
 
 |pypi version| |Build status| |Code coverage status| |Zenodo Badge|
 
 .. |pypi version| image:: https://img.shields.io/pypi/v/mpmath.svg
    :target: https://pypi.python.org/pypi/mpmath
-.. |Build status| image:: https://github.com/fredrik-johansson/mpmath/workflows/test/badge.svg
-   :target: https://github.com/fredrik-johansson/mpmath/actions?workflow=test
-.. |Code coverage status| image:: https://codecov.io/gh/fredrik-johansson/mpmath/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/fredrik-johansson/mpmath
+.. |Build status| image:: https://github.com/mpmath/mpmath/workflows/test/badge.svg
+   :target: https://github.com/mpmath/mpmath/actions?workflow=test
+.. |Code coverage status| image:: https://codecov.io/gh/mpmath/mpmath/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/mpmath/mpmath
 .. |Zenodo Badge| image:: https://zenodo.org/badge/2934512.svg
    :target: https://zenodo.org/badge/latestdoi/2934512
 
 A Python library for arbitrary-precision floating-point arithmetic.
 
-Website: http://mpmath.org/
+Website: https://mpmath.org/
 Main author: Fredrik Johansson <fredrik.johansson@gmail.com>
 
 Mpmath is free software released under the New BSD License (see the
-LICENSE file for details)
+LICENSE file for details).
 
 0. History and credits
 ----------------------
 
 The following people (among others) have contributed major patches
 or new features to mpmath:
 
@@ -82,14 +82,15 @@
   implementations.
 * George Brandl for developing the Sphinx documentation tool
   used to build mpmath's documentation
 
 Release history:
 
 * Version 1.3.0 released on March 7, 2023
+* Version 1.2.1 released on February 9, 2021
 * Version 1.2.0 released on February 1, 2021
 * Version 1.1.0 released on December 11, 2018
 * Version 1.0.0 released on September 27, 2017
 * Version 0.19 released on June 10, 2014
 * Version 0.18 released on December 31, 2013
 * Version 0.17 released on February 1, 2011
 * Version 0.16 released on September 24, 2010
@@ -108,66 +109,58 @@
 * Version 0.3 released on October 5, 2007
 * Version 0.2 released on October 2, 2007
 * Version 0.1 released on September 27, 2007
 
 1. Download & installation
 --------------------------
 
-Mpmath requires Python 2.7 or 3.5 (or later versions). It has been tested
-with CPython 2.7, 3.5 through 3.7 and for PyPy.
+Mpmath requires Python 3.8 or later versions. It has been tested
+with CPython 3.8 through 3.12 and for PyPy.
 
 The latest release of mpmath can be downloaded from the mpmath
-website and from https://github.com/fredrik-johansson/mpmath/releases
+website and from https://github.com/mpmath/mpmath/releases
 
 It should also be available in the Python Package Index at
 https://pypi.python.org/pypi/mpmath
 
 To install latest release of Mpmath with pip, simply run
 
 ``pip install mpmath``
 
-Or unpack the mpmath archive and run
+or from the source tree
 
-``python setup.py install``
-
-Mpmath can also be installed using
-
-``python -m easy_install mpmath``
+``pip install .``
 
 The latest development code is available from
-https://github.com/fredrik-johansson/mpmath
+https://github.com/mpmath/mpmath
 
 See the main documentation for more detailed instructions.
 
-2. Running tests
+2. Documentation
 ----------------
 
-The unit tests in mpmath/tests/ can be run via the script
-runtests.py, but it is recommended to run them with py.test
-(https://pytest.org/), especially
-to generate more useful reports in case there are failures.
+Documentation in reStructuredText format is available in the
+docs directory included with the source package. These files
+are human-readable, but can be compiled to prettier HTML using
+`Sphinx <https://www.sphinx-doc.org/>`_.
 
-You may also want to check out the demo scripts in the demo
-directory.
+The most recent documentation is also available in HTML format:
 
-The master branch is automatically tested by Travis CI.
+https://mpmath.org/doc/current/
 
-3. Documentation
+3. Running tests
 ----------------
 
-Documentation in reStructuredText format is available in the
-doc directory included with the source package. These files
-are human-readable, but can be compiled to prettier HTML using
-the build.py script (requires Sphinx, http://sphinx.pocoo.org/).
-
-See setup.txt in the documentation for more information.
+The unit tests in mpmath/tests/ can be run with `pytest
+<https://pytest.org/>`_, see the main documentation.
 
-The most recent documentation is also available in HTML format:
+You may also want to check out the demo scripts in the demo
+directory.
 
-http://mpmath.org/doc/current/
+The master branch is automatically tested on the Github Actions.
 
 4. Known problems
 -----------------
 
 Mpmath is a work in progress. Major issues include:
 
 * Some functions may return incorrect values when given extremely
@@ -184,11 +177,11 @@
 * The interface for switching precision and rounding is not finalized.
   The current method is not threadsafe.
 
 5. Help and bug reports
 -----------------------
 
 General questions and comments can be sent to the mpmath mailinglist,
-mpmath@googlegroups.com
+mailto:mpmath@googlegroups.com
 
 You can also report bugs and send patches to the mpmath issue tracker,
-https://github.com/fredrik-johansson/mpmath/issues
+https://github.com/mpmath/mpmath/issues
```

### Comparing `mpmath-1.3.0/mpmath/__init__.py` & `mpmath-1.4.0a0/mpmath/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-__version__ = '1.3.0'
+from importlib.metadata import version
+
+__version__ = version(__name__)
+del version
+
+import functools
+import sys
+import types
 
 from .usertools import monitor, timing
 
 from .ctx_fp import FPContext
 from .ctx_mp import MPContext
 from .ctx_iv import MPIntervalContext
 
@@ -168,14 +175,15 @@
 eigsy = mp.eigsy
 eighe = mp.eighe
 eigh = mp.eigh
 svd_r = mp.svd_r
 svd_c = mp.svd_c
 svd = mp.svd
 gauss_quadrature = mp.gauss_quadrature
+rank = mp.rank
 
 expm = mp.expm
 sqrtm = mp.sqrtm
 powm = mp.powm
 logm = mp.logm
 sinm = mp.sinm
 cosm = mp.cosm
@@ -303,14 +311,16 @@
 bernpoly = mp.bernpoly
 eulerpoly = mp.eulerpoly
 eulernum = mp.eulernum
 polylog = mp.polylog
 clsin = mp.clsin
 clcos = mp.clcos
 gammainc = mp.gammainc
+lower_gamma = mp.lower_gamma
+upper_gamma = mp.upper_gamma
 gammaprod = mp.gammaprod
 binomial = mp.binomial
 rf = mp.rf
 ff = mp.ff
 hyper = mp.hyper
 hyp0f1 = mp.hyp0f1
 hyp1f1 = mp.hyp1f1
@@ -428,41 +438,23 @@
 stirling2 = mp.stirling2
 squarew = mp.squarew
 trianglew = mp.trianglew
 sawtoothw = mp.sawtoothw
 unit_triangle = mp.unit_triangle
 sigmoid = mp.sigmoid
 
-# be careful when changing this name, don't use test*!
-def runtests():
-    """
-    Run all mpmath tests and print output.
-    """
-    import os.path
-    from inspect import getsourcefile
-    from .tests import runtests as tests
-    testdir = os.path.dirname(os.path.abspath(getsourcefile(tests)))
-    importdir = os.path.abspath(testdir + '/../..')
-    tests.testit(importdir, testdir)
-
-def doctests(filter=[]):
-    import sys
-    from timeit import default_timer as clock
-    for i, arg in enumerate(sys.argv):
-        if '__init__.py' in arg:
-            filter = [sn for sn in sys.argv[i+1:] if not sn.startswith("-")]
-            break
-    import doctest
-    globs = globals().copy()
-    for obj in globs: #sorted(globs.keys()):
-        if filter:
-            if not sum([pat in obj for pat in filter]):
-                continue
-        sys.stdout.write(str(obj) + " ")
-        sys.stdout.flush()
-        t1 = clock()
-        doctest.run_docstring_examples(globs[obj], {}, verbose=("-v" in sys.argv))
-        t2 = clock()
-        print(round(t2-t1, 3))
 
-if __name__ == '__main__':
-    doctests()
+# Hack to guard against setting module properties instead of 'mp', Issue #657
+class _MPMathModule(types.ModuleType):
+
+    def _helper(self, *args, prop=''):
+        raise AttributeError("cannot set '{name}' on 'mpmath'. Did you mean to "
+                             "set '{name}' on 'mpmath.mp'?".format(name=prop))
+
+    dps = property(fset=functools.partial(_helper, prop='dps'))
+    prec = property(fset=functools.partial(_helper, prop='prec'))
+    pretty = property(fset=functools.partial(_helper, prop='pretty'))
+    trap_complex = property(fset=functools.partial(_helper, prop='trap_complex'))
+
+
+sys.modules[__name__].__class__ = _MPMathModule
+del functools, sys, types
```

### Comparing `mpmath-1.3.0/mpmath/calculus/approximation.py` & `mpmath-1.4.0a0/mpmath/calculus/approximation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ..libmp.backend import xrange
 from .calculus import defun
 
 #----------------------------------------------------------------------------#
 #                              Approximation methods                         #
 #----------------------------------------------------------------------------#
 
 # The Chebyshev approximation formula is given at:
@@ -56,16 +55,16 @@
     into a fast machine-precision version of the same.)
 
     **Examples**
 
     Here we use :func:`~mpmath.chebyfit` to generate a low-degree approximation
     of `f(x) = \cos(x)`, valid on the interval `[1, 2]`::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, chebyfit, cos, nprint, polyval
+        >>> mp.pretty = True
         >>> poly, err = chebyfit(cos, [1, 2], 5, error=True)
         >>> nprint(poly)
         [0.00291682, 0.146166, -0.732491, 0.174141, 0.949553]
         >>> nprint(err, 12)
         1.61351758081e-5
 
     The polynomial can be evaluated using ``polyval``::
@@ -158,16 +157,17 @@
     **Examples**
 
     The function `f(x) = x` has a simple Fourier series on the standard
     interval `[-\pi, \pi]`. The cosine coefficients are all zero (because
     the function has odd symmetry), and the sine coefficients are
     rational numbers::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (mp, fourier, pi, nprint, plot, cosh, quad,
+        ...                     sqrt, fourierval)
+        >>> mp.pretty = True
         >>> c, s = fourier(lambda x: x, [-pi, pi], 5)
         >>> nprint(c)
         [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
         >>> nprint(s)
         [0.0, 2.0, -1.0, 0.666667, -0.5, 0.4]
 
     This computes a Fourier series of a nonsymmetric function on
@@ -209,15 +209,15 @@
     interval = ctx._as_points(interval)
     a = interval[0]
     b = interval[-1]
     L = b-a
     cos_series = []
     sin_series = []
     cutoff = ctx.eps*10
-    for n in xrange(N+1):
+    for n in range(N+1):
         m = 2*n*ctx.pi/L
         an = 2*ctx.quadgl(lambda t: f(t)*ctx.cos(m*t), interval)/L
         bn = 2*ctx.quadgl(lambda t: f(t)*ctx.sin(m*t), interval)/L
         if n == 0:
             an /= 2
         if abs(an) < cutoff: an = ctx.zero
         if abs(bn) < cutoff: bn = ctx.zero
@@ -237,10 +237,10 @@
     """
     cs, ss = series
     ab = ctx._as_points(interval)
     a = interval[0]
     b = interval[-1]
     m = 2*ctx.pi/(ab[-1]-ab[0])
     s = ctx.zero
-    s += ctx.fsum(cs[n]*ctx.cos(m*n*x) for n in xrange(len(cs)) if cs[n])
-    s += ctx.fsum(ss[n]*ctx.sin(m*n*x) for n in xrange(len(ss)) if ss[n])
+    s += ctx.fsum(cs[n]*ctx.cos(m*n*x) for n in range(len(cs)) if cs[n])
+    s += ctx.fsum(ss[n]*ctx.sin(m*n*x) for n in range(len(ss)) if ss[n])
     return s
```

### Comparing `mpmath-1.3.0/mpmath/calculus/differentiation.py` & `mpmath-1.4.0a0/mpmath/calculus/differentiation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ..libmp.backend import xrange
 from .calculus import defun
 
 try:
     iteritems = dict.iteritems
 except AttributeError:
     iteritems = dict.items
 
@@ -19,15 +18,15 @@
     .. math ::
 
         \Delta^n = \sum_{k=0}^{\infty} (-1)^{k+n} {n \choose k} s_k.
     """
     n = int(n)
     d = ctx.zero
     b = (-1) ** (n & 1)
-    for k in xrange(n+1):
+    for k in range(n+1):
         d += b * s[k]
         b = (b * (k-n)) // (k+1)
     return d
 
 def hsteps(ctx, f, x, n, prec, **options):
     singular = options.get('singular')
     addprec = options.get('addprec', 10)
@@ -45,19 +44,19 @@
             h = ctx.ldexp(1, -prec-addprec-hextramag)
         else:
             h = ctx.convert(h)
         # Directed: steps x, x+h, ... x+n*h
         direction = options.get('direction', 0)
         if direction:
             h *= ctx.sign(direction)
-            steps = xrange(n+1)
+            steps = range(n+1)
             norm = h
         # Central: steps x-n*h, x-(n-2)*h ..., x, ..., x+(n-2)*h, x+n*h
         else:
-            steps = xrange(-n, n+1, 2)
+            steps = range(-n, n+1, 2)
             norm = (2*h)
         # Perturb
         if singular:
             x += 0.5*h
         values = [f(x+k*h) for k in steps]
         return values, norm, workprec
     finally:
@@ -67,16 +66,16 @@
 @defun
 def diff(ctx, f, x, n=1, **options):
     r"""
     Numerically computes the derivative of `f`, `f'(x)`, or generally for
     an integer `n \ge 0`, the `n`-th derivative `f^{(n)}(x)`.
     A few basic examples are::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, diff, nprint, sqrt, cos, exp, j, chop
+        >>> mp.pretty = True
         >>> diff(lambda x: x**2 + x, 1.0)
         3.0
         >>> diff(lambda x: x**2 + x, 1.0, 2)
         2.0
         >>> diff(lambda x: x**2 + x, 1.0, 3)
         0.0
         >>> nprint([diff(exp, 3, n) for n in range(5)])   # exp'(x) = exp(x)
@@ -150,15 +149,15 @@
 
         >>> diff(abs, 0, direction=j)
         (0.0 - 1.0j)
 
     With integration, the result may have a small imaginary part
     even even if the result is purely real::
 
-        >>> diff(sqrt, 1, method='quad')    # doctest:+ELLIPSIS
+        >>> diff(sqrt, 1, method='quad')
         (0.5 - 4.59...e-26j)
         >>> chop(_)
         0.5
 
     Adding precision to obtain an accurate value::
 
         >>> diff(cos, 1e-30)
@@ -239,16 +238,15 @@
     needed derivatives is known in advance, this is further
     slightly more efficient.
 
     Options are the same as for :func:`~mpmath.diff`.
 
     **Examples**
 
-        >>> from mpmath import *
-        >>> mp.dps = 15
+        >>> from mpmath import nprint, diffs, cos
         >>> nprint(list(diffs(cos, 1, 5)))
         [0.540302, -0.841471, -0.540302, 0.841471, 0.540302, -0.841471]
         >>> for i, d in zip(range(6), diffs(cos, 1)):
         ...     print("%s %s" % (i, d))
         ...
         0 0.54030230586814
         1 -0.841470984807897
@@ -278,15 +276,15 @@
     if n == ctx.inf:
         A, B = 1, 2
     else:
         A, B = 1, n+1
     while 1:
         callprec = ctx.prec
         y, norm, workprec = hsteps(ctx, f, x, B, callprec, **options)
-        for k in xrange(A, B):
+        for k in range(A, B):
             try:
                 ctx.prec = workprec
                 d = ctx.difference(y, k) / norm**k
             finally:
                 ctx.prec = callprec
             yield +d
             if k >= n:
@@ -294,15 +292,15 @@
         A, B = B, int(A*1.4+1)
         B = min(B, n)
 
 def iterable_to_function(gen):
     gen = iter(gen)
     data = []
     def f(k):
-        for i in xrange(len(data), k+1):
+        for i in range(len(data), k+1):
             data.append(next(gen))
         return data[k]
     return f
 
 @defun
 def diffs_prod(ctx, factors):
     r"""
@@ -316,16 +314,16 @@
     admit direct computation.
 
     Note: This function does not increase the working precision internally,
     so guard digits may have to be added externally for full accuracy.
 
     **Examples**
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, exp, sin, cos, diffs
+        >>> mp.pretty = True
         >>> f = lambda x: exp(x)*cos(x)*sin(x)
         >>> u = diffs(f, 1)
         >>> v = mp.diffs_prod([diffs(exp,1), diffs(cos,1), diffs(sin,1)])
         >>> next(u); next(v)
         1.23586333600241
         1.23586333600241
         >>> next(u); next(v)
@@ -344,18 +342,18 @@
         for c in factors[0]:
             yield c
     else:
         u = iterable_to_function(ctx.diffs_prod(factors[:N//2]))
         v = iterable_to_function(ctx.diffs_prod(factors[N//2:]))
         n = 0
         while 1:
-            #yield sum(binomial(n,k)*u(n-k)*v(k) for k in xrange(n+1))
+            #yield sum(binomial(n,k)*u(n-k)*v(k) for k in range(n+1))
             s = u(n) * v(0)
             a = 1
-            for k in xrange(1,n+1):
+            for k in range(1,n+1):
                 a = a * (n-k+1) // k
                 s += a * u(n-k) * v(k)
             yield s
             n += 1
 
 def dpoly(n, _cache={}):
     """
@@ -404,16 +402,16 @@
     so guard digits may have to be added externally for full accuracy.
 
     **Examples**
 
     The derivatives of the gamma function can be computed using
     logarithmic differentiation::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, loggamma, diffs_exp, diffs, gamma, psi
+        >>> mp.pretty = True
         >>>
         >>> def diffs_loggamma(x):
         ...     yield loggamma(x)
         ...     i = 0
         ...     while 1:
         ...         yield psi(i,x)
         ...         i += 1
@@ -472,16 +470,17 @@
 
     **Examples**
 
     There is an exact formula for the fractional derivative of a
     monomial `x^p`, which may be used as a reference. For example,
     the following gives a half-derivative (order 0.5)::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (mp, mpf, differint, gamma, inf, exp, pi,
+        ...                     j, lower_gamma)
+        >>> mp.pretty = True
         >>> x = mpf(3); p = 2; n = 0.5
         >>> differint(lambda t: t**p, x, n)
         7.81764019044672
         >>> gamma(p+1)/gamma(p-n+1) * x**(p-n)
         7.81764019044672
 
     Another useful test function is the exponential function, whose
@@ -504,15 +503,15 @@
     Riemann-Liouville differintegral::
 
         >>> x = mpf(3.5)
         >>> c = pi
         >>> n = 1+2*j
         >>> differint(lambda x: exp(c*x), x, n)
         (-123295.005390743 + 140955.117867654j)
-        >>> x**(-n) * exp(c)**x * (x*c)**n * gammainc(-n, 0, x*c) / gamma(-n)
+        >>> x**(-n) * exp(c)**x * (x*c)**n * lower_gamma(-n, x*c) / gamma(-n)
         (-123295.005390743 + 140955.117867654j)
 
 
     """
     m = max(int(ctx.ceil(ctx.re(n)))+1, 1)
     r = m-n-1
     g = lambda x: ctx.quad(lambda t: (x-t)**r * f(t), [x0, x])
@@ -520,16 +519,16 @@
 
 @defun
 def diffun(ctx, f, n=1, **options):
     r"""
     Given a function `f`, returns a function `g(x)` that evaluates the nth
     derivative `f^{(n)}(x)`::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import diffun, sin, cos, mp
+        >>> mp.pretty = True
         >>> cos2 = diffun(sin)
         >>> sin2 = diffun(sin, 4)
         >>> cos(1.3), cos2(1.3)
         (0.267498828624587, 0.267498828624587)
         >>> sin(1.3), sin2(1.3)
         (0.963558185417193, 0.963558185417193)
 
@@ -545,16 +544,16 @@
 
 @defun
 def taylor(ctx, f, x, n, **options):
     r"""
     Produces a degree-`n` Taylor polynomial around the point `x` of the
     given function `f`. The coefficients are returned as a list.
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, sin, nprint, chop, exp, polyval, taylor
+        >>> mp.pretty = True
         >>> nprint(chop(taylor(sin, 0, 5)))
         [0.0, 1.0, 0.0, -0.166667, 0.0, 0.00833333]
 
     The coefficients are computed using high-order numerical
     differentiation. The function must be possible to evaluate
     to arbitrary precision. See :func:`~mpmath.diff` for additional details
     and supported keyword options.
@@ -596,16 +595,16 @@
         A(x) Q(x) = P(x) + O(x^{L+M+1})
 
     `P(x)/Q(x)` can provide a good approximation to an analytic function
     beyond the radius of convergence of its Taylor series (example
     from G.A. Baker 'Essentials of Pade Approximants' Academic Press,
     Ch.1A)::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, mpf, sqrt, taylor, pade, polyval
+        >>> mp.pretty = True
         >>> one = mpf(1)
         >>> def f(x):
         ...     return sqrt((one + 2*x)/(one + x))
         ...
         >>> a = taylor(f, 0, 6)
         >>> p, q = pade(a, 3, 3)
         >>> x = 10
```

### Comparing `mpmath-1.3.0/mpmath/calculus/extrapolation.py` & `mpmath-1.4.0a0/mpmath/calculus/extrapolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-try:
-    from itertools import izip
-except ImportError:
-    izip = zip
-
-from ..libmp.backend import xrange
 from .calculus import defun
 
-try:
-    next = next
-except NameError:
-    next = lambda _: _.next()
 
 @defun
 def richardson(ctx, seq):
     r"""
     Given a list ``seq`` of the first `N` elements of a slowly convergent
     infinite sequence, :func:`~mpmath.richardson` computes the `N`-term
     Richardson extrapolate for the limit.
@@ -52,15 +42,15 @@
     three elements do not differ monotonically, and in that case
     applies extrapolation only to the even-index elements.
 
     **Example**
 
     Applying Richardson extrapolation to the Leibniz series for `\pi`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, mpf, richardson, nprint, pi
         >>> mp.dps = 30; mp.pretty = True
         >>> S = [4*sum(mpf(-1)**n/(2*n+1) for n in range(m))
         ...     for m in range(1,30)]
         >>> v, c = richardson(S[:10])
         >>> v
         3.2126984126984126984126984127
         >>> nprint([v-pi, c])
@@ -84,15 +74,15 @@
     N = len(seq)//2-1
     s = ctx.zero
     # The general weight is c[k] = (N+k)**N * (-1)**(k+N) / k! / (N-k)!
     # To avoid repeated factorials, we simplify the quotient
     # of successive weights to obtain a recurrence relation
     c = (-1)**N * N**N / ctx.mpf(ctx._ifac(N))
     maxc = 1
-    for k in xrange(N+1):
+    for k in range(N+1):
         s += c * seq[N+k]
         maxc = max(abs(c), maxc)
         c *= (k-N)*ctx.mpf(k+N+1)**N
         c /= ((1+k)*ctx.mpf(k+N)**N)
     return s, maxc
 
 @defun
@@ -171,15 +161,15 @@
     (TODO: find a better solution to this problem.)
 
     **Examples**
 
     We illustrate by applying Shanks transformation to the Leibniz
     series for `\pi`::
 
-        >>> from mpmath import *
+        >>> from mpmath import shanks, mp, nprint, mpf, pi
         >>> mp.dps = 50
         >>> S = [4*sum(mpf(-1)**n/(2*n+1) for n in range(m))
         ...     for m in range(1,30)]
         >>>
         >>> T = shanks(S[:7])
         >>> for row in T:
         ...     nprint(row)
@@ -236,17 +226,17 @@
         STOP -= 1
     one = ctx.one
     eps = +ctx.eps
     if randomized:
         from random import Random
         rnd = Random()
         rnd.seed(START)
-    for i in xrange(START, STOP):
+    for i in range(START, STOP):
         row = []
-        for j in xrange(i+1):
+        for j in range(i+1):
             if j == 0:
                 a, b = 0, seq[i+1]-seq[i]
             else:
                 if j == 1:
                     a = seq[i]
                 else:
                     a = table[i-1][j-2]
@@ -364,15 +354,14 @@
     must be chosen.
 
     **Examples**
 
     First we sum the zeta function::
 
         >>> from mpmath import mp
-        >>> mp.prec = 53
         >>> eps = mp.mpf(mp.eps)
         >>> with mp.extraprec(2 * mp.prec): # levin needs a high working precision
         ...     L = mp.levin(method = "levin", variant = "u")
         ...     S, s, n = [], 0, 1
         ...     while 1:
         ...         s += mp.one / (n * n)
         ...         n += 1
@@ -446,15 +435,15 @@
         ...         v, e = L.step_psum(s)
         ...         if e < eps:
         ...             break
         ...         if n > 1000: raise RuntimeError("iteration limit exceeded")
         >>> print(mp.chop(v - exact))
         0.0
         >>> w = mp.nsum(lambda n: (-z)**n * mp.fac(4 * n) / (mp.fac(n) * mp.fac(2 * n) * (4 ** n)),
-        ...   [0, mp.inf], method = "levin", levin_variant = "t", workprec = 8*mp.prec, steps = [2] + [1 for x in xrange(1000)])
+        ...   [0, mp.inf], method = "levin", levin_variant = "t", workprec = 8*mp.prec, steps = [2] + [1 for x in range(1000)])
         >>> print(mp.chop(v - w))
         0.0
 
     These examples run with 15-20 decimal digits precision. For higher precision the
     working precision must be raised.
 
     **Examples for nsum**
@@ -478,15 +467,15 @@
     Hypergeometric series can also be summed outside their range of convergence.
     The stepsize in :func:`~mpmath.nsum` must not be chosen too large, otherwise it will miss the
     point where the Levin transform converges resulting in numerical overflow/garbage::
 
         >>> z = 2 + 1j
         >>> exact = mp.hyp2f1(2 / mp.mpf(3), 4 / mp.mpf(3), 1 / mp.mpf(3), z)
         >>> f = lambda n: mp.rf(2 / mp.mpf(3), n) * mp.rf(4 / mp.mpf(3), n) * z**n / (mp.rf(1 / mp.mpf(3), n) * mp.fac(n))
-        >>> v = mp.nsum(f, [0, mp.inf], method = "levin", steps = [10 for x in xrange(1000)])
+        >>> v = mp.nsum(f, [0, mp.inf], method = "levin", steps = [10 for x in range(1000)])
         >>> print(mp.chop(exact-v))
         0.0
 
     References:
 
       [1] E.J. Weniger - "Nonlinear Sequence Transformations for the Acceleration of
           Convergence and the Summation of Divergent Series" arXiv:math/0306302
@@ -834,15 +823,15 @@
         n = len(A)
         d = (3 + self.ctx.sqrt(8)) ** n
         d = (d + 1 / d) / 2
         b = -self.ctx.one
         c = -d
         s = 0
 
-        for k in xrange(n):
+        for k in range(n):
             c = b - c
             if k % 2 == 0:
                 s = s + c * A[k]
             else:
                 s = s - c * A[k]
             b = 2 * (k + n) * (k - n) * b / ((2 * k + 1) * (k + self.ctx.one))
 
@@ -870,15 +859,15 @@
 
         n = len(S)
         d = (3 + self.ctx.sqrt(8)) ** n
         d = (d + 1 / d) / 2
         b = self.ctx.one
         s = 0
 
-        for k in xrange(n):
+        for k in range(n):
             b = 2 * (n + k) * (n - k) * b / ((2 * k + 1) * (k + self.ctx.one))
             s += b * S[k]
 
         value = s / d
 
         err = abs(value - self.last)
         self.last = value
@@ -912,15 +901,16 @@
 
     **Examples**
 
     The Abel-Plana formula is particularly useful when the summand
     decreases like a power of `k`; for example when the sum is a pure
     zeta function::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, sumap, zeta, inf, chop, expint, log,
+        ...                     polylog)
         >>> mp.dps = 25; mp.pretty = True
         >>> sumap(lambda k: 1/k**2.5, [1,inf])
         1.34148725725091717975677
         >>> zeta(2.5)
         1.34148725725091717975677
         >>> sumap(lambda k: 1/(k+1j)**(2.5+2.5j), [1,inf])
         (-3.385361068546473342286084 - 0.7432082105196321803869551j)
@@ -1011,15 +1001,15 @@
     `f(a), f'(a), f''(a), \ldots` (and the equivalent for `b`).
 
     **Examples**
 
     Summation of an infinite series, with automatic and symbolic
     integral and derivative values (the second should be much faster)::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, sumem, inf, fac, mpf
         >>> mp.dps = 50; mp.pretty = True
         >>> sumem(lambda n: 1/n**2, [32, inf])
         0.03174336652030209012658168043874142714132886413417
         >>> I = mpf(1)/32
         >>> D = adiffs=((-1)**n*fac(n+1)*32**(-2-n) for n in range(999))
         >>> sumem(lambda n: 1/n**2, [32, inf], integral=I, adiffs=D)
         0.03174336652030209012658168043874142714132886413417
@@ -1035,24 +1025,24 @@
     tol = tol or +ctx.eps
     interval = ctx._as_points(interval)
     a = ctx.convert(interval[0])
     b = ctx.convert(interval[-1])
     err = ctx.zero
     prev = 0
     M = 10000
-    if a == ctx.ninf: adiffs = (0 for n in xrange(M))
+    if a == ctx.ninf: adiffs = (0 for n in range(M))
     else:             adiffs = adiffs or ctx.diffs(f, a)
-    if b == ctx.inf:  bdiffs = (0 for n in xrange(M))
+    if b == ctx.inf:  bdiffs = (0 for n in range(M))
     else:             bdiffs = bdiffs or ctx.diffs(f, b)
     orig = ctx.prec
     #verbose = 1
     try:
         ctx.prec += 10
         s = ctx.zero
-        for k, (da, db) in enumerate(izip(adiffs, bdiffs)):
+        for k, (da, db) in enumerate(zip(adiffs, bdiffs)):
             if k & 1:
                 term = (db-da) * ctx.bernoulli(k+1) / ctx.factorial(k+1)
                 mag = abs(term)
                 if verbose:
                     print("term", k, "magnitude =", ctx.nstr(mag))
                 if k > 4 and mag < tol:
                     s += term
@@ -1095,17 +1085,17 @@
         tol = option('tol', ctx.eps*2**10)
     else:
         tol = option('tol', ctx.eps/2**10)
     verbose = option('verbose', False)
     maxterms = option('maxterms', ctx.dps*10)
     method = set(option('method', 'r+s').split('+'))
     skip = option('skip', 0)
-    steps = iter(option('steps', xrange(10, 10**9, 10)))
+    steps = iter(option('steps', range(10, 10**9, 10)))
     strict = option('strict')
-    #steps = (10 for i in xrange(1000))
+    #steps = (10 for i in range(1000))
     summer=[]
     if 'd' in method or 'direct' in method:
         TRY_RICHARDSON = TRY_SHANKS = TRY_EULER_MACLAURIN = False
     else:
         TRY_RICHARDSON = ('r' in method) or ('richardson' in method)
         TRY_SHANKS = ('s' in method) or ('shanks' in method)
         TRY_EULER_MACLAURIN = ('e' in method) or \
@@ -1158,15 +1148,15 @@
             try:
                 step = next(steps)
             except StopIteration:
                 pass
             if verbose:
                 print("-"*70)
                 print("Adding terms #%i-#%i" % (index, index+step))
-            update(partial, xrange(index, index+step))
+            update(partial, range(index, index+step))
             index += step
 
             # Check direct error
             best = partial[-1]
             error = abs(best - partial[-2])
             if verbose:
                 print("Direct error: %s" % ctx.nstr(error))
@@ -1260,16 +1250,17 @@
 
     if multiple intervals are given.
 
     Two examples of infinite series that can be summed by :func:`~mpmath.nsum`,
     where the first converges rapidly and the second converges slowly,
     are::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (mp, fac, inf, nsum, sin, cos, zeta, mpf, pi,
+        ...                     log, sqrt, diff, ln2, altzeta, sech)
+        >>> mp.pretty = True
         >>> nsum(lambda n: 1/fac(n), [0, inf])
         2.71828182845905
         >>> nsum(lambda n: 1/n**2, [1, inf])
         1.64493406684823
 
     When appropriate, :func:`~mpmath.nsum` applies convergence acceleration to
     accurately estimate the sums of slowly convergent series. If the series is
@@ -1504,25 +1495,25 @@
     numerical cancellation.
 
       >>> mp.dps = 15
       >>> z = mp.mpf(2)
       >>> # exact = mp.quad(lambda x: mp.exp( -x * x / 2 - z * x ** 4), [0,mp.inf]) * 2 / mp.sqrt(2 * mp.pi)
       >>> exact = mp.exp(mp.one / (32 * z)) * mp.besselk(mp.one / 4, mp.one / (32 * z)) / (4 * mp.sqrt(z * mp.pi)) # this is the symbolic expression for the integral
       >>> w = mp.nsum(lambda n: (-z)**n * mp.fac(4 * n) / (mp.fac(n) * mp.fac(2 * n) * (4 ** n)),
-      ...   [0, mp.inf], method = "levin", levin_variant = "t", workprec = 8*mp.prec, steps = [2] + [1 for x in xrange(1000)])
+      ...   [0, mp.inf], method = "levin", levin_variant = "t", workprec = 8*mp.prec, steps = [2] + [1 for x in range(1000)])
       >>> print(mp.chop(w - exact))
       0.0
 
     The hypergeoemtric function can also be summed outside its range of convergence:
 
       >>> mp.dps = 15
       >>> z = 2 + 1j
       >>> exact = mp.hyp2f1(2 / mp.mpf(3), 4 / mp.mpf(3), 1 / mp.mpf(3), z)
       >>> f = lambda n: mp.rf(2 / mp.mpf(3), n) * mp.rf(4 / mp.mpf(3), n) * z**n / (mp.rf(1 / mp.mpf(3), n) * mp.fac(n))
-      >>> v = mp.nsum(f, [0, mp.inf], method = "levin", steps = [10 for x in xrange(1000)])
+      >>> v = mp.nsum(f, [0, mp.inf], method = "levin", steps = [10 for x in range(1000)])
       >>> print(mp.chop(exact-v))
       0.0
 
     **Examples with Cohen's alternating series resummation**
 
       The next example sums the alternating zeta function:
 
@@ -1763,15 +1754,15 @@
         yield tuple(prod)
 
 def fold_finite(ctx, f, intervals):
     if not intervals:
         return f
     indices = [v[0] for v in intervals]
     points = [v[1] for v in intervals]
-    ranges = [xrange(a, b+1) for (a,b) in points]
+    ranges = [range(a, b+1) for (a,b) in points]
     def g(*args):
         args = list(args)
         s = ctx.zero
         for xs in cartesian_product(ranges):
             for dim, x in zip(indices, xs):
                 args[dim] = ctx.mpf(x)
             s += f(*args)
@@ -1818,19 +1809,19 @@
     def g(*args):
         args = list(args)
         #args.insert(dim2, None)
         n = int(args[dim1])
         s = ctx.zero
         #y = ctx.mpf(n)
         args[dim2] = ctx.mpf(n) #y
-        for x in xrange(n+1):
+        for x in range(n+1):
             args[dim1] = ctx.mpf(x)
             s += f(*args)
         args[dim1] = ctx.mpf(n) #ctx.mpf(n)
-        for y in xrange(n):
+        for y in range(n):
             args[dim2] = ctx.mpf(y)
             s += f(*args)
         return s
     #print "Folded infinite from", len(intervals), "to", (len(intervals)-1)
     return fold_infinite(ctx, g, intervals[:-1])
 
 @defun
@@ -1859,15 +1850,16 @@
     also required (and used automatically) when Euler-Maclaurin
     summation is requested.
 
     **Examples**
 
     A simple finite product::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, nprod, inf, csch, cosh, exp, pi, sinh,
+        ...                     sqrt, exp, euler, cos, tanh, log, jtheta)
         >>> mp.dps = 25; mp.pretty = True
         >>> nprod(lambda k: k, [1, 4])
         24.0
 
     A large number of infinite products have known exact values,
     and can therefore be used as a reference. Most of the following
     examples are taken from MathWorld [1].
@@ -1978,15 +1970,15 @@
 
     a, b = ctx._as_points(interval)
     if a == ctx.ninf:
         if b == ctx.inf:
             return f(0) * ctx.nprod(lambda k: f(-k) * f(k), [1, ctx.inf], **kwargs)
         return ctx.nprod(f, [-b, ctx.inf], **kwargs)
     elif b != ctx.inf:
-        return ctx.fprod(f(ctx.mpf(k)) for k in xrange(int(a), int(b)+1))
+        return ctx.fprod(f(ctx.mpf(k)) for k in range(int(a), int(b)+1))
 
     a = int(a)
 
     def update(partial_products, indices):
         if partial_products:
             pprod = partial_products[-1]
         else:
@@ -2038,15 +2030,16 @@
     are extremely close to the limit point (or if infinite,
     very large arguments).
 
     **Examples**
 
     A basic evaluation of a removable singularity::
 
-        >>> from mpmath import *
+        >>> from mpmath import (limit, mp, sin, inf, exp, fac, sqrt, pi, e,
+        ...                     mpf, log, euler)
         >>> mp.dps = 30; mp.pretty = True
         >>> limit(lambda x: (x-sin(x))/x**3, 0)
         0.166666666666666666666666666667
 
     Computing the exponential function using its limit definition::
 
         >>> limit(lambda n: (1+3/n)**n, inf)
@@ -2105,11 +2098,11 @@
         g = lambda k: h(2**k)
 
     def update(values, indices):
         for k in indices:
             values.append(g(k+1))
 
     # XXX: steps used by nsum don't work well
-    if not 'steps' in kwargs:
+    if 'steps' not in kwargs:
         kwargs['steps'] = [10]
 
     return +ctx.adaptive_extrapolation(update, None, kwargs)
```

### Comparing `mpmath-1.3.0/mpmath/calculus/inverselaplace.py` & `mpmath-1.4.0a0/mpmath/calculus/inverselaplace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # contributed to mpmath by Kristopher L. Kuhlman, February 2017
 # contributed to mpmath by Guillermo Navas-Palencia, February 2022
 
-class InverseLaplaceTransform(object):
+class InverseLaplaceTransform:
     r"""
     Inverse Laplace transform methods are implemented using this
     class, in order to simplify the code and provide a common
     infrastructure.
 
     Implement a custom inverse Laplace transform algorithm by
     subclassing :class:`InverseLaplaceTransform` and implementing the
@@ -660,15 +660,15 @@
             self.ctx.dps = self.dps_orig
 
         return result
 
 
 # ****************************************
 
-class LaplaceTransformInversionMethods(object):
+class LaplaceTransformInversionMethods:
     def __init__(ctx, *args, **kwargs):
         ctx._fixed_talbot = FixedTalbot(ctx)
         ctx._stehfest = Stehfest(ctx)
         ctx._de_hoog = deHoog(ctx)
         ctx._cohen = Cohen(ctx)
 
     def invertlaplace(ctx, f, t, **kwargs):
@@ -695,16 +695,17 @@
 
             \bar{f}(p) = \frac{1}{(p+1)^2}
 
         .. math ::
 
             f(t) = t e^{-t}
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (besselj, euler, exp, invertlaplace, log,
+        ...                     mp, nstr, sinh, sqrt)
+        >>> mp.pretty = True
         >>> tt = [0.001, 0.01, 0.1, 1, 10]
         >>> fp = lambda p: 1/(p+1)**2
         >>> ft = lambda t: t*exp(-t)
         >>> ft(tt[0]),ft(tt[0])-invertlaplace(fp,tt[0],method='talbot')
         (0.000999000499833375, 8.57923043561212e-20)
         >>> ft(tt[1]),ft(tt[1])-invertlaplace(fp,tt[1],method='talbot')
         (0.00990049833749168, 3.27007646698047e-19)
@@ -770,16 +771,16 @@
 
         Mpmath implements four numerical inverse Laplace transform
         algorithms, attributed to: Talbot, Stehfest, and de Hoog,
         Knight and Stokes. These can be selected by using
         *method='talbot'*, *method='stehfest'*, *method='dehoog'* or
         *method='cohen'* or by passing the classes *method=FixedTalbot*,
         *method=Stehfest*, *method=deHoog*, or *method=Cohen*. The functions
-        :func:`~mpmath.invlaptalbot`, :func:`~mpmath.invlapstehfest`,
-        :func:`~mpmath.invlapdehoog`, and :func:`~mpmath.invlapcohen`
+        ``invlaptalbot()``, ``invlapstehfest()``,
+        ``invlapdehoog()``, and ``invlapcohen()``
         are also available as shortcuts.
 
         All four algorithms implement a heuristic balance between the
         requested precision and the precision used internally for the
         calculations. This has been tuned for a typical exponentially
         decaying function and precision up to few hundred decimal
         digits.
@@ -960,14 +961,7 @@
     def invlapdehoog(ctx, *args, **kwargs):
         kwargs['method'] = 'dehoog'
         return ctx.invertlaplace(*args, **kwargs)
 
     def invlapcohen(ctx, *args, **kwargs):
         kwargs['method'] = 'cohen'
         return ctx.invertlaplace(*args, **kwargs)
-
-
-# ****************************************
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/calculus/odes.py` & `mpmath-1.4.0a0/mpmath/calculus/odes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bisect import bisect
-from ..libmp.backend import xrange
 
-class ODEMethods(object):
+class ODEMethods:
     pass
 
 def ode_taylor(ctx, derivs, x0, y0, tol_prec, n):
     h = tol = ctx.ldexp(1, -tol_prec)
     dim = len(y0)
     xs = [x0]
     ys = [y0]
@@ -14,15 +13,15 @@
     orig = ctx.prec
     try:
         ctx.prec = orig*(1+n)
         # Use n steps with Euler's method to get
         # evaluation points for derivatives
         for i in range(n):
             fxy = derivs(x, y)
-            y = [y[i]+h*fxy[i] for i in xrange(len(y))]
+            y = [y[i]+h*fxy[i] for i in range(len(y))]
             x += h
             xs.append(x)
             ys.append(y)
         # Compute derivatives
         ser = [[] for d in range(dim)]
         for j in range(n+1):
             s = [0]*dim
@@ -118,16 +117,17 @@
     and continuing the evaluation up to `x_2 > x_1` is also fast.
 
     **Examples of first-order ODEs**
 
     We will solve the standard test problem `y'(x) = y(x), y(0) = 1`
     which has explicit solution `y(x) = \exp(x)`::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (atan, cos, exp, mp, mpf, nprint, odefun,
+        ...                     pi, sin, quad)
+        >>> mp.pretty = True
         >>> f = odefun(lambda x, y: y, 0, 1)
         >>> for x in [0, 1, 2.5]:
         ...     print((f(x), exp(x)))
         ...
         (1.0, 1.0)
         (2.71828182845905, 2.71828182845905)
         (12.1824939607035, 12.1824939607035)
@@ -188,33 +188,33 @@
         y_0' = y_1 \\
         y_1' = -y_0
         \end{cases}
 
     To get a well-defined IVP, we need two initial values. With
     `y(0) = y_0(0) = 1` and `-y'(0) = y_1(0) = 0`, the problem will of
     course be solved by `y(x) = y_0(x) = \cos(x)` and
-    `-y'(x) = y_1(x) = \sin(x)`. We check this::
+    `y'(x) = y_1(x) = -y_0(x) = -\sin(x)`. We check this::
 
-        >>> f = odefun(lambda x, y: [-y[1], y[0]], 0, [1, 0])
+        >>> f = odefun(lambda x, y: [y[1], -y[0]], 0, [1, 0])
         >>> for x in [0, 1, 2.5, 10]:
         ...     nprint(f(x), 15)
-        ...     nprint([cos(x), sin(x)], 15)
+        ...     nprint([cos(x), -sin(x)], 15)
         ...     print("---")
         ...
         [1.0, 0.0]
         [1.0, 0.0]
         ---
-        [0.54030230586814, 0.841470984807897]
-        [0.54030230586814, 0.841470984807897]
+        [0.54030230586814, -0.841470984807897]
+        [0.54030230586814, -0.841470984807897]
         ---
-        [-0.801143615546934, 0.598472144103957]
-        [-0.801143615546934, 0.598472144103957]
+        [-0.801143615546934, -0.598472144103957]
+        [-0.801143615546934, -0.598472144103957]
         ---
-        [-0.839071529076452, -0.54402111088937]
-        [-0.839071529076452, -0.54402111088937]
+        [-0.839071529076452, 0.54402111088937]
+        [-0.839071529076452, 0.54402111088937]
         ---
 
     Note that we get both the sine and the cosine solutions
     simultaneously.
 
     **TODO**
 
@@ -278,11 +278,7 @@
         if return_vector:
             return [+yk for yk in y]
         else:
             return +y[0]
     return interpolant
 
 ODEMethods.odefun = odefun
-
-if __name__ == "__main__":
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/calculus/optimization.py` & `mpmath-1.4.0a0/mpmath/calculus/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from __future__ import print_function
-
 from copy import copy
 
-from ..libmp.backend import xrange
 
-class OptimizationMethods(object):
+class OptimizationMethods:
     def __init__(ctx):
         pass
 
 ##############
 # 1D-SOLVERS #
 ##############
 
@@ -34,15 +31,15 @@
     def __init__(self, ctx, f, x0, **kwargs):
         self.ctx = ctx
         if len(x0) == 1:
             self.x0 = x0[0]
         else:
             raise ValueError('expected 1 starting point, got %i' % len(x0))
         self.f = f
-        if not 'df' in kwargs:
+        if 'df' not in kwargs:
             def df(x):
                 return self.ctx.diff(f, x)
         else:
             df = kwargs['df']
         self.df = df
 
     def __iter__(self):
@@ -122,21 +119,21 @@
 
     def __init__(self, ctx, f, x0, **kwargs):
         self.ctx = ctx
         if not len(x0) == 1:
             raise ValueError('expected 1 starting point, got %i' % len(x0))
         self.x0 = x0[0]
         self.f = f
-        if not 'df' in kwargs:
+        if 'df' not in kwargs:
             def df(x):
                 return self.ctx.diff(f, x)
         else:
             df = kwargs['df']
         self.df = df
-        if not 'd2f' in kwargs:
+        if 'd2f' not in kwargs:
             def d2f(x):
                 return self.ctx.diff(df, x)
         else:
             d2f = kwargs['df']
         self.d2f = d2f
 
     def __iter__(self):
@@ -179,21 +176,21 @@
 
     def __init__(self, ctx, f, x0, **kwargs):
         self.ctx = ctx
         if not len(x0) == 1:
             raise ValueError('expected 1 starting point, got %i' % len(x0))
         self.x0 = x0[0]
         self.f = f
-        if not 'df' in kwargs:
+        if 'df' not in kwargs:
             def df(x):
                 return self.ctx.diff(f, x)
         else:
             df = kwargs['df']
         self.df = df
-        if not 'd2f' in kwargs:
+        if 'd2f' not in kwargs:
             def d2f(x):
                 return self.ctx.diff(df, x)
         else:
             d2f = kwargs['df']
         self.d2f = d2f
 
     def __iter__(self):
@@ -525,15 +522,15 @@
 
     def __init__(self, ctx, f, x0, **kwargs):
         self.ctx = ctx
         if not len(x0) == 1:
             raise ValueError('expected 1 starting point, got %i' % len(x0))
         self.x0 = x0[0]
         self.f = f
-        if not 'df' in kwargs:
+        if 'df' not in kwargs:
             def df(x):
                 return self.ctx.diff(f, x)
         else:
             df = kwargs['df']
         self.df = df
         def phi(x):
             return x - f(x) / df(x)
@@ -586,19 +583,19 @@
     """
     x = ctx.matrix(x)
     h = ctx.sqrt(ctx.eps)
     fx = ctx.matrix(f(*x))
     m = len(fx)
     n = len(x)
     J = ctx.matrix(m, n)
-    for j in xrange(n):
+    for j in range(n):
         xj = x.copy()
         xj[j] += h
         Jj = (ctx.matrix(f(*xj)) - fx) / h
-        for i in xrange(m):
+        for i in range(m):
             J[i,j] = Jj[i]
     return J
 
 # TODO: test with user-specified jacobian matrix
 class MDNewton:
     """
     Find the root of a vector function numerically using Newton's method.
@@ -664,15 +661,15 @@
                 print('s:', s)
             # damping step size TODO: better strategy (hard task)
             l = self.ctx.one
             x1 = x0 + s
             while True:
                 if x1 == x0:
                     if self.verbose:
-                        print("canceled, won't get more excact")
+                        print("canceled, won't get more exact")
                     cancel = True
                     break
                 fx = self.ctx.matrix(f(*x1))
                 newnorm = norm(fx)
                 if newnorm < fxnorm:
                     # new x accepted
                     fxnorm = newnorm
@@ -712,23 +709,24 @@
     **Arguments**
 
     *f*
         one dimensional function
     *x0*
         starting point, several starting points or interval (depends on solver)
     *tol*
-        the returned solution has an error smaller than this
+        the returned solution has an error smaller than this, with
+        the defailt value ``2**10`` times epsilon of working precision
     *verbose*
         print additional information for each iteration if true
     *verify*
         verify the solution and raise a ValueError if `|f(x)|^2 > \mathrm{tol}`
     *solver*
         a generator for *f* and *x0* returning approximative solution and error
     *maxsteps*
-        after how many steps the solver will cancel
+        the solver will cancel at least after that number of iterations
     *df*
         first derivative of *f* (used by some solvers)
     *d2f*
         second derivative of *f* (used by some solvers)
     *multidimensional*
         force multidimensional solving
     *J*
@@ -747,15 +745,16 @@
 
     **Examples**
 
     The function :func:`~mpmath.findroot` locates a root of a given function using the
     secant method by default. A simple example use of the secant method is to
     compute `\pi` as the root of `\sin x` closest to `x_0 = 3`::
 
-        >>> from mpmath import *
+        >>> from mpmath import (diff, gamma, findroot, sin, zeta, exp, log,
+        ...                     lambertw, mp, j)
         >>> mp.dps = 30; mp.pretty = True
         >>> findroot(sin, 3)
         3.14159265358979323846264338328
 
     The secant method can be used to find complex roots of analytic functions,
     although it must in that case generally be given a nonreal starting value
     (or else it will never leave the real line)::
@@ -882,15 +881,15 @@
     with multiple roots and usually need a sign change to find a root::
 
         >>> findroot(lambda x: x**3, (-1, 1), solver='anderson')
         0.0
 
     Be careful with symmetric functions::
 
-        >>> findroot(lambda x: x**2, (-1, 1), solver='anderson') #doctest:+ELLIPSIS
+        >>> findroot(lambda x: x**2, (-1, 1), solver='anderson')
         Traceback (most recent call last):
           ...
         ZeroDivisionError
 
     It fails even for better starting points, because there is no sign change::
 
         >>> findroot(lambda x: x**2, (-1, .5), solver='anderson')
@@ -940,15 +939,15 @@
             fx = f(x0[0])
             multidimensional = False
         if 'multidimensional' in kwargs:
             multidimensional = kwargs['multidimensional']
         if multidimensional:
             # only one multidimensional solver available at the moment
             solver = MDNewton
-            if not 'norm' in kwargs:
+            if 'norm' not in kwargs:
                 norm = lambda x: ctx.norm(x, 'inf')
                 kwargs['norm'] = norm
             else:
                 norm = kwargs['norm']
         else:
             norm = abs
 
@@ -957,18 +956,15 @@
             if multidimensional:
                 return ctx.matrix(x0)
             else:
                 return x0[0]
 
         # use solver
         iterations = solver(ctx, f, x0, **kwargs)
-        if 'maxsteps' in kwargs:
-            maxsteps = kwargs['maxsteps']
-        else:
-            maxsteps = iterations.maxsteps
+        maxsteps = kwargs.get('maxsteps', iterations.maxsteps)
         i = 0
         for x, error in iterations:
             if verbose:
                 print('x:    ', x)
                 print('error:', error)
             i += 1
             if error < tol * max(1, norm(x)) or i >= maxsteps:
@@ -996,23 +992,23 @@
     Return the multiplicity of a given root of f.
 
     Internally, numerical derivatives are used. This might be inefficient for
     higher order derviatives. Due to this, ``multiplicity`` cancels after
     evaluating 10 derivatives by default. You can be specify the n-th derivative
     using the dnf keyword.
 
-    >>> from mpmath import *
+    >>> from mpmath import multiplicity, pi, sin
     >>> multiplicity(lambda x: sin(x) - 1, pi/2)
     2
 
     """
     if tol is None:
         tol = ctx.eps ** 0.8
     kwargs['d0f'] = f
-    for i in xrange(maxsteps):
+    for i in range(maxsteps):
         dfstr = 'd' + str(i) + 'f'
         if dfstr in kwargs:
             df = kwargs[dfstr]
         else:
             df = lambda x: ctx.diff(f, x, i)
         if not abs(df(root)) < tol:
             break
@@ -1042,15 +1038,15 @@
     Let's try Steffensen's method:
 
     >>> f = lambda x: x**2
     >>> from mpmath.calculus.optimization import steffensen
     >>> F = steffensen(f)
     >>> for x in [0.5, 0.9, 2.0]:
     ...     fx = Fx = x
-    ...     for i in xrange(9):
+    ...     for i in range(9):
     ...         try:
     ...             fx = f(fx)
     ...         except OverflowError:
     ...             pass
     ...         try:
     ...             Fx = F(Fx)
     ...         except ZeroDivisionError:
@@ -1092,11 +1088,7 @@
         ffx = f(fx)
         return (x*ffx - fx**2) / (ffx - 2*fx + x)
     return F
 
 OptimizationMethods.jacobian = jacobian
 OptimizationMethods.findroot = findroot
 OptimizationMethods.multiplicity = multiplicity
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/calculus/polynomials.py` & `mpmath-1.4.0a0/mpmath/calculus/polynomials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ..libmp.backend import xrange
 from .calculus import defun
 
 #----------------------------------------------------------------------------#
 #                                Polynomials                                 #
 #----------------------------------------------------------------------------#
 
 # XXX: extra precision
@@ -16,15 +15,15 @@
 
         P(x) = c_n x^n + \ldots + c_2 x^2 + c_1 x + c_0.
 
     If *derivative=True* is set, :func:`~mpmath.polyval` simultaneously
     evaluates `P(x)` with the derivative, `P'(x)`, and returns the
     tuple `(P(x), P'(x))`.
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, polyval
         >>> mp.pretty = True
         >>> polyval([3, 0, 2], 0.5)
         2.75
         >>> polyval([3, 0, 2], 0.5, derivative=True)
         (2.75, 3.0)
 
     The coefficients and the evaluation point may be any combination
@@ -57,16 +56,16 @@
     With *error=True*, :func:`~mpmath.polyroots` returns a tuple *(roots, err)*
     where *err* is an estimate of the maximum error among the computed roots.
 
     **Examples**
 
     Finding the three real roots of `x^3 - x^2 - 14x + 24`::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, polyroots, nprint, sqrt, polyval
+        >>> mp.pretty = True
         >>> nprint(polyroots([1,-1,-14,24]), 4)
         [-4.0, 2.0, 3.0]
 
     Finding the two complex conjugate roots of `4x^2 + 3x + 2`, with an
     error estimate::
 
         >>> roots, err = polyroots([4,3,2], error=True)
@@ -165,27 +164,27 @@
         lead = ctx.convert(coeffs[0])
         if lead == 1:
             coeffs = [ctx.convert(c) for c in coeffs]
         else:
             coeffs = [c/lead for c in coeffs]
         f = lambda x: ctx.polyval(coeffs, x)
         if roots_init is None:
-            roots = [ctx.mpc((0.4+0.9j)**n) for n in xrange(deg)]
+            roots = [ctx.mpc((0.4+0.9j)**n) for n in range(deg)]
         else:
-            roots = [None]*deg;
+            roots = [None]*deg
             deg_init = min(deg, len(roots_init))
             roots[:deg_init] = list(roots_init[:deg_init])
             roots[deg_init:] = [ctx.mpc((0.4+0.9j)**n) for n
-                                in xrange(deg_init,deg)]
-        err = [ctx.one for n in xrange(deg)]
+                                in range(deg_init,deg)]
+        err = [ctx.one for n in range(deg)]
         # Durand-Kerner iteration until convergence
-        for step in xrange(maxsteps):
+        for step in range(maxsteps):
             if abs(max(err)) < tol:
                 break
-            for i in xrange(deg):
+            for i in range(deg):
                 p = roots[i]
                 x = f(p)
                 for j in range(deg):
                     if i != j:
                         try:
                             x /= (p-roots[j])
                         except ZeroDivisionError:
@@ -193,15 +192,15 @@
                 roots[i] = p - x
                 err[i] = abs(x)
         if abs(max(err)) >= tol:
             raise ctx.NoConvergence("Didn't converge in maxsteps=%d steps." \
                     % maxsteps)
         # Remove small real or imaginary parts
         if cleanup:
-            for i in xrange(deg):
+            for i in range(deg):
                 if abs(roots[i]) < tol:
                     roots[i] = ctx.zero
                 elif abs(ctx._im(roots[i])) < tol:
                     roots[i] = roots[i].real
                 elif abs(ctx._re(roots[i])) < tol:
                     roots[i] = roots[i].imag * 1j
         roots.sort(key=lambda x: (abs(ctx._im(x)), ctx._re(x)))
```

### Comparing `mpmath-1.3.0/mpmath/calculus/quadrature.py` & `mpmath-1.4.0a0/mpmath/calculus/quadrature.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import math
 
-from ..libmp.backend import xrange
 
-class QuadratureRule(object):
+class QuadratureRule:
     """
     Quadrature rules are implemented using this class, in order to
     simplify the code and provide a common infrastructure
     for tasks such as error estimation and node caching.
 
     You can implement a custom quadrature rule by subclassing
     :class:`QuadratureRule` and implementing the appropriate
     methods. The subclass can then be used by :func:`~mpmath.quad` by
     passing it as the *method* argument.
 
     :class:`QuadratureRule` instances are supposed to be singletons.
-    :class:`QuadratureRule` therefore implements instance caching
-    in :func:`~mpmath.__new__`.
     """
 
     def __init__(self, ctx):
         self.ctx = ctx
         self.standard_cache = {}
         self.transformed_cache = {}
         self.interval_count = {}
@@ -32,28 +29,30 @@
         self.transformed_cache = {}
         self.interval_count = {}
 
     def calc_nodes(self, degree, prec, verbose=False):
         r"""
         Compute nodes for the standard interval `[-1, 1]`. Subclasses
         should probably implement only this method, and use
-        :func:`~mpmath.get_nodes` method to retrieve the nodes.
+        :func:`~mpmath.calculus.quadrature.QuadratureRule.get_nodes`
+        method to retrieve the nodes.
         """
         raise NotImplementedError
 
     def get_nodes(self, a, b, degree, prec, verbose=False):
         """
         Return nodes for given interval, degree and precision. The
         nodes are retrieved from a cache if already computed;
-        otherwise they are computed by calling :func:`~mpmath.calc_nodes`
+        otherwise they are computed by calling
+        :func:`~mpmath.calculus.quadrature.QuadratureRule.calc_nodes`
         and are then cached.
 
-        Subclasses should probably not implement this method,
-        but just implement :func:`~mpmath.calc_nodes` for the actual
-        node computation.
+        Subclasses should probably not implement this method, but just
+        implement :func:`~mpmath.calculus.quadrature.QuadratureRule.calc_nodes`
+        for the actual node computation.
         """
         key = (a, b, degree, prec)
         if key in self.transformed_cache:
             return self.transformed_cache[key]
         orig = self.ctx.prec
         try:
             self.ctx.prec = prec+20
@@ -141,15 +140,15 @@
         to `m` iterations. The value of `m` should be a slight
         overestimate, so that "slightly bad" integrals can be dealt
         with automatically using a few extra iterations. On the
         other hand, it should not be too big, so :func:`~mpmath.quad` can
         quit within a reasonable amount of time when it is given
         an "unsolvable" integral.
 
-        The default formula used by :func:`~mpmath.guess_degree` is tuned
+        The default formula used by :func:`~mpmath.calculus.quadrature.QuadratureRule.guess_degree` is tuned
         for both :class:`TanhSinh` and :class:`GaussLegendre`.
         The output is roughly as follows:
 
             +---------+---------+
             | `p`     | `m`     |
             +=========+=========+
             | 50      | 6       |
@@ -201,35 +200,35 @@
         return self.ctx.mpf(10) ** int(D4)
 
     def summation(self, f, points, prec, epsilon, max_degree, verbose=False):
         """
         Main integration function. Computes the 1D integral over
         the interval specified by *points*. For each subinterval,
         performs quadrature of degree from 1 up to *max_degree*
-        until :func:`~mpmath.estimate_error` signals convergence.
+        until :func:`~mpmath.calculus.quadrature.QuadratureRule.estimate_error` signals convergence.
 
-        :func:`~mpmath.summation` transforms each subintegration to
-        the standard interval and then calls :func:`~mpmath.sum_next`.
+        :func:`~mpmath.calculus.quadrature.QuadratureRule.summation` transforms each subintegration to
+        the standard interval and then calls :func:`~mpmath.calculus.quadrature.QuadratureRule.sum_next`.
         """
         ctx = self.ctx
         I = total_err = ctx.zero
-        for i in xrange(len(points)-1):
+        for i in range(len(points)-1):
             a, b = points[i], points[i+1]
             if a == b:
                 continue
             # XXX: we could use a single variable transformation,
             # but this is not good in practice. We get better accuracy
             # by having 0 as an endpoint.
             if (a, b) == (ctx.ninf, ctx.inf):
                 _f = f
                 f = lambda x: _f(-x) + _f(x)
                 a, b = (ctx.zero, ctx.inf)
             results = []
             err = ctx.zero
-            for degree in xrange(1, max_degree+1):
+            for degree in range(1, max_degree+1):
                 nodes = self.get_nodes(a, b, degree, prec, verbose)
                 if verbose:
                     print("Integrating from %s to %s (degree %s of %s)" % \
                         (ctx.nstr(a), ctx.nstr(b), degree, max_degree))
                 result = self.sum_next(f, nodes, degree, prec, results, verbose)
                 results.append(result)
                 if degree > 1:
@@ -246,16 +245,16 @@
         return I, total_err
 
     def sum_next(self, f, nodes, degree, prec, previous, verbose=False):
         r"""
         Evaluates the step sum `\sum w_k f(x_k)` where the *nodes* list
         contains the `(w_k, x_k)` pairs.
 
-        :func:`~mpmath.summation` will supply the list *results* of
-        values computed by :func:`~mpmath.sum_next` at previous degrees, in
+        :func:`~mpmath.calculus.quadrature.QuadratureRule.summation` will supply the list *results* of
+        values computed by :func:`~mpmath.calculus.quadrature.QuadratureRule.sum_next` at previous degrees, in
         case the quadrature rule is able to reuse them.
         """
         return self.ctx.fdot((w, f(x)) for (x,w) in nodes)
 
 
 class TanhSinh(QuadratureRule):
     r"""
@@ -349,15 +348,15 @@
         # by simply multiplying by exp(h)
         expt0 = ctx.exp(t0)
         a = pi4 * expt0
         b = pi4 / expt0
         udelta = ctx.exp(h)
         urdelta = 1/udelta
 
-        for k in xrange(0, 20*2**degree+1):
+        for k in range(0, 20*2**degree+1):
             # Reference implementation:
             # t = t0 + k*h
             # x = tanh(pi/2 * sinh(t))
             # w = pi/2 * cosh(t) / cosh(pi/2 * sinh(t))**2
 
             # Fast implementation. Note that c = exp(pi/2 * sinh(t))
             c = ctx.exp(a-b)
@@ -428,23 +427,23 @@
             w = ctx.mpf(5)/9
             nodes = [(-x,w),(ctx.zero,ctx.mpf(8)/9),(x,w)]
             ctx.prec = orig
             return nodes
         nodes = []
         n = 3*2**(degree-1)
         upto = n//2 + 1
-        for j in xrange(1, upto):
+        for j in range(1, upto):
             # Asymptotic formula for the roots
             r = ctx.mpf(math.cos(math.pi*(j-0.25)/(n+0.5)))
             # Newton iteration
             while 1:
                 t1, t2 = 1, 0
                 # Evaluates the Legendre polynomial using its defining
                 # recurrence relation
-                for j1 in xrange(1,n+1):
+                for j1 in range(1,n+1):
                     t3, t2, t1 = t2, t1, ((2*j1-1)*r*t1 - (j1-1)*t2)/j1
                 t4 = n*(r*t1-t2)/(r**2-1)
                 a = t1/t4
                 r = r - a
                 if abs(a) < epsilon:
                     break
             x = r
@@ -452,27 +451,28 @@
             if verbose  and j % 30 == 15:
                 print("Computing nodes (%i of %i)" % (j, upto))
             nodes.append((x, w))
             nodes.append((-x, w))
         ctx.prec = orig
         return nodes
 
-class QuadratureMethods(object):
+class QuadratureMethods:
 
     def __init__(ctx, *args, **kwargs):
         ctx._gauss_legendre = GaussLegendre(ctx)
         ctx._tanh_sinh = TanhSinh(ctx)
 
     def quad(ctx, f, *points, **kwargs):
         r"""
         Computes a single, double or triple integral over a given
         1D interval, 2D rectangle, or 3D cuboid. A basic example::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import (mp, quad, cos, pi, exp, inf, sqrt,
+            ...                     chop, sin, j, log, euler, e, linspace)
+            >>> mp.pretty = True
             >>> quad(sin, [0, pi])
             2.0
 
         A basic 2D integral::
 
             >>> f = lambda x, y: cos(x+y/2)
             >>> quad(f, [-pi/2, pi/2], [0, pi])
@@ -518,15 +518,15 @@
 
         **Algorithms**
 
         Mpmath presently implements two integration algorithms: tanh-sinh
         quadrature and Gauss-Legendre quadrature. These can be selected
         using *method='tanh-sinh'* or *method='gauss-legendre'* or by
         passing the classes *method=TanhSinh*, *method=GaussLegendre*.
-        The functions :func:`~mpmath.quadts` and :func:`~mpmath.quadgl` are also available
+        The functions ``quadts()`` and ``quadgl()`` are also available
         as shortcuts.
 
         Both algorithms have the property that doubling the number of
         evaluation points roughly doubles the accuracy, so both are ideal
         for high precision quadrature (hundreds or thousands of digits).
 
         At high precision, computing the nodes and weights for the
@@ -542,25 +542,24 @@
         Gauss-Legendre quadrature often requires fewer function
         evaluations, and is therefore often faster for repeated use, but
         the algorithm does not handle endpoint singularities as well and
         the nodes are more expensive to compute. Gauss-Legendre quadrature
         can be a better choice if the integrand is smooth and repeated
         integrations are required (e.g. for multiple integrals).
 
-        See the documentation for :class:`TanhSinh` and
-        :class:`GaussLegendre` for additional details.
+        See the documentation for :class:`~mpmath.calculus.quadrature.TanhSinh` and
+        :class:`~mpmath.calculus.quadrature.GaussLegendre` for additional details.
 
         **Examples of 1D integrals**
 
         Intervals may be infinite or half-infinite. The following two
         examples evaluate the limits of the inverse tangent function
         (`\int 1/(1+x^2) = \tan^{-1} x`), and the Gaussian integral
         `\int_{\infty}^{\infty} \exp(-x^2)\,dx = \sqrt{\pi}`::
 
-            >>> mp.dps = 15
             >>> quad(lambda x: 2/(x**2+1), [0, inf])
             3.14159265358979
             >>> quad(lambda x: exp(-x**2), [-inf, inf])**2
             3.14159265358979
 
         Integrals can typically be resolved to high precision.
         The following computes 50 digits of `\pi` by integrating the
@@ -570,15 +569,15 @@
             >>> mp.dps = 50
             >>> 2*quad(lambda x: sqrt(1-x**2), [-1, 1])
             3.1415926535897932384626433832795028841971693993751
 
         One can just as well compute 1000 digits (output truncated)::
 
             >>> mp.dps = 1000
-            >>> 2*quad(lambda x: sqrt(1-x**2), [-1, 1])  #doctest:+ELLIPSIS
+            >>> 2*quad(lambda x: sqrt(1-x**2), [-1, 1])
             3.141592653589793238462643383279502884...216420199
 
         Complex integrals are supported. The following computes
         a residue at `z = 0` by integrating counterclockwise along the
         diamond-shaped path from `1` to `+i` to `-1` to `-i` to `1`::
 
             >>> mp.dps = 15
@@ -839,16 +838,18 @@
         Accordingly, :func:`~mpmath.quadosc` requires information about the
         zeros of `f(x)`. For a periodic function, you can specify
         the zeros by either providing the angular frequency `\omega`
         (*omega*) or the *period* `2 \pi/\omega`. In general, you can
         specify the `n`-th zero by providing the *zeros* arguments.
         Below is an example of each::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import (mp, sin, quadosc, pi, ei, cos, inf, j0,
+            ...                     j1, sqrt, findroot, exp, e, si, ci, j,
+            ...                     quad, log)
+            >>> mp.pretty = True
             >>> f = lambda x: sin(3*x)/(x**2+1)
             >>> quadosc(f, [0,inf], omega=3)
             0.37833007080198
             >>> quadosc(f, [0,inf], period=2*pi/3)
             0.37833007080198
             >>> quadosc(f, [0,inf], zeros=lambda n: pi*n/3)
             0.37833007080198
@@ -981,15 +982,15 @@
                 "must specify exactly one of omega, period, zeros")
         if a == ctx.ninf and b == ctx.inf:
             s1 = ctx.quadosc(f, [a, 0], omega=omega, zeros=zeros, period=period)
             s2 = ctx.quadosc(f, [0, b], omega=omega, zeros=zeros, period=period)
             return s1 + s2
         if a == ctx.ninf:
             if zeros:
-                return ctx.quadosc(lambda x:f(-x), [-b,-a], lambda n: zeros(-n))
+                return ctx.quadosc(lambda x:f(-x), [-b,-a], zeros=lambda n: zeros(-n))
             else:
                 return ctx.quadosc(lambda x:f(-x), [-b,-a], omega=omega, period=period)
         if b != ctx.inf:
             raise ValueError("quadosc requires an infinite integration interval")
         if not zeros:
             if omega:
                 period = 2*ctx.pi/omega
@@ -1012,16 +1013,17 @@
         Computes the integral of *f* over the interval or path specified
         by *interval*, using :func:`~mpmath.quad` together with adaptive
         subdivision of the interval.
 
         This function gives an accurate answer for some integrals where
         :func:`~mpmath.quad` fails::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import (mp, sin, pi, quad, quadsubdiv, ceil, exp,
+            ...                     sech, linspace, fp, ci)
+            >>> mp.pretty = True
             >>> quad(lambda x: abs(sin(x)), [0, 2*pi])
             3.99900894176779
             >>> quadsubdiv(lambda x: abs(sin(x)), [0, 2*pi])
             4.0
             >>> quadsubdiv(sin, [0, 1000])
             0.437620923709297
             >>> quadsubdiv(lambda x: 1/(1+x**2), [-100, 100])
@@ -1105,11 +1107,7 @@
                     queue.append((m, b))
         finally:
             ctx.prec = orig
         if kwargs.get("error"):
             return +total, +total_error
         else:
             return +total
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/ctx_base.py` & `mpmath-1.4.0a0/mpmath/ctx_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from operator import gt, lt
+import random
 
-from .libmp.backend import xrange
-
-from .functions.functions import SpecialFunctions
-from .functions.rszeta import RSCache
-from .calculus.quadrature import QuadratureMethods
-from .calculus.inverselaplace import LaplaceTransformInversionMethods
+from . import libmp
 from .calculus.calculus import CalculusMethods
-from .calculus.optimization import OptimizationMethods
+from .calculus.inverselaplace import LaplaceTransformInversionMethods
 from .calculus.odes import ODEMethods
-from .matrices.matrices import MatrixMethods
+from .calculus.optimization import OptimizationMethods
+from .calculus.quadrature import QuadratureMethods
+from .functions.functions import SpecialFunctions
+from .functions.rszeta import RSCache
+from .identification import IdentificationMethods
 from .matrices.calculus import MatrixCalculusMethods
-from .matrices.linalg import LinearAlgebraMethods
 from .matrices.eigen import Eigen
-from .identification import IdentificationMethods
+from .matrices.linalg import LinearAlgebraMethods
+from .matrices.matrices import MatrixMethods
 from .visualization import VisualizationMethods
 
-from . import libmp
 
-class Context(object):
+class Context:
     pass
 
 class StandardBaseContext(Context,
     SpecialFunctions,
     RSCache,
     QuadratureMethods,
     LaplaceTransformInversionMethods,
@@ -127,16 +126,15 @@
 
     def chop(ctx, x, tol=None):
         """
         Chops off small real or imaginary parts, or converts
         numbers close to zero to exact zeros. The input can be a
         single number or an iterable::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import chop, nprint
             >>> chop(5+1e-10j, tol=1e-9)
             mpf('5.0')
             >>> nprint(chop([1.0, 1e-20, 3+1e-18j, -4, 2]))
             [1.0, 0.0, 3.0, -4.0, 2.0]
 
         The tolerance defaults to ``100*eps``.
         """
@@ -176,16 +174,15 @@
         `p` is the current working precision and `m` is a small
         integer. The default setting typically allows :func:`~mpmath.almosteq`
         to be used to check for mathematical equality
         in the presence of small rounding errors.
 
         **Examples**
 
-            >>> from mpmath import *
-            >>> mp.dps = 15
+            >>> from mpmath import almosteq
             >>> almosteq(3.141592653589793, 3.141592653589790)
             True
             >>> almosteq(3.141592653589793, 3.141592653589700)
             False
             >>> almosteq(3.141592653589793, 3.141592653589700, 1e-10)
             True
             >>> almosteq(1e-20, 2e-20)
@@ -210,36 +207,35 @@
             err = diff/abst
         else:
             err = diff/abss
         return err <= rel_eps
 
     def arange(ctx, *args):
         r"""
-        This is a generalized version of Python's :func:`~mpmath.range` function
+        This is a generalized version of Python's :class:`range` function
         that accepts fractional endpoints and step sizes and
-        returns a list of ``mpf`` instances. Like :func:`~mpmath.range`,
+        returns a list of ``mpf`` instances. Like :class:`range`,
         :func:`~mpmath.arange` can be called with 1, 2 or 3 arguments:
 
         ``arange(b)``
             `[0, 1, 2, \ldots, x]`
         ``arange(a, b)``
             `[a, a+1, a+2, \ldots, x]`
         ``arange(a, b, h)``
             `[a, a+h, a+h, \ldots, x]`
 
         where `b-1 \le x < b` (in the third case, `b-h \le x < b`).
 
-        Like Python's :func:`~mpmath.range`, the endpoint is not included. To
+        Like Python's :class:`range`, the endpoint is not included. To
         produce ranges where the endpoint is included, :func:`~mpmath.linspace`
         is more convenient.
 
         **Examples**
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import arange
             >>> arange(4)
             [mpf('0.0'), mpf('1.0'), mpf('2.0'), mpf('3.0')]
             >>> arange(1, 2, 0.25)
             [mpf('1.0'), mpf('1.25'), mpf('1.5'), mpf('1.75')]
             >>> arange(1, -1, -0.75)
             [mpf('1.0'), mpf('0.25'), mpf('-0.5')]
 
@@ -291,16 +287,15 @@
         samples from `a` to `b`. The syntax ``linspace(mpi(a,b), n)``
         is also valid.
 
         This function is often more convenient than :func:`~mpmath.arange`
         for partitioning an interval into subintervals, since
         the endpoint is included::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import linspace
             >>> linspace(1, 4, 4)
             [mpf('1.0'), mpf('2.0'), mpf('3.0'), mpf('4.0')]
 
         You may also provide the keyword argument ``endpoint=False``::
 
             >>> linspace(1, 4, 4, endpoint=False)
             [mpf('1.0'), mpf('1.75'), mpf('2.5'), mpf('3.25')]
@@ -316,23 +311,23 @@
             b = args[0].b
             n = int(args[1])
         else:
             raise TypeError('linspace expected 2 or 3 arguments, got %i' \
                             % len(args))
         if n < 1:
             raise ValueError('n must be greater than 0')
-        if not 'endpoint' in kwargs or kwargs['endpoint']:
+        if 'endpoint' not in kwargs or kwargs['endpoint']:
             if n == 1:
                 return [ctx.mpf(a)]
             step = (b - a) / ctx.mpf(n - 1)
-            y = [i*step + a for i in xrange(n)]
+            y = [i*step + a for i in range(n)]
             y[-1] = b
         else:
             step = (b - a) / ctx.mpf(n)
-            y = [i*step + a for i in xrange(n)]
+            y = [i*step + a for i in range(n)]
         return y
 
     def cos_sin(ctx, z, **kwargs):
         return ctx.cos(z, **kwargs), ctx.sin(z, **kwargs)
 
     def cospi_sinpi(ctx, z, **kwargs):
         return ctx.cospi(z, **kwargs), ctx.sinpi(z, **kwargs)
@@ -353,14 +348,15 @@
     def sum_accurately(ctx, terms, check_step=1):
         prec = ctx.prec
         try:
             extraprec = 10
             while 1:
                 ctx.prec = prec + extraprec + 5
                 max_mag = ctx.ninf
+                sum_mag = ctx.zero
                 s = ctx.zero
                 k = 0
                 for term in terms():
                     s += term
                     if (not k % check_step) and term:
                         term_mag = ctx.mag(term)
                         max_mag = max(max_mag, term_mag)
@@ -408,72 +404,95 @@
                 extraprec += min(ctx.prec, cancellation)
             return s
         finally:
             ctx.prec = prec
 
     def power(ctx, x, y):
         r"""Converts `x` and `y` to mpmath numbers and evaluates
-        `x^y = \exp(y \log(x))`::
+        the principal value of `\exp(y \log(x))`::
 
-            >>> from mpmath import *
+            >>> from mpmath import mp, power
             >>> mp.dps = 30; mp.pretty = True
             >>> power(2, 0.5)
             1.41421356237309504880168872421
 
         This shows the leading few digits of a large Mersenne prime
         (performing the exact calculation ``2**43112609-1`` and
         displaying the result in Python would be very slow)::
 
             >>> power(2, 43112609)-1
             3.16470269330255923143453723949e+12978188
+
+        **See Also**
+
+        :func:`~mpmath.root`
         """
         return ctx.convert(x) ** ctx.convert(y)
 
     def _zeta_int(ctx, n):
         return ctx.zeta(n)
 
     def maxcalls(ctx, f, N):
         """
         Return a wrapped copy of *f* that raises ``NoConvergence`` when *f*
         has been called more than *N* times::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15
+            >>> from mpmath import maxcalls, sin
             >>> f = maxcalls(sin, 10)
             >>> print(sum(f(n) for n in range(10)))
             1.95520948210738
-            >>> f(10) # doctest: +IGNORE_EXCEPTION_DETAIL
+            >>> f(10)
             Traceback (most recent call last):
               ...
             NoConvergence: maxcalls: function evaluated 10 times
 
         """
         counter = [0]
         def f_maxcalls_wrapped(*args, **kwargs):
             counter[0] += 1
             if counter[0] > N:
                 raise ctx.NoConvergence("maxcalls: function evaluated %i times" % N)
             return f(*args, **kwargs)
         return f_maxcalls_wrapped
 
+    def rand(ctx):
+        """
+        Get a random number in the range ``[0.0, 1.0)`` with (almost) uniform distribution.
+
+        This method is a replacement for ``random.random()``. It is roughly equal
+        to ``random.randint(0, 2 ** prec - 1) / (2 ** prec)``, where ``prec``
+        is the current resolution in bits.
+
+        Just like ``random.random()`` and most other floating-point random number
+        generators, the distribution is not perfect:
+
+        Some float values within ``[0,1)`` will never be returned, for example,
+        ``2 ** -(prec + 1)`` is impossible. See
+        http://mumble.net/~campbell/2014/04/28/uniform-random-float
+        for a lengthy discussion.
+        """
+        # slow default implementation of rand() that works for arbitrary precision.
+        return ctx.convert(random.getrandbits(ctx.prec)) * (ctx.convert(2) ** (-ctx.prec))
+
+
     def memoize(ctx, f):
         """
         Return a wrapped copy of *f* that caches computed values, i.e.
         a memoized copy of *f*. Values are only reused if the cached precision
         is equal to or higher than the working precision::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import memoize, maxcalls, mp, sin
+            >>> mp.pretty = True
             >>> f = memoize(maxcalls(sin, 1))
             >>> f(2)
             0.909297426825682
             >>> f(2)
             0.909297426825682
             >>> mp.dps = 25
-            >>> f(2) # doctest: +IGNORE_EXCEPTION_DETAIL
+            >>> f(2)
             Traceback (most recent call last):
               ...
             NoConvergence: maxcalls: function evaluated 1 times
 
         """
         f_cache = {}
         def f_cached(*args, **kwargs):
```

### Comparing `mpmath-1.3.0/mpmath/ctx_fp.py` & `mpmath-1.4.0a0/mpmath/ctx_fp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-from .ctx_base import StandardBaseContext
-
-import math
 import cmath
-from . import math2
+import functools
+import math
+import sys
 
-from . import function_docs
+from . import function_docs, libfp, libmp
+from .ctx_base import StandardBaseContext
+from .libmp import int_types, mpf_bernoulli, to_float
 
-from .libmp import mpf_bernoulli, to_float, int_types
-from . import libmp
 
 class FPContext(StandardBaseContext):
     """
     Context for fast low-precision arithmetic (53-bit precision, giving at most
     about 15-digit accuracy), using Python's builtin float and complex.
     """
 
     def __init__(ctx):
         StandardBaseContext.__init__(ctx)
 
         # Override SpecialFunctions implementation
-        ctx.loggamma = math2.loggamma
-        ctx._bernoulli_cache = {}
+        ctx.loggamma = libfp.loggamma
         ctx.pretty = False
 
         ctx._init_aliases()
 
-    _mpq = lambda cls, x: float(x[0])/x[1]
-
     NoConvergence = libmp.NoConvergence
 
     def _get_prec(ctx): return 53
     def _set_prec(ctx, p): return
     def _get_dps(ctx): return 15
     def _set_dps(ctx, p): return
 
     _fixed_precision = True
 
     prec = property(_get_prec, _set_prec)
     dps = property(_get_dps, _set_dps)
 
     zero = 0.0
     one = 1.0
-    eps = math2.EPS
-    inf = math2.INF
-    ninf = math2.NINF
-    nan = math2.NAN
+    eps = sys.float_info.epsilon
+    inf = libfp.INF
+    ninf = -math.inf
+    nan = math.nan
     j = 1j
 
     # Called by SpecialFunctions.__init__()
     @classmethod
     def _wrap_specfun(cls, name, f, wrap):
         if wrap:
             def f_wrapped(ctx, *args, **kwargs):
@@ -56,140 +52,137 @@
                 args = [convert(a) for a in args]
                 return f(ctx, *args, **kwargs)
         else:
             f_wrapped = f
         f_wrapped.__doc__ = function_docs.__dict__.get(name, f.__doc__)
         setattr(cls, name, f_wrapped)
 
-    def bernoulli(ctx, n):
-        cache = ctx._bernoulli_cache
-        if n in cache:
-            return cache[n]
-        cache[n] = to_float(mpf_bernoulli(n, 53, 'n'), strict=True)
-        return cache[n]
-
-    pi = math2.pi
-    e = math2.e
-    euler = math2.euler
+    @functools.lru_cache
+    def bernoulli(ctx, n, plus=False):
+        return to_float(mpf_bernoulli(n, 53, 'n', plus=plus), strict=True)
+
+    pi = libfp.pi
+    e = math.e
+    euler = libfp.euler
     sqrt2 = 1.4142135623730950488
     sqrt5 = 2.2360679774997896964
     phi = 1.6180339887498948482
     ln2 = 0.69314718055994530942
     ln10 = 2.302585092994045684
-    euler = 0.57721566490153286061
+    euler = libfp.euler
     catalan = 0.91596559417721901505
     khinchin = 2.6854520010653064453
     apery = 1.2020569031595942854
     glaisher = 1.2824271291006226369
 
     absmin = absmax = abs
 
     def is_special(ctx, x):
         return x - x != 0.0
 
     def isnan(ctx, x):
         return x != x
 
     def isinf(ctx, x):
-        return abs(x) == math2.INF
+        return abs(x) == libfp.INF
+
+    def isfinite(ctx, x):
+        if type(x) is complex:
+            return all(map(math.isfinite, [x.real, x.imag]))
+        return math.isfinite(x)
 
     def isnormal(ctx, x):
         if x:
             return x - x == 0.0
         return False
 
     def isnpint(ctx, x):
         if type(x) is complex:
             if x.imag:
                 return False
             x = x.real
-        return x <= 0.0 and round(x) == x
+        return math.isfinite(x) and x <= 0.0 and round(x) == x
 
     mpf = float
     mpc = complex
 
     def convert(ctx, x):
         try:
             return float(x)
         except:
             return complex(x)
 
-    power = staticmethod(math2.pow)
-    sqrt = staticmethod(math2.sqrt)
-    exp = staticmethod(math2.exp)
-    ln = log = staticmethod(math2.log)
-    cos = staticmethod(math2.cos)
-    sin = staticmethod(math2.sin)
-    tan = staticmethod(math2.tan)
-    cos_sin = staticmethod(math2.cos_sin)
-    acos = staticmethod(math2.acos)
-    asin = staticmethod(math2.asin)
-    atan = staticmethod(math2.atan)
-    cosh = staticmethod(math2.cosh)
-    sinh = staticmethod(math2.sinh)
-    tanh = staticmethod(math2.tanh)
-    gamma = staticmethod(math2.gamma)
-    rgamma = staticmethod(math2.rgamma)
-    fac = factorial = staticmethod(math2.factorial)
-    floor = staticmethod(math2.floor)
-    ceil = staticmethod(math2.ceil)
-    cospi = staticmethod(math2.cospi)
-    sinpi = staticmethod(math2.sinpi)
-    cbrt = staticmethod(math2.cbrt)
-    _nthroot = staticmethod(math2.nthroot)
-    _ei = staticmethod(math2.ei)
-    _e1 = staticmethod(math2.e1)
-    _zeta = _zeta_int = staticmethod(math2.zeta)
-
-    # XXX: math2
-    def arg(ctx, z):
-        z = complex(z)
-        return math.atan2(z.imag, z.real)
+    power = staticmethod(libfp.pow)
+    sqrt = staticmethod(libfp.sqrt)
+    exp = staticmethod(libfp.exp)
+    ln = log = staticmethod(libfp.log)
+    cos = staticmethod(libfp.cos)
+    sin = staticmethod(libfp.sin)
+    tan = staticmethod(libfp.tan)
+    cos_sin = staticmethod(libfp.cos_sin)
+    acos = staticmethod(libfp.acos)
+    asin = staticmethod(libfp.asin)
+    atan = staticmethod(libfp.atan)
+    cosh = staticmethod(libfp.cosh)
+    sinh = staticmethod(libfp.sinh)
+    tanh = staticmethod(libfp.tanh)
+    acosh = staticmethod(libfp.acosh)
+    asinh = staticmethod(libfp.asinh)
+    atanh = staticmethod(libfp.atanh)
+    gamma = staticmethod(libfp.gamma)
+    rgamma = staticmethod(libfp.rgamma)
+    fac = factorial = staticmethod(libfp.factorial)
+    floor = staticmethod(libfp.floor)
+    ceil = staticmethod(libfp.ceil)
+    cospi = staticmethod(libfp.cospi)
+    sinpi = staticmethod(libfp.sinpi)
+    cbrt = staticmethod(libfp.cbrt)
+    _nthroot = staticmethod(libfp.nthroot)
+    _ei = staticmethod(libfp.ei)
+    _e1 = staticmethod(libfp.e1)
+    _zeta = _zeta_int = staticmethod(libfp.zeta)
+    arg = staticmethod(cmath.phase)
 
     def expj(ctx, x):
         return ctx.exp(ctx.j*x)
 
     def expjpi(ctx, x):
         return ctx.exp(ctx.j*ctx.pi*x)
 
     ldexp = math.ldexp
     frexp = math.frexp
 
     def mag(ctx, z):
         if z:
-            return ctx.frexp(abs(z))[1]
+            n, e = ctx.frexp(abs(z))
+            if e:
+                return e
+            return ctx.convert(n)
         return ctx.ninf
 
     def isint(ctx, z):
-        if hasattr(z, "imag"):   # float/int don't have .real/.imag in py2.5
-            if z.imag:
-                return False
-            z = z.real
+        if z.imag:
+            return False
+        z = z.real
         try:
             return z == int(z)
         except:
             return False
 
     def nint_distance(ctx, z):
-        if hasattr(z, "imag"):   # float/int don't have .real/.imag in py2.5
-            n = round(z.real)
-        else:
-            n = round(z)
+        n = round(z.real)
         if n == z:
             return n, ctx.ninf
         return n, ctx.mag(abs(z-n))
 
     def _convert_param(ctx, z):
         if type(z) is tuple:
             p, q = z
             return ctx.mpf(p) / q, 'R'
-        if hasattr(z, "imag"):    # float/int don't have .real/.imag in py2.5
-            intz = int(z.real)
-        else:
-            intz = int(z)
+        intz = int(z.real)
         if z == intz:
             return intz, 'Z'
         return z, 'R'
 
     def _is_real_type(ctx, z):
         return isinstance(z, float) or isinstance(z, int_types)
 
@@ -208,24 +201,23 @@
             for i in den: t /= (coeffs[i]+k)
             k += 1; t /= k; t *= z; s += t
             if abs(t) < tol:
                 return s
             if k > maxterms:
                 raise ctx.NoConvergence
 
-    def atan2(ctx, x, y):
-        return math.atan2(x, y)
+    atan2 = staticmethod(math.atan2)
 
     def psi(ctx, m, z):
         m = int(m)
         if m == 0:
             return ctx.digamma(z)
         return (-1)**(m+1) * ctx.fac(m) * ctx.zeta(m+1, z)
 
-    digamma = staticmethod(math2.digamma)
+    digamma = staticmethod(libfp.digamma)
 
     def harmonic(ctx, x):
         x = ctx.convert(x)
         if x == 0 or x == 1:
             return x
         return ctx.digamma(x+1) + ctx.euler
 
@@ -234,16 +226,16 @@
     def to_fixed(ctx, x, prec):
         return int(math.ldexp(x, prec))
 
     def rand(ctx):
         import random
         return random.random()
 
-    _erf = staticmethod(math2.erf)
-    _erfc = staticmethod(math2.erfc)
+    _erf = staticmethod(math.erf)
+    _erfc = staticmethod(math.erfc)
 
     def sum_accurately(ctx, terms, check_step=1):
         s = ctx.zero
         k = 0
         for term in terms():
             s += term
             if (not k % check_step) and term:
```

### Comparing `mpmath-1.3.0/mpmath/ctx_iv.py` & `mpmath-1.4.0a0/mpmath/ctx_iv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,36 @@
-import operator
+import numbers
 
 from . import libmp
-
-from .libmp.backend import basestring
-
-from .libmp import (
-    int_types, MPZ_ONE,
-    prec_to_dps, dps_to_prec, repr_dps,
-    round_floor, round_ceiling,
-    fzero, finf, fninf, fnan,
-    mpf_le, mpf_neg,
-    from_int, from_float, from_str, from_rational,
-    mpi_mid, mpi_delta, mpi_str,
-    mpi_abs, mpi_pos, mpi_neg, mpi_add, mpi_sub,
-    mpi_mul, mpi_div, mpi_pow_int, mpi_pow,
-    mpi_from_str,
-    mpci_pos, mpci_neg, mpci_add, mpci_sub, mpci_mul, mpci_div, mpci_pow,
-    mpci_abs, mpci_pow, mpci_exp, mpci_log,
-    ComplexResult,
-    mpf_hash, mpc_hash)
+from .libmp import (MPZ_ONE, ComplexResult, dps_to_prec, finf, fnan, fninf,
+                    from_float, from_int, from_str, fzero, int_types, mpc_hash,
+                    mpci_abs, mpci_add, mpci_div, mpci_mul, mpci_neg, mpci_pos,
+                    mpci_pow, mpci_sub, mpf_hash, mpf_le, mpf_neg, mpi_abs,
+                    mpi_add, mpi_delta, mpi_div, mpi_from_str, mpi_mid,
+                    mpi_mul, mpi_neg, mpi_pos, mpi_pow, mpi_str, mpi_sub,
+                    prec_to_dps, repr_dps, round_ceiling, round_floor)
 from .matrices.matrices import _matrix
 
+
 mpi_zero = (fzero, fzero)
 
 from .ctx_base import StandardBaseContext
 
+
 new = object.__new__
 
 def convert_mpf_(x, prec, rounding):
     if hasattr(x, "_mpf_"): return x._mpf_
     if isinstance(x, int_types): return from_int(x, prec, rounding)
     if isinstance(x, float): return from_float(x, prec, rounding)
-    if isinstance(x, basestring): return from_str(x, prec, rounding)
+    if isinstance(x, str): return from_str(x, prec, rounding)
     raise NotImplementedError
 
 
-class ivmpf(object):
+class ivmpf:
     """
     Interval arithmetic class. Precision is controlled by iv.prec.
     """
 
     def __new__(cls, x=0):
         return cls.ctx.convert(x)
 
@@ -144,15 +135,15 @@
         return self.ctx.make_mpf(mpi_pos(self._mpi_, self.ctx.prec))
     def __neg__(self):
         return self.ctx.make_mpf(mpi_neg(self._mpi_, self.ctx.prec))
 
     def ae(s, t, rel_eps=None, abs_eps=None):
         return s.ctx.almosteq(s, t, rel_eps, abs_eps)
 
-class ivmpc(object):
+class ivmpc:
 
     def __new__(cls, re=0, im=0):
         re = cls.ctx.convert(re)
         im = cls.ctx.convert(im)
         y = new(cls)
         y._mpci_ = re._mpi_, im._mpi_
         return y
@@ -400,30 +391,24 @@
         return a
 
     def make_mpc(ctx, v):
         a = new(ctx.mpc)
         a._mpci_ = v
         return a
 
-    def _mpq(ctx, pq):
-        p, q = pq
-        a = libmp.from_rational(p, q, ctx.prec, round_floor)
-        b = libmp.from_rational(p, q, ctx.prec, round_ceiling)
-        return ctx.make_mpf((a, b))
-
     def convert(ctx, x):
         if isinstance(x, (ctx.mpf, ctx.mpc)):
             return x
         if isinstance(x, ctx._constant):
             return +x
         if isinstance(x, complex) or hasattr(x, "_mpc_"):
             re = ctx.convert(x.real)
             im = ctx.convert(x.imag)
             return ctx.mpc(re,im)
-        if isinstance(x, basestring):
+        if isinstance(x, str):
             v = mpi_from_str(x, ctx.prec)
             return ctx.make_mpf(v)
         if hasattr(x, "_mpi_"):
             a, b = x._mpi_
         else:
             try:
                 a, b = x
@@ -534,18 +519,13 @@
             #if abs(t) < tol:
             #    return s
             if k > maxterms:
                 raise ctx.NoConvergence
 
 
 # Register with "numbers" ABC
-#     We do not subclass, hence we do not use the @abstractmethod checks. While
-#     this is less invasive it may turn out that we do not actually support
-#     parts of the expected interfaces.  See
-#     http://docs.python.org/2/library/numbers.html for list of abstract
-#     methods.
-try:
-    import numbers
-    numbers.Complex.register(ivmpc)
-    numbers.Real.register(ivmpf)
-except ImportError:
-    pass
+#   We do not subclass, hence we do not use the @abstractmethod checks. While
+#   this is less invasive it may turn out that we do not actually support
+#   parts of the expected interfaces.  See
+#   https://docs.python.org/3/library/numbers.html for list of abstract methods.
+numbers.Complex.register(ivmpc)
+numbers.Real.register(ivmpf)
```

### Comparing `mpmath-1.3.0/mpmath/ctx_mp.py` & `mpmath-1.4.0a0/mpmath/ctx_mp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,118 +1,82 @@
 """
 This module defines the mpf, mpc classes, and standard functions for
 operating with them.
 """
-__docformat__ = 'plaintext'
 
 import functools
-
 import re
+import warnings
 
+from . import function_docs, libmp
 from .ctx_base import StandardBaseContext
+from .libmp import (MPQ, MPZ_ONE, ComplexResult, dps_to_prec, finf, fnan,
+                    fninf, fone, from_rational, fzero, int_types, mpc_add,
+                    mpc_add_mpf, mpc_div, mpc_div_mpf, mpc_mul, mpc_mul_mpf,
+                    mpc_neg, mpc_sub, mpc_sub_mpf, mpc_to_str, mpf_add,
+                    mpf_apery, mpf_catalan, mpf_degree, mpf_div, mpf_e,
+                    mpf_euler, mpf_glaisher, mpf_khinchin, mpf_ln2, mpf_ln10,
+                    mpf_mertens, mpf_mul, mpf_neg, mpf_phi, mpf_pi, mpf_rand,
+                    mpf_sub, mpf_twinprime, repr_dps, to_str)
 
-from .libmp.backend import basestring, BACKEND
-
-from . import libmp
-
-from .libmp import (MPZ, MPZ_ZERO, MPZ_ONE, int_types, repr_dps,
-    round_floor, round_ceiling, dps_to_prec, round_nearest, prec_to_dps,
-    ComplexResult, to_pickable, from_pickable, normalize,
-    from_int, from_float, from_str, to_int, to_float, to_str,
-    from_rational, from_man_exp,
-    fone, fzero, finf, fninf, fnan,
-    mpf_abs, mpf_pos, mpf_neg, mpf_add, mpf_sub, mpf_mul, mpf_mul_int,
-    mpf_div, mpf_rdiv_int, mpf_pow_int, mpf_mod,
-    mpf_eq, mpf_cmp, mpf_lt, mpf_gt, mpf_le, mpf_ge,
-    mpf_hash, mpf_rand,
-    mpf_sum,
-    bitcount, to_fixed,
-    mpc_to_str,
-    mpc_to_complex, mpc_hash, mpc_pos, mpc_is_nonzero, mpc_neg, mpc_conjugate,
-    mpc_abs, mpc_add, mpc_add_mpf, mpc_sub, mpc_sub_mpf, mpc_mul, mpc_mul_mpf,
-    mpc_mul_int, mpc_div, mpc_div_mpf, mpc_pow, mpc_pow_mpf, mpc_pow_int,
-    mpc_mpf_div,
-    mpf_pow,
-    mpf_pi, mpf_degree, mpf_e, mpf_phi, mpf_ln2, mpf_ln10,
-    mpf_euler, mpf_catalan, mpf_apery, mpf_khinchin,
-    mpf_glaisher, mpf_twinprime, mpf_mertens,
-    int_types)
-
-from . import function_docs
-from . import rational
-
-new = object.__new__
 
 get_complex = re.compile(r'^\(?(?P<re>[\+\-]?\d*(\.\d*)?(e[\+\-]?\d+)?)??'
                          r'(?P<im>[\+\-]?\d*(\.\d*)?(e[\+\-]?\d+)?j)?\)?$')
 
-if BACKEND == 'sage':
-    from sage.libs.mpmath.ext_main import Context as BaseMPContext
-    # pickle hack
-    import sage.libs.mpmath.ext_main as _mpf_module
-else:
-    from .ctx_mp_python import PythonMPContext as BaseMPContext
-    from . import ctx_mp_python as _mpf_module
+def __getattr__(name):
+    if name == 'mpnumeric':
+        from .ctx_mp_python import mpnumeric
+        warnings.warn(f"{name} is deprecated", DeprecationWarning)
+        return mpnumeric
+    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
+
+from . import ctx_mp_python as _mpf_module
+from .ctx_mp_python import PythonMPContext as BaseMPContext
 
-from .ctx_mp_python import _mpf, _mpc, mpnumeric
 
 class MPContext(BaseMPContext, StandardBaseContext):
     """
     Context for multiprecision arithmetic with a global precision.
     """
 
     def __init__(ctx):
         BaseMPContext.__init__(ctx)
         ctx.trap_complex = False
         ctx.pretty = False
         ctx.types = [ctx.mpf, ctx.mpc, ctx.constant]
-        ctx._mpq = rational.mpq
         ctx.default()
         StandardBaseContext.__init__(ctx)
 
-        ctx.mpq = rational.mpq
         ctx.init_builtins()
 
         ctx.hyp_summators = {}
 
         ctx._init_aliases()
 
-        # XXX: automate
-        try:
-            ctx.bernoulli.im_func.func_doc = function_docs.bernoulli
-            ctx.primepi.im_func.func_doc = function_docs.primepi
-            ctx.psi.im_func.func_doc = function_docs.psi
-            ctx.atan2.im_func.func_doc = function_docs.atan2
-        except AttributeError:
-            # python 3
-            ctx.bernoulli.__func__.func_doc = function_docs.bernoulli
-            ctx.primepi.__func__.func_doc = function_docs.primepi
-            ctx.psi.__func__.func_doc = function_docs.psi
-            ctx.atan2.__func__.func_doc = function_docs.atan2
-
-        ctx.digamma.func_doc = function_docs.digamma
-        ctx.cospi.func_doc = function_docs.cospi
-        ctx.sinpi.func_doc = function_docs.sinpi
+        ctx.bernoulli.__func__.__doc__ = function_docs.bernoulli
+        ctx.primepi.__func__.__doc__ = function_docs.primepi
+        ctx.psi.__func__.__doc__ = function_docs.psi
+        ctx.atan2.__func__.__doc__ = function_docs.atan2
+
+        ctx.digamma.__doc__ = function_docs.digamma
+        ctx.cospi.__doc_ = function_docs.cospi
+        ctx.sinpi.__doc_ = function_docs.sinpi
 
     def init_builtins(ctx):
-
-        mpf = ctx.mpf
-        mpc = ctx.mpc
-
         # Exact constants
         ctx.one = ctx.make_mpf(fone)
         ctx.zero = ctx.make_mpf(fzero)
         ctx.j = ctx.make_mpc((fzero,fone))
         ctx.inf = ctx.make_mpf(finf)
         ctx.ninf = ctx.make_mpf(fninf)
         ctx.nan = ctx.make_mpf(fnan)
 
-        eps = ctx.constant(lambda prec, rnd: (0, MPZ_ONE, 1-prec, 1),
-            "epsilon of working precision", "eps")
-        ctx.eps = eps
+        ctx.eps = ctx.constant(lambda prec, rnd: (0, MPZ_ONE, 1-prec, 1),
+                               "epsilon of working precision", "eps",
+                               lambda: ctx.dps)
 
         # Approximate constants
         ctx.pi = ctx.constant(mpf_pi, "pi", "pi")
         ctx.ln2 = ctx.constant(mpf_ln2, "ln(2)", "ln2")
         ctx.ln10 = ctx.constant(mpf_ln10, "ln(10)", "ln10")
         ctx.phi = ctx.constant(mpf_phi, "Golden ratio phi", "phi")
         ctx.e = ctx.constant(mpf_e, "e = exp(1)", "e")
@@ -168,21 +132,14 @@
         ctx._ellipe = ctx._wrap_libmp_function(libmp.mpf_ellipe, libmp.mpc_ellipe)
         ctx.agm1 = ctx._wrap_libmp_function(libmp.mpf_agm1, libmp.mpc_agm1)
         ctx._erf = ctx._wrap_libmp_function(libmp.mpf_erf, None)
         ctx._erfc = ctx._wrap_libmp_function(libmp.mpf_erfc, None)
         ctx._zeta = ctx._wrap_libmp_function(libmp.mpf_zeta, libmp.mpc_zeta)
         ctx._altzeta = ctx._wrap_libmp_function(libmp.mpf_altzeta, libmp.mpc_altzeta)
 
-        # Faster versions
-        ctx.sqrt = getattr(ctx, "_sage_sqrt", ctx.sqrt)
-        ctx.exp = getattr(ctx, "_sage_exp", ctx.exp)
-        ctx.ln = getattr(ctx, "_sage_ln", ctx.ln)
-        ctx.cos = getattr(ctx, "_sage_cos", ctx.cos)
-        ctx.sin = getattr(ctx, "_sage_sin", ctx.sin)
-
     def to_fixed(ctx, x, prec):
         return x.to_fixed(prec)
 
     def hypot(ctx, x, y):
         r"""
         Computes the Euclidean norm of the vector `(x, y)`, equal
         to `\sqrt{x^2 + y^2}`. Both `x` and `y` must be real."""
@@ -245,16 +202,16 @@
                 pass
         if hasattr(a, '_mpf_'): a = (a._mpf_, libmp.fzero)
         else: a = a._mpc_
         if hasattr(b, '_mpf_'): b = (b._mpf_, libmp.fzero)
         else: b = b._mpc_
         return ctx.make_mpc(libmp.mpc_agm(a, b, prec, rounding))
 
-    def bernoulli(ctx, n):
-        return ctx.make_mpf(libmp.mpf_bernoulli(int(n), *ctx._prec_rounding))
+    def bernoulli(ctx, n, plus=False):
+        return ctx.make_mpf(libmp.mpf_bernoulli(int(n), *ctx._prec_rounding, plus=plus))
 
     def _zeta_int(ctx, n):
         return ctx.make_mpf(libmp.mpf_zeta_int(int(n), *ctx._prec_rounding))
 
     def atan2(ctx, y, x):
         x = ctx.convert(x)
         y = ctx.convert(y)
@@ -317,42 +274,42 @@
 
     def isnan(ctx, x):
         """
         Return *True* if *x* is a NaN (not-a-number), or for a complex
         number, whether either the real or complex part is NaN;
         otherwise return *False*::
 
-            >>> from mpmath import *
+            >>> from mpmath import isnan, nan, mpc
             >>> isnan(3.14)
             False
             >>> isnan(nan)
             True
             >>> isnan(mpc(3.14,2.72))
             False
             >>> isnan(mpc(3.14,nan))
             True
 
         """
         if hasattr(x, "_mpf_"):
             return x._mpf_ == fnan
         if hasattr(x, "_mpc_"):
             return fnan in x._mpc_
-        if isinstance(x, int_types) or isinstance(x, rational.mpq):
+        if isinstance(x, int_types) or isinstance(x, MPQ):
             return False
         x = ctx.convert(x)
         if hasattr(x, '_mpf_') or hasattr(x, '_mpc_'):
             return ctx.isnan(x)
         raise TypeError("isnan() needs a number as input")
 
     def isfinite(ctx, x):
         """
         Return *True* if *x* is a finite number, i.e. neither
         an infinity or a NaN.
 
-            >>> from mpmath import *
+            >>> from mpmath import isfinite, inf, nan, mpc
             >>> isfinite(inf)
             False
             >>> isfinite(-inf)
             False
             >>> isfinite(3)
             True
             >>> isfinite(nan)
@@ -378,16 +335,16 @@
         if hasattr(x, '_mpf_'):
             sign, man, exp, bc = x._mpf_
             return sign and exp >= 0
         if hasattr(x, '_mpc_'):
             return not x.imag and ctx.isnpint(x.real)
         if type(x) in int_types:
             return x <= 0
-        if isinstance(x, ctx.mpq):
-            p, q = x._mpq_
+        if isinstance(x, MPQ):
+            p, q = x.numerator, x.denominator
             if not p:
                 return True
             return q == 1 and p <= 0
         return ctx.isnpint(ctx.convert(x))
 
     def __str__(ctx):
         lines = ["Mpmath settings:",
@@ -470,28 +427,27 @@
         **Examples**
 
         Many functions are sensitive to perturbations of the input arguments.
         If the arguments are decimal numbers, they may have to be converted
         to binary at a much higher precision. If the amount of required
         extra precision is unknown, :func:`~mpmath.autoprec` is convenient::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15
+            >>> from mpmath import mp, besselj, autoprec, sin, pi, exp, expm1
             >>> mp.pretty = True
             >>> besselj(5, 125 * 10**28)    # Exact input
             -8.03284785591801e-17
             >>> besselj(5, '1.25e30')   # Bad
             7.12954868316652e-16
             >>> autoprec(besselj)(5, '1.25e30')   # Good
             -8.03284785591801e-17
 
         The following fails to converge because `\sin(\pi) = 0` whereas all
         finite-precision approximations of `\pi` give nonzero values::
 
-            >>> autoprec(sin)(pi) # doctest: +IGNORE_EXCEPTION_DETAIL
+            >>> autoprec(sin)(pi)
             Traceback (most recent call last):
               ...
             NoConvergence: autoprec: prec increased to 2910 without convergence
 
         As the following example shows, :func:`~mpmath.autoprec` can protect against
         cancellation, but is fooled by too severe cancellation::
 
@@ -572,25 +528,25 @@
         to each element. For unrecognized classes, :func:`~mpmath.nstr`
         simply returns ``str(x)``.
 
         The companion function :func:`~mpmath.nprint` prints the result
         instead of returning it.
 
         The keyword arguments *strip_zeros*, *min_fixed*, *max_fixed*
-        and *show_zero_exponent* are forwarded to :func:`~mpmath.libmp.to_str`.
+        and *show_zero_exponent* are forwarded to ``mpmath.libmp.to_str()``.
 
         The number will be printed in fixed-point format if the position
         of the leading digit is strictly between min_fixed
         (default = min(-dps/3,-5)) and max_fixed (default = dps).
 
         To force fixed-point format always, set min_fixed = -inf,
         max_fixed = +inf. To force floating-point format, set
         min_fixed >= max_fixed.
 
-            >>> from mpmath import *
+            >>> from mpmath import nstr, ldexp, mpf, pi, nprint
             >>> nstr([+pi, ldexp(1,-500)])
             '[3.14159, 3.05494e-151]'
             >>> nprint([+pi, ldexp(1,-500)])
             [3.14159, 3.05494e-151]
             >>> nstr(mpf("5e-10"), 5)
             '5.0e-10'
             >>> nstr(mpf("5e-10"), 5, strip_zeros=False)
@@ -605,22 +561,22 @@
             return "[%s]" % (", ".join(ctx.nstr(c, n, **kwargs) for c in x))
         if isinstance(x, tuple):
             return "(%s)" % (", ".join(ctx.nstr(c, n, **kwargs) for c in x))
         if hasattr(x, '_mpf_'):
             return to_str(x._mpf_, n, **kwargs)
         if hasattr(x, '_mpc_'):
             return "(" + mpc_to_str(x._mpc_, n, **kwargs)  + ")"
-        if isinstance(x, basestring):
+        if isinstance(x, str):
             return repr(x)
         if isinstance(x, ctx.matrix):
             return x.__nstr__(n, **kwargs)
         return str(x)
 
     def _convert_fallback(ctx, x, strings):
-        if strings and isinstance(x, basestring):
+        if strings and isinstance(x, str):
             if 'j' in x.lower():
                 x = x.lower().replace(' ', '')
                 match = get_complex.match(x)
                 re = match.group('re')
                 if not re:
                     re = 0
                 im = match.group('im').rstrip('j')
@@ -701,15 +657,15 @@
                     magnitude_check[n] += d
                 else:
                     magnitude_check[n] = d
                 extraprec = max(extraprec, d - prec + 60)
             max_total_jump += abs(d)
         while 1:
             if extraprec > maxprec:
-                raise ValueError(ctx._hypsum_msg % (prec, prec+extraprec))
+                raise ctx.NoConvergence(ctx._hypsum_msg % (prec, prec+extraprec))
             wp = prec + extraprec
             if magnitude_check:
                 mag_dict = dict((n,None) for n in magnitude_check)
             else:
                 mag_dict = {}
             zv, have_complex, magnitude = summator(coeffs, v, prec, wp, \
                 epsshift, mag_dict, **kwargs)
@@ -750,16 +706,15 @@
 
     def ldexp(ctx, x, n):
         r"""
         Computes `x 2^n` efficiently. No rounding is performed.
         The argument `x` must be a real floating-point number (or
         possible to convert into one) and `n` must be a Python ``int``.
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import ldexp
             >>> ldexp(1, 10)
             mpf('1024.0')
             >>> ldexp(1, -3)
             mpf('0.125')
 
         """
         x = ctx.convert(x)
@@ -767,16 +722,15 @@
 
     def frexp(ctx, x):
         r"""
         Given a real number `x`, returns `(y, n)` with `y \in [0.5, 1)`,
         `n` a Python integer, and such that `x = y 2^n`. No rounding is
         performed.
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import frexp
             >>> frexp(7.5)
             (mpf('0.9375'), 3)
 
         """
         x = ctx.convert(x)
         y, n = libmp.mpf_frexp(x._mpf_)
         return ctx.make_mpf(y), n
@@ -789,16 +743,15 @@
         See the documentation of :func:`~mpmath.fadd` for a detailed description
         of how to specify precision and rounding.
 
         **Examples**
 
         An mpmath number is returned::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fneg, fadd, mpf, log, inf
             >>> fneg(2.5)
             mpf('-2.5')
             >>> fneg(-5+2j)
             mpc(real='5.0', imag='-2.0')
 
         Precise control over rounding is possible::
 
@@ -851,16 +804,15 @@
         nearest (default), ``'f'`` for floor, ``'c'`` for ceiling, ``'d'``
         for down, ``'u'`` for up.
 
         **Examples**
 
         Using :func:`~mpmath.fadd` with precision and rounding control::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fadd, nprint, mpf, inf
             >>> fadd(2, 1e-20)
             mpf('2.0')
             >>> fadd(2, 1e-20, rounding='u')
             mpf('2.0000000000000004')
             >>> nprint(fadd(2, 1e-20, prec=100), 25)
             2.00000000000000000001
             >>> nprint(fadd(2, 1e-20, dps=15), 25)
@@ -917,16 +869,15 @@
         See the documentation of :func:`~mpmath.fadd` for a detailed description
         of how to specify precision and rounding.
 
         **Examples**
 
         Using :func:`~mpmath.fsub` with precision and rounding control::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fsub, nprint, mpf, inf
             >>> fsub(2, 1e-20)
             mpf('2.0')
             >>> fsub(2, 1e-20, rounding='d')
             mpf('1.9999999999999998')
             >>> nprint(fsub(2, 1e-20, prec=100), 25)
             1.99999999999999999999
             >>> nprint(fsub(2, 1e-20, dps=15), 25)
@@ -983,16 +934,15 @@
         See the documentation of :func:`~mpmath.fadd` for a detailed description
         of how to specify precision and rounding.
 
         **Examples**
 
         The result is an mpmath number::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fmul, mpf, mpc
             >>> fmul(2, 5.0)
             mpf('10.0')
             >>> fmul(0.5j, 0.5)
             mpc(real='0.0', imag='0.25')
 
         Avoiding roundoff::
 
@@ -1052,16 +1002,15 @@
         See the documentation of :func:`~mpmath.fadd` for a detailed description
         of how to specify precision and rounding.
 
         **Examples**
 
         The result is an mpmath number::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fdiv
             >>> fdiv(3, 2)
             mpf('1.5')
             >>> fdiv(2, 3)
             mpf('0.66666666666666663')
             >>> fdiv(2+4j, 0.5)
             mpc(real='4.0', imag='8.0')
 
@@ -1112,15 +1061,15 @@
 
     def nint_distance(ctx, x):
         r"""
         Return `(n,d)` where `n` is the nearest integer to `x` and `d` is
         an estimate of `\log_2(|x-n|)`. If `d < 0`, `-d` gives the precision
         (measured in bits) lost to cancellation when computing `x-n`.
 
-            >>> from mpmath import *
+            >>> from mpmath import nint_distance, mpf, mpc
             >>> n, d = nint_distance(5)
             >>> print(n); print(d)
             5
             -inf
             >>> n, d = nint_distance(mpf(5))
             >>> print(n); print(d)
             5
@@ -1142,23 +1091,23 @@
             5
             -19
 
         """
         typx = type(x)
         if typx in int_types:
             return int(x), ctx.ninf
-        elif typx is rational.mpq:
-            p, q = x._mpq_
+        elif typx is MPQ:
+            p, q = x.numerator, x.denominator
             n, r = divmod(p, q)
             if 2*r >= q:
                 n += 1
             elif not r:
                 return n, ctx.ninf
             # log(p/q-n) = log((p-nq)/q) = log(p-nq) - log(q)
-            d = bitcount(abs(p-n*q)) - bitcount(q)
+            d = (p-n*q).bit_length() - q.bit_length()
             return n, d
         if hasattr(x, "_mpf_"):
             re = x._mpf_
             im_dist = ctx.ninf
         elif hasattr(x, "_mpc_"):
             re, im = x._mpc_
             isign, iman, iexp, ibc = im
@@ -1194,15 +1143,15 @@
                 t = man >> d
                 if t & 1:
                     t += 1
                     man = (t<<d) - man
                 else:
                     man -= (t<<d)
                 n = t>>1   # int(t)>>1
-                re_dist = exp+bitcount(man)
+                re_dist = exp+man.bit_length()
             if sign:
                 n = -n
         elif re == fzero:
             re_dist = ctx.ninf
             n = 0
         else:
             raise ValueError("requires a finite number")
@@ -1210,16 +1159,15 @@
 
     def fprod(ctx, factors):
         r"""
         Calculates a product containing a finite number of factors (for
         infinite products, see :func:`~mpmath.nprod`). The factors will be
         converted to mpmath numbers.
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fprod
             >>> fprod([1, 2, 0.5, 7])
             mpf('7.0')
 
         """
         orig = ctx.prec
         try:
             v = ctx.one
@@ -1238,26 +1186,24 @@
         return ctx.make_mpf(mpf_rand(ctx._prec))
 
     def fraction(ctx, p, q):
         """
         Given Python integers `(p, q)`, returns a lazy ``mpf`` representing
         the fraction `p/q`. The value is updated with the precision.
 
-            >>> from mpmath import *
-            >>> mp.dps = 15
+            >>> from mpmath import fraction, mpf, mp
             >>> a = fraction(1,100)
             >>> b = mpf(1)/100
             >>> print(a); print(b)
             0.01
             0.01
             >>> mp.dps = 30
             >>> print(a); print(b)      # a will be accurate
             0.01
             0.0100000000000000002081668171172
-            >>> mp.dps = 15
         """
         return ctx.constant(lambda prec, rnd: from_rational(p, q, prec, rnd),
             '%s/%s' % (p, q))
 
     def absmin(ctx, x):
         return abs(ctx.convert(x))
 
@@ -1328,12 +1274,7 @@
         if self.precfun:
             self.ctx.prec = self.precfun(self.ctx.prec)
         else:
             self.ctx.dps = self.dpsfun(self.ctx.dps)
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.ctx.prec = self.origp
         return False
-
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/ctx_mp_python.py` & `mpmath-1.4.0a0/mpmath/ctx_mp_python.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-#from ctx_base import StandardBaseContext
+import numbers
 
-from .libmp.backend import basestring, exec_
-
-from .libmp import (MPZ, MPZ_ZERO, MPZ_ONE, int_types, repr_dps,
-    round_floor, round_ceiling, dps_to_prec, round_nearest, prec_to_dps,
-    ComplexResult, to_pickable, from_pickable, normalize,
-    from_int, from_float, from_npfloat, from_Decimal, from_str, to_int, to_float, to_str,
-    from_rational, from_man_exp,
-    fone, fzero, finf, fninf, fnan,
-    mpf_abs, mpf_pos, mpf_neg, mpf_add, mpf_sub, mpf_mul, mpf_mul_int,
-    mpf_div, mpf_rdiv_int, mpf_pow_int, mpf_mod,
-    mpf_eq, mpf_cmp, mpf_lt, mpf_gt, mpf_le, mpf_ge,
-    mpf_hash, mpf_rand,
-    mpf_sum,
-    bitcount, to_fixed,
-    mpc_to_str,
-    mpc_to_complex, mpc_hash, mpc_pos, mpc_is_nonzero, mpc_neg, mpc_conjugate,
-    mpc_abs, mpc_add, mpc_add_mpf, mpc_sub, mpc_sub_mpf, mpc_mul, mpc_mul_mpf,
-    mpc_mul_int, mpc_div, mpc_div_mpf, mpc_pow, mpc_pow_mpf, mpc_pow_int,
-    mpc_mpf_div,
-    mpf_pow,
-    mpf_pi, mpf_degree, mpf_e, mpf_phi, mpf_ln2, mpf_ln10,
-    mpf_euler, mpf_catalan, mpf_apery, mpf_khinchin,
-    mpf_glaisher, mpf_twinprime, mpf_mertens,
-    int_types)
-
-from . import rational
 from . import function_docs
+from .libmp import (MPQ, MPZ, ComplexResult, dps_to_prec, finf, fnan, fninf,
+                    from_Decimal, from_float, from_int, from_man_exp,
+                    from_npfloat, from_rational, from_str, fzero, int_types,
+                    mpc_abs, mpc_add, mpc_add_mpf, mpc_conjugate, mpc_div,
+                    mpc_div_mpf, mpc_hash, mpc_is_nonzero, mpc_mpf_div,
+                    mpc_mul, mpc_mul_int, mpc_mul_mpf, mpc_neg, mpc_pos,
+                    mpc_pow, mpc_pow_int, mpc_pow_mpf, mpc_sub, mpc_sub_mpf,
+                    mpc_to_complex, mpc_to_str, mpf_abs, mpf_add, mpf_cmp,
+                    mpf_div, mpf_eq, mpf_ge, mpf_gt, mpf_hash, mpf_le, mpf_lt,
+                    mpf_mod, mpf_mul, mpf_mul_int, mpf_neg, mpf_pos, mpf_pow,
+                    mpf_pow_int, mpf_rdiv_int, mpf_sub, mpf_sum, normalize,
+                    prec_to_dps, round_nearest, to_fixed, to_float, to_int,
+                    to_rational, to_str)
+
 
 new = object.__new__
 
-class mpnumeric(object):
+class mpnumeric:
     """Base class for mpf and mpc."""
     __slots__ = []
     def __new__(cls, val):
         raise NotImplementedError
 
 class _mpf(mpnumeric):
     """
@@ -50,64 +38,60 @@
         format."""
         prec, rounding = cls.context._prec_rounding
         if kwargs:
             prec = kwargs.get('prec', prec)
             if 'dps' in kwargs:
                 prec = dps_to_prec(kwargs['dps'])
             rounding = kwargs.get('rounding', rounding)
+        v = new(cls)
         if type(val) is cls:
-            sign, man, exp, bc = val._mpf_
-            if (not man) and exp:
-                return val
-            v = new(cls)
-            v._mpf_ = normalize(sign, man, exp, bc, prec, rounding)
-            return v
+            val = val._mpf_
         elif type(val) is tuple:
-            if len(val) == 2:
-                v = new(cls)
-                v._mpf_ = from_man_exp(val[0], val[1], prec, rounding)
-                return v
             if len(val) == 4:
-                if val not in (finf, fninf, fnan):
-                    sign, man, exp, bc = val
-                    val = normalize(sign, MPZ(man), exp, bc, prec, rounding)
-                v = new(cls)
-                v._mpf_ = val
+                pass
+            elif len(val) == 2:
+                v._mpf_ = from_man_exp(val[0], val[1], prec, rounding)
                 return v
-            raise ValueError
+            else:
+                raise ValueError
         else:
-            v = new(cls)
-            v._mpf_ = mpf_pos(cls.mpf_convert_arg(val, prec, rounding), prec, rounding)
-            return v
+            val = cls.mpf_convert_arg(val, prec, rounding)
+        v._mpf_ = mpf_pos(val, prec, rounding)
+        return v
 
     @classmethod
     def mpf_convert_arg(cls, x, prec, rounding):
         if isinstance(x, int_types): return from_int(x)
         if isinstance(x, float): return from_float(x)
-        if isinstance(x, basestring): return from_str(x, prec, rounding)
+        if isinstance(x, str): return from_str(x, prec, rounding)
         if isinstance(x, cls.context.constant): return x.func(prec, rounding)
+        if isinstance(x, numbers.Rational): return from_rational(x.numerator,
+                                                                 x.denominator,
+                                                                 prec, rounding)
         if hasattr(x, '_mpf_'): return x._mpf_
         if hasattr(x, '_mpmath_'):
             t = cls.context.convert(x._mpmath_(prec, rounding))
             if hasattr(t, '_mpf_'):
                 return t._mpf_
         if hasattr(x, '_mpi_'):
             a, b = x._mpi_
             if a == b:
                 return a
             raise ValueError("can only create mpf from zero-width interval")
+        if type(x).__module__ == 'decimal':
+            return from_Decimal(x, prec, rounding)
         raise TypeError("cannot create mpf from " + repr(x))
 
     @classmethod
     def mpf_convert_rhs(cls, x):
         if isinstance(x, int_types): return from_int(x)
         if isinstance(x, float): return from_float(x)
         if isinstance(x, complex_types): return cls.context.mpc(x)
-        if isinstance(x, rational.mpq):
-            p, q = x._mpq_
+        if isinstance(x, MPQ):
+            p, q = x.numerator, x.denominator
             return from_rational(p, q, cls.context.prec)
         if hasattr(x, '_mpf_'): return x._mpf_
         if hasattr(x, '_mpmath_'):
             t = cls.context.convert(x._mpmath_(*cls.context._prec_rounding))
             if hasattr(t, '_mpf_'):
                 return t._mpf_
             return t
@@ -126,31 +110,30 @@
     bc = property(lambda self: self._mpf_[3])
 
     real = property(lambda self: self)
     imag = property(lambda self: self.context.zero)
 
     conjugate = lambda self: self
 
-    def __getstate__(self): return to_pickable(self._mpf_)
-    def __setstate__(self, val): self._mpf_ = from_pickable(val)
+    def as_integer_ratio(self):
+        return to_rational(self._mpf_)
+
+    def __reduce__(self): return self.__class__, (self._mpf_,)
 
     def __repr__(s):
         if s.context.pretty:
             return str(s)
         return "mpf('%s')" % to_str(s._mpf_, s.context._repr_digits)
 
     def __str__(s): return to_str(s._mpf_, s.context._str_digits)
     def __hash__(s): return mpf_hash(s._mpf_)
     def __int__(s): return int(to_int(s._mpf_))
-    def __long__(s): return long(to_int(s._mpf_))
     def __float__(s): return to_float(s._mpf_, rnd=s.context._prec_rounding[1])
     def __complex__(s): return complex(float(s))
-    def __nonzero__(s): return s._mpf_ != fzero
-
-    __bool__ = __nonzero__
+    def __bool__(s): return s._mpf_ != fzero
 
     def __abs__(s):
         cls, new, (prec, rounding) = s._ctxdata
         v = new(cls)
         v._mpf_ = mpf_abs(s._mpf_, prec, rounding)
         return v
 
@@ -171,176 +154,359 @@
             t = t._mpf_
         else:
             t = s.mpf_convert_rhs(t)
             if t is NotImplemented:
                 return t
         return func(s._mpf_, t)
 
-    def __cmp__(s, t): return s._cmp(t, mpf_cmp)
     def __lt__(s, t): return s._cmp(t, mpf_lt)
     def __gt__(s, t): return s._cmp(t, mpf_gt)
     def __le__(s, t): return s._cmp(t, mpf_le)
     def __ge__(s, t): return s._cmp(t, mpf_ge)
 
-    def __ne__(s, t):
-        v = s.__eq__(t)
-        if v is NotImplemented:
-            return v
-        return not v
+    def __eq__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            return mpf_eq(sval, tval)
+        if hasattr(other, '_mpc_'):
+            tval = other._mpc_
+            mpc = type(other)
+            return (tval[1] == fzero) and mpf_eq(tval[0], sval)
+        ttype = type(other)
+        if ttype in int_types:
+            return mpf_eq(sval, from_int(other))
+        if ttype is float:
+            tval = from_float(other)
+            return mpf_eq(sval, tval)
+        if ttype is complex:
+            tval = from_float(other.real), from_float(other.imag)
+            mpc = self.context.mpc
+            return (tval[1] == fzero) and mpf_eq(tval[0], sval)
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__eq__(other)
+
+    def __add__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            val = mpf_add(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if hasattr(other, '_mpc_'):
+            tval = other._mpc_
+            mpc = type(other)
+            val = mpc_add_mpf(tval, sval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        ttype = type(other)
+        if ttype in int_types:
+            val = mpf_add(sval, from_int(other), prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is float:
+            tval = from_float(other)
+            val = mpf_add(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is complex:
+            tval = from_float(other.real), from_float(other.imag)
+            val = mpc_add_mpf(tval, sval, prec, rounding)
+            mpc = self.context.mpc
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__add__(other)
+    __radd__ = __add__
+
+    def __sub__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            val = mpf_sub(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if hasattr(other, '_mpc_'):
+            tval = other._mpc_
+            mpc = type(other)
+            val = mpc_sub((sval, fzero), tval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        ttype = type(other)
+        if ttype in int_types:
+            val = mpf_sub(sval, from_int(other), prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is float:
+            tval = from_float(other)
+            val = mpf_sub(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is complex:
+            tval = from_float(other.real), from_float(other.imag)
+            mpc = self.context.mpc
+            val = mpc_sub((sval, fzero), tval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__sub__(other)
 
     def __rsub__(s, t):
         cls, new, (prec, rounding) = s._ctxdata
         if type(t) in int_types:
             v = new(cls)
             v._mpf_ = mpf_sub(from_int(t), s._mpf_, prec, rounding)
             return v
         t = s.mpf_convert_lhs(t)
         if t is NotImplemented:
             return t
         return t - s
 
-    def __rdiv__(s, t):
+    def __mul__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            val = mpf_mul(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if hasattr(other, '_mpc_'):
+            tval = other._mpc_
+            mpc = type(other)
+            val = mpc_mul_mpf(tval, sval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        ttype = type(other)
+        if ttype in int_types:
+            val = mpf_mul_int(sval, other, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is float:
+            tval = from_float(other)
+            val = mpf_mul(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is complex:
+            tval = from_float(other.real), from_float(other.imag)
+            mpc = self.context.mpc
+            val = mpc_mul_mpf(tval, sval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__mul__(other)
+    __rmul__ = __mul__
+
+    def __truediv__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            val = mpf_div(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if hasattr(other, '_mpc_'):
+            tval = other._mpc_
+            mpc = type(other)
+            val = mpc_mpf_div(sval, tval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        ttype = type(other)
+        if ttype in int_types:
+            val = mpf_div(sval, from_int(other), prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is float:
+            tval = from_float(other)
+            val = mpf_div(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is complex:
+            tval = from_float(other.real), from_float(other.imag)
+            mpc = self.context.mpc
+            val = mpc_mpf_div(sval, tval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__truediv__(other)
+
+    def __rtruediv__(s, t):
         cls, new, (prec, rounding) = s._ctxdata
         if isinstance(t, int_types):
             v = new(cls)
             v._mpf_ = mpf_rdiv_int(t, s._mpf_, prec, rounding)
             return v
         t = s.mpf_convert_lhs(t)
         if t is NotImplemented:
             return t
         return t / s
 
-    def __rpow__(s, t):
+    def __mod__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            val = mpf_mod(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if hasattr(other, '_mpc_'):
+            return NotImplemented
+        ttype = type(other)
+        if ttype in int_types:
+            val = mpf_mod(sval, from_int(other), prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is float:
+            tval = from_float(other)
+            val = mpf_mod(sval, tval, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is complex:
+            return NotImplemented
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__mod__(other)
+
+    def __rmod__(s, t):
         t = s.mpf_convert_lhs(t)
         if t is NotImplemented:
             return t
-        return t ** s
+        return t % s
 
-    def __rmod__(s, t):
+    def __pow__(self, other):
+        mpf, new, (prec, rounding) = self._ctxdata
+        sval = self._mpf_
+        if hasattr(other, '_mpf_'):
+            tval = other._mpf_
+            try:
+                val = mpf_pow(sval, tval, prec, rounding)
+                obj = new(mpf)
+                obj._mpf_ = val
+                return obj
+            except ComplexResult:
+                if mpf.context.trap_complex:
+                    raise
+                mpc = mpf.context.mpc
+                val = mpc_pow((sval, fzero), (tval, fzero), prec, rounding)
+                obj = new(mpc)
+                obj._mpc_ = val
+                return obj
+        if hasattr(other, '_mpc_'):
+            tval = other._mpc_
+            mpc = type(other)
+            val = mpc_pow((sval, fzero), tval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        ttype = type(other)
+        if ttype in int_types:
+            val = mpf_pow_int(sval, other, prec, rounding)
+            obj = new(mpf)
+            obj._mpf_ = val
+            return obj
+        if ttype is float:
+            tval = from_float(other)
+            try:
+                val = mpf_pow(sval, tval, prec, rounding)
+                obj = new(mpf)
+                obj._mpf_ = val
+                return obj
+            except ComplexResult:
+                if mpf.context.trap_complex:
+                    raise
+                mpc = mpf.context.mpc
+                val = mpc_pow((sval, fzero), (tval, fzero), prec, rounding)
+                obj = new(mpc)
+                obj._mpc_ = val
+                return obj
+        if ttype is complex:
+            tval = from_float(other.real), from_float(other.imag)
+            mpc = self.context.mpc
+            val = mpc_pow((sval, fzero), tval, prec, rounding)
+            obj = new(mpc)
+            obj._mpc_ = val
+            return obj
+        try:
+            other = mpf.context.convert(other, strings=False)
+        except TypeError:
+            return NotImplemented
+        return self.__pow__(other)
+
+    def __rpow__(s, t):
         t = s.mpf_convert_lhs(t)
         if t is NotImplemented:
             return t
-        return t % s
+        return t ** s
 
     def sqrt(s):
         return s.context.sqrt(s)
 
     def ae(s, t, rel_eps=None, abs_eps=None):
         return s.context.almosteq(s, t, rel_eps, abs_eps)
 
     def to_fixed(self, prec):
         return to_fixed(self._mpf_, prec)
 
     def __round__(self, *args):
         return round(float(self), *args)
 
-mpf_binary_op = """
-def %NAME%(self, other):
-    mpf, new, (prec, rounding) = self._ctxdata
-    sval = self._mpf_
-    if hasattr(other, '_mpf_'):
-        tval = other._mpf_
-        %WITH_MPF%
-    ttype = type(other)
-    if ttype in int_types:
-        %WITH_INT%
-    elif ttype is float:
-        tval = from_float(other)
-        %WITH_MPF%
-    elif hasattr(other, '_mpc_'):
-        tval = other._mpc_
-        mpc = type(other)
-        %WITH_MPC%
-    elif ttype is complex:
-        tval = from_float(other.real), from_float(other.imag)
-        mpc = self.context.mpc
-        %WITH_MPC%
-    if isinstance(other, mpnumeric):
-        return NotImplemented
-    try:
-        other = mpf.context.convert(other, strings=False)
-    except TypeError:
-        return NotImplemented
-    return self.%NAME%(other)
-"""
-
-return_mpf = "; obj = new(mpf); obj._mpf_ = val; return obj"
-return_mpc = "; obj = new(mpc); obj._mpc_ = val; return obj"
-
-mpf_pow_same = """
-        try:
-            val = mpf_pow(sval, tval, prec, rounding) %s
-        except ComplexResult:
-            if mpf.context.trap_complex:
-                raise
-            mpc = mpf.context.mpc
-            val = mpc_pow((sval, fzero), (tval, fzero), prec, rounding) %s
-""" % (return_mpf, return_mpc)
-
-def binary_op(name, with_mpf='', with_int='', with_mpc=''):
-    code = mpf_binary_op
-    code = code.replace("%WITH_INT%", with_int)
-    code = code.replace("%WITH_MPC%", with_mpc)
-    code = code.replace("%WITH_MPF%", with_mpf)
-    code = code.replace("%NAME%", name)
-    np = {}
-    exec_(code, globals(), np)
-    return np[name]
-
-_mpf.__eq__ = binary_op('__eq__',
-    'return mpf_eq(sval, tval)',
-    'return mpf_eq(sval, from_int(other))',
-    'return (tval[1] == fzero) and mpf_eq(tval[0], sval)')
-
-_mpf.__add__ = binary_op('__add__',
-    'val = mpf_add(sval, tval, prec, rounding)' + return_mpf,
-    'val = mpf_add(sval, from_int(other), prec, rounding)' + return_mpf,
-    'val = mpc_add_mpf(tval, sval, prec, rounding)' + return_mpc)
-
-_mpf.__sub__ = binary_op('__sub__',
-    'val = mpf_sub(sval, tval, prec, rounding)' + return_mpf,
-    'val = mpf_sub(sval, from_int(other), prec, rounding)' + return_mpf,
-    'val = mpc_sub((sval, fzero), tval, prec, rounding)' + return_mpc)
-
-_mpf.__mul__ = binary_op('__mul__',
-    'val = mpf_mul(sval, tval, prec, rounding)' + return_mpf,
-    'val = mpf_mul_int(sval, other, prec, rounding)' + return_mpf,
-    'val = mpc_mul_mpf(tval, sval, prec, rounding)' + return_mpc)
-
-_mpf.__div__ = binary_op('__div__',
-    'val = mpf_div(sval, tval, prec, rounding)' + return_mpf,
-    'val = mpf_div(sval, from_int(other), prec, rounding)' + return_mpf,
-    'val = mpc_mpf_div(sval, tval, prec, rounding)' + return_mpc)
-
-_mpf.__mod__ = binary_op('__mod__',
-    'val = mpf_mod(sval, tval, prec, rounding)' + return_mpf,
-    'val = mpf_mod(sval, from_int(other), prec, rounding)' + return_mpf,
-    'raise NotImplementedError("complex modulo")')
-
-_mpf.__pow__ = binary_op('__pow__',
-    mpf_pow_same,
-    'val = mpf_pow_int(sval, other, prec, rounding)' + return_mpf,
-    'val = mpc_pow((sval, fzero), tval, prec, rounding)' + return_mpc)
-
-_mpf.__radd__ = _mpf.__add__
-_mpf.__rmul__ = _mpf.__mul__
-_mpf.__truediv__ = _mpf.__div__
-_mpf.__rtruediv__ = _mpf.__rdiv__
-
 
 class _constant(_mpf):
     """Represents a mathematical constant with dynamic precision.
     When printed or used in an arithmetic operation, a constant
     is converted to a regular mpf at the working precision. A
     regular mpf can also be obtained using the operation +x."""
 
-    def __new__(cls, func, name, docname=''):
+    def __new__(cls, func, name, docname='', _reprdps_getter=lambda: 15):
         a = object.__new__(cls)
         a.name = name
         a.func = func
+        a._reprdps_getter = _reprdps_getter
         a.__doc__ = getattr(function_docs, docname, '')
         return a
 
     def __call__(self, prec=None, dps=None, rounding=None):
         prec2, rounding2 = self.context._prec_rounding
         if not prec: prec = prec2
         if not rounding: rounding = rounding2
@@ -349,46 +515,53 @@
 
     @property
     def _mpf_(self):
         prec, rounding = self.context._prec_rounding
         return self.func(prec, rounding)
 
     def __repr__(self):
-        return "<%s: %s~>" % (self.name, self.context.nstr(self(dps=15)))
+        return "<%s: %s~>" % (self.name, self.context.nstr(self(dps=self._reprdps_getter())))
 
 
 class _mpc(mpnumeric):
     """
-    An mpc represents a complex number using a pair of mpf:s (one
+    An mpc represents a complex number using a pair of mpf's (one
     for the real part and another for the imaginary part.) The mpc
     class behaves fairly similarly to Python's complex type.
     """
 
     __slots__ = ['_mpc_']
 
     def __new__(cls, real=0, imag=0):
         s = object.__new__(cls)
+        if isinstance(real, str):
+            real = cls.context.convert(real)
         if isinstance(real, complex_types):
-            real, imag = real.real, real.imag
+            r_real, r_imag = real.real, real.imag
         elif hasattr(real, '_mpc_'):
-            s._mpc_ = real._mpc_
-            return s
-        real = cls.context.mpf(real)
-        imag = cls.context.mpf(imag)
+            r_real, r_imag = real._mpc_
+        else:
+            r_real, r_imag = real, 0
+        if isinstance(imag, complex_types):
+            i_real, i_imag = imag.real, imag.imag
+        elif hasattr(imag, '_mpc_'):
+            i_real, i_imag = imag._mpc_
+        else:
+            i_real, i_imag = imag, 0
+        r_real, r_imag = map(cls.context.mpf, [r_real, r_imag])
+        i_real, i_imag = map(cls.context.mpf, [i_real, i_imag])
+        real = r_real - i_imag
+        imag = r_imag + i_real
         s._mpc_ = (real._mpf_, imag._mpf_)
         return s
 
     real = property(lambda self: self.context.make_mpf(self._mpc_[0]))
     imag = property(lambda self: self.context.make_mpf(self._mpc_[1]))
 
-    def __getstate__(self):
-        return to_pickable(self._mpc_[0]), to_pickable(self._mpc_[1])
-
-    def __setstate__(self, val):
-        self._mpc_ = from_pickable(val[0]), from_pickable(val[1])
+    def __reduce__(self): return self.__class__, self._mpc_
 
     def __repr__(s):
         if s.context.pretty:
             return str(s)
         r = repr(s.real)[4:-1]
         i = repr(s.imag)[4:-1]
         return "%s(real=%s, imag=%s)" % (type(s).__name__, r, i)
@@ -419,19 +592,17 @@
 
     def conjugate(s):
         cls, new, (prec, rounding) = s._ctxdata
         v = new(cls)
         v._mpc_ = mpc_conjugate(s._mpc_, prec, rounding)
         return v
 
-    def __nonzero__(s):
+    def __bool__(s):
         return mpc_is_nonzero(s._mpc_)
 
-    __bool__ = __nonzero__
-
     def __hash__(s):
         return mpc_hash(s._mpc_)
 
     @classmethod
     def mpc_convert_lhs(cls, x):
         try:
             y = cls.context.convert(x)
@@ -444,28 +615,14 @@
             if isinstance(t, str):
                 return False
             t = s.mpc_convert_lhs(t)
             if t is NotImplemented:
                 return t
         return s.real == t.real and s.imag == t.imag
 
-    def __ne__(s, t):
-        b = s.__eq__(t)
-        if b is NotImplemented:
-            return b
-        return not b
-
-    def _compare(*args):
-        raise TypeError("no ordering relation is defined for complex numbers")
-
-    __gt__ = _compare
-    __le__ = _compare
-    __gt__ = _compare
-    __ge__ = _compare
-
     def __add__(s, t):
         cls, new, (prec, rounding) = s._ctxdata
         if not hasattr(t, '_mpc_'):
             t = s.mpc_convert_lhs(t)
             if t is NotImplemented:
                 return t
             if hasattr(t, '_mpf_'):
@@ -505,15 +662,15 @@
                 v._mpc_ = mpc_mul_mpf(s._mpc_, t._mpf_, prec, rounding)
                 return v
             t = s.mpc_convert_lhs(t)
         v = new(cls)
         v._mpc_ = mpc_mul(s._mpc_, t._mpc_, prec, rounding)
         return v
 
-    def __div__(s, t):
+    def __truediv__(s, t):
         cls, new, (prec, rounding) = s._ctxdata
         if not hasattr(t, '_mpc_'):
             t = s.mpc_convert_lhs(t)
             if t is NotImplemented:
                 return t
             if hasattr(t, '_mpf_'):
                 v = new(cls)
@@ -554,38 +711,34 @@
             v._mpc_ = mpc_mul_int(s._mpc_, t, prec, rounding)
             return v
         t = s.mpc_convert_lhs(t)
         if t is NotImplemented:
             return t
         return t * s
 
-    def __rdiv__(s, t):
+    def __rtruediv__(s, t):
         t = s.mpc_convert_lhs(t)
         if t is NotImplemented:
             return t
         return t / s
 
     def __rpow__(s, t):
         t = s.mpc_convert_lhs(t)
         if t is NotImplemented:
             return t
         return t ** s
 
-    __truediv__ = __div__
-    __rtruediv__ = __rdiv__
-
     def ae(s, t, rel_eps=None, abs_eps=None):
         return s.context.almosteq(s, t, rel_eps, abs_eps)
 
 
 complex_types = (complex, _mpc)
 
 
-class PythonMPContext(object):
-
+class PythonMPContext:
     def __init__(ctx):
         ctx._prec_rounding = [53, round_nearest]
         ctx.mpf = type('mpf', (_mpf,), {})
         ctx.mpc = type('mpc', (_mpc,), {})
         ctx.mpf._ctxdata = [ctx.mpf, new, ctx._prec_rounding]
         ctx.mpc._ctxdata = [ctx.mpc, new, ctx._prec_rounding]
         ctx.mpf.context = ctx
@@ -626,16 +779,15 @@
         ``mpc``, ``int``, ``float``, ``complex``, the conversion
         will be performed losslessly.
 
         If *x* is a string, the result will be rounded to the present
         working precision. Strings representing fractions or complex
         numbers are permitted.
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import mpmathify
             >>> mpmathify(3.5)
             mpf('3.5')
             >>> mpmathify('2.1')
             mpf('2.1000000000000001')
             >>> mpmathify('3/4')
             mpf('0.75')
             >>> mpmathify('2+3j')
@@ -644,82 +796,50 @@
         """
         if type(x) in ctx.types: return x
         if isinstance(x, int_types): return ctx.make_mpf(from_int(x))
         if isinstance(x, float): return ctx.make_mpf(from_float(x))
         if isinstance(x, complex):
             return ctx.make_mpc((from_float(x.real), from_float(x.imag)))
         if type(x).__module__ == 'numpy': return ctx.npconvert(x)
-        if isinstance(x, numbers.Rational): # e.g. Fraction
-            try: x = rational.mpq(int(x.numerator), int(x.denominator))
-            except: pass
         prec, rounding = ctx._prec_rounding
-        if isinstance(x, rational.mpq):
-            p, q = x._mpq_
+        if isinstance(x, numbers.Rational):
+            p, q = x.numerator, x.denominator
             return ctx.make_mpf(from_rational(p, q, prec))
-        if strings and isinstance(x, basestring):
+        if strings and isinstance(x, str):
             try:
                 _mpf_ = from_str(x, prec, rounding)
                 return ctx.make_mpf(_mpf_)
             except ValueError:
                 pass
         if hasattr(x, '_mpf_'): return ctx.make_mpf(x._mpf_)
         if hasattr(x, '_mpc_'): return ctx.make_mpc(x._mpc_)
         if hasattr(x, '_mpmath_'):
             return ctx.convert(x._mpmath_(prec, rounding))
         if type(x).__module__ == 'decimal':
-            try: return ctx.make_mpf(from_Decimal(x, prec, rounding))
-            except: pass
+            return ctx.make_mpf(from_Decimal(x, prec, rounding))
         return ctx._convert_fallback(x, strings)
 
     def npconvert(ctx, x):
         """
         Converts *x* to an ``mpf`` or ``mpc``. *x* should be a numpy
         scalar.
         """
         import numpy as np
         if isinstance(x, np.integer): return ctx.make_mpf(from_int(int(x)))
         if isinstance(x, np.floating): return ctx.make_mpf(from_npfloat(x))
         if isinstance(x, np.complexfloating):
             return ctx.make_mpc((from_npfloat(x.real), from_npfloat(x.imag)))
         raise TypeError("cannot create mpf from " + repr(x))
 
-    def isnan(ctx, x):
-        """
-        Return *True* if *x* is a NaN (not-a-number), or for a complex
-        number, whether either the real or complex part is NaN;
-        otherwise return *False*::
-
-            >>> from mpmath import *
-            >>> isnan(3.14)
-            False
-            >>> isnan(nan)
-            True
-            >>> isnan(mpc(3.14,2.72))
-            False
-            >>> isnan(mpc(3.14,nan))
-            True
-
-        """
-        if hasattr(x, "_mpf_"):
-            return x._mpf_ == fnan
-        if hasattr(x, "_mpc_"):
-            return fnan in x._mpc_
-        if isinstance(x, int_types) or isinstance(x, rational.mpq):
-            return False
-        x = ctx.convert(x)
-        if hasattr(x, '_mpf_') or hasattr(x, '_mpc_'):
-            return ctx.isnan(x)
-        raise TypeError("isnan() needs a number as input")
-
     def isinf(ctx, x):
         """
         Return *True* if the absolute value of *x* is infinite;
         otherwise return *False*::
 
-            >>> from mpmath import *
+            >>> from mpmath import isinf, inf, mpc
             >>> isinf(inf)
             True
             >>> isinf(-inf)
             True
             >>> isinf(3)
             False
             >>> isinf(3+4j)
@@ -731,30 +851,28 @@
 
         """
         if hasattr(x, "_mpf_"):
             return x._mpf_ in (finf, fninf)
         if hasattr(x, "_mpc_"):
             re, im = x._mpc_
             return re in (finf, fninf) or im in (finf, fninf)
-        if isinstance(x, int_types) or isinstance(x, rational.mpq):
+        if isinstance(x, int_types) or isinstance(x, MPQ):
             return False
         x = ctx.convert(x)
-        if hasattr(x, '_mpf_') or hasattr(x, '_mpc_'):
-            return ctx.isinf(x)
-        raise TypeError("isinf() needs a number as input")
+        return ctx.isinf(x)
 
     def isnormal(ctx, x):
         """
         Determine whether *x* is "normal" in the sense of floating-point
         representation; that is, return *False* if *x* is zero, an
         infinity or NaN; otherwise return *True*. By extension, a
         complex number *x* is considered "normal" if its magnitude is
         normal::
 
-            >>> from mpmath import *
+            >>> from mpmath import isnormal, inf, nan, mpc
             >>> isnormal(3)
             True
             >>> isnormal(0)
             False
             >>> isnormal(inf); isnormal(-inf); isnormal(nan)
             False
             False
@@ -771,27 +889,25 @@
         if hasattr(x, "_mpc_"):
             re, im = x._mpc_
             re_normal = bool(re[1])
             im_normal = bool(im[1])
             if re == fzero: return im_normal
             if im == fzero: return re_normal
             return re_normal and im_normal
-        if isinstance(x, int_types) or isinstance(x, rational.mpq):
+        if isinstance(x, int_types) or isinstance(x, MPQ):
             return bool(x)
         x = ctx.convert(x)
-        if hasattr(x, '_mpf_') or hasattr(x, '_mpc_'):
-            return ctx.isnormal(x)
-        raise TypeError("isnormal() needs a number as input")
+        return ctx.isnormal(x)
 
     def isint(ctx, x, gaussian=False):
         """
         Return *True* if *x* is integer-valued; otherwise return
         *False*::
 
-            >>> from mpmath import *
+            >>> from mpmath import isint, mpf, inf
             >>> isint(3)
             True
             >>> isint(mpf(3))
             True
             >>> isint(3.2)
             False
             >>> isint(inf)
@@ -817,32 +933,29 @@
             rsign, rman, rexp, rbc = re
             isign, iman, iexp, ibc = im
             re_isint = (rman and rexp >= 0) or re == fzero
             if gaussian:
                 im_isint = (iman and iexp >= 0) or im == fzero
                 return re_isint and im_isint
             return re_isint and im == fzero
-        if isinstance(x, rational.mpq):
-            p, q = x._mpq_
+        if isinstance(x, MPQ):
+            p, q = x.numerator, x.denominator
             return p % q == 0
         x = ctx.convert(x)
-        if hasattr(x, '_mpf_') or hasattr(x, '_mpc_'):
-            return ctx.isint(x, gaussian)
-        raise TypeError("isint() needs a number as input")
+        return ctx.isint(x, gaussian)
 
     def fsum(ctx, terms, absolute=False, squared=False):
         """
         Calculates a sum containing a finite number of terms (for infinite
         series, see :func:`~mpmath.nsum`). The terms will be converted to
         mpmath numbers. For len(terms) > 2, this function is generally
         faster and produces more accurate results than the builtin
         Python function :func:`sum`.
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fsum
             >>> fsum([1, 2, 0.5, 7])
             mpf('10.5')
 
         With squared=True each term is squared, and with absolute=True
         the absolute value of each term is used.
         """
         prec, rnd = ctx._prec_rounding
@@ -906,16 +1019,15 @@
 
         .. math ::
 
             \sum_{k=0} A_k \overline{B_k}
 
         **Examples**
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import fdot, j
             >>> A = [2, 1.5, 3]
             >>> B = [1, -1, 2]
             >>> fdot(A, B)
             mpf('6.5')
             >>> list(zip(A, B))
             [(2, 1), (1.5, -1), (3, 2)]
             >>> fdot(_)
@@ -1038,49 +1150,45 @@
             v = x._mpf_
         else:
             if type(x) in int_types:
                 return int(x), 'Z'
             p = None
             if isinstance(x, tuple):
                 p, q = x
-            elif hasattr(x, '_mpq_'):
-                p, q = x._mpq_
-            elif isinstance(x, basestring) and '/' in x:
+            elif isinstance(x, str) and '/' in x:
                 p, q = x.split('/')
                 p = int(p)
                 q = int(q)
             if p is not None:
                 if not p % q:
                     return p // q, 'Z'
-                return ctx.mpq(p,q), 'Q'
+                return MPQ(p,q), 'Q'
             x = ctx.convert(x)
             if hasattr(x, "_mpc_"):
                 v, im = x._mpc_
                 if im != fzero:
                     return x, 'C'
             elif hasattr(x, "_mpf_"):
                 v = x._mpf_
             else:
-                return x, 'U'
+                raise NotImplementedError
         sign, man, exp, bc = v
         if man:
             if exp >= -4:
                 if sign:
                     man = -man
                 if exp >= 0:
                     return int(man) << exp, 'Z'
-                if exp >= -4:
-                    p, q = int(man), (1<<(-exp))
-                    return ctx.mpq(p,q), 'Q'
+                p, q = int(man), (1<<(-exp))
+                return MPQ(p,q), 'Q'
             x = ctx.make_mpf(v)
             return x, 'R'
-        elif not exp:
+        if not exp:
             return 0, 'Z'
-        else:
-            return x, 'U'
+        raise NotImplementedError
 
     def _mpf_mag(ctx, x):
         sign, man, exp, bc = x
         if man:
             return exp+bc
         if x == fzero:
             return ctx.ninf
@@ -1093,57 +1201,48 @@
         Quick logarithmic magnitude estimate of a number. Returns an
         integer or infinity `m` such that `|x| <= 2^m`. It is not
         guaranteed that `m` is an optimal bound, but it will never
         be too large by more than 2 (and probably not more than 1).
 
         **Examples**
 
-            >>> from mpmath import *
+            >>> from mpmath import mp, mag, ceil, mpf, log, inf, nan
             >>> mp.pretty = True
             >>> mag(10), mag(10.0), mag(mpf(10)), int(ceil(log(10,2)))
             (4, 4, 4, 4)
             >>> mag(10j), mag(10+10j)
             (4, 5)
             >>> mag(0.01), int(ceil(log(0.01,2)))
             (-6, -6)
             >>> mag(0), mag(inf), mag(-inf), mag(nan)
             (-inf, +inf, +inf, nan)
 
         """
         if hasattr(x, "_mpf_"):
             return ctx._mpf_mag(x._mpf_)
-        elif hasattr(x, "_mpc_"):
+        if hasattr(x, "_mpc_"):
             r, i = x._mpc_
             if r == fzero:
                 return ctx._mpf_mag(i)
             if i == fzero:
                 return ctx._mpf_mag(r)
             return 1+max(ctx._mpf_mag(r), ctx._mpf_mag(i))
-        elif isinstance(x, int_types):
+        if isinstance(x, int_types):
             if x:
-                return bitcount(abs(x))
+                return x.bit_length()
             return ctx.ninf
-        elif isinstance(x, rational.mpq):
-            p, q = x._mpq_
+        if isinstance(x, MPQ):
+            p, q = x.numerator, x.denominator
             if p:
-                return 1 + bitcount(abs(p)) - bitcount(q)
+                return 1 + p.bit_length() - q.bit_length()
             return ctx.ninf
-        else:
-            x = ctx.convert(x)
-            if hasattr(x, "_mpf_") or hasattr(x, "_mpc_"):
-                return ctx.mag(x)
-            else:
-                raise TypeError("requires an mpf/mpc")
+        x = ctx.convert(x)
+        return ctx.mag(x)
 
 
 # Register with "numbers" ABC
-#     We do not subclass, hence we do not use the @abstractmethod checks. While
-#     this is less invasive it may turn out that we do not actually support
-#     parts of the expected interfaces.  See
-#     http://docs.python.org/2/library/numbers.html for list of abstract
-#     methods.
-try:
-    import numbers
-    numbers.Complex.register(_mpc)
-    numbers.Real.register(_mpf)
-except ImportError:
-    pass
+#   We do not subclass, hence we do not use the @abstractmethod checks. While
+#   this is less invasive it may turn out that we do not actually support
+#   parts of the expected interfaces.  See
+#   https://docs.python.org/3/library/numbers.html for list of abstract methods.
+numbers.Complex.register(_mpc)
+numbers.Real.register(_mpf)
```

### Comparing `mpmath-1.3.0/mpmath/function_docs.py` & `mpmath-1.4.0a0/mpmath/function_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 pi = r"""
 `\pi`, roughly equal to 3.141592654, represents the area of the unit
 circle, the half-period of trigonometric functions, and many other
 things in mathematics.
 
 Mpmath can evaluate `\pi` to arbitrary precision::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, pi, sin, sinpi
     >>> mp.dps = 50; mp.pretty = True
     >>> +pi
     3.1415926535897932384626433832795028841971693993751
 
 This shows digits 99991-100000 of `\pi` (the last digit is actually
 a 4 when the decimal expansion is truncated, but here the nearest
 rounding is used)::
@@ -51,15 +51,15 @@
 """
 
 degree = r"""
 Represents one degree of angle, `1^{\circ} = \pi/180`, or
 about 0.01745329. This constant may be evaluated to arbitrary
 precision::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, degree, sin
     >>> mp.dps = 50; mp.pretty = True
     >>> +degree
     0.017453292519943295769236907684886127134428718885417
 
 The :data:`degree` object is convenient for conversion
 to radians::
 
@@ -72,15 +72,15 @@
 e = r"""
 The transcendental number `e` = 2.718281828... is the base of the
 natural logarithm (:func:`~mpmath.ln`) and of the exponential function
 (:func:`~mpmath.exp`).
 
 Mpmath can be evaluate `e` to arbitrary precision::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, e
     >>> mp.dps = 50; mp.pretty = True
     >>> +e
     2.7182818284590452353602874713526624977572470937
 
 This shows digits 99991-100000 of `e` (the last digit is actually
 a 5 when the decimal expansion is truncated, but here the nearest
 rounding is used)::
@@ -102,15 +102,15 @@
 """
 
 phi = r"""
 Represents the golden ratio `\phi = (1+\sqrt 5)/2`,
 approximately equal to 1.6180339887. To high precision,
 its value is::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, phi, sqrt, findroot, fib, inf, limit
     >>> mp.dps = 50; mp.pretty = True
     >>> +phi
     1.6180339887498948482045868343656381177203091798058
 
 Formulas for the golden ratio include the following::
 
     >>> (1+sqrt(5))/2
@@ -131,15 +131,16 @@
     \gamma = \lim_{n\to\infty} H_n - \log n
 
 where `H_n = 1 + \frac{1}{2} + \ldots + \frac{1}{n}` is a harmonic
 number (see :func:`~mpmath.harmonic`).
 
 Evaluation of `\gamma` is supported at arbitrary precision::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, euler, harmonic, limit, log, inf, exp,
+    ...                     zeta, gamma, nsum, diff, nprod)
     >>> mp.dps = 50; mp.pretty = True
     >>> +euler
     0.57721566490153286060651209008240243104215933593992
 
 We can also compute `\gamma` directly from the definition,
 although this is less efficient::
 
@@ -192,15 +193,16 @@
 
 .. math ::
 
     K = \sum_{k=0}^{\infty} \frac{(-1)^k}{(2k+1)^2}.
 
 Mpmath can evaluate it to arbitrary precision::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, catalan, nsum, inf, quad, log, atan,
+    ...                     ellipk, pi, zeta)
     >>> mp.dps = 50; mp.pretty = True
     >>> +catalan
     0.91596559417721901505460351493238411077414937428167
 
 One can also compute `K` directly from the definition, although
 this is significantly less efficient::
 
@@ -237,15 +239,15 @@
 """
 
 khinchin = r"""
 Khinchin's constant `K` = 2.68542... is a number that
 appears in the theory of continued fractions. Mpmath can evaluate
 it to arbitrary precision::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, khinchin, log, quad, sincpi, exp, nsum, mpf
     >>> mp.dps = 50; mp.pretty = True
     >>> +khinchin
     2.6854520010653064453097148354817956938203822939945
 
 An integral representation is::
 
     >>> I = quad(lambda x: log((1-x**2)/sincpi(x))/x/(1+x), [0, 1])
@@ -269,15 +271,15 @@
 
 The constant is defined  as `A = \exp(1/12-\zeta'(-1))` where
 `\zeta'(s)` denotes the derivative of the Riemann zeta function
 (see :func:`~mpmath.zeta`).
 
 Mpmath can evaluate Glaisher's constant to arbitrary precision:
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, glaisher, quad, log, gamma, pi, mpf, zeta
     >>> mp.dps = 50; mp.pretty = True
     >>> +glaisher
     1.282427129100622636875342568869791727767688927325
 
 We can verify that the value computed by :data:`glaisher` is
 correct using mpmath's facilities for numerical
 differentiation and arbitrary evaluation of the zeta function:
@@ -310,15 +312,15 @@
 .. math ::
 
     \zeta(3) = \sum_{k=1}^\infty\frac{1}{k^3}.
 
 The calculation is based on an efficient hypergeometric
 series. To 50 decimal places, the value is given by::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, apery, zeta, psi, nsum, inf, exp, pi
     >>> mp.dps = 50; mp.pretty = True
     >>> +apery
     1.2020569031595942853997381615114499907649862923405
 
 Other ways to evaluate Apery's constant using mpmath
 include::
 
@@ -350,15 +352,15 @@
 
 Here `p_k` denotes the `k`-th prime number. Other names for this
 constant include the Hadamard-de la Vallee-Poussin constant or
 the prime reciprocal constant.
 
 The following gives the Mertens constant to 50 digits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, mertens
     >>> mp.dps = 50; mp.pretty = True
     >>> +mertens
     0.2614972128476427837554268386086958590515666482612
 
 References:
 http://mathworld.wolfram.com/MertensConstant.html
 """
@@ -376,15 +378,15 @@
 
 .. math ::
 
     C_2 = \prod_{p\ge3} \frac{p(p-2)}{(p-1)^2} \approx 0.66016
 
 Computing `C_2` to 50 digits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, twinprime
     >>> mp.dps = 50; mp.pretty = True
     >>> +twinprime
     0.66016181584686957392781211001455577843262336028473
 
 References:
 http://mathworld.wolfram.com/TwinPrimesConstant.html
 """
@@ -403,16 +405,16 @@
 For all mpmath numbers ``x``, calling ``sqrt(x)`` is equivalent to
 performing ``x**0.5``.
 
 **Examples**
 
 Basic examples and limits::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, sqrt, inf, iv
+    >>> mp.pretty = True
     >>> sqrt(10)
     3.16227766016838
     >>> sqrt(100)
     10.0
     >>> sqrt(-4)
     (0.0 + 2.0j)
     >>> sqrt(1+1j)
@@ -423,33 +425,32 @@
 Square root evaluation is fast at huge precision::
 
     >>> mp.dps = 50000
     >>> a = sqrt(3)
     >>> str(a)[-10:]
     '9329332815'
 
-:func:`mpmath.iv.sqrt` supports interval arguments::
+``mpmath.iv.sqrt()`` supports interval arguments::
 
-    >>> iv.dps = 15; iv.pretty = True
+    >>> iv.pretty = True
     >>> iv.sqrt([16,100])
     [4.0, 10.0]
     >>> iv.sqrt(2)
     [1.4142135623730949234, 1.4142135623730951455]
     >>> iv.sqrt(2) ** 2
     [1.9999999999999995559, 2.0000000000000004441]
 
 """
 
 cbrt = r"""
 ``cbrt(x)`` computes the cube root of `x`, `x^{1/3}`. This
 function is faster and more accurate than raising to a floating-point
 fraction::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import mpf, cbrt, mp
     >>> 125**(mpf(1)/3)
     mpf('4.9999999999999991')
     >>> cbrt(125)
     mpf('5.0')
 
 Every nonzero complex number has three cube roots. This function
 returns the cube root defined by `\exp(\log(x)/3)` where the
@@ -474,15 +475,16 @@
 
     \exp(x+yi) = e^x (\cos y + i \sin y).
 
 **Basic examples**
 
 Some values of the exponential function::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, exp, inf, iv, pi, j, chop, nprint, taylor,
+    ...                     diff, quad, limit, odefun, fac, nsum, cosh, sinh)
     >>> mp.dps = 25; mp.pretty = True
     >>> exp(0)
     1.0
     >>> exp(1)
     2.718281828459045235360287
     >>> exp(-1)
     0.3678794411714423215955238
@@ -495,27 +497,27 @@
 
     >>> exp(10000)
     8.806818225662921587261496e+4342
     >>> exp(-10000)
     1.135483865314736098540939e-4343
 
 Evaluation is supported for interval arguments via
-:func:`mpmath.iv.exp`::
+``mpmath.iv.exp()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.exp([-inf,0])
     [0.0, 1.0]
     >>> iv.exp([0,1])
     [1.0, 2.71828182845904523536028749558]
 
 The exponential function can be evaluated efficiently to arbitrary
 precision::
 
     >>> mp.dps = 10000
-    >>> exp(pi)  #doctest: +ELLIPSIS
+    >>> exp(pi)
     23.140692632779269005729...8984304016040616
 
 **Functional properties**
 
 Numerical verification of Euler's identity for the complex
 exponential function::
 
@@ -552,15 +554,15 @@
     23.1406926327793
 """
 
 cosh = r"""
 Computes the hyperbolic cosine of `x`,
 `\cosh(x) = (e^x + e^{-x})/2`. Values and limits include::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, cosh, inf, chop, taylor, nprint, cos
     >>> mp.dps = 25; mp.pretty = True
     >>> cosh(0)
     1.0
     >>> cosh(1)
     1.543080634815243778477906
     >>> cosh(-inf), cosh(+inf)
     (+inf, +inf)
@@ -582,15 +584,15 @@
     (-3.724545504915322565473971 + 0.5118225699873846088344638j)
 """
 
 sinh = r"""
 Computes the hyperbolic sine of `x`,
 `\sinh(x) = (e^x - e^{-x})/2`. Values and limits include::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, sinh, inf, chop, taylor, nprint, j
     >>> mp.dps = 25; mp.pretty = True
     >>> sinh(0)
     0.0
     >>> sinh(1)
     1.175201193643801456882382
     >>> sinh(-inf), sinh(+inf)
     (-inf, +inf)
@@ -611,15 +613,15 @@
     (-3.590564589985779952012565 + 0.5309210862485198052670401j)
 """
 
 tanh = r"""
 Computes the hyperbolic tangent of `x`,
 `\tanh(x) = \sinh(x)/\cosh(x)`. Values and limits include::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, tanh, inf, nprint, chop, taylor, j
     >>> mp.dps = 25; mp.pretty = True
     >>> tanh(0)
     0.0
     >>> tanh(1)
     0.7615941559557648881194583
     >>> tanh(-inf), tanh(inf)
     (-1.0, 1.0)
@@ -640,109 +642,109 @@
     >>> j*tan(3-2j)
     (0.9653858790221331242784803 - 0.009884375038322493720314034j)
 """
 
 cos = r"""
 Computes the cosine of `x`, `\cos(x)`.
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, cos, pi, inf, nprint, chop, taylor, iv
     >>> mp.dps = 25; mp.pretty = True
     >>> cos(pi/3)
     0.5
     >>> cos(100000001)
     -0.9802850113244713353133243
     >>> cos(2+3j)
     (-4.189625690968807230132555 - 9.109227893755336597979197j)
     >>> cos(inf)
     nan
     >>> nprint(chop(taylor(cos, 0, 6)))
     [1.0, 0.0, -0.5, 0.0, 0.0416667, 0.0, -0.00138889]
 
-Intervals are supported via :func:`mpmath.iv.cos`::
+Intervals are supported via ``mpmath.iv.cos()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.cos([0,1])
     [0.540302305868139717400936602301, 1.0]
     >>> iv.cos([0,2])
     [-0.41614683654714238699756823214, 1.0]
 """
 
 sin = r"""
 Computes the sine of `x`, `\sin(x)`.
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, sin, inf, nprint, chop, taylor, iv
     >>> mp.dps = 25; mp.pretty = True
     >>> sin(pi/3)
     0.8660254037844386467637232
     >>> sin(100000001)
     0.1975887055794968911438743
     >>> sin(2+3j)
     (9.1544991469114295734673 - 4.168906959966564350754813j)
     >>> sin(inf)
     nan
     >>> nprint(chop(taylor(sin, 0, 6)))
     [0.0, 1.0, 0.0, -0.166667, 0.0, 0.00833333, 0.0]
 
-Intervals are supported via :func:`mpmath.iv.sin`::
+Intervals are supported via ``mpmath.iv.sin()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.sin([0,1])
     [0.0, 0.841470984807896506652502331201]
     >>> iv.sin([0,2])
     [0.0, 1.0]
 """
 
 tan = r"""
 Computes the tangent of `x`, `\tan(x) = \frac{\sin(x)}{\cos(x)}`.
 The tangent function is singular at `x = (n+1/2)\pi`, but
 ``tan(x)`` always returns a finite result since `(n+1/2)\pi`
 cannot be represented exactly using floating-point arithmetic.
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, iv, tan, pi, inf, nprint, chop, taylor
     >>> mp.dps = 25; mp.pretty = True
     >>> tan(pi/3)
     1.732050807568877293527446
     >>> tan(100000001)
     -0.2015625081449864533091058
     >>> tan(2+3j)
     (-0.003764025641504248292751221 + 1.003238627353609801446359j)
     >>> tan(inf)
     nan
     >>> nprint(chop(taylor(tan, 0, 6)))
     [0.0, 1.0, 0.0, 0.333333, 0.0, 0.133333, 0.0]
 
-Intervals are supported via :func:`mpmath.iv.tan`::
+Intervals are supported via ``mpmath.iv.tan()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.tan([0,1])
     [0.0, 1.55740772465490223050697482944]
     >>> iv.tan([0,2])  # Interval includes a singularity
     [-inf, +inf]
 """
 
 sec = r"""
 Computes the secant of `x`, `\mathrm{sec}(x) = \frac{1}{\cos(x)}`.
 The secant function is singular at `x = (n+1/2)\pi`, but
 ``sec(x)`` always returns a finite result since `(n+1/2)\pi`
 cannot be represented exactly using floating-point arithmetic.
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, pi, sec, inf, nprint, chop, taylor, iv
     >>> mp.dps = 25; mp.pretty = True
     >>> sec(pi/3)
     2.0
     >>> sec(10000001)
     -1.184723164360392819100265
     >>> sec(2+3j)
     (-0.04167496441114427004834991 + 0.0906111371962375965296612j)
     >>> sec(inf)
     nan
     >>> nprint(chop(taylor(sec, 0, 6)))
     [1.0, 0.0, 0.5, 0.0, 0.208333, 0.0, 0.0847222]
 
-Intervals are supported via :func:`mpmath.iv.sec`::
+Intervals are supported via ``mpmath.iv.sec()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.sec([0,1])
     [1.0, 1.85081571768092561791175326276]
     >>> iv.sec([0,2])  # Interval includes a singularity
     [-inf, +inf]
 """
@@ -750,26 +752,26 @@
 csc = r"""
 Computes the cosecant of `x`, `\mathrm{csc}(x) = \frac{1}{\sin(x)}`.
 This cosecant function is singular at `x = n \pi`, but with the
 exception of the point `x = 0`, ``csc(x)`` returns a finite result
 since `n \pi` cannot be represented exactly using floating-point
 arithmetic.
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, csc, inf, iv, pi
     >>> mp.dps = 25; mp.pretty = True
     >>> csc(pi/3)
     1.154700538379251529018298
     >>> csc(10000001)
     -1.864910497503629858938891
     >>> csc(2+3j)
     (0.09047320975320743980579048 + 0.04120098628857412646300981j)
     >>> csc(inf)
     nan
 
-Intervals are supported via :func:`mpmath.iv.csc`::
+Intervals are supported via ``mpmath.iv.csc()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.csc([0,1])  # Interval includes a singularity
     [1.18839510577812121626159943988, +inf]
     >>> iv.csc([0,2])
     [1.0, +inf]
 """
@@ -778,26 +780,26 @@
 Computes the cotangent of `x`,
 `\mathrm{cot}(x) = \frac{1}{\tan(x)} = \frac{\cos(x)}{\sin(x)}`.
 This cotangent function is singular at `x = n \pi`, but with the
 exception of the point `x = 0`, ``cot(x)`` returns a finite result
 since `n \pi` cannot be represented exactly using floating-point
 arithmetic.
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, cot, pi, inf, iv
     >>> mp.dps = 25; mp.pretty = True
     >>> cot(pi/3)
     0.5773502691896257645091488
     >>> cot(10000001)
     1.574131876209625656003562
     >>> cot(2+3j)
     (-0.003739710376336956660117409 - 0.9967577965693583104609688j)
     >>> cot(inf)
     nan
 
-Intervals are supported via :func:`mpmath.iv.cot`::
+Intervals are supported via ``mpmath.iv.cot()``::
 
     >>> iv.dps = 25; iv.pretty = True
     >>> iv.cot([0,1])  # Interval includes a singularity
     [0.642092615934330703006419974862, +inf]
     >>> iv.cot([1,2])
     [-inf, +inf]
 """
@@ -807,15 +809,15 @@
 Since `-1 \le \cos(x) \le 1` for real `x`, the inverse
 cosine is real-valued only for `-1 \le x \le 1`. On this interval,
 :func:`~mpmath.acos` is defined to be a monotonically decreasing
 function assuming values between `+\pi` and `0`.
 
 Basic values are::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, acos, nprint, chop, taylort, cos
     >>> mp.dps = 25; mp.pretty = True
     >>> acos(-1)
     3.141592653589793238462643
     >>> acos(0)
     1.570796326794896619231322
     >>> acos(1)
     0.0
@@ -852,15 +854,15 @@
 Since `-1 \le \sin(x) \le 1` for real `x`, the inverse
 sine is real-valued only for `-1 \le x \le 1`.
 On this interval, it is defined to be a monotonically increasing
 function assuming values between `-\pi/2` and `\pi/2`.
 
 Basic values are::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, asin, nprint, chop, taylor, sin
     >>> mp.dps = 25; mp.pretty = True
     >>> asin(-1)
     -1.570796326794896619231322
     >>> asin(0)
     0.0
     >>> asin(1)
     1.570796326794896619231322
@@ -895,15 +897,15 @@
 atan = r"""
 Computes the inverse tangent or arctangent of `x`, `\tan^{-1}(x)`.
 This is a real-valued function for all real `x`, with range
 `(-\pi/2, \pi/2)`.
 
 Basic values are::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, inf, atan, nprint, chop
     >>> mp.dps = 25; mp.pretty = True
     >>> atan(-inf)
     -1.570796326794896619231322
     >>> atan(-1)
     -0.7853981633974483096156609
     >>> atan(0)
     0.0
@@ -988,28 +990,28 @@
 
 
 
 sinpi = r"""
 Computes `\sin(\pi x)`, more accurately than the expression
 ``sin(pi*x)``::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, sinpi, pi, sin
+    >>> mp.pretty = True
     >>> sinpi(10**10), sin(pi*(10**10))
     (0.0, -2.23936276195592e-6)
     >>> sinpi(10**10+0.5), sin(pi*(10**10+0.5))
     (1.0, 0.999999999998721)
 """
 
 cospi = r"""
 Computes `\cos(\pi x)`, more accurately than the expression
 ``cos(pi*x)``::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, cospi, cos, pi
+    >>> mp.pretty = True
     >>> cospi(10**10), cos(pi*(10**10))
     (1.0, 0.999999999997493)
     >>> cospi(10**10+0.5), cos(pi*(10**10+0.5))
     (0.0, 1.59960492420134e-6)
 """
 
 sinc = r"""
@@ -1022,16 +1024,16 @@
         1,         & \mbox{if } x = 0.
     \end{cases}
 
 See :func:`~mpmath.sincpi` for the normalized sinc function.
 
 Simple values and limits include::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, sinc, inf, quad, si
+    >>> mp.pretty = True
     >>> sinc(0)
     1.0
     >>> sinc(1)
     0.841470984807897
     >>> sinc(inf)
     0.0
 
@@ -1055,30 +1057,30 @@
 
 Equivalently, we have
 `\mathrm{sinc}_{\pi}(x) = \mathrm{sinc}(\pi x)`.
 
 The normalization entails that the function integrates
 to unity over the entire real line::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, inf, quadosc, sincpi
+    >>> mp.pretty = True
     >>> quadosc(sincpi, [-inf, inf], period=2.0)
     1.0
 
 Like, :func:`~mpmath.sinpi`, :func:`~mpmath.sincpi` is evaluated accurately
 at its roots::
 
     >>> sincpi(10)
     0.0
 """
 
 expj = r"""
 Convenience function for computing `e^{ix}`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, expj, j
     >>> mp.dps = 25; mp.pretty = True
     >>> expj(0)
     (1.0 + 0.0j)
     >>> expj(-1)
     (0.5403023058681397174009366 - 0.8414709848078965066525023j)
     >>> expj(j)
     (0.3678794411714423215955238 + 0.0j)
@@ -1087,15 +1089,15 @@
 """
 
 expjpi = r"""
 Convenience function for computing `e^{i \pi x}`.
 Evaluation is accurate near zeros (see also :func:`~mpmath.cospi`,
 :func:`~mpmath.sinpi`)::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, expjpi, j
     >>> mp.dps = 25; mp.pretty = True
     >>> expjpi(0)
     (1.0 + 0.0j)
     >>> expjpi(1)
     (-1.0 + 0.0j)
     >>> expjpi(0.5)
     (0.0 + 1.0j)
@@ -1107,30 +1109,28 @@
     (-0.04321391826377224977441774 + 0.0j)
 """
 
 floor = r"""
 Computes the floor of `x`, `\lfloor x \rfloor`, defined as
 the largest integer less than or equal to `x`::
 
-    >>> from mpmath import *
-    >>> mp.pretty = False
+    >>> from mpmath import floor
     >>> floor(3.5)
     mpf('3.0')
 
 .. note ::
 
     :func:`~mpmath.floor`, :func:`~mpmath.ceil` and :func:`~mpmath.nint` return a
     floating-point number, not a Python ``int``. If `\lfloor x \rfloor` is
     too large to be represented exactly at the present working precision,
     the result will be rounded, not necessarily in the direction
     implied by the mathematical definition of the function.
 
 To avoid rounding, use *prec=0*::
 
-    >>> mp.dps = 15
     >>> print(int(floor(10**30+1)))
     1000000000000000019884624838656
     >>> print(int(floor(10**30+1, prec=0)))
     1000000000000000000000000000001
 
 The floor function is defined for complex numbers and
 acts on the real and imaginary parts separately::
@@ -1139,16 +1139,15 @@
     mpc(real='3.0', imag='4.0')
 """
 
 ceil = r"""
 Computes the ceiling of `x`, `\lceil x \rceil`, defined as
 the smallest integer greater than or equal to `x`::
 
-    >>> from mpmath import *
-    >>> mp.pretty = False
+    >>> from mpmath import ceil
     >>> ceil(3.5)
     mpf('4.0')
 
 The ceiling function is defined for complex numbers and
 acts on the real and imaginary parts separately::
 
     >>> ceil(3.25+4.75j)
@@ -1158,16 +1157,15 @@
 """
 
 nint = r"""
 Evaluates the nearest integer function, `\mathrm{nint}(x)`.
 This gives the nearest integer to `x`; on a tie, it
 gives the nearest even integer::
 
-    >>> from mpmath import *
-    >>> mp.pretty = False
+    >>> from mpmath import nint
     >>> nint(3.2)
     mpf('3.0')
     >>> nint(3.8)
     mpf('4.0')
     >>> nint(3.5)
     mpf('4.0')
     >>> nint(4.5)
@@ -1184,16 +1182,15 @@
 
 frac = r"""
 Gives the fractional part of `x`, defined as
 `\mathrm{frac}(x) = x - \lfloor x \rfloor` (see :func:`~mpmath.floor`).
 In effect, this computes `x` modulo 1, or `x+n` where
 `n \in \mathbb{Z}` is such that `x+n \in [0,1)`::
 
-    >>> from mpmath import *
-    >>> mp.pretty = False
+    >>> from mpmath import frac, nprint, fourier, pi
     >>> frac(1.25)
     mpf('0.25')
     >>> frac(3)
     mpf('0.0')
     >>> frac(-1.25)
     mpf('0.75')
 
@@ -1203,15 +1200,14 @@
     >>> frac(2.25+3.75j)
     mpc(real='0.25', imag='0.75')
 
 Plotted, the fractional part function gives a sawtooth
 wave. The Fourier series coefficients have a simple
 form::
 
-    >>> mp.dps = 15
     >>> nprint(fourier(lambda x: frac(x)-0.5, [0,1], 4))
     ([0.0, 0.0, 0.0, 0.0, 0.0], [0.0, -0.31831, -0.159155, -0.106103, -0.0795775])
     >>> nprint([-1/(pi*k) for k in range(1,5)])
     [-0.31831, -0.159155, -0.106103, -0.0795775]
 
 .. note::
 
@@ -1222,39 +1218,38 @@
 
 """
 
 sign = r"""
 Returns the sign of `x`, defined as `\mathrm{sign}(x) = x / |x|`
 (with the special case `\mathrm{sign}(0) = 0`)::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import sign, mp, j
     >>> sign(10)
     mpf('1.0')
     >>> sign(-10)
     mpf('-1.0')
     >>> sign(0)
     mpf('0.0')
 
 Note that the sign function is also defined for complex numbers,
 for which it gives the projection onto the unit circle::
 
-    >>> mp.dps = 15; mp.pretty = True
+    >>> mp.pretty = True
     >>> sign(1+j)
     (0.707106781186547 + 0.707106781186547j)
 
 """
 
 arg = r"""
 Computes the complex argument (phase) of `x`, defined as the
 signed angle between the positive real axis and `x` in the
 complex plane::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import arg, mp
+    >>> mp.pretty = True
     >>> arg(3)
     0.0
     >>> arg(3+3j)
     0.785398163397448
     >>> arg(3j)
     1.5707963267949
     >>> arg(-3)
@@ -1270,92 +1265,88 @@
 """
 
 fabs = r"""
 Returns the absolute value of `x`, `|x|`. Unlike :func:`abs`,
 :func:`~mpmath.fabs` converts non-mpmath numbers (such as ``int``)
 into mpmath numbers::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import fabs
     >>> fabs(3)
     mpf('3.0')
     >>> fabs(-3)
     mpf('3.0')
     >>> fabs(3+4j)
     mpf('5.0')
 """
 
 re = r"""
 Returns the real part of `x`, `\Re(x)`. :func:`~mpmath.re`
 converts a non-mpmath number to an mpmath number::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import re
     >>> re(3)
     mpf('3.0')
     >>> re(-1+4j)
     mpf('-1.0')
 """
 
 im = r"""
 Returns the imaginary part of `x`, `\Im(x)`. :func:`~mpmath.im`
 converts a non-mpmath number to an mpmath number::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import im
     >>> im(3)
     mpf('0.0')
     >>> im(-1+4j)
     mpf('4.0')
 """
 
 conj = r"""
 Returns the complex conjugate of `x`, `\overline{x}`. Unlike
 ``x.conjugate()``, :func:`~mpmath.im` converts `x` to a mpmath number::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import conj
     >>> conj(3)
     mpf('3.0')
     >>> conj(-1+4j)
     mpc(real='-1.0', imag='-4.0')
 """
 
 polar = r"""
 Returns the polar representation of the complex number `z`
 as a pair `(r, \phi)` such that `z = r e^{i \phi}`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import polar, mp
+    >>> mp.pretty = True
     >>> polar(-2)
     (2.0, 3.14159265358979)
     >>> polar(3-4j)
     (5.0, -0.927295218001612)
 """
 
 rect = r"""
 Returns the complex number represented by polar
 coordinates `(r, \phi)`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import rect, mp, pi, chop, sqrt
+    >>> mp.pretty = True
     >>> chop(rect(2, pi))
     -2.0
     >>> rect(sqrt(2), -pi/4)
     (1.0 - 1.0j)
 """
 
 expm1 = r"""
 Computes `e^x - 1`, accurately for small `x`.
 
 Unlike the expression ``exp(x) - 1``, ``expm1(x)`` does not suffer from
 potentially catastrophic cancellation::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, exp, expm1
+    >>> mp.pretty = True
     >>> exp(1e-10)-1; print(expm1(1e-10))
     1.00000008274037e-10
     1.00000000005e-10
     >>> exp(1e-20)-1; print(expm1(1e-20))
     0.0
     1.0e-20
     >>> 1/(exp(1e-20)-1)
@@ -1373,16 +1364,16 @@
     1.0e-10000000
 
 """
 
 log1p = r"""
 Computes `\log(1+x)`, accurately for small `x`.
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, log, log1p
+    >>> mp.pretty = True
     >>> log(1+1e-10); print(mp.log1p(1e-10))
     1.00000008269037e-10
     9.9999999995e-11
     >>> mp.log1p(1e-100j)
     (5.0e-201 + 1.0e-100j)
     >>> mp.log1p(0)
     0.0
@@ -1391,16 +1382,16 @@
 
 
 powm1 = r"""
 Computes `x^y - 1`, accurately when `x^y` is very close to 1.
 
 This avoids potentially catastrophic cancellation::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, power, powm1, j, fadd
+    >>> mp.pretty = True
     >>> power(0.99999995, 1e-10) - 1
     0.0
     >>> powm1(0.99999995, 1e-10)
     -5.00000012791934e-18
 
 Powers exactly equal to 1, and only those powers, yield 0 exactly::
 
@@ -1419,15 +1410,15 @@
     (-1.23370055013617e-2000 + 1.5707963267949e-1000j)
 
 """
 
 root = r"""
 ``root(z, n, k=0)`` computes an `n`-th root of `z`, i.e. returns a number
 `r` that (up to possible approximation error) satisfies `r^n = z`.
-(``nthroot`` is available as an alias for ``root``.)
+(``nthroot()`` is available as an alias for :func:`~mpmath.root`.)
 
 Every complex number `z \ne 0` has `n` distinct `n`-th roots, which are
 equidistant points on a circle with radius `|z|^{1/n}`, centered around the
 origin. A specific root may be selected using the optional index
 `k`. The roots are indexed counterclockwise, starting with `k = 0` for the root
 closest to the positive real half-axis.
 
@@ -1449,23 +1440,22 @@
 Both `k` and `n` should be integers; `k` outside of ``range(n)`` will be
 reduced modulo `n`. If `n` is negative, `x^{-1/n} = 1/x^{1/n}` (or
 the equivalent reciprocal for a non-principal root with `k \ne 0`) is computed.
 
 :func:`~mpmath.root` is implemented to use Newton's method for small
 `n`. At high precision, this makes `x^{1/n}` not much more
 expensive than the regular exponentiation, `x^n`. For very large
-`n`, :func:`~mpmath.nthroot` falls back to use the exponential function.
+`n`, :func:`~mpmath.root` falls back to use the exponential function.
 
 **Examples**
 
-:func:`~mpmath.nthroot`/:func:`~mpmath.root` is faster and more accurate than raising to a
+``nthroot()``/:func:`~mpmath.root` is faster and more accurate than raising to a
 floating-point fraction::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = False
+    >>> from mpmath import root, mpf, nthroot, mp
     >>> 16807 ** (mpf(1)/5)
     mpf('7.0000000000000009')
     >>> root(16807, 5)
     mpf('7.0')
     >>> nthroot(16807, 5)    # Alias
     mpf('7.0')
 
@@ -1534,16 +1524,16 @@
 circle. They are ordered counterclockwise with increasing `k`, starting
 with `\zeta_0 = 1`.
 
 **Examples**
 
 The roots of unity up to `n = 4`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, nprint, unitroots, chop, fsum, nprint
+    >>> mp.pretty = True
     >>> nprint(unitroots(1))
     [1.0]
     >>> nprint(unitroots(2))
     [1.0, -1.0]
     >>> nprint(unitroots(3))
     [1.0, (-0.5 + 0.866025j), (-0.5 - 0.866025j)]
     >>> nprint(unitroots(4))
@@ -1616,16 +1606,16 @@
 `x` is complex. The principal branch of the complex logarithm is
 used, meaning that `\Im(\ln(x)) = -\pi < \arg(x) \le \pi`.
 
 **Examples**
 
 Some basic values and limits::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, log, inf, quad, diff, nprint, taylor, j, pi
+    >>> mp.pretty = True
     >>> log(1)
     0.0
     >>> log(2)
     0.693147180559945
     >>> log(1000,10)
     3.0
     >>> log(4, 16)
@@ -1671,40 +1661,40 @@
 is equivalent to ``log(x, 10)``.
 """
 
 fmod = r"""
 Converts `x` and `y` to mpmath numbers and returns `x \mod y`.
 For mpmath numbers, this is equivalent to ``x % y``.
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, pi, fmod
+    >>> mp.pretty = True
     >>> fmod(100, pi)
     2.61062773871641
 
 You can use :func:`~mpmath.fmod` to compute fractional parts of numbers::
 
     >>> fmod(10.25, 1)
     0.25
 
 """
 
 radians = r"""
 Converts the degree angle `x` to radians::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, radians
+    >>> mp.pretty = True
     >>> radians(60)
     1.0471975511966
 """
 
 degrees = r"""
 Converts the radian angle `x` to a degree angle::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, degrees, pi
+    >>> mp.pretty = True
     >>> degrees(pi/3)
     60.0
 """
 
 atan2 = r"""
 Computes the two-argument arctangent, `\mathrm{atan2}(y, x)`,
 giving the signed angle between the positive `x`-axis and the
@@ -1712,16 +1702,16 @@
 real `x` and `y` only.
 
 The two-argument arctangent essentially computes
 `\mathrm{atan}(y/x)`, but accounts for the signs of both
 `x` and `y` to give the angle for the correct quadrant. The
 following examples illustrate the difference::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, atan2, atan
+    >>> mp.pretty = True
     >>> atan2(1,1), atan(1/1.)
     (0.785398163397448, 0.785398163397448)
     >>> atan2(1,-1), atan(1/-1.)
     (2.35619449019234, -0.785398163397448)
     >>> atan2(-1,1), atan(-1/1.)
     (-0.785398163397448, -0.785398163397448)
     >>> atan2(-1,-1), atan(-1/-1.)
@@ -1742,23 +1732,23 @@
 
   F(z) = \frac{\phi^z - \cos(\pi z) \phi^{-z}}{\sqrt 5}
 
 where `\phi` is the golden ratio. :func:`~mpmath.fibonacci` also uses this
 continuous formula to compute `F(n)` for extremely large `n`, where
 calculating the exact integer would be wasteful.
 
-For convenience, :func:`~mpmath.fib` is available as an alias for
+For convenience, ``fib()`` is available as an alias for
 :func:`~mpmath.fibonacci`.
 
 **Basic examples**
 
 Some small Fibonacci numbers are::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, fibonacci, fib, pi, findroot, nsum, sqrt, inf
+    >>> mp.pretty = True
     >>> for i in range(10):
     ...     print(fibonacci(i))
     ...
     0.0
     1.0
     1.0
     2.0
@@ -1878,15 +1868,15 @@
 Gives the Dirichlet eta function, `\eta(s)`, also known as the
 alternating zeta function. This function is defined in analogy
 with the Riemann zeta function as providing the sum of the
 alternating series
 
 .. math ::
 
-    \eta(s) = \sum_{k=0}^{\infty} \frac{(-1)^k}{k^s}
+    \eta(s) = \sum_{k=1}^{\infty} \frac{(-1)^{k-1}}{k^s}
         = 1-\frac{1}{2^s}+\frac{1}{3^s}-\frac{1}{4^s}+\ldots
 
 The eta function, unlike the Riemann zeta function, is an entire
 function, having a finite value for all complex `s`. The special case
 `\eta(1) = \log(2)` gives the value of the alternating harmonic series.
 
 The alternating zeta function may expressed using the Riemann zeta function
@@ -1894,16 +1884,16 @@
 in terms of the Hurwitz zeta function, for example using
 :func:`~mpmath.dirichlet` (see documentation for that function).
 
 **Examples**
 
 Some special values are::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, altzeta, mpf, pi, inf
+    >>> mp.pretty = True
     >>> altzeta(1)
     0.693147180559945
     >>> altzeta(0)
     0.5
     >>> altzeta(-1)
     0.25
     >>> altzeta(-2)
@@ -1951,16 +1941,16 @@
 `n! = 1 \cdot 2 \cdots (n-1) \cdot n` and more generally the factorial
 is defined for real or complex `x` by `x! = \Gamma(x+1)`.
 
 **Examples**
 
 Basic values and limits::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, fac, sqrt, inf, pi, exp, nsum
+    >>> mp.pretty = True
     >>> for k in range(6):
     ...     print("%s %s" % (k, fac(k)))
     ...
     0 1.0
     1 1.0
     2 2.0
     3 6.0
@@ -1976,15 +1966,15 @@
 
     >>> x = 10**10
     >>> fac(x)
     2.32579620567308e+95657055186
     >>> sqrt(2*pi*x)*(x/e)**x
     2.32579597597705e+95657055186
 
-:func:`~mpmath.fac` supports evaluation for astronomically large values::
+:func:`~mpmath.factorial` supports evaluation for astronomically large values::
 
     >>> fac(10**30)
     6.22311232304258e+29565705518096748172348871081098
 
 Reciprocal factorials appear in the Taylor series of the
 exponential function (among many other contexts)::
 
@@ -2008,16 +1998,16 @@
 for any real or complex `x` with `\Re(x) > 0` and for `\Re(x) < 0`
 by analytic continuation.
 
 **Examples**
 
 Basic values and limits::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, gamma, inf, sqrt, pi, exp, quad
+    >>> mp.pretty = True
     >>> for k in range(1, 6):
     ...     print("%s %s" % (k, gamma(k)))
     ...
     1 1.0
     2 1.0
     3 2.0
     4 6.0
@@ -2085,15 +2075,16 @@
 at `z = 0, -1, -2, \ldots`).
 
 **Examples**
 
 For various rational arguments, the polygamma function reduces to
 a combination of standard mathematical constants::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, psi, euler, catalan, pi, apery, quad, diff,
+    ...                     sqrt, nsum, inf, j, nprint, polyroots)
     >>> mp.dps = 25; mp.pretty = True
     >>> psi(0, 1), -euler
     (-0.5772156649015328606065121, -0.5772156649015328606065121)
     >>> psi(1, '1/4'), pi**2+8*catalan
     (17.19732915450711073927132, 17.19732915450711073927132)
     >>> psi(2, '1/2'), -14*apery
     (-16.82879664423431999559633, -16.82879664423431999559633)
@@ -2169,16 +2160,16 @@
 
 .. math ::
 
     H(n) = 1 + \frac{1}{2} + \frac{1}{3} + \ldots + \frac{1}{n}
 
 The first few harmonic numbers are::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, harmonic, inf, pi, findroot, ceil
+    >>> mp.pretty = True
     >>> for n in range(8):
     ...     print("%s %s" % (n, harmonic(n)))
     ...
     0 0.0
     1 1.0
     2 1.5
     3 1.83333333333333
@@ -2233,20 +2224,23 @@
 bernoulli = r"""
 Computes the nth Bernoulli number, `B_n`, for any integer `n \ge 0`.
 
 The Bernoulli numbers are rational numbers, but this function
 returns a floating-point approximation. To obtain an exact
 fraction, use :func:`~mpmath.bernfrac` instead.
 
+Optional ``plus`` flag (default: False) control the sign choice of
+the `B_1` value (default: `-0.5`).
+
 **Examples**
 
 Numerical values of the first few Bernoulli numbers::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, bernoulli, pi, fac, zeta
+    >>> mp.pretty = True
     >>> for n in range(15):
     ...     print("%s %s" % (n, bernoulli(n)))
     ...
     0 1.0
     1 -0.5
     2 0.166666666666667
     3 0.0
@@ -2287,14 +2281,19 @@
 For small `n` (`n < 3000`) :func:`~mpmath.bernoulli` uses a recurrence
 formula due to Ramanujan. All results in this range are cached,
 so sequential computation of small Bernoulli numbers is
 guaranteed to be fast.
 
 For larger `n`, `B_n` is evaluated in terms of the Riemann zeta
 function.
+
+**References**
+
+1. https://en.wikipedia.org/wiki/Bernoulli_number
+
 """
 
 stieltjes = r"""
 For a nonnegative integer `n`, ``stieltjes(n)`` computes the
 `n`-th Stieltjes constant `\gamma_n`, defined as the
 `n`-th coefficient in the Laurent series expansion of the
 Riemann zeta function around the pole at `s = 1`. That is,
@@ -2309,16 +2308,16 @@
 coefficient `\gamma_n(a)` for the Hurwitz zeta function
 `\zeta(s,a)` (with `\gamma_n = \gamma_n(1)`).
 
 **Examples**
 
 The zeroth Stieltjes constant is just Euler's constant `\gamma`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, stieltjes, extradps, zeta, diff
+    >>> mp.pretty = True
     >>> stieltjes(0)
     0.577215664901533
 
 Some more values are::
 
     >>> stieltjes(1)
     -0.0728158454836767
@@ -2410,16 +2409,16 @@
 * If there are more poles in the denominator, :func:`~mpmath.gammaprod`
   returns 0.
 
 **Examples**
 
 The reciprocal gamma function `1/\Gamma(x)` evaluated at `x = 0`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15
+    >>> from mpmath import mp, gammaprod, limit, gamma
+    >>> mp.pretty = True
     >>> gammaprod([], [0])
     0.0
 
 A limit::
 
     >>> gammaprod([-4], [-3])
     -0.25
@@ -2442,16 +2441,16 @@
 
 **Examples**
 
 For integer and half-integer arguments where all three gamma
 functions are finite, the beta function becomes either rational
 number or a rational multiple of `\pi`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, beta, inf, j, pi, e, quad, sqrt, sin, cos
+    >>> mp.pretty = True
     >>> beta(5, 2)
     0.0333333333333333
     >>> beta(1.5, 2)
     0.266666666666667
     >>> 16*beta(2.5, 1.5)
     3.14159265358979
 
@@ -2521,15 +2520,15 @@
     ``betainc(a,b,0,x2,regularized=True)``.
 
 **Examples**
 
 Verifying that :func:`~mpmath.betainc` computes the integral in the
 definition::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, betainc, quad, identify, chop, pi, e
     >>> mp.dps = 25; mp.pretty = True
     >>> x,y,a,b = 3, 4, 0, 6
     >>> betainc(x, y, a, b)
     -4010.4
     >>> quad(lambda t: t**(x-1) * (1-t)**(y-1), [a, b])
     -4010.4
 
@@ -2578,16 +2577,16 @@
 coefficient is a well-defined function of arbitrary real or
 complex `n` and `k`, via the gamma function.
 
 **Examples**
 
 Generate Pascal's triangle::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, binomial, nprint, exp, taylor, j, chop, quad, pi
+    >>> mp.pretty = True
     >>> for n in range(5):
     ...     nprint([binomial(n,k) for k in range(n+1)])
     ...
     [1.0]
     [1.0, 1.0]
     [1.0, 2.0, 1.0]
     [1.0, 3.0, 3.0, 1.0]
@@ -2636,16 +2635,16 @@
 
 where the rightmost expression is valid for nonintegral `n`.
 
 **Examples**
 
 For integral `n`, the rising factorial is a polynomial::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import rf, mp, nprint, taylor
+    >>> mp.pretty = True
     >>> for n in range(5):
     ...     nprint(taylor(lambda x: rf(x,n), 0, n))
     ...
     [1.0]
     [0.0, 1.0]
     [0.0, 1.0, 1.0]
     [0.0, 2.0, 3.0, 1.0]
@@ -2666,16 +2665,16 @@
 
 where the rightmost expression is valid for nonintegral `n`.
 
 **Examples**
 
 For integral `n`, the falling factorial is a polynomial::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, ff, nprint, taylor
+    >>> mp.pretty = True
     >>> for n in range(5):
     ...     nprint(taylor(lambda x: ff(x,n), 0, n))
     ...
     [1.0]
     [0.0, 1.0]
     [0.0, -1.0, 1.0]
     [0.0, 2.0, -3.0, 1.0]
@@ -2705,16 +2704,17 @@
     x!! = 2^{x/2} \left(\frac{\pi}{2}\right)^{(\cos(\pi x)-1)/4}
           \Gamma\left(\frac{x}{2}+1\right).
 
 **Examples**
 
 The integer sequence of double factorials begins::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, fac2, nprint, mpf, exp, pi, nsum, sqrt, e,
+    ...                     gamma, inf, erf, fac)
+    >>> mp.pretty = True
     >>> nprint([fac2(n) for n in range(10)])
     [1.0, 1.0, 2.0, 3.0, 8.0, 15.0, 48.0, 105.0, 384.0, 945.0]
 
 For large `x`, double factorials follow a Stirling-like asymptotic
 approximation::
 
     >>> x = mpf(10000)
@@ -2798,15 +2798,16 @@
 far the most common).
 
 **Examples**
 
 Verifying that :func:`~mpmath.hyper` gives the sum in the definition, by
 comparison with :func:`~mpmath.nsum`::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, hyper, rf, fac, nsum, inf, mpf, sqrt, pi,
+    ...                     exp, identify, extradps)
     >>> mp.dps = 25; mp.pretty = True
     >>> a,b,c,d = 2,3,4,5
     >>> x = 0.25
     >>> hyper([a,b],[c,d],x)
     1.078903941164934876086237
     >>> fn = lambda n: rf(a,n)*rf(b,n)/rf(c,n)/rf(d,n)*x**n/fac(n)
     >>> nsum(fn, [0, inf])
@@ -2888,15 +2889,15 @@
 for some parameter values.
 
 Evaluation may be aborted if convergence appears to be too slow.
 The optional ``maxterms`` (limiting the number of series terms) and ``maxprec``
 (limiting the internal precision) keyword arguments can be used
 to control evaluation::
 
-    >>> hyper([1,2,3], [4,5,6], 10000)              # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> hyper([1,2,3], [4,5,6], 10000)
     Traceback (most recent call last):
       ...
     NoConvergence: Hypergeometric series converges too slowly. Try increasing maxterms.
     >>> hyper([1,2,3], [4,5,6], 10000, maxterms=10**6)
     7.622806053177969474396918e+4310
 
 Additional options include ``force_series`` (which forces direct use of
@@ -2918,15 +2919,15 @@
     (1.108287213689475145830699 + 0.5327107430640678181200491j)
 
 With the following magnitude of argument, the asymptotic series for `\,_3F_1`
 gives only a few digits. Using Borel summation, ``hyper`` can produce
 a value with full accuracy::
 
     >>> mp.dps = 15
-    >>> hyper([2,0.5,4], [5.25], '0.08', force_series=True)             # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> hyper([2,0.5,4], [5.25], '0.08', force_series=True)
     Traceback (most recent call last):
       ...
     NoConvergence: Hypergeometric series converges too slowly. Try increasing maxterms.
     >>> hyper([2,0.5,4], [5.25], '0.08', asymp_tol=1e-4)
     1.0725535790737
     >>> hyper([2,0.5,4], [5.25], '0.08')
     (1.07269542893559 + 5.54668863216891e-5j)
@@ -2944,15 +2945,15 @@
 By default, a parameter that appears in both ``a_s`` and ``b_s`` will be removed
 unless it is a nonpositive integer. This generally speeds up evaluation
 by producing a hypergeometric function of lower order.
 This optimization can be disabled by passing ``eliminate=False``.
 
     >>> hyper([1,2,3], [4,5,3], 10000)
     1.268943190440206905892212e+4321
-    >>> hyper([1,2,3], [4,5,3], 10000, eliminate=False)             # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> hyper([1,2,3], [4,5,3], 10000, eliminate=False)
     Traceback (most recent call last):
       ...
     NoConvergence: Hypergeometric series converges too slowly. Try increasing maxterms.
     >>> hyper([1,2,3], [4,5,3], 10000, eliminate=False, maxterms=10**6)
     1.268943190440206905892212e+4321
 
 If a nonpositive integer `-n` appears in both ``a_s`` and ``b_s``, this parameter
@@ -3005,16 +3006,16 @@
 
     (a-1) \frac{\Gamma(a-3)}{\Gamma(a-4)} \,_1F_1(a,a-1,z) = e^z(a-4)(a+z-1)
 
 with `a=1, z=3`. There is a zero factor, two gamma function poles, and
 the 1F1 function is singular; all singularities cancel out to give a finite
 value::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, hypercomb, exp
+    >>> mp.pretty = True
     >>> hypercomb(lambda a: [([a-1],[1],[a-3],[a-4],[a],[a-1],3)], [1])
     -180.769832308689
     >>> -9*exp(3)
     -180.769832308689
 
 """
 
@@ -3032,15 +3033,15 @@
 ``hyp0f1(a,z)`` is equivalent to ``hyper([],[a],z)``; see documentation for
 :func:`~mpmath.hyper` for more information.
 
 **Examples**
 
 Evaluation for arbitrary arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp0f1, chop, diff
     >>> mp.dps = 25; mp.pretty = True
     >>> hyp0f1(2, 0.25)
     1.130318207984970054415392
     >>> hyp0f1((1,2), 1234567)
     6.27287187546220705604627e+964
     >>> hyp0f1(3+4j, 1000000j)
     (3.905169561300910030267132e+606 + 3.807708544441684513934213e+606j)
@@ -3089,15 +3090,15 @@
 information.
 
 **Examples**
 
 Evaluation for real and complex values of the argument `z`, with
 fixed parameters `a = 2, b = -1/3`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp1f1, j, chop, diff, exp, quad, gammaprod
     >>> mp.dps = 25; mp.pretty = True
     >>> hyp1f1(2, (-1,3), 3.25)
     -2815.956856924817275640248
     >>> hyp1f1(2, (-1,3), -3.25)
     -1.145036502407444445553107
     >>> hyp1f1(2, (-1,3), 1000)
     -8.021799872770764149793693e+441
@@ -3148,15 +3149,15 @@
 hyp1f2 = r"""
 Gives the hypergeometric function `\,_1F_2(a_1,a_2;b_1,b_2; z)`.
 The call ``hyp1f2(a1,b1,b2,z)`` is equivalent to
 ``hyper([a1],[b1,b2],z)``.
 
 Evaluation works for complex and arbitrarily large arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp1f2, j
     >>> mp.dps = 25; mp.pretty = True
     >>> a, b, c = 1.5, (-1,3), 2.25
     >>> hyp1f2(a, b, c, 10**20)
     -1.159388148811981535941434e+8685889639
     >>> hyp1f2(a, b, c, -10**20)
     -12.60262607892655945795907
     >>> hyp1f2(a, b, c, 10**20*j)
@@ -3169,15 +3170,15 @@
 hyp2f2 = r"""
 Gives the hypergeometric function `\,_2F_2(a_1,a_2;b_1,b_2; z)`.
 The call ``hyp2f2(a1,a2,b1,b2,z)`` is equivalent to
 ``hyper([a1,a2],[b1,b2],z)``.
 
 Evaluation works for complex and arbitrarily large arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp2f2, j
     >>> mp.dps = 25; mp.pretty = True
     >>> a, b, c, d = 1.5, (-1,3), 2.25, 4
     >>> hyp2f2(a, b, c, d, 10**20)
     -5.275758229007902299823821e+43429448190325182663
     >>> hyp2f2(a, b, c, d, -10**20)
     2561445.079983207701073448
     >>> hyp2f2(a, b, c, d, 10**20*j)
@@ -3190,15 +3191,15 @@
 hyp2f3 = r"""
 Gives the hypergeometric function `\,_2F_3(a_1,a_2;b_1,b_2,b_3; z)`.
 The call ``hyp2f3(a1,a2,b1,b2,b3,z)`` is equivalent to
 ``hyper([a1,a2],[b1,b2,b3],z)``.
 
 Evaluation works for arbitrarily large arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp2f3, j
     >>> mp.dps = 25; mp.pretty = True
     >>> a1,a2,b1,b2,b3 = 1.5, (-1,3), 2.25, 4, (1,5)
     >>> hyp2f3(a1,a2,b1,b2,b3,10**20)
     -4.169178177065714963568963e+8685889590
     >>> hyp2f3(a1,a2,b1,b2,b3,-10**20)
     7064472.587757755088178629
     >>> hyp2f3(a1,a2,b1,b2,b3,10**20*j)
@@ -3232,15 +3233,15 @@
 is equivalent to ``hyper([a,b],[c],z)``.
 
 **Examples**
 
 Evaluation with `z` inside, outside and on the unit circle, for
 fixed parameters::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp2f1, j, gammaprod, quad, diff, chop
     >>> mp.dps = 25; mp.pretty = True
     >>> hyp2f1(2, (1,2), 4, 0.75)
     1.303703703703703703703704
     >>> hyp2f1(2, (1,2), 4, -1.75)
     0.7431290566046919177853916
     >>> hyp2f1(2, (1,2), 4, 1.75)
     (1.418075801749271137026239 - 1.114976146679907015775102j)
@@ -3307,15 +3308,15 @@
 and for `|z| \ge 1` by analytic continuation. The analytic structure of this
 function is similar to that of `\,_2F_1`, generally with a singularity at
 `z = 1` and a branch cut on `(1, \infty)`.
 
 Evaluation is supported inside, on, and outside
 the circle of convergence `|z| = 1`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp3f2, sqrt, j, pi, ln2, ellipe, hyp2f1
     >>> mp.dps = 25; mp.pretty = True
     >>> hyp3f2(1,2,3,4,5,0.25)
     1.083533123380934241548707
     >>> hyp3f2(1,2+2j,3,4,5,-10+10j)
     (0.1574651066006004632914361 - 0.03194209021885226400892963j)
     >>> hyp3f2(1,2,3,4,5,-10)
     0.3071141169208772603266489
@@ -3378,15 +3379,15 @@
 hypergeometric differential equation (the first is provided by `\,_1F_1`  --
 see :func:`~mpmath.hyp1f1`).
 
 **Examples**
 
 Evaluation for arbitrary complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyperu, chop, diff, quad, gamma, exp, inf
     >>> mp.dps = 25; mp.pretty = True
     >>> hyperu(2,3,4)
     0.0625
     >>> hyperu(0.25, 5, 1000)
     0.1779949416140579573763523
     >>> hyperu(0.25, 5, -1000)
     (0.1256256609322773150118907 - 0.1256256609322773150118907j)
@@ -3437,15 +3438,15 @@
 is a nonpositive integer, as it then terminates into a polynomial
 after `-a` or `-b` terms.
 
 **Examples**
 
 Evaluation is supported for arbitrary complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hyp2f0, j, nprint, identify, taylor
     >>> mp.dps = 25; mp.pretty = True
     >>> hyp2f0((2,3), 1.25, -100)
     0.07095851870980052763312791
     >>> hyp2f0((2,3), 1.25, 100)
     (-0.03254379032170590665041131 + 0.07269254613282301012735797j)
     >>> hyp2f0(-0.75, 1-j, 4j)
     (-0.3579987031082732264862155 - 3.052951783922142735255881j)
@@ -3526,95 +3527,121 @@
   P(z,a,b) = \frac{\Gamma(z,a,b)}{\Gamma(z)}.
 
 **Examples**
 
 We can compare with numerical quadrature to verify that
 :func:`~mpmath.gammainc` computes the integral in the definition::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, gammainc, quad, exp, findroot, mpf, sqrt,
+    ...                     erf, pi, identify, ei, lower_gamma, upper_gamma)
     >>> mp.dps = 25; mp.pretty = True
     >>> gammainc(2+3j, 4, 10)
     (0.00977212668627705160602312 - 0.0770637306312989892451977j)
     >>> quad(lambda t: t**(2+3j-1) * exp(-t), [4, 10])
     (0.00977212668627705160602312 - 0.0770637306312989892451977j)
 
 Argument symmetries follow directly from the integral definition::
 
     >>> gammainc(3, 4, 5) + gammainc(3, 5, 4)
     0.0
-    >>> gammainc(3,0,2) + gammainc(3,2,4); gammainc(3,0,4)
+    >>> lower_gamma(3,2) + gammainc(3,2,4); lower_gamma(3,4)
     1.523793388892911312363331
     1.523793388892911312363331
     >>> findroot(lambda z: gammainc(2,z,3), 1)
     3.0
 
 Evaluation for arbitrarily large arguments::
 
-    >>> gammainc(10, 100)
+    >>> upper_gamma(10, 100)
     4.083660630910611272288592e-26
-    >>> gammainc(10, 10000000000000000)
+    >>> upper_gamma(10, 10000000000000000)
     5.290402449901174752972486e-4342944819032375
-    >>> gammainc(3+4j, 1000000+1000000j)
+    >>> upper_gamma(3+4j, 1000000+1000000j)
     (-1.257913707524362408877881e-434284 + 2.556691003883483531962095e-434284j)
 
 Evaluation of a generalized incomplete gamma function automatically chooses
 the representation that gives a more accurate result, depending on which
 parameter is larger::
 
-    >>> gammainc(10000000, 3) - gammainc(10000000, 2)   # Bad
+    >>> upper_gamma(10000000, 3) - upper_gamma(10000000, 2)   # Bad
     0.0
     >>> gammainc(10000000, 2, 3)   # Good
     1.755146243738946045873491e+4771204
-    >>> gammainc(2, 0, 100000001) - gammainc(2, 0, 100000000)   # Bad
+    >>> lower_gamma(2, 100000001) - lower_gamma(2, 100000000)   # Bad
     0.0
     >>> gammainc(2, 100000000, 100000001)   # Good
     4.078258353474186729184421e-43429441
 
 The incomplete gamma functions satisfy simple recurrence
 relations::
 
     >>> mp.dps = 25
     >>> z, a = mpf(3.5), mpf(2)
-    >>> gammainc(z+1, a); z*gammainc(z,a) + a**z*exp(-a)
+    >>> upper_gamma(z+1, a); z*upper_gamma(z,a) + a**z*exp(-a)
     10.60130296933533459267329
     10.60130296933533459267329
-    >>> gammainc(z+1,0,a); z*gammainc(z,0,a) - a**z*exp(-a)
+    >>> lower_gamma(z+1,a); z*lower_gamma(z,a) - a**z*exp(-a)
     1.030425427232114336470932
     1.030425427232114336470932
 
 Evaluation at integers and poles::
 
     >>> gammainc(-3, -4, -5)
     (-0.2214577048967798566234192 + 0.0j)
-    >>> gammainc(-3, 0, 5)
+    >>> lower_gamma(-3, 5)
     +inf
 
 If `z` is an integer, the recurrence reduces the incomplete gamma
 function to `P(a) \exp(-a) + Q(b) \exp(-b)` where `P` and
 `Q` are polynomials::
 
-    >>> gammainc(1, 2); exp(-2)
+    >>> upper_gamma(1, 2); exp(-2)
     0.1353352832366126918939995
     0.1353352832366126918939995
     >>> mp.dps = 50
     >>> identify(gammainc(6, 1, 2), ['exp(-1)', 'exp(-2)'])
     '(326*exp(-1) + (-872)*exp(-2))'
 
 The incomplete gamma functions reduce to functions such as
 the exponential integral Ei and the error function for special
 arguments::
 
     >>> mp.dps = 25
-    >>> gammainc(0, 4); -ei(-4)
+    >>> upper_gamma(0, 4); -ei(-4)
     0.00377935240984890647887486
     0.00377935240984890647887486
-    >>> gammainc(0.5, 0, 2); sqrt(pi)*erf(sqrt(2))
+    >>> lower_gamma(0.5, 2); sqrt(pi)*erf(sqrt(2))
     1.691806732945198336509541
     1.691806732945198336509541
 
+**Related functions**
+
+See also :func:`~mpmath.lower_gamma` and :func:`~mpmath.upper_gamma`.
+
+"""
+
+lower_gamma = r"""
+``lower_gamma(z, b)`` is the "lower" incomplete gamma function.
+
+.. math ::
+
+  \Gamma(z,0,b) = \int_0^b t^{z-1} e^{-t} \, dt
+
+See also :func:`~mpmath.gammainc`.
+"""
+
+upper_gamma = r"""
+``upper_gamma(z, a)`` is the "upper" incomplete gamma function.
+
+.. math ::
+
+  \Gamma(z,a,\infty) = \int_a^{\infty} t^{z-1} e^{-t} \, dt
+
+See also :func:`~mpmath.gammainc`.
+
 """
 
 erf = r"""
 Computes the error function, `\mathrm{erf}(x)`. The error
 function is the normalized antiderivative of the Gaussian function
 `\exp(-t^2)`. More precisely,
 
@@ -3622,16 +3649,16 @@
 
   \mathrm{erf}(x) = \frac{2}{\sqrt \pi} \int_0^x \exp(-t^2) \,dt
 
 **Basic examples**
 
 Simple values and limits include::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, erf, inf, nprint, chop, taylor, j
+    >>> mp.pretty = True
     >>> erf(0)
     0.0
     >>> erf(1)
     0.842700792949715
     >>> erf(-1)
     -0.842700792949715
     >>> erf(inf)
@@ -3688,16 +3715,16 @@
 
 erfc = r"""
 Computes the complementary error function,
 `\mathrm{erfc}(x) = 1-\mathrm{erf}(x)`.
 This function avoids cancellation that occurs when naively
 computing the complementary error function as ``1-erf(x)``::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, erf, erfc
+    >>> mp.pretty = True
     >>> 1 - erf(10)
     0.0
     >>> erfc(10)
     2.08848758376254e-45
 
 :func:`~mpmath.erfc` works accurately even for ludicrously large
 arguments::
@@ -3728,16 +3755,16 @@
 `\mathrm{erfi}(x) = -i\,\mathrm{erf}(ix)` for all complex
 numbers `x`.
 
 **Examples**
 
 Basic values and limits::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, erfi, inf, erf
+    >>> mp.pretty = True
     >>> erfi(0)
     0.0
     >>> erfi(1)
     1.65042575879754
     >>> erfi(-1)
     -1.65042575879754
     >>> erfi(inf)
@@ -3784,16 +3811,16 @@
 
 This function is defined only for `-1 \le x \le 1`.
 
 **Examples**
 
 Special values include::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, erfinv, erf, quad, sqrt, pi
+    >>> mp.pretty = True
     >>> erfinv(0)
     0.0
     >>> erfinv(1)
     +inf
     >>> erfinv(-1)
     -inf
 
@@ -3842,16 +3869,16 @@
 ``npdf(x, mu=0, sigma=1)`` evaluates the probability density
 function of a normal distribution with mean value `\mu`
 and variance `\sigma^2`.
 
 Elementary properties of the probability distribution can
 be verified using numerical integration::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, quad, inf, npdf
+    >>> mp.pretty = True
     >>> quad(npdf, [-inf, inf])
     1.0
     >>> quad(lambda x: npdf(x, 3), [3, inf])
     0.5
     >>> quad(lambda x: npdf(x, 3, 2), [3, inf])
     0.5
 
@@ -3864,16 +3891,16 @@
 function of a normal distribution with mean value `\mu`
 and variance `\sigma^2`.
 
 See also :func:`~mpmath.npdf`, which gives the probability density.
 
 Elementary properties include::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, ncdf, pi, inf, diff, npdf
+    >>> mp.pretty = True
     >>> ncdf(pi, mu=pi)
     0.5
     >>> ncdf(-inf)
     0.0
     >>> ncdf(+inf)
     1.0
 
@@ -3888,29 +3915,29 @@
     >>> diff(lambda x: ncdf(x, 1, 0.5), 0)
     0.107981933026376
     >>> npdf(0, 1, 0.5)
     0.107981933026376
 """
 
 expint = r"""
-:func:`~mpmath.expint(n,z)` gives the generalized exponential integral
+:func:`~mpmath.expint` gives the generalized exponential integral
 or En-function,
 
 .. math ::
 
     \mathrm{E}_n(z) = \int_1^{\infty} \frac{e^{-zt}}{t^n} dt,
 
 where `n` and `z` may both be complex numbers. The case with `n = 1` is
 also given by :func:`~mpmath.e1`.
 
 **Examples**
 
 Evaluation at real and complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, expint, fac, exp, pi
     >>> mp.dps = 25; mp.pretty = True
     >>> expint(1, 6.25)
     0.0002704758872637179088496194
     >>> expint(-3, 2+3j)
     (0.00299658467335472929656159 + 0.06100816202125885450319632j)
     >>> expint(2+3j, 4-5j)
     (0.001803529474663565056945248 - 0.002235061547756185403349091j)
@@ -3942,15 +3969,15 @@
 
 This is equivalent to :func:`~mpmath.expint` with `n = 1`.
 
 **Examples**
 
 Two ways to evaluate this function::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, e1, expint, ei
     >>> mp.dps = 25; mp.pretty = True
     >>> e1(6.25)
     0.0002704758872637179088496194
     >>> expint(1,6.25)
     0.0002704758872637179088496194
 
 The E1-function is essentially the same as the Ei-function (:func:`~mpmath.ei`)
@@ -3984,16 +4011,17 @@
 The Ei-function is related to the more general family of exponential
 integral functions denoted by `E_n`, which are available as :func:`~mpmath.expint`.
 
 **Basic examples**
 
 Some basic values and limits are::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, ei, inf, quad, exp, chop, si, pi, j, chi,
+    ...                     shi, hyper, euler, ln, ci)
+    >>> mp.pretty = True
     >>> ei(0)
     -inf
     >>> ei(1)
     1.89511781635594
     >>> ei(inf)
     +inf
     >>> ei(-inf)
@@ -4085,15 +4113,15 @@
 the polylogarithm (also denoted by Li), which is implemented
 as :func:`~mpmath.polylog`.
 
 **Examples**
 
 Some basic values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, li, findroot, ei, log, quad, inf, ln
     >>> mp.dps = 30; mp.pretty = True
     >>> li(0)
     0.0
     >>> li(1)
     -inf
     >>> li(1)
     -inf
@@ -4168,15 +4196,16 @@
     \mathrm{Ci}(x) = -\int_x^{\infty} \frac{\cos t}{t}\,dt
     = \gamma + \log x + \int_0^x \frac{\cos t - 1}{t}\,dt
 
 **Examples**
 
 Some values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, ci, pi, inf, chop, sinc, limit, findroot,
+    ...                     cos, quadosc, fac, nsum, euler, j)
     >>> mp.dps = 25; mp.pretty = True
     >>> ci(0)
     -inf
     >>> ci(1)
     0.3374039229009681346626462
     >>> ci(pi)
     0.07366791204642548599010096
@@ -4237,15 +4266,15 @@
 The sine integral is thus the antiderivative of the sinc
 function (see :func:`~mpmath.sinc`).
 
 **Examples**
 
 Some values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import si, mp, pi, inf, j, quad, sinc, nsum, fac
     >>> mp.dps = 25; mp.pretty = True
     >>> si(0)
     0.0
     >>> si(1)
     0.9460830703671830149413533
     >>> si(-1)
     -0.9460830703671830149413533
@@ -4295,15 +4324,15 @@
 .. math ::
 
     \mathrm{Chi}(x) = -\int_x^{\infty} \frac{\cosh t}{t}\,dt
     = \gamma + \log x + \int_0^x \frac{\cosh t - 1}{t}\,dt
 
 Some values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, chi, inf, findroot, j
     >>> mp.dps = 25; mp.pretty = True
     >>> chi(0)
     -inf
     >>> chi(1)
     0.8378669409802082408946786
     >>> chi(inf)
     +inf
@@ -4325,15 +4354,15 @@
 
 .. math ::
 
     \mathrm{Shi}(x) = \int_0^x \frac{\sinh t}{t}\,dt.
 
 Some values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, shi, inf, j
     >>> mp.dps = 25; mp.pretty = True
     >>> shi(0)
     0.0
     >>> shi(1)
     1.057250875375728514571842
     >>> shi(-1)
     -1.057250875375728514571842
@@ -4359,15 +4388,15 @@
 Note that some sources define this function
 without the normalization factor `\pi/2`.
 
 **Examples**
 
 Some basic values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, fresnels, inf, quad, sin, pi
     >>> mp.dps = 25; mp.pretty = True
     >>> fresnels(0)
     0.0
     >>> fresnels(inf)
     0.5
     >>> fresnels(-inf)
     -0.5
@@ -4394,15 +4423,15 @@
 Note that some sources define this function
 without the normalization factor `\pi/2`.
 
 **Examples**
 
 Some basic values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, fresnelc, inf, quad, cos, pi
     >>> mp.dps = 25; mp.pretty = True
     >>> fresnelc(0)
     0.0
     >>> fresnelc(inf)
     0.5
     >>> fresnelc(-inf)
     -0.5
@@ -4474,15 +4503,17 @@
 .. literalinclude :: /plots/ai_c.py
 .. image :: /plots/ai_c.png
 
 **Basic examples**
 
 Limits and values include::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, airyai, power, gamma, inf, j, findroot,
+    ...                     airyaizero, chop, airybi, besselj, nprint,
+    ...                     taylor, sqrt, diff, quad, pi, differint)
     >>> mp.dps = 25; mp.pretty = True
     >>> airyai(0); 1/(power(3,'2/3')*gamma('2/3'))
     0.3550280538878172392600632
     0.3550280538878172392600632
     >>> airyai(1)
     0.1352924163128814155241474
     >>> airyai(-1)
@@ -4667,15 +4698,17 @@
 .. literalinclude :: /plots/bi_c.py
 .. image :: /plots/bi_c.png
 
 **Basic examples**
 
 Limits and values include::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, airybi, power, gamma, inf, airybizero, findroot,
+    ...                     quad, nprint, taylor, mpf, sqrt, besselj, chop, diff,
+    ...                     differint, pi, j)
     >>> mp.dps = 25; mp.pretty = True
     >>> airybi(0); 1/(power(3,'1/6')*gamma('2/3'))
     0.6149266274460007351509224
     0.6149266274460007351509224
     >>> airybi(1)
     1.207423594952871259436379
     >>> airybi(-1)
@@ -4826,15 +4859,15 @@
 zero `a'_k` of the derivative function, i.e.
 `\operatorname{Ai}'(a'_k) = 0`, is computed.
 
 **Examples**
 
 Some values of `a_k`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, airyaizero, airyai, chop
     >>> mp.dps = 25; mp.pretty = True
     >>> airyaizero(1)
     -2.338107410459767038489197
     >>> airyaizero(2)
     -4.087949444130970616636989
     >>> airyaizero(3)
     -5.520559828095551059129856
@@ -4875,15 +4908,15 @@
 `\operatorname{Bi}'(b'_k) = 0` or `\operatorname{Bi}'(\beta'_k) = 0`,
 is computed.
 
 **Examples**
 
 Some values of `b_k`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, airybizero, airybi, chop, conj, pi, arg
     >>> mp.dps = 25; mp.pretty = True
     >>> airybizero(1)
     -1.17371322270912792491998
     >>> airybizero(2)
     -3.271093302836352715680228
     >>> airybizero(3)
     -4.830737841662015932667709
@@ -4967,15 +5000,15 @@
 .. literalinclude :: /plots/ellipk.py
 .. image :: /plots/ellipk.png
 
 **Examples**
 
 Values and limits include::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, ellipk, inf, sin, quad, pi, hyp2f1, quad
     >>> mp.dps = 25; mp.pretty = True
     >>> ellipk(0)
     1.570796326794896619231322
     >>> ellipk(inf)
     (0.0 + 0.0j)
     >>> ellipk(-inf)
     0.0
@@ -5027,16 +5060,17 @@
 **Examples**
 
 It is a well-known theorem that the geometric mean of
 two distinct positive numbers is less than the arithmetic
 mean. It follows that the arithmetic-geometric mean lies
 between the two means::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, mpf, agm, pi, log, j, quad, cos, sin,
+    ...                     gamma, sqrt, e, inf)
+    >>> mp.pretty = True
     >>> a = mpf(3)
     >>> b = mpf(4)
     >>> sqrt(a*b)
     3.46410161513775
     >>> agm(a,b)
     3.48202767635957
     >>> (a+b)/2
@@ -5117,31 +5151,33 @@
 
 The branch cut chosen for complex `a` and `b` is somewhat
 arbitrary.
 
 """
 
 gegenbauer = r"""
-Evaluates the Gegenbauer polynomial, or ultraspherical polynomial,
+Evaluates the Gegenbauer function, a generalization of Gegenbauer (or
+ultraspherical) polynomials.
 
 .. math ::
 
-    C_n^{(a)}(z) = {n+2a-1 \choose n} \,_2F_1\left(-n, n+2a;
-        a+\frac{1}{2}; \frac{1}{2}(1-z)\right).
+    C_n^{(a)}(z) = \frac{\Gamma\left(n+2a\right)}
+                    {\Gamma\left(2a\right)\Gamma\left(n+1\right)}
+        \,_2F_1\left(-n, n+2a;a+\frac{1}{2}; \frac{1}{2}(1-z)\right).
 
 When `n` is a nonnegative integer, this formula gives a polynomial
 in `z` of degree `n`, but all parameters are permitted to be
 complex numbers. With `a = 1/2`, the Gegenbauer polynomial
 reduces to a Legendre polynomial.
 
 **Examples**
 
 Evaluation for arbitrary arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, gegenbauer, chop, diff, taylor, quad
     >>> mp.dps = 25; mp.pretty = True
     >>> gegenbauer(3, 0.5, -10)
     -2485.0
     >>> gegenbauer(1000, 10, 100)
     3.012757178975667428359374e+2322
     >>> gegenbauer(2+3j, -0.75, -1000j)
     (-5038991.358609026523401901 + 9414549.285447104177860806j)
@@ -5207,15 +5243,15 @@
 .. literalinclude :: /plots/laguerre.py
 .. image :: /plots/laguerre.png
 
 **Examples**
 
 Evaluation for arbitrary arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, laguerre, j, chop, fac, taylor, quad, exp, inf
     >>> mp.dps = 25; mp.pretty = True
     >>> laguerre(5, 0, 0.25)
     0.03726399739583333333333333
     >>> laguerre(1+j, 0.5, 2+3j)
     (4.474921610704496808379097 - 11.02058050372068958069241j)
     >>> laguerre(2, 0, 10000)
     49980001.0
@@ -5284,15 +5320,15 @@
 .. literalinclude :: /plots/hermite.py
 .. image :: /plots/hermite.png
 
 **Examples**
 
 Evaluation for arbitrary arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, hermite, chop, taylor, chop, diff, exp, inf, quad
     >>> mp.dps = 25; mp.pretty = True
     >>> hermite(0, 10)
     1.0
     >>> hermite(1, 10); hermite(2, 10)
     20.0
     398.0
     >>> hermite(10000, 2)
@@ -5367,16 +5403,17 @@
 terminates after a finite number of terms, giving
 a polynomial in `x`.
 
 **Evaluation of Jacobi polynomials**
 
 A special evaluation is `P_n^{(a,b)}(1) = {n+a \choose n}`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, jacobi, binomial, nprint, taylor, chop,
+    ...                     quad, diff, pi)
+    >>> mp.pretty = True
     >>> jacobi(4, 0.5, 0.25, 1)
     2.4609375
     >>> binomial(4+0.5, 4)
     2.4609375
 
 A Jacobi polynomial of degree `n` is equal to its
 Taylor polynomial of degree `n`. The explicit
@@ -5428,15 +5465,15 @@
 .. math ::
 
   (1-x^2) y'' + (b-a-(a+b+2)x) y' + n (n+a+b+1) y = 0.
 
 We can verify that :func:`~mpmath.jacobi` approximately satisfies
 this equation::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, jacobi, diff, nprint, pi
     >>> mp.dps = 15
     >>> a = 2.5
     >>> b = 4
     >>> n = 3
     >>> y = lambda x: jacobi(n,a,b,x)
     >>> x = pi
     >>> A0 = n*(n+a+b+1)*y(x)
@@ -5485,16 +5522,17 @@
 .. image :: /plots/legendre.png
 
 **Basic evaluation**
 
 The Legendre polynomials assume fixed values at the points
 `x = -1` and `x = 1`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, legendre, nprint, chop, taylor, polyroots,
+    ...                     quad, diff)
+    >>> mp.pretty = True
     >>> nprint([legendre(n, 1) for n in range(6)])
     [1.0, 1.0, 1.0, 1.0, 1.0, 1.0]
     >>> nprint([legendre(n, -1) for n in range(6)])
     [1.0, -1.0, 1.0, -1.0, 1.0, -1.0]
 
 The coefficients of Legendre polynomials can be recovered
 using degree-`n` Taylor expansion::
@@ -5594,15 +5632,16 @@
 `C_1`, `C_2`, where `Q_n^m(z)` is a Legendre function of the
 second kind as implemented by :func:`~mpmath.legenq`.
 
 **Examples**
 
 Evaluation for arbitrary parameters and arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, legenp, legendre, chop, legenq, diff,
+    ...                     mpmathify, j)
     >>> mp.dps = 25; mp.pretty = True
     >>> legenp(2, 0, 10); legendre(2, 10)
     149.5
     149.5
     >>> legenp(-2, 0.5, 2.5)
     (1.972260393822275434196053 - 1.972260393822275434196053j)
     >>> legenp(2+3j, 1-j, -0.5+4j)
@@ -5666,15 +5705,15 @@
 Abramowitz & Stegun (eq. 8.1.3) but with `(z+1)^{m/2}(z-1)^{m/2}` instead
 of `(z^2-1)^{m/2}`, giving slightly different branches.
 
 **Examples**
 
 Evaluation for arbitrary parameters and arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, legenq, j, chop
     >>> mp.dps = 25; mp.pretty = True
     >>> legenq(2, 0, 0.5)
     -0.8186632680417568557122028
     >>> legenq(-1.5, -2, 2.5)
     (0.6655964618250228714288277 + 0.3937692045497259717762649j)
     >>> legenq(2-j, 3+4j, -6+5j)
     (-10001.95256487468541686564 - 6011.691337610097577791134j)
@@ -5711,16 +5750,16 @@
 .. image :: /plots/chebyt.png
 
 **Basic evaluation**
 
 The coefficients of the `n`-th polynomial can be recovered
 using using degree-`n` Taylor expansion::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, nprint, chop, taylor, chebyt, quad, sqrt
+    >>> mp.pretty = True
     >>> for n in range(5):
     ...     nprint(chop(taylor(lambda x: chebyt(n, x), 0, n)))
     ...
     [1.0]
     [0.0, 1.0]
     [-1.0, 0.0, 2.0]
     [0.0, -3.0, 0.0, 4.0]
@@ -5761,16 +5800,16 @@
 .. image :: /plots/chebyu.png
 
 **Basic evaluation**
 
 The coefficients of the `n`-th polynomial can be recovered
 using using degree-`n` Taylor expansion::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, nprint, taylor, chop, chebyu, sqrt, quad
+    >>> mp.pretty = True
     >>> for n in range(5):
     ...     nprint(chop(taylor(lambda x: chebyu(n, x), 0, n)))
     ...
     [1.0]
     [0.0, 2.0]
     [-1.0, 0.0, 4.0]
     [0.0, -4.0, 0.0, 8.0]
@@ -5832,16 +5871,17 @@
 .. image :: /plots/besselj_c.png
 
 **Examples**
 
 Evaluation is supported for arbitrary arguments, and at
 arbitrary precision::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, besselj, pi, nprint, findroot, quadosc, sqrt,
+    ...                     pi, sin, cos, diff, j0, j1, quad, differint, j, inf)
+    >>> mp.pretty = True
     >>> besselj(2, 1000)
     -0.024777229528606
     >>> besselj(4, 0.75)
     0.000801070086542314
     >>> besselj(2, 1000j)
     (-2.48071721019185e+432 + 6.41567059811949e-437j)
     >>> mp.dps = 25
@@ -5951,15 +5991,15 @@
 .. literalinclude :: /plots/besseli_c.py
 .. image :: /plots/besseli_c.png
 
 **Examples**
 
 Some values of `I_n(x)`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, besseli, exp, cos, pi, diff, quad
     >>> mp.dps = 25; mp.pretty = True
     >>> besseli(0,0)
     1.0
     >>> besseli(1,0)
     0.0
     >>> besseli(0,1)
     1.266065877752008335598245
@@ -6026,15 +6066,15 @@
 .. literalinclude :: /plots/bessely_c.py
 .. image :: /plots/bessely_c.png
 
 **Examples**
 
 Some values of `Y_n(x)`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, bessely, pi, diff, quad
     >>> mp.dps = 25; mp.pretty = True
     >>> bessely(0,0), bessely(1,0), bessely(2,0)
     (-inf, -inf, -inf)
     >>> bessely(1, pi)
     0.3588729167767189594679827
     >>> bessely(0.5, 3+4j)
     (9.242861436961450520325216 - 3.085042824915332562522402j)
@@ -6089,15 +6129,15 @@
 .. literalinclude :: /plots/besselk_c.py
 .. image :: /plots/besselk_c.png
 
 **Examples**
 
 Evaluation is supported for arbitrary complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, besselk, j, fmul
     >>> mp.dps = 25; mp.pretty = True
     >>> besselk(0,1)
     0.4210244382407083333356274
     >>> besselk(0, -1)
     (0.4210244382407083333356274 - 3.97746326050642263725661j)
     >>> besselk(3.5, 2+3j)
     (-0.02090732889633760668464128 + 0.2464022641351420167819697j)
@@ -6151,15 +6191,15 @@
 .. literalinclude :: /plots/hankel1_c.py
 .. image :: /plots/hankel1_c.png
 
 **Examples**
 
 The Hankel function is generally complex-valued::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, pi, hankel1
     >>> mp.dps = 25; mp.pretty = True
     >>> hankel1(2, pi)
     (0.4854339326315091097054957 - 0.0999007139290278787734903j)
     >>> hankel1(3.5, pi)
     (0.2340002029630507922628888 - 0.6419643823412927142424049j)
 """
 
@@ -6178,15 +6218,15 @@
 .. literalinclude :: /plots/hankel2_c.py
 .. image :: /plots/hankel2_c.png
 
 **Examples**
 
 The Hankel function is generally complex-valued::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, pi, hankel2
     >>> mp.dps = 25; mp.pretty = True
     >>> hankel2(2, pi)
     (0.4854339326315091097054957 + 0.0999007139290278787734903j)
     >>> hankel2(3.5, pi)
     (0.2340002029630507922628888 + 0.6419643823412927142424049j)
 """
 
@@ -6219,15 +6259,16 @@
 .. literalinclude :: /plots/lambertw_c.py
 .. image :: /plots/lambertw_c.png
 
 **Basic examples**
 
 The Lambert W function is the inverse of `w \exp(w)`::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, lambertw, exp, chop, mpf, log, nprint,
+    ...                     taylor, inf, e, eps)
     >>> mp.dps = 25; mp.pretty = True
     >>> w = lambertw(1)
     >>> w
     0.5671432904097838729999687
     >>> w*exp(w)
     1.0
 
@@ -6340,16 +6381,17 @@
 For positive integers `n`, we have have relation to superfactorials
 `G(n) = \mathrm{sf}(n-2) = 0! \cdot 1! \cdots (n-2)!`.
 
 **Examples**
 
 Some elementary values and limits of the Barnes G-function::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, barnesg, sqrt, exp, log, glaisher, inf,
+    ...                     catalan, pi, nthroot, gamma, limit, mpf, psi, diff)
+    >>> mp.pretty = True
     >>> barnesg(1), barnesg(2), barnesg(3)
     (1.0, 1.0, 1.0)
     >>> barnesg(4)
     2.0
     >>> barnesg(5)
     12.0
     >>> barnesg(6)
@@ -6453,16 +6495,16 @@
 For general complex `z`, `\mathrm{sf}(z)` is defined
 in terms of the Barnes G-function (see :func:`~mpmath.barnesg`).
 
 **Examples**
 
 The first few superfactorials are (OEIS A000178)::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, superfac, pi, diff
+    >>> mp.pretty = True
     >>> for n in range(10):
     ...     print("%s %s" % (n, superfac(n)))
     ...
     0 1.0
     1 1.0
     2 2.0
     3 12.0
@@ -6523,16 +6565,17 @@
         \right].
 
 **Examples**
 
 The rapidly-growing sequence of hyperfactorials begins
 (OEIS A002109)::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, hyperfac, diff, pi, mpf, chop, exp, quad,
+    ...                     binomial, loggamma, sqrt, j)
+    >>> mp.pretty = True
     >>> for n in range(10):
     ...     print("%s %s" % (n, hyperfac(n)))
     ...
     0 1.0
     1 1.0
     2 4.0
     3 108.0
@@ -6605,15 +6648,15 @@
 function evaluates to zero at the poles
 of the gamma function, `z = 0, -1, -2, \ldots`.
 
 **Examples**
 
 Basic examples::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, rgamma, inf, pi, log, exp, quad, e
     >>> mp.dps = 25; mp.pretty = True
     >>> rgamma(1)
     1.0
     >>> rgamma(4)
     0.1666666666666666666666667
     >>> rgamma(0); rgamma(-1)
     0.0
@@ -6651,15 +6694,16 @@
 Computationally, it is advantageous to use :func:`~mpmath.loggamma`
 instead of :func:`~mpmath.gamma` for extremely large arguments.
 
 **Examples**
 
 Comparing with `\ln(\Gamma(z))`::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, log, loggamma, pi, j, ln2, sqrt, inf, quad,
+    ...                     diff, psi)
     >>> mp.dps = 25; mp.pretty = True
     >>> loggamma('13.2'); log(gamma('13.2'))
     20.49400419456603678498394
     20.49400419456603678498394
     >>> loggamma(3+4j)
     (-1.756626784603784110530604 + 4.742664438034657928194889j)
     >>> log(gamma(3+4j))
@@ -6748,15 +6792,16 @@
     }{2i} - \frac{\log \pi}{2} t.
 
 The Riemann-Siegel theta function is important in
 providing the phase factor for the Z-function
 (see :func:`~mpmath.siegelz`). Evaluation is supported for real and
 complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, siegeltheta, inf, diff, nprint, chop, taylor,
+    ...                     findroot, diffun, log, pi, mpf)
     >>> mp.dps = 25; mp.pretty = True
     >>> siegeltheta(0)
     0.0
     >>> siegeltheta(inf)
     +inf
     >>> siegeltheta(-inf)
     -inf
@@ -6797,15 +6842,15 @@
 grampoint = r"""
 Gives the `n`-th Gram point `g_n`, defined as the solution
 to the equation `\theta(g_n) = \pi n` where `\theta(t)`
 is the Riemann-Siegel theta function (:func:`~mpmath.siegeltheta`).
 
 The first few Gram points are::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, grampoint, siegeltheta, pi, findroot
     >>> mp.dps = 25; mp.pretty = True
     >>> grampoint(0)
     17.84559954041086081682634
     >>> grampoint(1)
     23.17028270124630927899664
     >>> grampoint(2)
     27.67018221781633796093849
@@ -6849,15 +6894,16 @@
 
 where `\zeta(s)` is the Riemann zeta function (:func:`~mpmath.zeta`)
 and where `\theta(t)` denotes the Riemann-Siegel theta function
 (see :func:`~mpmath.siegeltheta`).
 
 Evaluation is supported for real and complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, siegelz, diff, nprint, chop, taylor,
+    ...                     findroot, zeta, grampoint)
     >>> mp.dps = 25; mp.pretty = True
     >>> siegelz(1)
     -0.7363054628673177346778998
     >>> siegelz(3+4j)
     (-0.1852895764366314976003936 - 0.2773099198055652246992479j)
 
 The first four derivatives are supported, using the
@@ -6945,16 +6991,16 @@
 
 **Examples**
 
 For small arguments, the Riemann R function almost exactly
 gives the prime counting function if rounded to the nearest
 integer::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, primepi, riemannr, nstr, li, diff, mpf
+    >>> mp.pretty = True
     >>> primepi(50), riemannr(50)
     (15, 14.9757023241462)
     >>> max(abs(primepi(n)-int(round(riemannr(n)))) for n in range(100))
     1
     >>> max(abs(primepi(n)-int(round(riemannr(n)))) for n in range(300))
     2
 
@@ -7018,15 +7064,15 @@
 precisely for large `x`, and the present implementation is
 not optimized in any way. For numerical approximation of the
 prime counting function, it is better to use :func:`~mpmath.primepi2`
 or :func:`~mpmath.riemannr`.
 
 Some values of the prime counting function::
 
-    >>> from mpmath import *
+    >>> from mpmath import primepi
     >>> [primepi(k) for k in range(20)]
     [0, 0, 1, 2, 2, 3, 3, 4, 4, 4, 4, 5, 5, 6, 6, 6, 6, 7, 7, 8]
     >>> primepi(3.5)
     2
     >>> primepi(100000)
     9592
 
@@ -7046,17 +7092,17 @@
 is returned. This estimate is rigorous assuming the truth of
 the Riemann hypothesis, and can be computed very quickly.
 
 **Examples**
 
 Exact values of the prime counting function for small `x`::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
-    >>> iv.dps = 15; iv.pretty = True
+    >>> from mpmath import mp, iv, primepi2, primepi, mpf, riemannr
+    >>> mp.pretty = True
+    >>> iv.pretty = True
     >>> primepi2(10)
     [4.0, 4.0]
     >>> primepi2(100)
     [25.0, 25.0]
     >>> primepi2(1000)
     [168.0, 168.0]
 
@@ -7105,15 +7151,16 @@
 half-plane `\mathrm{Re}(s) > 0`.
 
 **Examples**
 
 Arbitrary-precision evaluation for real and complex arguments is
 supported::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, primezeta, extradps, log, eps, mertens,
+    ...                     euler, inf, mpf, pi)
     >>> mp.dps = 30; mp.pretty = True
     >>> primezeta(2)
     0.452247420041065498506543364832
     >>> primezeta(pi)
     0.15483752698840284272036497397
     >>> mp.dps = 50
     >>> primezeta(3)
@@ -7168,16 +7215,16 @@
 """
 
 bernpoly = r"""
 Evaluates the Bernoulli polynomial `B_n(z)`.
 
 The first few Bernoulli polynomials are::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import mp, nprint, chop, taylor, bernpoly, bernoulli
+    >>> mp.pretty = True
     >>> for n in range(6):
     ...     nprint(chop(taylor(lambda x: bernpoly(n,x), 0, n)))
     ...
     [1.0]
     [-0.5, 1.0]
     [0.166667, -1.0, 1.0]
     [0.0, 0.5, -1.5, 1.0]
@@ -7217,16 +7264,17 @@
 as :func:`~mpmath.li`.
 
 **Examples**
 
 The polylogarithm satisfies a huge number of functional identities.
 A sample of polylogarithm evaluations is shown below::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, polylog, log, pi, phi, zeta, j, catalan, exp,
+    ...                     zeta, quad, diff, taylor, altzeta, nsum, inf, nprint)
+    >>> mp.pretty = True
     >>> polylog(1,0.5), log(2)
     (0.693147180559945, 0.693147180559945)
     >>> polylog(2,0.5), (pi**2-6*log(2)**2)/12
     (0.582240526465012, 0.582240526465012)
     >>> polylog(2,-phi), -log(phi)**2-pi**2/10
     (-1.21852526068613, -1.21852526068613)
     >>> polylog(3,0.5), 7*zeta(3)/8-pi**2*log(2)/12+log(2)**3/6
@@ -7349,15 +7397,15 @@
 continuous in `n`; :func:`~mpmath.bell` can thus be evaluated,
 differentiated, etc for arbitrary complex arguments.
 
 **Examples**
 
 Simple evaluations::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, bell, nprint, taylor, det, superfac
     >>> mp.dps = 25; mp.pretty = True
     >>> bell(0, 2.5)
     1.0
     >>> bell(1, 2.5)
     2.5
     >>> bell(2, 2.5)
     8.75
@@ -7447,15 +7495,15 @@
 is a nonzero integer, but not otherwise. In particular, they differ
 at `n = 0`.
 
 **Examples**
 
 Evaluating a series::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, nsum, sqrt, fac, inf, polyexp, pi, hyper
     >>> mp.dps = 25; mp.pretty = True
     >>> nsum(lambda k: sqrt(k)/fac(k), [1,inf])
     2.101755547733791780315904
     >>> polyexp(0.5,1)
     2.101755547733791780315904
 
 Evaluation for arbitrary arguments::
@@ -7516,16 +7564,17 @@
     \Phi_6(x) = x^2 - x + 1
 
 **Examples**
 
 The coefficients of low-order cyclotomic polynomials can be recovered
 using Taylor expansion::
 
-    >>> from mpmath import *
-    >>> mp.dps = 15; mp.pretty = True
+    >>> from mpmath import (mp, chop, taylor, cyclotomic, nstr, fprod,
+    ...                     unitroots, polyroots)
+    >>> mp.pretty = True
     >>> for n in range(9):
     ...     p = chop(taylor(lambda x: cyclotomic(n,x), 0, 10))
     ...     print("%s %s" % (n, nstr(p[:10+1-p[::-1].index(1)])))
     ...
     0 [1.0]
     1 [-1.0, 1.0]
     2 [1.0, 1.0]
@@ -7622,15 +7671,17 @@
 
 **Examples**
 
 Many standard functions are special cases of the Meijer G-function
 (possibly rescaled and/or with branch cut corrections). We define
 some test parameters::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, mpf, meijerg, exp, log, sin, cos, sqrt, pi,
+    ...                     besselj, bessely, chop, gamma, expint, besseli,
+    ...                     besselk, erfc)
     >>> mp.dps = 25; mp.pretty = True
     >>> a = mpf(0.75)
     >>> b = mpf(1.5)
     >>> z = mpf(2.25)
 
 The exponential function:
 `e^z = G^{1,0}_{0,1} \left( \left. \begin{matrix} - \\ 0 \end{matrix} \;
@@ -7785,15 +7836,17 @@
 series. The complementary function :func:`~mpmath.clcos` gives the corresponding
 cosine sum.
 
 **Examples**
 
 Evaluation for arbitrarily chosen `s` and `z`::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, clsin, nsum, sin, inf, chop, log, exp, j,
+    ...                     ln, quad, pi, chop, cot, csc, extraprec, sqrt,
+    ...                     catalan)
     >>> mp.dps = 25; mp.pretty = True
     >>> s, z = 3, 4
     >>> clsin(s, z); nsum(lambda k: sin(z*k)/k**s, [1,inf])
     -0.6533010136329338746275795
     -0.6533010136329338746275795
 
 Using `z + \pi` instead of `z` gives an alternating series::
@@ -7905,15 +7958,16 @@
 
     = \mathrm{Re}\left[\mathrm{Li}_s(e^{iz})\right] \quad (s, z \in \mathbb{R}).
 
 **Examples**
 
 Evaluation for arbitrarily chosen `s` and `z`::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, clcos, cos, inf, nsum, pi, sqrt, exp, log, j,
+    ...                     sin, chop, nsum, csc, zeta, altzeta, extraprec)
     >>> mp.dps = 25; mp.pretty = True
     >>> s, z = 3, 4
     >>> clcos(s, z); nsum(lambda k: cos(z*k)/k**s, [1,inf])
     -0.6518926267198991308332759
     -0.6518926267198991308332759
 
 Using `z + \pi` instead of `z` gives an alternating series::
@@ -8031,15 +8085,16 @@
     W(k,m,z) = e^{-\frac{1}{2}z} z^{\frac{1}{2}+m}
         U(\tfrac{1}{2}+m-k, 1+2m, z).
 
 **Examples**
 
 Evaluation for arbitrary real and complex arguments is supported::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, whitm, j, mpf, chop, diff, inf, sqrt, pi,
+    ...                     quad, exp, whitw)
     >>> mp.dps = 25; mp.pretty = True
     >>> whitm(1, 1, 1)
     0.7302596799460411820509668
     >>> whitm(1, 1, -1)
     (0.0 - 1.417977827655098025684246j)
     >>> whitm(j, j/2, 2+3j)
     (3.245477713363581112736478 - 0.822879187542699127327782j)
@@ -8081,15 +8136,15 @@
 Evaluates the Whittaker function `W(k,m,z)`, which gives a second
 solution to the Whittaker differential equation. (See :func:`~mpmath.whitm`.)
 
 **Examples**
 
 Evaluation for arbitrary real and complex arguments is supported::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, whitw, j, mpf, chop, diff
     >>> mp.dps = 25; mp.pretty = True
     >>> whitw(1, 1, 1)
     1.19532063107581155661012
     >>> whitw(1, 1, -1)
     (-0.9424875979222187313924639 - 0.2607738054097702293308689j)
     >>> whitw(j, j/2, 2+3j)
     (0.1782899315111033879430369 - 0.01609578360403649340169406j)
@@ -8140,15 +8195,15 @@
 .. literalinclude :: /plots/ber.py
 .. image :: /plots/ber.png
 
 **Examples**
 
 Verifying the defining relation::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, ber, besselj, root, j, bei
     >>> mp.dps = 25; mp.pretty = True
     >>> n, x = 2, 3.5
     >>> ber(n,x)
     1.442338852571888752631129
     >>> bei(n,x)
     -0.948359035324558320217678
     >>> besselj(n, x*root(1,8,3))
@@ -8185,15 +8240,15 @@
 .. literalinclude :: /plots/ker.py
 .. image :: /plots/ker.png
 
 **Examples**
 
 Verifying the defining relation::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, ker, exp, kei, pi, j, besselk, root
     >>> mp.dps = 25; mp.pretty = True
     >>> n, x = 2, 4.5
     >>> ker(n,x)
     0.02542895201906369640249801
     >>> kei(n,x)
     -0.02074960467222823237055351
     >>> exp(-n*pi*j/2) * besselk(n, x*root(1,8,1))
@@ -8230,15 +8285,15 @@
 
     z^2 f''(z) + z f'(z) + (z^2-n^2) f(z) = \frac{2 z^{n+1}}{\pi (2n-1)!!}.
 
 **Examples**
 
 Evaluation for arbitrary real and complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, struveh, j, sqrt, cos, pi, mpf, diff, fac2, pi
     >>> mp.dps = 25; mp.pretty = True
     >>> struveh(0, 3.5)
     0.3608207733778295024977797
     >>> struveh(-1, 10)
     -0.255212719726956768034732
     >>> struveh(1, -100.5)
     0.5819566816797362287502246
@@ -8284,15 +8339,15 @@
 
     z^2 f''(z) + z f'(z) - (z^2+n^2) f(z) = \frac{2 z^{n+1}}{\pi (2n-1)!!}.
 
 **Examples**
 
 Evaluation for arbitrary real and complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, struvel, j, mpf, diff, fac2, pi
     >>> mp.dps = 25; mp.pretty = True
     >>> struvel(0, 3.5)
     7.180846515103737996249972
     >>> struvel(-1, 10)
     2670.994904980850550721511
     >>> struvel(1, -100.5)
     1.757089288053346261497686e+42
@@ -8331,15 +8386,16 @@
 although :func:`~mpmath.appellf1` can evaluate an analytic continuation
 with respecto to either variable, and sometimes both.
 
 **Examples**
 
 Evaluation is supported for real and complex parameters::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, appellf1, hyp2f1, chop, diff, mpmathify,
+    ...                     quad, ellipe, re, pi, mpf, sin, sqrt, j)
     >>> mp.dps = 25; mp.pretty = True
     >>> appellf1(1,0,0.5,1,0.5,0.25)
     1.154700538379251529018298
     >>> appellf1(1,1+j,0.5,1,0.5,0.5j)
     (1.138403860350148085179415 + 1.510544741058517621110615j)
 
 For some integer parameters, the F1 series reduces to a polynomial::
@@ -8458,15 +8514,16 @@
     f''(z) + \frac{1}{z}f'(z) + \left(1-\frac{\nu^2}{z^2}\right) f(z)
         = \frac{(z-\nu)}{\pi z^2} \sin(\pi \nu).
 
 **Examples**
 
 Evaluation for real and complex parameter and argument::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, angerj, besselj, mpf, diff, sinpi, quad,
+    ...                     sin, cos, pi)
     >>> mp.dps = 25; mp.pretty = True
     >>> angerj(2,3)
     0.4860912605858910769078311
     >>> angerj(-3+4j, 2+5j)
     (-5033.358320403384472395612 + 585.8011892476145118551756j)
     >>> angerj(3.25, 1e6j)
     (4.630743639715893346570743e+434290 - 1.117960409887505906848456e+434291j)
@@ -8521,15 +8578,15 @@
     f''(z) + \frac{1}{z}f'(z) + \left(1-\frac{\nu^2}{z^2}\right) f(z)
         = -\frac{1}{\pi z^2} (z+\nu+(z-\nu)\cos(\pi \nu)).
 
 **Examples**
 
 Evaluation for real and complex parameter and argument::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, webere, struveh, pi, diff, cospi, mpf, sin, quad
     >>> mp.dps = 25; mp.pretty = True
     >>> webere(2,3)
     -0.1057668973099018425662646
     >>> webere(-3+4j, 2+5j)
     (-585.8081418209852019290498 - 5033.314488899926921597203j)
     >>> webere(3.25, 1e6j)
     (-1.117960409887505906848456e+434291 - 4.630743639715893346570743e+434290j)
@@ -8589,15 +8646,16 @@
 .. literalinclude :: /plots/lommels1.py
 .. image :: /plots/lommels1.png
 
 **Examples**
 
 An integral representation::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, mpf, lommels1, quad, bessely, besselj, pi,
+    ...                     gamma, sqrt, power, struveh, diff)
     >>> mp.dps = 25; mp.pretty = True
     >>> u,v,z = 0.25, 0.125, mpf(0.75)
     >>> lommels1(u,v,z)
     0.4276243877565150372999126
     >>> (bessely(v,z)*quad(lambda t: t**u*besselj(v,t), [0,z]) - \
     ...  besselj(v,z)*quad(lambda t: t**u*bessely(v,t), [0,z]))*(pi/2)
     0.4276243877565150372999126
@@ -8644,15 +8702,16 @@
 .. literalinclude :: /plots/lommels2.py
 .. image :: /plots/lommels2.png
 
 **Examples**
 
 For large `|z|`, `S_{\mu,\nu} \sim z^{\mu-1}`::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, lommels2, power, struveh, bessely, power,
+    ...                     sqrt, pi, gamma, diff, mpf)
     >>> mp.dps = 25; mp.pretty = True
     >>> lommels2(10,2,30000)
     1.968299831601008419949804e+40
     >>> power(30000,9)
     1.9683e+40
 
 A special value::
@@ -8688,15 +8747,15 @@
 
 The series is generally absolutely convergent for `|x| + |y| < 1`.
 
 **Examples**
 
 Evaluation for real and complex arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, appellf2, chop, mpf, j, diff
     >>> mp.dps = 25; mp.pretty = True
     >>> appellf2(1,2,3,4,5,0.25,0.125)
     1.257417193533135344785602
     >>> appellf2(1,-3,-4,2,3,2,3)
     -42.8
     >>> appellf2(0.5,0.25,-0.25,2,3,0.25j,0.25)
     (0.9880539519421899867041719 + 0.01497616165031102661476978j)
@@ -8746,15 +8805,16 @@
 
 The series is generally absolutely convergent for `|x| < 1, |y| < 1`.
 
 **Examples**
 
 Evaluation for various parameters and variables::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, appellf3, hyp2f1, j, mpf, polylog, gammaprod,
+    ...                     hyp3f2, chop, diff)
     >>> mp.dps = 25; mp.pretty = True
     >>> appellf3(1,2,3,4,5,0.5,0.25)
     2.221557778107438938158705
     >>> appellf3(1,2,3,4,5,6,0); hyp2f1(1,3,5,6)
     (-0.5189554589089861284537389 - 0.1454441043328607980769742j)
     (-0.5189554589089861284537389 - 0.1454441043328607980769742j)
     >>> appellf3(1,-2,-3,1,1,4,6)
@@ -8817,15 +8877,15 @@
 The series is generally absolutely convergent for
 `\sqrt{|x|} + \sqrt{|y|} < 1`.
 
 **Examples**
 
 Evaluation for various parameters and arguments::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, appellf4, hyp2f1, diff, chop, mpf
     >>> mp.dps = 25; mp.pretty = True
     >>> appellf4(1,1,2,2,0.25,0.125)
     1.286182069079718313546608
     >>> appellf4(-2,-3,4,5,4,5)
     34.8
     >>> appellf4(5,4,2,3,0.25j,-0.125j)
     (-0.2585967215437846642163352 + 2.436102233553582711818743j)
@@ -8899,15 +8959,17 @@
 arbitrary complex `a`, but may be slow and/or inaccurate when `\Re(s) < 0` for
 nonrational `a` or when computing derivatives.
 
 **Examples**
 
 Some values of the Riemann zeta function::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, zeta, pi, inf, euler, j, zetazero, findroot,
+    ...                     chop, catalan, psi, ln, loggamma, fac, mpf, diff,
+    ...                     nsum)
     >>> mp.dps = 25; mp.pretty = True
     >>> zeta(2); pi**2 / 6
     1.644934066848226436472415
     1.644934066848226436472415
     >>> zeta(0)
     -0.5
     >>> zeta(-1)
@@ -9081,15 +9143,16 @@
 Also the derivative with respect to `s` (currently only a first
 derivative) can be evaluated.
 
 **Examples**
 
 The ordinary Riemann zeta function::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, zeta, dirichlet, ln, pi, catalan, diff, log,
+    ...                     gamma, log, sqrt, euler, nsum, inf, ln2)
     >>> mp.dps = 25; mp.pretty = True
     >>> dirichlet(3, [1]); zeta(3)
     1.202056903159594285399738
     1.202056903159594285399738
     >>> dirichlet(1, [1])
     +inf
 
@@ -9170,15 +9233,16 @@
 .. literalinclude :: /plots/coulombf_c.py
 .. image :: /plots/coulombf_c.png
 
 **Examples**
 
 Evaluation is supported for arbitrary magnitudes of `z`::
 
-    >>> from mpmath import *
+    >>> from mpmath import  (mp, coulombf, mpf, chop, diff, coulombg, sqrt,
+    ...                      exp, j, quad, coulombc, fac, inf)
     >>> mp.dps = 25; mp.pretty = True
     >>> coulombf(2, 1.5, 3.5)
     0.4080998961088761187426445
     >>> coulombf(-2, 1.5, 3.5)
     0.7103040849492536747533465
     >>> coulombf(2, 1.5, '1e-10')
     4.143324917492256448770769e-33
@@ -9285,15 +9349,15 @@
 .. literalinclude :: /plots/coulombg_c.py
 .. image :: /plots/coulombg_c.png
 
 **Examples**
 
 Evaluation is supported for arbitrary magnitudes of `z`::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, coulombg, diff
     >>> mp.dps = 25; mp.pretty = True
     >>> coulombg(-2, 1.5, 3.5)
     1.380011900612186346255524
     >>> coulombg(2, 1.5, 3.5)
     1.919153700722748795245926
     >>> coulombg(-2, 1.5, '1e-10')
     201126715824.7329115106793
@@ -9362,15 +9426,15 @@
         \frac{\vartheta_2(t,q)}{\vartheta_4(t,q)}
 
     \mathrm{dn}(u,m) = \frac{\vartheta_4(0,q)}{\vartheta_3(0,q)}
         \frac{\vartheta_3(t,q)}{\vartheta_4(t,q)},
 
 or more generally computes a ratio of two such functions. Here
 `t = u/\vartheta_3(0,q)^2`, and `q = q(m)` denotes the nome (see
-:func:`~mpmath.nome`). Optionally, you can specify the nome directly
+``mpmath.functions.elliptic.nome()``). Optionally, you can specify the nome directly
 instead of `m` by passing ``q=<value>``, or you can directly
 specify the elliptic parameter `k` with ``k=<value>``.
 
 The first argument should be a two-character string specifying the
 function using any combination of ``'s'``, ``'c'``, ``'d'``, ``'n'``. These
 letters respectively denote the basic functions
 `\mathrm{sn}(u,m)`, `\mathrm{cn}(u,m)`, `\mathrm{dn}(u,m)`, and `1`.
@@ -9390,15 +9454,15 @@
 If called with only the first argument, a function object
 evaluating the chosen function for given arguments is returned.
 
 **Examples**
 
 Basic evaluation::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, ellipfun, ellipk, chop, j
     >>> mp.dps = 25; mp.pretty = True
     >>> ellipfun('cd', 3.5, 0.5)
     -0.9891101840595543931308394
     >>> ellipfun('cd', 3.5, q=0.25)
     0.07111979240214668158441418
 
 The sn-function is doubly periodic in the complex plane with periods
@@ -9473,15 +9537,16 @@
 
 **Examples and basic properties**
 
 Considered as functions of `z`, the Jacobi theta functions may be
 viewed as generalizations of the ordinary trigonometric functions
 cos and sin. They are periodic functions::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, jtheta, pi, nprint, fourier, exp, j, mpf,
+    ...                     gamma, diff, sqrt)
     >>> mp.dps = 25; mp.pretty = True
     >>> jtheta(1, 0.25, '0.2')
     0.2945120798627300045053104
     >>> jtheta(1, 0.25 + 2*pi, '0.2')
     0.2945120798627300045053104
 
 Indeed, the series defining the theta functions are essentially
@@ -9593,15 +9658,15 @@
 Euler polynomials (see :func:`~mpmath.eulerpoly`) as `E_n = 2^n E_n(1/2)`.
 
 **Examples**
 
 Computing the first few Euler numbers and verifying that they
 agree with the Taylor series::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, eulernum, chop, diffs, sech, sqrt, pi, e
     >>> mp.dps = 25; mp.pretty = True
     >>> [eulernum(n) for n in range(11)]
     [1.0, 0.0, -1.0, 0.0, 5.0, 0.0, -61.0, 0.0, 1385.0, 0.0, -50521.0]
     >>> chop(diffs(sech, 0, 10))
     [1.0, 0.0, -1.0, 0.0, 5.0, 0.0, -61.0, 0.0, 1385.0, 0.0, -50521.0]
 
 Euler numbers grow very rapidly. :func:`~mpmath.eulernum` efficiently
@@ -9653,15 +9718,15 @@
 Special values include the Euler numbers `E_n = 2^n E_n(1/2)` (see
 :func:`~mpmath.eulernum`).
 
 **Examples**
 
 Computing the coefficients of the first few Euler polynomials::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, chop, taylor, eulerpoly, inf, eulernum
     >>> mp.dps = 25; mp.pretty = True
     >>> for n in range(6):
     ...     chop(taylor(lambda z: eulerpoly(n,z), 0, n))
     ...
     [1.0]
     [-0.5, 1.0]
     [0.0, -1.0, 1.0]
@@ -9755,15 +9820,15 @@
 
 .. image :: /plots/spherharm44.png
 
 **Examples**
 
 Some low-order spherical harmonics with reference values::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, spherharm, pi, sqrt, expj, sin, fp, j, cos
     >>> mp.dps = 25; mp.pretty = True
     >>> theta = pi/4
     >>> phi = pi/3
     >>> spherharm(0,0,theta,phi); 0.5*sqrt(1/pi)*expj(0)
     (0.2820947917738781434740397 + 0.0j)
     (0.2820947917738781434740397 + 0.0j)
     >>> spherharm(1,-1,theta,phi); 0.5*sqrt(3/(2*pi))*expj(-phi)*sin(theta)
@@ -9823,15 +9888,16 @@
 .. literalinclude :: /plots/gi_c.py
 .. image :: /plots/gi_c.png
 
 **Examples**
 
 Some values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, scorergi, power, gamma, diff, inf, airybi,
+    ...                     scorerhi, chop, airyai, pi)
     >>> mp.dps = 25; mp.pretty = True
     >>> scorergi(0); 1/(power(3,'7/6')*gamma('2/3'))
     0.2049755424820002450503075
     0.2049755424820002450503075
     >>> diff(scorergi, 0); 1/(power(3,'5/6')*gamma('1/3'))
     0.1494294524512754526382746
     0.1494294524512754526382746
@@ -9917,15 +9983,16 @@
 .. literalinclude :: /plots/hi_c.py
 .. image :: /plots/hi_c.png
 
 **Examples**
 
 Some values and limits::
 
-    >>> from mpmath import *
+    >>> from mpmath import (mp, scorerhi, power, gamma, diff, inf, airyai,
+    ...                     airybi, chop)
     >>> mp.dps = 25; mp.pretty = True
     >>> scorerhi(0); 2/(power(3,'7/6')*gamma('2/3'))
     0.4099510849640004901006149
     0.4099510849640004901006149
     >>> diff(scorerhi,0); 2/(power(3,'5/6')*gamma('1/3'))
     0.2988589049025509052765491
     0.2988589049025509052765491
@@ -9988,15 +10055,15 @@
 The value is computed using an integer recurrence. The implementation
 is not optimized for approximating large values quickly.
 
 **Examples**
 
 Comparing with the generating function::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, taylor, ff, stirling1, matrix, stirling2
     >>> mp.dps = 25; mp.pretty = True
     >>> taylor(lambda x: ff(x, 5), 0, 5)
     [0.0, 24.0, -50.0, 35.0, -10.0, 1.0]
     >>> [stirling1(5, k) for k in range(6)]
     [0.0, 24.0, -50.0, 35.0, -10.0, 1.0]
 
 Recurrence relation::
@@ -10040,15 +10107,15 @@
 The value is computed using integer arithmetic to evaluate a power sum.
 The implementation is not optimized for approximating large values quickly.
 
 **Examples**
 
 Comparing with the generating function::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, stirling2, taylor, ff
     >>> mp.dps = 25; mp.pretty = True
     >>> taylor(lambda x: sum(stirling2(5,k) * ff(x,k) for k in range(6)), 0, 5)
     [0.0, 0.0, 0.0, 0.0, 0.0, 1.0]
 
 Recurrence relation::
 
     >>> n, k = 5, 3
@@ -10073,15 +10140,15 @@
 
 where `P` is the period of the wave and `A` is the amplitude.
 
 **Examples**
 
 Square wave with period = 2, amplitude = 1 ::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, squarew
     >>> mp.dps = 25; mp.pretty = True
     >>> squarew(0,1,2)
     1.0
     >>> squarew(0.5,1,2)
     1.0
     >>> squarew(1,1,2)
     -1.0
@@ -10100,15 +10167,15 @@
 where :math:`\operatorname{frac}\left(\frac{t}{T}\right) = \frac{t}{T}-\left\lfloor{\frac{t}{T}}\right\rfloor`
 , `P` is the period of the wave, and `A` is the amplitude.
 
 **Examples**
 
 Triangle wave with period = 2, amplitude = 1 ::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, trianglew
     >>> mp.dps = 25; mp.pretty = True
     >>> trianglew(0,1,2)
     0.0
     >>> trianglew(0.25,1,2)
     0.5
     >>> trianglew(0.5,1,2)
     1.0
@@ -10129,15 +10196,15 @@
 where :math:`\operatorname{frac}\left(\frac{t}{T}\right) = \frac{t}{T}-\left\lfloor{\frac{t}{T}}\right\rfloor`,
 `P` is the period of the wave, and `A` is the amplitude.
 
 **Examples**
 
 Sawtooth wave with period = 2, amplitude = 1 ::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, sawtoothw
     >>> mp.dps = 25; mp.pretty = True
     >>> sawtoothw(0,1,2)
     0.0
     >>> sawtoothw(0.5,1,2)
     0.25
     >>> sawtoothw(1,1,2)
     0.5
@@ -10155,15 +10222,15 @@
 
 where `A` is the amplitude.
 
 **Examples**
 
 Unit triangle with amplitude = 1 ::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, unit_triangle
     >>> mp.dps = 25; mp.pretty = True
     >>> unit_triangle(-1,1)
     0.0
     >>> unit_triangle(-0.5,1)
     0.5
     >>> unit_triangle(0,1)
     1.0
@@ -10181,15 +10248,15 @@
 
 where `A` is the amplitude.
 
 **Examples**
 
 Sigmoid function with amplitude = 1 ::
 
-    >>> from mpmath import *
+    >>> from mpmath import mp, sigmoid
     >>> mp.dps = 25; mp.pretty = True
     >>> sigmoid(-1,1)
     0.2689414213699951207488408
     >>> sigmoid(-0.5,1)
     0.3775406687981454353610994
     >>> sigmoid(0,1)
     0.5
```

### Comparing `mpmath-1.3.0/mpmath/functions/bessel.py` & `mpmath-1.4.0a0/mpmath/functions/bessel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ..libmp.backend import MPQ
 from .functions import defun, defun_wrapped
 
 @defun
 def j0(ctx, x):
     """Computes the Bessel function `J_0(x)`. See :func:`~mpmath.besselj`."""
     return ctx.besselj(0, x)
 
@@ -146,15 +147,17 @@
         ctx.prec -= d
     # TODO: avoid cancellation for imaginary arguments
     cos, sin = ctx.cospi_sinpi(n)
     return (ctx.besselj(n,z,derivative,**kwargs)*cos - \
         ctx.besselj(-n,z,derivative,**kwargs))/sin
 
 @defun_wrapped
-def besselk(ctx, n, z, **kwargs):
+def besselk(ctx, n, z, derivative=0, **kwargs):
+    if derivative:
+        raise NotImplementedError
     if not z:
         return ctx.inf
     M = ctx.mag(z)
     if M < 1:
         # Represent as limit definition
         def h(n):
             r = (z/2)**2
@@ -255,15 +258,15 @@
         return [([z/2, 0.5*ctx.sqrt(ctx.pi)], [n+1, -1], [], [n+1.5], [1], [1.5, n+1.5], (z/2)**2)]
     return ctx.hypercomb(h, [n], **kwargs)
 
 def _anger(ctx,which,v,z,**kwargs):
     v = ctx._convert_param(v)[0]
     z = ctx.convert(z)
     def h(v):
-        b = ctx.mpq_1_2
+        b = MPQ(1,2)
         u = v*b
         m = b*3
         a1,a2,b1,b2 = m-u, m+u, 1-u, 1+u
         c, s = ctx.cospi_sinpi(u)
         if which == 0:
             A, B = [b*z, s], [c]
         if which == 1:
@@ -284,33 +287,33 @@
 
 @defun
 def lommels1(ctx, u, v, z, **kwargs):
     u = ctx._convert_param(u)[0]
     v = ctx._convert_param(v)[0]
     z = ctx.convert(z)
     def h(u,v):
-        b = ctx.mpq_1_2
+        b = MPQ(1,2)
         w = ctx.square_exp_arg(z, mult=-0.25)
         return ([u-v+1, u+v+1, z], [-1, -1, u+1], [], [], [1], \
             [b*(u-v+3),b*(u+v+3)], w),
     return ctx.hypercomb(h, [u,v], **kwargs)
 
 @defun
 def lommels2(ctx, u, v, z, **kwargs):
     u = ctx._convert_param(u)[0]
     v = ctx._convert_param(v)[0]
     z = ctx.convert(z)
     # Asymptotic expansion (GR p. 947) -- need to be careful
     # not to use for small arguments
     # def h(u,v):
-    #    b = ctx.mpq_1_2
+    #    b = MPQ(1,2)
     #    w = -(z/2)**(-2)
     #    return ([z], [u-1], [], [], [b*(1-u+v)], [b*(1-u-v)], w),
     def h(u,v):
-        b = ctx.mpq_1_2
+        b = MPQ(1,2)
         w = ctx.square_exp_arg(z, mult=-0.25)
         T1 = [u-v+1, u+v+1, z], [-1, -1, u+1], [], [], [1], [b*(u-v+3),b*(u+v+3)], w
         T2 = [2, z], [u+v-1, -v], [v, b*(u+v+1)], [b*(v-u+1)], [], [1-v], w
         T3 = [2, z], [u-v-1, v], [-v, b*(u-v+1)], [b*(1-u-v)], [], [1+v], w
         #c1 = ctx.cospi((u-v)*b)
         #c2 = ctx.cospi((u+v)*b)
         #s = ctx.sinpi(v)
@@ -421,15 +424,15 @@
 
 # Derivatives at z = 0
 # TODO: could be expressed more elegantly using triple factorials
 def _airyderiv_0(ctx, z, n, ntype, which):
     if ntype == 'Z':
         if n < 0:
             return z
-        r = ctx.mpq_1_3
+        r = MPQ(1,3)
         prec = ctx.prec
         try:
             ctx.prec += 10
             v = ctx.gamma((n+1)*r) * ctx.power(3,n*r) / ctx.pi
             if which == 0:
                 v *= ctx.sinpi(2*(n+1)*r)
                 v /= ctx.power(3,'2/3')
@@ -485,27 +488,27 @@
                 # http://functions.wolfram.com/03.07.26.0001.01
                 else:
                     ctx.prec += extraprec
                     w = z**3 / 9
                     ctx.prec -= extraprec
                     C1 = _airyai_C1(ctx) * 0.5
                     C2 = _airyai_C2(ctx)
-                    T1 = [C1,z],[1,2],[],[],[],[ctx.mpq_5_3],w
-                    T2 = [C2],[1],[],[],[],[ctx.mpq_1_3],w
+                    T1 = [C1,z],[1,2],[],[],[],[MPQ(5,3)],w
+                    T2 = [C2],[1],[],[],[],[MPQ(1,3)],w
                     return T1, T2
             return ctx.hypercomb(h, [], **kwargs)
         else:
             if z == 0:
                 return _airyderiv_0(ctx, z, n, ntype, 0)
             # http://functions.wolfram.com/03.05.20.0004.01
             def h(n):
                 ctx.prec += extraprec
                 w = z**3/9
                 ctx.prec -= extraprec
-                q13,q23,q43 = ctx.mpq_1_3, ctx.mpq_2_3, ctx.mpq_4_3
+                q13,q23,q43 = MPQ(1,3), MPQ(2,3), MPQ(4,3)
                 a1=q13; a2=1; b1=(1-n)*q13; b2=(2-n)*q13; b3=1-n*q13
                 T1 = [3, z], [n-q23, -n], [a1], [b1,b2,b3], \
                     [a1,a2], [b1,b2,b3], w
                 a1=q23; b1=(2-n)*q13; b2=1-n*q13; b3=(4-n)*q13
                 T2 = [3, z, -z], [n-q43, -n, 1], [a1], [b1,b2,b3], \
                     [a1,a2], [b1,b2,b3], w
                 return T1, T2
@@ -526,16 +529,16 @@
                 return ([C],[1],[],[],[(1,6),(5,6)],[],r),
             else:
                 ctx.prec += extraprec
                 w = z**3 / 9
                 ctx.prec -= extraprec
                 C1 = _airyai_C1(ctx)
                 C2 = _airyai_C2(ctx)
-                T1 = [C1],[1],[],[],[],[ctx.mpq_2_3],w
-                T2 = [z*C2],[1],[],[],[],[ctx.mpq_4_3],w
+                T1 = [C1],[1],[],[],[],[MPQ(2,3)],w
+                T2 = [z*C2],[1],[],[],[],[MPQ(4,3)],w
                 return T1, T2
         return ctx.hypercomb(h, [], **kwargs)
 
 @defun
 def airybi(ctx, z, derivative=0, **kwargs):
     z = ctx.convert(z)
     if derivative:
@@ -570,28 +573,28 @@
             # http://functions.wolfram.com/03.08.26.0001.01
             def h():
                 ctx.prec += extraprec
                 w = z**3 / 9
                 ctx.prec -= extraprec
                 C1 = _airybi_C1(ctx)*0.5
                 C2 = _airybi_C2(ctx)
-                T1 = [C1,z],[1,2],[],[],[],[ctx.mpq_5_3],w
-                T2 = [C2],[1],[],[],[],[ctx.mpq_1_3],w
+                T1 = [C1,z],[1,2],[],[],[],[MPQ(5,3)],w
+                T2 = [C2],[1],[],[],[],[MPQ(1,3)],w
                 return T1, T2
             return ctx.hypercomb(h, [], **kwargs)
         else:
             if z == 0:
                 return _airyderiv_0(ctx, z, n, ntype, 1)
             def h(n):
                 ctx.prec += extraprec
                 w = z**3/9
                 ctx.prec -= extraprec
-                q13,q23,q43 = ctx.mpq_1_3, ctx.mpq_2_3, ctx.mpq_4_3
-                q16 = ctx.mpq_1_6
-                q56 = ctx.mpq_5_6
+                q13,q23,q43 = MPQ(1,3), MPQ(2,3), MPQ(4,3)
+                q16 = MPQ(1,6)
+                q56 = MPQ(5,6)
                 a1=q13; a2=1; b1=(1-n)*q13; b2=(2-n)*q13; b3=1-n*q13
                 T1 = [3, z], [n-q16, -n], [a1], [b1,b2,b3], \
                     [a1,a2], [b1,b2,b3], w
                 a1=q23; b1=(2-n)*q13; b2=1-n*q13; b3=(4-n)*q13
                 T2 = [3, z], [n-q56, 1-n], [a1], [b1,b2,b3], \
                     [a1,a2], [b1,b2,b3], w
                 return T1, T2
@@ -602,39 +605,39 @@
     else:
         def h():
             ctx.prec += extraprec
             w = z**3 / 9
             ctx.prec -= extraprec
             C1 = _airybi_C1(ctx)
             C2 = _airybi_C2(ctx)
-            T1 = [C1],[1],[],[],[],[ctx.mpq_2_3],w
-            T2 = [z*C2],[1],[],[],[],[ctx.mpq_4_3],w
+            T1 = [C1],[1],[],[],[],[MPQ(2,3)],w
+            T2 = [z*C2],[1],[],[],[],[MPQ(4,3)],w
             return T1, T2
         return ctx.hypercomb(h, [], **kwargs)
 
 def _airy_zero(ctx, which, k, derivative, complex=False):
     # Asymptotic formulas are given in DLMF section 9.9
     def U(t): return t**(2/3.)*(1-7/(t**2*48))
     def T(t): return t**(2/3.)*(1+5/(t**2*48))
     k = int(k)
     if k < 1:
         raise ValueError("k cannot be less than 1")
-    if not derivative in (0,1):
+    if derivative not in (0, 1):
         raise ValueError("Derivative should lie between 0 and 1")
     if which == 0:
         if derivative:
             return ctx.findroot(lambda z: ctx.airyai(z,1),
                 -U(3*ctx.pi*(4*k-3)/8))
         return ctx.findroot(ctx.airyai, -T(3*ctx.pi*(4*k-1)/8))
-    if which == 1 and complex == False:
+    if which == 1 and complex is False:
         if derivative:
             return ctx.findroot(lambda z: ctx.airybi(z,1),
                 -U(3*ctx.pi*(4*k-1)/8))
         return ctx.findroot(ctx.airybi, -T(3*ctx.pi*(4*k-3)/8))
-    if which == 1 and complex == True:
+    if which == 1 and complex is True:
         if derivative:
             t = 3*ctx.pi*(4*k-3)/8 + 0.75j*ctx.ln2
             s = ctx.expjpi(ctx.mpf(1)/3) * T(t)
             return ctx.findroot(lambda z: ctx.airybi(z,1), s)
         t = 3*ctx.pi*(4*k-1)/8 + 0.75j*ctx.ln2
         s = ctx.expjpi(ctx.mpf(1)/3) * U(t)
         return ctx.findroot(ctx.airybi, s)
@@ -682,15 +685,15 @@
         if which == 1:
             A *= 2
             B *= -1
         ctx.prec += extraprec
         w = z**3/9
         ctx.prec -= extraprec
         T1 = [A], [1], [], [], [], [], 0
-        T2 = [B,z], [-1,2], [], [], [1], [ctx.mpq_4_3,ctx.mpq_5_3], w
+        T2 = [B,z], [-1,2], [], [], [1], [MPQ(4,3),MPQ(5,3)], w
         return T1, T2
     return ctx.hypercomb(h, [], **kwargs)
 
 @defun
 def scorergi(ctx, z, **kwargs):
     return _scorer(ctx, z, 0, kwargs)
 
@@ -857,15 +860,15 @@
         v = ctx.mpf(v)
         m = int(m)
         prime = int(prime)
         if v < 0:
             raise ValueError("v cannot be negative")
         if m < 1:
             raise ValueError("m cannot be less than 1")
-        if not prime in (0,1):
+        if prime not in (0, 1):
             raise ValueError("prime should lie between 0 and 1")
         if kind == 1:
             if prime: f = lambda x: ctx.besselj(v,x,derivative=1)
             else:     f = lambda x: ctx.besselj(v,x)
         if kind == 2:
             if prime: f = lambda x: ctx.bessely(v,x,derivative=1)
             else:     f = lambda x: ctx.bessely(v,x)
@@ -926,15 +929,15 @@
 
         j_{\nu,1} < j_{\nu+1,2} < j_{\nu,2} < j_{\nu+1,2} < j_{\nu,3} < \cdots
 
     **Examples**
 
     Initial zeros of the Bessel functions `J_0(z), J_1(z), J_2(z)`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, besseljzero, mpf, gamma, nprod, inf, besselj
         >>> mp.dps = 25; mp.pretty = True
         >>> besseljzero(0,1); besseljzero(0,2); besseljzero(0,3)
         2.404825557695772768621632
         5.520078110286310649596604
         8.653727912911012216954199
         >>> besseljzero(1,1); besseljzero(1,2); besseljzero(1,3)
         3.831705970207512315614436
@@ -1033,15 +1036,15 @@
 
         y_{\nu,1} < y_{\nu+1,2} < y_{\nu,2} < y_{\nu+1,2} < y_{\nu,3} < \cdots
 
     **Examples**
 
     Initial zeros of the Bessel functions `Y_0(z), Y_1(z), Y_2(z)`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, besselyzero
         >>> mp.dps = 25; mp.pretty = True
         >>> besselyzero(0,1); besselyzero(0,2); besselyzero(0,3)
         0.8935769662791675215848871
         3.957678419314857868375677
         7.086051060301772697623625
         >>> besselyzero(1,1); besselyzero(1,2); besselyzero(1,3)
         2.197141326031017035149034
```

### Comparing `mpmath-1.3.0/mpmath/functions/elliptic.py` & `mpmath-1.4.0a0/mpmath/functions/elliptic.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 from .functions import defun, defun_wrapped
 
 @defun_wrapped
 def eta(ctx, tau):
     r"""
     Returns the Dedekind eta function of tau in the upper half-plane.
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, eta, gamma, pi, sqrt, diff, chop, exp
         >>> mp.dps = 25; mp.pretty = True
         >>> eta(1j); gamma(0.25) / (2*pi**0.75)
         (0.7682254223260566590025942 + 0.0j)
         0.7682254223260566590025942
         >>> tau = sqrt(2) + sqrt(5)*1j
         >>> eta(-1/tau); sqrt(-1j*tau) * eta(tau)
         (0.9022859908439376463573294 + 0.07985093673948098408048575j)
@@ -97,15 +97,15 @@
         return m
     if m == ctx.one:
         return m
     if ctx.isnan(m):
         return m
     if ctx.isinf(m):
         if m == ctx.ninf:
-            return type(m)(-1)
+            return -ctx.one
         else:
             return ctx.mpc(-1)
     a = ctx.ellipk(ctx.one-m)
     b = ctx.ellipk(m)
     v = ctx.exp(-ctx.pi*a/b)
     if not ctx._im(m) and ctx._re(m) < 1:
         if ctx._is_real_type(m):
@@ -117,15 +117,15 @@
     return v
 
 @defun_wrapped
 def qfrom(ctx, q=None, m=None, k=None, tau=None, qbar=None):
     r"""
     Returns the elliptic nome `q`, given any of `q, m, k, \tau, \bar{q}`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, qfrom, mfrom, kfrom, taufrom, qbarfrom
         >>> mp.dps = 25; mp.pretty = True
         >>> qfrom(q=0.25)
         0.25
         >>> qfrom(m=mfrom(q=0.25))
         0.25
         >>> qfrom(k=kfrom(q=0.25))
         0.25
@@ -148,15 +148,16 @@
 
 @defun_wrapped
 def qbarfrom(ctx, q=None, m=None, k=None, tau=None, qbar=None):
     r"""
     Returns the number-theoretic nome `\bar q`, given any of
     `q, m, k, \tau, \bar{q}`::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, qbarfrom, qfrom, extraprec, mfrom,
+        ...                     kfrom, taufrom)
         >>> mp.dps = 25; mp.pretty = True
         >>> qbarfrom(qbar=0.25)
         0.25
         >>> qbarfrom(q=qfrom(qbar=0.25))
         0.25
         >>> qbarfrom(m=extraprec(20)(mfrom)(qbar=0.25))  # ill-conditioned
         0.25
@@ -179,15 +180,15 @@
 
 @defun_wrapped
 def taufrom(ctx, q=None, m=None, k=None, tau=None, qbar=None):
     r"""
     Returns the elliptic half-period ratio `\tau`, given any of
     `q, m, k, \tau, \bar{q}`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, taufrom, qfrom, mfrom, kfrom, qbarfrom
         >>> mp.dps = 25; mp.pretty = True
         >>> taufrom(tau=0.5j)
         (0.0 + 0.5j)
         >>> taufrom(q=qfrom(tau=0.5j))
         (0.0 + 0.5j)
         >>> taufrom(m=mfrom(tau=0.5j))
         (0.0 + 0.5j)
@@ -213,15 +214,15 @@
 
 @defun_wrapped
 def kfrom(ctx, q=None, m=None, k=None, tau=None, qbar=None):
     r"""
     Returns the elliptic modulus `k`, given any of
     `q, m, k, \tau, \bar{q}`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, kfrom, mfrom, qfrom, taufrom, qbarfrom
         >>> mp.dps = 25; mp.pretty = True
         >>> kfrom(k=0.25)
         0.25
         >>> kfrom(m=mfrom(k=0.25))
         0.25
         >>> kfrom(q=qfrom(k=0.25))
         0.25
@@ -258,15 +259,15 @@
 
 @defun_wrapped
 def mfrom(ctx, q=None, m=None, k=None, tau=None, qbar=None):
     r"""
     Returns the elliptic parameter `m`, given any of
     `q, m, k, \tau, \bar{q}`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, mfrom, qfrom, kfrom, taufrom, qbarfrom, taylor
         >>> mp.dps = 25; mp.pretty = True
         >>> mfrom(m=0.25)
         0.25
         >>> mfrom(q=qfrom(m=0.25))
         0.25
         >>> mfrom(k=kfrom(m=0.25))
         0.25
@@ -397,15 +398,16 @@
     .. literalinclude :: /plots/kleinj2.py
     .. image :: /plots/kleinj2.png
 
     **Examples**
 
     Verifying the functional equation `J(\tau) = J(\tau+1) = J(-\tau^{-1})`::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, j, kleinj, taylor, sqrt, extraprec,
+        ...                     chop, identify, cbrt)
         >>> mp.dps = 25; mp.pretty = True
         >>> tau = 0.625+0.75*j
         >>> tau = 0.625+0.75*j
         >>> kleinj(tau)
         (-0.1507492166511182267125242 + 0.07595948379084571927228948j)
         >>> kleinj(tau+1)
         (-0.1507492166511182267125242 + 0.07595948379084571927228948j)
@@ -643,15 +645,16 @@
     and as `t \to 0` non-principal branches are chosen as necessary so as to
     make the integrand continuous.
 
     **Examples**
 
     Some basic values and limits::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, elliprf, pi, inf, ellipk, ellipe,
+        ...                     elliprd, mpf, quad, extradps, sqrt, j, gamma)
         >>> mp.dps = 25; mp.pretty = True
         >>> elliprf(0,1,1); pi/2
         1.570796326794896619231322
         1.570796326794896619231322
         >>> elliprf(0,1,inf)
         0.0
         >>> elliprf(1,1,1)
@@ -768,15 +771,16 @@
             \cosh^{-1}\left(\sqrt{\dfrac{x}{y}}\right),  & x > y \\
         \end{cases}.
 
     **Examples**
 
     Some special values and limits::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, elliprc, pi, acosh, sqrt, acos,
+        ...                     extradps, quad, inf, j)
         >>> mp.dps = 25; mp.pretty = True
         >>> elliprc(1,2)*4; elliprc(0,1)*2; +pi
         3.141592653589793238462643
         3.141592653589793238462643
         3.141592653589793238462643
         >>> elliprc(1,0)
         +inf
@@ -832,15 +836,16 @@
     is defined so as to be continuous along the path of integration for
     complex values of the arguments.
 
     **Examples**
 
     Some values and limits::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, elliprj, sqrt, gamma, pi, chop, mpf,
+        ...                     quad, inf, j)
         >>> mp.dps = 25; mp.pretty = True
         >>> elliprj(1,1,1,1)
         1.0
         >>> elliprj(2,2,2,2); 1/(2*sqrt(2))
         0.3535533905932737622004222
         0.3535533905932737622004222
         >>> elliprj(0,1,2,2)
@@ -902,15 +907,16 @@
     of the third kind or Carlson elliptic integral of the
     second kind `R_D(x,y,z) = R_J(x,y,z,z)`.
 
     See :func:`~mpmath.elliprj` for additional information.
 
     **Examples**
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, elliprd, elliprj, extradps, quad, sqrt,
+        ...                     gamma, pi)
         >>> mp.dps = 25; mp.pretty = True
         >>> elliprd(1,2,3)
         0.2904602810289906442326534
         >>> elliprj(1,2,3,3)
         0.2904602810289906442326534
 
     The so-called *second lemniscate constant*, a transcendental number::
@@ -937,15 +943,15 @@
             \frac{t}{\sqrt{(t+x)(t+y)(t+z)}}
             \left( \frac{x}{t+x} + \frac{y}{t+y} + \frac{z}{t+z}\right) dt.
 
     **Examples**
 
     Evaluation for real and complex arguments::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, pi, elliprg, chop, fp, nprint, mpf, j
         >>> mp.dps = 25; mp.pretty = True
         >>> elliprg(0,1,1)*4; +pi
         3.141592653589793238462643
         3.141592653589793238462643
         >>> elliprg(0,0.5,1)
         0.6753219405238377512600874
         >>> chop(elliprg(1+j, 1-j, 2))
@@ -1023,15 +1029,16 @@
     .. literalinclude :: /plots/ellipf.py
     .. image :: /plots/ellipf.png
 
     **Examples**
 
     Basic values and limits::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, ellipf, log, sec, tan, pi, eps, ellipk,
+        ...                     sin, appellf1, quad)
         >>> mp.dps = 25; mp.pretty = True
         >>> ellipf(0,1)
         0.0
         >>> ellipf(0,0)
         0.0
         >>> ellipf(1,0); ellipf(2+3j,0)
         1.0
@@ -1143,15 +1150,16 @@
     .. literalinclude :: /plots/ellipe.py
     .. image :: /plots/ellipe.png
 
     **Examples for the complete integral**
 
     Basic values and limits::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, ellipe, inf, quad, sqrt, sin, pi,
+        ...                     hyp2f1, appellf1)
         >>> mp.dps = 25; mp.pretty = True
         >>> ellipe(0)
         1.570796326794896619231322
         >>> ellipe(1)
         1.0
         >>> ellipe(-1)
         1.910098894513856008952381
@@ -1302,15 +1310,16 @@
     .. literalinclude :: /plots/ellippi.py
     .. image :: /plots/ellippi.png
 
     **Examples for the complete integral**
 
     Some basic values and limits::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, ellippi, ellipk, inf, pi, sqrt, ellipe,
+        ...                     log, sec, tan, ellipf)
         >>> mp.dps = 25; mp.pretty = True
         >>> ellippi(0,-5); ellipk(-5)
         0.9555039270640439337379334
         0.9555039270640439337379334
         >>> ellippi(inf,2)
         0.0
         >>> ellippi(2,inf)
```

### Comparing `mpmath-1.3.0/mpmath/functions/expintegrals.py` & `mpmath-1.4.0a0/mpmath/functions/expintegrals.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,30 +27,30 @@
     if ctx._is_real_type(z):
         try:
             return ctx._erf(z)
         except NotImplementedError:
             pass
     if ctx._is_complex_type(z) and not z.imag:
         try:
-            return type(z)(ctx._erf(z.real))
+            return ctx.mpc(ctx._erf(z.real))
         except NotImplementedError:
             pass
     return ctx._erf_complex(z)
 
 @defun
 def erfc(ctx, z):
     z = ctx.convert(z)
     if ctx._is_real_type(z):
         try:
             return ctx._erfc(z)
         except NotImplementedError:
             pass
     if ctx._is_complex_type(z) and not z.imag:
         try:
-            return type(z)(ctx._erfc(z.real))
+            return ctx.mpc(ctx._erfc(z.real))
         except NotImplementedError:
             pass
     return ctx._erfc_complex(z)
 
 @defun
 def square_exp_arg(ctx, z, mult=1, reciprocal=False):
     prec = ctx.prec*4+20
@@ -104,15 +104,15 @@
         return ctx.erfc(-a)/2
     else:
         return (1+ctx.erf(a))/2
 
 @defun_wrapped
 def betainc(ctx, a, b, x1=0, x2=1, regularized=False):
     if x1 == x2:
-        v = 0
+        v = ctx.zero
     elif not x1:
         if x1 == 0 and x2 == 1:
             v = ctx.beta(a, b)
         else:
             v = x2**a * ctx.hyp2f1(a, 1-b, a+1, x2) / a
     else:
         m, d = ctx.nint_distance(a)
@@ -162,40 +162,44 @@
     if ctx.re(a) > ctx.re(b):
         return -ctx.gammainc(z, b, a, regularized)
     # Generalized gamma
     if upper_modified and lower_modified:
         return +ctx._gamma3(z, a, b, regularized)
     # Upper gamma
     elif lower_modified:
-        return ctx._upper_gamma(z, a, regularized)
+        return ctx.upper_gamma(z, a, regularized)
     # Lower gamma
     elif upper_modified:
-        return ctx._lower_gamma(z, b, regularized)
+        return ctx.lower_gamma(z, b, regularized)
 
 @defun
-def _lower_gamma(ctx, z, b, regularized=False):
+def lower_gamma(ctx, z, b, regularized=False):
+    z = ctx.convert(z)
+    b = ctx.convert(b)
     # Pole
     if ctx.isnpint(z):
-        return type(z)(ctx.inf)
+        return ctx.inf
     G = [z] * regularized
     negb = ctx.fneg(b, exact=True)
     def h(z):
         T1 = [ctx.exp(negb), b, z], [1, z, -1], [], G, [1], [1+z], b
         return (T1,)
     return ctx.hypercomb(h, [z])
 
 @defun
-def _upper_gamma(ctx, z, a, regularized=False):
+def upper_gamma(ctx, z, a, regularized=False):
+    z = ctx.convert(z)
+    a = ctx.convert(a)
     # Fast integer case, when available
     if ctx.isint(z):
         try:
             if regularized:
                 # Gamma pole
                 if ctx.isnpint(z):
-                    return type(z)(ctx.zero)
+                    return ctx.zero
                 orig = ctx.prec
                 try:
                     ctx.prec += 10
                     return ctx._gamma_upper_int(z, a) / ctx.gamma(z)
                 finally:
                     ctx.prec = orig
             else:
@@ -259,22 +263,22 @@
         return z*n
     if z == ctx.inf:
         return 1/z
     if z == 0:
         # integral from 1 to infinity of t^n
         if ctx.re(n) <= 1:
             # TODO: reasonable sign of infinity
-            return type(z)(ctx.inf)
+            return ctx.inf
         else:
             return ctx.one/(n-1)
     if n == 0:
         return ctx.exp(-z)/z
     if n == -1:
         return ctx.exp(-z)*(z+1)/z**2
-    return z**(n-1) * ctx.gammainc(1-n, z)
+    return z**(n-1) * ctx.upper_gamma(1-n, z)
 
 @defun_wrapped
 def li(ctx, z, offset=False):
     if offset:
         if z == 2:
             return ctx.zero
         return ctx.ei(ctx.ln(z)) - ctx.ei(ctx.ln2)
```

### Comparing `mpmath-1.3.0/mpmath/functions/factorials.py` & `mpmath-1.4.0a0/mpmath/functions/factorials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ..libmp.backend import xrange
 from .functions import defun, defun_wrapped
 
 @defun
 def gammaprod(ctx, a, b, _infsign=False):
     a = [ctx.convert(x) for x in a]
     b = [ctx.convert(x) for x in b]
     poles_num = []
@@ -118,15 +117,15 @@
     z -= 1
     s = ctx.mpf(1)/12
     s -= ctx.log(ctx.glaisher)
     s += z*ctx.log(2*ctx.pi)/2
     s += (z**2/2-ctx.mpf(1)/12)*ctx.log(z)
     s -= 3*z**2/4
     z2k = z2 = z**2
-    for k in xrange(1, N+1):
+    for k in range(1, N+1):
         t = ctx.bernoulli(2*k+2) / (4*k*(k+1)*z2k)
         if abs(t) < ctx.eps:
             #print k, N      # check how many terms were needed
             break
         z2k *= z2
         s += t
     #if k == N:
```

### Comparing `mpmath-1.3.0/mpmath/functions/functions.py` & `mpmath-1.4.0a0/mpmath/functions/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from ..libmp.backend import xrange
-
-class SpecialFunctions(object):
+class SpecialFunctions:
     """
     This class implements special functions using high-level code.
 
     Elementary and some other functions (e.g. gamma function, basecase
     hypergeometric series) are assumed to be predefined by the context as
     "builtins" or "low-level" functions.
     """
@@ -17,32 +15,14 @@
 
     def __init__(self):
         cls = self.__class__
         for name in cls.defined_functions:
             f, wrap = cls.defined_functions[name]
             cls._wrap_specfun(name, f, wrap)
 
-        self.mpq_1 = self._mpq((1,1))
-        self.mpq_0 = self._mpq((0,1))
-        self.mpq_1_2 = self._mpq((1,2))
-        self.mpq_3_2 = self._mpq((3,2))
-        self.mpq_1_4 = self._mpq((1,4))
-        self.mpq_1_16 = self._mpq((1,16))
-        self.mpq_3_16 = self._mpq((3,16))
-        self.mpq_5_2 = self._mpq((5,2))
-        self.mpq_3_4 = self._mpq((3,4))
-        self.mpq_7_4 = self._mpq((7,4))
-        self.mpq_5_4 = self._mpq((5,4))
-        self.mpq_1_3 = self._mpq((1,3))
-        self.mpq_2_3 = self._mpq((2,3))
-        self.mpq_4_3 = self._mpq((4,3))
-        self.mpq_1_6 = self._mpq((1,6))
-        self.mpq_5_6 = self._mpq((5,6))
-        self.mpq_5_3 = self._mpq((5,3))
-
         self._misc_const_cache = {}
 
         self._aliases.update({
             'phase' : 'arg',
             'conjugate' : 'conj',
             'nthroot' : 'root',
             'polygamma' : 'psi',
@@ -270,24 +250,20 @@
 @defun
 def fabs(ctx, x):
     return abs(ctx.convert(x))
 
 @defun
 def re(ctx, x):
     x = ctx.convert(x)
-    if hasattr(x, "real"):    # py2.5 doesn't have .real/.imag for all numbers
-        return x.real
-    return x
+    return x.real
 
 @defun
 def im(ctx, x):
     x = ctx.convert(x)
-    if hasattr(x, "imag"):    # py2.5 doesn't have .real/.imag for all numbers
-        return x.imag
-    return ctx.zero
+    return x.imag
 
 @defun
 def conj(ctx, x):
     x = ctx.convert(x)
     try:
         return x.conjugate()
     except AttributeError:
@@ -341,24 +317,19 @@
     return ctx.ln(z)
 
 import math
 import cmath
 
 def _lambertw_approx_hybrid(z, k):
     imag_sign = 0
-    if hasattr(z, "imag"):
-        x = float(z.real)
-        y = z.imag
-        if y:
-            imag_sign = (-1) ** (y < 0)
-        y = float(y)
-    else:
-        x = float(z)
-        y = 0.0
-        imag_sign = 0
+    x = float(z.real)
+    y = z.imag
+    if y:
+        imag_sign = (-1) ** (y < 0)
+    y = float(y)
     # hack to work regardless of whether Python supports -0.0
     if not y:
         y = 0.0
     z = complex(x,y)
     if k == 0:
         if -4.0 < y < 4.0 and -1.0 < x < 2.5:
             if imag_sign:
@@ -428,17 +399,17 @@
                 a = {0:ctx.mpf(2), 1:ctx.mpf(-1)}
                 if k != 0:
                     p = -p
                 s = ctx.zero
                 # The series converges, so we could use it directly, but unless
                 # *extremely* close, it is better to just use the first few
                 # terms to get a good approximation for the iteration
-                for l in xrange(max(2,cancellation)):
+                for l in range(max(2, cancellation)):
                     if l not in u:
-                        a[l] = ctx.fsum(u[j]*u[l+1-j] for j in xrange(2,l))
+                        a[l] = ctx.fsum(u[j]*u[l+1-j] for j in range(2, l))
                         u[l] = (l-1)*(u[l-2]/2+a[l-2]/4)/(l+1)-a[l]/2-u[l-1]/(l+1)
                     term = u[l] * p**l
                     s += term
                     if ctx.mag(term) < -tol:
                         return s, True
                     l += 1
                 ctx.prec += cancellation//2
@@ -470,15 +441,15 @@
     ctx.prec += 20 + ctx.mag(k or 1)
     wp = ctx.prec
     tol = wp - 5
     w, done = _lambertw_series(ctx, z, k, tol)
     if not done:
         # Use Halley iteration to solve w*exp(w) = z
         two = ctx.mpf(2)
-        for i in xrange(100):
+        for i in range(100):
             ew = ctx.exp(w)
             wew = w*ew
             wewz = wew-z
             wn = w - wewz/(wew+ew-(w+two)*wewz/(two*w+two))
             if ctx.mag(wn-w) <= ctx.mag(wn) - tol:
                 w = wn
                 break
@@ -491,15 +462,15 @@
 
 @defun_wrapped
 def bell(ctx, n, x=1):
     x = ctx.convert(x)
     if not n:
         if ctx.isnan(x):
             return x
-        return type(x)(1)
+        return ctx.one
     if ctx.isinf(x) or ctx.isinf(n) or ctx.isnan(x) or ctx.isnan(n):
         return x**n
     if n == 1: return x
     if n == 2: return x*(x+1)
     if x == 0: return ctx.sincpi(n)
     return _polyexp(ctx, n, x, True) / ctx.exp(x)
 
@@ -572,15 +543,15 @@
 def mangoldt(ctx, n):
     r"""
     Evaluates the von Mangoldt function `\Lambda(n) = \log p`
     if `n = p^k` a power of a prime, and `\Lambda(n) = 0` otherwise.
 
     **Examples**
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, mangoldt, fsum
         >>> mp.dps = 25; mp.pretty = True
         >>> [mangoldt(n) for n in range(-2,3)]
         [0.0, 0.0, 0.0, 0.0, 0.6931471805599453094172321]
         >>> mangoldt(6)
         0.0
         >>> mangoldt(7)
         1.945910149055313305105353
```

### Comparing `mpmath-1.3.0/mpmath/functions/hypergeometric.py` & `mpmath-1.4.0a0/mpmath/functions/hypergeometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..libmp.backend import xrange
+from ..libmp.backend import MPQ
 from .functions import defun, defun_wrapped
 
 def _check_need_perturb(ctx, terms, prec, discard_known_zeros):
     perturb = recompute = False
     extraprec = 0
     discard = []
     for term_index, term in enumerate(terms):
@@ -193,14 +193,16 @@
 
 @defun
 def hyper(ctx, a_s, b_s, z, **kwargs):
     """
     Hypergeometric function, general case.
     """
     z = ctx.convert(z)
+    if ctx.isnan(z):
+        return ctx.nan
     p = len(a_s)
     q = len(b_s)
     a_s = [ctx._convert_param(a) for a in a_s]
     b_s = [ctx._convert_param(b) for b in b_s]
     # Reduce degree by eliminating common parameters
     if kwargs.get('eliminate', True):
         elim_nonpositive = kwargs.get('eliminate_all', False)
@@ -286,18 +288,18 @@
             orig = ctx.prec
             try:
                 ctx.prec += 12 + magz//2
                 def h():
                     w = ctx.sqrt(-z)
                     jw = ctx.j*w
                     u = 1/(4*jw)
-                    c = ctx.mpq_1_2 - b
+                    c = MPQ(1,2) - b
                     E = ctx.exp(2*jw)
-                    T1 = ([-jw,E], [c,-1], [], [], [b-ctx.mpq_1_2, ctx.mpq_3_2-b], [], -u)
-                    T2 = ([jw,E], [c,1], [], [], [b-ctx.mpq_1_2, ctx.mpq_3_2-b], [], u)
+                    T1 = ([-jw,E], [c,-1], [], [], [b-MPQ(1,2), MPQ(3,2)-b], [], -u)
+                    T2 = ([jw,E], [c,1], [], [], [b-MPQ(1,2), MPQ(3,2)-b], [], u)
                     return T1, T2
                 v = ctx.hypercomb(h, [], force_series=True)
                 v = ctx.gamma(b)/(2*ctx.sqrt(ctx.pi))*v
             finally:
                 ctx.prec = orig
             if ctx._is_real_type(b) and ctx._is_real_type(z):
                 v = ctx._re(v)
@@ -359,16 +361,16 @@
         e = ctx.mpf(1)
         f = ctx.mpf(0)
         k = 0
         # Common subexpression elimination, unfortunately making
         # things a bit unreadable. The formula is quite messy to begin
         # with, though...
         abz = a*b*z
-        ch = c * ctx.mpq_1_2
-        c1h = (c+1) * ctx.mpq_1_2
+        ch = c * MPQ(1,2)
+        c1h = (c+1) * MPQ(1,2)
         nz = 1-z
         g = z/nz
         abg = a*b*g
         cba = c-b-a
         z2 = z-2
         tol = -ctx.prec - 10
         nstr = ctx.nstr
@@ -434,28 +436,33 @@
             # Pole in series
             return ctx.inf
 
     absz = abs(z)
 
     # Fast case: standard series converges rapidly,
     # possibly in finitely many terms
-    if absz <= 0.8 or (ctx.isint(a) and a <= 0 and a >= -1000) or \
-                      (ctx.isint(b) and b <= 0 and b >= -1000):
-        return ctx.hypsum(2, 1, (atype, btype, ctype), [a, b, c], z, **kwargs)
+    if ctx.isfinite(z) and (absz <= 0.8 or
+                            (ctx.isint(a) and -1000 <= a <= 0) or
+                            (ctx.isint(b) and -1000 <= b <= 0)):
+        try:
+            return ctx.hypsum(2, 1, (atype, btype, ctype), [a, b, c], z, **kwargs)
+        except ctx.NoConvergence:
+            if kwargs.get('force_series', False):
+                raise
 
     orig = ctx.prec
     try:
         ctx.prec += 10
 
         # Use 1/z transformation
         if absz >= 1.3:
             def h(a,b):
-                t = ctx.mpq_1-c; ab = a-b; rz = 1/z
-                T1 = ([-z],[-a], [c,-ab],[b,c-a], [a,t+a],[ctx.mpq_1+ab],  rz)
-                T2 = ([-z],[-b], [c,ab],[a,c-b], [b,t+b],[ctx.mpq_1-ab],  rz)
+                t = MPQ(1)-c; ab = a-b; rz = 1/z
+                T1 = ([-z],[-a], [c,-ab],[b,c-a], [a,t+a],[MPQ(1)+ab],  rz)
+                T2 = ([-z],[-b], [c,ab],[a,c-b], [b,t+b],[MPQ(1)-ab],  rz)
                 return T1, T2
             v = ctx.hypercomb(h, [a,b], **kwargs)
 
         # Use 1-z transformation
         elif abs(1-z) <= 0.75:
             def h(a,b):
                 t = c-a-b; ca = c-a; cb = c-b; rz = 1-z
@@ -555,16 +562,16 @@
                 for a in a_s: t *= ctx.rf(a,kk)
                 for b in b_s: t /= ctx.rf(b,kk)
                 return t
             if k in _cache:
                 return _cache[k]
             t = term(k-1)
             m = k-1
-            for j in xrange(p): t *= (a_s[j]+m)
-            for j in xrange(q): t /= (b_s[j]+m)
+            for j in range(p): t *= (a_s[j]+m)
+            for j in range(q): t /= (b_s[j]+m)
             t *= z
             t /= k
             _cache[k] = t
             return t
 
         sum_method = kwargs.get('sum_method', 'r+s+e')
 
@@ -632,16 +639,16 @@
                 yield v
 
         tol = ctx.eps / 1024
         prec = ctx.prec
         try:
             trunc = 50 * ctx.dps
             ctx.prec += 20
-            for i in xrange(5):
-                head = ctx.fsum(term(k) for k in xrange(trunc))
+            for i in range(5):
+                head = ctx.fsum(term(k) for k in range(trunc))
                 tail, err = ctx.sumem(term, [trunc, ctx.inf], tol=tol,
                     adiffs=hyper_diffs(trunc),
                     verbose=kwargs.get('verbose'),
                     error=True,
                     _fast_abort=True)
                 if err < tol:
                     v = head + tail
@@ -707,15 +714,15 @@
             for a in a_s: t *= (a+(k-1))
             for b in b_s: t /= (b+(k-1))
             t *= z
             t /= k
             cache[k] = t
             return t
         s = ctx.one
-        for k in xrange(1, ctx.prec):
+        for k in range(1, ctx.prec):
             t = term(k)
             s += t
             if abs(t) <= tol:
                 return s
     finally:
         ctx.prec = prec
     if p <= q+3:
@@ -835,31 +842,31 @@
         #print "using asymp"
         try:
             try:
                 ctx.prec += asymp_extraprec
                 # http://functions.wolfram.com/HypergeometricFunctions/
                 # Hypergeometric1F2/06/02/03/
                 def h(a1,b1,b2):
-                    X = ctx.mpq_1_2*(a1-b1-b2+ctx.mpq_1_2)
+                    X = MPQ(1,2)*(a1-b1-b2+MPQ(1,2))
                     c = {}
                     c[0] = ctx.one
-                    c[1] = 2*(ctx.mpq_1_4*(3*a1+b1+b2-2)*(a1-b1-b2)+b1*b2-ctx.mpq_3_16)
-                    c[2] = 2*(b1*b2+ctx.mpq_1_4*(a1-b1-b2)*(3*a1+b1+b2-2)-ctx.mpq_3_16)**2+\
-                        ctx.mpq_1_16*(-16*(2*a1-3)*b1*b2 + \
+                    c[1] = 2*(MPQ(1,4)*(3*a1+b1+b2-2)*(a1-b1-b2)+b1*b2-MPQ(3,16))
+                    c[2] = 2*(b1*b2+MPQ(1,4)*(a1-b1-b2)*(3*a1+b1+b2-2)-MPQ(3,16))**2+\
+                        MPQ(1,16)*(-16*(2*a1-3)*b1*b2 + \
                         4*(a1-b1-b2)*(-8*a1**2+11*a1+b1+b2-2)-3)
                     s1 = 0
                     s2 = 0
                     k = 0
                     tprev = 0
                     while 1:
                         if k not in c:
                             uu1 = (3*k**2+(-6*a1+2*b1+2*b2-4)*k + 3*a1**2 - \
-                                (b1-b2)**2 - 2*a1*(b1+b2-2) + ctx.mpq_1_4)
-                            uu2 = (k-a1+b1-b2-ctx.mpq_1_2)*(k-a1-b1+b2-ctx.mpq_1_2)*\
-                                (k-a1+b1+b2-ctx.mpq_5_2)
+                                (b1-b2)**2 - 2*a1*(b1+b2-2) + MPQ(1,4))
+                            uu2 = (k-a1+b1-b2-MPQ(1,2))*(k-a1-b1+b2-MPQ(1,2))*\
+                                (k-a1+b1+b2-MPQ(5,2))
                             c[k] = ctx.one/(2*k)*(uu1*c[k-1]-uu2*c[k-2])
                         w = c[k] * (-z)**(-0.5*k)
                         t1 = (-ctx.j)**k * ctx.mpf(2)**(-k) * w
                         t2 = ctx.j**k * ctx.mpf(2)**(-k) * w
                         if abs(t1) < 0.1*ctx.eps:
                             #print "Convergence :)"
                             break
@@ -914,24 +921,24 @@
         #print "using asymp"
         try:
             try:
                 ctx.prec += asymp_extraprec
                 # http://functions.wolfram.com/HypergeometricFunctions/
                 # Hypergeometric2F3/06/02/03/01/0002/
                 def h(a1,a2,b1,b2,b3):
-                    X = ctx.mpq_1_2*(a1+a2-b1-b2-b3+ctx.mpq_1_2)
+                    X = MPQ(1,2)*(a1+a2-b1-b2-b3+MPQ(1,2))
                     A2 = a1+a2
                     B3 = b1+b2+b3
                     A = a1*a2
                     B = b1*b2+b3*b2+b1*b3
                     R = b1*b2*b3
                     c = {}
                     c[0] = ctx.one
-                    c[1] = 2*(B - A + ctx.mpq_1_4*(3*A2+B3-2)*(A2-B3) - ctx.mpq_3_16)
-                    c[2] = ctx.mpq_1_2*c[1]**2 + ctx.mpq_1_16*(-16*(2*A2-3)*(B-A) + 32*R +\
+                    c[1] = 2*(B - A + MPQ(1,4)*(3*A2+B3-2)*(A2-B3) - MPQ(3,16))
+                    c[2] = MPQ(1,2)*c[1]**2 + MPQ(1,16)*(-16*(2*A2-3)*(B-A) + 32*R +\
                         4*(-8*A2**2 + 11*A2 + 8*A + B3 - 2)*(A2-B3)-3)
                     s1 = 0
                     s2 = 0
                     k = 0
                     tprev = 0
                     while 1:
                         if k not in c:
@@ -1176,15 +1183,15 @@
     can sometimes give better results.
 
     **Examples**
 
     Two separable cases: a product of two geometric series, and a
     product of two Gaussian hypergeometric functions::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, mpf, hyper2d, hyp2f1, exp
         >>> mp.dps = 25; mp.pretty = True
         >>> x, y = mpf(0.25), mpf(0.5)
         >>> hyper2d({'m':1,'n':1}, {}, x,y)
         2.666666666666666666666667
         >>> 1/(1-x)/(1-y)
         2.666666666666666666666667
         >>> hyper2d({'m':[1,2],'n':[3,4]}, {'m':[5],'n':[6]}, x,y)
@@ -1197,15 +1204,15 @@
         >>> hyper2d({'m':1,'n':1},{'m+n':1},x,y)
         2.013417124712514809623881
         >>> (exp(x)*x-exp(y)*y)/(x-y)
         2.013417124712514809623881
 
     Six of the 34 Horn functions, G1-G3 and H1-H3::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, hyper2d, nsum, fac, inf, rf
         >>> mp.dps = 10; mp.pretty = True
         >>> x, y = 0.0625, 0.125
         >>> a1,a2,b1,b2,c1,c2,d = 1.1,-1.2,-1.3,-1.4,1.5,-1.6,1.7
         >>> hyper2d({'m+n':a1,'n-m':b1,'m-n':b2},{},x,y)  # G1
         1.139090746
         >>> nsum(lambda m,n: rf(a1,m+n)*rf(b1,n-m)*rf(b2,m-n)*\
         ...     x**m*y**n/fac(m)/fac(n), [0,inf], [0,inf])
@@ -1363,15 +1370,15 @@
     functions. In order for the series to make sense, none of the
     parameters may be integers.
 
     **Examples**
 
     The value of `\,_2H_2` at `z = 1` is given by Dougall's formula::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, bihyper, mpf, hyper, gammaprod
         >>> mp.dps = 25; mp.pretty = True
         >>> a,b,c,d = 0.5, 1.5, 2.25, 3.25
         >>> bihyper([a,b],[c,d],1)
         -14.49118026212345786148847
         >>> gammaprod([c,d,1-a,1-b,c+d-a-b-1],[c-a,d-a,c-b,d-b])
         -14.49118026212345786148847
```

### Comparing `mpmath-1.3.0/mpmath/functions/orthogonal.py` & `mpmath-1.4.0a0/mpmath/functions/orthogonal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from ..libmp.backend import MPQ
 from .functions import defun, defun_wrapped
 
 def _hermite_param(ctx, n, z, parabolic_cylinder):
     """
     Combined calculation of the Hermite polynomial H_n(z) (and its
     generalization to complex n) and the parabolic cylinder
     function D.
     """
     n, ntyp = ctx._convert_param(n)
     z = ctx.convert(z)
-    q = -ctx.mpq_1_2
+    q = -MPQ(1,2)
     # For re(z) > 0, 2F0 -- http://functions.wolfram.com/
     #     HypergeometricFunctions/HermiteHGeneral/06/02/0009/
     # Otherwise, there is a reflection formula
     # 2F0 + http://functions.wolfram.com/HypergeometricFunctions/
     #           HermiteHGeneral/16/01/01/0006/
     #
     # TODO:
@@ -82,15 +83,15 @@
     **Plots**
 
     .. literalinclude :: /plots/pcfd.py
     .. image :: /plots/pcfd.png
 
     **Examples**
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, pcfd, mpf, chop, diff, taylor
         >>> mp.dps = 25; mp.pretty = True
         >>> pcfd(0,0); pcfd(1,0); pcfd(2,0); pcfd(3,0)
         1.0
         0.0
         -1.0
         0.0
         >>> pcfd(4,0); pcfd(-3,0)
@@ -140,15 +141,15 @@
             U'(a,0) z \,_1F_1\left(-\tfrac{a}{2}+\tfrac{3}{4};
             \tfrac{3}{2}; -\tfrac{1}{2}z^2\right).
 
     **Examples**
 
     Connection to other functions::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, mpf, pcfu, sqrt, pi, exp, erfc
         >>> mp.dps = 25; mp.pretty = True
         >>> z = mpf(3)
         >>> pcfu(0.5,z)
         0.03210358129311151450551963
         >>> sqrt(pi/2)*exp(z**2/4)*erfc(z/sqrt(2))
         0.03210358129311151450551963
         >>> pcfu(0.5,-z)
@@ -158,15 +159,15 @@
         >>> pcfu(0.5,-z)
         23.75012332835297233711255
         >>> sqrt(pi/2)*exp(z**2/4)*erfc(-z/sqrt(2))
         23.75012332835297233711255
 
     """
     n, _ = ctx._convert_param(a)
-    return ctx.pcfd(-n-ctx.mpq_1_2, z)
+    return ctx.pcfd(-n-MPQ(1,2), z)
 
 @defun
 def pcfv(ctx, a, z, **kwargs):
     r"""
     Gives the parabolic cylinder function `V(a,z)`, which can be
     represented in terms of :func:`~mpmath.pcfu` as
 
@@ -174,15 +175,15 @@
 
         V(a,z) = \frac{\Gamma(a+\tfrac{1}{2}) (U(a,-z)-\sin(\pi a) U(a,z)}{\pi}.
 
     **Examples**
 
     Wronskian relation between `U` and `V`::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, pcfu, diff, pcfv, sqrt, pi, chop
         >>> mp.dps = 25; mp.pretty = True
         >>> a, z = 2, 3
         >>> pcfu(a,z)*diff(pcfv,(a,z),(0,1))-diff(pcfu,(a,z),(0,1))*pcfv(a,z)
         0.7978845608028653558798921
         >>> sqrt(2/pi)
         0.7978845608028653558798921
         >>> a, z = 2.5, 3
@@ -194,16 +195,16 @@
         >>> a, z = 2+1j, 2+3j
         >>> chop(pcfu(a,z)*diff(pcfv,(a,z),(0,1))-diff(pcfu,(a,z),(0,1))*pcfv(a,z))
         0.7978845608028653558798921
 
     """
     n, ntype = ctx._convert_param(a)
     z = ctx.convert(z)
-    q = ctx.mpq_1_2
-    r = ctx.mpq_1_4
+    q = MPQ(1,2)
+    r = MPQ(1,4)
     if ntype == 'Q' and ctx.isint(n*2):
         # Faster for half-integers
         def h():
             jz = ctx.fmul(z, -1j, exact=True)
             T1terms = _hermite_param(ctx, -n-q, z, 1)
             T2terms = _hermite_param(ctx, n-q, jz, 1)
             for T in T1terms:
@@ -242,15 +243,15 @@
     r"""
     Gives the parabolic cylinder function `W(a,z)` defined in (DLMF 12.14).
 
     **Examples**
 
     Value at the origin::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, mpf, pcfw, power, gamma, sqrt, diff
         >>> mp.dps = 25; mp.pretty = True
         >>> a = mpf(0.25)
         >>> pcfw(a,0)
         0.9722833245718180765617104
         >>> power(2,-0.75)*sqrt(abs(gamma(0.25+0.5j*a)/gamma(0.75+0.5j*a)))
         0.9722833245718180765617104
         >>> diff(pcfw,(a,0),(0,1))
@@ -283,28 +284,28 @@
     a, _ = ctx._convert_param(n)
     z = ctx.convert(z)
     def h():
         w = ctx.square_exp_arg(z)
         w1 = ctx.fmul(w, -0.25, exact=True)
         w2 = ctx.fmul(w, 0.5, exact=True)
         e = ctx.exp(w1)
-        return [e], [1], [], [], [ctx.mpq_1_2*a+ctx.mpq_1_4], [ctx.mpq_1_2], w2
+        return [e], [1], [], [], [MPQ(1,2)*a+MPQ(1,4)], [MPQ(1,2)], w2
     return ctx.hypercomb(h, [], **kwargs)
 
 @defun
 def pcfy2(ctx, a, z, **kwargs):
     a, _ = ctx._convert_param(n)
     z = ctx.convert(z)
     def h():
         w = ctx.square_exp_arg(z)
         w1 = ctx.fmul(w, -0.25, exact=True)
         w2 = ctx.fmul(w, 0.5, exact=True)
         e = ctx.exp(w1)
-        return [e, z], [1, 1], [], [], [ctx.mpq_1_2*a+ctx.mpq_3_4], \
-            [ctx.mpq_3_2], w2
+        return [e, z], [1, 1], [], [], [MPQ(1,2)*a+MPQ(3,4)], \
+            [MPQ(3,2)], w2
     return ctx.hypercomb(h, [], **kwargs)
 """
 
 @defun_wrapped
 def gegenbauer(ctx, n, a, z, **kwargs):
     # Special cases: a+0.5, a*2 poles
     if ctx.isnpint(a):
```

### Comparing `mpmath-1.3.0/mpmath/functions/qfunctions.py` & `mpmath-1.4.0a0/mpmath/functions/qfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     is also known as the Euler function, or (up to a factor `q^{-1/24}`)
     the Dedekind eta function.
 
     **Examples**
 
     If `n` is a positive integer, the function amounts to a finite product::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, qp, fprod, limit, rf, taylor, findroot,
+        ...                     diffun, mpf, jtheta, pi, root)
         >>> mp.dps = 25; mp.pretty = True
         >>> qp(2,3,5)
         -725305.0
         >>> fprod(1-2*3**k for k in range(5))
         -725305.0
         >>> qp(2,3,0)
         1.0
@@ -138,15 +139,15 @@
         \Gamma_q(z) = \frac{(q; q)_{\infty}}{(q^z; q)_{\infty}} (1-q)^{1-z}.
 
 
     **Examples**
 
     Evaluation for real and complex arguments::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, qgamma, mpf
         >>> mp.dps = 25; mp.pretty = True
         >>> qgamma(4,0.75)
         4.046875
         >>> qgamma(6,6)
         121226245.0
         >>> qgamma(3+4j, 0.5j)
         (0.1663082382255199834630088 + 0.01952474576025952984418217j)
@@ -180,15 +181,15 @@
 
     .. math ::
 
         [z]_q! = \frac{(q;q)_z}{(1-q)^z}.
 
     **Examples**
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, qfac
         >>> mp.dps = 25; mp.pretty = True
         >>> qfac(0,0)
         1.0
         >>> qfac(4,3)
         2080.0
         >>> qfac(5,6)
         121226245.0
@@ -220,15 +221,15 @@
 
     where `(a;q)_n` denotes the q-Pochhammer symbol (see :func:`~mpmath.qp`).
 
     **Examples**
 
     Evaluation works for real and complex arguments::
 
-        >>> from mpmath import *
+        >>> from mpmath import qhyper, mp, nsum, qp, inf, j
         >>> mp.dps = 25; mp.pretty = True
         >>> qhyper([0.5], [2.25], 0.25, 4)
         -0.1975849091263356009534385
         >>> qhyper([0.5], [2.25], 0.25-0.25j, 4)
         (2.806330244925716649839237 + 3.568997623337943121769938j)
         >>> qhyper([1+j], [2,3+0.5j], 0.25, 3+4j)
         (9.112885171773400017270226 - 1.272756997166375050700388j)
```

### Comparing `mpmath-1.3.0/mpmath/functions/rszeta.py` & `mpmath-1.4.0a0/mpmath/functions/rszeta.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 on sigma.  The program gives an error when the Riemann-Siegel
 formula can not compute to the wanted precision.
 
 """
 
 import math
 
-class RSCache(object):
+class RSCache:
     def __init__(ctx):
         ctx._rs_cache = [0, 10, {}, {}]
 
 from .functions import defun
 
 #-------------------------------------------------------------------------------#
 #                                                                               #
```

### Comparing `mpmath-1.3.0/mpmath/functions/signals.py` & `mpmath-1.4.0a0/mpmath/functions/signals.py`

 * *Files identical despite different names*

### Comparing `mpmath-1.3.0/mpmath/functions/theta.py` & `mpmath-1.4.0a0/mpmath/functions/theta.py`

 * *Files identical despite different names*

### Comparing `mpmath-1.3.0/mpmath/functions/zeta.py` & `mpmath-1.4.0a0/mpmath/functions/zeta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from __future__ import print_function
-
-from ..libmp.backend import xrange
 from .functions import defun, defun_wrapped, defun_static
 
 @defun
 def stieltjes(ctx, n, a=1):
     n = ctx.convert(n)
     a = ctx.convert(a)
     if n < 0:
@@ -284,55 +281,59 @@
                 yield t
     return ctx.sum_accurately(terms)
 
 # TODO: for bernpoly and eulerpoly, ensure that all exact zeros are covered
 
 @defun_wrapped
 def bernpoly(ctx, n, z):
-    # Slow implementation:
-    #return sum(ctx.binomial(n,k)*ctx.bernoulli(k)*z**(n-k) for k in xrange(0,n+1))
     n = int(n)
     if n < 0:
         raise ValueError("Bernoulli polynomials only defined for n >= 0")
-    if z == 0 or (z == 1 and n > 1):
-        return ctx.bernoulli(n)
-    if z == 0.5:
-        return (ctx.ldexp(1,1-n)-1)*ctx.bernoulli(n)
     if n <= 3:
         if n == 0: return z ** 0
         if n == 1: return z - 0.5
         if n == 2: return (6*z*(z-1)+1)/6
         if n == 3: return z*(z*(z-1.5)+0.5)
+    if z == 0 or z == 1:
+        return ctx.bernoulli(n)
+    if z == 0.5:
+        return (ctx.ldexp(1,1-n)-1)*ctx.bernoulli(n)
     if ctx.isinf(z):
         return z ** n
     if ctx.isnan(z):
         return z
     if abs(z) > 2:
         def terms():
             t = ctx.one
             yield t
             r = ctx.one/z
-            k = 1
+            t = t*n*r
+            yield -t/2
+            k = 2
             while k <= n:
                 t = t*(n+1-k)/k*r
-                if not (k > 2 and k & 1):
+                if not k & 1:
                     yield t*ctx.bernoulli(k)
                 k += 1
         return ctx.sum_accurately(terms) * z**n
     else:
         def terms():
             yield ctx.bernoulli(n)
             t = ctx.one
             k = 1
-            while k <= n:
+            while k < n - 1:
                 t = t*(n+1-k)/k * z
                 m = n-k
-                if not (m > 2 and m & 1):
+                if not m & 1:
                     yield t*ctx.bernoulli(m)
                 k += 1
+            t = t*2/(n-1)*z
+            yield -t/2
+            t = t/n*z
+            yield t
         return ctx.sum_accurately(terms)
 
 @defun_wrapped
 def eulerpoly(ctx, n, z):
     n = int(n)
     if n < 0:
         raise ValueError("Euler polynomials only defined for n >= 0")
@@ -358,21 +359,22 @@
     # http://functions.wolfram.com/Polynomials/EulerE2/06/01/02/01/0002/
     def terms():
         t = ctx.one
         k = 0
         w = ctx.ldexp(1,n+2)
         while 1:
             v = n-k+1
-            if not (v > 2 and v & 1):
+            if not v & 1:
                 yield (2-w)*ctx.bernoulli(v)*t
             k += 1
-            if k > n:
-                break
             t = t*z*(n-k+2)/k
             w *= 0.5
+            if k >= n:
+                break
+        yield -(2-w)*t/2
     return ctx.sum_accurately(terms) / m
 
 @defun
 def eulernum(ctx, n, exact=False):
     n = int(n)
     if exact:
         return int(ctx._eulernum(n))
@@ -549,23 +551,21 @@
         #        return ctx._zeta(s, **kwargs)
         #    except NotImplementedError:
         #        if verbose:
         #            print "zeta: Could not use the Borwein algorithm"
         #        pass
         if abs(im) > 500*prec and 10*re < prec and derivative <= 4 or \
             method == 'riemann-siegel':
-            try:   #  py2.4 compatible try block
-                try:
-                    if verbose:
-                        print("zeta: Attempting to use the Riemann-Siegel algorithm")
-                    return ctx.rs_zeta(s, derivative, **kwargs)
-                except NotImplementedError:
-                    if verbose:
-                        print("zeta: Could not use the Riemann-Siegel algorithm")
-                    pass
+            try:
+                if verbose:
+                    print("zeta: Attempting to use the Riemann-Siegel algorithm")
+                return ctx.rs_zeta(s, derivative, **kwargs)
+            except NotImplementedError:
+                if verbose:
+                    print("zeta: Could not use the Riemann-Siegel algorithm")
             finally:
                 ctx.prec = prec
     if s == 1:
         return ctx.inf
     abss = abs(s)
     if abss == ctx.inf:
         if ctx.re(s) == ctx.inf:
@@ -629,34 +629,34 @@
             return ctx.bernpoly(1-n, a) / (n-1)
     if not (atype == 'Q' or atype == 'Z'):
         raise NotImplementedError
     t = 1-s
     # We now require a to be standardized
     v = 0
     shift = 0
-    b = a
+    b = ctx.mpf(a)
     while ctx.re(b) > 1:
         b -= 1
         v -= b**negs
         shift -= 1
     while ctx.re(b) <= 0:
         v += b**negs
         b += 1
         shift += 1
     # Rational reflection formula
     try:
-        p, q = a._mpq_
+        p, q = a.numerator, a.denominator
     except:
         assert a == int(a)
         p = int(a)
         q = 1
     p += shift*q
     assert 1 <= p <= q
     g = ctx.fsum(ctx.cospi(t/2-2*k*b)*ctx._hurwitz(t,(k,q)) \
-        for k in range(1,q+1))
+        for k in range(1, q+1))
     g *= 2*ctx.gamma(t)/(2*ctx.pi*q)**t
     v += g
     return v
 
 def _hurwitz_em(ctx, s, a, d, prec, verbose):
     # May not be converted at this point
     a = ctx.convert(a)
@@ -701,16 +701,16 @@
             else:
                 upds = [j2-2, j2-1]
             for m in upds:
                 D = min(m,d+1)
                 if m <= d:
                     logs.append(logs[-1] * logr)
                 Un = [0]*(D+1)
-                for i in xrange(D): Un[i] = (1-m-s)*U[i]
-                for i in xrange(1,D+1): Un[i] += (d-(i-1))*U[i-1]
+                for i in range(D): Un[i] = (1-m-s)*U[i]
+                for i in range(1, D+1): Un[i] += (d-(i-1))*U[i-1]
                 U = Un
                 r *= rM2a
             t = ctx.fdot(U, logs) * r * ctx.bernoulli(j2)/(-fact)
             tailsum += t
             if ctx.mag(t) < tol:
                 return lsum, (-1)**d * tailsum
             fact *= (j2+1)*(j2+2)
@@ -742,28 +742,28 @@
         except NotImplementedError:
             pass
     negs = ctx.fneg(s, exact=True)
     have_derivatives = derivatives != [0]
     have_one_derivative = len(derivatives) == 1
     if not reflect:
         if not have_derivatives:
-            return [ctx.fsum((a+k)**negs for k in xrange(n+1))], []
+            return [ctx.fsum((a+k)**negs for k in range(n+1))], []
         if have_one_derivative:
             d = derivatives[0]
-            x = ctx.fsum(ctx.ln(a+k)**d * (a+k)**negs for k in xrange(n+1))
+            x = ctx.fsum(ctx.ln(a+k)**d * (a+k)**negs for k in range(n+1))
             return [(-1)**d * x], []
     maxd = max(derivatives)
     if not have_one_derivative:
         derivatives = range(maxd+1)
     xs = [ctx.zero for d in derivatives]
     if reflect:
         ys = [ctx.zero for d in derivatives]
     else:
         ys = []
-    for k in xrange(n+1):
+    for k in range(n+1):
         w = a + k
         xterm = w ** negs
         if reflect:
             yterm = ctx.conj(ctx.one / (w * xterm))
         if have_derivatives:
             logw = -ctx.ln(w)
             if have_one_derivative:
@@ -801,15 +801,15 @@
                     have_pole = False
                     h = +ctx.eps
                     ctx.prec *= 2*(d+1)
                     s += h
             if have_pole:
                 return +ctx.inf
         z = ctx.zero
-        for p in range(1,q+1):
+        for p in range(1, q+1):
             if chi[p%q]:
                 if d == 1:
                     z += chi[p%q] * (ctx.zeta(s, (p,q), 1) - \
                         ctx.zeta(s, (p,q))*ctx.log(q))
                 else:
                     z += chi[p%q] * ctx.zeta(s, (p,q))
         z /= q**s
@@ -928,16 +928,16 @@
 
     `Z(s)` extends to a meromorphic function on `\mathbb{C}`  with a
     double pole at `s=1` and  simple poles at the points `-2n` for
     `n=0`,  1, 2, ...
 
     **Examples**
 
-        >>> from mpmath import *
-        >>> mp.pretty = True; mp.dps = 15
+        >>> from mpmath import mp, secondzeta, pi, gamma, zeta, diff, chop, j
+        >>> mp.pretty = True
         >>> secondzeta(2)
         0.023104993115419
         >>> xi = lambda s: 0.5*s*(s-1)*pi**(-0.5*s)*gamma(0.5*s)*zeta(s)
         >>> Xi = lambda t: xi(0.5+t*j)
         >>> chop(-0.5*diff(Xi,0,n=2)/Xi(0))
         0.023104993115419
 
@@ -1068,15 +1068,16 @@
     The Lerch transcendent generalizes the Hurwitz zeta function :func:`zeta`
     (`z = 1`) and the polylogarithm :func:`polylog` (`a = 1`).
 
     **Examples**
 
     Several evaluations in terms of simpler functions::
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, lerchphi, catalan, diff, zeta, pi, log,
+        ...                     atanh, sqrt, j, polylog)
         >>> mp.dps = 25; mp.pretty = True
         >>> lerchphi(-1,2,0.5); 4*catalan
         3.663862376708876060218414
         3.663862376708876060218414
         >>> diff(lerchphi, (-1,-2,1), (0,1,0)); 7*zeta(3)/(4*pi**2)
         0.2131391994087528954617607
         0.2131391994087528954617607
@@ -1134,15 +1135,15 @@
         return ctx.polylog(s, z) / z
     if ctx.re(a) < 1:
         if ctx.isnpint(a):
             raise ValueError("Lerch transcendent complex infinity")
         m = int(ctx.ceil(1-ctx.re(a)))
         v = ctx.zero
         zpow = ctx.one
-        for n in xrange(m):
+        for n in range(m):
             v += zpow / (a+n)**s
             zpow *= z
         return zpow * ctx.lerchphi(z,s, a+m) + v
     g = ctx.ln(z)
     v = 1/(2*a**s) + ctx.gammainc(1-s, -a*g) * (-g)**(s-1) / z**a
     h = s / 2
     r = 2*ctx.pi
```

### Comparing `mpmath-1.3.0/mpmath/functions/zetazeros.py` & `mpmath-1.4.0a0/mpmath/functions/zetazeros.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,15 +345,15 @@
     `s = \frac{1}{2} + ti` for which `\zeta(s) = 0`. Equivalently, the
     imaginary part `t` is a zero of the Z-function (:func:`~mpmath.siegelz`).
 
     **Examples**
 
     The first few zeros::
 
-        >>> from mpmath import *
+        >>> from mpmath import mp, zetazero, chop, zeta, siegelz
         >>> mp.dps = 25; mp.pretty = True
         >>> zetazero(1)
         (0.5 + 14.13472514173469379045725j)
         >>> zetazero(2)
         (0.5 + 21.02203963877155499262848j)
         >>> zetazero(20)
         (0.5 + 77.14484006887480537268266j)
@@ -476,16 +476,16 @@
     Computes the number of zeros of the Riemann zeta function in
     `(0,1) \times (0,t]`, usually denoted by `N(t)`.
 
     **Examples**
 
     The first zero has imaginary part between 14 and 15::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, nzeros, zetazero
+        >>> mp.pretty = True
         >>> nzeros(14)
         0
         >>> nzeros(15)
         1
         >>> zetazero(1)
         (0.5 + 14.1347251417347j)
 
@@ -548,16 +548,17 @@
     Computes the function
     `S(t) = \operatorname{arg} \zeta(\frac{1}{2} + it) / \pi`.
 
     See Titchmarsh Section 9.3 for details of the definition.
 
     **Examples**
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (mp, backlunds, chop, grampoint, extraprec,
+        ...                     nzeros, siegeltheta, pi)
+        >>> mp.pretty = True
         >>> backlunds(217.3)
         0.16302205431184
 
     Generally, the value is a small number. At Gram points it is an integer,
     frequently equal to 0::
 
         >>> chop(backlunds(grampoint(200)))
```

### Comparing `mpmath-1.3.0/mpmath/identification.py` & `mpmath-1.4.0a0/mpmath/identification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Implements the PSLQ algorithm for integer relation detection,
 and derivative algorithms for constant recognition.
 """
 
-from .libmp.backend import xrange
 from .libmp import int_types, sqrt_fixed
 
 # round to nearest integer (can be done more elegantly...)
 def round_fixed(x, prec):
     return ((x + (1<<(prec-1))) >> prec) << prec
 
-class IdentificationMethods(object):
+class IdentificationMethods:
     pass
 
 
 def pslq(ctx, x, tol=None, maxcoeff=1000, maxsteps=100, verbose=False):
     r"""
     Given a vector of real numbers `x = [x_0, x_1, ..., x_n]`, ``pslq(x)``
     uses the PSLQ algorithm to find a list of integers
@@ -28,16 +27,16 @@
     exists, :func:`~mpmath.pslq` returns ``None``. The tolerance defaults to
     3/4 of the working precision.
 
     **Examples**
 
     Find rational approximations for `\pi`::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import mp, pslq, pi, mpf, sqrt, acot
+        >>> mp.pretty = True
         >>> pslq([-1, pi], tol=0.01)
         [22, 7]
         >>> pslq([-1, pi], tol=0.001)
         [355, 113]
         >>> mpf(22)/7; mpf(355)/113; +pi
         3.14285714285714
         3.14159292035398
@@ -174,58 +173,58 @@
 
     g = sqrt_fixed((4<<prec)//3, prec)
     A = {}
     B = {}
     H = {}
     # Initialization
     # step 1
-    for i in xrange(1, n+1):
-        for j in xrange(1, n+1):
+    for i in range(1, n+1):
+        for j in range(1, n+1):
             A[i,j] = B[i,j] = (i==j) << prec
             H[i,j] = 0
     # step 2
     s = [None] + [0] * n
-    for k in xrange(1, n+1):
+    for k in range(1, n+1):
         t = 0
-        for j in xrange(k, n+1):
+        for j in range(k, n+1):
             t += (x[j]**2 >> prec)
         s[k] = sqrt_fixed(t, prec)
     t = s[1]
     y = x[:]
-    for k in xrange(1, n+1):
+    for k in range(1, n+1):
         y[k] = (x[k] << prec) // t
         s[k] = (s[k] << prec) // t
     # step 3
-    for i in xrange(1, n+1):
-        for j in xrange(i+1, n):
+    for i in range(1, n+1):
+        for j in range(i+1, n):
             H[i,j] = 0
         if i <= n-1:
             if s[i]:
                 H[i,i] = (s[i+1] << prec) // s[i]
             else:
                 H[i,i] = 0
         for j in range(1, i):
             sjj1 = s[j]*s[j+1]
             if sjj1:
                 H[i,j] = ((-y[i]*y[j])<<prec)//sjj1
             else:
                 H[i,j] = 0
     # step 4
-    for i in xrange(2, n+1):
-        for j in xrange(i-1, 0, -1):
+    for i in range(2, n+1):
+        for j in range(i-1, 0, -1):
             #t = floor(H[i,j]/H[j,j] + 0.5)
             if H[j,j]:
                 t = round_fixed((H[i,j] << prec)//H[j,j], prec)
             else:
                 #t = 0
                 continue
             y[j] = y[j] + (t*y[i] >> prec)
-            for k in xrange(1, j+1):
+            for k in range(1, j+1):
                 H[i,k] = H[i,k] - (t*H[j,k] >> prec)
-            for k in xrange(1, n+1):
+            for k in range(1, n+1):
                 A[i,k] = A[i,k] - (t*A[j,k] >> prec)
                 B[k,j] = B[k,j] + (t*B[k,i] >> prec)
     # Main algorithm
     for REP in range(maxsteps):
         # Step 1
         m = -1
         szmax = -1
@@ -233,54 +232,54 @@
             h = H[i,i]
             sz = (g**i * abs(h)) >> (prec*(i-1))
             if sz > szmax:
                 m = i
                 szmax = sz
         # Step 2
         y[m], y[m+1] = y[m+1], y[m]
-        for i in xrange(1,n+1): H[m,i], H[m+1,i] = H[m+1,i], H[m,i]
-        for i in xrange(1,n+1): A[m,i], A[m+1,i] = A[m+1,i], A[m,i]
-        for i in xrange(1,n+1): B[i,m], B[i,m+1] = B[i,m+1], B[i,m]
+        for i in range(1,n+1): H[m,i], H[m+1,i] = H[m+1,i], H[m,i]
+        for i in range(1,n+1): A[m,i], A[m+1,i] = A[m+1,i], A[m,i]
+        for i in range(1,n+1): B[i,m], B[i,m+1] = B[i,m+1], B[i,m]
         # Step 3
         if m <= n - 2:
             t0 = sqrt_fixed((H[m,m]**2 + H[m,m+1]**2)>>prec, prec)
             # A zero element probably indicates that the precision has
             # been exhausted. XXX: this could be spurious, due to
             # using fixed-point arithmetic
             if not t0:
                 break
             t1 = (H[m,m] << prec) // t0
             t2 = (H[m,m+1] << prec) // t0
-            for i in xrange(m, n+1):
+            for i in range(m, n+1):
                 t3 = H[i,m]
                 t4 = H[i,m+1]
                 H[i,m] = (t1*t3+t2*t4) >> prec
                 H[i,m+1] = (-t2*t3+t1*t4) >> prec
         # Step 4
-        for i in xrange(m+1, n+1):
-            for j in xrange(min(i-1, m+1), 0, -1):
+        for i in range(m+1, n+1):
+            for j in range(min(i-1, m+1), 0, -1):
                 try:
                     t = round_fixed((H[i,j] << prec)//H[j,j], prec)
                 # Precision probably exhausted
                 except ZeroDivisionError:
                     break
                 y[j] = y[j] + ((t*y[i]) >> prec)
-                for k in xrange(1, j+1):
+                for k in range(1, j+1):
                     H[i,k] = H[i,k] - (t*H[j,k] >> prec)
-                for k in xrange(1, n+1):
+                for k in range(1, n+1):
                     A[i,k] = A[i,k] - (t*A[j,k] >> prec)
                     B[k,j] = B[k,j] + (t*B[k,i] >> prec)
         # Until a relation is found, the error typically decreases
         # slowly (e.g. a factor 1-10) with each step TODO: we could
         # compare err from two successive iterations. If there is a
         # large drop (several orders of magnitude), that indicates a
         # "high quality" relation was detected. Reporting this to
         # the user somehow might be useful.
         best_err = maxcoeff<<prec
-        for i in xrange(1, n+1):
+        for i in range(1, n+1):
             err = abs(y[i])
             # Maybe we are done?
             if err < tol:
                 # We are done if the coefficients are acceptable
                 vec = [int(round_fixed(B[j,i], prec) >> prec) for j in \
                 range(1,n+1)]
                 if max(abs(v) for v in vec) < maxcoeff:
@@ -326,16 +325,17 @@
     at high precision; preferably 50 digits or more.
 
     **Examples**
 
     By default (degree `n = 1`), :func:`~mpmath.findpoly` simply finds a linear
     polynomial with a rational root::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (mp, findpoly, nprint, polyval, polyroots,
+        ...                     sqrt, pi, phi, euler, findroot)
+        >>> mp.pretty = True
         >>> findpoly(0.7)
         [-10, 7]
 
     The generated coefficient list is valid input to ``polyval`` and
     ``polyroots``::
 
         >>> nprint(polyval(findpoly(phi, 2), phi), 1)
@@ -372,28 +372,26 @@
     If :func:`~mpmath.findpoly` fails to find a polynomial with given
     coefficient size and tolerance constraints, that means no such
     polynomial exists.
 
     We can verify that `\pi` is not an algebraic number of degree 3 with
     coefficients less than 1000::
 
-        >>> mp.dps = 15
         >>> findpoly(pi, 3)
         >>>
 
     It is always possible to find an algebraic approximation of a number
     using one (or several) of the following methods:
 
         1. Increasing the permitted degree
         2. Allowing larger coefficients
         3. Reducing the tolerance
 
     One example of each method is shown below::
 
-        >>> mp.dps = 15
         >>> findpoly(pi, 4)
         [95, -545, 863, -183, -298]
         >>> findpoly(pi, 3, maxcoeff=10000)
         [836, -1734, -2658, -457]
         >>> findpoly(pi, 3, tol=1e-7)
         [-4, 22, -29, -2]
 
@@ -536,16 +534,17 @@
     formula for `x`. This formula is returned as a string. If no match
     is found, ``None`` is returned. With ``full=True``, a list of
     matching formulas is returned.
 
     As a simple example, :func:`~mpmath.identify` will find an algebraic
     formula for the golden ratio::
 
-        >>> from mpmath import *
-        >>> mp.dps = 15; mp.pretty = True
+        >>> from mpmath import (mp, identify, phi, pi, e, sqrt, log, mpf,
+        ...                     exp, catalan)
+        >>> mp.pretty = True
         >>> identify(phi)
         '((1+sqrt(5))/2)'
 
     :func:`~mpmath.identify` can identify simple algebraic numbers and simple
     combinations of given base constants, as well as certain basic
     transformations thereof. More specifically, :func:`~mpmath.identify`
     looks for the following:
@@ -570,15 +569,14 @@
 
     **Examples**
 
     Simple identifications can be performed safely at standard
     precision. Here the default recognition of rational, algebraic,
     and exp/log of algebraic numbers is demonstrated::
 
-        >>> mp.dps = 15
         >>> identify(0.22222222222222222)
         '(2/9)'
         >>> identify(1.9662210973805663)
         'sqrt(((24+sqrt(48))/8))'
         >>> identify(4.1132503787829275)
         'exp((sqrt(8)/2))'
         >>> identify(0.881373587019543)
@@ -654,15 +652,14 @@
     With ``full=True``, and by supplying a few base constants,
     ``identify`` can generate almost endless lists of approximations
     for any number (the output below has been truncated to show only
     the first few)::
 
         >>> for p in identify(pi, ['e', 'catalan'], tol=1e-5, full=True):
         ...     print(p)
-        ...  # doctest: +ELLIPSIS
         e/log((6 + (-4/3)*e))
         (3**3*5*e*catalan**2)/(2*7**2)
         sqrt(((-13) + 1*e + 22*catalan))
         log(((-6) + 24*e + 4*catalan)/e)
         exp(catalan*((-1/5) + (8/15)*e))
         catalan*(6 + (-6)*e + 15*catalan)
         sqrt((5 + 26*e + (-3)*catalan))/e
@@ -683,23 +680,23 @@
         >>> log(24*e-6+4*catalan)-1
         3.14158791577159
 
     **Symbolic processing**
 
     The output formula can be evaluated as a Python expression.
     Note however that if fractions (like '2/3') are present in
-    the formula, Python's :func:`~mpmath.eval()` may erroneously perform
+    the formula, Python's :func:`eval` may erroneously perform
     integer division. Note also that the output is not necessarily
     in the algebraically simplest form::
 
         >>> identify(sqrt(2))
         '(sqrt(8)/2)'
 
     As a solution to both problems, consider using SymPy's
-    :func:`~mpmath.sympify` to convert the formula into a symbolic expression.
+    :func:`~sympy.core.sympify.sympify` to convert the formula into a symbolic expression.
     SymPy can be used to pretty-print or further simplify the formula
     symbolically::
 
         >>> from sympy import sympify # doctest: +SKIP
         >>> sympify(identify(sqrt(2))) # doctest: +SKIP
         2**(1/2)
 
@@ -715,15 +712,15 @@
         2/(6 - 2*5**(1/2))**(1/2)
         >>> mp.dps = 30 # doctest: +SKIP
         >>> x = sympify(identify(x.evalf(30))) # doctest: +SKIP
         >>> x # doctest: +SKIP
         1/2 + 5**(1/2)/2
 
     (In fact, this functionality is available directly in SymPy as the
-    function :func:`~mpmath.nsimplify`, which is essentially a wrapper for
+    function :func:`~sympy.simplify.simplify.nsimplify`, which is essentially a wrapper for
     :func:`~mpmath.identify`.)
 
     **Miscellaneous issues and limitations**
 
     The input `x` must be a real number. All base constants must be
     positive real numbers and must not be rationals or rational linear
     combinations of each other.
@@ -833,12 +830,7 @@
         return sorted(solutions, key=len)
     else:
         return None
 
 IdentificationMethods.pslq = pslq
 IdentificationMethods.findpoly = findpoly
 IdentificationMethods.identify = identify
-
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/libmp/gammazeta.py` & `mpmath-1.4.0a0/mpmath/libmp/gammazeta.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,55 +12,37 @@
 
 -----------------------------------------------------------------------
 """
 
 import math
 import sys
 
-from .backend import xrange
-from .backend import MPZ, MPZ_ZERO, MPZ_ONE, MPZ_THREE, gmpy
-
-from .libintmath import list_primes, ifac, ifac2, moebius
-
-from .libmpf import (\
-    round_floor, round_ceiling, round_down, round_up,
-    round_nearest, round_fast,
-    lshift, sqrt_fixed, isqrt_fast,
-    fzero, fone, fnone, fhalf, ftwo, finf, fninf, fnan,
-    from_int, to_int, to_fixed, from_man_exp, from_rational,
-    mpf_pos, mpf_neg, mpf_abs, mpf_add, mpf_sub,
-    mpf_mul, mpf_mul_int, mpf_div, mpf_sqrt, mpf_pow_int,
-    mpf_rdiv_int,
-    mpf_perturb, mpf_le, mpf_lt, mpf_gt, mpf_shift,
-    negative_rnd, reciprocal_rnd,
-    bitcount, to_float, mpf_floor, mpf_sign, ComplexResult
-)
-
-from .libelefun import (\
-    constant_memo,
-    def_mpf_constant,
-    mpf_pi, pi_fixed, ln2_fixed, log_int_fixed, mpf_ln2,
-    mpf_exp, mpf_log, mpf_pow, mpf_cosh,
-    mpf_cos_sin, mpf_cosh_sinh, mpf_cos_sin_pi, mpf_cos_pi, mpf_sin_pi,
-    ln_sqrt2pi_fixed, mpf_ln_sqrt2pi, sqrtpi_fixed, mpf_sqrtpi,
-    cos_sin_fixed, exp_fixed
-)
-
-from .libmpc import (\
-    mpc_zero, mpc_one, mpc_half, mpc_two,
-    mpc_abs, mpc_shift, mpc_pos, mpc_neg,
-    mpc_add, mpc_sub, mpc_mul, mpc_div,
-    mpc_add_mpf, mpc_mul_mpf, mpc_div_mpf, mpc_mpf_div,
-    mpc_mul_int, mpc_pow_int,
-    mpc_log, mpc_exp, mpc_pow,
-    mpc_cos_pi, mpc_sin_pi,
-    mpc_reciprocal, mpc_square,
-    mpc_sub_mpf
-)
-
+from .backend import MPZ, MPZ_ONE, MPZ_THREE, MPZ_ZERO, gmpy
+from .libelefun import (constant_memo, cos_sin_fixed, def_mpf_constant,
+                        exp_fixed, ln2_fixed, ln_sqrt2pi_fixed, log_int_fixed,
+                        mpf_cos_pi, mpf_cos_sin, mpf_cos_sin_pi, mpf_cosh,
+                        mpf_cosh_sinh, mpf_exp, mpf_ln2, mpf_ln_sqrt2pi,
+                        mpf_log, mpf_pi, mpf_pow, mpf_sin_pi, mpf_sqrtpi,
+                        pi_fixed, sqrtpi_fixed)
+from .libintmath import ifac, ifac2, list_primes, moebius
+from .libmpc import (mpc_abs, mpc_add, mpc_add_mpf, mpc_cos_pi, mpc_div,
+                     mpc_div_mpf, mpc_exp, mpc_half, mpc_log, mpc_mpf_div,
+                     mpc_mul, mpc_mul_int, mpc_mul_mpf, mpc_neg, mpc_one,
+                     mpc_pos, mpc_pow, mpc_pow_int, mpc_reciprocal, mpc_shift,
+                     mpc_sin_pi, mpc_square, mpc_sub, mpc_sub_mpf, mpc_two,
+                     mpc_zero)
+from .libmpf import (ComplexResult, fhalf, finf, fnan, fninf, fnone, fone,
+                     from_int, from_man_exp, from_rational, ftwo, fzero,
+                     isqrt_fast, lshift, mpf_abs, mpf_add, mpf_div, mpf_floor,
+                     mpf_gt, mpf_le, mpf_lt, mpf_mul, mpf_mul_int, mpf_neg,
+                     mpf_perturb, mpf_pos, mpf_pow_int, mpf_rdiv_int,
+                     mpf_shift, mpf_sign, mpf_sqrt, mpf_sub, negative_rnd,
+                     reciprocal_rnd, round_ceiling, round_down, round_fast,
+                     round_floor, round_nearest, round_up, sqrt_fixed,
+                     to_fixed, to_float, to_int)
 
 
 # Catalan's constant is computed using Lupas's rapidly convergent series
 # (listed on http://mathworld.wolfram.com/CatalansConstant.html)
 #            oo
 #            ___       n-1  8n     2                   3    2
 #        1  \      (-1)    2   (40n  - 24n + 3) [(2n)!] (n!)
@@ -310,15 +292,15 @@
         s = mpf_add(s, t)
         m += 1
     return to_fixed(s, prec)
 
 @constant_memo
 def twinprime_fixed(prec):
     def I(n):
-        return sum(moebius(d)<<(n//d) for d in xrange(1,n+1) if not n%d)//n
+        return sum(moebius(d)<<(n//d) for d in range(1,n+1) if not n%d)//n
     wp = 2*prec + 30
     res = fone
     primes = [from_rational(1,p,wp) for p in [2,3,5,7]]
     ppowers = [mpf_mul(p,p,wp) for p in primes]
     n = 2
     while 1:
         a = mpf_zeta_int(n, wp)
@@ -394,23 +376,23 @@
 def bernoulli_size(n):
     """Accurately estimate the size of B_n (even n > 2 only)"""
     lgn = math.log(n,2)
     return int(2.326 + 0.5*lgn + n*(lgn - 4.094))
 
 BERNOULLI_PREC_CUTOFF = bernoulli_size(MAX_BERNOULLI_CACHE)
 
-def mpf_bernoulli(n, prec, rnd=None):
+def mpf_bernoulli(n, prec, rnd=None, plus=False):
     """Computation of Bernoulli numbers (numerically)"""
     if n < 2:
         if n < 0:
             raise ValueError("Bernoulli numbers only defined for n >= 0")
         if n == 0:
             return fone
         if n == 1:
-            return mpf_neg(fhalf)
+            return fhalf if plus else mpf_neg(fhalf)
     # For odd n > 1, the Bernoulli numbers are zero
     if n & 1:
         return fzero
     # If precision is extremely high, we can save time by computing
     # the Bernoulli number at a lower precision that is sufficient to
     # obtain the exact fraction, round to the exact fraction, and
     # convert the fraction back to an mpf value at the original precision
@@ -446,15 +428,15 @@
         szbm = bernoulli_size(m)
         s = 0
         sexp = max(0, szbm)  - wp
         if m < 6:
             a = MPZ_ZERO
         else:
             a = bin1
-        for j in xrange(1, m//6+1):
+        for j in range(1, m//6+1):
             usign, uman, uexp, ubc = u = numbers[m-6*j]
             if usign:
                 uman = -uman
             s += lshift(a*uman, uexp-sexp)
             # Update inner binomial coefficient
             j6 = 6*j
             a *= ((m-5-j6)*(m-4-j6)*(m-3-j6)*(m-2-j6)*(m-1-j6)*(m-j6))
@@ -480,26 +462,29 @@
     v = mpf_mul(v, mpf_zeta_int(n, wp), wp)
     v = mpf_mul(v, mpf_pow_int(mpf_pi(piprec), -n, wp))
     v = mpf_shift(v, 1-n)
     if not n & 3:
         v = mpf_neg(v)
     return mpf_pos(v, prec, rnd or round_fast)
 
-def bernfrac(n):
+def bernfrac(n, plus=False):
     r"""
     Returns a tuple of integers `(p, q)` such that `p/q = B_n` exactly,
     where `B_n` denotes the `n`-th Bernoulli number. The fraction is
     always reduced to lowest terms. Note that for `n > 1` and `n` odd,
     `B_n = 0`, and `(0, 1)` is returned.
 
+    Optional ``plus`` flag (default: False) control the sign choice of
+    the `B_1` value (default: `(-1, 2)`).
+
     **Examples**
 
     The first few Bernoulli numbers are exactly::
 
-        >>> from mpmath import *
+        >>> from mpmath import bernfrac, mp, mpf, bernoulli
         >>> for n in range(15):
         ...     p, q = bernfrac(n)
         ...     print("%s %s/%s" % (n, p, q))
         ...
         0 1/1
         1 -1/2
         2 1/6
@@ -514,14 +499,18 @@
         11 0/1
         12 -691/2730
         13 0/1
         14 7/6
 
     This function works for arbitrarily large `n`::
 
+        >>> import sys
+        >>> if hasattr(sys, 'set_int_max_str_digits'):
+        ...     sys.set_int_max_str_digits(30000)
+        >>> del sys
         >>> p, q = bernfrac(10**4)
         >>> print(q)
         2338224387510
         >>> print(len(str(p)))
         27692
         >>> mp.dps = 15
         >>> print(mpf(p) / q)
@@ -550,18 +539,20 @@
 
     1. MathWorld, von Staudt-Clausen Theorem:
        http://mathworld.wolfram.com/vonStaudt-ClausenTheorem.html
 
     2. The Bernoulli Number Page:
        http://www.bernoulli.org/
 
+    3. https://en.wikipedia.org/wiki/Bernoulli_number
+
     """
     n = int(n)
     if n < 3:
-        return [(1, 1), (-1, 2), (1, 6)][n]
+        return [(1, 1), (1 if plus else -1, 2), (1, 6)][n]
     if n & 1:
         return (0, 1)
     q = 1
     for k in list_primes(n+1):
         if not (n % (k-1)):
             q *= k
     prec = bernoulli_size(n) + int(math.log(q,2)) + 20
@@ -681,15 +672,15 @@
     # Initial recurrence to obtain a large enough x
     m = to_int(x)
     n = int(0.11*wp) + 2
     s = MPZ_ZERO
     x = to_fixed(x, wp)
     one = MPZ_ONE << wp
     if m < n:
-        for k in xrange(m, n):
+        for k in range(m, n):
             s -= (one << wp) // x
             x += one
     x -= one
     # Logarithmic term
     s += to_fixed(mpf_log(from_man_exp(x, -wp, wp), wp), wp)
     # Endpoint term in Euler-Maclaurin expansion
     s += (one << wp) // (2*x)
@@ -734,15 +725,15 @@
     if (not sign) and bc + exp > wp:
         return mpc_log(mpc_sub(z, mpc_one, wp), prec, rnd)
     # Initial recurrence to obtain a large enough z
     w = to_int(re)
     n = int(0.11*wp) + 2
     s = mpc_zero
     if w < n:
-        for k in xrange(w, n):
+        for k in range(w, n):
             s = mpc_sub(s, mpc_reciprocal(z, wp), wp)
             z = mpc_add_mpf(z, fone, wp)
     z = mpc_sub(z, mpc_one, wp)
     # Logarithmic and endpoint term
     s = mpc_add(s, mpc_log(z, wp), wp)
     s = mpc_add(s, mpc_div(mpc_half, z, wp), wp)
     # Euler-Maclaurin remainder sum
@@ -794,15 +785,15 @@
         if re == fnan:
             return (fnan, fnan)
     # Recurrence
     w = to_int(re)
     n = int(0.4*wp + 4*m)
     s = mpc_zero
     if w < n:
-        for k in xrange(w, n):
+        for k in range(w, n):
             t = mpc_pow_int(z, -m-1, wp)
             s = mpc_add(s, t, wp)
             z = mpc_add_mpf(z, fone, wp)
     zm = mpc_pow_int(z, -m, wp)
     z2 = mpc_pow_int(z, -2, wp)
     # 1/m*(z+N)^m
     integral_term = mpc_div_mpf(zm, from_int(m), wp)
@@ -946,15 +937,15 @@
                     t = mpf_mul(t, a, wp)
                 return mpf_div(fone, t, wp)
     # Use Borwein's algorithm
     n = int(wp/2.54 + 5)
     d = borwein_coefficients(n)
     t = MPZ_ZERO
     s = MPZ(s)
-    for k in xrange(n):
+    for k in range(n):
         t += (((-1)**k * (d[k] - d[n])) << wp) // (k+1)**s
     t = (t << wp) // (-d[n])
     t = (t << wp) // ((1 << wp) - (1 << (wp+1-s)))
     if (s in zeta_int_cache and zeta_int_cache[s][0] < wp) or (s not in zeta_int_cache):
         zeta_int_cache[s] = (wp, from_man_exp(t, -wp-wp))
     return from_man_exp(t, -wp-wp, prec, rnd)
 
@@ -1019,15 +1010,15 @@
     #wp += 16 - (prec & 15)
     # Use Borwein's algorithm
     n = int(wp/2.54 + 5)
     d = borwein_coefficients(n)
     t = MPZ_ZERO
     sf = to_fixed(s, wp)
     ln2 = ln2_fixed(wp)
-    for k in xrange(n):
+    for k in range(n):
         u = (-sf*log_int_fixed(k+1, wp, ln2)) >> wp
         #esign, eman, eexp, ebc = mpf_exp(u, wp)
         #offset = eexp + wp
         #if offset >= 0:
         #    w = ((d[k] - d[n]) * eman) << offset
         #else:
         #    w = ((d[k] - d[n]) * eman) >> (-offset)
@@ -1107,15 +1098,15 @@
     tim = MPZ_ZERO
     one = MPZ_ONE << wp
     one_2wp = MPZ_ONE << (2*wp)
     critical_line = re == fhalf
     ln2 = ln2_fixed(wp)
     pi2 = pi_fixed(wp-1)
     wp2 = wp+wp
-    for k in xrange(n):
+    for k in range(n):
         log = log_int_fixed(k+1, wp, ln2)
         # A square root is much cheaper than an exp
         if critical_line:
             w = one_2wp // isqrt_fast((k+1) << wp2)
         else:
             w = exp_fixed((-ref*log) >> wp, wp)
         if k & 1:
@@ -1170,15 +1161,15 @@
         mult = mult_cache#[:n+1]
         return sieve, primes, mult
     sieve = [0] * (n+1)
     mult = [0] * (n+1)
     primes = list_primes(n)
     for p in primes:
         #sieve[p::p] = p
-        for k in xrange(p,n+1,p):
+        for k in range(p,n+1,p):
             sieve[k] = p
     for i, p in enumerate(sieve):
         if i >= 2:
             m = 1
             n = i // p
             while not n % p:
                 n //= p
@@ -1216,15 +1207,15 @@
             tre, tim = ((pre*tre-pim*tim)>>wp), ((pim*tre+pre*tim)>>wp)
             basic_powers[p].append((tre,tim))
     xre = MPZ_ZERO
     xim = MPZ_ZERO
     if a == 1:
         xre += one
     aa = max(a,2)
-    for k in xrange(aa, a+n+1):
+    for k in range(aa, a+n+1):
         p = sieve[k]
         if p in basic_powers:
             m = mult[k]
             tre, tim = basic_powers[p][m-1]
             while 1:
                 k //= p**m
                 if k == 1:
@@ -1287,15 +1278,15 @@
     one = MPZ_ONE << wp
     one_2wp = MPZ_ONE << (2*wp)
 
     ln2 = ln2_fixed(wp)
     pi2 = pi_fixed(wp-1)
     wp2 = wp+wp
 
-    for w in xrange(a, a+n+1):
+    for w in range(a, a+n+1):
         log = log_int_fixed(w, wp, ln2)
         cos, sin = cos_sin_fixed((-sim*log)>>wp, wp, pi2)
         if critical_line:
             u = one_2wp // isqrt_fast(w<<wp2)
         else:
             u = exp_fixed((-sre*log)>>wp, wp)
         xterm_re = (u * cos) >> wp
@@ -1410,49 +1401,49 @@
         q2 = to_fixed(q2, wp)
         q2 = (k * q2 * pi) >> wp
         exps3.append((q1, q2))
         # Multiply for next round
         exp_2pi_k = mpf_mul(exp_2pi_k, exp_2pi, wp)
         k += 1
     # Exponential sum
-    for n in xrange(3, N+1, 2):
+    for n in range(3, N+1, 2):
         s = MPZ_ZERO
         k = 1
         for e1, e2 in exps3:
             if n%4 == 3:
                 t = e1 // k**n
             else:
                 U = (n-1)//4
                 t = (e1 + e2//U) // k**n
             if not t:
                 break
             s += t
             k += 1
         zeta_values[n] = -2*s
     # Even zeta values
-    B = [mpf_abs(mpf_bernoulli(k,wp)) for k in xrange(N+2)]
+    B = [mpf_abs(mpf_bernoulli(k,wp)) for k in range(N+2)]
     pi_pow = fpi = mpf_pow_int(mpf_shift(mpf_pi(wp), 1), 2, wp)
     pi_pow = mpf_div(pi_pow, from_int(4), wp)
-    for n in xrange(2,N+2,2):
+    for n in range(2,N+2,2):
         z = mpf_mul(B[n], pi_pow, wp)
         zeta_values[n] = to_fixed(z, wp)
         pi_pow = mpf_mul(pi_pow, fpi, wp)
         pi_pow = mpf_div(pi_pow, from_int((n+1)*(n+2)), wp)
     # Zeta sum
     reciprocal_pi = (one << wp) // pi
-    for n in xrange(3, N+1, 4):
+    for n in range(3, N+1, 4):
         U = (n-3)//4
         s = zeta_values[4*U+4]*(4*U+7)//4
-        for k in xrange(1, U+1):
+        for k in range(1, U+1):
             s -= (zeta_values[4*k] * zeta_values[4*U+4-4*k]) >> wp
         zeta_values[n] += (2*s*reciprocal_pi) >> wp
-    for n in xrange(5, N+1, 4):
+    for n in range(5, N+1, 4):
         U = (n-1)//4
         s = zeta_values[4*U+2]*(2*U+1)
-        for k in xrange(1, 2*U+1):
+        for k in range(1, 2*U+1):
             s += ((-1)**k*2*k* zeta_values[2*k] * zeta_values[4*U+2-2*k])>>wp
         zeta_values[n] += ((s*reciprocal_pi)>>wp)//(2*U)
     return [x>>extra for x in zeta_values]
 
 def gamma_taylor_coefficients(inprec):
     """
     Gives the Taylor coefficients of 1/gamma(1+x) as
@@ -1491,19 +1482,19 @@
 
     wp = prec + 20
     A = [0] * N
     A[0] = MPZ_ZERO
     A[1] = MPZ_ONE << wp
     A[2] = euler_fixed(wp)
     # SLOW, reference implementation
-    #zeta_values = [0,0]+[to_fixed(mpf_zeta_int(k,wp),wp) for k in xrange(2,N)]
+    #zeta_values = [0,0]+[to_fixed(mpf_zeta_int(k,wp),wp) for k in range(2,N)]
     zeta_values = zeta_array(N, wp)
-    for k in xrange(3, N):
+    for k in range(3, N):
         a = (-A[2]*A[k-1])>>wp
-        for j in xrange(2,k):
+        for j in range(2,k):
             a += ((-1)**j * zeta_values[j] * A[k-j]) >> wp
         a //= (1-k)
         A[k] = a
     A = [a>>20 for a in A]
     A = A[::-1]
     A = A[:-1]
     gamma_taylor_cache[prec] = A
@@ -1515,15 +1506,15 @@
     #n = int(x >> (wp-1))
     #steps = (n-1)>>1
     nearest_int = ((x >> (wp-1)) + MPZ_ONE) >> 1
     one = MPZ_ONE << wp
     coeffs, cwp = gamma_taylor_coefficients(wp)
     if nearest_int > 0:
         r = one
-        for i in xrange(nearest_int-1):
+        for i in range(nearest_int-1):
             x -= one
             r = (r*x) >> wp
         x -= one
         p = MPZ_ZERO
         for c in coeffs:
             p = c + ((x*p)>>wp)
         p >>= (cwp-wp)
@@ -1531,22 +1522,22 @@
             return from_man_exp((r<<wp)//p, -wp, prec, rnd)
         if type == 2:
             return mpf_shift(from_rational(p, (r<<wp), prec, rnd), wp)
         if type == 3:
             return mpf_log(mpf_abs(from_man_exp((r<<wp)//p, -wp)), prec, rnd)
     else:
         r = one
-        for i in xrange(-nearest_int):
+        for i in range(-nearest_int):
             r = (r*x) >> wp
             x += one
         p = MPZ_ZERO
         for c in coeffs:
             p = c + ((x*p)>>wp)
         p >>= (cwp-wp)
-        if wp - bitcount(abs(x)) > 10:
+        if wp - x.bit_length() > 10:
             # pass very close to 0, so do floating-point multiply
             g = mpf_add(xmpf, from_int(-nearest_int))  # exact
             r = from_man_exp(p*r,-wp-wp)
             r = mpf_mul(r, g, wp)
             if type == 0:
                 return mpf_div(fone, r, prec, rnd)
             if type == 2:
@@ -1560,15 +1551,15 @@
             if type == 3: return mpf_neg(mpf_log(mpf_abs(r), prec, rnd))
 
 def stirling_coefficient(n):
     if n in gamma_stirling_cache:
         return gamma_stirling_cache[n]
     p, q = bernfrac(n)
     q *= MPZ(n*(n-1))
-    gamma_stirling_cache[n] = p, q, bitcount(abs(p)), bitcount(q)
+    gamma_stirling_cache[n] = p, q, p.bit_length(), q.bit_length()
     return gamma_stirling_cache[n]
 
 def real_stirling_series(x, prec):
     """
     Sums the rational part of Stirling's expansion,
 
     log(sqrt(2*pi)) - z + 1/(12*z) - 1/(360*z^3) + ...
@@ -1590,16 +1581,16 @@
     s -= 3617*t//122400;   t = (t*u)>>prec
     s += 43867*t//244188;  t = (t*u)>>prec
     s -= 174611*t//125400;  t = (t*u)>>prec
     if not t: return s
     k = 22
     # From here on, the coefficients are growing, so we
     # have to keep t at a roughly constant size
-    usize = bitcount(abs(u))
-    tsize = bitcount(abs(t))
+    usize = u.bit_length()
+    tsize = t.bit_length()
     texp = 0
     while 1:
         p, q, pb, qb = stirling_coefficient(k)
         term_mag = tsize + pb + texp
         shift = -texp
         m = pb - term_mag
         if m > 0 and shift < m:
@@ -1629,43 +1620,43 @@
     ure = (tre*tre - tim*tim) >> prec
     uim = tim*tre >> (prec-1)
     # s = log(sqrt(2*pi)) - z
     sre = ln_sqrt2pi_fixed(prec) - x
     sim = -y
 
     # Add initial terms of Stirling's series
-    sre += tre//12; sim += tim//12;
+    sre += tre//12; sim += tim//12
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre -= tre//360; sim -= tim//360;
+    sre -= tre//360; sim -= tim//360
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre += tre//1260; sim += tim//1260;
+    sre += tre//1260; sim += tim//1260
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre -= tre//1680; sim -= tim//1680;
+    sre -= tre//1680; sim -= tim//1680
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
     if abs(tre) + abs(tim) < 5: return sre, sim
-    sre += tre//1188; sim += tim//1188;
+    sre += tre//1188; sim += tim//1188
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre -= 691*tre//360360; sim -= 691*tim//360360;
+    sre -= 691*tre//360360; sim -= 691*tim//360360
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre += tre//156; sim += tim//156;
+    sre += tre//156; sim += tim//156
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
     if abs(tre) + abs(tim) < 5: return sre, sim
-    sre -= 3617*tre//122400; sim -= 3617*tim//122400;
+    sre -= 3617*tre//122400; sim -= 3617*tim//122400
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre += 43867*tre//244188; sim += 43867*tim//244188;
+    sre += 43867*tre//244188; sim += 43867*tim//244188
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
-    sre -= 174611*tre//125400; sim -= 174611*tim//125400;
+    sre -= 174611*tre//125400; sim -= 174611*tim//125400
     tre, tim = ((tre*ure-tim*uim)>>prec), ((tre*uim+tim*ure)>>prec)
     if abs(tre) + abs(tim) < 5: return sre, sim
 
     k = 22
     # From here on, the coefficients are growing, so we
     # have to keep t at a roughly constant size
-    usize = bitcount(max(abs(ure), abs(uim)))
-    tsize = bitcount(max(abs(tre), abs(tim)))
+    usize = (max(abs(ure), abs(uim))).bit_length()
+    tsize = (max(abs(tre), abs(tim))).bit_length()
     texp = 0
     while 1:
         p, q, pb, qb = stirling_coefficient(k)
         term_mag = tsize + pb + texp
         shift = -texp
         m = pb - term_mag
         if m > 0 and shift < m:
@@ -1750,15 +1741,15 @@
     # Estimate log(gamma(|x|),2) as x*log(x,2)
     mag = exp + bc
     gamma_size = n*mag
 
     if type == 3:
         wp = prec + 20
     else:
-        wp = prec + bitcount(gamma_size) + 20
+        wp = prec + gamma_size.bit_length() + 20
 
     # Very close to 0, pole
     if mag < -wp:
         if type == 0:
             return mpf_sub(mpf_div(fone,x, wp),mpf_shift(fone,-wp),prec,rnd)
         if type == 1: return mpf_sub(fone, x, prec, rnd)
         if type == 2: return mpf_add(x, mpf_shift(fone,mag-wp), prec, rnd)
@@ -1810,15 +1801,15 @@
     else:           absxman = man >> (-offset)
 
     # For log gamma, provide accurate evaluation for x = 1+eps and 2+eps
     if type == 3 and not sign:
         one = MPZ_ONE << wp
         one_dist = abs(absxman-one)
         two_dist = abs(absxman-2*one)
-        cancellation = (wp - bitcount(min(one_dist, two_dist)))
+        cancellation = (wp - min(one_dist, two_dist).bit_length())
         if cancellation > 10:
             xsub1 = mpf_sub(fone, x)
             xsub2 = mpf_sub(ftwo, x)
             xsub1mag = xsub1[2]+xsub1[3]
             xsub2mag = xsub2[2]+xsub2[3]
             if xsub1mag < -wp:
                 return mpf_mul(mpf_euler(wp), mpf_sub(fone, x), prec, rnd)
@@ -1843,15 +1834,15 @@
     xorig = x
 
     # Argument reduction
     r = 0
     if n < n_for_stirling:
         r = one = MPZ_ONE << wp
         d = n_for_stirling - n
-        for k in xrange(d):
+        for k in range(d):
             r = (r * absxman) >> wp
             absxman += one
         x = xabs = from_man_exp(absxman, -wp)
         if sign:
             x = mpf_neg(x)
     else:
         xabs = mpf_abs(x)
@@ -1951,15 +1942,15 @@
     an = abs(to_int(a))
     bn = abs(to_int(b))
     absn = max(an, bn)
     gamma_size = absn*mag
     if type == 3:
         pass
     else:
-        wp += bitcount(gamma_size)
+        wp += gamma_size.bit_length()
 
     # Reflect to the right half-plane. Note that Stirling's expansion
     # is valid in the left half-plane too, as long as we're not too close
     # to the real axis, but in order to use this argument reduction
     # in the negative direction must be implemented.
     #need_reflection = asign and ((bmag < 0) or (amag-bmag > 4))
     need_reflection = asign
@@ -2036,15 +2027,15 @@
         zprered = z
         # Argument reduction
         if absn < n_for_stirling:
             absn = complex(an, bn)
             d = int((1 + n_for_stirling**2 - bn**2)**0.5 - an)
             rre = one = MPZ_ONE << wp
             rim = MPZ_ZERO
-            for k in xrange(d):
+            for k in range(d):
                 rre, rim = ((afix*rre-bfix*rim)>>wp), ((afix*rim + bfix*rre)>>wp)
                 afix += one
             r = from_man_exp(rre, -wp), from_man_exp(rim, -wp)
             a = from_man_exp(afix, -wp)
             z = a, b
 
         yre, yim = complex_stirling_series(afix, bfix, wp)
```

### Comparing `mpmath-1.3.0/mpmath/libmp/libelefun.py` & `mpmath-1.4.0a0/mpmath/libmp/libelefun.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,25 @@
 see libmpc and libmpi.
 
 """
 
 import math
 from bisect import bisect
 
-from .backend import xrange
-from .backend import MPZ, MPZ_ZERO, MPZ_ONE, MPZ_TWO, MPZ_FIVE, BACKEND
-
-from .libmpf import (
-    round_floor, round_ceiling, round_down, round_up,
-    round_nearest, round_fast,
-    ComplexResult,
-    bitcount, bctable, lshift, rshift, giant_steps, sqrt_fixed,
-    from_int, to_int, from_man_exp, to_fixed, to_float, from_float,
-    from_rational, normalize,
-    fzero, fone, fnone, fhalf, finf, fninf, fnan,
-    mpf_cmp, mpf_sign, mpf_abs,
-    mpf_pos, mpf_neg, mpf_add, mpf_sub, mpf_mul, mpf_div, mpf_shift,
-    mpf_rdiv_int, mpf_pow_int, mpf_sqrt,
-    reciprocal_rnd, negative_rnd, mpf_perturb,
-    isqrt_fast
-)
-
+from .backend import BACKEND, MPZ, MPZ_FIVE, MPZ_ONE, MPZ_TWO, MPZ_ZERO
 from .libintmath import ifib
+from .libmpf import (ComplexResult, bctable, fhalf, finf, fnan, fninf, fnone,
+                     fone, from_float, from_int, from_man_exp, from_rational,
+                     fzero, giant_steps, isqrt_fast, lshift, mpf_abs, mpf_add,
+                     mpf_cmp, mpf_div, mpf_mul, mpf_neg, mpf_perturb, mpf_pos,
+                     mpf_pow_int, mpf_rdiv_int, mpf_shift, mpf_sign, mpf_sqrt,
+                     mpf_sub, negative_rnd, normalize, reciprocal_rnd,
+                     round_ceiling, round_down, round_fast, round_floor,
+                     round_nearest, round_up, rshift, sqrt_fixed, to_fixed,
+                     to_float, to_int)
 
 
 #-------------------------------------------------------------------------------
 # Tuning parameters
 #-------------------------------------------------------------------------------
 
 # Cutoff for computing exp from cosh+sinh. This reduces the
@@ -68,15 +60,15 @@
 ATAN_TAYLOR_PREC = 3000  # Same as for log
 ATAN_TAYLOR_SHIFT = 7   # steps of size 2^-N
 atan_taylor_cache = {}
 
 
 # ~= next power of two + 20
 cache_prec_steps = [22,22]
-for k in xrange(1, bitcount(LOG_TAYLOR_PREC)+1):
+for k in range(1, LOG_TAYLOR_PREC.bit_length()+1):
     cache_prec_steps += [min(2**k,LOG_TAYLOR_PREC)+20] * 2**(k-1)
 
 
 #----------------------------------------------------------------------------#
 #                                                                            #
 #                   Elementary mathematical constants                        #
 #                                                                            #
@@ -112,15 +104,15 @@
     the fixed-point function rounds to floor.
     """
     def f(prec, rnd=round_fast):
         wp = prec + 20
         v = fixed(wp)
         if rnd in (round_up, round_ceiling):
             v += 1
-        return normalize(0, v, -wp, bitcount(v), prec, rnd)
+        return normalize(0, v, -wp, v.bit_length(), prec, rnd)
     f.__doc__ = fixed.__doc__
     return f
 
 def bsp_acot(q, a, b, hyperbolic):
     if b - a == 1:
         a1 = MPZ(2*a + 3)
         if hyperbolic or a&1:
@@ -334,30 +326,32 @@
                     reciprocal_rnd[rnd]), prec, rnd)
             return mpf_sqrt(s, prec, rnd)
         else:
             if tsign:
                 return mpf_pow_int(mpf_sqrt(s, prec+10,
                     reciprocal_rnd[rnd]), -tman, prec, rnd)
             return mpf_pow_int(mpf_sqrt(s, prec+10, rnd), tman, prec, rnd)
+    if s == fone:
+        return fone
     # General formula: s**t = exp(t*log(s))
     # TODO: handle rnd direction of the logarithm carefully
     c = mpf_log(s, prec+10, rnd)
     return mpf_exp(mpf_mul(t, c), prec, rnd)
 
 def int_pow_fixed(y, n, prec):
     """n-th power of a fixed point number with precision prec
 
        Returns the power in the form man, exp,
        man * 2**exp ~= y**n
     """
     if n == 2:
         return (y*y), 0
-    bc = bitcount(y)
+    bc = y.bit_length()
     exp = 0
-    workprec = 2 * (prec + 4*bitcount(n) + 4)
+    workprec = 2 * (prec + 4*n.bit_length() + 4)
     _, pm, pe, pbc = fone
     while 1:
         if n & 1:
             pm = pm*y
             pe = pe+exp
             pbc += bc - 2
             pbc = pbc + bctable[int(pm >> pbc)]
@@ -519,22 +513,16 @@
     intended for zeta sums.
     """
     if n in log_int_cache:
         value, vprec = log_int_cache[n]
         if vprec >= prec:
             return value >> (vprec - prec)
     wp = prec + 10
-    if wp <= LOG_TAYLOR_SHIFT:
-        if ln2 is None:
-            ln2 = ln2_fixed(wp)
-        r = bitcount(n)
-        x = n << (wp-r)
-        v = log_taylor_cached(x, wp) + r*ln2
-    else:
-        v = to_fixed(mpf_log(from_int(n), wp+5), wp)
+    assert wp > LOG_TAYLOR_SHIFT
+    v = to_fixed(mpf_log(from_int(n), wp+5), wp)
     if n < MAX_LOG_INT_CACHE:
         log_int_cache[n] = (v, wp)
     return v >> (wp-prec)
 
 def agm_fixed(a, b, prec):
     """
     Fixed-point computation of agm(a,b), assuming
@@ -602,15 +590,15 @@
     Fixed-point calculation of log(x). It is assumed that x is close
     enough to 1 for the Taylor series to converge quickly. Convergence
     can be improved by specifying r > 0 to compute
     log(x^(1/2^r))*2^r, at the cost of performing r square roots.
 
     The caller must provide sufficient guard bits.
     """
-    for i in xrange(r):
+    for i in range(r):
         x = isqrt_fast(x<<prec)
     one = MPZ_ONE << prec
     v = ((x-one)<<prec)//(x+one)
     sign = v < 0
     if sign:
         v = -v
     v2 = (v*v) >> prec
@@ -697,29 +685,29 @@
     if abs_mag <= 1:
         # Calculate t = x-1 to measure distance from 1 in bits
         tsign = 1-abs_mag
         if tsign:
             tman = (MPZ_ONE<<bc) - man
         else:
             tman = man - (MPZ_ONE<<(bc-1))
-        tbc = bitcount(tman)
+        tbc = tman.bit_length()
         cancellation = bc - tbc
         if cancellation > wp:
             t = normalize(tsign, tman, abs_mag-bc, tbc, tbc, 'n')
             return mpf_perturb(t, tsign, prec, rnd)
         else:
             wp += cancellation
         # TODO: if close enough to 1, we could use Taylor series
         # even in the AGM precision range, since the Taylor series
         # converges rapidly
     #------------------------------------------------------------------
     # Another special case:
     # n*log(2) is a good enough approximation
     if abs_mag > 10000:
-        if bitcount(abs_mag) > wp:
+        if abs_mag.bit_length() > wp:
             return from_man_exp(exp*ln2_fixed(wp), -wp, prec, rnd)
     #------------------------------------------------------------------
     # General case.
     # Perform argument reduction using log(x) = log(x*2^n) - n*log(2):
     # If we are in the Taylor precision range, choose magnitude 0 or 1.
     # If we are in the AGM precision range, choose magnitude -m for
     # some large m; benchmarking on one machine showed m = prec/20 to be
@@ -800,15 +788,15 @@
     return rshift(r, prevp-prec)
 
 def atan_taylor_get_cached(n, prec):
     # Taylor series with caching wins up to huge precisions
     # To avoid unnecessary precomputation at low precision, we
     # do it in steps
     # Round to next power of 2
-    prec2 = (1<<(bitcount(prec-1))) + 20
+    prec2 = (1<<(prec-1).bit_length()) + 20
     dprec = prec2 - prec
     if (n, prec2) in atan_taylor_cache:
         a, atan_a = atan_taylor_cache[n, prec2]
     else:
         a = n << (prec2 - ATAN_TAYLOR_SHIFT)
         atan_a = atan_newton(a, prec2)
         atan_taylor_cache[n, prec2] = (a, atan_a)
@@ -984,17 +972,17 @@
     sign, man, exp, bc = x
     if not man:
         if x == fninf:
             return fnan
         return x
     # F(2^n) ~= 2^(2^n)
     size = abs(exp+bc)
-    if exp >= 0:
+    if exp >= 0 and not sign:
         # Exact
-        if size < 10 or size <= bitcount(prec):
+        if size < 10 or size <= prec.bit_length():
             return from_int(ifib(to_int(x)), prec, rnd)
     # Use the modified Binet formula
     wp = prec + size + 20
     a = mpf_phi(wp)
     b = mpf_add(mpf_shift(a, 1), fnone, wp)
     u = mpf_pow(a, x, wp)
     v = mpf_cos_pi(x, wp)
@@ -1018,15 +1006,15 @@
     """
     if x < 0:
         x = -x
         sign = 1
     else:
         sign = 0
     r = int(0.5*prec**0.5)
-    xmag = bitcount(x) - prec
+    xmag = x.bit_length() - prec
     r = max(0, xmag + r)
     extra = 10 + 2*max(r,-xmag)
     wp = prec + extra
     x <<= (extra - r)
     one = MPZ_ONE << wp
     alt = (type == 2)
     if prec < EXP_SERIES_U_CUTOFF:
@@ -1043,43 +1031,43 @@
             c = s1 - s0 + one
         else:
             c = s1 + s0 + one
     else:
         u = int(0.3*prec**0.35)
         x2 = a = (x*x) >> wp
         xpowers = [one, x2]
-        for i in xrange(1, u):
+        for i in range(1, u):
             xpowers.append((xpowers[-1]*x2)>>wp)
         sums = [MPZ_ZERO] * u
         k = 2
         while a:
-            for i in xrange(u):
+            for i in range(u):
                 a //= (k-1)*k
                 if alt and k & 2: sums[i] -= a
                 else:             sums[i] += a
                 k += 2
             a = (a*xpowers[-1]) >> wp
-        for i in xrange(1, u):
+        for i in range(1, u):
             sums[i] = (sums[i]*xpowers[i]) >> wp
         c = sum(sums) + one
     if type == 0:
         s = isqrt_fast(c*c - (one<<wp))
         if sign:
             v = c - s
         else:
             v = c + s
-        for i in xrange(r):
+        for i in range(r):
             v = (v*v) >> wp
         return v >> extra
     else:
         # Repeatedly apply the double-angle formula
         # cosh(2*x) = 2*cosh(x)^2 - 1
         # cos(2*x) = 2*cos(x)^2 - 1
         pshift = wp-1
-        for i in xrange(r):
+        for i in range(r):
             c = ((c*c) >> pshift) - one
         # With the abs, this is the same for sinh and sin
         s = isqrt_fast(abs((one<<wp) - c*c))
         if sign:
             s = -s
         return (c>>extra), (s>>extra)
 
@@ -1343,15 +1331,15 @@
             if which == 0: return c, s
             if which == 1: return c
             if which == 2: return s
             if which == 3: return mpf_div(s, c, prec, rnd)
         # Subtract nearest half-integer (= mod by pi/2)
         n = ((man >> (-exp-2)) + 1) >> 1
         man = man - (n << (-exp-1))
-        mag2 = bitcount(man) + exp
+        mag2 = man.bit_length() + exp
         wp = prec + 10 - mag2
         offset = exp + wp
         if offset >= 0:
             t = man << offset
         else:
             t = man >> (-offset)
         t = (t*pi_fixed(wp)) >> wp
@@ -1406,23 +1394,7 @@
     n, t = divmod(x, ln2)
     n = int(n)
     v = exp_basecase(t, prec)
     if n >= 0:
         return v << n
     else:
         return v >> (-n)
-
-
-if BACKEND == 'sage':
-    try:
-        import sage.libs.mpmath.ext_libmp as _lbmp
-        mpf_sqrt = _lbmp.mpf_sqrt
-        mpf_exp = _lbmp.mpf_exp
-        mpf_log = _lbmp.mpf_log
-        mpf_cos = _lbmp.mpf_cos
-        mpf_sin = _lbmp.mpf_sin
-        mpf_pow = _lbmp.mpf_pow
-        exp_fixed = _lbmp.exp_fixed
-        cos_sin_fixed = _lbmp.cos_sin_fixed
-        log_int_fixed = _lbmp.log_int_fixed
-    except (ImportError, AttributeError):
-        print("Warning: Sage imports in libelefun failed")
```

### Comparing `mpmath-1.3.0/mpmath/libmp/libhyper.py` & `mpmath-1.4.0a0/mpmath/libmp/libhyper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 """
 This module implements computation of hypergeometric and related
 functions. In particular, it provides code for generic summation
 of hypergeometric series. Optimized versions for various special
 cases are also provided.
 """
 
-import operator
 import math
+import operator
 
-from .backend import MPZ_ZERO, MPZ_ONE, BACKEND, xrange, exec_
-
-from .libintmath import gcd
-
-from .libmpf import (\
-    ComplexResult, round_fast, round_nearest,
-    negative_rnd, bitcount, to_fixed, from_man_exp, from_int, to_int,
-    from_rational,
-    fzero, fone, fnone, ftwo, finf, fninf, fnan,
-    mpf_sign, mpf_add, mpf_abs, mpf_pos,
-    mpf_cmp, mpf_lt, mpf_le, mpf_gt, mpf_min_max,
-    mpf_perturb, mpf_neg, mpf_shift, mpf_sub, mpf_mul, mpf_div,
-    sqrt_fixed, mpf_sqrt, mpf_rdiv_int, mpf_pow_int,
-    to_rational,
-)
-
-from .libelefun import (\
-    mpf_pi, mpf_exp, mpf_log, pi_fixed, mpf_cos_sin, mpf_cos, mpf_sin,
-    mpf_sqrt, agm_fixed,
-)
-
-from .libmpc import (\
-    mpc_one, mpc_sub, mpc_mul_mpf, mpc_mul, mpc_neg, complex_int_pow,
-    mpc_div, mpc_add_mpf, mpc_sub_mpf,
-    mpc_log, mpc_add, mpc_pos, mpc_shift,
-    mpc_is_infnan, mpc_zero, mpc_sqrt, mpc_abs,
-    mpc_mpf_div, mpc_square, mpc_exp
-)
-
+from .backend import MPZ_ONE, MPZ_ZERO
+from .gammazeta import euler_fixed, mpf_euler, mpf_gamma_int
+from .libelefun import (agm_fixed, mpf_cos, mpf_cos_sin, mpf_exp, mpf_log,
+                        mpf_pi, mpf_sin, mpf_sqrt, pi_fixed)
 from .libintmath import ifac
-from .gammazeta import mpf_gamma_int, mpf_euler, euler_fixed
+from .libmpc import (complex_int_pow, mpc_abs, mpc_add, mpc_add_mpf, mpc_div,
+                     mpc_exp, mpc_is_infnan, mpc_log, mpc_mpf_div, mpc_mul,
+                     mpc_mul_mpf, mpc_neg, mpc_one, mpc_pos, mpc_shift,
+                     mpc_sqrt, mpc_square, mpc_sub, mpc_sub_mpf, mpc_zero)
+from .libmpf import (ComplexResult, finf, fnan, fninf, fnone, fone, from_int,
+                     from_man_exp, from_rational, ftwo, fzero, mpf_abs,
+                     mpf_add, mpf_cmp, mpf_div, mpf_gt, mpf_le, mpf_lt,
+                     mpf_min_max, mpf_mul, mpf_neg, mpf_perturb, mpf_pos,
+                     mpf_pow_int, mpf_rdiv_int, mpf_shift, mpf_sign, mpf_sqrt,
+                     mpf_sub, negative_rnd, round_fast, round_nearest,
+                     sqrt_fixed, to_fixed, to_int, to_rational)
+
 
 class NoConvergence(Exception):
     pass
 
 
 #-----------------------------------------------------------------------#
 #                                                                       #
@@ -123,15 +109,15 @@
     for i, flag in enumerate(param_types):
         W = ["A", "B"][i >= p]
         if flag == 'Z':
             ([aint,bint][i >= p]).append(i)
             add("%sINT_%i = coeffs[%i]" % (W, i, i))
         elif flag == 'Q':
             ([arat,brat][i >= p]).append(i)
-            add("%sP_%i, %sQ_%i = coeffs[%i]._mpq_" % (W, i, W, i, i))
+            add("%sP_%i, %sQ_%i = coeffs[%i].numerator, coeffs[%i].denominator" % (W, i, W, i, i, i))
         elif flag == 'R':
             ([areal,breal][i >= p]).append(i)
             add("xsign, xm, xe, xbc = coeffs[%i]._mpf_" % i)
             add("if xsign: xm = -xm")
             add("offset = xe + wp")
             add("if offset >= 0:")
             add("    %sREAL_%i = xm << offset" % (W, i))
@@ -161,20 +147,20 @@
     l_areal = len(areal)
     l_breal = len(breal)
     cancellable_real = min(l_areal, l_breal)
     noncancellable_real_num = areal[cancellable_real:]
     noncancellable_real_den = breal[cancellable_real:]
 
     # LOOP
-    add("for n in xrange(1,10**8):")
+    add("for n in range(1,10**8):")
 
     add("    if n in magnitude_check:")
-    add("        p_mag = bitcount(abs(PRE))")
+    add("        p_mag = PRE.bit_length()")
     if have_complex:
-        add("        p_mag = max(p_mag, bitcount(abs(PIM)))")
+        add("        p_mag = max(p_mag, PIM.bit_length())")
     add("        magnitude_check[n] = wp-p_mag")
 
     # Real factors
     multiplier = " * ".join(["AINT_#".replace("#", str(i)) for i in aint] + \
                             ["AP_#".replace("#", str(i)) for i in arat] + \
                             ["BQ_#".replace("#", str(i)) for i in brat])
 
@@ -297,36 +283,20 @@
         add("return a, False, magn")
 
     source = "\n".join(("    " + line) for line in source)
     source = ("def %s(coeffs, z, prec, wp, epsshift, magnitude_check, **kwargs):\n" % fname) + source
 
     namespace = {}
 
-    exec_(source, globals(), namespace)
+    exec(source, globals(), namespace)
 
     #print source
     return source, namespace[fname]
 
 
-if BACKEND == 'sage':
-
-    def make_hyp_summator(key):
-        """
-        Returns a function that sums a generalized hypergeometric series,
-        for given parameter types (integer, rational, real, complex).
-        """
-        from sage.libs.mpmath.ext_main import hypsum_internal
-        p, q, param_types, ztype = key
-        def _hypsum(coeffs, z, prec, wp, epsshift, magnitude_check, **kwargs):
-            return hypsum_internal(p, q, param_types, ztype, coeffs, z,
-                prec, wp, epsshift, magnitude_check, kwargs)
-
-        return "(none)", _hypsum
-
-
 #-----------------------------------------------------------------------#
 #                                                                       #
 #                              Error functions                          #
 #                                                                       #
 #-----------------------------------------------------------------------#
 
 # TODO: mpf_erf should call mpf_erfc when appropriate (currently
@@ -629,15 +599,15 @@
     if gamma:
         n = 1-n
     wp = prec + 20
     xmag = exp + bc
     # Beware of near-poles
     if xmag < -10:
         raise NotImplementedError
-    nmag = bitcount(abs(n))
+    nmag = n.bit_length()
     have_imag = n > 0 and sign
     negx = mpf_neg(x)
     # Skip series if direct convergence
     if n == 0 or 2*nmag - xmag < -wp:
         if gamma:
             v = mpf_exp(negx, wp)
             re = mpf_mul(v, mpf_pow_int(x, n_orig-1, wp), prec, rnd)
@@ -647,15 +617,15 @@
     else:
         # Finite number of terms, or...
         can_use_asymptotic_series = -3*wp < n <= 0
         # ...large enough?
         if not can_use_asymptotic_series:
             xi = abs(to_int(x))
             m = min(max(1, xi-n), 2*wp)
-            siz = -n*nmag + (m+n)*bitcount(abs(m+n)) - m*xmag - (144*m//100)
+            siz = -n*nmag + (m+n)*(m+n).bit_length() - m*xmag - (144*m//100)
             tol = -wp-10
             can_use_asymptotic_series = siz < tol
         if can_use_asymptotic_series:
             r = ((-MPZ_ONE) << (wp+wp)) // to_fixed(x, wp)
             m = n
             t = r*m
             s = MPZ_ONE << wp
@@ -915,15 +885,15 @@
 # is very small
 
 def mpf_besseljn(n, x, prec, rounding=round_fast):
     prec += 50
     negate = n < 0 and n & 1
     mag = x[2]+x[3]
     n = abs(n)
-    wp = prec + 20 + n*bitcount(n)
+    wp = prec + 20 + n*n.bit_length()
     if mag < 0:
         wp -= n * mag
     x = to_fixed(x, wp)
     x2 = (x**2) >> wp
     if not n:
         s = t = MPZ_ONE << wp
     else:
@@ -939,15 +909,15 @@
 
 def mpc_besseljn(n, z, prec, rounding=round_fast):
     negate = n < 0 and n & 1
     n = abs(n)
     origprec = prec
     zre, zim = z
     mag = max(zre[2]+zre[3], zim[2]+zim[3])
-    prec += 20 + n*bitcount(n) + abs(mag)
+    prec += 20 + n*n.bit_length() + abs(mag)
     if mag < 0:
         prec -= n * mag
     zre = to_fixed(zre, prec)
     zim = to_fixed(zim, prec)
     z2re = (zre**2 - zim**2) >> prec
     z2im = (zre*zim) >> (prec-1)
     if not n:
```

### Comparing `mpmath-1.3.0/mpmath/libmp/libintmath.py` & `mpmath-1.4.0a0/mpmath/libmp/libintmath.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 TODO: rename, cleanup, perhaps move the gmpy wrapper code
 here from settings.py
 
 """
 
 import math
+import sys
 from bisect import bisect
+from functools import lru_cache
+
+from .backend import BACKEND, MPZ, MPZ_ONE, MPZ_ZERO, gmpy
 
-from .backend import xrange
-from .backend import BACKEND, gmpy, sage, sage_utils, MPZ, MPZ_ONE, MPZ_ZERO
 
 small_trailing = [0] * 256
 for j in range(1,8):
     small_trailing[1<<j::1<<(j+1)] = [j] * (1<<(7-j))
 
 def giant_steps(start, target, n=2):
     """
@@ -50,91 +52,46 @@
 def lshift(x, n):
     """For an integer x, calculate x << n. Unlike the plain Python
     expression (x << n), n is allowed to be negative, in which case a
     right shift with default (floor) rounding is performed."""
     if n >= 0: return x << n
     else:      return x >> (-n)
 
-if BACKEND == 'sage':
-    import operator
-    rshift = operator.rshift
-    lshift = operator.lshift
-
-def python_trailing(n):
+def trailing(n):
     """Count the number of trailing zero bits in abs(n)."""
     if not n:
         return 0
     low_byte = n & 0xff
     if low_byte:
         return small_trailing[low_byte]
     t = 8
     n >>= 8
     while not n & 0xff:
         n >>= 8
         t += 8
     return t + small_trailing[n & 0xff]
 
-if BACKEND == 'gmpy':
-    if gmpy.version() >= '2':
-        def gmpy_trailing(n):
-            """Count the number of trailing zero bits in abs(n) using gmpy."""
-            if n: return MPZ(n).bit_scan1()
-            else: return 0
-    else:
-        def gmpy_trailing(n):
-            """Count the number of trailing zero bits in abs(n) using gmpy."""
-            if n: return MPZ(n).scan1()
-            else: return 0
-
-# Small powers of 2
-powers = [1<<_ for _ in range(300)]
-
-def python_bitcount(n):
-    """Calculate bit size of the nonnegative integer n."""
-    bc = bisect(powers, n)
-    if bc != 300:
-        return bc
-    bc = int(math.log(n, 2)) - 4
-    return bc + bctable[n>>bc]
-
-def gmpy_bitcount(n):
-    """Calculate bit size of the nonnegative integer n."""
-    if n: return MPZ(n).numdigits(2)
-    else: return 0
-
-#def sage_bitcount(n):
-#    if n: return MPZ(n).nbits()
-#    else: return 0
-
-def sage_trailing(n):
-    return MPZ(n).trailing_zero_bits()
+def bitcount(n):
+    """Calculate bit size of abs(n)."""
+    return MPZ(n).bit_length()
 
 if BACKEND == 'gmpy':
-    bitcount = gmpy_bitcount
-    trailing = gmpy_trailing
-elif BACKEND == 'sage':
-    sage_bitcount = sage_utils.bitcount
-    bitcount = sage_bitcount
-    trailing = sage_trailing
-else:
-    bitcount = python_bitcount
-    trailing = python_trailing
-
-if BACKEND == 'gmpy' and 'bit_length' in dir(gmpy):
     bitcount = gmpy.bit_length
+    def trailing(n):
+        return MPZ(n).bit_scan1() if n else MPZ(0)
 
 # Used to avoid slow function calls as far as possible
 trailtable = [trailing(n) for n in range(256)]
-bctable = [bitcount(n) for n in range(1024)]
+bctable = [n.bit_length() for n in range(1024)]
 
 # TODO: speed up for bases 2, 4, 8, 16, ...
 
 def bin_to_radix(x, xbits, base, bdigits):
     """Changes radix of a fixed-point number; i.e., converts
-    x * 2**xbits to floor(x * 10**bdigits)."""
+    x * 2**xbits to floor(x * base**bdigits)."""
     return x * (MPZ(base)**bdigits) >> xbits
 
 stddigits = '0123456789abcdefghijklmnopqrstuvwxyz'
 
 def small_numeral(n, base=10, digits=stddigits):
     """Return the string numeral of a positive integer in an arbitrary
     base. Most efficient for small input."""
@@ -205,24 +162,20 @@
 def isqrt_small_python(x):
     """
     Correctly (floor) rounded integer square root, using
     division. Fast up to ~200 digits.
     """
     if not x:
         return x
-    if x < _1_800:
-        # Exact with IEEE double precision arithmetic
-        if x < _1_50:
-            return int(x**0.5)
-        # Initial estimate can be any integer >= the true root; round up
-        r = int(x**0.5 * 1.00000000000001) + 1
-    else:
-        bc = bitcount(x)
-        n = bc//2
-        r = int((x>>(2*n-100))**0.5+2)<<(n-50)  # +2 is to round up
+    assert x < _1_800
+    # Exact with IEEE double precision arithmetic
+    if x < _1_50:
+        return int(x**0.5)
+    # Initial estimate can be any integer >= the true root; round up
+    r = int(x**0.5 * 1.00000000000001) + 1
     # The following iteration now precisely computes floor(sqrt(x))
     # See e.g. Crandall & Pomerance, "Prime Numbers: A Computational
     # Perspective"
     while 1:
         y = (r+x//r)>>1
         if y >= r:
             return r
@@ -251,15 +204,15 @@
         if x >= _1_100:
             y = (y + x//y) >> 1
             if x >= _1_200:
                 y = (y + x//y) >> 1
                 if x >= _1_400:
                     y = (y + x//y) >> 1
         return y
-    bc = bitcount(x)
+    bc = x.bit_length()
     guard_bits = 10
     x <<= 2*guard_bits
     bc += 2*guard_bits
     bc += (bc&1)
     hbc = bc//2
     startprec = min(50, hbc)
     # Newton iteration for 1/sqrt(x), with floating-point starting value
@@ -302,73 +255,65 @@
 
 def sqrt_fixed(x, prec):
     return isqrt_fast(x<<prec)
 
 sqrt_fixed2 = sqrt_fixed
 
 if BACKEND == 'gmpy':
-    if gmpy.version() >= '2':
-        isqrt_small = isqrt_fast = isqrt = gmpy.isqrt
-        sqrtrem = gmpy.isqrt_rem
-    else:
-        isqrt_small = isqrt_fast = isqrt = gmpy.sqrt
-        sqrtrem = gmpy.sqrtrem
-elif BACKEND == 'sage':
-    isqrt_small = isqrt_fast = isqrt = \
-        getattr(sage_utils, "isqrt", lambda n: MPZ(n).isqrt())
-    sqrtrem = lambda n: MPZ(n).sqrtrem()
+    isqrt_small = isqrt_fast = isqrt = gmpy.isqrt
+    sqrtrem = gmpy.isqrt_rem
 else:
-    isqrt_small = isqrt_small_python
-    isqrt_fast = isqrt_fast_python
-    isqrt = isqrt_python
+    if sys.version_info >= (3, 12):
+        isqrt_small = isqrt_fast = isqrt = math.isqrt
+    else:
+        isqrt_small = isqrt_small_python
+        isqrt_fast = isqrt_fast_python
+        isqrt = isqrt_python
     sqrtrem = sqrtrem_python
+    _gcd2 = math.gcd
+
+
+if sys.version_info >= (3, 9) and BACKEND == 'python':
+    gcd = math.gcd
+elif BACKEND == 'gmpy':
+    gcd = gmpy.gcd
+else:
+    def gcd(*args):
+        res = MPZ_ZERO
+        for a in args:
+            a = MPZ(a)
+            if res != MPZ_ONE:
+                res = _gcd2(res, a)
+        return res
 
 
-def ifib(n, _cache={}):
+@lru_cache(maxsize=250)
+def ifib(n):
     """Computes the nth Fibonacci number as an integer, for
     integer n."""
     if n < 0:
         return (-1)**(-n+1) * ifib(-n)
-    if n in _cache:
-        return _cache[n]
     m = n
     # Use Dijkstra's logarithmic algorithm
     # The following implementation is basically equivalent to
     # http://en.literateprograms.org/Fibonacci_numbers_(Scheme)
     a, b, p, q = MPZ_ONE, MPZ_ZERO, MPZ_ZERO, MPZ_ONE
     while n:
         if n & 1:
             aq = a*q
             a, b = b*q+aq+a*p, b*p+aq
             n -= 1
         else:
             qq = q*q
             p, q = p*p+qq, qq+2*p*q
             n >>= 1
-    if m < 250:
-        _cache[m] = b
     return b
 
 MAX_FACTORIAL_CACHE = 1000
 
-def ifac(n, memo={0:1, 1:1}):
-    """Return n factorial (for integers n >= 0 only)."""
-    f = memo.get(n)
-    if f:
-        return f
-    k = len(memo)
-    p = memo[k-1]
-    MAX = MAX_FACTORIAL_CACHE
-    while k <= n:
-        p *= k
-        if k <= MAX:
-            memo[k] = p
-        k += 1
-    return p
-
 def ifac2(n, memo_pair=[{0:1}, {1:1}]):
     """Return n!! (double factorial), integers n >= 0 only."""
     memo = memo_pair[n&1]
     f = memo.get(n)
     if f:
         return f
     k = max(memo)
@@ -379,34 +324,31 @@
         p *= k
         if k <= MAX:
             memo[k] = p
     return p
 
 if BACKEND == 'gmpy':
     ifac = gmpy.fac
-elif BACKEND == 'sage':
-    ifac = lambda n: int(sage.factorial(n))
-    ifib = sage.fibonacci
+    ifac2 = gmpy.double_fac
+    ifib = gmpy.fib
+else:
+    ifac = math.factorial
+
+ifac = lru_cache(maxsize=1024)(ifac)
 
 def list_primes(n):
     n = n + 1
-    sieve = list(xrange(n))
+    sieve = list(range(n))
     sieve[:2] = [0, 0]
-    for i in xrange(2, int(n**0.5)+1):
+    for i in range(2, int(n**0.5)+1):
         if sieve[i]:
-            for j in xrange(i**2, n, i):
+            for j in range(i**2, n, i):
                 sieve[j] = 0
     return [p for p in sieve if p]
 
-if BACKEND == 'sage':
-    # Note: it is *VERY* important for performance that we convert
-    # the list to Python ints.
-    def list_primes(n):
-        return [int(_) for _ in sage.primes(n+1)]
-
 small_odd_primes = (3,5,7,11,13,17,19,23,29,31,37,41,43,47)
 small_odd_primes_set = set(small_odd_primes)
 
 def isprime(n):
     """
     Determines whether n is a prime number. A probabilistic test is
     performed if n is very large. No special trick is used for detecting
@@ -429,15 +371,15 @@
     m = n-1
     s = trailing(m)
     d = m >> s
     def test(a):
         x = pow(a,d,n)
         if x == 1 or x == m:
             return True
-        for r in xrange(1,s):
+        for r in range(1,s):
             x = x**2 % n
             if x == m:
                 return True
         return False
     # See http://primes.utm.edu/prove/prove2_3.html
     if n < 1373653:
         witnesses = [2,3]
@@ -446,43 +388,36 @@
     else:
         witnesses = small_odd_primes
     for a in witnesses:
         if not test(a):
             return False
     return True
 
+if BACKEND == 'gmpy':
+    isprime = gmpy.is_prime
+
 def moebius(n):
     """
     Evaluates the Moebius function which is `mu(n) = (-1)^k` if `n`
     is a product of `k` distinct primes and `mu(n) = 0` otherwise.
 
     TODO: speed up using factorization
     """
     n = abs(int(n))
     if n < 2:
         return n
     factors = []
-    for p in xrange(2, n+1):
+    for p in range(2, n+1):
         if not (n % p):
             if not (n % p**2):
                 return 0
             if not sum(p % f for f in factors):
                 factors.append(p)
     return (-1)**len(factors)
 
-def gcd(*args):
-    a = 0
-    for b in args:
-        if a:
-            while b:
-                a, b = b, a % b
-        else:
-            a = b
-    return a
-
 
 #  Comment by Juan Arias de Reyna:
 #
 #  I learn this method to compute EulerE[2n] from van de Lune.
 #
 #  We apply the formula   EulerE[2n] = (-1)^n 2**(-2n) sum_{j=0}^n a(2n,2j+1)
 #
@@ -502,17 +437,16 @@
 #
 #  Important Observation: If we pretend to use the numbers
 #     EulerE[1], EulerE[2], ... , EulerE[n]
 #     it is convenient to compute first EulerE[n], since the algorithm
 #     computes first all
 #     the previous ones, and keeps them in the CACHE
 
-MAX_EULER_CACHE = 500
-
-def eulernum(m, _cache={0:MPZ_ONE}):
+@lru_cache(maxsize=500)
+def eulernum(m):
     r"""
     Computes the Euler numbers `E(n)`, which can be defined as
     coefficients of the Taylor expansion of `1/cosh x`:
 
     .. math ::
 
         \frac{1}{\cosh x} = \sum_{n=0}^\infty \frac{E_n}{n!} x^n
@@ -524,46 +458,40 @@
         >>> [int(eulernum(n)) for n in range(11)]   # test cache
         [1, 0, -1, 0, 5, 0, -61, 0, 1385, 0, -50521]
 
     """
     # for odd m > 1, the Euler numbers are zero
     if m & 1:
         return MPZ_ZERO
-    f = _cache.get(m)
-    if f:
-        return f
-    MAX = MAX_EULER_CACHE
     n = m
     a = [MPZ(_) for _ in [0,0,1,0,0,0]]
+    suma = MPZ(1)
     for  n in range(1, m+1):
         for j in range(n+1, -1, -2):
             a[j+1] = (j-1)*a[j] + (j+1)*a[j+2]
         a.append(0)
         suma = 0
         for k in range(n+1, -1, -2):
             suma += a[k+1]
-            if n <= MAX:
-                _cache[n] = ((-1)**(n//2))*(suma // 2**n)
-        if n == m:
-            return ((-1)**(n//2))*suma // 2**n
+    return ((-1)**(n//2))*suma // 2**n
 
 def stirling1(n, k):
     """
     Stirling number of the first kind.
     """
     if n < 0 or k < 0:
         raise ValueError
     if k >= n:
         return MPZ(n == k)
     if k < 1:
         return MPZ_ZERO
     L = [MPZ_ZERO] * (k+1)
     L[1] = MPZ_ONE
-    for m in xrange(2, n+1):
-        for j in xrange(min(k, m), 0, -1):
+    for m in range(2, n+1):
+        for j in range(min(k, m), 0, -1):
             L[j] = (m-1) * L[j] + L[j-1]
     return (-1)**(n+k) * L[k]
 
 def stirling2(n, k):
     """
     Stirling number of the second kind.
     """
@@ -571,14 +499,14 @@
         raise ValueError
     if k >= n:
         return MPZ(n == k)
     if k <= 1:
         return MPZ(k == 1)
     s = MPZ_ZERO
     t = MPZ_ONE
-    for j in xrange(k+1):
+    for j in range(k+1):
         if (k + j) & 1:
             s -= t * MPZ(j)**n
         else:
             s += t * MPZ(j)**n
         t = t * (k - j) // (j + 1)
     return s // ifac(k)
```

### Comparing `mpmath-1.3.0/mpmath/libmp/libmpc.py` & `mpmath-1.4.0a0/mpmath/libmp/libmpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 """
 Low-level functions for complex arithmetic.
 """
 
 import sys
 
-from .backend import MPZ, MPZ_ZERO, MPZ_ONE, MPZ_TWO, BACKEND
+from .backend import MPZ, MPZ_ONE, MPZ_TWO, MPZ_ZERO
+from .libelefun import (mpf_acos, mpf_acosh, mpf_asin, mpf_atan, mpf_atan2,
+                        mpf_cos, mpf_cos_pi, mpf_cos_sin, mpf_cos_sin_pi,
+                        mpf_cosh, mpf_cosh_sinh, mpf_exp, mpf_fibonacci,
+                        mpf_log, mpf_log_hypot, mpf_nthroot, mpf_phi, mpf_pi,
+                        mpf_pow_int, mpf_sin, mpf_sin_pi, mpf_sinh, mpf_tan,
+                        mpf_tanh)
+from .libmpf import (ComplexResult, bctable, fhalf, finf, fnan, fninf, fnone,
+                     fone, from_float, from_int, from_man_exp, ftwo, fzero,
+                     giant_steps, lshift, mpf_abs, mpf_add, mpf_ceil, mpf_div,
+                     mpf_floor, mpf_frac, mpf_hash, mpf_hypot, mpf_mul,
+                     mpf_mul_int, mpf_neg, mpf_nint, mpf_pos, mpf_rdiv_int,
+                     mpf_shift, mpf_sign, mpf_sqrt, mpf_sub, negative_rnd,
+                     normalize, reciprocal_rnd, round_ceiling, round_down,
+                     round_fast, round_floor, round_nearest, round_up, rshift,
+                     to_fixed, to_float, to_int, to_str)
 
-from .libmpf import (\
-    round_floor, round_ceiling, round_down, round_up,
-    round_nearest, round_fast, bitcount,
-    bctable, normalize, normalize1, reciprocal_rnd, rshift, lshift, giant_steps,
-    negative_rnd,
-    to_str, to_fixed, from_man_exp, from_float, to_float, from_int, to_int,
-    fzero, fone, ftwo, fhalf, finf, fninf, fnan, fnone,
-    mpf_abs, mpf_pos, mpf_neg, mpf_add, mpf_sub, mpf_mul,
-    mpf_div, mpf_mul_int, mpf_shift, mpf_sqrt, mpf_hypot,
-    mpf_rdiv_int, mpf_floor, mpf_ceil, mpf_nint, mpf_frac,
-    mpf_sign, mpf_hash,
-    ComplexResult
-)
-
-from .libelefun import (\
-    mpf_pi, mpf_exp, mpf_log, mpf_cos_sin, mpf_cosh_sinh, mpf_tan, mpf_pow_int,
-    mpf_log_hypot,
-    mpf_cos_sin_pi, mpf_phi,
-    mpf_cos, mpf_sin, mpf_cos_pi, mpf_sin_pi,
-    mpf_atan, mpf_atan2, mpf_cosh, mpf_sinh, mpf_tanh,
-    mpf_asin, mpf_acos, mpf_acosh, mpf_nthroot, mpf_fibonacci
-)
 
 # An mpc value is a (real, imag) tuple
 mpc_one = fone, fzero
 mpc_zero = fzero, fzero
 mpc_two = ftwo, fzero
 mpc_half = (fhalf, fzero)
 
@@ -61,25 +54,19 @@
         return rs + " + " + to_str(im, dps, **kwargs) + "j"
 
 def mpc_to_complex(z, strict=False, rnd=round_fast):
     re, im = z
     return complex(to_float(re, strict, rnd), to_float(im, strict, rnd))
 
 def mpc_hash(z):
-    if sys.version_info >= (3, 2):
-        re, im = z
-        h = mpf_hash(re) + sys.hash_info.imag * mpf_hash(im)
-        # Need to reduce either module 2^32 or 2^64
-        h = h % (2**sys.hash_info.width)
-        return int(h)
-    else:
-        try:
-            return hash(mpc_to_complex(z, strict=True))
-        except OverflowError:
-            return hash(z)
+    re, im = z
+    h = mpf_hash(re) + sys.hash_info.imag * mpf_hash(im)
+    # Need to reduce either module 2^32 or 2^64
+    h = h % (2**sys.hash_info.width)
+    return int(h)
 
 def mpc_conjugate(z, prec, rnd=round_fast):
     re, im = z
     return re, mpf_neg(im, prec, rnd)
 
 def mpc_is_nonzero(z):
     return z != mpc_zero
@@ -732,16 +719,18 @@
             re = mpf_sub(mpf_pi(wp), re, wp)
         else:
             re = mpf_neg(re)
     if not bsign and n == 0:
         im = mpf_neg(im)
     if bsign and n == 1:
         im = mpf_neg(im)
-    re = normalize(re[0], re[1], re[2], re[3], prec, rnd)
-    im = normalize(im[0], im[1], im[2], im[3], prec, rnd)
+    if re[3] >= 0:
+        re = normalize(re[0], re[1], re[2], re[3], prec, rnd)
+    if im[3] >= 0:
+        im = normalize(im[0], im[1], im[2], im[3], prec, rnd)
     return re, im
 
 def mpc_acos(z, prec, rnd=round_fast):
     return acos_asin(z, prec, rnd, 0)
 
 def mpc_asin(z, prec, rnd=round_fast):
     return acos_asin(z, prec, rnd, 1)
@@ -820,16 +809,7 @@
     if re == fzero:
         return mpf_exp(im, prec, rnd), fzero
     ey = mpf_exp(im, prec+10)
     c, s = mpf_cos_sin_pi(re, prec+10)
     re = mpf_mul(ey, c, prec, rnd)
     im = mpf_mul(ey, s, prec, rnd)
     return re, im
-
-
-if BACKEND == 'sage':
-    try:
-        import sage.libs.mpmath.ext_libmp as _lbmp
-        mpc_exp = _lbmp.mpc_exp
-        mpc_sqrt = _lbmp.mpc_sqrt
-    except (ImportError, AttributeError):
-        print("Warning: Sage imports in libmpc failed")
```

### Comparing `mpmath-1.3.0/mpmath/libmp/libmpf.py` & `mpmath-1.4.0a0/mpmath/libmp/libmpf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,36 @@
 """
 Low-level functions for arbitrary-precision floating-point arithmetic.
 """
 
-__docformat__ = 'plaintext'
-
 import math
-
+import sys
 from bisect import bisect
 
-import sys
 
 # Importing random is slow
 #from random import getrandbits
 getrandbits = None
 
-from .backend import (MPZ, MPZ_TYPE, MPZ_ZERO, MPZ_ONE, MPZ_TWO, MPZ_FIVE,
-    BACKEND, STRICT, HASH_MODULUS, HASH_BITS, gmpy, sage, sage_utils)
+from .backend import (BACKEND, HASH_BITS, HASH_MODULUS, MPZ, MPZ_FIVE, MPZ_ONE,
+                      MPZ_TWO, MPZ_ZERO, STRICT, gmpy)
+from .libintmath import (bctable, bin_to_radix, giant_steps, isqrt, isqrt_fast,
+                         lshift, numeral, rshift, sqrt_fixed, sqrtrem,
+                         trailing, trailtable)
 
-from .libintmath import (giant_steps,
-    trailtable, bctable, lshift, rshift, bitcount, trailing,
-    sqrt_fixed, numeral, isqrt, isqrt_fast, sqrtrem,
-    bin_to_radix)
-
-# We don't pickle tuples directly for the following reasons:
-#   1: pickle uses str() for ints, which is inefficient when they are large
-#   2: pickle doesn't work for gmpy mpzs
-# Both problems are solved by using hex()
-
-if BACKEND == 'sage':
-    def to_pickable(x):
-        sign, man, exp, bc = x
-        return sign, hex(man), exp, bc
-else:
-    def to_pickable(x):
-        sign, man, exp, bc = x
-        return sign, hex(man)[2:], exp, bc
-
-def from_pickable(x):
-    sign, man, exp, bc = x
-    return (sign, MPZ(man, 16), exp, bc)
 
 class ComplexResult(ValueError):
     pass
 
-try:
-    intern
-except NameError:
-    intern = lambda x: x
-
 # All supported rounding modes
-round_nearest = intern('n')
-round_floor = intern('f')
-round_ceiling = intern('c')
-round_up = intern('u')
-round_down = intern('d')
+round_nearest = sys.intern('n')
+round_floor = sys.intern('f')
+round_ceiling = sys.intern('c')
+round_up = sys.intern('u')
+round_down = sys.intern('d')
 round_fast = round_down
 
 def prec_to_dps(n):
     """Return number of accurate decimals that can be represented
     with a precision of n bits."""
     return max(1, int(round(int(n)/3.3219280948873626)-1))
 
@@ -76,30 +49,29 @@
     return dps + 3
 
 #----------------------------------------------------------------------------#
 #                    Some commonly needed float values                       #
 #----------------------------------------------------------------------------#
 
 # Regular number format:
-# (-1)**sign * mantissa * 2**exponent, plus bitcount of mantissa
+# (-1)**sign * mantissa * 2**exponent, plus mantissa.bit_length()
 fzero = (0, MPZ_ZERO, 0, 0)
 fnzero = (1, MPZ_ZERO, 0, 0)
 fone = (0, MPZ_ONE, 0, 1)
 fnone = (1, MPZ_ONE, 0, 1)
 ftwo = (0, MPZ_ONE, 1, 1)
 ften = (0, MPZ_FIVE, 1, 3)
 fhalf = (0, MPZ_ONE, -1, 1)
 
 # Arbitrary encoding for special numbers: zero mantissa, nonzero exponent
 fnan = (0, MPZ_ZERO, -123, -1)
 finf = (0, MPZ_ZERO, -456, -2)
 fninf = (1, MPZ_ZERO, -789, -3)
 
-# Was 1e1000; this is broken in Python 2.4
-math_float_inf = 1e300 * 1e300
+math_float_inf = 1e1000
 
 
 #----------------------------------------------------------------------------#
 #                                  Rounding                                  #
 #----------------------------------------------------------------------------#
 
 # This function can be used to round a mantissa generally. However,
@@ -157,15 +129,15 @@
     direction if its size exceeds the precision. Trailing zero bits
     are also stripped from the mantissa to ensure that the
     representation is canonical.
 
     Conditions on the input:
     * The input must represent a regular (finite) number
     * The sign bit must be 0 or 1
-    * The mantissa must be positive
+    * The mantissa must be nonnegative
     * The exponent must be an integer
     * The bitcount must be exact
 
     If these conditions are not met, use from_man_exp, mpf_pos, or any
     of the conversion functions to create normalized raw mpf tuples.
     """
     if not man:
@@ -183,154 +155,92 @@
             man >>= n
         else:
             man = -((-man)>>n)
         exp += n
         bc = prec
     # Strip trailing bits
     if not man & 1:
-        t = trailtable[int(man & 255)]
-        if not t:
-            while not man & 255:
-                man >>= 8
-                exp += 8
-                bc -= 8
-            t = trailtable[int(man & 255)]
-        man >>= t
-        exp += t
-        bc -= t
-    # Bit count can be wrong if the input mantissa was 1 less than
-    # a power of 2 and got rounded up, thereby adding an extra bit.
-    # With trailing bits removed, all powers of two have mantissa 1,
-    # so this is easy to check for.
-    if man == 1:
-        bc = 1
-    return sign, man, exp, bc
-
-def _normalize1(sign, man, exp, bc, prec, rnd):
-    """same as normalize, but with the added condition that
-       man is odd or zero
-    """
-    if not man:
-        return fzero
-    if bc <= prec:
-        return sign, man, exp, bc
-    n = bc - prec
-    if rnd == round_nearest:
-        t = man >> (n-1)
-        if t & 1 and ((t & 2) or (man & h_mask[n<300][n])):
-            man = (t>>1)+1
-        else:
-            man = t>>1
-    elif shifts_down[rnd][sign]:
-        man >>= n
-    else:
-        man = -((-man)>>n)
-    exp += n
-    bc = prec
-    # Strip trailing bits
-    if not man & 1:
-        t = trailtable[int(man & 255)]
+        t = trailtable[man & 255]
         if not t:
             while not man & 255:
                 man >>= 8
                 exp += 8
                 bc -= 8
-            t = trailtable[int(man & 255)]
+            t = trailtable[man & 255]
         man >>= t
         exp += t
         bc -= t
     # Bit count can be wrong if the input mantissa was 1 less than
     # a power of 2 and got rounded up, thereby adding an extra bit.
     # With trailing bits removed, all powers of two have mantissa 1,
     # so this is easy to check for.
     if man == 1:
         bc = 1
     return sign, man, exp, bc
 
-try:
-    _exp_types = (int, long)
-except NameError:
-    _exp_types = (int,)
+_exp_types = (int,)
 
 def strict_normalize(sign, man, exp, bc, prec, rnd):
     """Additional checks on the components of an mpf. Enable tests by setting
        the environment variable MPMATH_STRICT to Y."""
-    assert type(man) == MPZ_TYPE
+    assert type(man) == MPZ
     assert type(bc) in _exp_types
     assert type(exp) in _exp_types
-    assert bc == bitcount(man)
+    assert bc == man.bit_length()
+    assert man >= 0
     return _normalize(sign, man, exp, bc, prec, rnd)
 
-def strict_normalize1(sign, man, exp, bc, prec, rnd):
-    """Additional checks on the components of an mpf. Enable tests by setting
-       the environment variable MPMATH_STRICT to Y."""
-    assert type(man) == MPZ_TYPE
-    assert type(bc) in _exp_types
-    assert type(exp) in _exp_types
-    assert bc == bitcount(man)
-    assert (not man) or (man & 1)
-    return _normalize1(sign, man, exp, bc, prec, rnd)
-
-if BACKEND == 'gmpy' and '_mpmath_normalize' in dir(gmpy):
+if BACKEND == 'gmpy':
     _normalize = gmpy._mpmath_normalize
-    _normalize1 = gmpy._mpmath_normalize
-
-if BACKEND == 'sage':
-    _normalize = _normalize1 = sage_utils.normalize
 
 if STRICT:
     normalize = strict_normalize
-    normalize1 = strict_normalize1
 else:
     normalize = _normalize
-    normalize1 = _normalize1
 
 #----------------------------------------------------------------------------#
 #                            Conversion functions                            #
 #----------------------------------------------------------------------------#
 
 def from_man_exp(man, exp, prec=None, rnd=round_fast):
     """Create raw mpf from (man, exp) pair. The mantissa may be signed.
     If no precision is specified, the mantissa is stored exactly."""
     man = MPZ(man)
     sign = 0
     if man < 0:
         sign = 1
         man = -man
     if man < 1024:
-        bc = bctable[int(man)]
+        bc = bctable[man]
     else:
-        bc = bitcount(man)
+        bc = man.bit_length()
     if not prec:
         if not man:
             return fzero
         if not man & 1:
             if man & 2:
                 return (sign, man >> 1, exp + 1, bc - 1)
-            t = trailtable[int(man & 255)]
+            t = trailtable[man & 255]
             if not t:
                 while not man & 255:
                     man >>= 8
                     exp += 8
                     bc -= 8
-                t = trailtable[int(man & 255)]
+                t = trailtable[man & 255]
             man >>= t
             exp += t
             bc -= t
         return (sign, man, exp, bc)
     return normalize(sign, man, exp, bc, prec, rnd)
 
 int_cache = dict((n, from_man_exp(n, 0)) for n in range(-10, 257))
 
-if BACKEND == 'gmpy' and '_mpmath_create' in dir(gmpy):
+if BACKEND == 'gmpy':
     from_man_exp = gmpy._mpmath_create
 
-if BACKEND == 'sage':
-    from_man_exp = sage_utils.from_man_exp
-
 def from_int(n, prec=0, rnd=round_fast):
     """Create a raw mpf from an integer. If no precision is specified,
     the mantissa is stored exactly."""
     if not prec:
         if n in int_cache:
             return int_cache[n]
     return from_man_exp(n, 0, prec, rnd)
@@ -408,39 +318,31 @@
     return mpf_sub(s, mpf_floor(s), prec, rnd)
 
 def from_float(x, prec=53, rnd=round_fast):
     """Create a raw mpf from a Python float, rounding if necessary.
     If prec >= 53, the result is guaranteed to represent exactly the
     same number as the input. If prec is not specified, use prec=53."""
     # frexp only raises an exception for nan on some platforms
-    if x != x:
-        return fnan
-    # in Python2.5 math.frexp gives an exception for float infinity
-    # in Python2.6 it returns (float infinity, 0)
-    try:
-        m, e = math.frexp(x)
-    except:
-        if x == math_float_inf: return finf
-        if x == -math_float_inf: return fninf
-        return fnan
+    if x != x: return fnan
     if x == math_float_inf: return finf
     if x == -math_float_inf: return fninf
-    return from_man_exp(int(m*(1<<53)), e-53, prec, rnd)
+    m, e = math.frexp(x)
+    return from_man_exp(MPZ(m*(1<<53)), e-53, prec, rnd)
 
 def from_npfloat(x, prec=113, rnd=round_fast):
     """Create a raw mpf from a numpy float, rounding if necessary.
     If prec >= 113, the result is guaranteed to represent exactly the
     same number as the input. If prec is not specified, use prec=113."""
     y = float(x)
     if x == y: # ldexp overflows for float16
         return from_float(y, prec, rnd)
     import numpy as np
     if np.isfinite(x):
         m, e = np.frexp(x)
-        return from_man_exp(int(np.ldexp(m, 113)), int(e-113), prec, rnd)
+        return from_man_exp(int(np.ldexp(m, 113)), e-113, prec, rnd)
     if np.isposinf(x): return finf
     if np.isneginf(x): return fninf
     return fnan
 
 def from_Decimal(x, prec=None, rnd=round_fast):
     """Create a raw mpf from a Decimal, rounding if necessary.
     If prec is not specified, use the equivalent bit precision
@@ -449,16 +351,16 @@
     if x.is_infinite(): return fninf if x.is_signed() else finf
     if prec is None:
         prec = int(len(x.as_tuple()[1])*3.3219280948873626)
     return from_str(str(x), prec, rnd)
 
 def to_float(s, strict=False, rnd=round_fast):
     """
-    Convert a raw mpf to a Python float. The result is exact if the
-    bitcount of s is <= 53 and no underflow/overflow occurs.
+    Convert a raw mpf to a Python float. The result is exact if
+    s.bit_length() <= 53 and no underflow/overflow occurs.
 
     If the number is too large or too small to represent as a regular
     float, it will be converted to inf or 0.0. Setting strict=True
     forces an OverflowError to be raised instead.
 
     Warning: with a directed rounding mode, the correct nearest representable
     floating-point number in the specified direction might not be computed
@@ -467,15 +369,15 @@
     sign, man, exp, bc = s
     if not man:
         if s == fzero: return 0.0
         if s == finf: return math_float_inf
         if s == fninf: return -math_float_inf
         return math_float_inf/math_float_inf
     if bc > 53:
-        sign, man, exp, bc = normalize1(sign, man, exp, bc, 53, rnd)
+        sign, man, exp, bc = normalize(sign, man, exp, bc, 53, rnd)
     if sign:
         man = -man
     try:
         return math.ldexp(man, exp)
     except OverflowError:
         if strict:
             raise
@@ -492,23 +394,25 @@
     """Create a raw mpf from a rational number p/q, round if
     necessary."""
     return mpf_div(from_int(p), from_int(q), prec, rnd)
 
 def to_rational(s):
     """Convert a raw mpf to a rational number. Return integers (p, q)
     such that s = p/q exactly."""
+    if s == fnan:
+        raise ValueError("cannot convert nan to a rational number")
+    if s in (finf, fninf):
+        raise OverflowError("cannot convert infinity to a rational number")
     sign, man, exp, bc = s
     if sign:
         man = -man
-    if bc == -1:
-        raise ValueError("cannot convert %s to a rational number" % man)
     if exp >= 0:
-        return man * (1<<exp), 1
+        return man * (1<<exp), MPZ(1)
     else:
-        return man, 1<<(-exp)
+        return man, MPZ(1)<<(-exp)
 
 def to_fixed(s, prec):
     """Convert a raw mpf to a fixed-point big integer"""
     sign, man, exp, bc = s
     offset = exp + prec
     if sign:
         if offset >= 0: return (-man) << offset
@@ -540,40 +444,30 @@
     if not s[1] or not t[1]:
         if s == fnan or t == fnan:
             return False
     return s == t
 
 def mpf_hash(s):
     # Duplicate the new hash algorithm introduces in Python 3.2.
-    if sys.version_info >= (3, 2):
-        ssign, sman, sexp, sbc = s
+    ssign, sman, sexp, sbc = s
 
-        # Handle special numbers
-        if not sman:
-            if s == fnan: return sys.hash_info.nan
-            if s == finf: return sys.hash_info.inf
-            if s == fninf: return -sys.hash_info.inf
-        h = sman % HASH_MODULUS
-        if sexp >= 0:
-            sexp = sexp % HASH_BITS
-        else:
-            sexp = HASH_BITS - 1 - ((-1 - sexp) % HASH_BITS)
-        h = (h << sexp) % HASH_MODULUS
-        if ssign: h = -h
-        if h == -1: h = -2
-        return int(h)
+    # Handle special numbers
+    if not sman:
+        if s == fnan: return sys.hash_info.nan
+        if s == finf: return sys.hash_info.inf
+        if s == fninf: return -sys.hash_info.inf
+    h = sman % HASH_MODULUS
+    if sexp >= 0:
+        sexp = sexp % HASH_BITS
     else:
-        try:
-            # Try to be compatible with hash values for floats and ints
-            return hash(to_float(s, strict=1))
-        except OverflowError:
-            # We must unfortunately sacrifice compatibility with ints here.
-            # We could do hash(man << exp) when the exponent is positive, but
-            # this would cause unreasonable inefficiency for large numbers.
-            return hash(s)
+        sexp = HASH_BITS - 1 - ((-1 - sexp) % HASH_BITS)
+    h = (h << sexp) % HASH_MODULUS
+    if ssign: h = -h
+    if h == -1: h = -2
+    return int(h)
 
 def mpf_cmp(s, t):
     """Compare the raw mpfs s and t. Return -1 if s < t, 0 if s == t,
     and 1 if s > t. (Same convention as Python's cmp() function.)"""
 
     # In principle, a comparison amounts to determining the sign of s-t.
     # A full subtraction is relatively slow, however, so we first try to
@@ -653,45 +547,45 @@
 def mpf_pos(s, prec=0, rnd=round_fast):
     """Calculate 0+s for a raw mpf (i.e., just round s to the specified
     precision)."""
     if prec:
         sign, man, exp, bc = s
         if (not man) and exp:
             return s
-        return normalize1(sign, man, exp, bc, prec, rnd)
+        return normalize(sign, man, exp, bc, prec, rnd)
     return s
 
 def mpf_neg(s, prec=None, rnd=round_fast):
     """Negate a raw mpf (return -s), rounding the result to the
     specified precision. The prec argument can be omitted to do the
     operation exactly."""
     sign, man, exp, bc = s
     if not man:
         if exp:
             if s == finf: return fninf
             if s == fninf: return finf
         return s
     if not prec:
         return (1-sign, man, exp, bc)
-    return normalize1(1-sign, man, exp, bc, prec, rnd)
+    return normalize(1-sign, man, exp, bc, prec, rnd)
 
 def mpf_abs(s, prec=None, rnd=round_fast):
     """Return abs(s) of the raw mpf s, rounded to the specified
     precision. The prec argument can be omitted to generate an
     exact result."""
     sign, man, exp, bc = s
     if (not man) and exp:
         if s == fninf:
             return finf
         return s
     if not prec:
         if sign:
             return (0, man, exp, bc)
         return s
-    return normalize1(0, man, exp, bc, prec, rnd)
+    return normalize(0, man, exp, bc, prec, rnd)
 
 def mpf_sign(s):
     """Return -1, 0, or 1 (as a Python int, not a raw mpf) depending on
     whether s is negative, zero, or positive. (Nan is taken to give 0.)"""
     sign, man, exp, bc = s
     if not man:
         if s == finf: return 1
@@ -719,83 +613,83 @@
                 if offset > 100 and prec:
                     delta = sbc + sexp - tbc - texp
                     if delta > prec + 4:
                         offset = prec + 4
                         sman <<= offset
                         if tsign == ssign: sman += 1
                         else:              sman -= 1
-                        return normalize1(ssign, sman, sexp-offset,
-                            bitcount(sman), prec, rnd)
+                        return normalize(ssign, sman, sexp-offset,
+                                         sman.bit_length(), prec, rnd)
                 # Add
                 if ssign == tsign:
                     man = tman + (sman << offset)
                 # Subtract
                 else:
                     if ssign: man = tman - (sman << offset)
                     else:     man = (sman << offset) - tman
                     if man >= 0:
                         ssign = 0
                     else:
                         man = -man
                         ssign = 1
-                bc = bitcount(man)
-                return normalize1(ssign, man, texp, bc, prec or bc, rnd)
+                bc = man.bit_length()
+                return normalize(ssign, man, texp, bc, prec or bc, rnd)
             elif offset < 0:
                 # Outside precision range; only need to perturb
                 if offset < -100 and prec:
                     delta = tbc + texp - sbc - sexp
                     if delta > prec + 4:
                         offset = prec + 4
                         tman <<= offset
                         if ssign == tsign: tman += 1
                         else:              tman -= 1
-                        return normalize1(tsign, tman, texp-offset,
-                            bitcount(tman), prec, rnd)
+                        return normalize(tsign, tman, texp-offset,
+                            tman.bit_length(), prec, rnd)
                 # Add
                 if ssign == tsign:
                     man = sman + (tman << -offset)
                 # Subtract
                 else:
                     if tsign: man = sman - (tman << -offset)
                     else:     man = (tman << -offset) - sman
                     if man >= 0:
                         ssign = 0
                     else:
                         man = -man
                         ssign = 1
-                bc = bitcount(man)
-                return normalize1(ssign, man, sexp, bc, prec or bc, rnd)
+                bc = man.bit_length()
+                return normalize(ssign, man, sexp, bc, prec or bc, rnd)
         # Equal exponents; no shifting necessary
         if ssign == tsign:
             man = tman + sman
         else:
             if ssign: man = tman - sman
             else:     man = sman - tman
             if man >= 0:
                 ssign = 0
             else:
                 man = -man
                 ssign = 1
-        bc = bitcount(man)
+        bc = man.bit_length()
         return normalize(ssign, man, texp, bc, prec or bc, rnd)
     # Handle zeros and special numbers
     if _sub:
         t = mpf_neg(t)
     if not sman:
         if sexp:
             if s == t or tman or not texp:
                 return s
             return fnan
         if tman:
-            return normalize1(tsign, tman, texp, tbc, prec or tbc, rnd)
+            return normalize(tsign, tman, texp, tbc, prec or tbc, rnd)
         return t
     if texp:
         return t
     if sman:
-        return normalize1(ssign, sman, sexp, sbc, prec or sbc, rnd)
+        return normalize(ssign, sman, sexp, sbc, prec or sbc, rnd)
     return s
 
 def mpf_sub(s, t, prec=0, rnd=round_fast):
     """Return the difference of two raw mpfs, s-t. This function is
     simply a wrapper of mpf_add that changes the sign of t."""
     return mpf_add(s, t, prec, rnd, 1)
 
@@ -820,15 +714,15 @@
             if xsign and not absolute:
                 xman = -xman
             delta = xexp - exp
             if xexp >= exp:
                 # x much larger than existing sum?
                 # first: quick test
                 if (delta > max_extra_prec) and \
-                    ((not man) or delta-bitcount(abs(man)) > max_extra_prec):
+                    ((not man) or delta-man.bit_length() > max_extra_prec):
                     man = xman
                     exp = xexp
                 else:
                     man += (xman << delta)
             else:
                 delta = -delta
                 # x much smaller than existing sum?
@@ -843,24 +737,24 @@
                 x = mpf_abs(x)
             special = mpf_add(special or fzero, x, 1)
     # Will be inf or nan
     if special:
         return special
     return from_man_exp(man, exp, prec, rnd)
 
-def gmpy_mpf_mul(s, t, prec=0, rnd=round_fast):
+def mpf_mul(s, t, prec=0, rnd=round_fast):
     """Multiply two raw mpfs"""
     ssign, sman, sexp, sbc = s
     tsign, tman, texp, tbc = t
     sign = ssign ^ tsign
     man = sman*tman
     if man:
-        bc = bitcount(man)
+        bc = man.bit_length()
         if prec:
-            return normalize1(sign, man, sexp+texp, bc, prec, rnd)
+            return normalize(sign, man, sexp+texp, bc, prec, rnd)
         else:
             return (sign, man, sexp+texp, bc)
     s_special = (not sman) and sexp
     t_special = (not tman) and texp
     if not s_special and not t_special:
         return fzero
     if fnan in (s, t): return fnan
@@ -875,63 +769,39 @@
         return mpf_mul(s, from_int(n), prec, rnd)
     if not n:
         return fzero
     if n < 0:
         sign ^= 1
         n = -n
     man *= n
-    return normalize(sign, man, exp, bitcount(man), prec, rnd)
-
-def python_mpf_mul(s, t, prec=0, rnd=round_fast):
-    """Multiply two raw mpfs"""
-    ssign, sman, sexp, sbc = s
-    tsign, tman, texp, tbc = t
-    sign = ssign ^ tsign
-    man = sman*tman
-    if man:
-        bc = sbc + tbc - 1
-        bc += int(man>>bc)
-        if prec:
-            return normalize1(sign, man, sexp+texp, bc, prec, rnd)
-        else:
-            return (sign, man, sexp+texp, bc)
-    s_special = (not sman) and sexp
-    t_special = (not tman) and texp
-    if not s_special and not t_special:
-        return fzero
-    if fnan in (s, t): return fnan
-    if (not tman) and texp: s, t = t, s
-    if t == fzero: return fnan
-    return {1:finf, -1:fninf}[mpf_sign(s) * mpf_sign(t)]
+    return normalize(sign, man, exp, man.bit_length(), prec, rnd)
 
 def python_mpf_mul_int(s, n, prec, rnd=round_fast):
     """Multiply by a Python integer."""
     sign, man, exp, bc = s
     if not man:
         return mpf_mul(s, from_int(n), prec, rnd)
     if not n:
         return fzero
     if n < 0:
         sign ^= 1
         n = -n
     man *= n
     # Generally n will be small
     if n < 1024:
-        bc += bctable[int(n)] - 1
+        bc += bctable[n] - 1
     else:
-        bc += bitcount(n) - 1
-    bc += int(man>>bc)
+        bc += n.bit_length() - 1
+    bc += man>>bc
     return normalize(sign, man, exp, bc, prec, rnd)
 
 
 if BACKEND == 'gmpy':
-    mpf_mul = gmpy_mpf_mul
     mpf_mul_int = gmpy_mpf_mul_int
 else:
-    mpf_mul = python_mpf_mul
     mpf_mul_int = python_mpf_mul_int
 
 def mpf_shift(s, n):
     """Quickly multiply the raw mpf s by 2**n without rounding."""
     sign, man, exp, bc = s
     if not man:
         return s
@@ -967,47 +837,49 @@
         if not t_special:
             if t == fzero:
                 return fnan
             return {1:finf, -1:fninf}[mpf_sign(s) * mpf_sign(t)]
         return fzero
     sign = ssign ^ tsign
     if tman == 1:
-        return normalize1(sign, sman, sexp-texp, sbc, prec, rnd)
+        return normalize(sign, sman, sexp-texp, sbc, prec, rnd)
     # Same strategy as for addition: if there is a remainder, perturb
     # the result a few bits outside the precision range before rounding
     extra = prec - sbc + tbc + 5
     if extra < 5:
         extra = 5
     quot, rem = divmod(sman<<extra, tman)
     if rem:
         quot = (quot<<1) + 1
         extra += 1
-        return normalize1(sign, quot, sexp-texp-extra, bitcount(quot), prec, rnd)
-    return normalize(sign, quot, sexp-texp-extra, bitcount(quot), prec, rnd)
+        return normalize(sign, quot, sexp-texp-extra, quot.bit_length(), prec, rnd)
+    return normalize(sign, quot, sexp-texp-extra, quot.bit_length(), prec, rnd)
 
 def mpf_rdiv_int(n, t, prec, rnd=round_fast):
     """Floating-point division n/t with a Python integer as numerator"""
     sign, man, exp, bc = t
     if not n or not man:
         return mpf_div(from_int(n), t, prec, rnd)
     if n < 0:
         sign ^= 1
         n = -n
     extra = prec + bc + 5
     quot, rem = divmod(n<<extra, man)
     if rem:
         quot = (quot<<1) + 1
         extra += 1
-        return normalize1(sign, quot, -exp-extra, bitcount(quot), prec, rnd)
-    return normalize(sign, quot, -exp-extra, bitcount(quot), prec, rnd)
+        return normalize(sign, quot, -exp-extra, quot.bit_length(), prec, rnd)
+    return normalize(sign, quot, -exp-extra, quot.bit_length(), prec, rnd)
 
 def mpf_mod(s, t, prec, rnd=round_fast):
     ssign, sman, sexp, sbc = s
     tsign, tman, texp, tbc = t
     if ((not sman) and sexp) or ((not tman) and texp):
+        if t == finf or t == fninf:
+            return s
         return fnan
     # Important special case: do nothing if t is larger
     if ssign == tsign and texp > sexp+sbc:
         return s
     # Another important special case: this allows us to do e.g. x % 1.0
     # to find the fractional part of x, and it will work when x is huge.
     if tman == 1 and sexp > texp+tbc:
@@ -1017,15 +889,15 @@
     tman = (-1)**tsign * tman
     man = (sman << (sexp-base)) % (tman << (texp-base))
     if man >= 0:
         sign = 0
     else:
         man = -man
         sign = 1
-    return normalize(sign, man, base, bitcount(man), prec, rnd)
+    return normalize(sign, man, base, man.bit_length(), prec, rnd)
 
 reciprocal_rnd = {
   round_down : round_up,
   round_up : round_down,
   round_floor : round_ceiling,
   round_ceiling : round_floor,
   round_nearest : round_nearest
@@ -1042,79 +914,81 @@
 def mpf_pow_int(s, n, prec, rnd=round_fast):
     """Compute s**n, where s is a raw mpf and n is a Python integer."""
     sign, man, exp, bc = s
 
     if (not man) and exp:
         if s == finf:
             if n > 0: return s
-            if n == 0: return fnan
+            if n == 0: return fone
             return fzero
         if s == fninf:
             if n > 0: return [finf, fninf][n & 1]
-            if n == 0: return fnan
+            if n == 0: return fone
             return fzero
+        if n == 0:
+            return fone
         return fnan
 
     n = int(n)
     if n == 0: return fone
     if n == 1: return mpf_pos(s, prec, rnd)
     if n == 2:
         _, man, exp, bc = s
         if not man:
             return fzero
         man = man*man
         if man == 1:
             return (0, MPZ_ONE, exp+exp, 1)
         bc = bc + bc - 2
-        bc += bctable[int(man>>bc)]
-        return normalize1(0, man, exp+exp, bc, prec, rnd)
+        bc += bctable[man>>bc]
+        return normalize(0, man, exp+exp, bc, prec, rnd)
     if n == -1: return mpf_div(fone, s, prec, rnd)
     if n < 0:
         inverse = mpf_pow_int(s, -n, prec+5, reciprocal_rnd[rnd])
         return mpf_div(fone, inverse, prec, rnd)
 
     result_sign = sign & n
 
     # Use exact integer power when the exact mantissa is small
     if man == 1:
         return (result_sign, MPZ_ONE, exp*n, 1)
     if bc*n < 1000:
         man **= n
-        return normalize1(result_sign, man, exp*n, bitcount(man), prec, rnd)
+        return normalize(result_sign, man, exp*n, man.bit_length(), prec, rnd)
 
     # Use directed rounding all the way through to maintain rigorous
     # bounds for interval arithmetic
     rounds_down = (rnd == round_nearest) or \
         shifts_down[rnd][result_sign]
 
     # Now we perform binary exponentiation. Need to estimate precision
     # to avoid rounding errors from temporary operations. Roughly log_2(n)
     # operations are performed.
-    workprec = prec + 4*bitcount(n) + 4
+    workprec = prec + 4*n.bit_length() + 4
     _, pm, pe, pbc = fone
     while 1:
         if n & 1:
             pm = pm*man
             pe = pe+exp
             pbc += bc - 2
-            pbc = pbc + bctable[int(pm >> pbc)]
+            pbc = pbc + bctable[pm >> pbc]
             if pbc > workprec:
                 if rounds_down:
                     pm = pm >> (pbc-workprec)
                 else:
                     pm = -((-pm) >> (pbc-workprec))
                 pe += pbc - workprec
                 pbc = workprec
             n -= 1
             if not n:
                 break
         man = man*man
         exp = exp+exp
         bc = bc + bc - 2
-        bc = bc + bctable[int(man >> bc)]
+        bc = bc + bctable[man >> bc]
         if bc > workprec:
             if rounds_down:
                 man = man >> (bc-workprec)
             else:
                 man = -((-man) >> (bc-workprec))
             exp += bc - workprec
             bc = workprec
@@ -1172,18 +1046,19 @@
     bitprec = int(dps * math.log(10,2)) + 10
 
     # Cut down to size
     # TODO: account for precision when doing this
     exp_from_1 = exp + bc
     if abs(exp_from_1) > 3500:
         from .libelefun import mpf_ln2, mpf_ln10
+
         # Set b = int(exp * log(2)/log(10))
         # If exp is huge, we must use high-precision arithmetic to
         # find the nearest power of ten
-        expprec = bitcount(abs(exp)) + 5
+        expprec = exp.bit_length() + 5
         tmp = from_int(exp)
         tmp = mpf_mul(tmp, mpf_ln2(expprec))
         tmp = mpf_div(tmp, mpf_ln10(expprec), expprec)
         b = to_int(tmp)
         s = mpf_div(s, mpf_pow_int(ften, b, bitprec), bitprec)
         _sign, man, exp, bc = s
         exponent = b
@@ -1214,15 +1089,15 @@
     (default = min(-dps/3,-5)) and max_fixed (default = dps).
 
     To force fixed-point format always, set min_fixed = -inf,
     max_fixed = +inf. To force floating-point format, set
     min_fixed >= max_fixed.
 
     The literal is formatted so that it can be parsed back to a number
-    by to_str, float() or Decimal().
+    by from_str, float() or Decimal().
     """
 
     # Special numbers
     if not s[1]:
         if s == fzero:
             if dps: t = '0.0'
             else:   t = '.0'
@@ -1261,15 +1136,15 @@
                 exponent += 1
         else:
             digits = digits[:dps]
 
         # Prettify numbers close to unit magnitude
         if min_fixed < exponent < max_fixed:
             if exponent < 0:
-                digits = ("0"*int(-exponent)) + digits
+                digits = ("0"*(-exponent)) + digits
                 split = 1
             else:
                 split = exponent + 1
                 if split > dps:
                     digits += "0"*(split-dps)
             exponent = 0
         else:
@@ -1285,84 +1160,95 @@
 
     if exponent == 0 and dps and not show_zero_exponent: return sign + digits
     if exponent >= 0: return sign + digits + "e+" + str(exponent)
     if exponent < 0: return sign + digits + "e" + str(exponent)
 
 def str_to_man_exp(x, base=10):
     """Helper function for from_str."""
-    x = x.lower().rstrip('l')
-    # Verify that the input is a valid float literal
-    float(x)
+    x = x.lower().rstrip('l').replace('_', '')
     # Split into mantissa, exponent
-    parts = x.split('e')
+    if base <= 10:
+        sep = 'e'
+    else:
+        sep = '@'
+    if pow(2, e2 := int(math.log2(base))) == base and e2 in [1, 4] and x.find('p') >= 0:
+        sep = 'p'
+    parts = x.split(sep)
     if len(parts) == 1:
         exp = 0
     else: # == 2
         x = parts[0]
         exp = int(parts[1])
     # Look for radix point in mantissa
     parts = x.split('.')
     if len(parts) == 2:
         a, b = parts[0], parts[1].rstrip('0')
-        exp -= len(b)
+        if sep != 'p':
+            exp -= len(b)
+        else:
+            exp -= len(b)*e2
+        if a == '':
+            a = '0'
         x = a + b
-    x = MPZ(int(x, base))
+    x = x.replace(' ', '').replace('+', '')  # workaround aleaxit/gmpy#381
+    x = MPZ(x, base)
     return x, exp
 
 special_str = {'inf':finf, '+inf':finf, '-inf':fninf, 'nan':fnan}
 
-def from_str(x, prec, rnd=round_fast):
-    """Create a raw mpf from a decimal literal, rounding in the
+def from_str(x, prec=0, rnd=round_fast, base=0):
+    """Create a raw mpf from a string x in a given base, rounding in the
     specified direction if the input number cannot be represented
     exactly as a binary floating-point number with the given number of
-    bits. The literal syntax accepted is the same as for Python
-    floats.
+    bits.  The string syntax accepted for float() or float.fromhex()
+    is accepted too.
 
     TODO: the rounding does not work properly for large exponents.
     """
     x = x.lower().strip()
     if x in special_str:
         return special_str[x]
 
+    if not base:
+        if x.startswith(('0b', '-0b', '0B', '-0B')):
+            base = 2
+        elif x.startswith(('0x', '-0x', '0X', '-0X')):
+            base = 16
+        elif x.startswith(('0o', '-0o')):
+            base = 8
+        else:
+            base = 10
+
     if '/' in x:
         p, q = x.split('/')
         p, q = p.rstrip('l'), q.rstrip('l')
-        return from_rational(int(p), int(q), prec, rnd)
+        return from_rational(int(p, base), int(q, base), prec, rnd)
 
-    man, exp = str_to_man_exp(x, base=10)
+    man, exp = str_to_man_exp(x, base)
 
-    # XXX: appropriate cutoffs & track direction
-    # note no factors of 5
-    if abs(exp) > 400:
-        s = from_int(man, prec+10)
-        s = mpf_mul(s, mpf_pow_int(ften, exp, prec+10), prec, rnd)
-    else:
-        if exp >= 0:
-            s = from_int(man * 10**exp, prec, rnd)
+    if base == 10:
+        # XXX: appropriate cutoffs & track direction
+        # note no factors of 5
+        if abs(exp) > 400:
+            s = from_int(man, prec+10)
+            s = mpf_mul(s, mpf_pow_int(ften, exp, prec+10), prec, rnd)
+        else:
+            if exp >= 0:
+                s = from_int(man * 10**exp, prec, rnd)
+            else:
+                s = from_rational(man, 10**-exp, prec, rnd)
+    elif pow(2, e2 := int(math.log2(base))) == base:
+        if x.find('p') < 0:
+            s = from_man_exp(man, exp*e2, prec, rnd)
         else:
-            s = from_rational(man, 10**-exp, prec, rnd)
+            s = from_man_exp(man, exp, prec, rnd)
+    else:
+        raise NotImplementedError
     return s
 
-# Binary string conversion. These are currently mainly used for debugging
-# and could use some improvement in the future
-
-def from_bstr(x):
-    man, exp = str_to_man_exp(x, base=2)
-    man = MPZ(man)
-    sign = 0
-    if man < 0:
-        man = -man
-        sign = 1
-    bc = bitcount(man)
-    return normalize(sign, man, exp, bc, bc, round_floor)
-
-def to_bstr(x):
-    sign, man, exp, bc = x
-    return ['','-'][sign] + numeral(man, size=bitcount(man), base=2) + ("e%i" % exp)
-
 
 #----------------------------------------------------------------------------#
 #                                Square roots                                #
 #----------------------------------------------------------------------------#
 
 
 def mpf_sqrt(s, prec, rnd=round_fast):
@@ -1376,15 +1262,15 @@
     if not man:
         return s
     if exp & 1:
         exp -= 1
         man <<= 1
         bc += 1
     elif man == 1:
-        return normalize1(sign, man, exp//2, bc, prec, rnd)
+        return normalize(sign, man, exp//2, bc, prec, rnd)
     shift = max(4, 2*prec-bc+4)
     shift += shift & 1
     if rnd in 'fd':
         man = isqrt(man<<shift)
     else:
         man, rem = sqrtrem(man<<shift)
         # Perturb up
@@ -1396,19 +1282,7 @@
 def mpf_hypot(x, y, prec, rnd=round_fast):
     """Compute the Euclidean norm sqrt(x**2 + y**2) of two raw mpfs
     x and y."""
     if y == fzero: return mpf_abs(x, prec, rnd)
     if x == fzero: return mpf_abs(y, prec, rnd)
     hypot2 = mpf_add(mpf_mul(x,x), mpf_mul(y,y), prec+4)
     return mpf_sqrt(hypot2, prec, rnd)
-
-
-if BACKEND == 'sage':
-    try:
-        import sage.libs.mpmath.ext_libmp as ext_lib
-        mpf_add = ext_lib.mpf_add
-        mpf_sub = ext_lib.mpf_sub
-        mpf_mul = ext_lib.mpf_mul
-        mpf_div = ext_lib.mpf_div
-        mpf_sqrt = ext_lib.mpf_sqrt
-    except ImportError:
-        pass
```

### Comparing `mpmath-1.3.0/mpmath/libmp/libmpi.py` & `mpmath-1.4.0a0/mpmath/libmp/libmpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 """
 Computational functions for interval arithmetic.
 
 """
+from .gammazeta import mpc_loggamma, mpf_gamma, mpf_loggamma, mpf_rgamma
+from .libelefun import (mod_pi2, mpf_atan, mpf_atan2, mpf_cos_sin, mpf_exp,
+                        mpf_log, mpf_pi, mpf_sqrt)
+from .libmpf import (MPZ_ONE, ComplexResult, dps_to_prec, fhalf, finf, fnan,
+                     fninf, fnone, fone, from_float, from_int, from_man_exp,
+                     from_str, fzero, mpf_abs, mpf_add, mpf_cmp, mpf_div,
+                     mpf_eq, mpf_floor, mpf_ge, mpf_gt, mpf_le, mpf_lt,
+                     mpf_min_max, mpf_mul, mpf_mul_int, mpf_neg, mpf_pos,
+                     mpf_pow_int, mpf_shift, mpf_sign, mpf_sub, prec_to_dps,
+                     repr_dps, round_ceiling, round_down, round_floor,
+                     round_nearest, round_up, to_int, to_str)
 
-from .backend import xrange
-
-from .libmpf import (
-    ComplexResult,
-    round_down, round_up, round_floor, round_ceiling, round_nearest,
-    prec_to_dps, repr_dps, dps_to_prec,
-    bitcount,
-    from_float,
-    fnan, finf, fninf, fzero, fhalf, fone, fnone,
-    mpf_sign, mpf_lt, mpf_le, mpf_gt, mpf_ge, mpf_eq, mpf_cmp,
-    mpf_min_max,
-    mpf_floor, from_int, to_int, to_str, from_str,
-    mpf_abs, mpf_neg, mpf_pos, mpf_add, mpf_sub, mpf_mul, mpf_mul_int,
-    mpf_div, mpf_shift, mpf_pow_int,
-    from_man_exp, MPZ_ONE)
-
-from .libelefun import (
-    mpf_log, mpf_exp, mpf_sqrt, mpf_atan, mpf_atan2,
-    mpf_pi, mod_pi2, mpf_cos_sin
-)
-
-from .gammazeta import mpf_gamma, mpf_rgamma, mpf_loggamma, mpc_loggamma
 
 def mpi_str(s, prec):
     sa, sb = s
     dps = prec_to_dps(prec) + 5
     return "[%s, %s]" % (to_str(sa, dps), to_str(sb, dps))
     #dps = prec_to_dps(prec)
     #m = mpi_mid(s, prec)
@@ -535,25 +524,26 @@
         limit the error to *error_dps* digits (mode 'plusminus and 'percent')
 
     Additional keyword arguments are forwarded to the mpf-to-string conversion
     for the components of the output.
 
     **Examples**
 
-        >>> from mpmath import mpi, mp
+        >>> from mpmath import mpi, mp, iv
         >>> mp.dps = 30
         >>> x = mpi(1, 2)._mpi_
         >>> mpi_to_str(x, 2, mode='plusminus')
         '1.5 +- 0.5'
         >>> mpi_to_str(x, 2, mode='percent')
         '1.5 (33.33%)'
         >>> mpi_to_str(x, 2, mode='brackets')
         '[1.0, 2.0]'
         >>> mpi_to_str(x, 2, mode='brackets' , brackets=('<', '>'))
         '<1.0, 2.0>'
+        >>> iv.dps = 30
         >>> x = mpi('5.2582327113062393041', '5.2582327113062749951')._mpi_
         >>> mpi_to_str(x, 15, mode='diff')
         '5.2582327113062[4, 7]'
         >>> mpi_to_str(mpi(0)._mpi_, 2, mode='percent')
         '0.0 (0.0%)'
 
     """
@@ -592,15 +582,15 @@
         if len(a) == 1:
             a.append('')
         b = b_str.split('e')
         if len(b) == 1:
             b.append('')
         if a[1] == b[1]:
             if a[0] != b[0]:
-                for i in xrange(len(a[0]) + 1):
+                for i in range(len(a[0]) + 1):
                     if a[0][i] != b[0][i]:
                         break
                 s = (a[0][:i] + br1 + a[0][i:] + ',' + sp + b[0][i:] + br2
                      + 'e'*min(len(a[1]), 1) + a[1])
             else: # no difference
                 s = a[0] + br1 + br2 + 'e'*min(len(a[1]), 1) + a[1]
         else:
@@ -868,15 +858,15 @@
             mag = max(amag, bmag)
         else:
             mag = bmag
         an = abs(to_int(a2))
         bn = abs(to_int(b2))
         absn = max(an, bn)
         gamma_size = max(0,absn*mag)
-        wp += bitcount(gamma_size)
+        wp += gamma_size.bit_length()
 
     # Assume type != 1
     if type == 1:
         (a1,a2) = mpi_add((a1,a2), mpi_one, wp); z = (a1,a2), (b1,b2)
         type = 0
 
     # Avoid non-monotonic region near the negative real axis
```

### Comparing `mpmath-1.3.0/mpmath/math2.py` & `mpmath-1.4.0a0/mpmath/libfp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 """
 This module complements the math and cmath builtin modules by providing
-fast machine precision versions of some additional functions (gamma, ...)
+fast machine precision versions of some additional functions (ei, e1, ...)
 and wrapping math/cmath functions so that they can be called with either
 real or complex arguments.
 """
 
 import operator
 import math
 import cmath
 
 # Irrational (?) constants
-pi = 3.1415926535897932385
-e = 2.7182818284590452354
-sqrt2 = 1.4142135623730950488
-sqrt5 = 2.2360679774997896964
-phi = 1.6180339887498948482
-ln2 = 0.69314718055994530942
-ln10 = 2.302585092994045684
+pi = math.pi
 euler = 0.57721566490153286061
-catalan = 0.91596559417721901505
-khinchin = 2.6854520010653064453
-apery = 1.2020569031595942854
 
 logpi = 1.1447298858494001741
 
 def _mathfun_real(f_real, f_complex):
     def f(x, **kwargs):
-        if type(x) is float:
-            return f_real(x)
-        if type(x) is complex:
-            return f_complex(x)
         try:
             x = float(x)
             return f_real(x)
         except (TypeError, ValueError):
             x = complex(x)
             return f_complex(x)
     f.__name__ = f_real.__name__
@@ -55,47 +42,36 @@
         try:
             return f_real(*(float(x) for x in args))
         except (TypeError, ValueError):
             return f_complex(*(complex(x) for x in args))
     f.__name__ = f_real.__name__
     return f
 
-# Workaround for non-raising log and sqrt in Python 2.5 and 2.4
-# on Unix system
-try:
-    math.log(-2.0)
-    def math_log(x):
-        if x <= 0.0:
-            raise ValueError("math domain error")
-        return math.log(x)
-    def math_sqrt(x):
-        if x < 0.0:
-            raise ValueError("math domain error")
-        return math.sqrt(x)
-except (ValueError, TypeError):
-    math_log = math.log
-    math_sqrt = math.sqrt
 
 pow = _mathfun_n(operator.pow, lambda x, y: complex(x)**y)
-log = _mathfun_n(math_log, cmath.log)
-sqrt = _mathfun(math_sqrt, cmath.sqrt)
+log = _mathfun_n(math.log, cmath.log)
+sqrt = _mathfun(math.sqrt, cmath.sqrt)
 exp = _mathfun_real(math.exp, cmath.exp)
 
 cos = _mathfun_real(math.cos, cmath.cos)
 sin = _mathfun_real(math.sin, cmath.sin)
 tan = _mathfun_real(math.tan, cmath.tan)
 
 acos = _mathfun(math.acos, cmath.acos)
 asin = _mathfun(math.asin, cmath.asin)
 atan = _mathfun_real(math.atan, cmath.atan)
 
 cosh = _mathfun_real(math.cosh, cmath.cosh)
 sinh = _mathfun_real(math.sinh, cmath.sinh)
 tanh = _mathfun_real(math.tanh, cmath.tanh)
 
+acosh = _mathfun(math.acosh, cmath.acosh)
+asinh = _mathfun(math.asinh, cmath.asinh)
+atanh = _mathfun_real(math.atanh, cmath.atanh)
+
 floor = _mathfun_real(math.floor,
     lambda z: complex(math.floor(z.real), math.floor(z.imag)))
 ceil = _mathfun_real(math.ceil,
     lambda z: complex(math.ceil(z.real), math.ceil(z.imag)))
 
 
 cos_sin = _mathfun_real(lambda x: (math.cos(x), math.sin(x)),
@@ -153,129 +129,84 @@
     if n == 1: return -cmath.sin(z)
     if n == 2: return -cmath.cos(z)
     if n == 3: return cmath.sin(z)
 
 cospi = _mathfun_real(_cospi_real, _cospi_complex)
 sinpi = _mathfun_real(_sinpi_real, _sinpi_complex)
 
-def tanpi(x):
-    try:
-        return sinpi(x) / cospi(x)
-    except OverflowError:
-        if complex(x).imag > 10:
-            return 1j
-        if complex(x).imag < 10:
-            return -1j
-        raise
-
 def cotpi(x):
     try:
         return cospi(x) / sinpi(x)
     except OverflowError:
         if complex(x).imag > 10:
             return -1j
         if complex(x).imag < 10:
             return 1j
         raise
 
-INF = 1e300*1e300
-NINF = -INF
-NAN = INF-INF
-EPS = 2.2204460492503131e-16
+INF = math.inf
 
 _exact_gamma = (INF, 1.0, 1.0, 2.0, 6.0, 24.0, 120.0, 720.0, 5040.0, 40320.0,
   362880.0, 3628800.0, 39916800.0, 479001600.0, 6227020800.0, 87178291200.0,
   1307674368000.0, 20922789888000.0, 355687428096000.0, 6402373705728000.0,
   121645100408832000.0, 2432902008176640000.0)
 
 _max_exact_gamma = len(_exact_gamma)-1
 
 # Lanczos coefficients used by the GNU Scientific Library
 _lanczos_g = 7
 _lanczos_p = (0.99999999999980993, 676.5203681218851, -1259.1392167224028,
      771.32342877765313, -176.61502916214059, 12.507343278686905,
      -0.13857109526572012, 9.9843695780195716e-6, 1.5056327351493116e-7)
 
-def _gamma_real(x):
-    _intx = int(x)
-    if _intx == x:
-        if _intx <= 0:
-            #return (-1)**_intx * INF
-            raise ZeroDivisionError("gamma function pole")
-        if _intx <= _max_exact_gamma:
-            return _exact_gamma[_intx]
-    if x < 0.5:
-        # TODO: sinpi
-        return pi / (_sinpi_real(x)*_gamma_real(1-x))
-    else:
-        x -= 1.0
-        r = _lanczos_p[0]
-        for i in range(1, _lanczos_g+2):
-            r += _lanczos_p[i]/(x+i)
-        t = x + _lanczos_g + 0.5
-        return 2.506628274631000502417 * t**(x+0.5) * math.exp(-t) * r
-
 def _gamma_complex(x):
     if not x.imag:
-        return complex(_gamma_real(x.real))
+        if x.real == -INF:
+            return math.nan
+        return complex(math.gamma(x.real))
     if x.real < 0.5:
         # TODO: sinpi
         return pi / (_sinpi_complex(x)*_gamma_complex(1-x))
     else:
         x -= 1.0
         r = _lanczos_p[0]
         for i in range(1, _lanczos_g+2):
             r += _lanczos_p[i]/(x+i)
         t = x + _lanczos_g + 0.5
         return 2.506628274631000502417 * t**(x+0.5) * cmath.exp(-t) * r
 
-gamma = _mathfun_real(_gamma_real, _gamma_complex)
+gamma = _mathfun_real(math.gamma, _gamma_complex)
 
 def rgamma(x):
     try:
         return 1./gamma(x)
     except ZeroDivisionError:
         return x*0.0
 
 def factorial(x):
     return gamma(x+1.0)
 
-def arg(x):
-    if type(x) is float:
-        return math.atan2(0.0,x)
-    return math.atan2(x.imag,x.real)
-
 # XXX: broken for negatives
 def loggamma(x):
     if type(x) not in (float, complex):
         try:
             x = float(x)
         except (ValueError, TypeError):
             x = complex(x)
-    try:
-        xreal = x.real
-        ximag = x.imag
-    except AttributeError:   # py2.5
-        xreal = x
-        ximag = 0.0
     # Reflection formula
     # http://functions.wolfram.com/GammaBetaErf/LogGamma/16/01/01/0003/
-    if xreal < 0.0:
+    if x.real < 0.0:
         if abs(x) < 0.5:
             v = log(gamma(x))
-            if ximag == 0:
+            if x.imag == 0:
                 v = v.conjugate()
             return v
         z = 1-x
-        try:
-            re = z.real
-            im = z.imag
-        except AttributeError:   # py2.5
-            re = z
-            im = 0.0
+        re = z.real
+        im = z.imag
         refloor = floor(re)
         if im == 0.0:
             imsign = 0
         elif im < 0.0:
             imsign = -1
         else:
             imsign = 1
@@ -328,15 +259,15 @@
     x2 = x**-2
     t = x2
     for c in _psi_coeff:
         s -= c*t
         if t < 1e-20:
             break
         t *= x2
-    return s + math_log(x) - 0.5/x
+    return s + math.log(x) - 0.5/x
 
 def _digamma_complex(x):
     if not x.imag:
         return complex(_digamma_real(x.real))
     if x.real < 0.5:
         x = 1.0-x
         s = pi*cotpi(x)
@@ -352,113 +283,21 @@
         if abs(t) < 1e-20:
             break
         t *= x2
     return s + cmath.log(x) - 0.5/x
 
 digamma = _mathfun_real(_digamma_real, _digamma_complex)
 
-# TODO: could implement complex erf and erfc here. Need
-# to find an accurate method (avoiding cancellation)
-# for approx. 1 < abs(x) < 9.
-
-_erfc_coeff_P = [
-    1.0000000161203922312,
-    2.1275306946297962644,
-    2.2280433377390253297,
-    1.4695509105618423961,
-    0.66275911699770787537,
-    0.20924776504163751585,
-    0.045459713768411264339,
-    0.0063065951710717791934,
-    0.00044560259661560421715][::-1]
-
-_erfc_coeff_Q = [
-    1.0000000000000000000,
-    3.2559100272784894318,
-    4.9019435608903239131,
-    4.4971472894498014205,
-    2.7845640601891186528,
-    1.2146026030046904138,
-    0.37647108453729465912,
-    0.080970149639040548613,
-    0.011178148899483545902,
-    0.00078981003831980423513][::-1]
-
 def _polyval(coeffs, x):
     p = coeffs[0]
     for c in coeffs[1:]:
         p = c + x*p
     return p
 
-def _erf_taylor(x):
-    # Taylor series assuming 0 <= x <= 1
-    x2 = x*x
-    s = t = x
-    n = 1
-    while abs(t) > 1e-17:
-        t *= x2/n
-        s -= t/(n+n+1)
-        n += 1
-        t *= x2/n
-        s += t/(n+n+1)
-        n += 1
-    return 1.1283791670955125739*s
-
-def _erfc_mid(x):
-    # Rational approximation assuming 0 <= x <= 9
-    return exp(-x*x)*_polyval(_erfc_coeff_P,x)/_polyval(_erfc_coeff_Q,x)
-
-def _erfc_asymp(x):
-    # Asymptotic expansion assuming x >= 9
-    x2 = x*x
-    v = exp(-x2)/x*0.56418958354775628695
-    r = t = 0.5 / x2
-    s = 1.0
-    for n in range(1,22,4):
-        s -= t
-        t *= r * (n+2)
-        s += t
-        t *= r * (n+4)
-        if abs(t) < 1e-17:
-            break
-    return s * v
-
-def erf(x):
-    """
-    erf of a real number.
-    """
-    x = float(x)
-    if x != x:
-        return x
-    if x < 0.0:
-        return -erf(-x)
-    if x >= 1.0:
-        if x >= 6.0:
-            return 1.0
-        return 1.0 - _erfc_mid(x)
-    return _erf_taylor(x)
-
-def erfc(x):
-    """
-    erfc of a real number.
-    """
-    x = float(x)
-    if x != x:
-        return x
-    if x < 0.0:
-        if x < -6.0:
-            return 2.0
-        return 2.0-erfc(-x)
-    if x > 9.0:
-        return _erfc_asymp(x)
-    if x >= 1.0:
-        return _erfc_mid(x)
-    return 1.0 - _erf_taylor(x)
-
-gauss42 = [\
+gauss42 = [
 (0.99839961899006235, 0.0041059986046490839),
 (-0.99839961899006235, 0.0041059986046490839),
 (0.9915772883408609, 0.009536220301748501),
 (-0.9915772883408609,0.009536220301748501),
 (0.97934250806374812, 0.014922443697357493),
 (-0.97934250806374812, 0.014922443697357493),
 (0.96175936533820439,0.020227869569052644),
@@ -498,22 +337,21 @@
 (0.036948943165351772, 0.073864234232172879),
 (-0.036948943165351772, 0.073864234232172879)]
 
 EI_ASYMP_CONVERGENCE_RADIUS = 40.0
 
 def ei_asymp(z, _e1=False):
     r = 1./z
-    s = t = 1.0
     k = 1
-    while 1:
+    t = 1.0*k*r
+    s = 1.0 + t
+    while abs(t) >= 1e-16:
+        k += 1
         t *= k*r
         s += t
-        if abs(t) < 1e-16:
-            break
-        k += 1
     v = s*exp(z)/z
     if _e1:
         if type(z) is complex:
             zreal = z.real
             zimag = z.imag
         else:
             zreal = z
@@ -539,28 +377,26 @@
         s += term
         k += 1
     s += euler
     if _e1:
         s += log(-z)
     else:
         if type(z) is float or z.imag == 0.0:
-            s += math_log(abs(z))
+            s += math.log(abs(z))
         else:
             s += cmath.log(z)
     return s
 
 def ei(z, _e1=False):
-    typez = type(z)
-    if typez not in (float, complex):
-        try:
-            z = float(z)
-            typez = float
-        except (TypeError, ValueError):
-            z = complex(z)
-            typez = complex
+    try:
+        z = float(z)
+        typez = float
+    except (TypeError, ValueError):
+        z = complex(z)
+        typez = complex
     if not z:
         return -INF
     absz = abs(z)
     if absz > EI_ASYMP_CONVERGENCE_RADIUS:
         return ei_asymp(z, _e1)
     elif absz <= 2.0 or (typez is float and z > 0.0):
         return ei_taylor(z, _e1)
@@ -582,30 +418,28 @@
     for x,w in gauss42:
         t = C*x+D
         s += w*_exp(t)/t
     ref -= C*s
     return ref
 
 def e1(z):
+    try:
+        z = float(z)
+        typez = float
+    except (TypeError, ValueError):
+        z = complex(z)
+        typez = complex
     # hack to get consistent signs if the imaginary part if 0
     # and signed
-    typez = type(z)
-    if type(z) not in (float, complex):
-        try:
-            z = float(z)
-            typez = float
-        except (TypeError, ValueError):
-            z = complex(z)
-            typez = complex
     if typez is complex and not z.imag:
         z = complex(z.real, 0.0)
     # end hack
     return -ei(-z, _e1=True)
 
-_zeta_int = [\
+_zeta_int = [
 -0.5,
 0.0,
 1.6449340668482264365,1.2020569031595942854,1.0823232337111381915,
 1.0369277551433699263,1.0173430619844491397,1.0083492773819228268,
 1.0040773561979443394,1.0020083928260822144,1.0009945751278180853,
 1.0004941886041194646,1.0002460865533080483,1.0001227133475784891,
 1.0000612481350587048,1.0000305882363070205,1.0000152822594086519,
@@ -659,14 +493,14 @@
     n = int(s)
     if n == s:
         if n >= 0:
             return _zeta_int[n]
         if not (n % 2):
             return 0.0
     if s <= 0.0:
-        return 2.**s*pi**(s-1)*_sinpi_real(0.5*s)*_gamma_real(1-s)*zeta(1-s)
+        return 2.**s*pi**(s-1)*_sinpi_real(0.5*s)*math.gamma(1-s)*zeta(1-s)
     if s <= 2.0:
         if s <= 1.0:
             return _polyval(_zeta_0,s)/(s-1)
         return _polyval(_zeta_1,s)/(s-1)
     z = _polyval(_zeta_P,s) / _polyval(_zeta_Q,s)
     return 1.0 + 2.0**(-s) + 3.0**(-s) + 4.0**(-s)*z
```

### Comparing `mpmath-1.3.0/mpmath/matrices/calculus.py` & `mpmath-1.4.0a0/mpmath/matrices/calculus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from ..libmp.backend import xrange
-
 # TODO: should use diagonalization-based algorithms
 
-class MatrixCalculusMethods(object):
+class MatrixCalculusMethods:
 
     def _exp_pade(ctx, a):
         """
         Exponential of a matrix using Pade approximants.
 
         See G. H. Golub, C. F. van Loan 'Matrix Computations',
         third Ed., page 572
@@ -63,16 +61,17 @@
         using the Taylor series. With method='pade', Pade approximants
         are used instead.
 
         **Examples**
 
         Basic examples::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import (mp, expm, zeros, eye, j, hilbert, chop,
+            ...                     mnorm, ones, matrix)
+            >>> mp.pretty = True
             >>> expm(zeros(3))
             [1.0  0.0  0.0]
             [0.0  1.0  0.0]
             [0.0  0.0  1.0]
             >>> expm(eye(3))
             [2.71828182845905               0.0               0.0]
             [             0.0  2.71828182845905               0.0]
@@ -82,16 +81,16 @@
             [ 2.26812870852145  2.44114713886289   1.42699786729125]
             [0.841130841230196  1.42699786729125    1.6000162976327]
             >>> expm([[1,1,0],[1,0,1],[0,1,0]], method='pade')
             [ 3.86814500615414  2.26812870852145  0.841130841230196]
             [ 2.26812870852145  2.44114713886289   1.42699786729125]
             [0.841130841230196  1.42699786729125    1.6000162976327]
             >>> expm([[1+j, 0], [1+j,1]])
-            [(1.46869393991589 + 2.28735528717884j)                        0.0]
-            [  (1.03776739863568 + 3.536943175722j)  (2.71828182845905 + 0.0j)]
+            [(1.46869393991589 + 2.28735528717884j)               0.0]
+            [  (1.03776739863568 + 3.536943175722j)  2.71828182845905]
 
         Matrices with large entries are allowed::
 
             >>> expm(matrix([[1,2],[2,3]])**25)
             [5.65024064048415e+2050488462815550  9.14228140091932e+2050488462815550]
             [9.14228140091932e+2050488462815550  1.47925220414035e+2050488462815551]
 
@@ -133,30 +132,30 @@
             k = 2
             while 1:
                 T *= A * (1/ctx.mpf(k))
                 if ctx.mnorm(T, 'inf') < tol:
                     break
                 Y += T
                 k += 1
-            for k in xrange(j):
+            for k in range(j):
                 Y = Y*Y
         finally:
             ctx.prec = prec
         Y *= 1
         return Y
 
     def cosm(ctx, A):
         r"""
         Gives the cosine of a square matrix `A`, defined in analogy
         with the matrix exponential.
 
         Examples::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import mp, eye, cosm, hilbert, j, matrix
+            >>> mp.pretty = True
             >>> X = eye(3)
             >>> cosm(X)
             [0.54030230586814               0.0               0.0]
             [             0.0  0.54030230586814               0.0]
             [             0.0               0.0  0.54030230586814]
             >>> X = hilbert(3)
             >>> cosm(X)
@@ -176,16 +175,16 @@
     def sinm(ctx, A):
         r"""
         Gives the sine of a square matrix `A`, defined in analogy
         with the matrix exponential.
 
         Examples::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import mp, eye, sinm, hilbert, matrix, j
+            >>> mp.pretty = True
             >>> X = eye(3)
             >>> sinm(X)
             [0.841470984807897                0.0                0.0]
             [              0.0  0.841470984807897                0.0]
             [              0.0                0.0  0.841470984807897]
             >>> X = hilbert(3)
             >>> sinm(X)
@@ -214,16 +213,16 @@
         a matrix `B = A^{1/2}` such that `B^2 = A`. The square root
         of a matrix, if it exists, is not unique.
 
         **Examples**
 
         Square roots of some simple matrices::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import mp, sqrtm, j, matrix, cos, sin, chop, mnorm
+            >>> mp.pretty = True
             >>> sqrtm([[1,0], [0,1]])
             [1.0  0.0]
             [0.0  1.0]
             >>> sqrtm([[0,0], [0,0]])
             [0.0  0.0]
             [0.0  0.0]
             >>> sqrtm([[2,0],[0,1]])
@@ -282,15 +281,15 @@
             >>> sqrtm([[0,1], [0,0]])
             Traceback (most recent call last):
               ...
             ZeroDivisionError: matrix is numerically singular
 
         Two examples from the documentation for Matlab's ``sqrtm``::
 
-            >>> mp.dps = 15; mp.pretty = True
+            >>> mp.pretty = True
             >>> sqrtm([[7,10],[15,22]])
             [1.56669890360128  1.74077655955698]
             [2.61116483933547  4.17786374293675]
             >>>
             >>> X = matrix(\
             ...   [[5,-4,1,0,0],
             ...   [-4,6,-4,1,0],
@@ -353,16 +352,17 @@
         a matrix `B = \log(A)` such that `\exp(B) = A`. The logarithm
         of a matrix, if it exists, is not unique.
 
         **Examples**
 
         Logarithms of some simple matrices::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import (mp, eye, logm, expm, matrix, j, nprint,
+            ...                     chop, hilbert, cos, sin, pi, re)
+            >>> mp.pretty = True
             >>> X = eye(3)
             >>> logm(X)
             [0.0  0.0  0.0]
             [0.0  0.0  0.0]
             [0.0  0.0  0.0]
             >>> logm(2*X)
             [0.693147180559945                0.0                0.0]
@@ -466,16 +466,17 @@
         Computes `A^r = \exp(A \log r)` for a matrix `A` and complex
         number `r`.
 
         **Examples**
 
         Powers and inverse powers of a matrix::
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = True
+            >>> from mpmath import (mp, matrix, powm, chop, extraprec, fib,
+            ...                     phi, sqrt)
+            >>> mp.pretty = True
             >>> A = matrix([[4,1,4],[7,8,9],[10,2,11]])
             >>> powm(A, 2)
             [ 63.0  20.0   69.0]
             [174.0  89.0  199.0]
             [164.0  48.0  179.0]
             >>> chop(powm(powm(A, 4), 1/4.))
             [ 4.0  1.0   4.0]
```

### Comparing `mpmath-1.3.0/mpmath/matrices/eigen.py` & `mpmath-1.4.0a0/mpmath/matrices/eigen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 ##################################################################################################
 #     module for the eigenvalue problem
 #       Copyright 2013 Timo Hartmann (thartmann15 at gmail.com)
 #
 # todo:
 #  - implement balancing
 #  - agressive early deflation
@@ -29,17 +26,16 @@
   hessenberg_reduce_1 : auxiliary routine to hessenberg_reduce_0
   qr_step : a single implicitly shifted QR step for an upper Hessenberg matrix
   hessenberg_qr : Schur decomposition of an upper Hessenberg matrix
   eig_tr_r : right eigenvectors of an upper triangular matrix
   eig_tr_l : left  eigenvectors of an upper triangular matrix
 """
 
-from ..libmp.backend import xrange
 
-class Eigen(object):
+class Eigen:
     pass
 
 def defun(f):
     setattr(Eigen, f.__name__, f)
     return f
 
 def hessenberg_reduce_0(ctx, A, T):
@@ -73,20 +69,20 @@
     # the last entry of v is stored in T.
     # the upper right part of A (including diagonal and subdiagonal) becomes H.
 
 
     n = A.rows
     if n <= 2: return
 
-    for i in xrange(n-1, 1, -1):
+    for i in range(n-1, 1, -1):
 
         # scale the vector
 
         scale = 0
-        for k in xrange(0, i):
+        for k in range(i):
             scale += abs(ctx.re(A[i,k])) + abs(ctx.im(A[i,k]))
 
         scale_inv = 0
         if scale != 0:
             scale_inv = 1 / scale
 
         if scale == 0 or ctx.isinf(scale_inv):
@@ -94,15 +90,15 @@
             T[i] = 0
             A[i,i-1] = 0
             continue
 
         # calculate parameters for housholder transformation
 
         H = 0
-        for k in xrange(0, i):
+        for k in range(i):
             A[i,k] *= scale_inv
             rr = ctx.re(A[i,k])
             ii = ctx.im(A[i,k])
             H += rr * rr + ii * ii
 
         F = A[i,i-1]
         f = abs(F)
@@ -116,37 +112,37 @@
             T[i] = F + G * ff
             A[i,i-1] *= ff
 
         H += G * f
         H = 1 / ctx.sqrt(H)
 
         T[i] *= H
-        for k in xrange(0, i - 1):
+        for k in range(i - 1):
             A[i,k] *= H
 
-        for j in xrange(0, i):
+        for j in range(i):
             # apply housholder transformation (from right)
 
             G = ctx.conj(T[i]) * A[j,i-1]
-            for k in xrange(0, i-1):
+            for k in range(i-1):
                 G += ctx.conj(A[i,k]) * A[j,k]
 
             A[j,i-1] -= G * T[i]
-            for k in xrange(0, i-1):
+            for k in range(i-1):
                 A[j,k] -= G * A[i,k]
 
-        for j in xrange(0, n):
+        for j in range(n):
             # apply housholder transformation (from left)
 
             G = T[i] * A[i-1,j]
-            for k in xrange(0, i-1):
+            for k in range(i-1):
                 G += A[i,k] * A[k,j]
 
             A[i-1,j] -= G * ctx.conj(T[i])
-            for k in xrange(0, i-1):
+            for k in range(i-1):
                 A[k,j] -= G * ctx.conj(A[i,k])
 
 
 
 def hessenberg_reduce_1(ctx, A, T):
     """
     This routine forms the unitary matrix Q described in hessenberg_reduce_0.
@@ -163,28 +159,28 @@
     if n == 1:
         A[0,0] = 1
         return
 
     A[0,0] = A[1,1] = 1
     A[0,1] = A[1,0] = 0
 
-    for i in xrange(2, n):
+    for i in range(2, n):
         if T[i] != 0:
 
-            for j in xrange(0, i):
+            for j in range(i):
                 G = T[i] * A[i-1,j]
-                for k in xrange(0, i-1):
+                for k in range(i-1):
                     G += A[i,k] * A[k,j]
 
                 A[i-1,j] -= G * ctx.conj(T[i])
-                for k in xrange(0, i-1):
+                for k in range(i-1):
                     A[k,j] -= G * ctx.conj(A[i,k])
 
         A[i,i] = 1
-        for j in xrange(0, i):
+        for j in range(i):
             A[j,i] = A[i,j] = 0
 
 
 
 @defun
 def hessenberg(ctx, A, overwrite_a = False):
     """
@@ -205,15 +201,15 @@
       Q : an unitary matrix
       H : an upper right Hessenberg matrix
 
     example:
       >>> from mpmath import mp
       >>> A = mp.matrix([[3, -1, 2], [2, 5, -5], [-2, -3, 7]])
       >>> Q, H = mp.hessenberg(A)
-      >>> mp.nprint(H, 3) # doctest:+SKIP
+      >>> mp.nprint(H, 3)
       [  3.15  2.23  4.44]
       [-0.769  4.85  3.05]
       [   0.0  3.61   7.0]
       >>> print(mp.chop(A - Q * H * Q.transpose_conj()))
       [0.0  0.0  0.0]
       [0.0  0.0  0.0]
       [0.0  0.0  0.0]
@@ -231,16 +227,16 @@
 
     T = ctx.matrix(n, 1)
 
     hessenberg_reduce_0(ctx, A, T)
     Q = A.copy()
     hessenberg_reduce_1(ctx, Q, T)
 
-    for x in xrange(n):
-        for y in xrange(x+2, n):
+    for x in range(n):
+        for y in range(x+2, n):
             A[y,x] = 0
 
     return Q, A
 
 
 ###########################################################################
 
@@ -305,39 +301,39 @@
     else:
         c /= v
         s /= v
 
     cc = ctx.conj(c)
     cs = ctx.conj(s)
 
-    for k in xrange(n0, n):
+    for k in range(n0, n):
         # apply givens rotation from the left
         x = A[n0  ,k]
         y = A[n0+1,k]
         A[n0  ,k] = cc * x + cs * y
         A[n0+1,k] = c * y - s * x
 
-    for k in xrange(min(n1, n0+3)):
+    for k in range(min(n1, n0+3)):
         # apply givens rotation from the right
         x = A[k,n0  ]
         y = A[k,n0+1]
         A[k,n0  ] = c * x + s * y
         A[k,n0+1] = cc * y - cs * x
 
     if not isinstance(Q, bool):
-        for k in xrange(n):
+        for k in range(n):
             # eigenvectors
             x = Q[k,n0  ]
             y = Q[k,n0+1]
             Q[k,n0  ] = c * x + s * y
             Q[k,n0+1] = cc * y - cs * x
 
     # chase the bulge
 
-    for j in xrange(n0, n1 - 2):
+    for j in range(n0, n1 - 2):
         # calculate givens rotation
 
         c = A[j+1,j]
         s = A[j+2,j]
 
         v = ctx.hypot(ctx.hypot(ctx.re(c), ctx.im(c)), ctx.hypot(ctx.re(s), ctx.im(s)))
 
@@ -352,30 +348,30 @@
             s /= v
 
         A[j+2,j] = 0
 
         cc = ctx.conj(c)
         cs = ctx.conj(s)
 
-        for k in xrange(j+1, n):
+        for k in range(j+1, n):
             # apply givens rotation from the left
             x = A[j+1,k]
             y = A[j+2,k]
             A[j+1,k] = cc * x + cs * y
             A[j+2,k] = c * y - s * x
 
-        for k in xrange(0, min(n1, j+4)):
+        for k in range(min(n1, j+4)):
             # apply givens rotation from the right
             x = A[k,j+1]
             y = A[k,j+2]
             A[k,j+1] = c * x + s * y
             A[k,j+2] = cc * y - cs * x
 
         if not isinstance(Q, bool):
-            for k in xrange(0, n):
+            for k in range(n):
                 # eigenvectors
                 x = Q[k,j+1]
                 y = Q[k,j+2]
                 Q[k,j+1] = c * x + s * y
                 Q[k,j+2] = cc * y - cs * x
 
 
@@ -398,16 +394,16 @@
                 matrix Q arising from the Schur decomposition. Q can also be
                 false, in which case the unitary matrix Q is not computated.
     """
 
     n = A.rows
 
     norm = 0
-    for x in xrange(n):
-        for y in xrange(min(x+2, n)):
+    for x in range(n):
+        for y in range(min(x+2, n)):
             norm += ctx.re(A[y,x]) ** 2 + ctx.im(A[y,x]) ** 2
     norm = ctx.sqrt(norm) / n
 
     if norm == 0:
         return
 
     n0 = 0
@@ -510,15 +506,15 @@
 
     return value:   (Q, R)
 
     example:
       >>> from mpmath import mp
       >>> A = mp.matrix([[3, -1, 2], [2, 5, -5], [-2, -3, 7]])
       >>> Q, R = mp.schur(A)
-      >>> mp.nprint(R, 3) # doctest:+SKIP
+      >>> mp.nprint(R, 3)
       [2.0  0.417  -2.53]
       [0.0    4.0  -4.74]
       [0.0    0.0    9.0]
       >>> print(mp.chop(A - Q * R * Q.transpose_conj()))
       [0.0  0.0  0.0]
       [0.0  0.0  0.0]
       [0.0  0.0  0.0]
@@ -536,16 +532,16 @@
 
     T = ctx.matrix(n, 1)
 
     hessenberg_reduce_0(ctx, A, T)
     Q = A.copy()
     hessenberg_reduce_1(ctx, Q, T)
 
-    for x in xrange(n):
-        for y in xrange(x + 2, n):
+    for x in range(n):
+        for y in range(x + 2, n):
             A[y,x] = 0
 
     hessenberg_qr(ctx, A, Q)
 
     return Q, A
 
 
@@ -575,40 +571,40 @@
     # original double has prec*20
 
     smlnum = unfl * (n / eps)
     simin = 1 / ctx.sqrt(eps)
 
     rmax = 1
 
-    for i in xrange(1, n):
+    for i in range(1, n):
         s = A[i,i]
 
         smin = max(eps * abs(s), smlnum)
 
-        for j in xrange(i - 1, -1, -1):
+        for j in range(i - 1, -1, -1):
 
             r = 0
-            for k in xrange(j + 1, i + 1):
+            for k in range(j + 1, i + 1):
                 r += A[j,k] * ER[k,i]
 
             t = A[j,j] - s
             if abs(t) < smin:
                 t = smin
 
             r = -r / t
             ER[j,i] = r
 
             rmax = max(rmax, abs(r))
             if rmax > simin:
-                for k in xrange(j, i+1):
+                for k in range(j, i+1):
                     ER[k,i] /= rmax
                 rmax = 1
 
         if rmax != 1:
-            for k in xrange(0, i + 1):
+            for k in range(i + 1):
                 ER[k,i] /= rmax
 
     return ER
 
 def eig_tr_l(ctx, A):
     """
     This routine calculates the left eigenvectors of an upper right triangular matrix.
@@ -633,40 +629,40 @@
     # original double has prec*20
 
     smlnum = unfl * (n / eps)
     simin = 1 / ctx.sqrt(eps)
 
     rmax = 1
 
-    for i in xrange(0, n - 1):
+    for i in range(n - 1):
         s = A[i,i]
 
         smin = max(eps * abs(s), smlnum)
 
-        for j in xrange(i + 1, n):
+        for j in range(i + 1, n):
 
             r = 0
-            for k in xrange(i, j):
+            for k in range(i, j):
                 r += EL[i,k] * A[k,j]
 
             t = A[j,j] - s
             if abs(t) < smin:
                 t = smin
 
             r = -r / t
             EL[i,j] = r
 
             rmax = max(rmax, abs(r))
             if rmax > simin:
-                for k in xrange(i, j + 1):
+                for k in range(i, j + 1):
                     EL[i,k] /= rmax
                 rmax = 1
 
         if rmax != 1:
-            for k in xrange(i, n):
+            for k in range(i, n):
                 EL[i,k] /= rmax
 
     return EL
 
 @defun
 def eig(ctx, A, left = False, right = True, overwrite_a = False):
     """
@@ -730,14 +726,17 @@
       - eigh (or eigsy, eighe) for the symmetric eigenvalue problem.
       - eig_sort for sorting of eigenvalues and eigenvectors
     """
 
     n = A.rows
 
     if n == 1:
+        if not (left or right):
+            return [A[0]]
+
         if left and (not right):
             return ([A[0]], ctx.matrix([[1]]))
 
         if right and (not left):
             return ([A[0]], ctx.matrix([[1]]))
 
         return ([A[0]], ctx.matrix([[1]]), ctx.matrix([[1]]))
@@ -751,22 +750,22 @@
 
     if left or right:
         Q = A.copy()
         hessenberg_reduce_1(ctx, Q, T)
     else:
         Q = False
 
-    for x in xrange(n):
-        for y in xrange(x + 2, n):
+    for x in range(n):
+        for y in range(x + 2, n):
             A[y,x] = 0
 
     hessenberg_qr(ctx, A, Q)
 
-    E = [0 for i in xrange(n)]
-    for i in xrange(n):
+    E = [0 for i in range(n)]
+    for i in range(n):
         E[i] = A[i,i]
 
     if not (left or right):
         return E
 
     if left:
         EL = eig_tr_l(ctx, A)
@@ -832,39 +831,39 @@
         else:
             raise RuntimeError("unknown function %s" % f)
 
     n = len(E)
 
     # Sort eigenvalues (bubble-sort)
 
-    for i in xrange(n):
+    for i in range(n):
         imax = i
         s = f(E[i])         # s is the current maximal element
 
-        for j in xrange(i + 1, n):
+        for j in range(i + 1, n):
             c = f(E[j])
             if c < s:
                 s = c
                 imax = j
 
         if imax != i:
             # swap eigenvalues
 
             z = E[i]
             E[i] = E[imax]
             E[imax] = z
 
             if not isinstance(EL, bool):
-                for j in xrange(n):
+                for j in range(n):
                     z = EL[i,j]
                     EL[i,j] = EL[imax,j]
                     EL[imax,j] = z
 
             if not isinstance(ER, bool):
-                for j in xrange(n):
+                for j in range(n):
                     z = ER[j,i]
                     ER[j,i] = ER[j,imax]
                     ER[j,imax] = z
 
     if isinstance(EL, bool) and isinstance(ER, bool):
         return E
```

### Comparing `mpmath-1.3.0/mpmath/matrices/eigen_symmetric.py` & `mpmath-1.4.0a0/mpmath/matrices/eigen_symmetric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 ##################################################################################################
 #     module for the symmetric eigenvalue problem
 #       Copyright 2013 Timo Hartmann (thartmann15 at gmail.com)
 #
 # todo:
 #  - implement balancing
 #
@@ -33,15 +30,14 @@
   c_he_tridiag_1 : auxiliary routine to c_he_tridiag_0
   c_he_tridiag_2 : auxiliary routine to c_he_tridiag_0
   tridiag_eigen : solves the real symmetric tridiagonal matrix eigenvalue problem
   svd_r_raw : raw singular value decomposition for real matrices
   svd_c_raw : raw singular value decomposition for complex matrices
 """
 
-from ..libmp.backend import xrange
 from .eigen import defun
 
 
 def r_sy_tridiag(ctx, A, D, E, calc_ev = True):
     """
     This routine transforms a real symmetric matrix A to a real symmetric
     tridiagonal matrix T using an orthogonal similarity transformation:
@@ -74,19 +70,19 @@
       Stoer, Bulirsch - Introduction to Numerical Analysis.
     """
 
     # note : the vector v of the i-th houshoulder reflector is stored in a[(i+1):,i]
     #        whereas v/<v,v> is stored in a[i,(i+1):]
 
     n = A.rows
-    for i in xrange(n - 1, 0, -1):
+    for i in range(n - 1, 0, -1):
         # scale the vector
 
         scale = 0
-        for k in xrange(0, i):
+        for k in range(i):
             scale += abs(A[k,i])
 
         scale_inv = 0
         if scale != 0:
             scale_inv = 1/scale
 
         # sadly there are floating point numbers not equal to zero whose reciprocal is infinity
@@ -95,76 +91,76 @@
             E[i] = A[i-1,i]        # nothing to do
             D[i] = 0
             continue
 
         # calculate parameters for housholder transformation
 
         H = 0
-        for k in xrange(0, i):
+        for k in range(i):
             A[k,i] *= scale_inv
             H += A[k,i] * A[k,i]
 
         F = A[i-1,i]
         G = ctx.sqrt(H)
         if F > 0:
             G = -G
         E[i] = scale * G
         H -= F * G
         A[i-1,i] = F - G
         F = 0
 
         # apply housholder transformation
 
-        for j in xrange(0, i):
+        for j in range(i):
             if calc_ev:
                 A[i,j] = A[j,i] / H
 
             G = 0                  # calculate A*U
-            for k in xrange(0, j + 1):
+            for k in range(j + 1):
                 G += A[k,j] * A[k,i]
-            for k in xrange(j + 1, i):
+            for k in range(j + 1, i):
                 G += A[j,k] * A[k,i]
 
             E[j] = G / H           # calculate P
             F += E[j] * A[j,i]
 
         HH = F / (2 * H)
 
-        for j in xrange(0, i):     # calculate reduced A
+        for j in range(i):     # calculate reduced A
             F = A[j,i]
             G = E[j] - HH * F      # calculate Q
             E[j] = G
 
-            for k in xrange(0, j + 1):
+            for k in range(j + 1):
                 A[k,j] -= F * E[k] + G * A[k,i]
 
         D[i] = H
 
-    for i in xrange(1, n):         # better for compatibility
+    for i in range(1, n):         # better for compatibility
         E[i-1] = E[i]
     E[n-1] = 0
 
     if calc_ev:
         D[0] = 0
-        for i in xrange(0, n):
+        for i in range(n):
             if D[i] != 0:
-                for j in xrange(0, i):     # accumulate transformation matrices
+                for j in range(i):     # accumulate transformation matrices
                     G = 0
-                    for k in xrange(0, i):
+                    for k in range(i):
                         G += A[i,k] * A[k,j]
-                    for k in xrange(0, i):
+                    for k in range(i):
                         A[k,j] -= G * A[k,i]
 
             D[i] = A[i,i]
             A[i,i] = 1
 
-            for j in xrange(0, i):
+            for j in range(i):
                 A[j,i] = A[i,j] = 0
     else:
-        for i in xrange(0, n):
+        for i in range(n):
             D[i] = A[i,i]
 
 
 
 
 
 def c_he_tridiag_0(ctx, A, D, E, T):
@@ -199,20 +195,20 @@
 
     For a good introduction to Householder reflections, see also
       Stoer, Bulirsch - Introduction to Numerical Analysis.
     """
 
     n = A.rows
     T[n-1] = 1
-    for i in xrange(n - 1, 0, -1):
+    for i in range(n - 1, 0, -1):
 
         # scale the vector
 
         scale = 0
-        for k in xrange(0, i):
+        for k in range(i):
             scale += abs(ctx.re(A[k,i])) + abs(ctx.im(A[k,i]))
 
         scale_inv = 0
         if scale != 0:
             scale_inv = 1 / scale
 
         # sadly there are floating point numbers not equal to zero whose reciprocal is infinity
@@ -233,15 +229,15 @@
             else:
                 T[i-1] = T[i]
             continue
 
         # calculate parameters for housholder transformation
 
         H = 0
-        for k in xrange(0, i):
+        for k in range(i):
             A[k,i] *= scale_inv
             rr = ctx.re(A[k,i])
             ii = ctx.im(A[k,i])
             H += rr * rr + ii * ii
 
         F = A[i-1,i]
         f = abs(F)
@@ -255,47 +251,47 @@
         else:
             TZ = -T[i]                   # T[i-1]=-T[i]
         A[i-1,i] += G
         F = 0
 
         # apply housholder transformation
 
-        for j in xrange(0, i):
+        for j in range(i):
             A[i,j] = A[j,i] / H
 
             G = 0                        # calculate A*U
-            for k in xrange(0, j + 1):
+            for k in range(j + 1):
                 G += ctx.conj(A[k,j]) * A[k,i]
-            for k in xrange(j + 1, i):
+            for k in range(j + 1, i):
                 G += A[j,k] * A[k,i]
 
             T[j] = G / H                 # calculate P
             F += ctx.conj(T[j]) * A[j,i]
 
         HH = F / (2 * H)
 
-        for j in xrange(0, i):           # calculate reduced A
+        for j in range(i):           # calculate reduced A
             F = A[j,i]
             G = T[j] - HH * F            # calculate Q
             T[j] = G
 
-            for k in xrange(0, j + 1):
+            for k in range(j + 1):
                 A[k,j] -= ctx.conj(F) * T[k] + ctx.conj(G) * A[k,i]
                 # as we use the lower left part for storage
                 # we have to use the transpose of the normal formula
 
         T[i-1] = TZ
         D[i] = H
 
-    for i in xrange(1, n):                # better for compatibility
+    for i in range(1, n):                # better for compatibility
         E[i-1] = E[i]
     E[n-1] = 0
 
     D[0] = 0
-    for i in xrange(0, n):
+    for i in range(n):
         zw = D[i]
         D[i] = ctx.re(A[i,i])
         A[i,i] = zw
 
 
 
 
@@ -312,30 +308,30 @@
 
       T    (input) On input, T is the same array as delivered by c_he_tridiag_0.
 
     """
 
     n = A.rows
 
-    for i in xrange(0, n):
+    for i in range(n):
         if A[i,i] != 0:
-            for j in xrange(0, i):
+            for j in range(i):
                 G = 0
-                for k in xrange(0, i):
+                for k in range(i):
                     G += ctx.conj(A[i,k]) * A[k,j]
-                for k in xrange(0, i):
+                for k in range(i):
                     A[k,j] -= G * A[k,i]
 
         A[i,i] = 1
 
-        for j in xrange(0, i):
+        for j in range(i):
             A[j,i] = A[i,j] = 0
 
-    for i in xrange(0, n):
-        for k in xrange(0, n):
+    for i in range(n):
+        for k in range(n):
             A[i,k] *= T[k]
 
 
 
 
 def c_he_tridiag_2(ctx, A, T, B):
     """
@@ -353,25 +349,25 @@
     This routine is a python translation of the fortran routine htribk.f in the
     software library EISPACK (see netlib.org). See c_he_tridiag_0 for more
     references.
     """
 
     n = A.rows
 
-    for i in xrange(0, n):
-        for k in xrange(0, n):
+    for i in range(n):
+        for k in range(n):
             B[k,i] *= T[k]
 
-    for i in xrange(0, n):
+    for i in range(n):
         if A[i,i] != 0:
-            for j in xrange(0, n):
+            for j in range(n):
                 G = 0
-                for k in xrange(0, i):
+                for k in range(i):
                     G += ctx.conj(A[i,k]) * B[k,j]
-                for k in xrange(0, i):
+                for k in range(i):
                     B[k,j] -= G * A[k,i]
 
 
 
 
 
 def tridiag_eigen(ctx, d, e, z = False):
@@ -408,15 +404,15 @@
     See also the routine gaussq.f in netlog.org or acm algorithm 726.
     """
 
     n = len(d)
     e[n-1] = 0
     iterlim = 2 * ctx.dps
 
-    for l in xrange(n):
+    for l in range(n):
         j = 0
         while 1:
             m = l
             while 1:
                 # look for a small subdiagonal element
                 if m + 1 == n:
                     break
@@ -442,15 +438,15 @@
             else:
                 s = g + r
 
             g = d[m] - p + e[l] / s
 
             s, c, p = 1, 1, 0
 
-            for i in xrange(m - 1, l - 1, -1):
+            for i in range(m - 1, l - 1, -1):
                 f = s * e[i]
                 b = c * e[i]
                 if abs(f) > abs(g):             # this here is a slight improvement also used in gaussq.f or acm algorithm 726.
                     c = g / f
                     r = ctx.hypot(c, 1)
                     e[i + 1] = f * r
                     s = 1 / r
@@ -465,40 +461,40 @@
                 r = (d[i] - g) * s + 2 * c * b
                 p = s * r
                 d[i + 1] = g + p
                 g = c * r - b
 
                 if not isinstance(z, bool):
                     # calculate eigenvectors
-                    for w in xrange(z.rows):
+                    for w in range(z.rows):
                         f = z[w,i+1]
                         z[w,i+1] = s * z[w,i] + c * f
                         z[w,i  ] = c * z[w,i] - s * f
 
             d[l] = d[l] - p
             e[l] = g
             e[m] = 0
 
-    for ii in xrange(1, n):
+    for ii in range(1, n):
         # sort eigenvalues and eigenvectors (bubble-sort)
         i = ii - 1
         k = i
         p = d[i]
-        for j in xrange(ii, n):
+        for j in range(ii, n):
             if d[j] >= p:
                 continue
             k = j
             p = d[k]
         if k == i:
             continue
         d[k] = d[i]
         d[i] = p
 
         if not isinstance(z, bool):
-            for w in xrange(z.rows):
+            for w in range(z.rows):
                 p = z[w,i]
                 z[w,i] = z[w,k]
                 z[w,k] = p
 
 ########################################################################################
 
 @defun
@@ -816,80 +812,80 @@
     z = ctx.zeros(1, n)
 
     z[0,0] = 1
 
     if qtype == "legendre":
         # legendre on the range -1 +1 , abramowitz, table 25.4, p.916
         w = 2
-        for i in xrange(n):
+        for i in range(n):
             j = i + 1
             e[i] = ctx.sqrt(j * j / (4 * j * j - ctx.mpf(1)))
     elif qtype == "legendre01":
         # legendre shifted to 0 1        , abramowitz, table 25.8, p.921
         w = 1
-        for i in xrange(n):
+        for i in range(n):
             d[i] = 1 / ctx.mpf(2)
             j = i + 1
             e[i] = ctx.sqrt(j * j / (16 * j * j - ctx.mpf(4)))
     elif qtype == "hermite":
         # hermite on the range -inf +inf , abramowitz, table 25.10,p.924
         w = ctx.sqrt(ctx.pi)
-        for i in xrange(n):
+        for i in range(n):
             j = i + 1
             e[i] = ctx.sqrt(j / ctx.mpf(2))
     elif qtype == "laguerre":
         # laguerre on the range 0 +inf , abramowitz, table 25.9, p. 923
         w = 1
-        for i in xrange(n):
+        for i in range(n):
             j = i + 1
             d[i] = 2 * j - 1
             e[i] = j
     elif qtype=="chebyshev1":
         # chebyshev polynimials of the first kind
         w = ctx.pi
-        for i in xrange(n):
+        for i in range(n):
             e[i] = 1 / ctx.mpf(2)
         e[0] = ctx.sqrt(1 / ctx.mpf(2))
     elif qtype == "chebyshev2":
         # chebyshev polynimials of the second kind
         w = ctx.pi / 2
-        for i in xrange(n):
+        for i in range(n):
             e[i] = 1 / ctx.mpf(2)
     elif qtype == "glaguerre":
         # generalized laguerre on the range 0 +inf
         w = ctx.gamma(1 + alpha)
-        for i in xrange(n):
+        for i in range(n):
             j = i + 1
             d[i] = 2 * j - 1 + alpha
             e[i] = ctx.sqrt(j * (j + alpha))
     elif qtype == "jacobi":
         # jacobi polynomials
         alpha = ctx.mpf(alpha)
         beta = ctx.mpf(beta)
         ab = alpha + beta
         abi = ab + 2
         w = (2**(ab+1)) * ctx.gamma(alpha + 1) * ctx.gamma(beta + 1) / ctx.gamma(abi)
         d[0] = (beta - alpha) / abi
         e[0] = ctx.sqrt(4 * (1 + alpha) * (1 + beta) / ((abi + 1) * (abi * abi)))
         a2b2 = beta * beta - alpha * alpha
-        for i in xrange(1, n):
+        for i in range(1, n):
             j = i + 1
             abi = 2 * j + ab
             d[i] = a2b2 / ((abi - 2) * abi)
             e[i] = ctx.sqrt(4 * j * (j + alpha) * (j + beta) * (j + ab) / ((abi * abi - 1) * abi * abi))
     elif isinstance(qtype, str):
         raise ValueError("unknown quadrature rule \"%s\"" % qtype)
     elif not isinstance(qtype, str):
         w = qtype(d, e)
     else:
         assert 0
 
     tridiag_eigen(ctx, d, e, z)
 
-    for i in xrange(len(z)):
+    for i in range(len(z)):
         z[i] *= z[i]
 
     z = z.transpose()
     return (d, w * z)
 
 ##################################################################################################
 ##################################################################################################
@@ -947,163 +943,163 @@
 
     # work is a temporary array of size n
     work = ctx.zeros(n, 1)
 
     g = scale = anorm = 0
     maxits = 3 * ctx.dps
 
-    for i in xrange(n):     # householder reduction to bidiagonal form
+    for i in range(n):     # householder reduction to bidiagonal form
         work[i] = scale*g
         g = s = scale = 0
         if i < m:
-            for k in xrange(i, m):
+            for k in range(i, m):
                 scale += ctx.fabs(A[k,i])
             if scale != 0:
-                for k in xrange(i, m):
+                for k in range(i, m):
                     A[k,i] /= scale
                     s += A[k,i] * A[k,i]
                 f = A[i,i]
                 g = -ctx.sqrt(s)
                 if f < 0:
                     g = -g
                 h = f * g - s
                 A[i,i] = f - g
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     s = 0
-                    for k in xrange(i, m):
+                    for k in range(i, m):
                         s += A[k,i] * A[k,j]
                     f = s / h
-                    for k in xrange(i, m):
+                    for k in range(i, m):
                         A[k,j] += f * A[k,i]
-                for k in xrange(i,m):
+                for k in range(i,m):
                     A[k,i] *= scale
 
         S[i] = scale * g
         g = s = scale = 0
 
         if i < m and i != n - 1:
-            for k in xrange(i+1, n):
+            for k in range(i+1, n):
                 scale += ctx.fabs(A[i,k])
             if scale:
-                for k in xrange(i+1, n):
+                for k in range(i+1, n):
                     A[i,k] /= scale
                     s += A[i,k] * A[i,k]
                 f = A[i,i+1]
                 g = -ctx.sqrt(s)
                 if f < 0:
                     g = -g
                 h = f * g - s
                 A[i,i+1] = f - g
 
-                for k in xrange(i+1, n):
+                for k in range(i+1, n):
                     work[k] = A[i,k] / h
 
-                for j in xrange(i+1, m):
+                for j in range(i+1, m):
                     s = 0
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         s += A[j,k] * A[i,k]
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         A[j,k] += s * work[k]
 
-                for k in xrange(i+1, n):
+                for k in range(i+1, n):
                     A[i,k] *= scale
 
         anorm = max(anorm, ctx.fabs(S[i]) + ctx.fabs(work[i]))
 
     if not isinstance(V, bool):
-        for i in xrange(n-2, -1, -1):     # accumulation of right hand transformations
+        for i in range(n-2, -1, -1):     # accumulation of right hand transformations
             V[i+1,i+1] = 1
 
             if work[i+1] != 0:
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     V[i,j] = (A[i,j] / A[i,i+1]) / work[i+1]
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     s = 0
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         s += A[i,k] * V[j,k]
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         V[j,k] += s * V[i,k]
 
-            for j in xrange(i+1, n):
+            for j in range(i+1, n):
                 V[j,i] = V[i,j] = 0
 
         V[0,0] = 1
 
     if m<n : minnm = m
     else   : minnm = n
 
     if calc_u:
-        for i in xrange(minnm-1, -1, -1): # accumulation of left hand transformations
+        for i in range(minnm-1, -1, -1): # accumulation of left hand transformations
             g = S[i]
-            for j in xrange(i+1, n):
+            for j in range(i+1, n):
                 A[i,j] = 0
             if g != 0:
                 g = 1 / g
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     s = 0
-                    for k in xrange(i+1, m):
+                    for k in range(i+1, m):
                         s += A[k,i] * A[k,j]
                     f = (s / A[i,i]) * g
-                    for k in xrange(i, m):
+                    for k in range(i, m):
                         A[k,j] += f * A[k,i]
-                for j in xrange(i, m):
+                for j in range(i, m):
                     A[j,i] *= g
             else:
-                for j in xrange(i, m):
+                for j in range(i, m):
                     A[j,i] = 0
             A[i,i] += 1
 
-    for k in xrange(n - 1, -1, -1):
+    for k in range(n - 1, -1, -1):
         # diagonalization of the bidiagonal form:
         #   loop over singular values, and over allowed itations
 
         its = 0
         while 1:
             its += 1
             flag = True
 
-            for l in xrange(k, -1, -1):
+            for l in range(k, -1, -1):
                 nm = l-1
 
                 if ctx.fabs(work[l]) + anorm == anorm:
                     flag = False
                     break
 
                 if ctx.fabs(S[nm]) + anorm == anorm:
                     break
 
             if flag:
                 c = 0
                 s = 1
-                for i in xrange(l, k + 1):
+                for i in range(l, k + 1):
                     f = s * work[i]
                     work[i] *= c
                     if ctx.fabs(f) + anorm == anorm:
                         break
                     g = S[i]
                     h = ctx.hypot(f, g)
                     S[i] = h
                     h = 1 / h
                     c = g * h
                     s = - f * h
 
                     if calc_u:
-                        for j in xrange(m):
+                        for j in range(m):
                             y = A[j,nm]
                             z = A[j,i]
                             A[j,nm] = y * c + z * s
                             A[j,i]  = z * c - y * s
 
             z = S[k]
 
             if l == k:               # convergence
                 if z < 0:            # singular value is made nonnegative
                     S[k] = -z
                     if not isinstance(V, bool):
-                        for j in xrange(n):
+                        for j in range(n):
                             V[k,j] = -V[k,j]
                 break
 
             if its >= maxits:
                 raise RuntimeError("svd: no convergence to an eigenvalue after %d iterations" % its)
 
             x = S[l]         # shift from bottom 2 by 2 minor
@@ -1114,82 +1110,82 @@
             f = ((y - z) * (y + z) + (g - h) * (g + h))/(2 * h * y)
             g = ctx.hypot(f, 1)
             if f >= 0: f = ((x - z) * (x + z) + h * ((y / (f + g)) - h)) / x
             else:      f = ((x - z) * (x + z) + h * ((y / (f - g)) - h)) / x
 
             c = s = 1         # next qt transformation
 
-            for j in xrange(l, nm + 1):
+            for j in range(l, nm + 1):
                 g = work[j+1]
                 y = S[j+1]
                 h = s * g
                 g = c * g
                 z = ctx.hypot(f, h)
                 work[j] = z
                 c = f / z
                 s = h / z
                 f = x * c + g * s
                 g = g * c - x * s
                 h = y * s
                 y *= c
                 if not isinstance(V, bool):
-                    for jj in xrange(n):
+                    for jj in range(n):
                         x = V[j  ,jj]
                         z = V[j+1,jj]
                         V[j    ,jj]= x * c + z * s
                         V[j+1  ,jj]= z * c - x * s
                 z = ctx.hypot(f, h)
                 S[j] = z
                 if z != 0:            # rotation can be arbitray if z=0
                     z = 1 / z
                     c = f * z
                     s = h * z
                 f = c * g + s * y
                 x = c * y - s * g
 
                 if calc_u:
-                    for jj in xrange(m):
+                    for jj in range(m):
                         y = A[jj,j  ]
                         z = A[jj,j+1]
                         A[jj,j    ] = y * c + z * s
                         A[jj,j+1  ] = z * c - y * s
 
             work[l] = 0
             work[k] = f
             S[k] = x
 
     ##########################
 
     # Sort singular values into decreasing order (bubble-sort)
 
-    for i in xrange(n):
+    for i in range(n):
         imax = i
         s = ctx.fabs(S[i])         # s is the current maximal element
 
-        for j in xrange(i + 1, n):
+        for j in range(i + 1, n):
             c = ctx.fabs(S[j])
             if c > s:
                 s = c
                 imax = j
 
         if imax != i:
             # swap singular values
 
             z = S[i]
             S[i] = S[imax]
             S[imax] = z
 
             if calc_u:
-                for j in xrange(m):
+                for j in range(m):
                     z = A[j,i]
                     A[j,i] = A[j,imax]
                     A[j,imax] = z
 
             if not isinstance(V, bool):
-                for j in xrange(n):
+                for j in range(n):
                     z = V[i,j]
                     V[i,j] = V[imax,j]
                     V[imax,j] = z
 
     return S
 
 #######################
@@ -1250,22 +1246,22 @@
     lbeta = ctx.zeros(n, 1)
     rbeta = ctx.zeros(n, 1)
     dwork = ctx.zeros(n, 1)
 
     g = scale = anorm = 0
     maxits = 3 * ctx.dps
 
-    for i in xrange(n):         # householder reduction to bidiagonal form
+    for i in range(n):         # householder reduction to bidiagonal form
         dwork[i] = scale * g    # dwork are the side-diagonal elements
         g = s = scale = 0
         if i < m:
-            for k in xrange(i, m):
+            for k in range(i, m):
                 scale += ctx.fabs(ctx.re(A[k,i])) + ctx.fabs(ctx.im(A[k,i]))
             if scale != 0:
-                for k in xrange(i, m):
+                for k in range(i, m):
                     A[k,i] /= scale
                     ar = ctx.re(A[k,i])
                     ai = ctx.im(A[k,i])
                     s += ar * ar + ai * ai
                 f = A[i,i]
                 g = -ctx.sqrt(s)
                 if ctx.re(f) < 0:
@@ -1275,32 +1271,32 @@
                     beta = -g + ctx.conj(f)
                 beta /= ctx.conj(beta)
                 beta += 1
                 h = 2 * (ctx.re(f) * g - s)
                 A[i,i] = f - g
                 beta /= h
                 lbeta[i] = (beta / scale) / scale
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     s = 0
-                    for k in xrange(i, m):
+                    for k in range(i, m):
                         s += ctx.conj(A[k,i]) * A[k,j]
                     f = beta * s
-                    for k in xrange(i, m):
+                    for k in range(i, m):
                         A[k,j] += f * A[k,i]
-                for k in xrange(i, m):
+                for k in range(i, m):
                     A[k,i] *= scale
 
         S[i] = scale * g     # S are the diagonal elements
         g = s = scale = 0
 
         if i < m and i != n - 1:
-            for k in xrange(i+1, n):
+            for k in range(i+1, n):
                 scale += ctx.fabs(ctx.re(A[i,k])) + ctx.fabs(ctx.im(A[i,k]))
             if scale:
-                for k in xrange(i+1, n):
+                for k in range(i+1, n):
                     A[i,k] /= scale
                     ar = ctx.re(A[i,k])
                     ai = ctx.im(A[i,k])
                     s += ar * ar + ai * ai
                 f = A[i,i+1]
                 g = -ctx.sqrt(s)
                 if ctx.re(f) < 0:
@@ -1314,122 +1310,122 @@
 
                 h = 2 * (ctx.re(f) * g - s)
                 A[i,i+1] = f - g
 
                 beta /= h
                 rbeta[i] = (beta / scale) / scale
 
-                for k in xrange(i+1, n):
+                for k in range(i+1, n):
                     work[k] = A[i, k]
 
-                for j in xrange(i+1, m):
+                for j in range(i+1, m):
                     s = 0
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         s += ctx.conj(A[i,k]) * A[j,k]
                     f = s * beta
-                    for k in xrange(i+1,n):
+                    for k in range(i+1,n):
                         A[j,k] += f * work[k]
 
-                for k in xrange(i+1, n):
+                for k in range(i+1, n):
                     A[i,k] *= scale
 
         anorm = max(anorm,ctx.fabs(S[i]) + ctx.fabs(dwork[i]))
 
     if not isinstance(V, bool):
-        for i in xrange(n-2, -1, -1):     # accumulation of right hand transformations
+        for i in range(n-2, -1, -1):     # accumulation of right hand transformations
             V[i+1,i+1] = 1
 
             if dwork[i+1] != 0:
                 f = ctx.conj(rbeta[i])
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     V[i,j] = A[i,j] * f
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     s = 0
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         s += ctx.conj(A[i,k]) * V[j,k]
-                    for k in xrange(i+1, n):
+                    for k in range(i+1, n):
                         V[j,k] += s * V[i,k]
 
-            for j in xrange(i+1,n):
+            for j in range(i+1,n):
                 V[j,i] = V[i,j] = 0
 
         V[0,0] = 1
 
     if m < n : minnm = m
     else     : minnm = n
 
     if calc_u:
-        for i in xrange(minnm-1, -1, -1): # accumulation of left hand transformations
+        for i in range(minnm-1, -1, -1): # accumulation of left hand transformations
             g = S[i]
-            for j in xrange(i+1, n):
+            for j in range(i+1, n):
                 A[i,j] = 0
             if g != 0:
                 g = 1 / g
-                for j in xrange(i+1, n):
+                for j in range(i+1, n):
                     s = 0
-                    for k in xrange(i+1, m):
+                    for k in range(i+1, m):
                         s += ctx.conj(A[k,i]) * A[k,j]
                     f = s * ctx.conj(lbeta[i])
-                    for k in xrange(i, m):
+                    for k in range(i, m):
                         A[k,j] += f * A[k,i]
-                for j in xrange(i, m):
+                for j in range(i, m):
                     A[j,i] *= g
             else:
-                for j in xrange(i, m):
+                for j in range(i, m):
                     A[j,i] = 0
             A[i,i] += 1
 
-    for k in xrange(n-1, -1, -1):
+    for k in range(n-1, -1, -1):
         # diagonalization of the bidiagonal form:
         #   loop over singular values, and over allowed itations
 
         its = 0
         while 1:
             its += 1
             flag = True
 
-            for l in xrange(k, -1, -1):
+            for l in range(k, -1, -1):
                 nm = l - 1
 
                 if ctx.fabs(dwork[l]) + anorm == anorm:
                     flag = False
                     break
 
                 if ctx.fabs(S[nm]) + anorm == anorm:
                     break
 
             if flag:
                 c = 0
                 s = 1
-                for i in xrange(l, k+1):
+                for i in range(l, k+1):
                     f = s * dwork[i]
                     dwork[i] *= c
                     if ctx.fabs(f) + anorm == anorm:
                         break
                     g = S[i]
                     h = ctx.hypot(f, g)
                     S[i] = h
                     h = 1 / h
                     c = g * h
                     s = -f * h
 
                     if calc_u:
-                        for j in xrange(m):
+                        for j in range(m):
                             y = A[j,nm]
                             z = A[j,i]
                             A[j,nm]= y * c + z * s
                             A[j,i] = z * c - y * s
 
             z = S[k]
 
             if l == k:         # convergence
                 if z < 0:    # singular value is made nonnegative
                     S[k] = -z
                     if not isinstance(V, bool):
-                        for j in xrange(n):
+                        for j in range(n):
                             V[k,j] = -V[k,j]
                 break
 
             if its >= maxits:
                 raise RuntimeError("svd: no convergence to an eigenvalue after %d iterations" % its)
 
             x = S[l]         # shift from bottom 2 by 2 minor
@@ -1440,81 +1436,81 @@
             f = ((y - z) * (y + z) + (g - h) * (g + h)) / (2 * h * y)
             g = ctx.hypot(f, 1)
             if f >=0: f = (( x - z) *( x + z) + h *((y / (f + g)) - h)) / x
             else:     f = (( x - z) *( x + z) + h *((y / (f - g)) - h)) / x
 
             c = s = 1         # next qt transformation
 
-            for j in xrange(l, nm + 1):
+            for j in range(l, nm + 1):
                 g = dwork[j+1]
                 y = S[j+1]
                 h = s * g
                 g = c * g
                 z = ctx.hypot(f, h)
                 dwork[j] = z
                 c = f / z
                 s = h / z
                 f = x * c + g * s
                 g = g * c - x * s
                 h = y * s
                 y *= c
                 if not isinstance(V, bool):
-                    for jj in xrange(n):
+                    for jj in range(n):
                         x = V[j  ,jj]
                         z = V[j+1,jj]
                         V[j    ,jj]= x * c + z * s
                         V[j+1,jj  ]= z * c - x * s
                 z = ctx.hypot(f, h)
                 S[j] = z
                 if z != 0:            # rotation can be arbitray if z=0
                     z = 1 / z
                     c = f * z
                     s = h * z
                 f = c * g + s * y
                 x = c * y - s * g
                 if calc_u:
-                    for jj in xrange(m):
+                    for jj in range(m):
                         y = A[jj,j  ]
                         z = A[jj,j+1]
                         A[jj,j    ]= y * c + z * s
                         A[jj,j+1  ]= z * c - y * s
 
             dwork[l] = 0
             dwork[k] = f
             S[k] = x
 
     ##########################
 
     # Sort singular values into decreasing order (bubble-sort)
 
-    for i in xrange(n):
+    for i in range(n):
         imax = i
         s = ctx.fabs(S[i])         # s is the current maximal element
 
-        for j in xrange(i + 1, n):
+        for j in range(i + 1, n):
             c = ctx.fabs(S[j])
             if c > s:
                 s = c
                 imax = j
 
         if imax != i:
             # swap singular values
 
             z = S[i]
             S[i] = S[imax]
             S[imax] = z
 
             if calc_u:
-                for j in xrange(m):
+                for j in range(m):
                     z = A[j,i]
                     A[j,i] = A[j,imax]
                     A[j,imax] = z
 
             if not isinstance(V, bool):
-                for j in xrange(n):
+                for j in range(n):
                     z = V[i,j]
                     V[i,j] = V[imax,j]
                     V[imax,j] = z
 
     return S
 
 ##################################################################################################
@@ -1610,15 +1606,15 @@
     else:
         if not overwrite_a:
             A = A.copy()
         V = ctx.zeros(n, n)
         S = svd_r_raw(ctx, A, V, calc_u = True)
 
         if n > m:
-            if full_matrices == False:
+            if full_matrices is False:
                 V = V[:m,:]
 
             S = S[:m]
             A = A[:,:m]
 
         return (A, S, V)
 
@@ -1714,15 +1710,15 @@
     else:
         if not overwrite_a:
             A = A.copy()
         V = ctx.zeros(n, n)
         S = svd_c_raw(ctx, A, V, calc_u = True)
 
         if n > m:
-            if full_matrices == False:
+            if full_matrices is False:
                 V = V[:m,:]
 
             S = S[:m]
             A = A[:,:m]
 
         return (A, S, V)
```

### Comparing `mpmath-1.3.0/mpmath/matrices/linalg.py` & `mpmath-1.4.0a0/mpmath/matrices/linalg.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 equation system::
 
       x + 2*y = -10
     3*x + 4*y =  10
 
 using ``lu_solve``::
 
-    >>> from mpmath import *
-    >>> mp.pretty = False
+    >>> from mpmath import matrix, lu_solve, residual, eps, fp, lu, iv
     >>> A = matrix([[1, 2], [3, 4]])
     >>> b = matrix([-10, 10])
     >>> x = lu_solve(A, b)
     >>> x
     matrix(
     [['30.0'],
      ['-20.0']])
@@ -35,15 +34,15 @@
 As you can see, the solution is quite accurate. The error is caused by the
 inaccuracy of the internal floating point arithmetic. Though, it's even smaller
 than the current machine epsilon, which basically means you can trust the
 result.
 
 If you need more speed, use NumPy, or ``fp.lu_solve`` for a floating-point computation.
 
-    >>> fp.lu_solve(A, b)   # doctest: +ELLIPSIS
+    >>> fp.lu_solve(A, b)
     matrix(...)
 
 ``lu_solve`` accepts overdetermined systems. It is usually not possible to solve
 such systems, so the residual is minimized instead. Internally this is done
 using Cholesky decomposition to compute a least squares approximation. This means
 that that ``lu_solve`` will square the errors. If you can't afford this, use
 ``qr_solve`` instead. It is twice as slow but more accurate, and it calculates
@@ -83,33 +82,32 @@
     >>> a = iv.matrix([['0.1','0.3','1.0'],
     ...             ['7.1','5.5','4.8'],
     ...             ['3.2','4.4','5.6']])
     >>>
     >>> b = iv.matrix(['4','0.6','0.5'])
     >>> c = iv.lu_solve(a, b)
     >>> print(c)
-    [   [5.2582327113062568605927528666, 5.25823271130625686059275702219]]
-    [[-13.1550493962678375411635581388, -13.1550493962678375411635540152]]
-    [  [7.42069154774972557628979076189, 7.42069154774972557628979190734]]
+    [  [5.2582327113062393041, 5.2582327113062749951]]
+    [[-13.155049396267856583, -13.155049396267821167]]
+    [  [7.4206915477497212555, 7.4206915477497310922]]
     >>> print(a*c)
-    [  [3.99999999999999999999999844904, 4.00000000000000000000000155096]]
-    [[0.599999999999999999999968898009, 0.600000000000000000000031763736]]
-    [[0.499999999999999999999979320485, 0.500000000000000000000020679515]]
+    [  [3.9999999999999866773, 4.0000000000000133227]]
+    [[0.59999999999972430942, 0.60000000000027142733]]
+    [[0.49999999999982236432, 0.50000000000018474111]]
 """
 
 # TODO:
 # *implement high-level qr()
 # *test unitvector
 # *iterative solving
 
 from copy import copy
 
-from ..libmp.backend import xrange
 
-class LinearAlgebraMethods(object):
+class LinearAlgebraMethods:
 
     def LU_decomp(ctx, A, overwrite=False, use_cache=True):
         """
         LU-factorization of a n*n matrix using the Gauss algorithm.
         Returns L and U in one matrix and the pivot indices.
 
         Use overwrite to specify whether A will be overwritten with L and U.
@@ -121,33 +119,36 @@
             return A._LU
         if not overwrite:
             orig = A
             A = A.copy()
         tol = ctx.absmin(ctx.mnorm(A,1) * ctx.eps) # each pivot element has to be bigger
         n = A.rows
         p = [None]*(n - 1)
-        for j in xrange(n - 1):
+        for j in range(n - 1):
             # pivoting, choose max(abs(reciprocal row sum)*abs(pivot element))
             biggest = 0
-            for k in xrange(j, n):
-                s = ctx.fsum([ctx.absmin(A[k,l]) for l in xrange(j, n)])
+            for k in range(j, n):
+                s = ctx.fsum([ctx.absmin(A[k,l]) for l in range(j, n)])
                 if ctx.absmin(s) <= tol:
                     raise ZeroDivisionError('matrix is numerically singular')
                 current = 1/s * ctx.absmin(A[k,j])
                 if current > biggest: # TODO: what if equal?
                     biggest = current
                     p[j] = k
+            # without pivot LU fails
+            if p[j] is None:
+                raise ZeroDivisionError('matrix is numerically singular')
             # swap rows according to p
             ctx.swap_row(A, j, p[j])
             if ctx.absmin(A[j,j]) <= tol:
                 raise ZeroDivisionError('matrix is numerically singular')
             # calculate elimination factors and add rows
-            for i in xrange(j + 1, n):
+            for i in range(j + 1, n):
                 A[i,j] /= A[j,j]
-                for k in xrange(j + 1, n):
+                for k in range(j + 1, n):
                     A[i,k] -= A[i,j]*A[j,k]
         if ctx.absmin(A[n - 1,n - 1]) <= tol:
             raise ZeroDivisionError('matrix is numerically singular')
         # cache decomposition
         if not overwrite and isinstance(orig, ctx.matrix):
             orig._LU = (A, p)
         return A, p
@@ -159,34 +160,34 @@
         if L.rows != L.cols:
             raise RuntimeError("need n*n matrix")
         n = L.rows
         if len(b) != n:
             raise ValueError("Value should be equal to n")
         b = copy(b)
         if p: # swap b according to p
-            for k in xrange(0, len(p)):
+            for k in range(len(p)):
                 ctx.swap_row(b, k, p[k])
         # solve
-        for i in xrange(1, n):
-            for j in xrange(i):
+        for i in range(1, n):
+            for j in range(i):
                 b[i] -= L[i,j] * b[j]
         return b
 
     def U_solve(ctx, U, y):
         """
         Solve the upper part of a LU factorized matrix for x.
         """
         if U.rows != U.cols:
             raise RuntimeError("need n*n matrix")
         n = U.rows
         if len(y) != n:
             raise ValueError("Value should be equal to n")
         x = copy(y)
-        for i in xrange(n - 1, -1, -1):
-            for j in xrange(i + 1, n):
+        for i in range(n - 1, -1, -1):
+            for j in range(i + 1, n):
                 x[i] -= U[i,j] * x[j]
             x[i] /= U[i,i]
         return x
 
     def lu_solve(ctx, A, b, **kwargs):
         """
         Ax = b => x
@@ -233,15 +234,15 @@
         Improve a solution to a linear equation system iteratively.
 
         This re-uses the LU decomposition and is thus cheap.
         Usually 3 up to 4 iterations are giving the maximal improvement.
         """
         if A.rows != A.cols:
             raise RuntimeError("need n*n matrix") # TODO: really?
-        for _ in xrange(maxsteps):
+        for _ in range(maxsteps):
             r = ctx.residual(A, x, b)
             if ctx.norm(r, 2) < 10*ctx.eps:
                 break
             # this uses cached LU decomposition and is thus cheap
             dx = ctx.lu_solve(A, -r)
             x += dx
         return x
@@ -259,26 +260,26 @@
         much more memory efficient.
         """
         # get factorization
         A, p = ctx.LU_decomp(A)
         n = A.rows
         L = ctx.matrix(n)
         U = ctx.matrix(n)
-        for i in xrange(n):
-            for j in xrange(n):
+        for i in range(n):
+            for j in range(n):
                 if i > j:
                     L[i,j] = A[i,j]
                 elif i == j:
                     L[i,j] = 1
                     U[i,j] = A[i,j]
                 else:
                     U[i,j] = A[i,j]
         # calculate permutation matrix
         P = ctx.eye(n)
-        for k in xrange(len(p)):
+        for k in range(len(p)):
             ctx.swap_row(P, k, p[k])
         return P, L, U
 
     def unitvector(ctx, n, i):
         """
         Return the i-th n-dimensional unit vector.
         """
@@ -298,23 +299,23 @@
             # do not overwrite A
             A = ctx.matrix(A, **kwargs).copy()
             n = A.rows
             # get LU factorisation
             A, p = ctx.LU_decomp(A)
             cols = []
             # calculate unit vectors and solve corresponding system to get columns
-            for i in xrange(1, n + 1):
+            for i in range(1, n + 1):
                 e = ctx.unitvector(n, i)
                 y = ctx.L_solve(A, e, p)
                 cols.append(ctx.U_solve(A, y))
             # convert columns to matrix
             inv = []
-            for i in xrange(n):
+            for i in range(n):
                 row = []
-                for j in xrange(n):
+                for j in range(n):
                     row.append(cols[j][i])
                 inv.append(row)
             result = ctx.matrix(inv, **kwargs)
         finally:
             ctx.prec = prec
         return result
 
@@ -331,33 +332,33 @@
             raise TypeError("A should be a type of ctx.matrix")
         m = A.rows
         n = A.cols
         if m < n - 1:
             raise RuntimeError("Columns should not be less than rows")
         # calculate Householder matrix
         p = []
-        for j in xrange(0, n - 1):
-            s = ctx.fsum(abs(A[i,j])**2 for i in xrange(j, m))
+        for j in range(n - 1):
+            s = ctx.fsum(abs(A[i,j])**2 for i in range(j, m))
             if not abs(s) > ctx.eps:
                 raise ValueError('matrix is numerically singular')
             p.append(-ctx.sign(ctx.re(A[j,j])) * ctx.sqrt(s))
             kappa = ctx.one / (s - p[j] * A[j,j])
             A[j,j] -= p[j]
-            for k in xrange(j+1, n):
-                y = ctx.fsum(ctx.conj(A[i,j]) * A[i,k] for i in xrange(j, m)) * kappa
-                for i in xrange(j, m):
+            for k in range(j+1, n):
+                y = ctx.fsum(ctx.conj(A[i,j]) * A[i,k] for i in range(j, m)) * kappa
+                for i in range(j, m):
                     A[i,k] -= A[i,j] * y
         # solve Rx = c1
-        x = [A[i,n - 1] for i in xrange(n - 1)]
-        for i in xrange(n - 2, -1, -1):
-            x[i] -= ctx.fsum(A[i,j] * x[j] for j in xrange(i + 1, n - 1))
+        x = [A[i,n - 1] for i in range(n - 1)]
+        for i in range(n - 2, -1, -1):
+            x[i] -= ctx.fsum(A[i,j] * x[j] for j in range(i + 1, n - 1))
             x[i] /= p[i]
         # calculate residual
         if not m == n - 1:
-            r = [A[m-1-i, n-1] for i in xrange(m - n + 1)]
+            r = [A[m-1-i, n-1] for i in range(m - n + 1)]
         else:
             # determined system, residual should be 0
             r = [0]*m # maybe a bad idea, changing r[i] will change all elements
         return A, p, x, r
 
     #def qr(ctx, A):
     #    """
@@ -427,15 +428,16 @@
         The optional parameter ``tol`` determines the tolerance for
         verifying positive-definiteness.
 
         **Examples**
 
         Cholesky decomposition of a positive-definite symmetric matrix::
 
-            >>> from mpmath import *
+            >>> from mpmath import (mp, eye, hilbert, nprint, cholesky,
+            ...                     chop, matrix)
             >>> mp.dps = 25; mp.pretty = True
             >>> A = eye(3) + hilbert(3)
             >>> nprint(A)
             [     2.0      0.5  0.333333]
             [     0.5  1.33333      0.25]
             [0.333333     0.25       1.2]
             >>> L = cholesky(A)
@@ -479,26 +481,26 @@
             raise RuntimeError("A should be a type of ctx.matrix")
         if not A.rows == A.cols:
             raise ValueError('need n*n matrix')
         if tol is None:
             tol = +ctx.eps
         n = A.rows
         L = ctx.matrix(n)
-        for j in xrange(n):
+        for j in range(n):
             c = ctx.re(A[j,j])
             if abs(c-A[j,j]) > tol:
                 raise ValueError('matrix is not Hermitian')
-            s = c - ctx.fsum((L[j,k] for k in xrange(j)),
+            s = c - ctx.fsum((L[j,k] for k in range(j)),
                 absolute=True, squared=True)
             if s < tol:
                 raise ValueError('matrix is not positive-definite')
             L[j,j] = ctx.sqrt(s)
-            for i in xrange(j, n):
-                it1 = (L[i,k] for k in xrange(j))
-                it2 = (L[j,k] for k in xrange(j))
+            for i in range(j, n):
+                it1 = (L[i,k] for k in range(j))
+                it2 = (L[j,k] for k in range(j))
                 t = ctx.fdot(it1, it2, conjugate=True)
                 L[i,j] = (A[i,j] - t) / L[j,j]
         return L
 
     def cholesky_solve(ctx, A, b, **kwargs):
         """
         Ax = b => x
@@ -520,40 +522,90 @@
                 raise ValueError('can only solve determined system')
             # Cholesky factorization
             L = ctx.cholesky(A)
             # solve
             n = L.rows
             if len(b) != n:
                 raise ValueError("Value should be equal to n")
-            for i in xrange(n):
-                b[i] -= ctx.fsum(L[i,j] * b[j] for j in xrange(i))
+            for i in range(n):
+                b[i] -= ctx.fsum(L[i,j] * b[j] for j in range(i))
                 b[i] /= L[i,i]
-            x = ctx.U_solve(L.T, b)
+            x = ctx.U_solve(L.H, b)
             return x
         finally:
             ctx.prec = prec
 
     def det(ctx, A):
         """
-        Calculate the determinant of a matrix.
+        Calculate the determinant of a square matrix.
+
+        The determinant is the normed, alternating n-linear from,
+        i.e. a multiplicative map for each matrix into the
+        field of numbers of its entries.
+
+        **Examples**
+
+        Determinant of identity is 1.
+
+        >>> from mpmath import eye, matrix, det
+        >>> A = eye(3)
+        >>> print(det(A))
+        1.0
+
+        But in general a matrix can have any number as its determinant.
+
+        >>> A = matrix([[2, 6, 4],[3, 8, 6],[1, 1, 2]])
+        >>> print(det(A))
+        0
+
+        The determinant is vanishing if a matrix has no inverse.
+
+        >>> A = matrix([[1, 3, 2],[0, 1, 0],[0, 0, 0]])
+        >>> print(det(A))
+        0
+
+        But, matrix has determinate different from zero full rank if and only is is equivalent to identity,
+
+        >>> A = matrix([[1, 3, -2], [1, 9, -6], [1, 4, -3]])
+        >>> print(det(A))
+        -2.0
+
+        i.e. has an inverse matrix.
+
+        >>> B = matrix([[3, -1, 0], [3, 1, -4], [5, 1, -6]]) / 2
+        >>> A*B == eye(3)
+        True
+        >>> print(det(B))
+        -0.5
+
+        Moreover, a matrix of integers has an inverse matrix of integers
+        if and only if the determinat is equal to either 1 or -1.
+
+        >>> A = matrix([[1, 0, 1],[-2, 1, -2],[-4, 1, -5]])
+        >>> B = matrix([[3, -1, 1],[2, 1, 0],[-2, 1, -1]])
+        >>> A*B == eye(3)
+        True
+        >>> print(det(A), det(B))
+        -1.0 -1.0
+
         """
         prec = ctx.prec
         try:
             # do not overwrite A
             A = ctx.matrix(A).copy()
             # use LU factorization to calculate determinant
             try:
                 R, p = ctx.LU_decomp(A)
             except ZeroDivisionError:
                 return 0
             z = 1
             for i, e in enumerate(p):
                 if i != e:
                     z *= -1
-            for i in xrange(A.rows):
+            for i in range(A.rows):
                 z *= R[i,i]
             return z
         finally:
             ctx.prec = prec
 
     def cond(ctx, A, norm=None):
         """
@@ -595,15 +647,15 @@
         (3) Any other value returns the leading m columns of Q
             and m rows of R
 
         edps is the increase in mp precision used for calculations
 
         **Examples**
 
-            >>> from mpmath import *
+            >>> from mpmath import mp, qr, matrix, chop, nprint, j
             >>> mp.dps = 15
             >>> mp.pretty = True
             >>> A = matrix([[1, 2], [3, 4], [1, 1]])
             >>> Q, R = qr(A)
             >>> Q
             [-0.301511344577764   0.861640436855329   0.408248290463863]
             [-0.904534033733291  -0.123091490979333  -0.408248290463863]
@@ -658,21 +710,21 @@
             # ---------------
             if cmplx:
                 one = ctx.mpc('1.0', '0.0')
                 zero = ctx.mpc('0.0', '0.0')
                 rzero = ctx.mpf('0.0')
 
                 # main loop to factor A (complex)
-                for j in xrange(0, n):
+                for j in range(n):
                     alpha = A[j,j]
                     alphr = ctx.re(alpha)
                     alphi = ctx.im(alpha)
 
                     if (m-j) >= 2:
-                        xnorm = ctx.fsum( A[i,j]*ctx.conj(A[i,j]) for i in xrange(j+1, m) )
+                        xnorm = ctx.fsum( A[i,j]*ctx.conj(A[i,j]) for i in range(j+1, m) )
                         xnorm = ctx.re( ctx.sqrt(xnorm) )
                     else:
                         xnorm = rzero
 
                     if (xnorm == rzero) and (alphi == rzero):
                         tau[j] = zero
                         continue
@@ -682,35 +734,35 @@
                     else:
                         beta = -ctx.sqrt(alphr**2 + alphi**2 + xnorm**2)
 
                     tau[j] = ctx.mpc( (beta - alphr) / beta, -alphi / beta )
                     t = -ctx.conj(tau[j])
                     za = one / (alpha - beta)
 
-                    for i in xrange(j+1, m):
+                    for i in range(j+1, m):
                         A[i,j] *= za
 
                     A[j,j] = one
-                    for k in xrange(j+1, n):
-                        y = ctx.fsum(A[i,j] * ctx.conj(A[i,k]) for i in xrange(j, m))
+                    for k in range(j+1, n):
+                        y = ctx.fsum(A[i,j] * ctx.conj(A[i,k]) for i in range(j, m))
                         temp = t * ctx.conj(y)
-                        for i in xrange(j, m):
+                        for i in range(j, m):
                             A[i,k] += A[i,j] * temp
 
                     A[j,j] = ctx.mpc(beta, '0.0')
             else:
                 one = ctx.mpf('1.0')
                 zero = ctx.mpf('0.0')
 
                 # main loop to factor A (real)
-                for j in xrange(0, n):
+                for j in range(n):
                     alpha = A[j,j]
 
                     if (m-j) > 2:
-                        xnorm = ctx.fsum( (A[i,j])**2 for i in xrange(j+1, m) )
+                        xnorm = ctx.fsum( (A[i,j])**2 for i in range(j+1, m) )
                         xnorm = ctx.sqrt(xnorm)
                     elif (m-j) == 2:
                         xnorm = abs( A[m-1,j] )
                     else:
                         xnorm = zero
 
                     if xnorm == zero:
@@ -722,69 +774,148 @@
                     else:
                         beta = -ctx.sqrt(alpha**2 + xnorm**2)
 
                     tau[j] = (beta - alpha) / beta
                     t = -tau[j]
                     da = one / (alpha - beta)
 
-                    for i in xrange(j+1, m):
+                    for i in range(j+1, m):
                         A[i,j] *= da
 
                     A[j,j] = one
-                    for k in xrange(j+1, n):
-                        y = ctx.fsum( A[i,j] * A[i,k] for i in xrange(j, m) )
+                    for k in range(j+1, n):
+                        y = ctx.fsum( A[i,j] * A[i,k] for i in range(j, m) )
                         temp = t * y
-                        for i in xrange(j,m):
+                        for i in range(j,m):
                             A[i,k] += A[i,j] * temp
 
                     A[j,j] = beta
 
             # return factorization in same internal format as LAPACK
             if (mode == 'raw') or (mode == 'RAW'):
                 return A, tau
 
             # ----------------------------------
             # FORM Q USING BACKWARD ACCUMULATION
             # ----------------------------------
 
             # form R before the values are overwritten
             R = A.copy()
-            for j in xrange(0, n):
-                for i in xrange(j+1, m):
+            for j in range(n):
+                for i in range(j+1, m):
                     R[i,j] = zero
 
             # set the value of p (number of columns of Q to return)
             p = m
             if (mode == 'skinny') or (mode == 'SKINNY'):
                 p = n
 
             # add columns to A if needed and initialize
             A.cols += (p-n)
-            for j in xrange(0, p):
+            for j in range(p):
                 A[j,j] = one
-                for i in xrange(0, j):
+                for i in range(j):
                     A[i,j] = zero
 
             # main loop to form Q
-            for j in xrange(n-1, -1, -1):
+            for j in range(n-1, -1, -1):
                 t = -tau[j]
                 A[j,j] += t
 
-                for k in xrange(j+1, p):
+                for k in range(j+1, p):
                     if cmplx:
-                        y = ctx.fsum(A[i,j] * ctx.conj(A[i,k]) for i in xrange(j+1, m))
+                        y = ctx.fsum(A[i,j] * ctx.conj(A[i,k]) for i in range(j+1, m))
                         temp = t * ctx.conj(y)
                     else:
-                        y = ctx.fsum(A[i,j] * A[i,k] for i in xrange(j+1, m))
+                        y = ctx.fsum(A[i,j] * A[i,k] for i in range(j+1, m))
                         temp = t * y
                     A[j,k] = temp
-                    for i in xrange(j+1, m):
+                    for i in range(j+1, m):
                         A[i,k] += A[i,j] * temp
 
-                for i in xrange(j+1, m):
+                for i in range(j+1, m):
                     A[i, j] *= t
 
             return A, R[0:p,0:n]
 
         # ------------------
         # END OF FUNCTION QR
         # ------------------
+
+    def rank(ctx, A, iszerofunc=None):
+        """
+        Calculate the rank of a matrix.
+
+        This corresponds to the maximal
+        number of linear independent
+        columns (or rows equivalently).
+
+        Rank is computed via singular value decomposition
+        by counting the number of non-zero singular values.
+
+        The argument 'iszerofunc' allows for the provision
+        of a custom function to enable zero detection customization.
+
+        **Examples**
+
+        Rank of identity is same as its dimension.
+
+        >>> from mpmath import eye, matrix, rank, zeros, qr
+        >>> A = eye(3)
+        >>> rank(A)
+        3
+
+        But in general a matrix has rank less or equal of its dimension.
+
+        >>> A = matrix([[2, 6, 4],[3, 8, 6],[1, 1, 2]])
+        >>> rank(A)
+        2
+
+        The rank is given by the number of non zero lines in an
+        equivalent triangular matrix.
+
+        >>> R = matrix([[1, 3, 2],[0, 1, 0],[0, 0, 0]])
+        >>> rank(A)
+        2
+
+        The rank is zero if and only if the matrix is zero.
+
+        >>> A = zeros(3)
+        >>> rank(A)
+        0
+
+        The matrix has full rank if and only ist is equivalent to identity,
+
+        >>> A = matrix([[1, 0, 1],[-2, 1, -2],[-4, 1, -5]])
+        >>> rank(A)
+        3
+
+        i.e. has an inverse matrix.
+
+        >>> B = matrix([[3, -1, 1],[2, 1, 0],[-2, 1, -1]])
+        >>> A*B == eye(3)
+        True
+        >>> rank(B)
+        3
+
+        to handle numerical precision zero evaluation can be customized
+        by providing an `iszerofunc`
+
+        >>> A = matrix([[2, 6, 4],[3, 8, 6],[1, 1, 2]])
+        >>> _, R = qr(A)
+        >>> R
+        matrix(
+        [['-3.74165738677394', '-9.8886659507597', '-7.48331477354788'],
+         ['0.0', '1.79284291400159', '-2.548055495426e-26'],
+         ['0.0', '0.0', '4.35114889954169e-27']])
+
+        to take advantage of full precision provide a custom `iszerofunc`
+
+        >>> iszerofunc = lambda x: not bool(x)
+        >>> rank(R, iszerofunc)
+        3
+
+        """
+        if iszerofunc is None:
+            iszerofunc = lambda v: ctx.absmin(v) < ctx.eps
+
+        return sum(1 for v in ctx.svd_r(A, compute_uv=False) if not iszerofunc(v))
```

### Comparing `mpmath-1.3.0/mpmath/matrices/matrices.py` & `mpmath-1.4.0a0/mpmath/matrices/matrices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from ..libmp.backend import xrange
 import warnings
 
 # TODO: interpret list as vectors (for multiplication)
 
 rowsep = '\n'
 colsep = '  '
 
-class _matrix(object):
+class _matrix:
     """
     Numerical matrix.
 
     Specify the dimensions or the data as a nested list.
     Elements default to zero.
     Use a flat list to create a column vector easily.
 
@@ -21,15 +20,16 @@
 
     Matrices in mpmath are implemented using dictionaries. Only non-zero values
     are stored, so it is cheap to represent sparse matrices.
 
     The most basic way to create one is to use the ``matrix`` class directly.
     You can create an empty matrix specifying the dimensions:
 
-        >>> from mpmath import *
+        >>> from mpmath import (mp, matrix, randmatrix, nprint, ones, norm,
+        ...                     mnorm, inf)
         >>> mp.dps = 15
         >>> matrix(2)
         matrix(
         [['0.0', '0.0'],
          ['0.0', '0.0']])
         >>> matrix(2, 3)
         matrix(
@@ -162,15 +162,15 @@
         matrix(
         [['-1.0', '6.0'],
          ['8.0', '13.0']])
         >>> A - B
         matrix(
         [['3.0', '-2.0'],
          ['-2.0', '-5.0']])
-        >>> A + ones(3) # doctest:+ELLIPSIS
+        >>> A + ones(3)
         Traceback (most recent call last):
           ...
         ValueError: incompatible dimensions for addition
 
     It is possible to multiply or add matrices and scalars. In the latter case the
     operation will be done element-wise::
 
@@ -184,34 +184,30 @@
          ['0.75', '1.0']])
         >>> A - 1
         matrix(
         [['0.0', '1.0'],
          ['2.0', '3.0']])
 
     Of course you can perform matrix multiplication, if the dimensions are
-    compatible, using ``@`` (for Python >= 3.5) or ``*``. For clarity, ``@`` is
+    compatible, using ``@`` or ``*``. For clarity, ``@`` is
     recommended (`PEP 465 <https://www.python.org/dev/peps/pep-0465/>`), because
     the meaning of ``*`` is different in many other Python libraries such as NumPy.
 
-        >>> A @ B # doctest:+SKIP
+        >>> A @ B
         matrix(
         [['8.0', '22.0'],
          ['14.0', '48.0']])
         >>> A * B # same as A @ B
         matrix(
         [['8.0', '22.0'],
          ['14.0', '48.0']])
         >>> matrix([[1, 2, 3]]) * matrix([[-6], [7], [-2]])
         matrix(
         [['2.0']])
 
-    ..
-        COMMENT: TODO: the above "doctest:+SKIP" may be removed as soon as we
-        have dropped support for Python 3.5 and below.
-
     You can raise powers of square matrices::
 
         >>> A**2
         matrix(
         [['7.0', '10.0'],
          ['15.0', '22.0']])
 
@@ -316,32 +312,32 @@
                     raise TypeError("expected int")
                 self.__rows = args[0]
                 self.__cols = args[1]
         elif isinstance(args[0], _matrix):
             A = args[0]
             self.__rows = A._matrix__rows
             self.__cols = A._matrix__cols
-            for i in xrange(A.__rows):
-                for j in xrange(A.__cols):
+            for i in range(A.__rows):
+                for j in range(A.__cols):
                     self[i, j] = A[i, j]
         elif hasattr(args[0], 'tolist'):
             A = self.ctx.matrix(args[0].tolist())
             self.__data = A._matrix__data
             self.__rows = A._matrix__rows
             self.__cols = A._matrix__cols
         else:
             raise TypeError('could not interpret given arguments')
 
     def apply(self, f):
         """
         Return a copy of self with the function `f` applied elementwise.
         """
         new = self.ctx.matrix(self.__rows, self.__cols)
-        for i in xrange(self.__rows):
-            for j in xrange(self.__cols):
+        for i in range(self.__rows):
+            for j in range(self.__cols):
                 new[i,j] = f(self[i,j])
         return new
 
     def __nstr__(self, n=None, **kwargs):
         # Build table of string representations of the elements
         res = []
         # Track per-column max lengths for pretty alignment
@@ -371,17 +367,17 @@
         Create a list string from a matrix.
 
         If avoid_type: avoid multiple 'mpf's.
         """
         # XXX: should be something like self.ctx._types
         typ = self.ctx.mpf
         s = '['
-        for i in xrange(self.__rows):
+        for i in range(self.__rows):
             s += '['
-            for j in xrange(self.__cols):
+            for j in range(self.__cols):
                 if not avoid_type or not isinstance(self[i,j], typ):
                     a = repr(self[i,j])
                 else:
                     a = "'" + str(self[i,j]) + "'"
                 s += a + ', '
             s = s[:-2]
             s += '],\n '
@@ -450,33 +446,37 @@
 
             #Rows
             if isinstance(key[0],slice):
                 #Check bounds
                 if (key[0].start is None or key[0].start >= 0) and \
                     (key[0].stop is None or key[0].stop <= self.__rows+1):
                     # Generate indices
-                    rows = xrange(*key[0].indices(self.__rows))
+                    rows = range(*key[0].indices(self.__rows))
                 else:
                     raise IndexError('Row index out of bounds')
             else:
                 # Single row
+                if key[0] >= self.__rows:
+                    raise IndexError('Row index out of bounds')
                 rows = [key[0]]
 
             # Columns
             if isinstance(key[1],slice):
                 # Check bounds
                 if (key[1].start is None or key[1].start >= 0) and \
                     (key[1].stop is None or key[1].stop <= self.__cols+1):
                     # Generate indices
-                    columns = xrange(*key[1].indices(self.__cols))
+                    columns = range(*key[1].indices(self.__cols))
                 else:
                     raise IndexError('Column index out of bounds')
 
             else:
                 # Single column
+                if key[1] >= self.__cols:
+                    raise IndexError('Column index out of bounds')
                 columns = [key[1]]
 
             # Create matrix slice
             m = self.ctx.matrix(len(rows),len(columns))
 
             # Assign elements to the output matrix
             for i,x in enumerate(rows):
@@ -514,27 +514,27 @@
         if isinstance(key[0],slice) or isinstance(key[1],slice):
             # Rows
             if isinstance(key[0],slice):
                 # Check bounds
                 if (key[0].start is None or key[0].start >= 0) and \
                     (key[0].stop is None or key[0].stop <= self.__rows+1):
                     # generate row indices
-                    rows = xrange(*key[0].indices(self.__rows))
+                    rows = range(*key[0].indices(self.__rows))
                 else:
                     raise IndexError('Row index out of bounds')
             else:
                 # Single row
                 rows = [key[0]]
             # Columns
             if isinstance(key[1],slice):
                 # Check bounds
                 if (key[1].start is None or key[1].start >= 0) and \
                     (key[1].stop is None or key[1].stop <= self.__cols+1):
                     # Generate column indices
-                    columns = xrange(*key[1].indices(self.__cols))
+                    columns = range(*key[1].indices(self.__cols))
                 else:
                     raise IndexError('Column index out of bounds')
             else:
                 # Single column
                 columns = [key[1]]
             # Assign slice with a scalar
             if isinstance(value,self.ctx.matrix):
@@ -564,38 +564,34 @@
                 del self.__data[key]
 
         if self._LU:
             self._LU = None
         return
 
     def __iter__(self):
-        for i in xrange(self.__rows):
-            for j in xrange(self.__cols):
+        for i in range(self.__rows):
+            for j in range(self.__cols):
                 yield self[i,j]
 
     def __mul__(self, other):
         if isinstance(other, self.ctx.matrix):
             # dot multiplication
             if self.__cols != other.__rows:
                 raise ValueError('dimensions not compatible for multiplication')
             new = self.ctx.matrix(self.__rows, other.__cols)
-            self_zero = self.ctx.zero
-            self_get = self.__data.get
-            other_zero = other.ctx.zero
-            other_get = other.__data.get
-            for i in xrange(self.__rows):
-                for j in xrange(other.__cols):
-                    new[i, j] = self.ctx.fdot((self_get((i,k), self_zero), other_get((k,j), other_zero))
-                                     for k in xrange(other.__rows))
+            for i in range(self.__rows):
+                for j in range(other.__cols):
+                    new[i, j] = self.ctx.fdot((self.__data[i,k], other.__data[k,j])
+                                              for k in range(other.__rows) if (i,k) in self.__data and (k,j) in other.__data)
             return new
         else:
             # try scalar multiplication
             new = self.ctx.matrix(self.__rows, self.__cols)
-            for i in xrange(self.__rows):
-                for j in xrange(self.__cols):
+            for i in range(self.__rows):
+                for j in range(self.__cols):
                     new[i, j] = other * self[i, j]
             return new
 
     def __matmul__(self, other):
         return self.__mul__(other)
 
     def __rmul__(self, other):
@@ -631,35 +627,35 @@
             y = self.ctx.inverse(y)
         return y
 
     def __div__(self, other):
         # assume other is scalar and do element-wise divison
         assert not isinstance(other, self.ctx.matrix)
         new = self.ctx.matrix(self.__rows, self.__cols)
-        for i in xrange(self.__rows):
-            for j in xrange(self.__cols):
+        for i in range(self.__rows):
+            for j in range(self.__cols):
                 new[i,j] = self[i,j] / other
         return new
 
     __truediv__ = __div__
 
     def __add__(self, other):
         if isinstance(other, self.ctx.matrix):
             if not (self.__rows == other.__rows and self.__cols == other.__cols):
                 raise ValueError('incompatible dimensions for addition')
             new = self.ctx.matrix(self.__rows, self.__cols)
-            for i in xrange(self.__rows):
-                for j in xrange(self.__cols):
+            for i in range(self.__rows):
+                for j in range(self.__cols):
                     new[i,j] = self[i,j] + other[i,j]
             return new
         else:
             # assume other is scalar and add element-wise
             new = self.ctx.matrix(self.__rows, self.__cols)
-            for i in xrange(self.__rows):
-                for j in xrange(self.__cols):
+            for i in range(self.__rows):
+                for j in range(self.__cols):
                     new[i,j] += self[i,j] + other
             return new
 
     def __radd__(self, other):
         return self.__add__(other)
 
     def __sub__(self, other):
@@ -677,16 +673,19 @@
     def __neg__(self):
         return (-1) * self
 
     def __rsub__(self, other):
         return -self + other
 
     def __eq__(self, other):
-        return self.__rows == other.__rows and self.__cols == other.__cols \
-               and self.__data == other.__data
+        try:
+            return (self.__rows == other.__rows and self.__cols == other.__cols
+                    and self.__data == other.__data)
+        except AttributeError:
+            return NotImplemented
 
     def __len__(self):
         if self.rows == 1:
             return self.cols
         elif self.cols == 1:
             return self.rows
         else:
@@ -712,16 +711,16 @@
                 del self.__data[key]
         self.__cols = value
 
     cols = property(__getcols, __setcols, doc='number of columns')
 
     def transpose(self):
         new = self.ctx.matrix(self.__cols, self.__rows)
-        for i in xrange(self.__rows):
-            for j in xrange(self.__cols):
+        for i in range(self.__rows):
+            for j in range(self.__cols):
                 new[j,i] = self[i,j]
         return new
 
     T = property(transpose)
 
     def conjugate(self):
         return self.apply(self.ctx.conj)
@@ -740,114 +739,111 @@
 
     def column(self, n):
         m = self.ctx.matrix(self.rows, 1)
         for i in range(self.rows):
             m[i] = self[i,n]
         return m
 
-class MatrixMethods(object):
+class MatrixMethods:
 
     def __init__(ctx):
         # XXX: subclass
         ctx.matrix = type('matrix', (_matrix,), {})
         ctx.matrix.ctx = ctx
         ctx.matrix.convert = ctx.convert
 
     def eye(ctx, n, **kwargs):
         """
         Create square identity matrix n x n.
         """
         A = ctx.matrix(n, **kwargs)
-        for i in xrange(n):
+        for i in range(n):
             A[i,i] = 1
         return A
 
     def diag(ctx, diagonal, **kwargs):
         """
         Create square diagonal matrix using given list.
 
         Example:
         >>> from mpmath import diag, mp
-        >>> mp.pretty = False
         >>> diag([1, 2, 3])
         matrix(
         [['1.0', '0.0', '0.0'],
          ['0.0', '2.0', '0.0'],
          ['0.0', '0.0', '3.0']])
         """
         A = ctx.matrix(len(diagonal), **kwargs)
-        for i in xrange(len(diagonal)):
+        for i in range(len(diagonal)):
             A[i,i] = diagonal[i]
         return A
 
     def zeros(ctx, *args, **kwargs):
         """
         Create matrix m x n filled with zeros.
         One given dimension will create square matrix n x n.
 
         Example:
         >>> from mpmath import zeros, mp
-        >>> mp.pretty = False
         >>> zeros(2)
         matrix(
         [['0.0', '0.0'],
          ['0.0', '0.0']])
         """
         if len(args) == 1:
             m = n = args[0]
         elif len(args) == 2:
             m = args[0]
             n = args[1]
         else:
             raise TypeError('zeros expected at most 2 arguments, got %i' % len(args))
         A = ctx.matrix(m, n, **kwargs)
-        for i in xrange(m):
-            for j in xrange(n):
+        for i in range(m):
+            for j in range(n):
                 A[i,j] = 0
         return A
 
     def ones(ctx, *args, **kwargs):
         """
         Create matrix m x n filled with ones.
         One given dimension will create square matrix n x n.
 
         Example:
         >>> from mpmath import ones, mp
-        >>> mp.pretty = False
         >>> ones(2)
         matrix(
         [['1.0', '1.0'],
          ['1.0', '1.0']])
         """
         if len(args) == 1:
             m = n = args[0]
         elif len(args) == 2:
             m = args[0]
             n = args[1]
         else:
             raise TypeError('ones expected at most 2 arguments, got %i' % len(args))
         A = ctx.matrix(m, n, **kwargs)
-        for i in xrange(m):
-            for j in xrange(n):
+        for i in range(m):
+            for j in range(n):
                 A[i,j] = 1
         return A
 
     def hilbert(ctx, m, n=None):
         """
         Create (pseudo) hilbert matrix m x n.
         One given dimension will create hilbert matrix n x n.
 
         The matrix is very ill-conditioned and symmetric, positive definite if
         square.
         """
         if n is None:
             n = m
         A = ctx.matrix(m, n)
-        for i in xrange(m):
-            for j in xrange(n):
+        for i in range(m):
+            for j in range(n):
                 A[i,j] = ctx.one / (i + j + 1)
         return A
 
     def randmatrix(ctx, m, n=None, min=0, max=1, **kwargs):
         """
         Create a random m x n matrix.
 
@@ -860,27 +856,27 @@
         matrix(
         [['0.53491598236191806', '0.57195669543302752'],
          ['0.85589992269513615', '0.82444367501382143']])
         """
         if not n:
             n = m
         A = ctx.matrix(m, n, **kwargs)
-        for i in xrange(m):
-            for j in xrange(n):
+        for i in range(m):
+            for j in range(n):
                 A[i,j] = ctx.rand() * (max - min) + min
         return A
 
     def swap_row(ctx, A, i, j):
         """
         Swap row i with row j.
         """
         if i == j:
             return
         if isinstance(A, ctx.matrix):
-            for k in xrange(A.cols):
+            for k in range(A.cols):
                 A[i,k], A[j,k] = A[j,k], A[i,k]
         elif isinstance(A, list):
             A[i], A[j] = A[j], A[i]
         else:
             raise TypeError('could not interpret type')
 
     def extend(ctx, A, b):
@@ -889,15 +885,15 @@
         """
         if not isinstance(A, ctx.matrix):
             raise TypeError("A should be a type of ctx.matrix")
         if A.rows != len(b):
             raise ValueError("Value should be equal to len(b)")
         A = A.copy()
         A.cols += 1
-        for i in xrange(A.rows):
+        for i in range(A.rows):
             A[i, A.cols-1] = b[i]
         return A
 
     def norm(ctx, x, p=2):
         r"""
         Gives the entrywise `p`-norm of an iterable *x*, i.e. the vector norm
         `\left(\sum_k |x_k|^p\right)^{1/p}`, for any given `1 \le p \le \infty`.
@@ -916,16 +912,15 @@
         For operator matrix norms, use :func:`~mpmath.mnorm` instead.
 
         You can use the string 'inf' as well as float('inf') or mpf('inf')
         to specify the infinity norm.
 
         **Examples**
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import matrix, norm, inf
             >>> x = matrix([-10, 2, 100])
             >>> norm(x, 1)
             mpf('112.0')
             >>> norm(x, 2)
             mpf('100.5186549850325')
             >>> norm(x, inf)
             mpf('100.0')
@@ -972,16 +967,15 @@
         The Frobenius norm lacks some mathematical properties that might
         be expected of a norm.
 
         For general elementwise `p`-norms, use :func:`~mpmath.norm` instead.
 
         **Examples**
 
-            >>> from mpmath import *
-            >>> mp.dps = 15; mp.pretty = False
+            >>> from mpmath import matrix, mnorm, inf
             >>> A = matrix([[1, -1000], [100, 50]])
             >>> mnorm(A, 1)
             mpf('1050.0')
             >>> mnorm(A, inf)
             mpf('1001.0')
             >>> mnorm(A, 'F')
             mpf('1006.2310867787777')
@@ -990,16 +984,12 @@
         A = ctx.matrix(A)
         if type(p) is not int:
             if type(p) is str and 'frobenius'.startswith(p.lower()):
                 return ctx.norm(A, 2)
             p = ctx.convert(p)
         m, n = A.rows, A.cols
         if p == 1:
-            return max(ctx.fsum((A[i,j] for i in xrange(m)), absolute=1) for j in xrange(n))
+            return max(ctx.fsum((A[i,j] for i in range(m)), absolute=1) for j in range(n))
         elif p == ctx.inf:
-            return max(ctx.fsum((A[i,j] for j in xrange(n)), absolute=1) for i in xrange(m))
+            return max(ctx.fsum((A[i,j] for j in range(n)), absolute=1) for i in range(m))
         else:
             raise NotImplementedError("matrix p-norm for arbitrary p")
-
-if __name__ == '__main__':
-    import doctest
-    doctest.testmod()
```

### Comparing `mpmath-1.3.0/mpmath/tests/extratest_gamma.py` & `mpmath-1.4.0a0/mpmath/tests/test_extra_gamma.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,34 @@
-from mpmath import *
-from mpmath.libmp import ifac
-
-import sys
-if "-dps" in sys.argv:
-    maxdps = int(sys.argv[sys.argv.index("-dps")+1])
-else:
-    maxdps = 1000
+import pytest
 
-raise_ = "-raise" in sys.argv
+from mpmath import (agm, eps, exp, factorial, fadd, fsub, gamma, j, log,
+                    loggamma, mp, mpc, mpf, nstr, pi, rgamma, sqrt)
+from mpmath.libmp import ifac
 
-errcount = 0
 
 def check(name, func, z, y):
-    global errcount
-    try:
-        x = func(z)
-    except:
-        errcount += 1
-        if raise_:
-            raise
-        print()
-        print(name)
-        print("EXCEPTION")
-        import traceback
-        traceback.print_tb(sys.exc_info()[2])
-        print()
-        return
+    x = func(z)
     xre = x.real
     xim = x.imag
     yre = y.real
     yim = y.imag
     tol = eps*8
     err = 0
-    if abs(xre-yre) > abs(yre)*tol:
-        err = 1
-        print()
-        print("Error! %s (re = %s, wanted %s, err=%s)" % (name, nstr(xre,10), nstr(yre,10), nstr(abs(xre-yre))))
-        errcount += 1
-        if raise_:
-            raise SystemExit
-    if abs(xim-yim) > abs(yim)*tol:
-        err = 1
-        print()
-        print("Error! %s (im = %s, wanted %s, err=%s)" % (name, nstr(xim,10), nstr(yim,10), nstr(abs(xim-yim))))
-        errcount += 1
-        if raise_:
-            raise SystemExit
-    if not err:
-        sys.stdout.write("%s ok; " % name)
-
-def testcase(case):
-    z, result = case
-    print("Testing z =", z)
-    mp.dps = 1010
-    z = eval(z)
-    mp.dps = maxdps + 50
-    if result is None:
-        gamma_val = gamma(z)
-        loggamma_val = loggamma(z)
-        factorial_val = factorial(z)
-        rgamma_val = rgamma(z)
-    else:
-        loggamma_val = eval(result)
-        gamma_val = exp(loggamma_val)
-        factorial_val = z * gamma_val
-        rgamma_val = 1/gamma_val
-    for dps in [5, 10, 15, 25, 40, 60, 90, 120, 250, 600, 1000, 1800, 3600]:
-        if dps > maxdps:
-            break
-        mp.dps = dps
-        print("dps = %s" % dps)
-        check("gamma", gamma, z, gamma_val)
-        check("rgamma", rgamma, z, rgamma_val)
-        check("loggamma", loggamma, z, loggamma_val)
-        check("factorial", factorial, z, factorial_val)
-        print()
-        mp.dps = 15
+    return abs(xre-yre) <= abs(yre)*tol and abs(xim-yim) <= abs(yim)*tol
 
 testcases = []
 
 # Basic values
 for n in list(range(1,200)) + list(range(201,2000,17)):
     testcases.append(["%s" % n, None])
 for n in range(-200,200):
     testcases.append(["%s+0.5" % n, None])
     testcases.append(["%s+0.37" % n, None])
 
-testcases += [\
+testcases += [
 ["(0.1+1j)", None],
 ["(-0.1+1j)", None],
 ["(0.1-1j)", None],
 ["(-0.1-1j)", None],
 ["10j", None],
 ["-10j", None],
 ["100j", None],
@@ -197,19 +135,29 @@
 for n in [0,1,2,3,4,25,-1,-2,-3,-4,-20,-21,-50,-51,-200,-201,-20000,-20001]:
     for t in ['1e-5', '1e-20', '1e-100', '1e-10000']:
         testcases.append(["fadd(%s,'%s',exact=True)" % (n, t), None])
         testcases.append(["fsub(%s,'%s',exact=True)" % (n, t), None])
         testcases.append(["fadd(%s,'%sj',exact=True)" % (n, t), None])
         testcases.append(["fsub(%s,'%sj',exact=True)" % (n, t), None])
 
-if __name__ == "__main__":
-    from timeit import default_timer as clock
-    tot_time = 0.0
-    for case in testcases:
-        t1 = clock()
-        testcase(case)
-        t2 = clock()
-        print("Test time:", t2-t1)
-        print()
-        tot_time += (t2-t1)
-    print("Total time:", tot_time)
-    print("Errors:", errcount)
+
+@pytest.mark.parametrize("z,result", testcases)
+def test_extra_gamma(z, result):
+    mp.dps = 1010
+    z = eval(z)
+    mp.dps = 1050
+    if result is None:
+        gamma_val = gamma(z)
+        loggamma_val = loggamma(z)
+        factorial_val = factorial(z)
+        rgamma_val = rgamma(z)
+    else:
+        loggamma_val = eval(result)
+        gamma_val = exp(loggamma_val)
+        factorial_val = z * gamma_val
+        rgamma_val = 1/gamma_val
+    for dps in [5, 10, 15, 25, 40, 60, 90, 120, 250, 600, 1000]:
+        mp.dps = dps
+        assert check("gamma", gamma, z, gamma_val)
+        assert check("rgamma", rgamma, z, rgamma_val)
+        assert check("loggamma", loggamma, z, loggamma_val)
+        assert check("factorial", factorial, z, factorial_val)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_bitwise.py` & `mpmath-1.4.0a0/mpmath/tests/test_bitwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 Test bit-level integer and mpf operations
 """
 
-from mpmath import *
-from mpmath.libmp import *
+from mpmath import eps, fadd, ldexp, mp, mpc, mpf
+from mpmath.libmp import (bitcount, fone, from_float, from_man_exp, fzero,
+                          mpf_add, mpf_neg, mpf_perturb, mpf_sub,
+                          round_ceiling, round_down, round_floor,
+                          round_nearest, round_up, to_float, trailing)
+
 
 def test_bitcount():
     assert bitcount(0) == 0
     assert bitcount(1) == 1
     assert bitcount(7) == 3
     assert bitcount(8) == 4
     assert bitcount(2**100) == 101
@@ -131,15 +135,14 @@
     assert mpf_sub(mpf_add(fone, ff(-1e-100)), fone) == ff(-1e-100)
     assert mpf_sub(mpf_add(ff(-1e-100), fone), fone) == ff(-1e-100)
     assert mpf_add(fone, fzero) == fone
     assert mpf_add(fzero, fone) == fone
     assert mpf_add(fzero, fzero) == fzero
 
 def test_long_exponent_shifts():
-    mp.dps = 15
     # Check for possible bugs due to exponent arithmetic overflow
     # in a C implementation
     x = mpf(1)
     for p in [32, 64]:
         a = ldexp(1,2**(p-1))
         b = ldexp(1,2**p)
         c = ldexp(1,2**(p+1))
@@ -181,8 +184,7 @@
         ca = complex(z)
         cb = complex(fadd(z,0,prec=53,rounding='n'))
         assert ca == cb
         for rnd in ['n', 'd', 'u', 'f', 'c']:
             fa = to_float(x._mpf_, rnd=rnd)
             fb = to_float(fadd(x,0,prec=53,rounding=rnd)._mpf_, rnd=rnd)
             assert fa == fb
-    mp.prec = 53
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_calculus.py` & `mpmath-1.4.0a0/mpmath/tests/test_calculus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import pytest
-from mpmath import *
+
+from mpmath import (arange, chebyfit, cos, differint, e, euler, exp, fourier,
+                    fourierval, inf, invertlaplace, j, limit, log, matrix, mp,
+                    mpf, pade, pi, polyroots, polyval, sin, sqrt)
+
 
 def test_approximation():
-    mp.dps = 15
     f = lambda x: cos(2-2*x)/x
     p, err = chebyfit(f, [2, 4], 8, error=True)
     assert err < 1e-5
     for i in range(10):
         x = 2 + i/5.
         assert abs(polyval(p, x) - f(x)) < err
 
 def test_limits():
-    mp.dps = 15
     assert limit(lambda x: (x-sin(x))/x**3, 0).ae(mpf(1)/6)
     assert limit(lambda n: (1+1/n)**n, inf).ae(e)
 
 def test_polyval():
     assert polyval([], 3) == 0
     assert polyval([0], 3) == 0
     assert polyval([5], 3) == 5
@@ -161,34 +163,30 @@
     for i in range(1, N+1):
         k *= i
         a.append(one/k)
     p, q = pade(a, N//2, N//2)
     for x in arange(0, 1, 0.1):
         r = polyval(p[::-1], x)/polyval(q[::-1], x)
         assert(r.ae(exp(x), 1.0e-10))
-    mp.dps = 15
 
 def test_fourier():
-    mp.dps = 15
     c, s = fourier(lambda x: x+1, [-1, 2], 2)
     #plot([lambda x: x+1, lambda x: fourierval((c, s), [-1, 2], x)], [-1, 2])
     assert c[0].ae(1.5)
     assert c[1].ae(-3*sqrt(3)/(2*pi))
     assert c[2].ae(3*sqrt(3)/(4*pi))
     assert s[0] == 0
     assert s[1].ae(3/(2*pi))
     assert s[2].ae(3/(4*pi))
     assert fourierval((c, s), [-1, 2], 1).ae(1.9134966715663442)
 
 def test_differint():
-    mp.dps = 15
     assert differint(lambda t: t, 2, -0.5).ae(8*sqrt(2/pi)/3)
 
 def test_invlap():
-    mp.dps = 15
     t = 0.01
     fp = lambda p: 1/(p+1)**2
     ft = lambda t: t*exp(-t)
     ftt = ft(t)
     assert invertlaplace(fp,t,method='talbot').ae(ftt)
     assert invertlaplace(fp,t,method='stehfest').ae(ftt)
     assert invertlaplace(fp,t,method='dehoog').ae(ftt)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_compatibility.py` & `mpmath-1.4.0a0/mpmath/tests/test_compatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from mpmath import *
-from random import seed, randint, random
 import math
+from random import randint, random, seed
+
+from mpmath import ceil, floor, mp, mpf
+
 
 # Test compatibility with Python floats, which are
 # IEEE doubles (53-bit)
 
 N = 5000
 seed(1)
 
@@ -18,15 +20,14 @@
 
 # Detect whether Python is compiled to use 80-bit floating-point
 # instructions, in which case the double compatibility test breaks
 uses_x87 = -4.1974624032366689e+117 / -8.4657370748010221e-47 \
     == 4.9581771393902231e+163
 
 def test_double_compatibility():
-    mp.prec = 53
     for x, y in zip(xs, ys):
         mpx = mpf(x)
         mpy = mpf(y)
         assert mpf(x) == x
         assert (mpx < mpy) == (x < y)
         assert (mpx > mpy) == (x > y)
         assert (mpx == mpy) == (x == y)
@@ -55,15 +56,14 @@
         assert ceil(mpx) == math.ceil(x)
         assert floor(mpx) == math.floor(x)
 
 def test_sqrt():
     # this fails quite often. it appers to be float
     # that rounds the wrong way, not mpf
     fail = 0
-    mp.prec = 53
     for x in xs:
         x = abs(x)
         mp.prec = 100
         mp_high = mpf(x)**0.5
         mp.prec = 53
         mp_low = mpf(x)**0.5
         fp = x**0.5
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_convert.py` & `mpmath-1.4.0a0/mpmath/tests/test_convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+import decimal
 import random
-from mpmath import *
-from mpmath.libmp import *
+from decimal import Decimal
+from fractions import Fraction
+
+import pytest
+
+from mpmath import iv, mp, mpc, mpf, mpi, mpmathify, sqrt
+from mpmath.libmp import (fhalf, from_float, from_rational, from_str,
+                          round_ceiling, round_floor, round_nearest,
+                          to_rational, to_str)
 
 
 def test_basic_string():
     """
     Test basic string conversion
     """
-    mp.dps = 15
     assert mpf('3') == mpf('3.0') == mpf('0003.') == mpf('0.03e2') == mpf(3.0)
     assert mpf('30') == mpf('30.0') == mpf('00030.') == mpf(30.0)
     for i in range(10):
         for j in range(10):
             assert mpf('%ie%i' % (i,j)) == i * 10**j
     assert str(mpf('25000.0')) == '25000.0'
     assert str(mpf('2500.0')) == '2500.0'
@@ -30,36 +37,48 @@
     assert str(mpf(-1.23402834e-15)) == '-1.23402834e-15'
     assert str(mpf(-1.2344e-15)) == '-1.2344e-15'
     assert repr(mpf(-1.2344e-15)) == "mpf('-1.2343999999999999e-15')"
     assert str(mpf("2163048125L")) == '2163048125.0'
     assert str(mpf("-2163048125l")) == '-2163048125.0'
     assert str(mpf("-2163048125L/1088391168")) == '-1.98738118113799'
     assert str(mpf("2163048125/1088391168l")) == '1.98738118113799'
+    assert str(mpf('inf')) == '+inf'
+
+    # issue 613
+    assert str(mpf('2_5_0_0.0')) == '2500.0'
+    # issue 377
+    assert to_str(from_str('1_234.567891', 80), 24) == '1234.567891'
+    assert to_str(from_str('1_234.567_891', 80), 24) == '1234.567891'
+    assert to_str(from_str('1_234.567_8_9_1', 80), 24) == '1234.567891'
+    assert to_str(from_str('1.0_0', 80), 24) == '1.0'
+    assert to_str(from_str('.000', 80), 24) == '0.0'
+
+def test_from_str():
+    assert mpf(from_str('ABC.ABC', base=16)) == mpf(float.fromhex('ABC.ABC'))
+    assert mpf(from_str('0xABC.ABC')) == mpf(float.fromhex('ABC.ABC'))
+    assert mpf(from_str('0x3.a7p10')) == mpf(float.fromhex('0x3.a7p10'))
+    assert mpf(from_str('0x1.4ace478p+33')) == mpf(float.fromhex('0x1.4ace478p+33'))
+    assert mpf(from_str('0x1.4ace478@+33')) == mpf('7.0354608312666732e+39')
+    assert mpf(from_str('0b1101.100101')) == mpf('13.578125')
+    assert mpf(from_str('0o1101.100101')) == mpf('577.12524795532227')
+
+def test_eps_repr():
+    mp.dps = 24
+    assert repr(mp.eps) == '<epsilon of working precision: 2.06795e-25~>'
 
 def test_pretty():
     mp.pretty = True
     assert repr(mpf(2.5)) == '2.5'
     assert repr(mpc(2.5,3.5)) == '(2.5 + 3.5j)'
-    mp.pretty = False
     iv.pretty = True
     assert repr(mpi(2.5,3.5)) == '[2.5, 3.5]'
-    iv.pretty = False
 
 def test_str_whitespace():
     assert mpf('1.26 ') == 1.26
 
-def test_unicode():
-    mp.dps = 15
-    try:
-        unicode = unicode
-    except NameError:
-        unicode = str
-    assert mpf(unicode('2.76')) == 2.76
-    assert mpf(unicode('inf')) == inf
-
 def test_str_format():
     assert to_str(from_float(0.1),15,strip_zeros=False) == '0.100000000000000'
     assert to_str(from_float(0.0),15,show_zero_exponent=True) == '0.0e+0'
     assert to_str(from_float(0.0),0,show_zero_exponent=True) == '.0e+0'
     assert to_str(from_float(0.0),0,show_zero_exponent=False) == '.0'
     assert to_str(from_float(0.0),1,show_zero_exponent=True) == '0.0e+0'
     assert to_str(from_float(0.0),1,show_zero_exponent=False) == '0.0'
@@ -68,48 +87,48 @@
     assert to_str(from_float(1.23456789000000e+2),15,strip_zeros=False,min_fixed=0,max_fixed=0) == '1.23456789000000e+2'
     assert to_str(from_float(2.1287e14), 15, max_fixed=1000) == '212870000000000.0'
     assert to_str(from_float(2.1287e15), 15, max_fixed=1000) == '2128700000000000.0'
     assert to_str(from_float(2.1287e16), 15, max_fixed=1000) == '21287000000000000.0'
     assert to_str(from_float(2.1287e30), 15, max_fixed=1000) == '2128700000000000000000000000000.0'
 
 def test_tight_string_conversion():
-    mp.dps = 15
     # In an old version, '0.5' wasn't recognized as representing
     # an exact binary number and was erroneously rounded up or down
     assert from_str('0.5', 10, round_floor) == fhalf
     assert from_str('0.5', 10, round_ceiling) == fhalf
 
 def test_eval_repr_invariant():
     """Test that eval(repr(x)) == x"""
     random.seed(123)
     for dps in [10, 15, 20, 50, 100]:
         mp.dps = dps
         for i in range(1000):
             a = mpf(random.random())**0.5 * 10**random.randint(-100, 100)
             assert eval(repr(a)) == a
-    mp.dps = 15
 
 def test_str_bugs():
-    mp.dps = 15
     # Decimal rounding used to give the wrong exponent in some cases
     assert str(mpf('1e600')) == '1.0e+600'
     assert str(mpf('1e10000')) == '1.0e+10000'
 
 def test_str_prec0():
     assert to_str(from_float(1.234), 0) == '.0e+0'
     assert to_str(from_float(1e-15), 0) == '.0e-15'
     assert to_str(from_float(1e+15), 0) == '.0e+15'
     assert to_str(from_float(-1e-15), 0) == '-.0e-15'
     assert to_str(from_float(-1e+15), 0) == '-.0e+15'
 
 def test_convert_rational():
-    mp.dps = 15
     assert from_rational(30, 5, 53, round_nearest) == (0, 3, 1, 2)
     assert from_rational(-7, 4, 53, round_nearest) == (1, 7, -2, 3)
     assert to_rational((0, 1, -1, 1)) == (1, 2)
+    assert to_rational((0, 1, 0, 1)) == (1, 1)
+    pytest.raises(ValueError, lambda: to_rational(mpf('nan')._mpf_))
+    pytest.raises(OverflowError, lambda: to_rational(mpf('inf')._mpf_))
+    pytest.raises(OverflowError, lambda: to_rational(mpf('-inf')._mpf_))
 
 def test_custom_class():
     class mympf:
         @property
         def _mpf_(self):
             return mpf(3.5)._mpf_
     class mympc:
@@ -118,14 +137,16 @@
             return mpf(3.5)._mpf_, mpf(2.5)._mpf_
     assert mpf(2) + mympf() == 5.5
     assert mympf() + mpf(2) == 5.5
     assert mpf(mympf()) == 3.5
     assert mympc() + mpc(2) == mpc(5.5, 2.5)
     assert mpc(2) + mympc() == mpc(5.5, 2.5)
     assert mpc(mympc()) == (3.5+2.5j)
+    assert mpmathify(mympf()) == mpf(3.5)
+    assert mpmathify(mympc()) == mpc(3.5, 2.5)
 
 def test_conversion_methods():
     class SomethingRandom:
         pass
     class SomethingReal:
         def _mpmath_(self, prec, rounding):
             return mp.make_mpf(from_str('1.3', prec, rounding))
@@ -158,37 +179,34 @@
     assert x.__radd__(a) is NotImplemented
     assert x.__lt__(a) is NotImplemented
     assert x.__gt__(a) is NotImplemented
     assert x.__le__(a) is NotImplemented
     assert x.__ge__(a) is NotImplemented
     assert x.__eq__(a) is NotImplemented
     assert x.__ne__(a) is NotImplemented
-    # implementation detail
-    if hasattr(x, "__cmp__"):
-        assert x.__cmp__(a) is NotImplemented
     assert x.__sub__(a) is NotImplemented
     assert x.__rsub__(a) is NotImplemented
     assert x.__mul__(a) is NotImplemented
     assert x.__rmul__(a) is NotImplemented
-    assert x.__div__(a) is NotImplemented
-    assert x.__rdiv__(a) is NotImplemented
+    assert x.__truediv__(a) is NotImplemented
+    assert x.__rtruediv__(a) is NotImplemented
     assert x.__mod__(a) is NotImplemented
     assert x.__rmod__(a) is NotImplemented
     assert x.__pow__(a) is NotImplemented
     assert x.__rpow__(a) is NotImplemented
     assert z.__add__(a) is NotImplemented
     assert z.__radd__(a) is NotImplemented
     assert z.__eq__(a) is NotImplemented
     assert z.__ne__(a) is NotImplemented
     assert z.__sub__(a) is NotImplemented
     assert z.__rsub__(a) is NotImplemented
     assert z.__mul__(a) is NotImplemented
     assert z.__rmul__(a) is NotImplemented
-    assert z.__div__(a) is NotImplemented
-    assert z.__rdiv__(a) is NotImplemented
+    assert z.__truediv__(a) is NotImplemented
+    assert z.__rtruediv__(a) is NotImplemented
     assert z.__pow__(a) is NotImplemented
     assert z.__rpow__(a) is NotImplemented
 
 def test_mpmathify():
     assert mpmathify('1/2') == 0.5
     assert mpmathify('(1.0+1.0j)') == mpc(1, 1)
     assert mpmathify('(1.2e-10 - 3.4e5j)') == mpc('1.2e-10', '-3.4e5')
@@ -201,33 +219,34 @@
         mpmathify('(' + '1' * 5000 + '!j')
     except:
         return
     # The expression is invalid and should raise an exception.
     assert False
 
 def test_compatibility():
-    try:
-        import numpy as np
-        from fractions import Fraction
-        from decimal import Decimal
-        import decimal
-    except ImportError:
-        return
+    np = pytest.importorskip("numpy")
     # numpy types
     for nptype in np.core.numerictypes.typeDict.values():
         if issubclass(nptype, np.complexfloating):
             x = nptype(complex(0.5, -0.5))
         elif issubclass(nptype, np.floating):
             x = nptype(0.5)
         elif issubclass(nptype, np.integer):
             x = nptype(2)
         # Handle the weird types
         try: diff = np.abs(type(np.sqrt(x))(sqrt(x)) - np.sqrt(x))
         except: continue
         assert diff < 2.0**-53
+    # issues 382 and 539
+    assert mp.sqrt(np.int64(1)) == mpf('1.0')
+    assert mpf(np.int64(1)) == mpf('1.0')
     #Fraction and Decimal
     oldprec = mp.prec
     mp.prec = 1000
     decimal.getcontext().prec = mp.dps
     assert sqrt(Fraction(2, 3)).ae(sqrt(mpf('2/3')))
     assert sqrt(Decimal(2)/Decimal(3)).ae(sqrt(mpf('2/3')))
     mp.prec = oldprec
+    pytest.raises(TypeError, lambda: mpmathify(np.array(1)))
+
+def test_issue465():
+    assert mpf(Fraction(1, 3)) == mpf('0.33333333333333331')
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_diff.py` & `mpmath-1.4.0a0/mpmath/tests/test_diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from mpmath import *
+from mpmath import (chop, cos, diff, diffs, diffun, e, exp, j, log, sin, sqrt,
+                    taylor)
+
 
 def test_diff():
-    mp.dps = 15
     assert diff(log, 2.0, n=0).ae(log(2))
     assert diff(cos, 1.0).ae(-sin(1))
     assert diff(abs, 0.0) == 0
     assert diff(abs, 0.0, direction=1) == 1
     assert diff(abs, 0.0, direction=-1) == -1
     assert diff(exp, 1.0).ae(e)
     assert diff(exp, 1.0, n=5).ae(e)
@@ -13,27 +14,24 @@
     assert diff(lambda x: x**2, 3.0, method='quad').ae(6)
     assert diff(lambda x: 3+x**5, 3.0, n=2, method='quad').ae(540)
     assert diff(lambda x: 3+x**5, 3.0, n=2, method='step').ae(540)
     assert diffun(sin)(2).ae(cos(2))
     assert diffun(sin, n=2)(2).ae(-sin(2))
 
 def test_diffs():
-    mp.dps = 15
     assert [chop(d) for d in diffs(sin, 0, 1)] == [0, 1]
     assert [chop(d) for d in diffs(sin, 0, 1, method='quad')] == [0, 1]
     assert [chop(d) for d in diffs(sin, 0, 2)] == [0, 1, 0]
     assert [chop(d) for d in diffs(sin, 0, 2, method='quad')] == [0, 1, 0]
 
 def test_taylor():
-    mp.dps = 15
     # Easy to test since the coefficients are exact in floating-point
     assert taylor(sqrt, 1, 4) == [1, 0.5, -0.125, 0.0625, -0.0390625]
 
 def test_diff_partial():
-    mp.dps = 15
     x,y,z = xyz = 2,3,7
     f = lambda x,y,z: 3*x**2 * (y+2)**3 * z**5
     assert diff(f, xyz, (0,0,0)).ae(25210500)
     assert diff(f, xyz, (0,0,1)).ae(18007500)
     assert diff(f, xyz, (0,0,2)).ae(10290000)
     assert diff(f, xyz, (0,1,0)).ae(15126300)
     assert diff(f, xyz, (0,1,1)).ae(10804500)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_division.py` & `mpmath-1.4.0a0/mpmath/tests/test_division.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,138 @@
-from mpmath.libmp import *
-from mpmath import mpf, mp
+from random import choice, randint, seed
 
-from random import randint, choice, seed
-
-all_modes = [round_floor, round_ceiling, round_down, round_up, round_nearest]
-
-fb = from_bstr
-fi = from_int
-ff = from_float
+from mpmath import mpf
+from mpmath.libmp import (from_int, from_str, mpf_div, mpf_mul, mpf_rdiv_int,
+                          round_ceiling, round_down, round_floor,
+                          round_nearest, round_up, trailing)
 
 
 def test_div_1_3():
-    a = fi(1)
-    b = fi(3)
-    c = fi(-1)
+    a = from_int(1)
+    b = from_int(3)
+    c = from_int(-1)
 
     # floor rounds down, ceiling rounds up
-    assert mpf_div(a, b, 7, round_floor)   == fb('0.01010101')
-    assert mpf_div(a, b, 7, round_ceiling) == fb('0.01010110')
-    assert mpf_div(a, b, 7, round_down)    == fb('0.01010101')
-    assert mpf_div(a, b, 7, round_up)      == fb('0.01010110')
-    assert mpf_div(a, b, 7, round_nearest) == fb('0.01010101')
+    assert mpf_div(a, b, 7, round_floor)   == from_str('0.01010101', base=2)
+    assert mpf_div(a, b, 7, round_ceiling) == from_str('0.01010110', base=2)
+    assert mpf_div(a, b, 7, round_down)    == from_str('0.01010101', base=2)
+    assert mpf_div(a, b, 7, round_up)      == from_str('0.01010110', base=2)
+    assert mpf_div(a, b, 7, round_nearest) == from_str('0.01010101', base=2)
 
     # floor rounds up, ceiling rounds down
-    assert mpf_div(c, b, 7, round_floor)   == fb('-0.01010110')
-    assert mpf_div(c, b, 7, round_ceiling) == fb('-0.01010101')
-    assert mpf_div(c, b, 7, round_down)    == fb('-0.01010101')
-    assert mpf_div(c, b, 7, round_up)      == fb('-0.01010110')
-    assert mpf_div(c, b, 7, round_nearest) == fb('-0.01010101')
+    assert mpf_div(c, b, 7, round_floor)   == from_str('-0.01010110', base=2)
+    assert mpf_div(c, b, 7, round_ceiling) == from_str('-0.01010101', base=2)
+    assert mpf_div(c, b, 7, round_down)    == from_str('-0.01010101', base=2)
+    assert mpf_div(c, b, 7, round_up)      == from_str('-0.01010110', base=2)
+    assert mpf_div(c, b, 7, round_nearest) == from_str('-0.01010101', base=2)
 
 def test_mpf_divi_1_3():
     a = 1
-    b = fi(3)
+    b = from_int(3)
     c = -1
-    assert mpf_rdiv_int(a, b, 7, round_floor)   == fb('0.01010101')
-    assert mpf_rdiv_int(a, b, 7, round_ceiling) == fb('0.01010110')
-    assert mpf_rdiv_int(a, b, 7, round_down)    == fb('0.01010101')
-    assert mpf_rdiv_int(a, b, 7, round_up)      == fb('0.01010110')
-    assert mpf_rdiv_int(a, b, 7, round_nearest) == fb('0.01010101')
-    assert mpf_rdiv_int(c, b, 7, round_floor)   == fb('-0.01010110')
-    assert mpf_rdiv_int(c, b, 7, round_ceiling) == fb('-0.01010101')
-    assert mpf_rdiv_int(c, b, 7, round_down)    == fb('-0.01010101')
-    assert mpf_rdiv_int(c, b, 7, round_up)      == fb('-0.01010110')
-    assert mpf_rdiv_int(c, b, 7, round_nearest) == fb('-0.01010101')
+    assert mpf_rdiv_int(a, b, 7, round_floor)   == from_str('0.01010101', base=2)
+    assert mpf_rdiv_int(a, b, 7, round_ceiling) == from_str('0.01010110', base=2)
+    assert mpf_rdiv_int(a, b, 7, round_down)    == from_str('0.01010101', base=2)
+    assert mpf_rdiv_int(a, b, 7, round_up)      == from_str('0.01010110', base=2)
+    assert mpf_rdiv_int(a, b, 7, round_nearest) == from_str('0.01010101', base=2)
+    assert mpf_rdiv_int(c, b, 7, round_floor)   == from_str('-0.01010110', base=2)
+    assert mpf_rdiv_int(c, b, 7, round_ceiling) == from_str('-0.01010101', base=2)
+    assert mpf_rdiv_int(c, b, 7, round_down)    == from_str('-0.01010101', base=2)
+    assert mpf_rdiv_int(c, b, 7, round_up)      == from_str('-0.01010110', base=2)
+    assert mpf_rdiv_int(c, b, 7, round_nearest) == from_str('-0.01010101', base=2)
 
 
 def test_div_300():
 
-    q = fi(1000000)
-    a = fi(300499999)    # a/q is a little less than a half-integer
-    b = fi(300500000)    # b/q exactly a half-integer
-    c = fi(300500001)    # c/q is a little more than a half-integer
+    q = from_int(1000000)
+    a = from_int(300499999)    # a/q is a little less than a half-integer
+    b = from_int(300500000)    # b/q exactly a half-integer
+    c = from_int(300500001)    # c/q is a little more than a half-integer
 
     # Check nearest integer rounding (prec=9 as 2**8 < 300 < 2**9)
 
-    assert mpf_div(a, q, 9, round_down) == fi(300)
-    assert mpf_div(b, q, 9, round_down) == fi(300)
-    assert mpf_div(c, q, 9, round_down) == fi(300)
-    assert mpf_div(a, q, 9, round_up) == fi(301)
-    assert mpf_div(b, q, 9, round_up) == fi(301)
-    assert mpf_div(c, q, 9, round_up) == fi(301)
+    assert mpf_div(a, q, 9, round_down) == from_int(300)
+    assert mpf_div(b, q, 9, round_down) == from_int(300)
+    assert mpf_div(c, q, 9, round_down) == from_int(300)
+    assert mpf_div(a, q, 9, round_up) == from_int(301)
+    assert mpf_div(b, q, 9, round_up) == from_int(301)
+    assert mpf_div(c, q, 9, round_up) == from_int(301)
 
     # Nearest even integer is down
-    assert mpf_div(a, q, 9, round_nearest) == fi(300)
-    assert mpf_div(b, q, 9, round_nearest) == fi(300)
-    assert mpf_div(c, q, 9, round_nearest) == fi(301)
+    assert mpf_div(a, q, 9, round_nearest) == from_int(300)
+    assert mpf_div(b, q, 9, round_nearest) == from_int(300)
+    assert mpf_div(c, q, 9, round_nearest) == from_int(301)
 
     # Nearest even integer is up
-    a = fi(301499999)
-    b = fi(301500000)
-    c = fi(301500001)
-    assert mpf_div(a, q, 9, round_nearest) == fi(301)
-    assert mpf_div(b, q, 9, round_nearest) == fi(302)
-    assert mpf_div(c, q, 9, round_nearest) == fi(302)
+    a = from_int(301499999)
+    b = from_int(301500000)
+    c = from_int(301500001)
+    assert mpf_div(a, q, 9, round_nearest) == from_int(301)
+    assert mpf_div(b, q, 9, round_nearest) == from_int(302)
+    assert mpf_div(c, q, 9, round_nearest) == from_int(302)
 
 
 def test_tight_integer_division():
     # Test that integer division at tightest possible precision is exact
     N = 100
     seed(1)
     for i in range(N):
         a = choice([1, -1]) * randint(1, 1<<randint(10, 100))
         b = choice([1, -1]) * randint(1, 1<<randint(10, 100))
         p = a * b
-        width = bitcount(abs(b)) - trailing(b)
-        a = fi(a); b = fi(b); p = fi(p)
-        for mode in all_modes:
+        width = b.bit_length() - trailing(b)
+        a = from_int(a); b = from_int(b); p = from_int(p)
+        for mode in [round_floor, round_ceiling, round_down,
+                     round_up, round_nearest]:
             assert mpf_div(p, a, width, mode) == b
 
 
 def test_epsilon_rounding():
     # Verify that mpf_div uses infinite precision; this result will
     # appear to be exactly 0.101 to a near-sighted algorithm
 
-    a = fb('0.101' + ('0'*200) + '1')
-    b = fb('1.10101')
+    a = from_str('0.101' + ('0'*200) + '1', base=2)
+    b = from_str('1.10101', base=2)
     c = mpf_mul(a, b, 250, round_floor) # exact
-    assert mpf_div(c, b, bitcount(a[1]), round_floor) == a # exact
+    assert mpf_div(c, b, a[1].bit_length(), round_floor) == a # exact
 
-    assert mpf_div(c, b, 2, round_down) == fb('0.10')
-    assert mpf_div(c, b, 3, round_down) == fb('0.101')
-    assert mpf_div(c, b, 2, round_up) == fb('0.11')
-    assert mpf_div(c, b, 3, round_up) == fb('0.110')
-    assert mpf_div(c, b, 2, round_floor) == fb('0.10')
-    assert mpf_div(c, b, 3, round_floor) == fb('0.101')
-    assert mpf_div(c, b, 2, round_ceiling) == fb('0.11')
-    assert mpf_div(c, b, 3, round_ceiling) == fb('0.110')
+    assert mpf_div(c, b, 2, round_down) == from_str('0.10', base=2)
+    assert mpf_div(c, b, 3, round_down) == from_str('0.101', base=2)
+    assert mpf_div(c, b, 2, round_up) == from_str('0.11', base=2)
+    assert mpf_div(c, b, 3, round_up) == from_str('0.110', base=2)
+    assert mpf_div(c, b, 2, round_floor) == from_str('0.10', base=2)
+    assert mpf_div(c, b, 3, round_floor) == from_str('0.101', base=2)
+    assert mpf_div(c, b, 2, round_ceiling) == from_str('0.11', base=2)
+    assert mpf_div(c, b, 3, round_ceiling) == from_str('0.110', base=2)
 
     # The same for negative numbers
-    a = fb('-0.101' + ('0'*200) + '1')
-    b = fb('1.10101')
+    a = from_str('-0.101' + ('0'*200) + '1', base=2)
+    b = from_str('1.10101', base=2)
     c = mpf_mul(a, b, 250, round_floor)
-    assert mpf_div(c, b, bitcount(a[1]), round_floor) == a
+    assert mpf_div(c, b, a[1].bit_length(), round_floor) == a
 
-    assert mpf_div(c, b, 2, round_down) == fb('-0.10')
-    assert mpf_div(c, b, 3, round_up) == fb('-0.110')
+    assert mpf_div(c, b, 2, round_down) == from_str('-0.10', base=2)
+    assert mpf_div(c, b, 3, round_up) == from_str('-0.110', base=2)
 
     # Floor goes up, ceiling goes down
-    assert mpf_div(c, b, 2, round_floor) == fb('-0.11')
-    assert mpf_div(c, b, 3, round_floor) == fb('-0.110')
-    assert mpf_div(c, b, 2, round_ceiling) == fb('-0.10')
-    assert mpf_div(c, b, 3, round_ceiling) == fb('-0.101')
+    assert mpf_div(c, b, 2, round_floor) == from_str('-0.11', base=2)
+    assert mpf_div(c, b, 3, round_floor) == from_str('-0.110', base=2)
+    assert mpf_div(c, b, 2, round_ceiling) == from_str('-0.10', base=2)
+    assert mpf_div(c, b, 3, round_ceiling) == from_str('-0.101', base=2)
 
 
 def test_mod():
-    mp.dps = 15
     assert mpf(234) % 1 == 0
     assert mpf(-3) % 256 == 253
     assert mpf(0.25) % 23490.5 == 0.25
     assert mpf(0.25) % -23490.5 == -23490.25
     assert mpf(-0.25) % 23490.5 == 23490.25
     assert mpf(-0.25) % -23490.5 == -0.25
     # Check that these cases are handled efficiently
     assert mpf('1e10000000000') % 1 == 0
     assert mpf('1.23e-1000000000') % 1 == mpf('1.23e-1000000000')
     # test __rmod__
     assert 3 % mpf('1.75') == 1.25
 
 def test_div_negative_rnd_bug():
-    mp.dps = 15
     assert (-3) / mpf('0.1531879017645047') == mpf('-19.583791966887116')
     assert mpf('-2.6342475750861301') / mpf('0.35126216427941814') == mpf('-7.4993775104985909')
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_eigen.py` & `mpmath-1.4.0a0/mpmath/tests/test_eigen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 from mpmath import mp
-from mpmath import libmp
 
-xrange = libmp.backend.xrange
 
 def run_hessenberg(A, verbose = 0):
     if verbose > 1:
         print("original matrix (hessenberg):\n", A)
 
     n = A.rows
 
@@ -19,22 +14,22 @@
         print("H:\n",H)
 
     B = Q * H * Q.transpose_conj()
 
     eps = mp.exp(0.8 * mp.log(mp.eps))
 
     err0 = 0
-    for x in xrange(n):
-        for y in xrange(n):
+    for x in range(n):
+        for y in range(n):
             err0 += abs(A[y,x] - B[y,x])
     err0 /= n * n
 
     err1 = 0
-    for x in xrange(n):
-        for y in xrange(x + 2, n):
+    for x in range(n):
+        for y in range(x + 2, n):
             err1 += abs(H[y,x])
 
     if verbose > 0:
         print("difference (H):", err0, err1)
 
     if verbose > 1:
         print("B:\n", B)
@@ -57,30 +52,30 @@
 
     B = Q * R * Q.transpose_conj()
     C = Q * Q.transpose_conj()
 
     eps = mp.exp(0.8 * mp.log(mp.eps))
 
     err0 = 0
-    for x in xrange(n):
-        for y in xrange(n):
+    for x in range(n):
+        for y in range(n):
             err0 += abs(A[y,x] - B[y,x])
     err0 /= n * n
 
     err1 = 0
-    for x in xrange(n):
-        for y in xrange(n):
+    for x in range(n):
+        for y in range(n):
             if x == y:
                 C[y,x] -= 1
             err1 += abs(C[y,x])
     err1 /= n * n
 
     err2 = 0
-    for x in xrange(n):
-        for y in xrange(x + 1, n):
+    for x in range(n):
+        for y in range(x + 1, n):
             err2 += abs(R[y,x])
 
     if verbose > 0:
         print("difference (S):", err0, err1, err2)
 
     if verbose > 1:
         print("B:\n", B)
@@ -101,15 +96,15 @@
         print("E:\n", E)
         print("EL:\n", EL)
         print("ER:\n", ER)
 
     eps = mp.exp(0.8 * mp.log(mp.eps))
 
     err0 = 0
-    for i in xrange(n):
+    for i in range(n):
         B = A * ER[:,i] - E[i] * ER[:,i]
         err0 = max(err0, mp.mnorm(B))
 
         B = EL[i,:] * A - EL[i,:] * E[i]
         err0 = max(err0, mp.mnorm(B))
 
     err0 /= n * n
@@ -119,30 +114,30 @@
 
     assert err0 < eps
 
 #####################
 
 def test_eig_dyn():
     v = 0
-    for i in xrange(5):
+    for i in range(5):
         n = 1 + int(mp.rand() * 5)
         if mp.rand() > 0.5:
             # real
             A = 2 * mp.randmatrix(n, n) - 1
             if mp.rand() > 0.5:
                 A *= 10
-                for x in xrange(n):
-                    for y in xrange(n):
+                for x in range(n):
+                    for y in range(n):
                         A[x,y] = int(A[x,y])
         else:
             A = (2 * mp.randmatrix(n, n) - 1) + 1j * (2 * mp.randmatrix(n, n) - 1)
             if mp.rand() > 0.5:
                 A *= 10
-                for x in xrange(n):
-                    for y in xrange(n):
+                for x in range(n):
+                    for y in range(n):
                         A[x,y] = int(mp.re(A[x,y])) + 1j * int(mp.im(A[x,y]))
 
         run_hessenberg(A, verbose = v)
         run_schur(A, verbose = v)
         run_eig(A, verbose = v)
 
 def test_eig():
@@ -173,7 +168,10 @@
     AS.append(A)
     AS.append(A.transpose())
 
     for A in AS:
         run_hessenberg(A, verbose = v)
         run_schur(A, verbose = v)
         run_eig(A, verbose = v)
+
+    A = mp.matrix(1)
+    assert mp.eig(A, left=False, right=False) == [0]
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_eigen_symmetric.py` & `mpmath-1.4.0a0/mpmath/tests/test_eigen_symmetric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 from mpmath import mp
-from mpmath import libmp
 
-xrange = libmp.backend.xrange
 
 def run_eigsy(A, verbose = False):
     if verbose:
         print("original matrix:\n", str(A))
 
     D, Q = mp.eigsy(A)
     B = Q * mp.diag(D) * Q.transpose()
@@ -69,15 +64,15 @@
     if verbose:
         print("original matrix:\n", str(A))
         print("full", full_matrices)
 
     U, S0, V = mp.svd_r(A, full_matrices = full_matrices)
 
     S = mp.zeros(U.cols, V.rows)
-    for j in xrange(min(m, n)):
+    for j in range(min(m, n)):
         S[j,j] = S0[j]
 
     if verbose:
         print("U:\n", str(U))
         print("S:\n", str(S0))
         print("V:\n", str(V))
 
@@ -108,15 +103,15 @@
     if verbose:
         print("original matrix:\n", str(A))
         print("full", full_matrices)
 
     U, S0, V = mp.svd_c(A, full_matrices = full_matrices)
 
     S = mp.zeros(U.cols, V.rows)
-    for j in xrange(min(m, n)):
+    for j in range(min(m, n)):
         S[j,j] = S0[j]
 
     if verbose:
         print("U:\n", str(U))
         print("S:\n", str(S0))
         print("V:\n", str(V))
 
@@ -144,22 +139,22 @@
     d, e = mp.gauss_quadrature(len(a), qtype)
     d -= mp.matrix(a)
     e -= mp.matrix(b)
 
     assert mp.mnorm(d) < eps
     assert mp.mnorm(e) < eps
 
-def irandmatrix(n, range = 10):
+def irandmatrix(n, r=10):
     """
     random matrix with integer entries
     """
     A = mp.matrix(n, n)
-    for i in xrange(n):
-        for j in xrange(n):
-            A[i,j]=int( (2 * mp.rand() - 1) * range)
+    for i in range(n):
+        for j in range(n):
+            A[i,j] = int((2 * mp.rand() - 1) * r)
     return A
 
 #######################
 
 def test_eighe_fixed_matrix():
     A = mp.matrix([[2, 3], [3, 5]])
     run_eigsy(A)
@@ -187,87 +182,87 @@
 
     A = mp.matrix([[2, 11 + 17j, 7 + 19j], [11 - 17j, 3, -13 + 23j], [7 - 19j, -13 - 23j, 5]])
     run_eighe(A)
 
 def test_eigsy_randmatrix():
     N = 5
 
-    for a in xrange(10):
+    for a in range(10):
         A = 2 * mp.randmatrix(N, N) - 1
 
-        for i in xrange(0, N):
-            for j in xrange(i + 1, N):
+        for i in range(0, N):
+            for j in range(i + 1, N):
                 A[j,i] = A[i,j]
 
         run_eigsy(A)
 
 def test_eighe_randmatrix():
     N = 5
 
-    for a in xrange(10):
+    for a in range(10):
         A = (2 * mp.randmatrix(N, N) - 1) + 1j * (2 * mp.randmatrix(N, N) - 1)
 
-        for i in xrange(0, N):
+        for i in range(0, N):
             A[i,i] = mp.re(A[i,i])
-            for j in xrange(i + 1, N):
+            for j in range(i + 1, N):
                 A[j,i] = mp.conj(A[i,j])
 
         run_eighe(A)
 
 def test_eigsy_irandmatrix():
     N = 4
     R = 4
 
-    for a in xrange(10):
+    for a in range(10):
         A=irandmatrix(N, R)
 
-        for i in xrange(0, N):
-            for j in xrange(i + 1, N):
+        for i in range(0, N):
+            for j in range(i + 1, N):
                 A[j,i] = A[i,j]
 
         run_eigsy(A)
 
 def test_eighe_irandmatrix():
     N = 4
     R = 4
 
-    for a in xrange(10):
+    for a in range(10):
         A=irandmatrix(N, R) + 1j * irandmatrix(N, R)
 
-        for i in xrange(0, N):
+        for i in range(0, N):
             A[i,i] = mp.re(A[i,i])
-            for j in xrange(i + 1, N):
+            for j in range(i + 1, N):
                 A[j,i] = mp.conj(A[i,j])
 
         run_eighe(A)
 
 def test_svd_r_rand():
-    for i in xrange(5):
+    for i in range(5):
         full = mp.rand() > 0.5
         m = 1 + int(mp.rand() * 10)
         n = 1 + int(mp.rand() * 10)
         A = 2 * mp.randmatrix(m, n) - 1
         if mp.rand() > 0.5:
             A *= 10
-            for x in xrange(m):
-                for y in xrange(n):
+            for x in range(m):
+                for y in range(n):
                     A[x,y]=int(A[x,y])
 
         run_svd_r(A, full_matrices = full, verbose = False)
 
 def test_svd_c_rand():
-    for i in xrange(5):
+    for i in range(5):
         full = mp.rand() > 0.5
         m = 1 + int(mp.rand() * 10)
         n = 1 + int(mp.rand() * 10)
         A = (2 * mp.randmatrix(m, n) - 1) + 1j * (2 * mp.randmatrix(m, n) - 1)
         if mp.rand() > 0.5:
             A *= 10
-            for x in xrange(m):
-                for y in xrange(n):
+            for x in range(m):
+                for y in range(n):
                     A[x,y]=int(mp.re(A[x,y])) + 1j * int(mp.im(A[x,y]))
 
         run_svd_c(A, full_matrices=full, verbose=False)
 
 def test_svd_test_case():
     # a test case from Golub and Reinsch
     #  (see wilkinson/reinsch: handbook for auto. comp., vol ii-linear algebra, 134-151(1971).)
@@ -323,23 +318,23 @@
 def test_gauss_quadrature_dynamic(verbose = False):
     n = 5
 
     A = mp.randmatrix(2 * n, 1)
 
     def F(x):
         r = 0
-        for i in xrange(len(A) - 1, -1, -1):
+        for i in range(len(A) - 1, -1, -1):
             r = r * x + A[i]
         return r
 
     def run(qtype, FW, R, alpha = 0, beta = 0):
         X, W = mp.gauss_quadrature(n, qtype, alpha = alpha, beta = beta)
 
         a = 0
-        for i in xrange(len(X)):
+        for i in range(len(X)):
             a += W[i] * F(X[i])
 
         b = mp.quad(lambda x: FW(x) * F(x), R)
 
         c = mp.fabs(a - b)
 
         if verbose:
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_elliptic.py` & `mpmath-1.4.0a0/mpmath/tests/test_elliptic.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 [1] Abramowitz & Stegun. 'Handbook of Mathematical Functions, 9th Ed.',
     (Dover duplicate of 1972 edition)
 [2] Whittaker 'A Course of Modern Analysis, 4th Ed.', 1946,
     Cambridge University Press
 
 """
 
-import mpmath
 import random
+
 import pytest
 
-from mpmath import *
+from mpmath import (cos, cosh, cot, coth, csc, csch, diff, ellipe, ellipfun,
+                    ellipk, ellippi, elliprc, elliprd, elliprf, elliprg,
+                    elliprj, eps, exp, isnan, j, jtheta, ldexp, ln2, mp, mpc,
+                    mpf, nan, pi, qfrom, sec, sech, sin, sinh, sqrt, tan, tanh)
+
 
 def mpc_ae(a, b, eps=eps):
     res = True
     res = res and a.real.ae(b.real, eps)
     res = res and a.imag.ae(b.imag, eps)
     return res
 
@@ -31,15 +35,14 @@
 jsn = ellipfun('sn')
 jcn = ellipfun('cn')
 jdn = ellipfun('dn')
 
 calculate_nome = lambda k: qfrom(k=k)
 
 def test_ellipfun():
-    mp.dps = 15
     assert ellipfun('ss', 0, 0) == 1
     assert ellipfun('cc', 0, 0) == 1
     assert ellipfun('dd', 0, 0) == 1
     assert ellipfun('nn', 0, 0) == 1
     assert ellipfun('sn', 0.25, 0).ae(sin(0.25))
     assert ellipfun('cn', 0.25, 0).ae(cos(0.25))
     assert ellipfun('dn', 0.25, 0).ae(1)
@@ -100,15 +103,15 @@
              (mpf(9)/10, mpf('0.1401731269542615524091055'))]
 
     for i in math1:
         m = i[0]
         q = calculate_nome(sqrt(m))
         assert q.ae(i[1])
 
-    mp.dps = 15
+    assert qfrom(m=mp.ninf).ae(mpf('-1.0'))
 
 def test_jtheta():
     mp.dps = 25
 
     z = q = zero
     for n in range(1,5):
         value = jtheta(n, z, q)
@@ -148,16 +151,14 @@
     for i in range(10):
         qstring = str(random.random())
         q = mpf(qstring)
         result = jtheta(1, z1, q)
         assert(result.ae(0))
         result = jtheta(2, z2, q)
         assert(result.ae(0))
-    mp.dps = 15
-
 
 def test_jtheta_issue_79():
     # near the circle of covergence |q| = 1 the convergence slows
     # down; for |q| > Q_LIM the theta functions raise ValueError
     mp.dps = 30
     mp.dps += 30
     q = mpf(6)/10 - one/10**6 - mpf(8)/10 * j
@@ -269,15 +270,14 @@
         # Abramowitz 16.28.5
         # v_2(0, q)**4 + v_4(0, q)**4 == v_3(0, q)**4
         term1 = (jtheta(2, zero, q))**4
         term2 = (jtheta(4, zero, q))**4
         term3 = (jtheta(3, zero, q))**4
         equality = term1 + term2 - term3
         assert(equality.ae(0, eps1))
-    mp.dps = 15
 
 def test_jtheta_complex():
     mp.dps = 30
     z = mpf(1)/4 + j/8
     q = mpf(1)/3 + j/7
     # Mathematica N[EllipticTheta[1, 1/4 + I/8, 1/3 + I/7], 35]
     res = mpf('0.31618034835986160705729105731678285') + \
@@ -314,15 +314,14 @@
         (t[3]*a[4])**2 - (t[4]*a[3])**2 + (t[1] *a[2])**2,
         (t[1]*a[4])**2 - (t[3]*a[2])**2 + (t[2] *a[3])**2,
         (t[4]*a[4])**2 - (t[3]*a[3])**2 + (t[2] *a[2])**2,
         a[2]**4 + a[4]**4 - a[3]**4]
     mp.dps -= 10
     for x in r:
         assert(mpc_ae(x, mpc(0)))
-    mp.dps = 15
 
 def test_djtheta():
     mp.dps = 30
 
     z = one/7 + j/3
     q = one/8 + j/5
     # Mathematica N[EllipticThetaPrime[1, 1/7 + I/3, 1/8 + I/5], 35]
@@ -373,15 +372,14 @@
     z = zero
     a = [0]*5
     a[1] = jtheta(1, z, q, 3)/jtheta(1, z, q, 1)
     for n in [2,3,4]:
         a[n] = jtheta(n, z, q, 2)/jtheta(n, z, q)
     equality = a[2] + a[3] + a[4] - a[1]
     assert(equality.ae(0))
-    mp.dps = 15
 
 def test_jsn():
     """
     Test some special cases of the sn(z, q) function.
     """
     mp.dps = 100
 
@@ -418,15 +416,14 @@
     result = jsn(arg, m)
     assert(result.ae(res))
 
     # N[JacobiSN[1/10, 1/10], 25]
     res = mpf('0.09981686718599080096451168')
     result = jsn(arg, arg)
     assert(result.ae(res))
-    mp.dps = 15
 
 def test_jcn():
     """
     Test some special cases of the cn(z, q) function.
     """
     mp.dps = 100
 
@@ -455,15 +452,14 @@
     result = jcn(arg, m)
     assert(result.ae(res))
 
     # N[JacobiCN[1/10, 1/10], 25]
     res = mpf('0.9950058256237368748520459')
     result = jcn(arg, arg)
     assert(result.ae(res))
-    mp.dps = 15
 
 def test_jdn():
     """
     Test some special cases of the dn(z, q) function.
     """
     mp.dps = 100
 
@@ -477,16 +473,14 @@
 
     mp.dps = 25
     # N[JacobiDN[1/10, 1/10], 25]
     res = mpf('0.9995017055025556219713297')
     arg = one/10
     result = jdn(arg, arg)
     assert(result.ae(res))
-    mp.dps = 15
-
 
 def test_sn_cn_dn_identities():
     """
     Tests the some of the jacobi elliptic function identities found
     on Mathworld. Haven't found in Abramowitz.
     """
     mp.dps = 100
@@ -546,16 +540,14 @@
 
         # Abramowitz Table 16.6.3
         # dn(z, 0) = 1, m == 0
         z = m
         value = jdn(z, zero)
         assert(value.ae(one))
 
-    mp.dps = 15
-
 def test_sn_cn_dn_complex():
     mp.dps = 30
     # N[JacobiSN[1/4 + I/8, 1/3 + I/7], 35] in Mathematica
     res = mpf('0.2495674401066275492326652143537') + \
           mpf('0.12017344422863833381301051702823') * j
     u = mpf(1)/4 + j/8
     m = mpf(1)/3 + j/7
@@ -571,19 +563,17 @@
     assert(mpc_ae(r, res))
 
     #N[JacobiDN[1/4 + I/8, 1/3 + I/7], 35]
     res = mpf('0.99639490163039577560547478589753039') - \
           mpf('0.01346296520008176393432491077244994')*j
     r = jdn(u, m)
     assert(mpc_ae(r, res))
-    mp.dps = 15
 
 def test_elliptic_integrals():
     # Test cases from Carlson's paper
-    mp.dps = 15
     assert elliprd(0,2,1).ae(1.7972103521033883112)
     assert elliprd(2,3,4).ae(0.16510527294261053349)
     assert elliprd(j,-j,2).ae(0.65933854154219768919)
     assert elliprd(0,j,-j).ae(1.2708196271909686299 + 2.7811120159520578777j)
     assert elliprd(0,j-1,j).ae(-1.8577235439239060056 - 0.96193450888838559989j)
     assert elliprd(-2-j,-j,-1+j).ae(1.8249027393703805305 - 1.2218475784827035855j)
     # extra test cases
@@ -664,7 +654,10 @@
     assert ellippi(2.0-0.5j, 0.5+1.0j).ae(0.936761970766645807 - 1.61876787838890786j)
     assert ellippi(2.0, 1.0+1.0j).ae(0.999881420735506708 - 2.4139272867045391j)
     assert ellippi(2.0+1.0j, 2.0-1.0j).ae(1.8578723151271115 + 1.18642180609983531j)
     assert ellippi(2.0+1.0j, 2.0).ae(2.78474654927885845 + 2.02204728966993314j)
 
 def test_issue_238():
     assert isnan(qfrom(m=nan))
+
+def test_issue_604():
+    assert ellipe(pi, 1).ae('2.0')
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_fp.py` & `mpmath-1.4.0a0/mpmath/tests/test_fp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 Easy-to-use test-generating code:
 
 cases = '''
 exp 2.25
 log 2.25
 '''
 
-from mpmath import *
+from mpmath import ae, fp, mp
 mp.dps = 20
 for test in cases.splitlines():
     if not test:
         continue
     words = test.split()
     fname = words[0]
     args = words[1:]
     argstr = ", ".join(args)
     testline = "%s(%s)" % (fname, argstr)
     ans = str(eval(testline))
     print "    assert ae(fp.%s, %s)" % (testline, ans)
 
 """
 
+import pytest
+
 from mpmath import fp
 
+
 def ae(x, y, tol=1e-12):
     if x == y:
         return True
     return abs(x-y) <= tol*abs(y)
 
 def test_conj():
     assert fp.conj(4) == 4
@@ -105,41 +108,48 @@
     assert ae(fp.sinpi(-0.7), -0.80901699437494750611)
     assert ae(fp.cospi(-0.7), -0.5877852522924730163)
     assert ae(fp.cospi(-3+2j), (-267.74676148374822225 + 0.0j))
     assert ae(fp.sinpi(-3+2j), (0.0 - 267.74489404101651426j))
     assert ae(fp.sinpi(-0.7+2j), (-216.6116802292079471 - 157.37650009392034693j))
     assert ae(fp.cospi(-0.7+2j), (-157.37759774921754565 + 216.61016943630197336j))
 
+def test_fp_asinh_acosh_atanh():
+    assert ae(fp.asinh(0), 0.0)
+    assert ae(fp.acosh(1), 0.0)
+    assert ae(fp.atanh(0), 0.0)
+
 def test_fp_expj():
     assert ae(fp.expj(0), (1.0 + 0.0j))
     assert ae(fp.expj(1), (0.5403023058681397174 + 0.84147098480789650665j))
     assert ae(fp.expj(2), (-0.416146836547142387 + 0.9092974268256816954j))
     assert ae(fp.expj(0.75), (0.73168886887382088631 + 0.68163876002333416673j))
     assert ae(fp.expj(2+3j), (-0.020718731002242879378 + 0.045271253156092975488j))
     assert ae(fp.expjpi(0), (1.0 + 0.0j))
     assert ae(fp.expjpi(1), (-1.0 + 0.0j))
     assert ae(fp.expjpi(2), (1.0 + 0.0j))
     assert ae(fp.expjpi(0.75), (-0.7071067811865475244 + 0.7071067811865475244j))
     assert ae(fp.expjpi(2+3j), (0.000080699517570304599239 + 0.0j))
 
-def test_fp_bernoulli():
-    assert ae(fp.bernoulli(0), 1.0)
-    assert ae(fp.bernoulli(1), -0.5)
-    assert ae(fp.bernoulli(2), 0.16666666666666666667)
-    assert ae(fp.bernoulli(10), 0.075757575757575757576)
-    assert ae(fp.bernoulli(11), 0.0)
+@pytest.mark.parametrize('plus', [True, False])
+def test_fp_bernoulli(plus):
+    assert ae(fp.bernoulli(0, plus), 1.0)
+    assert ae(fp.bernoulli(1, plus), 0.5 if plus else -0.5)
+    assert ae(fp.bernoulli(2, plus), 0.16666666666666666667)
+    assert ae(fp.bernoulli(10, plus), 0.075757575757575757576)
+    assert ae(fp.bernoulli(11, plus), 0.0)
 
 def test_fp_gamma():
     assert ae(fp.gamma(1), 1.0)
     assert ae(fp.gamma(1.5), 0.88622692545275801365)
     assert ae(fp.gamma(10), 362880.0)
     assert ae(fp.gamma(-0.5), -3.5449077018110320546)
     assert ae(fp.gamma(-7.1), 0.0016478244570263333622)
     assert ae(fp.gamma(12.3), 83385367.899970000963)
     assert ae(fp.gamma(2+0j), (1.0 + 0.0j))
+    assert fp.isnan(fp.gamma(-fp.inf))
     assert ae(fp.gamma(-2.5+0j), (-0.94530872048294188123 + 0.0j))
     assert ae(fp.gamma(3+4j), (0.0052255384713692141947 - 0.17254707929430018772j))
     assert ae(fp.gamma(-3-4j), (0.00001460997305874775607 - 0.000020760733311509070396j))
     assert ae(fp.fac(0), 1.0)
     assert ae(fp.fac(1), 1.0)
     assert ae(fp.fac(20), 2432902008176640000.0)
     assert ae(fp.fac(-3.5), -0.94530872048294188123)
@@ -1665,7 +1675,35 @@
     assert ae(v, (3.070744996327018106e+84 + 1.7243244846769415903e+84j), tol=ATOL)
     assert ae(v.real, 3.070744996327018106e+84, tol=PTOL)
     assert ae(v.imag, 1.7243244846769415903e+84, tol=PTOL)
     v = fp.ei((320.0 - 80.0j))
     assert ae(v, (-9.9960598637998647276e+135 + 2.6855081527595608863e+136j), tol=ATOL)
     assert ae(v.real, -9.9960598637998647276e+135, tol=PTOL)
     assert ae(v.imag, 2.6855081527595608863e+136, tol=PTOL)
+
+def test_fp_isfinite():
+    assert fp.isfinite(1.2)
+    assert fp.isfinite(1+2j)
+    assert not fp.isfinite(fp.inf)
+    assert not fp.isfinite(fp.nan)
+
+def test_fp_nan_in_args():
+    assert fp.isnan(fp.ei(fp.nan))  # issue 483
+    assert fp.isnan(fp.li(fp.nan))  # issue 484
+    assert fp.isnan(fp.ci(fp.nan))  # issue 480
+    assert fp.isnan(fp.si(fp.nan))  # issue 481
+    assert fp.isnan(fp.chi(fp.nan))  # issue 482
+    assert fp.isnan(fp.shi(fp.nan))
+    assert fp.isnan(fp.e1(fp.nan))  # issue 487
+    assert fp.isnan(fp.chebyt(1.3, fp.nan))  # issue 478
+    assert fp.isnan(fp.chebyt(13, fp.nan))
+    assert fp.isnan(fp.hyp2f2(0.4, 2.5, 2.2, 0.7, fp.nan))  # issue 509
+
+def test_issue_510():
+    assert fp.rgamma(fp.inf) == fp.zero
+
+def test_issue_491():
+    assert fp.appellf1(0, 0.4, 2.5, 2.2, fp.inf, 1.4) == fp.one
+
+def test_issue_521():
+    assert fp.ff(1, -fp.inf) == 0.0
+    assert fp.isnan(fp.ff(1, fp.inf))
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_functions.py` & `mpmath-1.4.0a0/mpmath/tests/test_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,28 @@
-from mpmath.libmp import *
-from mpmath import *
-import random
-import time
-import math
 import cmath
+import math
+import random
+
+import pytest
+
+from mpmath import (acos, acosh, acot, acoth, acsc, acsch, arange, arg, asec,
+                    asech, asin, asinh, atan, atan2, atanh, catalan, cbrt,
+                    ceil, conj, cos, cos_sin, cosh, cospi, cospi_sinpi, cot,
+                    coth, csc, csch, cyclotomic, degree, degrees, e, eps,
+                    euler, exp, expj, expjpi, expm1, fabs, fadd, fib,
+                    fibonacci, floor, fmod, fp, frexp, glaisher, hypot, im,
+                    inf, isnan, j, khinchin, ldexp, linspace, ln, ln2, ln10,
+                    log, log1p, log10, mertens, mp, mpc, mpf, nan, nthroot,
+                    phi, pi, power, powm1, radians, rand, re, root, sec, sech,
+                    sign, sin, sinc, sincpi, sinh, sinpi, sqrt, tan, tanh,
+                    twinprime, unitroots)
+from mpmath.libmp import (ComplexResult, from_int, mpf_gt, mpf_lt, mpf_mul,
+                          mpf_pow_int, mpf_rand, mpf_sqrt, round_ceiling,
+                          round_down, round_nearest, round_up)
+
 
 def mpc_ae(a, b, eps=eps):
     res = True
     res = res and a.real.ae(b.real, eps)
     res = res and a.imag.ae(b.imag, eps)
     return res
 
@@ -106,26 +121,30 @@
     assert sqrt(b, rounding='d') < 3
     assert sqrt(b, rounding='n') == 3
     assert sqrt(b, rounding='u') == 3
     # A worst case, from the MPFR test suite
     assert sqrt(mpf('7.0503726185518891')) == mpf('2.655253776675949')
 
 def test_float_sqrt():
-    mp.dps = 15
     # These should round identically
     for x in [0, 1e-7, 0.1, 0.5, 1, 2, 3, 4, 5, 0.333, 76.19]:
         assert sqrt(mpf(x)) == float(x)**0.5
     assert sqrt(-1) == 1j
     assert sqrt(-2).ae(cmath.sqrt(-2))
     assert sqrt(-3).ae(cmath.sqrt(-3))
     assert sqrt(-100).ae(cmath.sqrt(-100))
     assert sqrt(1j).ae(cmath.sqrt(1j))
     assert sqrt(-1j).ae(cmath.sqrt(-1j))
     assert sqrt(math.pi + math.e*1j).ae(cmath.sqrt(math.pi + math.e*1j))
     assert sqrt(math.pi - math.e*1j).ae(cmath.sqrt(math.pi - math.e*1j))
+    mp2 = mp.clone()
+    mp2.trap_complex = True
+    pytest.raises(ComplexResult, lambda: mp2.sqrt(-1))
+    pytest.raises(ComplexResult, lambda: mp2.mpf(-1)**0.5)
+    pytest.raises(ComplexResult, lambda: mp2.mpf(-1)**mp2.mpf(0.5))
 
 def test_hypot():
     assert hypot(0, 0) == 0
     assert hypot(0, 0.33) == mpf(0.33)
     assert hypot(0.33, 0) == mpf(0.33)
     assert hypot(-0.33, 0) == mpf(0.33)
     assert hypot(3, 4) == mpf(5)
@@ -134,39 +153,37 @@
     for i in range(0, 20000, 200):
         assert cbrt(mpf(i*i*i)) == i
     random.seed(1)
     for prec in [100, 300, 1000, 10000]:
         mp.dps = prec
         A = random.randint(10**(prec//2-2), 10**(prec//2-1))
         assert cbrt(mpf(A*A*A)) == A
-    mp.dps = 15
 
 def test_exp():
     assert exp(0) == 1
     assert exp(10000).ae(mpf('8.8068182256629215873e4342'))
     assert exp(-10000).ae(mpf('1.1354838653147360985e-4343'))
     a = exp(mpf((1, 8198646019315405, -53, 53)))
-    assert(a.bc == bitcount(a.man))
+    assert a.bc == a.man.bit_length()
     mp.prec = 67
     a = exp(mpf((1, 1781864658064754565, -60, 61)))
-    assert(a.bc == bitcount(a.man))
+    assert a.bc == a.man.bit_length()
     mp.prec = 53
     assert exp(ln2 * 10).ae(1024)
     assert exp(2+2j).ae(cmath.exp(2+2j))
 
 def test_issue_73():
     mp.dps = 512
     a = exp(-1)
     b = exp(1)
     mp.dps = 15
     assert (+a).ae(0.36787944117144233)
     assert (+b).ae(2.7182818284590451)
 
 def test_log():
-    mp.dps = 15
     assert log(1) == 0
     for x in [0.5, 1.5, 2.0, 3.0, 100, 10**50, 1e-50]:
         assert log(x).ae(math.log(x))
         assert log(x, x) == 1
     assert log(1024, 2) == 10
     assert log(10**1234, 10) == 1234
     assert log(2+2j).ae(cmath.log(2+2j))
@@ -246,15 +263,14 @@
     mp.dps = 15
     random.seed(1)
     for (z1, z2) in random_complexes(100):
         assert (mpc(z1)**mpc(z2)).ae(z1**z2, 1e-12)
     assert (e**(-pi*1j)).ae(-1)
     mp.dps = 50
     assert (e**(-pi*1j)).ae(-1)
-    mp.dps = 15
 
 def test_complex_sqrt_accuracy():
     def test_mpc_sqrt(lst):
         for a, b in lst:
             z = mpc(a + j*b)
             assert mpc_ae(sqrt(z*z), z)
             z = mpc(-a + j*b)
@@ -265,18 +281,16 @@
             assert mpc_ae(sqrt(z*z), -z)
     random.seed(2)
     N = 10
     mp.dps = 30
     dps = mp.dps
     test_mpc_sqrt([(random.uniform(0, 10),random.uniform(0, 10)) for i in range(N)])
     test_mpc_sqrt([(i + 0.1, (i + 0.2)*10**i) for i in range(N)])
-    mp.dps = 15
 
 def test_atan():
-    mp.dps = 15
     assert atan(-2.3).ae(math.atan(-2.3))
     assert atan(1e-50) == 1e-50
     assert atan(1e50).ae(pi/2)
     assert atan(-1e-50) == -1e-50
     assert atan(-1e50).ae(-pi/2)
     assert atan(10**1000).ae(pi/2)
     for dps in [25, 70, 100, 300, 1000]:
@@ -294,15 +308,14 @@
     assert atan(mpc(-inf,0)).ae(-pi2)
     assert atan(mpc(-inf,-1)).ae(-pi2)
     assert atan(mpc(-1,-inf)).ae(-pi2)
     assert atan(mpc(0,-inf)).ae(-pi2)
     assert atan(mpc(1,-inf)).ae(pi2)
 
 def test_atan2():
-    mp.dps = 15
     assert atan2(1,1).ae(pi/4)
     assert atan2(1,-1).ae(3*pi/4)
     assert atan2(-1,-1).ae(-3*pi/4)
     assert atan2(-1,1).ae(-pi/4)
     assert atan2(-1,0).ae(-pi/2)
     assert atan2(1,0).ae(pi/2)
     assert atan2(0,0) == 0
@@ -358,18 +371,16 @@
 
     dps = mp.dps
     mp.dps = 300
     assert isinstance(asin(0.5), mpf)
     mp.dps = 1000
     assert asin(1).ae(pi/2)
     assert asin(-1).ae(-pi/2)
-    mp.dps = dps
 
 def test_invhyperb_inaccuracy():
-    mp.dps = 15
     assert (asinh(1e-5)*10**5).ae(0.99999999998333333)
     assert (asinh(1e-10)*10**10).ae(1)
     assert (asinh(1e-50)*10**50).ae(1)
     assert (asinh(-1e-5)*10**5).ae(-0.99999999998333333)
     assert (asinh(-1e-10)*10**10).ae(-1)
     assert (asinh(-1e-50)*10**50).ae(-1)
     assert asinh(10**20).ae(46.744849040440862)
@@ -389,16 +400,14 @@
             assert sin(mpc(z)).ae(cmath.sin(z))
             assert tan(mpc(z)).ae(cmath.tan(z))
             assert sinh(mpc(z)).ae(cmath.sinh(z))
             assert cosh(mpc(z)).ae(cmath.cosh(z))
             assert tanh(mpc(z)).ae(cmath.tanh(z))
 
 def test_complex_inverse_functions():
-    mp.dps = 15
-    iv.dps = 15
     for (z1, z2) in random_complexes(30):
         # apparently cmath uses a different branch, so we
         # can't use it for comparison
         assert sinh(asinh(z1)).ae(z1)
         #
         assert acosh(z1).ae(cmath.acosh(z1))
         assert atanh(z1).ae(cmath.atanh(z1))
@@ -438,22 +447,20 @@
     assert asech(0.5).ae(1.31695789692481671)
     assert acsch(3).ae(0.327450150237258443)
     assert acoth(3).ae(0.346573590279972655)
     assert acot(0).ae(1.5707963267948966192)
     assert acoth(0).ae(1.5707963267948966192j)
 
 def test_ldexp():
-    mp.dps = 15
     assert ldexp(mpf(2.5), 0) == 2.5
     assert ldexp(mpf(2.5), -1) == 1.25
     assert ldexp(mpf(2.5), 2) == 10
     assert ldexp(mpf('inf'), 3) == mpf('inf')
 
 def test_frexp():
-    mp.dps = 15
     assert frexp(0) == (0.0, 0)
     assert frexp(9) == (0.5625, 4)
     assert frexp(1) == (0.5, 1)
     assert frexp(0.2) == (0.8, -2)
     assert frexp(1000) == (0.9765625, 10)
 
 def test_aliases():
@@ -489,15 +496,14 @@
     assert sign(-3*j) == -j
     assert sign(1+j).ae((1+j)/sqrt(2))
 
 def test_misc_bugs():
     # test that this doesn't raise an exception
     mp.dps = 1000
     log(1302)
-    mp.dps = 15
 
 def test_arange():
     assert arange(10) == [mpf('0.0'), mpf('1.0'), mpf('2.0'), mpf('3.0'),
                           mpf('4.0'), mpf('5.0'), mpf('6.0'), mpf('7.0'),
                           mpf('8.0'), mpf('9.0')]
     assert arange(-5, 5) == [mpf('-5.0'), mpf('-4.0'), mpf('-3.0'),
                              mpf('-2.0'), mpf('-1.0'), mpf('0.0'),
@@ -541,15 +547,14 @@
         assert r1.ae(r2, eps)
     mp.dps = 100
     for n in range(100, 301, 100):
         w = 10**n + j*10**-3
         z = w*w*w
         r = cbrt(z)
         assert mpc_ae(r, w, eps)
-    mp.dps = 15
 
 def test_root():
     mp.dps = 30
     random.seed(1)
     a = random.randint(0, 10000)
     p = a*a*a
     r = nthroot(mpf(p), 3)
@@ -630,18 +635,16 @@
         assert r.ae(mpf(10)**(-5) * (1 + j) * mpf(2)**(-0.5))
     mp.dps = 80
     assert nthroot('-1e-3', 4).ae(mpf(10)**(-3./4) * (1 + j)/sqrt(2))
     assert nthroot('-1e-6', 4).ae((1 + j)/(10 * sqrt(20)))
     # Check that this doesn't take eternity to compute
     mp.dps = 20
     assert nthroot('-1e100000000', 4).ae((1+j)*mpf('1e25000000')/sqrt(2))
-    mp.dps = 15
 
 def test_mpcfun_real_imag():
-    mp.dps = 15
     x = mpf(0.3)
     y = mpf(0.4)
     assert exp(mpc(x,0)) == exp(x)
     assert exp(mpc(0,y)) == mpc(cos(y),sin(y))
     assert cos(mpc(x,0)) == cos(x)
     assert sin(mpc(x,0)) == sin(x)
     assert cos(mpc(0,y)) == cosh(y)
@@ -795,42 +798,38 @@
     assert sinc(-inf) == sincpi(-inf) == 0
     assert sinc(2).ae(0.45464871341284084770)
     assert sinc(2+3j).ae(0.4463290318402435457-2.7539470277436474940j)
     assert sincpi(2) == 0
     assert sincpi(1.5).ae(-0.212206590789193781)
 
 def test_fibonacci():
-    mp.dps = 15
     assert [fibonacci(n) for n in range(-5, 10)] == \
         [5, -3, 2, -1, 1, 0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
     assert fib(2.5).ae(1.4893065462657091)
     assert fib(3+4j).ae(-5248.51130728372 - 14195.962288353j)
     assert fib(1000).ae(4.3466557686937455e+208)
     assert str(fib(10**100)) == '6.24499112864607e+2089876402499787337692720892375554168224592399182109535392875613974104853496745963277658556235103534'
     mp.dps = 2100
     a = fib(10000)
     assert a % 10**10 == 9947366875
     mp.dps = 15
     assert fibonacci(inf) == inf
     assert fib(3+0j) == 2
 
 def test_call_with_dps():
-    mp.dps = 15
     assert abs(exp(1, dps=30)-e(dps=35)) < 1e-29
 
 def test_tanh():
-    mp.dps = 15
     assert tanh(0) == 0
     assert tanh(inf) == 1
     assert tanh(-inf) == -1
     assert isnan(tanh(nan))
     assert tanh(mpc('inf', '0')) == 1
 
 def test_atanh():
-    mp.dps = 15
     assert atanh(0) == 0
     assert atanh(0.5).ae(0.54930614433405484570)
     assert atanh(-0.5).ae(-0.54930614433405484570)
     assert atanh(1) == inf
     assert atanh(-1) == -inf
     assert isnan(atanh(nan))
     assert isinstance(atanh(1), mpf)
@@ -849,31 +848,28 @@
     assert atanh(mpc(-inf,0)).ae(jpi2)
     assert atanh(mpc(-inf,-1)).ae(-jpi2)
     assert atanh(mpc(-1,-inf)).ae(-jpi2)
     assert atanh(mpc(0,-inf)).ae(-jpi2)
     assert atanh(mpc(1,-inf)).ae(-jpi2)
 
 def test_expm1():
-    mp.dps = 15
     assert expm1(0) == 0
     assert expm1(3).ae(exp(3)-1)
     assert expm1(inf) == inf
     assert expm1(1e-50).ae(1e-50)
     assert (expm1(1e-10)*1e10).ae(1.00000000005)
 
 def test_log1p():
-    mp.dps = 15
     assert log1p(0) == 0
     assert log1p(3).ae(log(1+3))
     assert log1p(inf) == inf
     assert log1p(1e-50).ae(1e-50)
     assert (log1p(1e-10)*1e10).ae(0.99999999995)
 
 def test_powm1():
-    mp.dps = 15
     assert powm1(2,3) == 7
     assert powm1(-1,2) == 0
     assert powm1(-1,0) == 0
     assert powm1(-2,0) == 0
     assert powm1(3+4j,0) == 0
     assert powm1(0,1) == -1
     assert powm1(0,0) == 0
@@ -898,15 +894,14 @@
     assert unitroots(2, primitive=True) == [-1]
     assert unitroots(3, primitive=True) == unitroots(3)[1:]
     assert unitroots(4, primitive=True) == [j, -j]
     assert len(unitroots(17, primitive=True)) == 16
     assert len(unitroots(16, primitive=True)) == 8
 
 def test_cyclotomic():
-    mp.dps = 15
     assert [cyclotomic(n,1) for n in range(31)] == [1,0,2,3,2,5,1,7,2,3,1,11,1,13,1,1,2,17,1,19,1,1,1,23,1,5,1,3,1,29,1]
     assert [cyclotomic(n,-1) for n in range(31)] == [1,-2,0,1,2,1,3,1,2,1,5,1,1,1,7,1,2,1,3,1,1,1,11,1,1,1,13,1,1,1,1]
     assert [cyclotomic(n,j) for n in range(21)] == [1,-1+j,1+j,j,0,1,-j,j,2,-j,1,j,3,1,-j,1,2,1,j,j,5]
     assert [cyclotomic(n,-j) for n in range(21)] == [1,-1-j,1-j,-j,0,1,j,-j,2,j,1,-j,3,1,j,1,2,1,-j,-j,5]
     assert cyclotomic(1624,j) == 1
     assert cyclotomic(33600,j) == 1
     u = sqrt(j, prec=500)
@@ -914,7 +909,48 @@
     assert cyclotomic(30, u).ae(5.8284271247461900976)
     assert cyclotomic(2040, u).ae(1)
     assert cyclotomic(0,2.5) == 1
     assert cyclotomic(1,2.5) == 2.5-1
     assert cyclotomic(2,2.5) == 2.5+1
     assert cyclotomic(3,2.5) == 2.5**2 + 2.5 + 1
     assert cyclotomic(7,2.5) == 406.234375
+
+def test_mp_nan_in_args():
+    assert mp.isnan(mp.legendre(1.2, mp.nan))  # issue 485
+    assert mp.isnan(mp.hyp2f1(0.5, 0.5, 0.5, mp.nan))
+    assert mp.isnan(mp.hyp2f1(0.5, 2.2, 0.5, mp.nan))
+    assert mp.isnan(mp.hyp2f1(0.4, 2.2, 0.5, mp.nan))  # issue 479
+    assert mp.isnan(mp.chebyt(2.3, mp.nan))  # issue 478
+    assert mp.isnan(mp.chebyt(13, mp.nan))
+    assert mp.isnan(mp.chebyt(17, mp.nan))
+    assert mp.isnan(mp.hyp1f1(0, 1, mp.nan))  # issue 507
+    assert mp.isnan(mp.hyp1f1(1, 1, mp.nan))
+    assert mp.isnan(mp.hyp1f1(1, 1.1, mp.nan))
+    assert mp.isnan(mp.hyp1f1(1, 2, mp.nan))
+    assert mp.isnan(mp.hyp1f1(1, 3, mp.nan))
+    assert mp.isnan(mp.hyp1f1(1, 4, mp.nan))
+    assert mp.isnan(mp.hyp1f1(2, 1, mp.nan))
+    assert mp.isnan(mp.hyp1f1(2, 2, mp.nan))
+    assert mp.isnan(mp.hyp1f1(0, 2, mp.nan))
+    assert mp.isnan(mp.hyp1f1(0, 4, mp.nan))
+    assert mp.isnan(mp.hyp0f1(2.5, mp.nan))  # issue 489
+    assert mp.isnan(mp.hyp0f1(25, mp.nan))
+    assert mp.isnan(mp.hyp0f1(2513, mp.nan))
+    assert mp.isnan(mp.hyp0f1(.25, mp.nan))
+    assert mp.isnan(mp.hyp1f1(2.5,2.2, mp.nan))  # issue 488
+    assert mp.isnan(mp.hyp1f1(1,2.2, mp.nan))
+    assert mp.isnan(mp.hyp1f1(1,2002.2, mp.nan))
+    assert mp.isnan(mp.hyp2f2(0.4, 2.5, 2.2, 0.7, mp.nan))  # issue 509
+    assert mp.isnan(mp.gegenbauer(0, 2.5, mp.nan))  # issue 508
+    assert mp.isnan(mp.gegenbauer(1, 2.5, mp.nan))
+    assert mp.isnan(mp.gegenbauer(2, 2.5, mp.nan))
+    assert mp.isnan(mp.gegenbauer(2, 5, mp.nan))
+    assert mp.isnan(mp.laguerre(0, 2.5, mp.nan))  # issue 506
+    assert mp.isnan(mp.laguerre(1, 2.5, mp.nan))
+    assert mp.isnan(mp.laguerre(1, 2.5345, mp.nan))
+    assert mp.isnan(mp.laguerre(2, 2, mp.nan))
+    assert mp.isnan(mp.laguerre(2, 5, mp.nan))
+
+def test_issue_749():
+    assert mp.asinh(mp.inf) == mp.inf
+    assert mp.asinh(mp.mpc(mp.inf, 0)) == mp.mpc(mp.inf, 0)
+    assert fp.asinh(fp.mpc(fp.inf, 0)) == fp.mpc(fp.inf, 0)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_functions2.py` & `mpmath-1.4.0a0/mpmath/tests/test_functions2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,26 @@
-import math
 import pytest
-from mpmath import *
+
+from mpmath import (agm, airyai, airybi, appellf1, bei, ber, besseli, besselj,
+                    besseljzero, besselk, bessely, besselyzero, betainc,
+                    chebyt, chebyu, chi, ci, convert, coulombg, e, e1, ei,
+                    ellipe, ellipk, eps, erf, erfc, erfi, erfinv, exp, expint,
+                    fadd, fmul, fp, fraction, fresnelc, fresnels, fsub, fsum,
+                    gamma, gammainc, gegenbauer, hankel1, hankel2, hermite,
+                    hyp0f1, hyp1f1, hyp1f2, hyp2f0, hyp2f1, hyp2f2, hyp2f3,
+                    hyper, hypercomb, hyperu, inf, isnan, j, j0, j1, jacobi,
+                    kei, ker, laguerre, lambertw, ldexp, legendre, legenp,
+                    legenq, lerchphi, li, log, lower_gamma, meijerg, mp, mpc,
+                    mpf, nan, ncdf, npdf, nthroot, pi, qp, quadts, shi, si,
+                    spherharm, sqrt, struveh, struvel, upper_gamma, whitm,
+                    whitw, zeta)
+from mpmath.libmp import BACKEND
+
 
 def test_bessel():
-    mp.dps = 15
     assert j0(1).ae(0.765197686557966551)
     assert j0(pi).ae(-0.304242177644093864)
     assert j0(1000).ae(0.0247866861524201746)
     assert j0(-25).ae(0.0962667832759581162)
     assert j1(1).ae(0.440050585744933516)
     assert j1(pi).ae(0.284615343179752757)
     assert j1(1000).ae(0.00472831190708952392)
@@ -74,69 +87,63 @@
     assert (besselk(3, 10**10) * mpf(10)**4342944824).ae(1.1628981033356187851)
     # test for issue 331, bug reported by Michael Hartmann
     for n in range(10,100,10):
         mp.dps = n
         assert besseli(91.5,24.7708).ae("4.00830632138673963619656140653537080438462342928377020695738635559218797348548092636896796324190271316137982810144874264e-41")
 
 def test_bessel_zeros():
-    mp.dps = 15
     assert besseljzero(0,1).ae(2.40482555769577276869)
     assert besseljzero(2,1).ae(5.1356223018406825563)
     assert besseljzero(1,50).ae(157.86265540193029781)
     assert besseljzero(10,1).ae(14.475500686554541220)
     assert besseljzero(0.5,3).ae(9.4247779607693797153)
     assert besseljzero(2,1,1).ae(3.0542369282271403228)
     assert besselyzero(0,1).ae(0.89357696627916752158)
     assert besselyzero(2,1).ae(3.3842417671495934727)
     assert besselyzero(1,50).ae(156.29183520147840108)
     assert besselyzero(10,1).ae(12.128927704415439387)
     assert besselyzero(0.5,3).ae(7.8539816339744830962)
     assert besselyzero(2,1,1).ae(5.0025829314460639452)
 
 def test_hankel():
-    mp.dps = 15
     assert hankel1(0,0.5).ae(0.93846980724081290423-0.44451873350670655715j)
     assert hankel1(1,0.5).ae(0.2422684576748738864-1.4714723926702430692j)
     assert hankel1(-1,0.5).ae(-0.2422684576748738864+1.4714723926702430692j)
     assert hankel1(1.5,0.5).ae(0.0917016996256513026-2.5214655504213378514j)
     assert hankel1(1.5,3+4j).ae(0.0066806866476728165382-0.0036684231610839127106j)
     assert hankel2(0,0.5).ae(0.93846980724081290423+0.44451873350670655715j)
     assert hankel2(1,0.5).ae(0.2422684576748738864+1.4714723926702430692j)
     assert hankel2(-1,0.5).ae(-0.2422684576748738864-1.4714723926702430692j)
     assert hankel2(1.5,0.5).ae(0.0917016996256513026+2.5214655504213378514j)
     assert hankel2(1.5,3+4j).ae(14.783528526098567526-7.397390270853446512j)
 
 def test_struve():
-    mp.dps = 15
     assert struveh(2,3).ae(0.74238666967748318564)
     assert struveh(-2.5,3).ae(0.41271003220971599344)
     assert struvel(2,3).ae(1.7476573277362782744)
     assert struvel(-2.5,3).ae(1.5153394466819651377)
 
 def test_whittaker():
-    mp.dps = 15
     assert whitm(2,3,4).ae(49.753745589025246591)
     assert whitw(2,3,4).ae(14.111656223052932215)
 
 def test_kelvin():
-    mp.dps = 15
     assert ber(2,3).ae(0.80836846563726819091)
     assert ber(3,4).ae(-0.28262680167242600233)
     assert ber(-3,2).ae(-0.085611448496796363669)
     assert bei(2,3).ae(-0.89102236377977331571)
     assert bei(-3,2).ae(-0.14420994155731828415)
     assert ker(2,3).ae(0.12839126695733458928)
     assert ker(-3,2).ae(-0.29802153400559142783)
     assert ker(0.5,3).ae(-0.085662378535217097524)
     assert kei(2,3).ae(0.036804426134164634000)
     assert kei(-3,2).ae(0.88682069845786731114)
     assert kei(0.5,3).ae(0.013633041571314302948)
 
 def test_hyper_misc():
-    mp.dps = 15
     assert hyp0f1(1,0) == 1
     assert hyp1f1(1,2,0) == 1
     assert hyp1f2(1,2,3,0) == 1
     assert hyp2f1(1,2,3,0) == 1
     assert hyp2f2(1,2,3,4,0) == 1
     assert hyp2f3(1,2,3,4,5,0) == 1
     # Degenerate case: 0F0
@@ -147,18 +154,16 @@
     #
     assert hyp2f1((1,3),(2,3),(5,6),mpf(27)/32).ae(1.6)
     assert hyp2f1((1,4),(1,2),(3,4),mpf(80)/81).ae(1.8)
     assert hyp2f1((2,3),(1,1),(3,2),(2+j)/3).ae(1.327531603558679093+0.439585080092769253j)
     mp.dps = 25
     v = mpc('1.2282306665029814734863026', '-0.1225033830118305184672133')
     assert hyper([(3,4),2+j,1],[1,5,j/3],mpf(1)/5+j/8).ae(v)
-    mp.dps = 15
 
 def test_elliptic_integrals():
-    mp.dps = 15
     assert ellipk(0).ae(pi/2)
     assert ellipk(0.5).ae(gamma(0.25)**2/(4*sqrt(pi)))
     assert ellipk(1) == inf
     assert ellipk(1+0j) == inf
     assert ellipk(-1).ae('1.3110287771460599052')
     assert ellipk(-2).ae('1.1714200841467698589')
     assert isinstance(ellipk(-2), mpf)
@@ -207,18 +212,16 @@
     assert ellipe(-10*pi).ae('5.926192483740483797854383268707108012328213431657645509')
     v = ellipk(pi)
     assert v.real.ae('0.973089521698042334840454592642137667227167622330325225')
     assert v.imag.ae('-1.156151296372835303836814390793087600271609993858798016')
     v = ellipe(pi)
     assert v.real.ae('0.4632848917264710404078033487934663562998345622611263332')
     assert v.imag.ae('1.0637961621753130852473300451583414489944099504180510966')
-    mp.dps = 15
 
 def test_exp_integrals():
-    mp.dps = 15
     x = +e
     z = e + sqrt(3)*j
     assert ei(x).ae(8.21168165538361560)
     assert li(x).ae(1.89511781635593676)
     assert si(x).ae(1.82104026914756705)
     assert ci(x).ae(0.213958001340379779)
     assert shi(x).ae(4.11520706247846193)
@@ -257,15 +260,14 @@
     assert shi(0) == 0
     assert shi(inf) == inf
     assert shi(-inf) == -inf
     assert chi(0) == -inf
     assert chi(inf) == inf
 
 def test_ei():
-    mp.dps = 15
     assert ei(0) == -inf
     assert ei(inf) == inf
     assert ei(-inf) == -0.0
     assert ei(20+70j).ae(6.1041351911152984397e6 - 2.7324109310519928872e6j)
     # tests for the asymptotic expansion
     # values checked with Mathematica ExpIntegralEi
     mp.dps = 50
@@ -279,15 +281,14 @@
     sre = '-3.255138234032069402493850638874410725961401274106e+8681'
     sim = '-2.1081929993474403520785942429469187647767369645423e+8681'
     assert str(r.real) == sre and str(r.imag) == sim
     mp.dps = 15
     # More asymptotic expansions
     assert chi(-10**6+100j).ae('1.3077239389562548386e+434288 + 7.6808956999707408158e+434287j')
     assert shi(-10**6+100j).ae('-1.3077239389562548386e+434288 - 7.6808956999707408158e+434287j')
-    mp.dps = 15
     assert ei(10j).ae(-0.0454564330044553726+3.2291439210137706686j)
     assert ei(100j).ae(-0.0051488251426104921+3.1330217936839529126j)
     u = ei(fmul(10**20, j, exact=True))
     assert u.real.ae(-6.4525128526578084421345e-21, abs_eps=0, rel_eps=8*eps)
     assert u.imag.ae(pi)
     assert ei(-10j).ae(-0.0454564330044553726-3.2291439210137706686j)
     assert ei(-100j).ae(-0.0051488251426104921-3.1330217936839529126j)
@@ -296,27 +297,25 @@
     assert u.imag.ae(-pi)
     assert ei(10+10j).ae(-1576.1504265768517448+436.9192317011328140j)
     u = ei(-10+10j)
     assert u.real.ae(7.6698978415553488362543e-7, abs_eps=0, rel_eps=8*eps)
     assert u.imag.ae(3.141595611735621062025)
 
 def test_e1():
-    mp.dps = 15
     assert e1(0) == inf
     assert e1(inf) == 0
     assert e1(-inf) == mpc(-inf, -pi)
     assert e1(10j).ae(0.045456433004455372635 + 0.087551267423977430100j)
     assert e1(100j).ae(0.0051488251426104921444 - 0.0085708599058403258790j)
     assert e1(fmul(10**20, j, exact=True)).ae(6.4525128526578084421e-21 - 7.6397040444172830039e-21j, abs_eps=0, rel_eps=8*eps)
     assert e1(-10j).ae(0.045456433004455372635 - 0.087551267423977430100j)
     assert e1(-100j).ae(0.0051488251426104921444 + 0.0085708599058403258790j)
     assert e1(fmul(-10**20, j, exact=True)).ae(6.4525128526578084421e-21 + 7.6397040444172830039e-21j, abs_eps=0, rel_eps=8*eps)
 
 def test_expint():
-    mp.dps = 15
     assert expint(0,0) == inf
     assert expint(0,1).ae(1/e)
     assert expint(0,1.5).ae(2/exp(1.5)/3)
     assert expint(1,1).ae(-ei(-1))
     assert expint(2,0).ae(1)
     assert expint(3,0).ae(1/2.)
     assert expint(4,0).ae(1/3.)
@@ -440,37 +439,34 @@
     assert ae(fp.shi(-50j), -1.5516170724859358947j)
     assert ae(fp.shi(2-50j), -0.017515007378437448-1.497884414277228461j)
     assert ae(fp.shi(20-2j), -4.050116856873293554e6-1.20747603112735722103e7j)
     assert ae(fp.shi(20), 1.2807826332028294459e7)
     assert ae(fp.shi(2+50j), -0.017515007378437448+1.497884414277228461j)
 
 def test_airy():
-    mp.dps = 15
     assert (airyai(10)*10**10).ae(1.1047532552898687)
     assert (airybi(10)/10**9).ae(0.45564115354822515)
     assert (airyai(1000)*10**9158).ae(9.306933063179556004)
     assert (airybi(1000)/10**9154).ae(5.4077118391949465477)
     assert airyai(-1000).ae(0.055971895773019918842)
     assert airybi(-1000).ae(-0.083264574117080633012)
     assert (airyai(100+100j)*10**188).ae(2.9099582462207032076 + 2.353013591706178756j)
     assert (airybi(100+100j)/10**185).ae(1.7086751714463652039 - 3.1416590020830804578j)
 
 def test_hyper_0f1():
-    mp.dps = 15
     v = 8.63911136507950465
     assert hyper([],[(1,3)],1.5).ae(v)
     assert hyper([],[1/3.],1.5).ae(v)
     assert hyp0f1(1/3.,1.5).ae(v)
     assert hyp0f1((1,3),1.5).ae(v)
     # Asymptotic expansion
     assert hyp0f1(3,1e9).ae('4.9679055380347771271e+27455')
     assert hyp0f1(3,1e9j).ae('-2.1222788784457702157e+19410 + 5.0840597555401854116e+19410j')
 
 def test_hyper_1f1():
-    mp.dps = 15
     v = 1.2917526488617656673
     assert hyper([(1,2)],[(3,2)],0.7).ae(v)
     assert hyper([(1,2)],[(3,2)],0.7+0j).ae(v)
     assert hyper([0.5],[(3,2)],0.7).ae(v)
     assert hyper([0.5],[1.5],0.7).ae(v)
     assert hyper([0.5],[(3,2)],0.7+0j).ae(v)
     assert hyper([0.5],[1.5],0.7+0j).ae(v)
@@ -484,15 +480,14 @@
     assert (hyp1f1(2,3,1e10j)*10**10).ae(-0.97501205020039745852 - 1.7462392454512132074j)
     # Shouldn't use asymptotic expansion
     assert hyp1f1(-2, 1, 10000).ae(49980001)
     # Bug
     assert hyp1f1(1j,fraction(1,3),0.415-69.739j).ae(25.857588206024346592 + 15.738060264515292063j)
 
 def test_hyper_2f1():
-    mp.dps = 15
     v = 1.0652207633823291032
     assert hyper([(1,2), (3,4)], [2], 0.3).ae(v)
     assert hyper([(1,2), 0.75], [2], 0.3).ae(v)
     assert hyper([0.5, 0.75], [2.0], 0.3).ae(v)
     assert hyper([0.5, 0.75], [2.0], 0.3+0j).ae(v)
     assert hyper([0.5+0j, (3,4)], [2.0], 0.3+0j).ae(v)
     assert hyper([0.5+0j, (3,4)], [2.0], 0.3).ae(v)
@@ -514,15 +509,14 @@
     assert hyper([0.2,(3,10)],[0.4+0j],1.5+0j).ae(v)
     v = 0.76922501362865848528 + 0.32640579593235886194j
     assert hyper([(2,10),(3,10)],[(4,10)],4+2j).ae(v)
     assert hyper([0.2,(3,10)],[0.4+0j],4+2j).ae(v)
     assert hyper([0.2,(3,10)],[(4,10)],4+2j).ae(v)
 
 def test_hyper_2f1_hard():
-    mp.dps = 15
     # Singular cases
     assert hyp2f1(2,-1,-1,3).ae(7)
     assert hyp2f1(2,-1,-1,3,eliminate_all=True).ae(0.25)
     assert hyp2f1(2,-2,-2,3).ae(34)
     assert hyp2f1(2,-2,-2,3,eliminate_all=True).ae(0.25)
     assert hyp2f1(2,-2,-3,3) == 14
     assert hyp2f1(2,-3,-2,3) == inf
@@ -586,37 +580,35 @@
     assert hyper([1,2.79,3.08,4.37],[5.2,6.1,7.3],5).ae(1.0996321464692607231-1.7748052293979985001j)
     assert hyper([1,1,1],[1,2],1) == inf
     assert hyper([1,1,1],[2,(101,100)],1).ae(100.01621213528313220)
     # slow -- covered by doctests
     #assert hyper([1,1,1],[2,3],0.9999).ae(1.2897972005319693905)
 
 def test_hyper_u():
-    mp.dps = 15
     assert hyperu(2,-3,0).ae(0.05)
     assert hyperu(2,-3.5,0).ae(4./99)
     assert hyperu(2,0,0) == 0.5
     assert hyperu(-5,1,0) == -120
     assert hyperu(-5,2,0) == inf
     assert hyperu(-5,-2,0) == 0
-    assert hyperu(7,7,3).ae(0.00014681269365593503986)  #exp(3)*gammainc(-6,3)
+    assert hyperu(7,7,3).ae(0.00014681269365593503986)  #exp(3)*upper_gamma(-6,3)
     assert hyperu(2,-3,4).ae(0.011836478100271995559)
     assert hyperu(3,4,5).ae(1./125)
     assert hyperu(2,3,0.0625) == 256
     assert hyperu(-1,2,0.25+0.5j) == -1.75+0.5j
     assert hyperu(0.5,1.5,7.25).ae(2/sqrt(29))
     assert hyperu(2,6,pi).ae(0.55804439825913399130)
     assert (hyperu((3,2),8,100+201j)*10**4).ae(-0.3797318333856738798 - 2.9974928453561707782j)
     assert (hyperu((5,2),(-1,2),-5000)*10**10).ae(-5.6681877926881664678j)
     # XXX: fails because of undetected cancellation in low level series code
     # Alternatively: could use asymptotic series here, if convergence test
     # tweaked back to recognize this one
     #assert (hyperu((5,2),(-1,2),-500)*10**7).ae(-1.82526906001593252847j)
 
 def test_hyper_2f0():
-    mp.dps = 15
     assert hyper([1,2],[],3) == hyp2f0(1,2,3)
     assert hyp2f0(2,3,7).ae(0.0116108068639728714668 - 0.0073727413865865802130j)
     assert hyp2f0(2,3,0) == 1
     assert hyp2f0(0,0,0) == 1
     assert hyp2f0(-1,-1,1).ae(2)
     assert hyp2f0(-4,1,1.5).ae(62.5)
     assert hyp2f0(-4,1,50).ae(147029801)
@@ -627,18 +619,18 @@
     assert hyp2f0((1,6),(5,6),-0.02371708245126284498).ae(0.996785723120804309)
     # Should be exact; polynomial case
     assert hyp2f0(-2,1,0.5+0.5j,zeroprec=200) == 0
     assert hyp2f0(1,-2,0.5+0.5j,zeroprec=200) == 0
     # There used to be a bug in thresholds that made one of the following hang
     for d in [15, 50, 80]:
         mp.dps = d
-        assert hyp2f0(1.5, 0.5, 0.009).ae('1.006867007239309717945323585695344927904000945829843527398772456281301440034218290443367270629519483 + 1.238277162240704919639384945859073461954721356062919829456053965502443570466701567100438048602352623e-46j')
+        assert hyp2f0(1.5, 0.5, 0.009).ae('1.006867007239309717945323585695344927904000945829843527398772456281301440034218290443367270629519483 +'
+                                          ' 1.238277162240704919639384945859073461954721356062919829456053965502443570466701567100438048602352623e-46j')
 
 def test_hyper_1f2():
-    mp.dps = 15
     assert hyper([1],[2,3],4) == hyp1f2(1,2,3,4)
     a1,b1,b2 = (1,10),(2,3),1./16
     assert hyp1f2(a1,b1,b2,10).ae(298.7482725554557568)
     assert hyp1f2(a1,b1,b2,100).ae(224128961.48602947604)
     assert hyp1f2(a1,b1,b2,1000).ae(1.1669528298622675109e+27)
     assert hyp1f2(a1,b1,b2,10000).ae(2.4780514622487212192e+86)
     assert hyp1f2(a1,b1,b2,100000).ae(1.3885391458871523997e+274)
@@ -653,15 +645,14 @@
     assert hyp1f2(a1,b1,b2,100000*j).ae(2.6398091437239324225e+193 + 4.1658080666870618332e+193j)
     assert hyp1f2(a1,b1,b2,1000000*j).ae('3.5999042951925965458e+613 + 1.5026014707128947992e+613j')
     assert hyp1f2(a1,b1,b2,10**7*j).ae('-8.3208715051623234801e+1939 - 3.6752883490851869429e+1941j')
     assert hyp1f2(a1,b1,b2,10**8*j).ae('2.0724195707891484454e+6140 - 1.3276619482724266387e+6141j')
     assert hyp1f2(a1,b1,b2,10**20*j).ae('-1.1734497974795488504e+6141851462 + 1.1498106965385471542e+6141851462j')
 
 def test_hyper_2f3():
-    mp.dps = 15
     assert hyper([1,2],[3,4,5],6) == hyp2f3(1,2,3,4,5,6)
     a1,a2,b1,b2,b3 = (1,10),(2,3),(3,10), 2, 1./16
     # Check asymptotic expansion
     assert hyp2f3(a1,a2,b1,b2,b3,10).ae(128.98207160698659976)
     assert hyp2f3(a1,a2,b1,b2,b3,1000).ae(6.6309632883131273141e25)
     assert hyp2f3(a1,a2,b1,b2,b3,10000).ae(4.6863639362713340539e84)
     assert hyp2f3(a1,a2,b1,b2,b3,100000).ae(8.6632451236103084119e271)
@@ -676,24 +667,22 @@
     assert hyp2f3(a1,a2,b1,b2,b3,100000*j).ae(2.9844228969804380301e+191 + 7.5587163231490273296e+190j)
     assert hyp2f3(a1,a2,b1,b2,b3,1000000*j).ae('7.4859161049322370311e+610 - 2.8467477015940090189e+610j')
     assert hyp2f3(a1,a2,b1,b2,b3,10**7*j).ae('-1.7477645579418800826e+1938 - 1.7606522995808116405e+1938j')
     assert hyp2f3(a1,a2,b1,b2,b3,10**8*j).ae('-1.6932731942958401784e+6137 - 2.4521909113114629368e+6137j')
     assert hyp2f3(a1,a2,b1,b2,b3,10**20*j).ae('-2.0988815677627225449e+6141851451 + 5.7708223542739208681e+6141851452j')
 
 def test_hyper_2f2():
-    mp.dps = 15
     assert hyper([1,2],[3,4],5) == hyp2f2(1,2,3,4,5)
     a1,a2,b1,b2 = (3,10),4,(1,2),1./16
     assert hyp2f2(a1,a2,b1,b2,10).ae(448225936.3377556696)
     assert hyp2f2(a1,a2,b1,b2,10000).ae('1.2012553712966636711e+4358')
     assert hyp2f2(a1,a2,b1,b2,-20000).ae(-0.04182343755661214626)
     assert hyp2f2(a1,a2,b1,b2,10**20).ae('1.1148680024303263661e+43429448190325182840')
 
 def test_orthpoly():
-    mp.dps = 15
     assert jacobi(-4,2,3,0.7).ae(22800./4913)
     assert jacobi(3,2,4,5.5) == 4133.125
     assert jacobi(1.5,5/6.,4,0).ae(-1.0851951434075508417)
     assert jacobi(-2, 1, 2, 4).ae(-0.16)
     assert jacobi(2, -1, 2.5, 4).ae(34.59375)
     #assert jacobi(2, -1, 2, 4) == 28.5
     assert legendre(5, 7) == 129367
@@ -704,23 +693,24 @@
     assert legendre(1, -1) == -1
     assert legendre(7, 1) == 1
     assert legendre(7, -1) == -1
     assert legendre(8,1.5).ae(15457523./32768)
     assert legendre(j,-j).ae(2.4448182735671431011 + 0.6928881737669934843j)
     assert chebyu(5,1) == 6
     assert chebyt(3,2) == 26
+    assert chebyu(5,inf) == inf  # issue 469
+    assert chebyt(5,inf) == inf
     assert legendre(3.5,-1) == inf
     assert legendre(4.5,-1) == -inf
     assert legendre(3.5+1j,-1) == mpc(inf,inf)
     assert legendre(4.5+1j,-1) == mpc(-inf,-inf)
     assert laguerre(4, -2, 3).ae(-1.125)
     assert laguerre(3, 1+j, 0.5).ae(0.2291666666666666667 + 2.5416666666666666667j)
 
 def test_hermite():
-    mp.dps = 15
     assert hermite(-2, 0).ae(0.5)
     assert hermite(-1, 0).ae(0.88622692545275801365)
     assert hermite(0, 0).ae(1)
     assert hermite(1, 0) == 0
     assert hermite(2, 0).ae(-2)
     assert hermite(0, 2).ae(1)
     assert hermite(1, 2).ae(4)
@@ -743,29 +733,34 @@
     assert hermite(-9.5, 100).ae(1.3776300722767084162e-22, abs_eps=0, rel_eps=eps)
     assert hermite(-9.5, -100).ae('1.3106082028470671626e4355')
     assert hermite(-9.5, 100j).ae(-9.7900218581864768430e-23 - 9.7900218581864768430e-23j, abs_eps=0, rel_eps=eps)
     assert hermite(-9.5, -100j).ae(-9.7900218581864768430e-23 + 9.7900218581864768430e-23j, abs_eps=0, rel_eps=eps)
     assert hermite(2+3j, -1-j).ae(851.3677063883687676 - 1496.4373467871007997j)
 
 def test_gegenbauer():
-    mp.dps = 15
     assert gegenbauer(1,2,3).ae(12)
     assert gegenbauer(2,3,4).ae(381)
     assert gegenbauer(0,0,0) == 0
     assert gegenbauer(2,-1,3) == 0
     assert gegenbauer(-7, 0.5, 3).ae(8989)
     assert gegenbauer(1, -0.5, 3).ae(-3)
     assert gegenbauer(1, -1.5, 3).ae(-9)
     assert gegenbauer(1, -0.5, 3).ae(-3)
     assert gegenbauer(-0.5, -0.5, 3).ae(-2.6383553159023906245)
     assert gegenbauer(2+3j, 1-j, 3+4j).ae(14.880536623203696780 + 20.022029711598032898j)
     #assert gegenbauer(-2, -0.5, 3).ae(-12)
+    assert gegenbauer(0, 0, 2.2) == 0  # issue 494
+    assert gegenbauer(0, 1, 2.2) == 1
+    assert gegenbauer(0, 4, 2.2) == 1
+    assert gegenbauer(0, 0, 1.8) == 0
+    assert gegenbauer(0, 1, 1.8) == 1
+    mp.dps = 200
+    assert gegenbauer(2,-1.0, 27397079.00297188) == 0  # issue 461
 
 def test_legenp():
-    mp.dps = 15
     assert legenp(2,0,4) == legendre(2,4)
     assert legenp(-2, -1, 0.5).ae(0.43301270189221932338)
     assert legenp(-2, -1, 0.5, type=3).ae(0.43301270189221932338j)
     assert legenp(-2, 1, 0.5).ae(-0.86602540378443864676)
     assert legenp(2+j, 3+4j, -j).ae(134742.98773236786148 + 429782.72924463851745j)
     assert legenp(2+j, 3+4j, -j, type=3).ae(802.59463394152268507 - 251.62481308942906447j)
     assert legenp(2,4,3).ae(0)
@@ -777,15 +772,14 @@
     assert legenp(3,4,3).ae(0)
     assert legenp(0,0.5,2).ae(0.52503756790433198939 - 0.52503756790433198939j)
     assert legenp(-1,-0.5,2).ae(0.60626116232846498110 + 0.60626116232846498110j)
     assert legenp(-2,0.5,2).ae(1.5751127037129959682 - 1.5751127037129959682j)
     assert legenp(-2,0.5,-0.5).ae(-0.85738275810499171286)
 
 def test_legenq():
-    mp.dps = 15
     f = legenq
     # Evaluation at poles
     assert isnan(f(3,2,1))
     assert isnan(f(3,2,-1))
     assert isnan(f(3,2,1,type=3))
     assert isnan(f(3,2,-1,type=3))
     # Evaluation at 0
@@ -837,78 +831,76 @@
     assert f(-2.5,1,-1.5,type=3).ae(0.29932356550447017254j)
     assert f(-2.5,1,-0.5,type=3).ae(-0.3158481299074220287 - 1.9290561746445456908j)
     assert f(-2.5,1,0,type=3).ae(1.2708196271909686292 - 1.2708196271909686299j)
     assert f(-2.5,1,0.5,type=3).ae(1.9290561746445456907 + 0.3158481299074220287j)
     assert f(-2.5,1,1.5,type=3).ae(-0.29932356550447017254)
 
 def test_agm():
-    mp.dps = 15
     assert agm(0,0) == 0
     assert agm(0,1) == 0
     assert agm(1,1) == 1
     assert agm(7,7) == 7
     assert agm(j,j) == j
     assert (1/agm(1,sqrt(2))).ae(0.834626841674073186)
     assert agm(1,2).ae(1.4567910310469068692)
     assert agm(1,3).ae(1.8636167832448965424)
     assert agm(1,j).ae(0.599070117367796104+0.599070117367796104j)
     assert agm(2) == agm(1,2)
     assert agm(-3,4).ae(0.63468509766550907+1.3443087080896272j)
 
 def test_gammainc():
-    mp.dps = 15
-    assert gammainc(2,5).ae(6*exp(-5))
-    assert gammainc(2,0,5).ae(1-6*exp(-5))
+    assert upper_gamma(2,5).ae(6*exp(-5))
+    assert lower_gamma(2,5).ae(1-6*exp(-5))
     assert gammainc(2,3,5).ae(-6*exp(-5)+4*exp(-3))
-    assert gammainc(-2.5,-0.5).ae(-0.9453087204829418812-5.3164237738936178621j)
+    assert upper_gamma(-2.5,-0.5).ae(-0.9453087204829418812-5.3164237738936178621j)
     assert gammainc(0,2,4).ae(0.045121158298212213088)
-    assert gammainc(0,3).ae(0.013048381094197037413)
+    assert upper_gamma(0,3).ae(0.013048381094197037413)
     assert gammainc(0,2+j,1-j).ae(0.00910653685850304839-0.22378752918074432574j)
-    assert gammainc(0,1-j).ae(0.00028162445198141833+0.17932453503935894015j)
+    assert upper_gamma(0,1-j).ae(0.00028162445198141833+0.17932453503935894015j)
     assert gammainc(3,4,5,True).ae(0.11345128607046320253)
-    assert gammainc(3.5,0,inf).ae(gamma(3.5))
-    assert gammainc(-150.5,500).ae('6.9825435345798951153e-627')
-    assert gammainc(-150.5,800).ae('4.6885137549474089431e-788')
-    assert gammainc(-3.5, -20.5).ae(0.27008820585226911 - 1310.31447140574997636j)
-    assert gammainc(-3.5, -200.5).ae(0.27008820585226911 - 5.3264597096208368435e76j) # XXX real part
-    assert gammainc(0,0,2) == inf
+    assert gammainc(3.5,0).ae(gamma(3.5))
+    assert upper_gamma(-150.5,500).ae('6.9825435345798951153e-627')
+    assert upper_gamma(-150.5,800).ae('4.6885137549474089431e-788')
+    assert upper_gamma(-3.5,-20.5).ae(0.27008820585226911 - 1310.31447140574997636j)
+    assert upper_gamma(-3.5,-200.5).ae(0.27008820585226911 - 5.3264597096208368435e76j) # XXX real part
+    assert lower_gamma(0,2) == inf
     assert gammainc(1,b=1).ae(0.6321205588285576784)
     assert gammainc(3,2,2) == 0
     assert gammainc(2,3+j,3-j).ae(-0.28135485191849314194j)
-    assert gammainc(4+0j,1).ae(5.8860710587430771455)
+    assert upper_gamma(4+0j,1).ae(5.8860710587430771455)
     # GH issue #301
-    assert gammainc(-1,-1).ae(-0.8231640121031084799 + 3.1415926535897932385j)
-    assert gammainc(-2,-1).ae(1.7707229202810768576 - 1.5707963267948966192j)
-    assert gammainc(-3,-1).ae(-1.4963349162467073643 + 0.5235987755982988731j)
-    assert gammainc(-4,-1).ae(1.05365418617643814992 - 0.13089969389957471827j)
+    assert upper_gamma(-1,-1).ae(-0.8231640121031084799 + 3.1415926535897932385j)
+    assert upper_gamma(-2,-1).ae(1.7707229202810768576 - 1.5707963267948966192j)
+    assert upper_gamma(-3,-1).ae(-1.4963349162467073643 + 0.5235987755982988731j)
+    assert upper_gamma(-4,-1).ae(1.05365418617643814992 - 0.13089969389957471827j)
     # Regularized upper gamma
     assert isnan(gammainc(0, 0, regularized=True))
     assert gammainc(-1, 0, regularized=True) == inf
     assert gammainc(1, 0, regularized=True) == 1
-    assert gammainc(0, 5, regularized=True) == 0
-    assert gammainc(0, 2+3j, regularized=True) == 0
-    assert gammainc(0, 5000, regularized=True) == 0
+    assert upper_gamma(0,5, regularized=True) == 0
+    assert upper_gamma(0,2+3j, regularized=True) == 0
+    assert upper_gamma(0,5000, regularized=True) == 0
     assert gammainc(0, 10**30, regularized=True) == 0
     assert gammainc(-1, 5, regularized=True) == 0
     assert gammainc(-1, 5000, regularized=True) == 0
     assert gammainc(-1, 10**30, regularized=True) == 0
     assert gammainc(-1, -5, regularized=True) == 0
     assert gammainc(-1, -5000, regularized=True) == 0
     assert gammainc(-1, -10**30, regularized=True) == 0
     assert gammainc(-1, 3+4j, regularized=True) == 0
-    assert gammainc(1, 5, regularized=True).ae(exp(-5))
-    assert gammainc(1, 5000, regularized=True).ae(exp(-5000))
+    assert upper_gamma(1,5, regularized=True).ae(exp(-5))
+    assert upper_gamma(1,5000, regularized=True).ae(exp(-5000))
     assert gammainc(1, 10**30, regularized=True).ae(exp(-10**30))
-    assert gammainc(1, 3+4j, regularized=True).ae(exp(-3-4j))
-    assert gammainc(-1000000,2).ae('1.3669297209397347754e-301037', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(1,3+4j, regularized=True).ae(exp(-3-4j))
+    assert upper_gamma(-1000000,2).ae('1.3669297209397347754e-301037', abs_eps=0, rel_eps=8*eps)
     assert gammainc(-1000000,2,regularized=True) == 0
-    assert gammainc(-1000000,3+4j).ae('-1.322575609404222361e-698979 - 4.9274570591854533273e-698978j', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(-1000000,3+4j).ae('-1.322575609404222361e-698979 - 4.9274570591854533273e-698978j', abs_eps=0, rel_eps=8*eps)
     assert gammainc(-1000000,3+4j,regularized=True) == 0
-    assert gammainc(2+3j, 4+5j, regularized=True).ae(0.085422013530993285774-0.052595379150390078503j)
-    assert gammainc(1000j, 1000j, regularized=True).ae(0.49702647628921131761 + 0.00297355675013575341j)
+    assert upper_gamma(2+3j,4+5j, regularized=True).ae(0.085422013530993285774-0.052595379150390078503j)
+    assert upper_gamma(1000j,1000j, regularized=True).ae(0.49702647628921131761 + 0.00297355675013575341j)
     # Generalized
     assert gammainc(3,4,2) == -gammainc(3,2,4)
     assert gammainc(4, 2, 3).ae(1.2593494302978947396)
     assert gammainc(4, 2, 3, regularized=True).ae(0.20989157171631578993)
     assert gammainc(0, 2, 3).ae(0.035852129613864082155)
     assert gammainc(0, 2, 3, regularized=True) == 0
     assert gammainc(-1, 2, 3).ae(0.015219822548487616132)
@@ -916,27 +908,26 @@
     assert gammainc(0, 2, 3).ae(0.035852129613864082155)
     assert gammainc(0, 2, 3, regularized=True) == 0
     # Should use upper gammas
     assert gammainc(5, 10000, 12000).ae('1.1359381951461801687e-4327', abs_eps=0, rel_eps=8*eps)
     # Should use lower gammas
     assert gammainc(10000, 2, 3).ae('8.1244514125995785934e4765')
     # GH issue 306
-    assert gammainc(3,-1-1j) == 0
-    assert gammainc(3,-1+1j) == 0
-    assert gammainc(2,-1) == 0
-    assert gammainc(2,-1+0j) == 0
-    assert gammainc(2+0j,-1) == 0
+    assert upper_gamma(3,-1-1j) == 0
+    assert upper_gamma(3,-1+1j) == 0
+    assert upper_gamma(2,-1) == 0
+    assert upper_gamma(2,-1+0j) == 0
+    assert upper_gamma(2+0j,-1) == 0
 
 def test_gammainc_expint_n():
     # These tests are intended to check all cases of the low-level code
     # for upper gamma and expint with small integer index.
     # Need to cover positive/negative arguments; small/large/huge arguments
     # for both positive and negative indices, as well as indices 0 and 1
     # which may be special-cased
-    mp.dps = 15
     assert expint(-3,3.5).ae(0.021456366563296693987)
     assert expint(-2,3.5).ae(0.014966633183073309405)
     assert expint(-1,3.5).ae(0.011092916359219041088)
     assert expint(0,3.5).ae(0.0086278238349481430685)
     assert expint(1,3.5).ae(0.0069701398575483929193)
     assert expint(2,3.5).ae(0.0058018939208991255223)
     assert expint(3,3.5).ae(0.0049453773495857807058)
@@ -984,91 +975,89 @@
     u = expint(2,-350000000000000000000000)
     assert u.imag.ae(-1.0995574287564276335e+24)
     assert u.ae('-3.7805306852415755699e+152003068666138139677871')
     u = expint(3,-350000000000000000000000)
     assert u.imag.ae(-1.9242255003237483586e+47)
     assert u.ae('-3.7805306852415755699e+152003068666138139677871')
     # Small case; no branch cut
-    assert gammainc(-3,3.5).ae(0.00010020262545203707109)
-    assert gammainc(-2,3.5).ae(0.00040370427343557393517)
-    assert gammainc(-1,3.5).ae(0.0016576839773997501492)
-    assert gammainc(0,3.5).ae(0.0069701398575483929193)
-    assert gammainc(1,3.5).ae(0.03019738342231850074)
-    assert gammainc(2,3.5).ae(0.13588822540043325333)
-    assert gammainc(3,3.5).ae(0.64169439772426814072)
+    assert upper_gamma(-3,3.5).ae(0.00010020262545203707109)
+    assert upper_gamma(-2,3.5).ae(0.00040370427343557393517)
+    assert upper_gamma(-1,3.5).ae(0.0016576839773997501492)
+    assert upper_gamma(0,3.5).ae(0.0069701398575483929193)
+    assert upper_gamma(1,3.5).ae(0.03019738342231850074)
+    assert upper_gamma(2,3.5).ae(0.13588822540043325333)
+    assert upper_gamma(3,3.5).ae(0.64169439772426814072)
     # Small case; with branch cut
-    assert gammainc(-3,-3.5).ae(0.03595832954467563286 + 0.52359877559829887308j)
-    assert gammainc(-2,-3.5).ae(-0.88024704597962022221 - 1.5707963267948966192j)
-    assert gammainc(-1,-3.5).ae(4.4637962926688170771 + 3.1415926535897932385j)
-    assert gammainc(0,-3.5).ae(-13.925353995152335292 - 3.1415926535897932385j)
-    assert gammainc(1,-3.5).ae(33.115451958692313751)
-    assert gammainc(2,-3.5).ae(-82.788629896730784377)
-    assert gammainc(3,-3.5).ae(240.08702670051927469)
+    assert upper_gamma(-3,-3.5).ae(0.03595832954467563286 + 0.52359877559829887308j)
+    assert upper_gamma(-2,-3.5).ae(-0.88024704597962022221 - 1.5707963267948966192j)
+    assert upper_gamma(-1,-3.5).ae(4.4637962926688170771 + 3.1415926535897932385j)
+    assert upper_gamma(0,-3.5).ae(-13.925353995152335292 - 3.1415926535897932385j)
+    assert upper_gamma(1,-3.5).ae(33.115451958692313751)
+    assert upper_gamma(2,-3.5).ae(-82.788629896730784377)
+    assert upper_gamma(3,-3.5).ae(240.08702670051927469)
     # Asymptotic case; no branch cut
-    assert gammainc(-3,350).ae(6.5424095113340358813e-163, abs_eps=0, rel_eps=8*eps)
-    assert gammainc(-2,350).ae(2.296312222489899769e-160, abs_eps=0, rel_eps=8*eps)
-    assert gammainc(-1,350).ae(8.059861834133858573e-158, abs_eps=0, rel_eps=8*eps)
-    assert gammainc(0,350).ae(2.8289659656701459404e-155, abs_eps=0, rel_eps=8*eps)
-    assert gammainc(1,350).ae(9.9295903962649792963e-153, abs_eps=0, rel_eps=8*eps)
-    assert gammainc(2,350).ae(3.485286229089007733e-150, abs_eps=0, rel_eps=8*eps)
-    assert gammainc(3,350).ae(1.2233453960006379793e-147, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(-3,350).ae(6.5424095113340358813e-163, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(-2,350).ae(2.296312222489899769e-160, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(-1,350).ae(8.059861834133858573e-158, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(0,350).ae(2.8289659656701459404e-155, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(1,350).ae(9.9295903962649792963e-153, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(2,350).ae(3.485286229089007733e-150, abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(3,350).ae(1.2233453960006379793e-147, abs_eps=0, rel_eps=8*eps)
     # Asymptotic case; branch cut
-    u = gammainc(-3,-350)
+    u = upper_gamma(-3,-350)
     assert u.ae(6.7889565783842895085e+141)
     assert u.imag.ae(0.52359877559829887308)
-    u = gammainc(-2,-350)
+    u = upper_gamma(-2,-350)
     assert u.ae(-2.3692668977889832121e+144)
     assert u.imag.ae(-1.5707963267948966192)
-    u = gammainc(-1,-350)
+    u = upper_gamma(-1,-350)
     assert u.ae(8.2685354361441858669e+146)
     assert u.imag.ae(3.1415926535897932385)
-    u = gammainc(0,-350)
+    u = upper_gamma(0,-350)
     assert u.ae(-2.8856710698020863568e+149)
     assert u.imag.ae(-3.1415926535897932385)
-    u = gammainc(1,-350)
+    u = upper_gamma(1,-350)
     assert u.ae(1.0070908870280797598e+152)
     assert u.imag == 0
-    u = gammainc(2,-350)
+    u = upper_gamma(2,-350)
     assert u.ae(-3.5147471957279983618e+154)
     assert u.imag == 0
-    u = gammainc(3,-350)
+    u = upper_gamma(3,-350)
     assert u.ae(1.2266568422179417091e+157)
     assert u.imag == 0
     # Extreme asymptotic case
-    assert gammainc(-3,350000000000000000000000).ae('5.0362468738874738859e-152003068666138139677990', abs_eps=0, rel_eps=8*eps)
-    assert gammainc(-2,350000000000000000000000).ae('1.7626864058606158601e-152003068666138139677966', abs_eps=0, rel_eps=8*eps)
-    assert gammainc(-1,350000000000000000000000).ae('6.1694024205121555102e-152003068666138139677943', abs_eps=0, rel_eps=8*eps)
-    assert gammainc(0,350000000000000000000000).ae('2.1592908471792544286e-152003068666138139677919', abs_eps=0, rel_eps=8*eps)
-    assert gammainc(1,350000000000000000000000).ae('7.5575179651273905e-152003068666138139677896', abs_eps=0, rel_eps=8*eps)
-    assert gammainc(2,350000000000000000000000).ae('2.645131287794586675e-152003068666138139677872', abs_eps=0, rel_eps=8*eps)
-    assert gammainc(3,350000000000000000000000).ae('9.2579595072810533625e-152003068666138139677849', abs_eps=0, rel_eps=8*eps)
-    u = gammainc(-3,-350000000000000000000000)
+    assert upper_gamma(-3,350000000000000000000000).ae('5.0362468738874738859e-152003068666138139677990', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(-2,350000000000000000000000).ae('1.7626864058606158601e-152003068666138139677966', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(-1,350000000000000000000000).ae('6.1694024205121555102e-152003068666138139677943', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(0,350000000000000000000000).ae('2.1592908471792544286e-152003068666138139677919', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(1,350000000000000000000000).ae('7.5575179651273905e-152003068666138139677896', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(2,350000000000000000000000).ae('2.645131287794586675e-152003068666138139677872', abs_eps=0, rel_eps=8*eps)
+    assert upper_gamma(3,350000000000000000000000).ae('9.2579595072810533625e-152003068666138139677849', abs_eps=0, rel_eps=8*eps)
+    u = upper_gamma(-3,-350000000000000000000000)
     assert u.ae('8.8175642804468234866e+152003068666138139677800')
     assert u.imag.ae(0.52359877559829887308)
-    u = gammainc(-2,-350000000000000000000000)
+    u = upper_gamma(-2,-350000000000000000000000)
     assert u.ae('-3.0861474981563882203e+152003068666138139677824')
     assert u.imag.ae(-1.5707963267948966192)
-    u = gammainc(-1,-350000000000000000000000)
+    u = upper_gamma(-1,-350000000000000000000000)
     assert u.ae('1.0801516243547358771e+152003068666138139677848')
     assert u.imag.ae(3.1415926535897932385)
-    u = gammainc(0,-350000000000000000000000)
+    u = upper_gamma(0,-350000000000000000000000)
     assert u.ae('-3.7805306852415755699e+152003068666138139677871')
     assert u.imag.ae(-3.1415926535897932385)
-    assert gammainc(1,-350000000000000000000000).ae('1.3231857398345514495e+152003068666138139677895')
-    assert gammainc(2,-350000000000000000000000).ae('-4.6311500894209300731e+152003068666138139677918')
-    assert gammainc(3,-350000000000000000000000).ae('1.6209025312973255256e+152003068666138139677942')
+    assert upper_gamma(1,-350000000000000000000000).ae('1.3231857398345514495e+152003068666138139677895')
+    assert upper_gamma(2,-350000000000000000000000).ae('-4.6311500894209300731e+152003068666138139677918')
+    assert upper_gamma(3,-350000000000000000000000).ae('1.6209025312973255256e+152003068666138139677942')
 
 def test_incomplete_beta():
-    mp.dps = 15
     assert betainc(-2,-3,0.5,0.75).ae(63.4305673311255413583969)
     assert betainc(4.5,0.5+2j,2.5,6).ae(0.2628801146130621387903065 + 0.5162565234467020592855378j)
     assert betainc(4,5,0,6).ae(90747.77142857142857142857)
 
 def test_erf():
-    mp.dps = 15
     assert erf(0) == 0
     assert erf(1).ae(0.84270079294971486934)
     assert erf(3+4j).ae(-120.186991395079444098 - 27.750337293623902498j)
     assert erf(-4-3j).ae(-0.99991066178539168236 + 0.00004972026054496604j)
     assert erf(pi).ae(0.99999112385363235839)
     assert erf(1j).ae(1.6504257587975428760j)
     assert erf(-1j).ae(-1.6504257587975428760j)
@@ -1123,29 +1112,27 @@
     assert v.real == 1
     assert v.imag.ae('-6.1481820666053078736e+1083')
     assert erfc(-100+5j).ae(2)
     assert (erfc(100+5j)*10**4335).ae(2.3973567853824133572 - 3.9339259530609420597j)
     assert erfc(100+100j).ae(0.00065234366376857698698 - 0.0039357263629214118437j)
 
 def test_pdf():
-    mp.dps = 15
     assert npdf(-inf) == 0
     assert npdf(inf) == 0
     assert npdf(5,0,2).ae(npdf(5+4,4,2))
     assert quadts(lambda x: npdf(x,-0.5,0.8), [-inf, inf]) == 1
     assert ncdf(0) == 0.5
     assert ncdf(3,3) == 0.5
     assert ncdf(-inf) == 0
     assert ncdf(inf) == 1
     assert ncdf(10) == 1
     # Verify that this is computed accurately
     assert (ncdf(-10)*10**24).ae(7.619853024160526)
 
 def test_lambertw():
-    mp.dps = 15
     assert lambertw(0) == 0
     assert lambertw(0+0j) == 0
     assert lambertw(inf) == inf
     assert isnan(lambertw(nan))
     assert lambertw(inf,1).real == inf
     assert lambertw(inf,1).imag.ae(2*pi)
     assert lambertw(-inf,1).real == inf
@@ -1332,15 +1319,14 @@
     assert lambertw(x).ae(ans)
     mp.dps = 50
     assert lambertw(x).ae(ans)
     mp.dps = 150
     assert lambertw(x).ae(ans)
 
 def test_meijerg():
-    mp.dps = 15
     assert meijerg([[2,3],[1]],[[0.5,2],[3,4]], 2.5).ae(4.2181028074787439386)
     assert meijerg([[],[1+j]],[[1],[1]], 3+4j).ae(271.46290321152464592 - 703.03330399954820169j)
     assert meijerg([[0.25],[1]],[[0.5],[2]],0) == 0
     assert meijerg([[0],[]],[[0,0,'1/3','2/3'], []], '2/27').ae(2.2019391389653314120)
     # Verify 1/z series being used
     assert meijerg([[-3],[-0.5]], [[-1],[-2.5]], -0.5).ae(-1.338096165935754898687431)
     assert meijerg([[1-(-1)],[1-(-2.5)]], [[1-(-3)],[1-(-0.5)]], -2.0).ae(-1.338096165935754898687431)
@@ -1351,41 +1337,41 @@
         x1 = hyp1f1(a,b,z)
         x2 = gamma(b)/gamma(a)*meijerg([[1-a],[]],[[0],[1-b]],-z)
         x3 = gamma(b)/gamma(a)*meijerg([[1-0],[1-(1-b)]],[[1-(1-a)],[]],-1/z)
         assert x1.ae(x2)
         assert x1.ae(x3)
 
 def test_appellf1():
-    mp.dps = 15
     assert appellf1(2,-2,1,1,2,3).ae(-1.75)
     assert appellf1(2,1,-2,1,2,3).ae(-8)
     assert appellf1(2,1,-2,1,0.5,0.25).ae(1.5)
     assert appellf1(-2,1,3,2,3,3).ae(19)
     assert appellf1(1,2,3,4,0.5,0.125).ae( 1.53843285792549786518)
 
 def test_coulomb():
     # Note: most tests are doctests
     # Test for a bug:
-    mp.dps = 15
     assert coulombg(mpc(-5,0),2,3).ae(20.087729487721430394)
 
 def test_hyper_param_accuracy():
-    mp.dps = 15
     As = [n+1e-10 for n in range(-5,-1)]
     Bs = [n+1e-10 for n in range(-12,-5)]
     assert hyper(As,Bs,10).ae(-381757055858.652671927)
     assert legenp(0.5, 100, 0.25).ae(-2.4124576567211311755e+144)
     assert (hyp1f1(1000,1,-100)*10**24).ae(5.2589445437370169113)
     assert (hyp2f1(10, -900, 10.5, 0.99)*10**24).ae(1.9185370579660768203)
     assert (hyp2f1(1000,1.5,-3.5,-1.5)*10**385).ae(-2.7367529051334000764)
     assert hyp2f1(-5, 10, 3, 0.5, zeroprec=500) == 0
     assert (hyp1f1(-10000, 1000, 100)*10**424).ae(-3.1046080515824859974)
     assert (hyp2f1(1000,1.5,-3.5,-0.75,maxterms=100000)*10**231).ae(-4.0534790813913998643)
+    assert (hyp2f1(1000,1.5,-3.5,-0.75,maxterms=10000)*10**231).ae(-4.0534790813913998643)
+    pytest.raises(mp.NoConvergence, lambda: mp.hyp2f1(1000,1.5,-3.5,-0.75,maxterms=10000,force_series=True))
+    pytest.raises(fp.NoConvergence, lambda: fp.hyp2f1(1000,1.5,-3.5,-0.75,maxterms=10000,force_series=True))
     assert legenp(2, 3, 0.25) == 0
-    pytest.raises(ValueError, lambda: hypercomb(lambda a: [([],[],[],[],[a],[-a],0.5)], [3]))
+    pytest.raises(mp.NoConvergence, lambda: hypercomb(lambda a: [([],[],[],[],[a],[-a],0.5)], [3]))
     assert hypercomb(lambda a: [([],[],[],[],[a],[-a],0.5)], [3], infprec=200) == inf
     assert meijerg([[],[]],[[0,0,0,0],[]],0.1).ae(1.5680822343832351418)
     assert (besselk(400,400)*10**94).ae(1.4387057277018550583)
     mp.dps = 5
     (hyp1f1(-5000.5, 1500, 100)*10**185).ae(8.5185229673381935522)
     (hyp1f1(-5000, 1500, 100)*10**185).ae(9.1501213424563944311)
     mp.dps = 15
@@ -1396,15 +1382,14 @@
 
 def test_hypercomb_zero_pow():
     # check that 0^0 = 1
     assert hypercomb(lambda a: (([0],[a],[],[],[],[],0),), [0]) == 1
     assert meijerg([[-1.5],[]],[[0],[-0.75]],0).ae(1.4464090846320771425)
 
 def test_spherharm():
-    mp.dps = 15
     t = 0.5; r = 0.25
     assert spherharm(0,0,t,r).ae(0.28209479177387814347)
     assert spherharm(1,-1,t,r).ae(0.16048941205971996369 - 0.04097967481096344271j)
     assert spherharm(1,0,t,r).ae(0.42878904414183579379)
     assert spherharm(1,1,t,r).ae(-0.16048941205971996369 - 0.04097967481096344271j)
     assert spherharm(2,-2,t,r).ae(0.077915886919031181734 - 0.042565643022253962264j)
     assert spherharm(2,-1,t,r).ae(0.31493387233497459884 - 0.08041582001959297689j)
@@ -1438,15 +1423,14 @@
     assert spherharm(-6, 3, 0.5, 0.25).ae(-0.16544349818782275459 - 0.15412657723253924562j)
     assert spherharm(-6, 1.5, 0.5, 0.25).ae(0.032208193499767402477 + 0.012678000924063664921j)
     assert spherharm(3,0,0,1).ae(0.74635266518023078283)
     assert spherharm(3,-2,0,1) == 0
     assert spherharm(3,-2,1,1).ae(-0.16270707338254028971 - 0.35552144137546777097j)
 
 def test_qfunctions():
-    mp.dps = 15
     assert qp(2,3,100).ae('2.7291482267247332183e2391')
 
 def test_issue_239():
     mp.prec = 150
     x = ldexp(2476979795053773,-52)
     assert betainc(206, 385, 0, 0.55, 1).ae('0.99999999999999999999996570910644857895771110649954')
     mp.dps = 15
@@ -2365,20 +2349,42 @@
   57.175005343085052,
   60.410169281219877,
   63.635442539153021,
   66.85235358587768]]
 
 @pytest.mark.slow
 def test_bessel_zeros_extra():
-    mp.dps = 15
     for v in range(V):
         for m in range(1,M+1):
             print(v, m, "of", V, M)
             # Twice to test cache (if used)
             assert besseljzero(v,m).ae(jn_small_zeros[v][m-1])
             assert besseljzero(v,m).ae(jn_small_zeros[v][m-1])
             assert besseljzero(v,m,1).ae(jnp_small_zeros[v][m-1])
             assert besseljzero(v,m,1).ae(jnp_small_zeros[v][m-1])
             assert besselyzero(v,m).ae(yn_small_zeros[v][m-1])
             assert besselyzero(v,m).ae(yn_small_zeros[v][m-1])
             assert besselyzero(v,m,1).ae(ynp_small_zeros[v][m-1])
             assert besselyzero(v,m,1).ae(ynp_small_zeros[v][m-1])
+
+def test_issue_569():
+    r = betainc(1, 2, 1, 1)
+    assert isinstance(r, mp.mpf) and r == 0
+
+@pytest.mark.skipif(BACKEND != 'gmpy', reason="gmpy isn't used")
+def test_issue_274():
+    with pytest.raises(ValueError):
+        mp.fraction(1, 100).func(1000, 0xdead)
+
+def test_issue_523():
+    assert mp.hermite(0, inf) == 1.0
+
+def test_issue_512():
+    assert mp.hyperu(0, 1, inf) == 1.0
+    assert mp.hyperu(0, 2, inf) == 1.0
+
+def test_issue_251():
+    assert lerchphi(1.0000000, 4.1+1j,
+                    1.0).ae(1.0497861493928464 - 0.053190918836910267j)
+    assert lerchphi(1.00000001, 4.1+1j,
+                    1.0).ae(1.0497861498996701 - 0.053190919646660638j)
+    assert zeta(4.1+1j, 1.0).ae(1.0497861493928464 - 0.053190918836910267j)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_gammazeta.py` & `mpmath-1.4.0a0/mpmath/tests/test_gammazeta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,69 @@
-from mpmath import *
-from mpmath.libmp import round_up, from_float, mpf_zeta_int
+import pytest
+
+from mpmath import (altzeta, apery, barnesg, bell, bernfrac, bernoulli,
+                    bernpoly, beta, binomial, catalan, digamma, e, euler,
+                    eulerpoly, fac, fac2, factorial, fadd, ff, findroot, fp,
+                    fraction, gamma, gammaprod, harmonic, hyperfac, inf, isnan,
+                    j, log, loggamma, mp, mpc, mpf, mpmathify, nan, pi,
+                    polyexp, polylog, primezeta, psi, rf, rgamma, sech,
+                    siegelz, sinc, sqrt, stieltjes, superfac, zeta)
+from mpmath.libmp import from_float, mpf_zeta_int, round_up
+
 
 def test_zeta_int_bug():
     assert mpf_zeta_int(0, 10) == from_float(-0.5)
 
-def test_bernoulli():
-    assert bernfrac(0) == (1,1)
-    assert bernfrac(1) == (-1,2)
-    assert bernfrac(2) == (1,6)
-    assert bernfrac(3) == (0,1)
-    assert bernfrac(4) == (-1,30)
-    assert bernfrac(5) == (0,1)
-    assert bernfrac(6) == (1,42)
-    assert bernfrac(8) == (-1,30)
-    assert bernfrac(10) == (5,66)
-    assert bernfrac(12) == (-691,2730)
-    assert bernfrac(18) == (43867,798)
-    p, q = bernfrac(228)
+@pytest.mark.parametrize('plus', [True, False])
+def test_bernoulli(plus):
+    assert bernfrac(0, plus) == (1,1)
+    assert bernfrac(1, plus) == (1,2) if plus else (-1,2)
+    assert bernfrac(2, plus) == (1,6)
+    assert bernfrac(3, plus) == (0,1)
+    assert bernfrac(4, plus) == (-1,30)
+    assert bernfrac(5, plus) == (0,1)
+    assert bernfrac(6, plus) == (1,42)
+    assert bernfrac(8, plus) == (-1,30)
+    assert bernfrac(10, plus) == (5,66)
+    assert bernfrac(12, plus) == (-691,2730)
+    assert bernfrac(18, plus) == (43867,798)
+    p, q = bernfrac(228, plus)
     assert p % 10**10 == 164918161
     assert q == 625170
-    p, q = bernfrac(1000)
+    p, q = bernfrac(1000, plus)
     assert p % 10**10 == 7950421099
     assert q == 342999030
     mp.dps = 15
-    assert bernoulli(0) == 1
-    assert bernoulli(1) == -0.5
-    assert bernoulli(2).ae(1./6)
-    assert bernoulli(3) == 0
-    assert bernoulli(4).ae(-1./30)
-    assert bernoulli(5) == 0
-    assert bernoulli(6).ae(1./42)
-    assert str(bernoulli(10)) == '0.0757575757575758'
-    assert str(bernoulli(234)) == '7.62772793964344e+267'
-    assert str(bernoulli(10**5)) == '-5.82229431461335e+376755'
-    assert str(bernoulli(10**8+2)) == '1.19570355039953e+676752584'
-
-    mp.dps = 50
-    assert str(bernoulli(10)) == '0.075757575757575757575757575757575757575757575757576'
-    assert str(bernoulli(234)) == '7.6277279396434392486994969020496121553385863373331e+267'
-    assert str(bernoulli(10**5)) == '-5.8222943146133508236497045360612887555320691004308e+376755'
-    assert str(bernoulli(10**8+2)) == '1.1957035503995297272263047884604346914602088317782e+676752584'
+    assert bernoulli(0, plus) == 1
+    assert bernoulli(1, plus) == 0.5 if plus else -0.5
+    assert bernoulli(2, plus).ae(1./6)
+    assert bernoulli(3, plus) == 0
+    assert bernoulli(4, plus).ae(-1./30)
+    assert bernoulli(5, plus) == 0
+    assert bernoulli(6, plus).ae(1./42)
+    assert str(bernoulli(10, plus)) == '0.0757575757575758'
+    assert str(bernoulli(234, plus)) == '7.62772793964344e+267'
+    assert str(bernoulli(10**5, plus)) == '-5.82229431461335e+376755'
+    assert str(bernoulli(10**8+2, plus)) == '1.19570355039953e+676752584'
+
+    mp.dps = 50
+    assert str(bernoulli(10, plus)) == '0.075757575757575757575757575757575757575757575757576'
+    assert str(bernoulli(234, plus)) == '7.6277279396434392486994969020496121553385863373331e+267'
+    assert str(bernoulli(10**5, plus)) == '-5.8222943146133508236497045360612887555320691004308e+376755'
+    assert str(bernoulli(10**8+2, plus)) == '1.1957035503995297272263047884604346914602088317782e+676752584'
 
     mp.dps = 1000
-    assert bernoulli(10).ae(mpf(5)/66)
+    assert bernoulli(10, plus).ae(mpf(5)/66)
 
     mp.dps = 50000
-    assert bernoulli(10).ae(mpf(5)/66)
+    assert bernoulli(10, plus).ae(mpf(5)/66)
 
     mp.dps = 15
 
 def test_bernpoly_eulerpoly():
-    mp.dps = 15
     assert bernpoly(0,-1).ae(1)
     assert bernpoly(0,0).ae(1)
     assert bernpoly(0,'1/2').ae(1)
     assert bernpoly(0,'3/4').ae(1)
     assert bernpoly(0,1).ae(1)
     assert bernpoly(0,2).ae(1)
     assert bernpoly(1,-1).ae('-3/2')
@@ -149,15 +158,14 @@
     assert eulerpoly(11,2).ae('699/4')
     # Potential accuracy issues
     assert bernpoly(10000,10000).ae('5.8196915936323387117e+39999')
     assert bernpoly(200,17.5).ae(3.8048418524583064909e244)
     assert eulerpoly(200,17.5).ae(-3.7309911582655785929e275)
 
 def test_gamma():
-    mp.dps = 15
     assert gamma(0.25).ae(3.6256099082219083119)
     assert gamma(0.0001).ae(9999.4228832316241908)
     assert gamma(300).ae('1.0201917073881354535e612')
     assert gamma(-0.5).ae(-3.5449077018110320546)
     assert gamma(-7.43).ae(0.00026524416464197007186)
     #assert gamma(Rational(1,2)) == gamma(0.5)
     #assert gamma(Rational(-7,3)).ae(gamma(mpf(-7)/3))
@@ -188,25 +196,23 @@
     assert rgamma(2) == 1.0
     assert rgamma(3) == 0.5
     assert loggamma(2+8j).ae(-8.5205176753667636926 + 10.8569497125597429366j)
     assert loggamma('1e10000').ae('2.302485092994045684017991e10004')
     assert loggamma('1e10000j').ae(mpc('-1.570796326794896619231322e10000','2.302485092994045684017991e10004'))
 
 def test_fac2():
-    mp.dps = 15
     assert [fac2(n) for n in range(10)] == [1,1,2,3,8,15,48,105,384,945]
     assert fac2(-5).ae(1./3)
     assert fac2(-11).ae(-1./945)
     assert fac2(50).ae(5.20469842636666623e32)
     assert fac2(0.5+0.75j).ae(0.81546769394688069176-0.34901016085573266889j)
     assert fac2(inf) == inf
     assert isnan(fac2(-inf))
 
 def test_gamma_quotients():
-    mp.dps = 15
     h = 1e-8
     ep = 1e-4
     G = gamma
     assert gammaprod([-1],[-3,-4]) == 0
     assert gammaprod([-1,0],[-5]) == inf
     assert abs(gammaprod([-1],[-2]) - G(-1+h)/G(-2+h)) < 1e-4
     assert abs(gammaprod([-4,-3],[-2,0]) - G(-4+h)*G(-3+h)/G(-2+h)/G(0+h)) < 1e-4
@@ -247,15 +253,14 @@
     assert beta(inf,-0.5) == -inf
     assert beta(1+2j,-1-j/2).ae(1.16396542451069943086+0.08511695947832914640j)
     assert beta(-0.5,0.5) == 0
     assert beta(-3,3).ae(-1/3.)
     assert beta('-255.5815971722918','-0.5119253100282322').ae('18.157330562703710339')  # issue 421
 
 def test_zeta():
-    mp.dps = 15
     assert zeta(2).ae(pi**2 / 6)
     assert zeta(2.0).ae(pi**2 / 6)
     assert zeta(mpc(2)).ae(pi**2 / 6)
     assert zeta(100).ae(1)
     assert zeta(0).ae(-0.5)
     assert zeta(0.5).ae(-1.46035450880958681)
     assert zeta(-1).ae(-mpf(1)/12)
@@ -282,15 +287,14 @@
     assert zeta(0,0.5) == 0
     assert zeta(0,0) == 0.5
     assert zeta(0,0.5,1).ae(-0.34657359027997265)
     # see issue #390
     assert zeta(-1.5,0.5j).ae(-0.13671400162512768475 + 0.11411333638426559139j)
 
 def test_altzeta():
-    mp.dps = 15
     assert altzeta(-2) == 0
     assert altzeta(-4) == 0
     assert altzeta(-100) == 0
     assert altzeta(0) == 0.5
     assert altzeta(-1) == 0.25
     assert altzeta(-3) == -0.125
     assert altzeta(-5) == 0.25
@@ -312,15 +316,14 @@
     assert altzeta(1.3).ae(0.73821404216623045)
     assert altzeta(1e-30).ae(0.5)
     assert altzeta(-1e-30).ae(0.5)
     assert altzeta(mpc(1e-30,1e-40)).ae(0.5)
     assert altzeta(mpc(-1e-30,1e-40)).ae(0.5)
 
 def test_zeta_huge():
-    mp.dps = 15
     assert zeta(inf) == 1
     mp.dps = 50
     assert zeta(100).ae('1.0000000000000000000000000000007888609052210118073522')
     assert zeta(40*pi).ae('1.0000000000000000000000000000000000000148407238666182')
     mp.dps = 10000
     v = zeta(33000)
     mp.dps = 15
@@ -333,18 +336,16 @@
 def test_zeta_negative():
     mp.dps = 150
     a = -pi*10**40
     mp.dps = 15
     assert str(zeta(a)) == '2.55880492708712e+1233536161668617575553892558646631323374078'
     mp.dps = 50
     assert str(zeta(a)) == '2.5588049270871154960875033337384432038436330847333e+1233536161668617575553892558646631323374078'
-    mp.dps = 15
 
 def test_polygamma():
-    mp.dps = 15
     psi0 = lambda z: psi(0,z)
     psi1 = lambda z: psi(1,z)
     assert psi0(3) == psi(0,3) == digamma(3)
     #assert psi2(3) == psi(2,3) == tetragamma(3)
     #assert psi3(3) == psi(3,3) == pentagamma(3)
     assert psi0(pi).ae(0.97721330794200673)
     assert psi0(-pi).ae(7.8859523853854902)
@@ -378,23 +379,24 @@
     assert isnan(psi(2,mpc(1,-inf)))
     assert isnan(psi(2,mpc(inf,inf)))
     assert isnan(psi(2,mpc(nan,nan)))
     assert isnan(psi(2,mpc(-inf,-inf)))
     mp.dps = 30
     # issue #534
     assert digamma(-0.75+1j).ae(mpc('0.46317279488182026118963809283042317', '2.4821070143037957102007677817351115'))
-    mp.dps = 15
+    # issue #647
+    mp.prec = 42
+    assert digamma(-0.5+0.5j).ae(mpc('0.131892637354523', '2.44065951997751'))
 
 def test_polygamma_high_prec():
     mp.dps = 100
     assert str(psi(0,pi)) == "0.9772133079420067332920694864061823436408346099943256380095232865318105924777141317302075654362928734"
     assert str(psi(10,pi)) == "-12.98876181434889529310283769414222588307175962213707170773803550518307617769657562747174101900659238"
 
 def test_polygamma_identities():
-    mp.dps = 15
     psi0 = lambda z: psi(0,z)
     psi1 = lambda z: psi(1,z)
     psi2 = lambda z: psi(2,z)
     assert psi0(0.5).ae(-euler-2*log(2))
     assert psi0(1).ae(-euler)
     assert psi1(0.5).ae(0.5*pi**2)
     assert psi1(1).ae(pi**2/6)
@@ -413,30 +415,28 @@
     psi0 = lambda z: psi(0,z)
     mp.dps = 50
     a = (-1)**fraction(1,3)
     b = (-1)**fraction(2,3)
     x = -psi0(0.5*a) - psi0(-0.5*b) + psi0(0.5*(1+a)) + psi0(0.5*(1-b))
     y = 2*pi*sech(0.5*sqrt(3)*pi)
     assert x.ae(y)
-    mp.dps = 15
 
 def test_polygamma_high_order():
     mp.dps = 100
     assert str(psi(50, pi)) == "-1344100348958402765749252447726432491812.641985273160531055707095989227897753035823152397679626136483"
     assert str(psi(50, pi + 14*e)) == "-0.00000000000000000189793739550804321623512073101895801993019919886375952881053090844591920308111549337295143780341396"
     assert str(psi(50, pi + 14*e*j)) == ("(-0.0000000000000000522516941152169248975225472155683565752375889510631513244785"
         "9377385233700094871256507814151956624433 - 0.00000000000000001813157041407010184"
         "702414110218205348527862196327980417757665282244728963891298080199341480881811613j)")
     mp.dps = 15
     assert str(psi(50, pi)) == "-1.34410034895841e+39"
     assert str(psi(50, pi + 14*e)) == "-1.89793739550804e-18"
     assert str(psi(50, pi + 14*e*j)) == "(-5.2251694115217e-17 - 1.81315704140701e-17j)"
 
 def test_harmonic():
-    mp.dps = 15
     assert harmonic(0) == 0
     assert harmonic(1) == 1
     assert harmonic(2) == 1.5
     assert harmonic(3).ae(1. + 1./2 + 1./3)
     assert harmonic(10**10).ae(23.603066594891989701)
     assert harmonic(10**1000).ae(2303.162308658947)
     assert harmonic(0.5).ae(2-2*log(2))
@@ -447,15 +447,14 @@
 def test_gamma_huge_1():
     mp.dps = 500
     x = mpf(10**10) / 7
     mp.dps = 15
     assert str(gamma(x)) == "6.26075321389519e+12458010678"
     mp.dps = 50
     assert str(gamma(x)) == "6.2607532138951929201303779291707455874010420783933e+12458010678"
-    mp.dps = 15
 
 def test_gamma_huge_2():
     mp.dps = 500
     x = mpf(10**100) / 19
     mp.dps = 15
     assert str(gamma(x)) == (\
         "1.82341134776679e+5172997469323364168990133558175077136829182824042201886051511"
@@ -483,23 +482,21 @@
         "77865238132302397236429627932441916056964386399485392600")
     assert str(y.imag) == (\
         "8.5464714367841748507479306948130687511711420234015e+263628614211256952450178147"
         "7865238132302397236429627932441916056964386399485392600")
 
 def test_gamma_huge_4():
     x = 3200+11500j
-    mp.dps = 15
     assert str(gamma(x)) == \
         "(8.95783268539713e+5164 - 1.94678798329735e+5164j)"
     mp.dps = 50
     assert str(gamma(x)) == (\
         "(8.9578326853971339570292952697675570822206567327092e+5164"
         " - 1.9467879832973509568895402139429643650329524144794e+51"
         "64j)")
-    mp.dps = 15
 
 def test_gamma_huge_5():
     mp.dps = 500
     x = 10**60 * j / 3
     mp.dps = 15
     y = gamma(x)
     assert str(y.real) == "-3.27753899634941e-227396058973640224580963937571892628368354580620654233316839"
@@ -508,15 +505,14 @@
     y = gamma(x)
     assert str(y.real) == (\
         "-3.2775389963494132168950056995974690946983219123935e-22739605897364022458096393"
         "7571892628368354580620654233316839")
     assert str(y.imag) == (\
         "-7.1519888950415979749736749222530209713136588885897e-22739605897364022458096393"
         "7571892628368354580620654233316841")
-    mp.dps = 15
 
 def test_gamma_huge_7():
     mp.dps = 100
     a = 3 + j/mpf(10)**1000
     mp.dps = 15
     y = gamma(a)
     assert str(y.real) == "2.0"
@@ -526,29 +522,27 @@
     mp.dps = 50
     y = gamma(a)
     assert str(y.real) == "2.0"
     #assert str(y.imag) == "2.1673536534260596065418805612488708028522563689298e-1000"
     assert str(y.imag) ==  "1.8455686701969342787869758198351951379156813281202e-1000"
 
 def test_stieltjes():
-    mp.dps = 15
     assert stieltjes(0).ae(+euler)
     mp.dps = 25
     assert stieltjes(1).ae('-0.07281584548367672486058637587')
     assert stieltjes(2).ae('-0.009690363192872318484530386035')
     assert stieltjes(3).ae('0.002053834420303345866160046543')
     assert stieltjes(4).ae('0.002325370065467300057468170178')
     mp.dps = 15
     assert stieltjes(1).ae(-0.07281584548367672486058637587)
     assert stieltjes(2).ae(-0.009690363192872318484530386035)
     assert stieltjes(3).ae(0.002053834420303345866160046543)
     assert stieltjes(4).ae(0.0023253700654673000574681701775)
 
 def test_barnesg():
-    mp.dps = 15
     assert barnesg(0) == barnesg(-1) == 0
     assert [superfac(i) for i in range(8)] == [1, 1, 2, 12, 288, 34560, 24883200, 125411328000]
     assert str(superfac(1000)) == '3.24570818422368e+1177245'
     assert isnan(barnesg(nan))
     assert isnan(superfac(nan))
     assert isnan(hyperfac(nan))
     assert barnesg(inf) == inf
@@ -561,15 +555,14 @@
     assert [hyperfac(n) for n in range(0,-7,-1)] == [1,1,-1,-4,108,27648,-86400000]
     a = barnesg(-3+0j)
     assert a == 0 and isinstance(a, mpc)
     a = hyperfac(-3+0j)
     assert a == -4 and isinstance(a, mpc)
 
 def test_polylog():
-    mp.dps = 15
     zs = [mpmathify(z) for z in [0, 0.5, 0.99, 4, -0.5, -4, 1j, 3+4j]]
     for z in zs: assert polylog(1, z).ae(-log(1-z))
     for z in zs: assert polylog(0, z).ae(z/(1-z))
     for z in zs: assert polylog(-1, z).ae(z/(1-z)**2)
     for z in zs: assert polylog(-2, z).ae(z*(1+z)/(1-z)**3)
     for z in zs: assert polylog(-3, z).ae(z*(1+4*z+z**2)/(1-z)**4)
     assert polylog(3, 7).ae(5.3192579921456754382-5.9479244480803301023j)
@@ -591,15 +584,14 @@
     # issue 390
     assert polylog(1.5, -48.910886523731889).ae(-6.272992229311817)
     assert polylog(1.5, 200).ae(-8.349608319033686529 - 8.159694826434266042j)
     assert polylog(-2+0j, -2).ae(mpf(1)/13.5)
     assert polylog(-2+0j, 1.25).ae(-180)
 
 def test_bell_polyexp():
-    mp.dps = 15
     # TODO: more tests for polyexp
     assert (polyexp(0,1e-10)*10**10).ae(1.00000000005)
     assert (polyexp(1,1e-10)*10**10).ae(1.0000000001)
     assert polyexp(5,3j).ae(-607.7044517476176454+519.962786482001476087j)
     assert polyexp(-1,3.5).ae(12.09537536175543444)
     # bell(0,x) = 1
     assert bell(0,0) == 1
@@ -629,23 +621,21 @@
     assert bell(74) == 5006908024247925379707076470957722220463116781409659160159536981161298714301202
     mp.dps = 15
     assert bell(10,20j) == 7504528595600+15649605360020j
     # continuity of the generalization
     assert bell(0.5,0).ae(sinc(pi*0.5))
 
 def test_primezeta():
-    mp.dps = 15
     assert primezeta(0.9).ae(1.8388316154446882243 + 3.1415926535897932385j)
     assert primezeta(4).ae(0.076993139764246844943)
     assert primezeta(1) == inf
     assert primezeta(inf) == 0
     assert isnan(primezeta(nan))
 
 def test_rs_zeta():
-    mp.dps = 15
     assert zeta(0.5+100000j).ae(1.0730320148577531321 + 5.7808485443635039843j)
     assert zeta(0.75+100000j).ae(1.837852337251873704 + 1.9988492668661145358j)
     assert zeta(0.5+1000000j, derivative=3).ae(1647.7744105852674733 - 1423.1270943036622097j)
     assert zeta(1+1000000j, derivative=3).ae(3.4085866124523582894 - 18.179184721525947301j)
     assert zeta(1+1000000j, derivative=1).ae(-0.10423479366985452134 - 0.74728992803359056244j)
     assert zeta(0.5-1000000j, derivative=1).ae(11.636804066002521459 + 17.127254072212996004j)
     # Additional sanity tests using fp arithmetic.
@@ -664,25 +654,23 @@
     assert ae(fp.zeta(0.5+100000j, derivative=4), -10407.160819314958615 + 13777.786698628045085j)
     assert ae(fp.zeta(0.75+100000j, derivative=1), -0.41742276699594321475 - 6.4453816275049955949j)
     assert ae(fp.zeta(0.75+100000j, derivative=2), -9.214314279161977266 + 35.07290795337967899j)
     assert ae(fp.zeta(0.75+100000j, derivative=3), 110.61331857820103469 - 236.87847130518129926j)
     assert ae(fp.zeta(0.75+100000j, derivative=4), -1054.334275898559401 + 1769.9177890161596383j)
 
 def test_siegelz():
-    mp.dps = 15
     assert siegelz(100000).ae(5.87959246868176504171)
     assert siegelz(100000, derivative=2).ae(-54.1172711010126452832)
     assert siegelz(100000, derivative=3).ae(-278.930831343966552538)
     assert siegelz(100000+j,derivative=1).ae(678.214511857070283307-379.742160779916375413j)
 
 
 
 def test_zeta_near_1():
     # Test for a former bug in mpf_zeta and mpc_zeta
-    mp.dps = 15
     s1 = fadd(1, '1e-10', exact=True)
     s2 = fadd(1, '-1e-10', exact=True)
     s3 = fadd(1, '1e-10j', exact=True)
     assert zeta(s1).ae(1.000000000057721566490881444e10)
     assert zeta(s2).ae(-9.99999999942278433510574872e9)
     z = zeta(s3)
     assert z.real.ae(0.57721566490153286060)
@@ -692,7 +680,12 @@
     s2 = fadd(1, '-1e-50', exact=True)
     s3 = fadd(1, '1e-50j', exact=True)
     assert zeta(s1).ae('1e50')
     assert zeta(s2).ae('-1e50')
     z = zeta(s3)
     assert z.real.ae('0.57721566490153286060651209008240243104215933593992')
     assert z.imag.ae('-1e50')
+
+def test_issue_723():
+    mp.dps = 16
+    assert zeta(-0.01 + 1000j).ae(-8.971459529241107 + 8.732179332810066j)
+    mp.dps = 15
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_hp.py` & `mpmath-1.4.0a0/mpmath/tests/test_hp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Check that the output from irrational functions is accurate for
 high-precision input, from 5 to 200 digits. The reference values were
 verified with Mathematica.
 """
 
-import time
-from mpmath import *
+from mpmath import cos, e, euler, exp, log, mp, mpc, mpf, pi, sin, sqrt, tan
+
 
 precs = [5, 15, 28, 35, 57, 80, 100, 150, 200]
 
 # sqrt(3) + pi/2
 a = \
 "3.302847134363773912758768033145623809041389953497933538543279275605"\
 "841220051904536395163599428307109666700184672047856353516867399774243594"\
@@ -195,15 +195,14 @@
         # abs_eps should be 0, but has to be set to 1e-205 to pass the
         # 200-digit case, probably due to slight inaccuracy in the
         # precomputed input
         assert (tan(abi).real).ae(mpf(tan_abi_real), abs_eps=1e-205)
         assert (tan(abi).imag).ae(mpf(tan_abi_imag), abs_eps=1e-205)
     mp.dps = 460
     assert str(log(3))[-20:] == '02166121184001409826'
-    mp.dps = 15
 
 # Since str(a) can differ in the last digit from rounded a, and I want
 # to compare the last digits of big numbers with the results in Mathematica,
 # I made this hack to get the last 20 digits of rounded a
 
 def last_digits(a):
     r = repr(a)
@@ -277,15 +276,13 @@
 
     r = log(a)
     res = last_digits(+r)
     # Mathematica N[Log[1 + 10^-100]*10^10, 10030]
     # ...3994733877377412241546890854692521568292338268273 10^-91
     assert res == '39947338773774122415', res
 
-    mp.dps = 15
-
 def test_exp_hp():
     mp.dps = 4000
     r = exp(mpf(1)/10)
     # IntegerPart[N[Exp[1/10] * 10^4000, 4000]]
     # ...92167105162069688129
     assert int(r * 10**mp.dps) % 10**20 == 92167105162069688129
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_identify.py` & `mpmath-1.4.0a0/mpmath/tests/test_identify.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from mpmath import *
+from mpmath import e, exp, identify, log, mp, pi, pslq, zeta
+
 
 def test_pslq():
-    mp.dps = 15
     assert pslq([3*pi+4*e/7, pi, e, log(2)]) == [7, -21, -4, 0]
     assert pslq([4.9999999999999991, 1]) == [1, -5]
     assert pslq([2,1]) == [1, -2]
 
 def test_identify():
     mp.dps = 20
     assert identify(zeta(4), ['log(2)', 'pi**4']) == '((1/90)*pi**4)'
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_interval.py` & `mpmath-1.4.0a0/mpmath/tests/test_interval.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from mpmath import *
+from mpmath import inf, iv, mp, mpf, mpi, pi, sqrt
+
 
 def test_interval_identity():
-    iv.dps = 15
     assert mpi(2) == mpi(2, 2)
     assert mpi(2) != mpi(-2, 2)
     assert not (mpi(2) != mpi(2, 2))
     assert mpi(-1, 1) == mpi(-1, 1)
     assert str(mpi('0.1')) == "[0.099999999999999991673, 0.10000000000000000555]"
     assert repr(mpi('0.1')) == "mpi('0.099999999999999992', '0.10000000000000001')"
     u = mpi(-1, 3)
@@ -18,26 +18,25 @@
     assert mpi(0, 1) in u
     assert mpi(-1.1, 2) not in u
     assert mpi(2.5, 3.1) not in u
     w = mpi(-inf, inf)
     assert mpi(-5, 5) in w
     assert mpi(2, inf) in w
     assert mpi(0, 2) in mpi(0, 10)
-    assert not (3 in mpi(-inf, 0))
+    assert 3 not in mpi(-inf, 0)
 
 def test_interval_hash():
     assert hash(mpi(3)) == hash(3)
     assert hash(mpi(3.25)) == hash(3.25)
     assert hash(mpi(3,4)) == hash(mpi(3,4))
     assert hash(iv.mpc(3)) == hash(3)
     assert hash(iv.mpc(3,4)) == hash(3+4j)
     assert hash(iv.mpc((1,3),(2,4))) == hash(iv.mpc((1,3),(2,4)))
 
 def test_interval_arithmetic():
-    iv.dps = 15
     assert mpi(2) + mpi(3,4) == mpi(5,6)
     assert mpi(1, 2)**2 == mpi(1, 4)
     assert mpi(1) + mpi(0, 1e-50) == mpi(1, mpf('1.0000000000000002'))
     x = 1 / (1 / mpi(3))
     assert x.a < 3 < x.b
     x = mpi(2) ** mpi(0.5)
     iv.dps += 5
@@ -189,15 +188,14 @@
     assert mpi(-1, -0.5) / mpi(-2, -0.5) == mpi(0.25, 2.0)
     assert mpi(-4, -0.5) / mpi(-2, -0.5) == mpi(0.25, 8.0)
     # Should be undefined?
     assert mpi(0, 0) / mpi(0, 0) == mpi(-inf, inf)
     assert mpi(0, 0) / mpi(0, 1) == mpi(-inf, inf)
 
 def test_interval_cos_sin():
-    iv.dps = 15
     cos = iv.cos
     sin = iv.sin
     tan = iv.tan
     pi = iv.pi
     # Around 0
     assert cos(mpi(0)) == 1
     assert sin(mpi(0)) == 0
@@ -267,16 +265,14 @@
         assert x.a < 0 < x.b
         x = iv.sin(n*iv.pi)
         if n:
             assert x.a < 0 < x.b
 
 def test_interval_complex():
     # TODO: many more tests
-    iv.dps = 15
-    mp.dps = 15
     assert iv.mpc(2,3) == 2+3j
     assert iv.mpc(2,3) != 2+4j
     assert iv.mpc(2,3) != 1+3j
     assert 1+3j in iv.mpc([1,2],[3,4])
     assert 2+5j not in iv.mpc([1,2],[3,4])
     assert iv.mpc(1,2) + 1j == 1+3j
     assert iv.mpc([1,2],[2,3]) + 2+3j == iv.mpc([3,4],[5,6])
@@ -307,16 +303,14 @@
     assert iv.mpc(2,2) ** (-2) == (2+2j) ** (-2)
     assert iv.cos(2).ae(mp.cos(2))
     assert iv.sin(2).ae(mp.sin(2))
     assert iv.cos(2+3j).ae(mp.cos(2+3j))
     assert iv.sin(2+3j).ae(mp.sin(2+3j))
 
 def test_interval_complex_arg():
-    mp.dps = 15
-    iv.dps = 15
     assert iv.arg(3) == 0
     assert iv.arg(0) == 0
     assert iv.arg([0,3]) == 0
     assert iv.arg(-3).ae(pi)
     assert iv.arg(2+3j).ae(iv.arg(2+3j))
     z = iv.mpc([-2,-1],[3,4])
     t = iv.arg(z)
@@ -352,15 +346,14 @@
     assert t.b.ae(mp.pi)
     z = iv.mpc([-2,2],[-3,3])
     t = iv.arg(z)
     assert t.a.ae(-mp.pi)
     assert t.b.ae(mp.pi)
 
 def test_interval_ae():
-    iv.dps = 15
     x = iv.mpf([1,2])
     assert x.ae(1) is None
     assert x.ae(1.5) is None
     assert x.ae(2) is None
     assert x.ae(2.01) is False
     assert x.ae(0.99) is False
     x = iv.mpf(3.5)
@@ -383,39 +376,36 @@
     assert iv.nstr(x, n, mode='brackets' , brackets=('<', '>')) == '<1.0, 2.0>'
     x = mpi('5.2582327113062393041', '5.2582327113062749951')
     assert iv.nstr(x, n, mode='diff') == '5.2582327113062[393041, 749951]'
     assert iv.nstr(iv.cos(mpi(1)), n, mode='diff', use_spaces=False) == '0.54030230586813971740093660744[2955,3053]'
     assert iv.nstr(mpi('1e123', '1e129'), n, mode='diff') == '[1.0e+123, 1.0e+129]'
     exp = iv.exp
     assert iv.nstr(iv.exp(mpi('5000.1')), n, mode='diff') == '3.2797365856787867069110487[0926, 1191]e+2171'
-    iv.dps = 15
 
 def test_mpi_from_str():
-    iv.dps = 15
     assert iv.convert('1.5 +- 0.5') == mpi(mpf('1.0'), mpf('2.0'))
     assert mpi(1, 2) in iv.convert('1.5 (33.33333333333333333333333333333%)')
     assert iv.convert('[1, 2]') == mpi(1, 2)
     assert iv.convert('1[2, 3]') == mpi(12, 13)
     assert iv.convert('1.[23,46]e-8') == mpi('1.23e-8', '1.46e-8')
     assert iv.convert('12[3.4,5.9]e4') == mpi('123.4e+4', '125.9e4')
 
 def test_interval_gamma():
-    mp.dps = 15
-    iv.dps = 15
     # TODO: need many more tests
     assert iv.rgamma(0) == 0
     assert iv.fac(0) == 1
     assert iv.fac(1) == 1
     assert iv.fac(2) == 2
     assert iv.fac(3) == 6
     assert iv.gamma(0) == [-inf,inf]
     assert iv.gamma(1) == 1
     assert iv.gamma(2) == 1
     assert iv.gamma(3) == 2
     assert -3.5449077018110320546 in iv.gamma(-0.5)
+    assert 0.49801566811835601-0.1549498283018107j in iv.gamma(1+1j)
     assert iv.loggamma(1) == 0
     assert iv.loggamma(2) == 0
     assert 0.69314718055994530942 in iv.loggamma(3)
     # Test tight log-gamma endpoints based on monotonicity
     xs = [iv.mpc([2,3],[1,4]),
           iv.mpc([2,3],[-4,-1]),
           iv.mpc([2,3],[-1,4]),
@@ -437,16 +427,14 @@
         z = iv.loggamma(x)
         assert z.a.ae(min_real)
         assert z.b.ae(max_real)
         assert z.c.ae(min_imag)
         assert z.d.ae(max_imag)
 
 def test_interval_conversions():
-    mp.dps = 15
-    iv.dps = 15
     for a, b in ((-0.0, 0), (0.0, 0.5), (1.0, 1), \
                  ('-inf', 20.5), ('-inf', float(sqrt(2)))):
         r = mpi(a, b)
         assert int(r.b) == int(b)
         assert float(r.a) == float(a)
         assert float(r.b) == float(b)
         assert complex(r.a) == complex(a)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_levin.py` & `mpmath-1.4.0a0/mpmath/tests/test_levin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 from mpmath import mp
-from mpmath import libmp
 
-xrange = libmp.backend.xrange
 
 # Attention:
 #   These tests run with 15-20 decimal digits precision. For higher precision the
 #   working precision must be raised.
 
 def test_levin_0():
     mp.dps = 17
@@ -92,15 +87,16 @@
             if n > 1000: raise RuntimeError("iteration limit exceeded")
     eps = mp.exp(0.8 * mp.log(eps))
     exact = mp.quad(lambda x: mp.exp( -x * x / 2 - z * x ** 4), [0,mp.inf]) * 2 / mp.sqrt(2 * mp.pi)
     # there is also a symbolic expression for the integral:
     #   exact = mp.exp(mp.one / (32 * z)) * mp.besselk(mp.one / 4, mp.one / (32 * z)) / (4 * mp.sqrt(z * mp.pi))
     err = abs(v - exact)
     assert err < eps
-    w = mp.nsum(lambda n: (-z)**n * mp.fac(4 * n) / (mp.fac(n) * mp.fac(2 * n) * (4 ** n)), [0, mp.inf], method = "levin", levin_variant = "t", workprec = 8*mp.prec, steps = [2] + [1 for x in xrange(1000)])
+    w = mp.nsum(lambda n: (-z)**n * mp.fac(4 * n) / (mp.fac(n) * mp.fac(2 * n) * (4 ** n)), [0, mp.inf],
+                method = "levin", levin_variant = "t", workprec = 8*mp.prec, steps = [2] + [1 for x in range(1000)])
     err = abs(v - w)
     assert err < eps
 
 def test_levin_nsum():
     mp.dps = 17
 
     with mp.extraprec(mp.prec):
@@ -111,15 +107,15 @@
     eps = mp.exp(0.8 * mp.log(mp.eps))
 
     a = mp.nsum(lambda n: (-1)**(n-1) / n, [1, mp.inf], method = "sidi")
     assert abs(a - mp.log(2)) < eps
 
     z = 2 + 1j
     f = lambda n: mp.rf(2 / mp.mpf(3), n) * mp.rf(4 / mp.mpf(3), n) * z**n / (mp.rf(1 / mp.mpf(3), n) * mp.fac(n))
-    v = mp.nsum(f, [0, mp.inf], method = "levin", steps = [10 for x in xrange(1000)])
+    v = mp.nsum(f, [0, mp.inf], method = "levin", steps = [10 for x in range(1000)])
     exact = mp.hyp2f1(2 / mp.mpf(3), 4 / mp.mpf(3), 1 / mp.mpf(3), z)
     assert abs(exact - v) < eps
 
 def test_cohen_alt_0():
     mp.dps = 17
     AC = mp.cohen_alt()
     S, s, n = [], 0, 1
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_linalg.py` & `mpmath-1.4.0a0/mpmath/tests/test_linalg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # TODO: don't use round
 
-from __future__ import division
-
 import pytest
-from mpmath import *
-xrange = libmp.backend.xrange
+
+from mpmath import (cond, det, diag, exp, expm, extend, extradps, eye, fp,
+                    hilbert, inf, inverse, iv, j, lu, lu_solve, matrix, mnorm,
+                    mp, mpc, mpf, nint, norm, pi, qr, qr_solve, rand, rank,
+                    randmatrix, residual, zeros, absmin, eps)
+
 
 # XXX: these shouldn't be visible(?)
 LU_decomp = mp.LU_decomp
 L_solve = mp.L_solve
 U_solve = mp.U_solve
 householder = mp.householder
 improve_solution = mp.improve_solution
@@ -64,14 +66,25 @@
 b9 = [10, 16, -15.5]
 
 A10 = matrix([[1.0 + 1.0j, 2.0, 2.0],
             [4.0, 5.0, 6.0],
             [7.0, 8.0, 9.0]])
 b10 = [1.0, 1.0 + 1.0j, 1.0]
 
+A11 = matrix([[4, 0, -2],
+             [2, 0, -4],
+             [2, 0, 5.5]])
+
+A12 = matrix([[1,0,0],
+              [0,1,0],
+              [0,0,1.0j]])
+
+A13 = matrix([[2, 6, 4],
+              [3, 8, 6],
+              [1, 1, 2]])
 
 def test_LU_decomp():
     A = A3.copy()
     b = b3
     A, p = LU_decomp(A)
     y = L_solve(A, b, p)
     x = U_solve(A, y)
@@ -87,21 +100,22 @@
     assert [round(i, 14) for i in x] == [2.6383625899619201, 2.6643834462368399,
             0.79208015947958998, -2.5088376454101899, -1.0567657691375001]
     A = randmatrix(3)
     bak = A.copy()
     LU_decomp(A, overwrite=1)
     assert A != bak
 
+    pytest.raises(ZeroDivisionError, LU_decomp, A11)
+
 def test_inverse():
     for A in [A1, A2, A5]:
         inv = inverse(A)
         assert mnorm(A*inv - eye(A.rows), 1) < 1.e-14
 
 def test_householder():
-    mp.dps = 15
     A, b = A8, b8
     H, p, x, r = householder(extend(A, b))
     assert H == matrix(
     [[mpf('3.0'), mpf('-2.0'), mpf('-1.0'), 0],
      [-1.0,mpf('3.333333333333333'),mpf('-2.9999999999999991'),mpf('2.0')],
      [-1.0, mpf('-0.66666666666666674'),mpf('2.8142135623730948'),
       mpf('-2.8284271247461898')],
@@ -168,51 +182,54 @@
 
 def test_solve_overdet_complex():
     A = matrix([[1, 2j], [3, 4j], [5, 6]])
     b = matrix([1 + j, 2, -j])
     assert norm(residual(A, lu_solve(A, b), b)) < 1.0208
 
 def test_singular():
-    mp.dps = 15
     A = [[5.6, 1.2], [7./15, .1]]
     B = repr(zeros(2))
     b = [1, 2]
     for i in ['lu_solve(%s, %s)' % (A, b), 'lu_solve(%s, %s)' % (B, b),
               'qr_solve(%s, %s)' % (A, b), 'qr_solve(%s, %s)' % (B, b)]:
         pytest.raises((ZeroDivisionError, ValueError), lambda: eval(i))
 
 def test_cholesky():
     assert fp.cholesky(fp.matrix(A9)) == fp.matrix([[2, 0, 0], [1, 2, 0], [-1, -3/2, 3/2]])
     x = fp.cholesky_solve(A9, b9)
     assert fp.norm(fp.residual(A9, x, b9), fp.inf) == 0
 
+    a = fp.matrix([[1, 0.5j], [-0.5j, 0.5]])
+    b = fp.ones(2, 1)
+    x = fp.cholesky_solve(a, b)
+    assert fp.norm(fp.residual(a, x, b), fp.inf) == 0
+
 def test_det():
     assert det(A1) == 1
     assert round(det(A2), 14) == 8
     assert round(det(A3)) == 1834
     assert round(det(A4)) == 4443376
     assert det(A5) == 1
     assert round(det(A6)) == 78356463
     assert det(zeros(3)) == 0
+    assert det(A11) == 0
+    assert absmin(det(A12*1e-30) - 1e-30) < eps
 
 def test_cond():
-    mp.dps = 15
     A = matrix([[1.2969, 0.8648], [0.2161, 0.1441]])
     assert cond(A, lambda x: mnorm(x,1)) == mpf('327065209.73817754')
     assert cond(A, lambda x: mnorm(x,inf)) == mpf('327065209.73817754')
     assert cond(A, lambda x: mnorm(x,'F')) == mpf('249729266.80008656')
 
 @extradps(50)
 def test_precision():
     A = randmatrix(10, 10)
     assert mnorm(inverse(inverse(A)) - A, 1) < 1.e-45
 
 def test_interval_matrix():
-    mp.dps = 15
-    iv.dps = 15
     a = iv.matrix([['0.1','0.3','1.0'],['7.1','5.5','4.8'],['3.2','4.4','5.6']])
     b = iv.matrix(['4','0.6','0.5'])
     c = iv.lu_solve(a, b)
     assert c[0].delta < 1e-13
     assert c[1].delta < 1e-13
     assert c[2].delta < 1e-13
     assert 5.25823271130625686059275 in c[0]
@@ -255,25 +272,23 @@
         mp.dps = dps
         e1 = expm(a1, method='pade')
         mp.dps = dps + extra
         d = e2 - e1
         #print d
         mp.dps = dps
         assert norm(d, inf).ae(0)
-    mp.dps = 15
 
 def test_qr():
-    mp.dps = 15                     # used default value for dps
     lowlimit = -9                   # lower limit of matrix element value
     uplimit = 9                     # uppter limit of matrix element value
     maxm = 4                        # max matrix size
     flg = False                     # toggle to create real vs complex matrix
     zero = mpf('0.0')
 
-    for k in xrange(0,10):
+    for k in range(10):
         exdps = 0
         mode = 'full'
         flg = bool(k % 2)
 
         # generate arbitrary matrix size (2 to maxm)
         num1 = nint(maxm*rand())
         num2 = nint(maxm*rand())
@@ -283,24 +298,24 @@
         # create matrix
         A = mp.matrix(m,n)
 
         # populate matrix values with arbitrary integers
         if flg:
             flg = False
             dtype = 'complex'
-            for j in xrange(0,n):
-                for i in xrange(0,m):
+            for j in range(n):
+                for i in range(m):
                     val = nint(lowlimit + (uplimit-lowlimit)*rand())
                     val2 = nint(lowlimit + (uplimit-lowlimit)*rand())
                     A[i,j] = mpc(val, val2)
         else:
             flg = True
             dtype = 'real'
-            for j in xrange(0,n):
-                for i in xrange(0,m):
+            for j in range(n):
+                for i in range(m):
                     val = nint(lowlimit + (uplimit-lowlimit)*rand())
                     A[i,j] = mpf(val)
 
         # perform A -> QR decomposition
         Q, R = qr(A, mode, edps = exdps)
 
         #print('\n\n A = \n', nstr(A, 4))
@@ -326,7 +341,22 @@
             n1 = norm(eye(m) - Q.T * Q.conjugate())
             #print ' Norm of I - Q.T * Q.conjugate() = ', n1
             assert n1 <= maxnorm
 
             n1 = norm(eye(m) - Q.conjugate() * Q.T)
             #print ' Norm of I - Q.conjugate() * Q.T = ', n1
             assert n1 <= maxnorm
+
+def test_rank():
+    assert rank(A1) == 3
+    assert rank(A2) == 4
+    assert rank(A3) == 5
+    assert rank(A4) == 5
+    assert rank(A5) == 3
+    assert rank(A6) == 3
+    assert rank(zeros(3)) == 0
+    assert rank(A11) == 2
+    assert rank(A1*A11) == 2
+    assert rank(A11*A11) == 2
+    iszerofunc = lambda x: not bool(x)
+    assert rank(A13) == 2
+    assert rank(A13, iszerofunc) == 3
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_matrices.py` & `mpmath-1.4.0a0/mpmath/tests/test_matrices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import pytest
-import sys
-from mpmath import *
+
+from mpmath import (convert, diag, extend, eye, fp, hilbert, inf, inverse, iv,
+                    j, matrix, mnorm, mp, mpc, mpf, mpi, norm, nstr, ones,
+                    randmatrix, sqrt, swap_row, zeros)
+
 
 def test_matrix_basic():
     A1 = matrix(3)
     for i in range(3):
         A1[i,i] = 1
     assert A1 == eye(3)
     assert A1 == matrix(A1)
     A2 = matrix(3, 2)
     assert not A2._matrix__data
     A3 = matrix([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     assert list(A3) == list(range(1, 10))
     A3[1,1] = 0
-    assert not (1, 1) in A3._matrix__data
+    assert (1, 1) not in A3._matrix__data
     A4 = matrix([[1, 2, 3], [4, 5, 6]])
     A5 = matrix([[6, -1], [3, 2], [0, -3]])
     assert A4 * A5 == matrix([[12, -6], [39, -12]])
     assert A1 * A3 == A3 * A1 == A3
     pytest.raises(ValueError, lambda: A2*A2)
     l = [[10, 20, 30], [40, 0, 60], [70, 80, 90]]
     A6 = matrix(l)
@@ -44,39 +47,39 @@
     assert eye(3)**10 == eye(3)
     pytest.raises(ValueError, lambda: A7**2)
     A9 = randmatrix(3)
     A10 = matrix(A9)
     A9[0,0] = -100
     assert A9 != A10
     assert nstr(A9)
+    assert A9 != None  # issue 283
+    pytest.raises(IndexError, lambda: zeros(1,1)[:, 1])  # issue 318
+    pytest.raises(IndexError, lambda: zeros(1,1)[1, :])
 
 def test_matmul():
     """
     Test the PEP465 "@" matrix multiplication syntax.
-    To avoid syntax errors when importing this file in Python 3.5 and below, we have to use exec() - sorry for that.
     """
-    # TODO remove exec() wrapper as soon as we drop support for Python <= 3.5
-    if sys.hexversion < 0x30500f0:
-        # we are on Python < 3.5
-        pytest.skip("'@' (__matmul__) is only supported in Python 3.5 or newer")
     A4 = matrix([[1, 2, 3], [4, 5, 6]])
     A5 = matrix([[6, -1], [3, 2], [0, -3]])
-    exec("assert A4 @ A5 == A4 * A5")
+    assert A4 @ A5 == A4 * A5
 
 def test_matrix_slices():
     A = matrix([    [1, 2, 3],
                         [4, 5 ,6],
                         [7, 8 ,9]])
     V = matrix([1,2,3,4,5])
 
     # Get slice
     assert A[:,:] == A
     assert A[:,1] == matrix([[2],[5],[8]])
     assert A[2,:] == matrix([[7, 8 ,9]])
     assert A[1:3,1:3] == matrix([[5,6],[8,9]])
+    assert A[0:2,0:2] == matrix([[1,2],[4,5]])  # issue 267
+    assert A[:2,:2] == matrix([[1,2],[4,5]])
     assert V[2:4] == matrix([3,4])
     pytest.raises(IndexError, lambda: A[:,1:6])
 
     # Assign slice with matrix
     A1 = matrix(3)
     A1[:,:] = A
     assert A1[:,:] == matrix([[1, 2, 3],
@@ -185,18 +188,15 @@
     assert A == C
     B[0,0] = 0
     assert A != B
     C[0,0] = 42
     assert A != C
 
 def test_matrix_numpy():
-    try:
-        import numpy
-    except ImportError:
-        return
+    numpy = pytest.importorskip("numpy")
     l = [[1, 2], [3, 4], [5, 6]]
     a = numpy.array(l)
     assert matrix(l) == matrix(a)
 
 def test_interval_matrix_scalar_mult():
     """Multiplication of iv.matrix and any scalar type"""
     a = mpi(-1, 1)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_ode.py` & `mpmath-1.4.0a0/mpmath/tests/test_ode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #from mpmath.calculus import ODE_step_euler, ODE_step_rk4, odeint, arange
-from mpmath import odefun, cos, sin, mpf, sinc, mp
+from mpmath import cos, mpf, odefun, sin, sinc
+
 
 '''
 solvers = [ODE_step_euler, ODE_step_rk4]
 
 def test_ode1():
     """
     Let's solve:
@@ -46,28 +47,25 @@
         x = [a[0] for a in sol]
         # the result is x = exp(t)
         # let's just check the end point for t = 1, i.e. x = e
         assert abs(x[-1] - 2.718281828) < 1e-2
 '''
 
 def test_odefun_rational():
-    mp.dps = 15
     # A rational function
     f = lambda t: 1/(1+mpf(t)**2)
     g = odefun(lambda x, y: [-2*x*y[0]**2], 0, [f(0)])
     assert f(2).ae(g(2)[0])
 
 def test_odefun_sinc_large():
-    mp.dps = 15
     # Sinc function; test for large x
     f = sinc
     g = odefun(lambda x, y: [(cos(x)-y[0])/x], 1, [f(1)], tol=0.01, degree=5)
     assert abs(f(100) - g(100)[0])/f(100) < 0.01
 
 def test_odefun_harmonic():
-    mp.dps = 15
     # Harmonic oscillator
     f = odefun(lambda x, y: [-y[1], y[0]], 0, [1, 0])
     for x in [0, 1, 2.5, 8, 3.7]:    #  we go back to 3.7 to check caching
         c, s = f(x)
         assert c.ae(cos(x))
         assert s.ae(sin(x))
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_power.py` & `mpmath-1.4.0a0/mpmath/tests/test_power.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from mpmath import *
-from mpmath.libmp import *
-
 import random
 
+from mpmath import make_mpf, mp, mpf
+from mpmath.libmp import (from_int, mpf_pow, mpf_pow_int, round_ceiling,
+                          round_down, round_floor, round_up, to_int)
+
+
 def test_fractional_pow():
-    mp.dps = 15
     assert mpf(16) ** 2.5 == 1024
     assert mpf(64) ** 0.5 == 8
     assert mpf(64) ** -0.5 == 0.125
     assert mpf(16) ** -2.5 == 0.0009765625
     assert (mpf(10) ** 0.5).ae(3.1622776601683791)
     assert (mpf(10) ** 2.5).ae(316.2277660168379)
     assert (mpf(10) ** -0.5).ae(0.31622776601683794)
@@ -33,30 +34,30 @@
 
 
 def test_pow_epsilon_rounding():
     """
     Stress test directed rounding for powers with integer exponents.
     Basically, we look at the following cases:
 
-    >>> 1.0001 ** -5 # doctest: +SKIP
-    0.99950014996500702
-    >>> 0.9999 ** -5 # doctest: +SKIP
+    >>> 1.0001 ** -5
+    0.999500149965007
+    >>> 0.9999 ** -5
     1.000500150035007
-    >>> (-1.0001) ** -5 # doctest: +SKIP
-    -0.99950014996500702
-    >>> (-0.9999) ** -5 # doctest: +SKIP
+    >>> (-1.0001) ** -5
+    -0.999500149965007
+    >>> (-0.9999) ** -5
     -1.000500150035007
 
-    >>> 1.0001 ** -6 # doctest: +SKIP
-    0.99940020994401269
-    >>> 0.9999 ** -6 # doctest: +SKIP
+    >>> 1.0001 ** -6
+    0.9994002099440127
+    >>> 0.9999 ** -6
     1.0006002100560125
-    >>> (-1.0001) ** -6 # doctest: +SKIP
-    0.99940020994401269
-    >>> (-0.9999) ** -6 # doctest: +SKIP
+    >>> (-1.0001) ** -6
+    0.9994002099440127
+    >>> (-0.9999) ** -6
     1.0006002100560125
 
     etc.
 
     We run the tests with values a very small epsilon away from 1:
     small enough that the result is indistinguishable from 1 when
     rounded to nearest at the output precision. We check that the
@@ -148,9 +149,7 @@
         assert powr(pos09999, -5, r) == 1
         assert powr(neg10001, -5, r) == -1
         assert powr(neg09999, -5, r) < -1
         assert powr(pos10001, -6, r) < 1
         assert powr(pos09999, -6, r) == 1
         assert powr(neg10001, -6, r) < 1
         assert powr(neg09999, -6, r) == 1
-
-    mp.dps = 15
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_quad.py` & `mpmath-1.4.0a0/mpmath/tests/test_quad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
-from mpmath import *
+
+from mpmath import (airyai, airyaizero, atan, cos, cosh, e, euler, exp, inf, j,
+                    log, mp, pi, quad, quadgl, quadosc, quadts, sign, sin,
+                    sinh, sqrt, tan)
+
 
 def ae(a, b):
     return abs(a-b) < 10**(-mp.dps+5)
 
 def test_basic_integrals():
     for prec in [15, 30, 100]:
         mp.dps = prec
@@ -13,15 +17,14 @@
         assert ae(quadts(sin, [0, 2*pi]), 0)
         assert ae(quadts(exp, [-inf, -1]), 1/e)
         assert ae(quadts(lambda x: exp(-x), [0, inf]), 1)
         assert ae(quadts(lambda x: exp(-x*x), [-inf, inf]), sqrt(pi))
         assert ae(quadts(lambda x: 1/(1+x*x), [-1, 1]), pi/2)
         assert ae(quadts(lambda x: 1/(1+x*x), [-inf, inf]), pi)
         assert ae(quadts(lambda x: 2*sqrt(1-x*x), [-1, 1]), pi)
-    mp.dps = 15
 
 def test_multiple_intervals():
     y,err = quad(lambda x: sign(x), [-0.5, 0.9, 1], maxdegree=2, error=True)
     assert abs(y-0.5) < 2*err
 
 def test_quad_symmetry():
     assert quadts(sin, [-1, 1]) == 0
@@ -35,16 +38,17 @@
 def test_quadgl_linear():
     assert quadgl(lambda x: x, [0, 1], maxdegree=1).ae(0.5)
 
 def test_complex_integration():
     assert quadts(lambda x: x, [0, 1+j]).ae(j)
 
 def test_quadosc():
-    mp.dps = 15
     assert quadosc(lambda x: sin(x)/x, [0, inf], period=2*pi).ae(pi/2)
+    # issue #652
+    assert ae(quadosc(airyai, [-inf, 0], zeros=lambda n: -airyaizero(-n)), 2/3)
 
 # Double integrals
 def test_double_trivial():
     assert ae(quadts(lambda x, y: x, [0, 1], [0, 1]), 0.5)
     assert ae(quadts(lambda x, y: x, [-1, 1], [-1, 1]), 0.0)
 
 def test_double_1():
@@ -80,15 +84,14 @@
         assert ae(quadts(lambda x: log(x)/cosh(x)**2, [0, inf]),            log(pi)-2*log(2)-euler)
         assert ae(quadts(lambda x: log(1+x**3)/(1-x+x**2), [0, inf]),       2*pi*log(3)/sqrt(3))
         assert ae(quadts(lambda x: log(x)**2 / (x**2+x+1), [0, 1]),         8*pi**3 / (81*sqrt(3)))
         assert ae(quadts(lambda x: log(cos(x))**2, [0, pi/2]),              pi/2 * (log(2)**2+pi**2/12))
         assert ae(quadts(lambda x: x**2 / sin(x)**2, [0, pi/2]),            pi*log(2))
         assert ae(quadts(lambda x: x**2/sqrt(exp(x)-1), [0, inf]),          4*pi*(log(2)**2 + pi**2/12))
         assert ae(quadts(lambda x: x*exp(-x)*sqrt(1-exp(-2*x)), [0, inf]),  pi*(1+2*log(2))/8)
-    mp.dps = 15
 
 # Do not reach full accuracy
 @pytest.mark.xfail
 def test_expmath_fail():
     assert ae(quadts(lambda x: sqrt(tan(x)), [0, pi/2]),          pi*sqrt(2)/2)
     assert ae(quadts(lambda x: atan(x)/(x*sqrt(1-x**2)), [0, 1]), pi*log(1+sqrt(2))/2)
     assert ae(quadts(lambda x: log(1+x**2)/x**2, [0, 1]),         pi/2-log(2))
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_rootfinding.py` & `mpmath-1.4.0a0/mpmath/tests/test_rootfinding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import pytest
-from mpmath import *
-from mpmath.calculus.optimization import Secant, Muller, Bisection, Illinois, \
-    Pegasus, Anderson, Ridder, ANewton, Newton, MNewton, MDNewton
+
+from mpmath import (cos, eps, findroot, fp, inf, iv, jacobian, matrix, mnorm,
+                    mp, mpc, mpf, multiplicity, norm, pi, polyval, sin, sqrt,
+                    workprec)
+from mpmath.calculus.optimization import (Anderson, ANewton, Bisection,
+                                          Illinois, MDNewton, MNewton, Muller,
+                                          Newton, Pegasus, Ridder, Secant)
+
 
 def test_findroot():
     # old tests, assuming secant
-    mp.dps = 15
     assert findroot(lambda x: 4*x-3, mpf(5)).ae(0.75)
     assert findroot(sin, mpf(3)).ae(pi)
     assert findroot(sin, (mpf(3), mpf(3.14))).ae(pi)
     assert findroot(lambda x: x*x+1, mpc(2+2j)).ae(1j)
     # test all solvers with 1 starting point
     f = lambda x: cos(x)
     for solver in [Newton, Secant, MNewton, Muller, ANewton]:
@@ -62,22 +66,28 @@
     assert abs(f(x)) < eps
 
 def test_multiplicity():
     for i in range(1, 5):
         assert multiplicity(lambda x: (x - 1)**i, 1) == i
     assert multiplicity(lambda x: x**2, 1) == 0
 
-def test_multidimensional():
+def test_multidimensional(capsys):
     def f(*x):
         return [3*x[0]**2-2*x[1]**2-1, x[0]**2-2*x[0]+x[1]**2+2*x[1]-8]
     assert mnorm(jacobian(f, (1,-2)) - matrix([[6,8],[0,-2]]),1) < 1.e-7
     for x, error in MDNewton(mp, f, (1,-2), verbose=0,
                              norm=lambda x: norm(x, inf)):
         pass
     assert norm(f(*x), 2) < 1e-14
+    for x, error in MDNewton(mp, f, (1,-2), verbose=1,
+                             norm=lambda x: norm(x, inf)):
+        pass
+    assert norm(f(*x), 2) < 1e-14
+    captured = capsys.readouterr()
+    assert captured.out.find("canceled, won't get more exact") >= 0
     # The Chinese mathematician Zhu Shijie was the very first to solve this
     # nonlinear system 700 years ago
     f1 = lambda x, y: -x + 2*y
     f2 = lambda x, y: (x**2 + x*(y**2 - 2) - 4*y)  /  (x + 4)
     f3 = lambda x, y: sqrt(x**2 + y**2)
     def f(x, y):
         f1x = f1(x, y)
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_special.py` & `mpmath-1.4.0a0/mpmath/tests/test_special.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from mpmath import *
+from mpmath import atan, exp, inf, isinf, isnan, log, mpf, nan, pi, sin, sqrt
+
 
 def test_special():
     assert inf == inf
     assert inf != -inf
     assert -inf == -inf
     assert inf != nan
     assert nan != nan
@@ -62,23 +63,24 @@
     assert isinf(inf)
     assert isinf(-inf)
     assert not isinf(mpf(0))
     assert not isinf(nan)
 
 def test_special_powers():
     assert inf**3 == inf
-    assert isnan(inf**0)
+    assert inf**0 == 1
     assert inf**-3 == 0
     assert (-inf)**2 == inf
     assert (-inf)**3 == -inf
-    assert isnan((-inf)**0)
+    assert (-inf)**0 == 1
     assert (-inf)**-2 == 0
     assert (-inf)**-3 == 0
     assert isnan(nan**5)
-    assert isnan(nan**0)
+    assert nan**0 == 1
+    assert 1**inf == 1
 
 def test_functions_special():
     assert exp(inf) == inf
     assert exp(-inf) == 0
     assert isnan(exp(nan))
     assert log(inf) == inf
     assert isnan(log(nan))
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_str.py` & `mpmath-1.4.0a0/mpmath/tests/test_str.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from mpmath import nstr, matrix, inf
+from mpmath import inf, matrix, nstr
+
 
 def test_nstr():
     m = matrix([[0.75, 0.190940654, -0.0299195971],
                 [0.190940654, 0.65625, 0.205663228],
                 [-0.0299195971, 0.205663228, 0.64453125e-20]])
     assert nstr(m, 4, min_fixed=-inf) == \
     '''[    0.75  0.1909                    -0.02992]
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_summation.py` & `mpmath-1.4.0a0/mpmath/tests/test_summation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from mpmath import *
+from mpmath import (e, exp, fac, factorial, fp, fprod, fsum, inf, isnan, iv, j,
+                    log, mpi, nprod, nsum, pi, sumem)
+
 
 def test_sumem():
-    mp.dps = 15
     assert sumem(lambda k: 1/k**2.5, [50, 100]).ae(0.0012524505324784962)
     assert sumem(lambda k: k**4 + 3*k + 1, [10, 100]).ae(2050333103)
 
 def test_nsum():
-    mp.dps = 15
     assert nsum(lambda x: x**2, [1, 3]) == 14
     assert nsum(lambda k: 1/factorial(k), [0, inf]).ae(e)
     assert nsum(lambda k: (-1)**(k+1) / k, [1, inf]).ae(log(2))
     assert nsum(lambda k: (-1)**(k+1) / k**2, [1, inf]).ae(pi**2 / 12)
     assert nsum(lambda k: (-1)**k / log(k), [2, inf]).ae(0.9242998972229388)
     assert nsum(lambda k: 1/k**2, [1, inf]).ae(pi**2 / 6)
     assert nsum(lambda k: 2**k/fac(k), [0, inf]).ae(exp(2))
     assert nsum(lambda k: 1/k**2, [4, inf], method='e').ae(0.2838229557371153)
     assert abs(fp.nsum(lambda k: 1/k**4, [1, fp.inf]) - 1.082323233711138) < 1e-5
     assert abs(fp.nsum(lambda k: 1/k**4, [1, fp.inf], method='e') - 1.082323233711138) < 1e-4
 
 def test_nprod():
-    mp.dps = 15
     assert nprod(lambda k: exp(1/k**2), [1,inf], method='r').ae(exp(pi**2/6))
     assert nprod(lambda x: x**2, [1, 3]) == 36
 
 def test_fsum():
-    mp.dps = 15
     assert fsum([]) == 0
     assert fsum([-4]) == -4
     assert fsum([2,3]) == 5
     assert fsum([1e-100,1]) == 1
     assert fsum([1,1e-100]) == 1
     assert fsum([1e100,1]) == 1e100
     assert fsum([1,1e100]) == 1e100
@@ -44,10 +42,9 @@
     assert isnan(fsum([inf,-inf]))
     assert fsum([inf,-inf], absolute=1) == inf
     assert fsum([inf,-inf], squared=1) == inf
     assert fsum([inf,-inf], absolute=1, squared=1) == inf
     assert iv.fsum([1,mpi(2,3)]) == mpi(3,4)
 
 def test_fprod():
-    mp.dps = 15
     assert fprod([]) == 1
     assert fprod([2,3]) == 6
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_trig.py` & `mpmath-1.4.0a0/mpmath/tests/test_trig.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from mpmath import *
-from mpmath.libmp import *
+from mpmath import cos, ldexp, mp, mpf, pi, sin, tan
+from mpmath.libmp import (round_ceiling, round_down, round_floor,
+                          round_nearest, round_up)
+
 
 def test_trig_misc_hard():
-    mp.prec = 53
     # Worst-case input for an IEEE double, from a paper by Kahan
     x = ldexp(6381956970095103,797)
     assert cos(x) == mpf('-4.6871659242546277e-19')
     assert sin(x) == 1
 
     mp.prec = 150
     a = mpf(10**50)
@@ -24,16 +25,14 @@
     assert cos(-1e-6j).ae(1.0000000000005)
     assert tan(1e-100) == 1e-100
     assert tan(1e-6).ae(1.0000000000003335e-006, rel_eps=2e-15, abs_eps=0)
     assert tan(1e-6j).ae(9.9999999999966644e-007j, rel_eps=2e-15, abs_eps=0)
     assert tan(-1e-6j).ae(-9.9999999999966644e-007j, rel_eps=2e-15, abs_eps=0)
 
 def test_trig_near_zero():
-    mp.dps = 15
-
     for r in [round_nearest, round_down, round_up, round_floor, round_ceiling]:
         assert sin(0, rounding=r) == 0
         assert cos(0, rounding=r) == 1
 
     a = mpf('1e-100')
     b = mpf('-1e-100')
 
@@ -57,16 +56,14 @@
     assert cos(b, rounding=round_down) < 1
     assert cos(b, rounding=round_floor) < 1
     assert cos(b, rounding=round_up) == 1
     assert cos(b, rounding=round_ceiling) == 1
 
 
 def test_trig_near_n_pi():
-
-    mp.dps = 15
     a = [n*pi for n in [1, 2, 6, 11, 100, 1001, 10000, 100001]]
     mp.dps = 135
     a.append(10**100 * pi)
     mp.dps = 15
 
     assert sin(a[0]) == mpf('1.2246467991473531772e-16')
     assert sin(a[1]) == mpf('-2.4492935982947063545e-16')
@@ -128,9 +125,7 @@
     assert cos(a[2], rounding=r) == 1
     assert cos(a[3], rounding=r) > -1
     assert cos(a[4], rounding=r) == 1
     assert cos(a[5], rounding=r) > -1
     assert cos(a[6], rounding=r) == 1
     assert cos(a[7], rounding=r) > -1
     assert cos(a[8], rounding=r) == 1
-
-    mp.dps = 15
```

### Comparing `mpmath-1.3.0/mpmath/tests/test_visualization.py` & `mpmath-1.4.0a0/mpmath/tests/test_visualization.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Limited tests of the visualization module. Right now it just makes
 sure that passing custom Axes works.
 
 """
 
-from mpmath import mp, fp
+from mpmath import fp, mp
+
 
 def test_axes():
     try:
         import matplotlib
         version = matplotlib.__version__.split("-")[0]
         version = version.split(".")[:2]
         if [int(_) for _ in version] < [0,99]:
```

### Comparing `mpmath-1.3.0/mpmath/usertools.py` & `mpmath-1.4.0a0/mpmath/usertools.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     Returns a wrapped copy of *f* that monitors evaluation by calling
     *input* with every input (*args*, *kwargs*) passed to *f* and
     *output* with every value returned from *f*. The default action
     (specify using the special string value ``'print'``) is to print
     inputs and outputs to stdout, along with the total evaluation
     count::
 
-        >>> from mpmath import *
-        >>> mp.dps = 5; mp.pretty = False
+        >>> from mpmath import mp, diff, monitor, exp, findroot, sin
+        >>> mp.dps = 5
         >>> diff(monitor(exp), 1)   # diff will eval f(x-h) and f(x+h)
         in  0 (mpf('0.99999999906867742538452148'),) {}
         out 0 mpf('2.7182818259274480055282064')
         in  1 (mpf('1.0000000009313225746154785'),) {}
         out 1 mpf('2.7182818309906424675501024')
         mpf('2.7182808')
 
@@ -80,14 +80,14 @@
     else:
         g = f
     from timeit import default_timer as clock
     t1=clock(); v=g(); t2=clock(); t=t2-t1
     if t > 0.05 or once:
         return t
     for i in range(3):
-        t1=clock();
+        t1=clock()
         # Evaluate multiple times because the timer function
         # has a significant overhead
         g();g();g();g();g();g();g();g();g();g()
         t2=clock()
         t=min(t,(t2-t1)/10)
     return t
```

### Comparing `mpmath-1.3.0/mpmath/visualization.py` & `mpmath-1.4.0a0/mpmath/visualization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Plotting (requires matplotlib)
 """
 
 from colorsys import hsv_to_rgb, hls_to_rgb
 from .libmp import NoConvergence
-from .libmp.backend import xrange
 
-class VisualizationMethods(object):
+class VisualizationMethods:
     plot_ignore = (ValueError, ArithmeticError, ZeroDivisionError, NoConvergence)
 
 def plot(ctx, f, xlim=[-5,5], ylim=None, points=200, file=None, dpi=None,
     singularities=[], axes=None):
     r"""
     Shows a simple 2D plot of a function `f(x)` or list of functions
     `[f_0(x), f_1(x), \ldots, f_n(x)]` over a given interval
@@ -49,15 +48,15 @@
     a, b = xlim
     colors = ['b', 'r', 'g', 'm', 'k']
     for n, func in enumerate(f):
         x = ctx.arange(a, b, (b-a)/float(points))
         segments = []
         segment = []
         in_complex = False
-        for i in xrange(len(x)):
+        for i in range(len(x)):
             try:
                 if i != 0:
                     for sing in singularities:
                         if x[i-1] <= sing and x[i] >= sing:
                             raise ValueError
                 v = func(x[i])
                 if ctx.isnan(v) or abs(v) > 1e300:
@@ -199,16 +198,16 @@
     x = pylab.linspace(rea, reb, M)
     y = pylab.linspace(ima, imb, N)
     # Note: we have to be careful to get the right rotation.
     # Test with these plots:
     #   cplot(lambda z: z if z.real < 0 else 0)
     #   cplot(lambda z: z if z.imag < 0 else 0)
     w = pylab.zeros((N, M, 3))
-    for n in xrange(N):
-        for m in xrange(M):
+    for n in range(N):
+        for m in range(M):
             z = ctx.mpc(x[m], y[n])
             try:
                 v = color(f(z))
             except ctx.plot_ignore:
                 v = (0.5, 0.5, 0.5)
             w[n,m] = v
         if verbose:
@@ -233,47 +232,46 @@
     `x = u` and `y = v`.
 
     If `f` returns three components, then this plots the parametric
     surface `x, y, z = f(u,v)` over the pairs of intervals `u` and `v`.
 
     For example, to plot a simple function::
 
-        >>> from mpmath import *
+        >>> from mpmath import sin, cos, pi, splot
         >>> f = lambda x, y: sin(x+y)*cos(y)
         >>> splot(f, [-pi,pi], [-pi,pi])    # doctest: +SKIP
 
     Plotting a donut::
 
         >>> r, R = 1, 2.5
         >>> f = lambda u, v: [r*cos(u), (R+r*sin(u))*cos(v), (R+r*sin(u))*sin(v)]
         >>> splot(f, [0, 2*pi], [0, 2*pi])    # doctest: +SKIP
 
     .. note :: This function requires matplotlib (pylab) 0.98.5.3 or higher.
     """
-    import pylab
-    import mpl_toolkits.mplot3d as mplot3d
+    import matplotlib.pyplot as plt
+    import numpy as np
     if file:
         axes = None
     fig = None
     if not axes:
-        fig = pylab.figure()
-        axes = mplot3d.axes3d.Axes3D(fig)
-    ua, ub = u
-    va, vb = v
+        fig, axes = plt.subplots(subplot_kw={'projection': '3d'})
+    ua, ub = map(float, u)
+    va, vb = map(float, v)
     du = ub - ua
     dv = vb - va
     if not isinstance(points, (list, tuple)):
         points = [points, points]
     M, N = points
-    u = pylab.linspace(ua, ub, M)
-    v = pylab.linspace(va, vb, N)
-    x, y, z = [pylab.zeros((M, N)) for i in xrange(3)]
-    xab, yab, zab = [[0, 0] for i in xrange(3)]
-    for n in xrange(N):
-        for m in xrange(M):
+    u = np.linspace(ua, ub, M)
+    v = np.linspace(va, vb, N)
+    x, y, z = [np.zeros((M, N)) for i in range(3)]
+    xab, yab, zab = [[0, 0] for i in range(3)]
+    for n in range(N):
+        for m in range(M):
             fdata = f(ctx.convert(u[m]), ctx.convert(v[n]))
             try:
                 x[m,n], y[m,n], z[m,n] = fdata
             except TypeError:
                 x[m,n], y[m,n], z[m,n] = u[m], v[n], fdata
             for c, cab in [(x[m,n], xab), (y[m,n], yab), (z[m,n], zab)]:
                 if c < cab[0]:
@@ -297,17 +295,17 @@
             delta = maxd - dy
             axes.set_ylim3d(yab[0] - delta / 2.0, yab[1] + delta / 2.0)
         if dz < maxd:
             delta = maxd - dz
             axes.set_zlim3d(zab[0] - delta / 2.0, zab[1] + delta / 2.0)
     if fig:
         if file:
-            pylab.savefig(file, dpi=dpi)
+            plt.savefig(file, dpi=dpi)
         else:
-            pylab.show()
+            plt.show()
 
 
 VisualizationMethods.plot = plot
 VisualizationMethods.default_color_function = default_color_function
 VisualizationMethods.phase_color_function = phase_color_function
 VisualizationMethods.cplot = cplot
 VisualizationMethods.splot = splot
```

### Comparing `mpmath-1.3.0/mpmath.egg-info/PKG-INFO` & `mpmath-1.4.0a0/mpmath.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 Metadata-Version: 2.1
 Name: mpmath
-Version: 1.3.0
+Version: 1.4.0a0
 Summary: Python library for arbitrary-precision floating-point arithmetic
-Home-page: http://mpmath.org/
-Author: Fredrik Johansson
-Author-email: fredrik.johansson@gmail.com
+Author-email: Fredrik Johansson <fredrik.johansson@gmail.com>
 License: BSD
-Project-URL: Source, https://github.com/fredrik-johansson/mpmath
-Project-URL: Tracker, https://github.com/fredrik-johansson/mpmath/issues
+Project-URL: Homepage, https://mpmath.org/
+Project-URL: Source Code, https://github.com/mpmath/mpmath
+Project-URL: Bug Tracker, https://github.com/mpmath/mpmath/issues
 Project-URL: Documentation, http://mpmath.org/doc/current/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: tests
+Requires-Dist: pytest>=6; extra == "tests"
+Requires-Dist: numpy<=1.25.2; python_version < "3.12" and extra == "tests"
 Provides-Extra: develop
+Requires-Dist: mpmath[tests]; extra == "develop"
+Requires-Dist: flake518>=1.5; python_version >= "3.9" and extra == "develop"
+Requires-Dist: pytest-cov; extra == "develop"
+Requires-Dist: wheel; extra == "develop"
+Requires-Dist: build; extra == "develop"
 Provides-Extra: gmpy
+Requires-Dist: gmpy2>=2.1.0a4; (platform_python_implementation != "PyPy" and python_version < "3.12") and extra == "gmpy"
+Requires-Dist: gmpy2>=2.2.0a1; (platform_python_implementation != "PyPy" and python_version >= "3.12") and extra == "gmpy"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Provides-Extra: ci
+Requires-Dist: pytest-xdist; extra == "ci"
 
 mpmath
 ======
 
 |pypi version| |Build status| |Code coverage status| |Zenodo Badge|
 
 .. |pypi version| image:: https://img.shields.io/pypi/v/mpmath.svg
    :target: https://pypi.python.org/pypi/mpmath
-.. |Build status| image:: https://github.com/fredrik-johansson/mpmath/workflows/test/badge.svg
-   :target: https://github.com/fredrik-johansson/mpmath/actions?workflow=test
-.. |Code coverage status| image:: https://codecov.io/gh/fredrik-johansson/mpmath/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/fredrik-johansson/mpmath
+.. |Build status| image:: https://github.com/mpmath/mpmath/workflows/test/badge.svg
+   :target: https://github.com/mpmath/mpmath/actions?workflow=test
+.. |Code coverage status| image:: https://codecov.io/gh/mpmath/mpmath/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/mpmath/mpmath
 .. |Zenodo Badge| image:: https://zenodo.org/badge/2934512.svg
    :target: https://zenodo.org/badge/latestdoi/2934512
 
 A Python library for arbitrary-precision floating-point arithmetic.
 
-Website: http://mpmath.org/
+Website: https://mpmath.org/
 Main author: Fredrik Johansson <fredrik.johansson@gmail.com>
 
 Mpmath is free software released under the New BSD License (see the
-LICENSE file for details)
+LICENSE file for details).
 
 0. History and credits
 ----------------------
 
 The following people (among others) have contributed major patches
 or new features to mpmath:
 
@@ -113,14 +125,15 @@
   implementations.
 * George Brandl for developing the Sphinx documentation tool
   used to build mpmath's documentation
 
 Release history:
 
 * Version 1.3.0 released on March 7, 2023
+* Version 1.2.1 released on February 9, 2021
 * Version 1.2.0 released on February 1, 2021
 * Version 1.1.0 released on December 11, 2018
 * Version 1.0.0 released on September 27, 2017
 * Version 0.19 released on June 10, 2014
 * Version 0.18 released on December 31, 2013
 * Version 0.17 released on February 1, 2011
 * Version 0.16 released on September 24, 2010
@@ -139,66 +152,58 @@
 * Version 0.3 released on October 5, 2007
 * Version 0.2 released on October 2, 2007
 * Version 0.1 released on September 27, 2007
 
 1. Download & installation
 --------------------------
 
-Mpmath requires Python 2.7 or 3.5 (or later versions). It has been tested
-with CPython 2.7, 3.5 through 3.7 and for PyPy.
+Mpmath requires Python 3.8 or later versions. It has been tested
+with CPython 3.8 through 3.12 and for PyPy.
 
 The latest release of mpmath can be downloaded from the mpmath
-website and from https://github.com/fredrik-johansson/mpmath/releases
+website and from https://github.com/mpmath/mpmath/releases
 
 It should also be available in the Python Package Index at
 https://pypi.python.org/pypi/mpmath
 
 To install latest release of Mpmath with pip, simply run
 
 ``pip install mpmath``
 
-Or unpack the mpmath archive and run
-
-``python setup.py install``
-
-Mpmath can also be installed using
+or from the source tree
 
-``python -m easy_install mpmath``
+``pip install .``
 
 The latest development code is available from
-https://github.com/fredrik-johansson/mpmath
+https://github.com/mpmath/mpmath
 
 See the main documentation for more detailed instructions.
 
-2. Running tests
+2. Documentation
 ----------------
 
-The unit tests in mpmath/tests/ can be run via the script
-runtests.py, but it is recommended to run them with py.test
-(https://pytest.org/), especially
-to generate more useful reports in case there are failures.
+Documentation in reStructuredText format is available in the
+docs directory included with the source package. These files
+are human-readable, but can be compiled to prettier HTML using
+`Sphinx <https://www.sphinx-doc.org/>`_.
 
-You may also want to check out the demo scripts in the demo
-directory.
+The most recent documentation is also available in HTML format:
 
-The master branch is automatically tested by Travis CI.
+https://mpmath.org/doc/current/
 
-3. Documentation
+3. Running tests
 ----------------
 
-Documentation in reStructuredText format is available in the
-doc directory included with the source package. These files
-are human-readable, but can be compiled to prettier HTML using
-the build.py script (requires Sphinx, http://sphinx.pocoo.org/).
-
-See setup.txt in the documentation for more information.
+The unit tests in mpmath/tests/ can be run with `pytest
+<https://pytest.org/>`_, see the main documentation.
 
-The most recent documentation is also available in HTML format:
+You may also want to check out the demo scripts in the demo
+directory.
 
-http://mpmath.org/doc/current/
+The master branch is automatically tested on the Github Actions.
 
 4. Known problems
 -----------------
 
 Mpmath is a work in progress. Major issues include:
 
 * Some functions may return incorrect values when given extremely
@@ -215,11 +220,11 @@
 * The interface for switching precision and rounding is not finalized.
   The current method is not threadsafe.
 
 5. Help and bug reports
 -----------------------
 
 General questions and comments can be sent to the mpmath mailinglist,
-mpmath@googlegroups.com
+mailto:mpmath@googlegroups.com
 
 You can also report bugs and send patches to the mpmath issue tracker,
-https://github.com/fredrik-johansson/mpmath/issues
+https://github.com/mpmath/mpmath/issues
```

