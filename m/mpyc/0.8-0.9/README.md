# Comparing `tmp/mpyc-0.8.tar.gz` & `tmp/mpyc-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpyc-0.8.tar", last modified: Mon Dec 27 13:11:33 2021, max compression
+gzip compressed data, was "mpyc-0.9.tar", last modified: Sun Feb 26 21:56:06 2023, max compression
```

## Comparing `mpyc-0.8.tar` & `mpyc-0.9.tar`

### file list

```diff
@@ -1,28 +1,43 @@
-drwxrwxrwx   0        0        0        0 2021-12-27 13:11:33.574577 mpyc-0.8/
--rw-rw-rw-   0        0        0     1096 2019-08-31 08:41:12.000000 mpyc-0.8/LICENSE
--rw-rw-rw-   0        0        0       92 2021-12-27 12:52:13.000000 mpyc-0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5194 2021-12-27 13:11:33.574577 mpyc-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3907 2021-12-24 17:54:13.000000 mpyc-0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-12-27 13:11:33.555343 mpyc-0.8/mpyc/
--rw-rw-rw-   0        0        0     1669 2021-12-27 11:36:50.000000 mpyc-0.8/mpyc/__init__.py
--rw-rw-rw-   0        0        0     7055 2021-12-24 17:55:29.000000 mpyc-0.8/mpyc/__main__.py
--rw-rw-rw-   0        0        0    13385 2021-12-24 17:55:29.000000 mpyc-0.8/mpyc/asyncoro.py
--rw-rw-rw-   0        0        0    18302 2021-11-27 11:31:03.000000 mpyc-0.8/mpyc/finfields.py
--rw-rw-rw-   0        0        0    43082 2021-12-27 11:36:50.000000 mpyc-0.8/mpyc/fingroups.py
--rw-rw-rw-   0        0        0    24210 2021-12-22 14:56:17.000000 mpyc-0.8/mpyc/gfpx.py
--rw-rw-rw-   0        0        0     7286 2021-12-27 11:36:50.000000 mpyc-0.8/mpyc/gmpy.py
--rw-rw-rw-   0        0        0     2683 2021-11-27 11:31:03.000000 mpyc-0.8/mpyc/mpctools.py
--rw-rw-rw-   0        0        0     9513 2021-12-24 17:55:29.000000 mpyc-0.8/mpyc/random.py
--rw-rw-rw-   0        0        0    87576 2021-12-27 11:36:50.000000 mpyc-0.8/mpyc/runtime.py
--rw-rw-rw-   0        0        0    24360 2021-12-24 17:55:29.000000 mpyc-0.8/mpyc/secgroups.py
--rw-rw-rw-   0        0        0    15008 2021-11-27 11:31:03.000000 mpyc-0.8/mpyc/seclists.py
--rw-rw-rw-   0        0        0    28898 2021-12-24 17:55:29.000000 mpyc-0.8/mpyc/sectypes.py
--rw-rw-rw-   0        0        0    23386 2021-12-24 17:55:29.000000 mpyc-0.8/mpyc/statistics.py
--rw-rw-rw-   0        0        0     5951 2020-10-24 17:31:50.000000 mpyc-0.8/mpyc/thresha.py
-drwxrwxrwx   0        0        0        0 2021-12-27 13:11:33.573577 mpyc-0.8/mpyc.egg-info/
--rw-rw-rw-   0        0        0     5194 2021-12-27 13:11:33.000000 mpyc-0.8/mpyc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2021-12-27 13:11:33.000000 mpyc-0.8/mpyc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-27 13:11:33.000000 mpyc-0.8/mpyc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2021-12-27 13:11:33.000000 mpyc-0.8/mpyc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2021-12-27 13:11:33.576575 mpyc-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1711 2020-11-01 08:27:33.000000 mpyc-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:56:06.144403 mpyc-0.9/
+-rw-rw-rw-   0        0        0     1096 2019-08-31 08:41:12.000000 mpyc-0.9/LICENSE
+-rw-rw-rw-   0        0        0       89 2021-12-27 13:28:40.000000 mpyc-0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5199 2023-02-26 21:56:06.144403 mpyc-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3919 2023-02-26 21:45:19.000000 mpyc-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-26 21:56:06.050657 mpyc-0.9/mpyc/
+-rw-rw-rw-   0        0        0     8352 2023-02-26 21:45:19.000000 mpyc-0.9/mpyc/__init__.py
+-rw-rw-rw-   0        0        0     6848 2022-06-29 06:19:42.000000 mpyc-0.9/mpyc/__main__.py
+-rw-rw-rw-   0        0        0    14378 2023-02-23 18:19:37.000000 mpyc-0.9/mpyc/asyncoro.py
+-rw-rw-rw-   0        0        0    47985 2023-02-26 21:45:19.000000 mpyc-0.9/mpyc/finfields.py
+-rw-rw-rw-   0        0        0    44085 2022-12-03 10:54:07.000000 mpyc-0.9/mpyc/fingroups.py
+-rw-rw-rw-   0        0        0    24441 2022-08-10 17:38:36.000000 mpyc-0.9/mpyc/gfpx.py
+-rw-rw-rw-   0        0        0     7324 2023-01-27 11:42:32.000000 mpyc-0.9/mpyc/gmpy.py
+-rw-rw-rw-   0        0        0     2683 2021-11-27 11:31:03.000000 mpyc-0.9/mpyc/mpctools.py
+-rw-rw-rw-   0        0        0     7515 2023-02-26 21:45:19.000000 mpyc-0.9/mpyc/numpy.py
+-rw-rw-rw-   0        0        0    10260 2023-01-28 13:51:18.000000 mpyc-0.9/mpyc/random.py
+-rw-rw-rw-   0        0        0   140667 2023-02-26 21:45:19.000000 mpyc-0.9/mpyc/runtime.py
+-rw-rw-rw-   0        0        0    24692 2022-09-17 09:27:45.000000 mpyc-0.9/mpyc/secgroups.py
+-rw-rw-rw-   0        0        0    14528 2022-06-29 06:19:42.000000 mpyc-0.9/mpyc/seclists.py
+-rw-rw-rw-   0        0        0    47871 2023-02-26 21:45:19.000000 mpyc-0.9/mpyc/sectypes.py
+-rw-rw-rw-   0        0        0    22394 2022-06-29 06:19:42.000000 mpyc-0.9/mpyc/statistics.py
+-rw-rw-rw-   0        0        0     9297 2023-02-25 13:07:59.000000 mpyc-0.9/mpyc/thresha.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:56:06.050657 mpyc-0.9/mpyc.egg-info/
+-rw-rw-rw-   0        0        0     5199 2023-02-26 21:56:05.000000 mpyc-0.9/mpyc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-02-26 21:56:05.000000 mpyc-0.9/mpyc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-26 21:56:05.000000 mpyc-0.9/mpyc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-02-26 21:56:05.000000 mpyc-0.9/mpyc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-02-26 21:56:06.144403 mpyc-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1545 2022-06-29 06:19:42.000000 mpyc-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:56:06.144403 mpyc-0.9/tests/
+-rw-rw-rw-   0        0        0    23127 2023-02-21 14:11:15.000000 mpyc-0.9/tests/test_finfields.py
+-rw-rw-rw-   0        0        0     6878 2022-06-18 11:42:54.000000 mpyc-0.9/tests/test_fingroups.py
+-rw-rw-rw-   0        0        0    10731 2022-05-05 08:20:19.000000 mpyc-0.9/tests/test_gfpx.py
+-rw-rw-rw-   0        0        0     4333 2022-11-11 11:40:52.000000 mpyc-0.9/tests/test_gmpy.py
+-rw-rw-rw-   0        0        0     2226 2021-11-27 11:31:03.000000 mpyc-0.9/tests/test_mpctools.py
+-rw-rw-rw-   0        0        0     3349 2022-09-02 11:56:40.000000 mpyc-0.9/tests/test_numpy.py
+-rw-rw-rw-   0        0        0     7220 2022-12-01 09:09:11.000000 mpyc-0.9/tests/test_random.py
+-rw-rw-rw-   0        0        0    49629 2023-02-26 21:45:19.000000 mpyc-0.9/tests/test_runtime.py
+-rw-rw-rw-   0        0        0     6733 2022-06-18 11:42:54.000000 mpyc-0.9/tests/test_secgroups.py
+-rw-rw-rw-   0        0        0     5842 2021-11-27 11:31:03.000000 mpyc-0.9/tests/test_seclists.py
+-rw-rw-rw-   0        0        0     7996 2023-01-27 11:42:32.000000 mpyc-0.9/tests/test_sectypes.py
+-rw-rw-rw-   0        0        0     8318 2022-06-29 06:19:42.000000 mpyc-0.9/tests/test_statistics.py
+-rw-rw-rw-   0        0        0     3361 2022-09-17 09:27:45.000000 mpyc-0.9/tests/test_thresha.py
```

### Comparing `mpyc-0.8/LICENSE` & `mpyc-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mpyc-0.8/PKG-INFO` & `mpyc-0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mpyc
-Version: 0.8
-Summary: MPyC -- Secure Multiparty Computation in Python
+Version: 0.9
+Summary: MPyC for Multiparty Computation in Python
 Home-page: https://github.com/lschoe/mpyc
 Author: Berry Schoenmakers
 Author-email: berry@win.tue.nl
 License: MIT License
 Keywords: crypto,cryptography,multiparty computation,MPC,secret sharing,Shamir threshold scheme,pseudorandom secret sharing,PRSS
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -19,69 +19,69 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lschoe/mpyc/master)
 [![Travis CI](https://app.travis-ci.com/lschoe/mpyc.svg)](https://app.travis-ci.com/lschoe/mpyc)
 [![codecov](https://codecov.io/gh/lschoe/mpyc/branch/master/graph/badge.svg)](https://codecov.io/gh/lschoe/mpyc)
 [![Read the Docs](https://readthedocs.org/projects/mpyc/badge/)](https://mpyc.readthedocs.io)
 [![PyPI](https://img.shields.io/pypi/v/mpyc.svg)](https://pypi.org/project/mpyc/)
 
-# MPyC [![MPyC logo](https://raw.githubusercontent.com/lschoe/mpyc/master/images/MPyC_Logo.svg)](https://github.com/lschoe/mpyc) Secure Multiparty Computation in Python
+# MPyC [![MPyC logo](https://raw.githubusercontent.com/lschoe/mpyc/master/images/MPyC_Logo.svg)](https://github.com/lschoe/mpyc) Multiparty Computation in Python
 
 MPyC supports secure *m*-party computation tolerating a dishonest minority of up to *t* passively corrupt parties,
 where *m &ge; 1* and *0 &le; t &lt; m/2*. The underlying cryptographic protocols are based on threshold secret sharing over finite
 fields (using Shamir's threshold scheme as well as pseudorandom secret sharing).
 
 The details of the secure computation protocols are mostly transparent due to the use of sophisticated operator overloading
 combined with asynchronous evaluation of the associated protocols.
 
-See the [MPyC homepage](https://www.win.tue.nl/~berry/mpyc/) for more info and background.
+## Documentation
 
-Click the "launch binder" badge above to view the entire repository and try out the Jupyter notebooks from the `demos` directory
-in the cloud, without any install.
+[Read the Docs](https://mpyc.readthedocs.io/) for `Sphinx`-based documentation, including an overview of the `demos`.\
+[GitHub Pages](https://lschoe.github.io/mpyc/) for `pydoc`-based documentation.
 
-## Installation:
+See `demos` for Python programs and Jupyter notebooks with lots of example code. Click the "launch binder" badge above to view the entire
+repository and try out the Jupyter notebooks from the `demos` directory in the cloud, without any install.
 
-Just run: `python setup.py install` (pure Python, no dependencies).
+The [MPyC homepage](https://www.win.tue.nl/~berry/mpyc/) has some more info and background.
 
-See `demos` for Python programs and Jupyter notebooks with lots of example code.
+## Installation
 
-See [Read the Docs](https://mpyc.readthedocs.io/) for `Sphinx`-based documentation, including an overview of the `demos`,
-and [GitHub Pages](https://lschoe.github.io/mpyc/) for `pydoc`-based documentation.
+Pure Python, no dependencies. Python 3.8+ (following [NumPy's deprecation policy](https://numpy.org/neps/nep-0029-deprecation_policy.html#support-table)).
 
-## Notes:
+Run `pip install .` in the root directory (containing file `setup.py`).\
+Or, run `pip install -e .`, if you want to edit the MPyC source files.
 
-1. Python 3.6+ (Python 3.5 or lower is not sufficient).
+Use `pip install numpy` to enable support for secure NumPy arrays in MPyC, along with vectorized implementations.
 
-2. Installing package [gmpy2](https://pypi.org/project/gmpy2/) is optional, but will considerably enhance the performance of `mpyc`.
-As of December 12, 2021 with the release of gmpy2 2.1, installation has been simplified greatly:
-`pip install gmpy2` is now supported on all major Linux/MacOS/Windows platforms via prebuilt wheels.
-If you use the [conda](https://docs.conda.io/) package and environment manager, `conda install gmpy2` should do the job.
+Use `pip install gmpy2` to run MPyC with the package [gmpy2](https://pypi.org/project/gmpy2/) for considerably better performance.
 
-3. Use `run-all.sh` or `run-all.bat` in the `demos` directory to have a quick look at all pure Python demos.
+### Some Tips
+
+- Try `run-all.sh` or `run-all.bat` in the `demos` directory to have a quick look at all pure Python demos.
 Demos `bnnmnist.py` and `cnnmnist.py` require [NumPy](https://www.numpy.org/), demo `kmsurvival.py` requires
 [pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), and [lifelines](https://pypi.org/project/lifelines/),
-and demo `ridgeregression.py` (and therefore demo `multilateration.py`) even require [Scikit-learn](https://scikit-learn.org/).
-Also note the example Linux shell scripts and Windows batch files in the `docs` and `tests` directories.
-
-4. Directory `demos\.config` contains configuration info used to run MPyC with multiple parties. Also, Windows batch
-file `gen.bat` shows how to generate fresh key material for SSL. To generate SSL key material of your own, first run
-`pip install cryptography` (alternatively, run `pip install pyOpenSSL`, which will also install the `cryptography` package).
-
-5. To use the [Jupyter](https://jupyter.org/) notebooks `demos\*.ipynb`, you need to have Jupyter installed,
-e.g., using `pip install jupyter`. The latest version of Jupyter will come with IPython 7.x, which supports
-top-level `await`. For example, instead of `mpc.run(mpc.start())` one can now simply write `await mpc.start()` anywhere in
-a notebook cell, even outside a coroutine.
-
-6. For Python 3.8+, you also get top-level `await` by running `python -m asyncio` to launch a natively async REPL.
+and demo `ridgeregression.py` (and therefore demo `multilateration.py`) even require [Scikit-learn](https://scikit-learn.org/).\
+Try `np-run-all.sh` or `np-run-all.bat` in the `demos` directory to run all Python demos employing MPyC's secure arrays.
+Major speedups are achieved due to the reduced overhead of secure arrays and vectorized processing throughout the
+protocols.
+
+- To use the [Jupyter](https://jupyter.org/) notebooks `demos\*.ipynb`, you need to have Jupyter installed,
+e.g., using `pip install jupyter`. An interesting feature of Jupyter is the support of top-level `await`.
+For example, instead of `mpc.run(mpc.start())` you can simply use `await mpc.start()` anywhere in
+a notebook cell, even outside a coroutine.\
+For Python, you also get top-level `await` by running `python -m asyncio` to launch a natively async REPL.
 By running `python -m mpyc` instead you even get this REPL with the MPyC runtime preloaded!
 
-Copyright &copy; 2018-2021 Berry Schoenmakers
+- Directory `demos\.config` contains configuration info used to run MPyC with multiple parties.
+The file `gen.bat` shows how to generate fresh key material for SSL. To generate SSL key material of your own, first run
+`pip install cryptography` (alternatively, run `pip install pyOpenSSL`).
 
+Copyright &copy; 2018-2023 Berry Schoenmakers
```

### Comparing `mpyc-0.8/README.md` & `mpyc-0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lschoe/mpyc/master)
 [![Travis CI](https://app.travis-ci.com/lschoe/mpyc.svg)](https://app.travis-ci.com/lschoe/mpyc)
 [![codecov](https://codecov.io/gh/lschoe/mpyc/branch/master/graph/badge.svg)](https://codecov.io/gh/lschoe/mpyc)
 [![Read the Docs](https://readthedocs.org/projects/mpyc/badge/)](https://mpyc.readthedocs.io)
 [![PyPI](https://img.shields.io/pypi/v/mpyc.svg)](https://pypi.org/project/mpyc/)
 
-# MPyC [![MPyC logo](https://raw.githubusercontent.com/lschoe/mpyc/master/images/MPyC_Logo.svg)](https://github.com/lschoe/mpyc) Secure Multiparty Computation in Python
+# MPyC [![MPyC logo](https://raw.githubusercontent.com/lschoe/mpyc/master/images/MPyC_Logo.svg)](https://github.com/lschoe/mpyc) Multiparty Computation in Python
 
 MPyC supports secure *m*-party computation tolerating a dishonest minority of up to *t* passively corrupt parties,
 where *m &ge; 1* and *0 &le; t &lt; m/2*. The underlying cryptographic protocols are based on threshold secret sharing over finite
 fields (using Shamir's threshold scheme as well as pseudorandom secret sharing).
 
 The details of the secure computation protocols are mostly transparent due to the use of sophisticated operator overloading
 combined with asynchronous evaluation of the associated protocols.
 
-See the [MPyC homepage](https://www.win.tue.nl/~berry/mpyc/) for more info and background.
+## Documentation
 
-Click the "launch binder" badge above to view the entire repository and try out the Jupyter notebooks from the `demos` directory
-in the cloud, without any install.
+[Read the Docs](https://mpyc.readthedocs.io/) for `Sphinx`-based documentation, including an overview of the `demos`.\
+[GitHub Pages](https://lschoe.github.io/mpyc/) for `pydoc`-based documentation.
 
-## Installation:
+See `demos` for Python programs and Jupyter notebooks with lots of example code. Click the "launch binder" badge above to view the entire
+repository and try out the Jupyter notebooks from the `demos` directory in the cloud, without any install.
 
-Just run: `python setup.py install` (pure Python, no dependencies).
+The [MPyC homepage](https://www.win.tue.nl/~berry/mpyc/) has some more info and background.
 
-See `demos` for Python programs and Jupyter notebooks with lots of example code.
+## Installation
 
-See [Read the Docs](https://mpyc.readthedocs.io/) for `Sphinx`-based documentation, including an overview of the `demos`,
-and [GitHub Pages](https://lschoe.github.io/mpyc/) for `pydoc`-based documentation.
+Pure Python, no dependencies. Python 3.8+ (following [NumPy's deprecation policy](https://numpy.org/neps/nep-0029-deprecation_policy.html#support-table)).
 
-## Notes:
+Run `pip install .` in the root directory (containing file `setup.py`).\
+Or, run `pip install -e .`, if you want to edit the MPyC source files.
 
-1. Python 3.6+ (Python 3.5 or lower is not sufficient).
+Use `pip install numpy` to enable support for secure NumPy arrays in MPyC, along with vectorized implementations.
 
-2. Installing package [gmpy2](https://pypi.org/project/gmpy2/) is optional, but will considerably enhance the performance of `mpyc`.
-As of December 12, 2021 with the release of gmpy2 2.1, installation has been simplified greatly:
-`pip install gmpy2` is now supported on all major Linux/MacOS/Windows platforms via prebuilt wheels.
-If you use the [conda](https://docs.conda.io/) package and environment manager, `conda install gmpy2` should do the job.
+Use `pip install gmpy2` to run MPyC with the package [gmpy2](https://pypi.org/project/gmpy2/) for considerably better performance.
 
-3. Use `run-all.sh` or `run-all.bat` in the `demos` directory to have a quick look at all pure Python demos.
+### Some Tips
+
+- Try `run-all.sh` or `run-all.bat` in the `demos` directory to have a quick look at all pure Python demos.
 Demos `bnnmnist.py` and `cnnmnist.py` require [NumPy](https://www.numpy.org/), demo `kmsurvival.py` requires
 [pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), and [lifelines](https://pypi.org/project/lifelines/),
-and demo `ridgeregression.py` (and therefore demo `multilateration.py`) even require [Scikit-learn](https://scikit-learn.org/).
-Also note the example Linux shell scripts and Windows batch files in the `docs` and `tests` directories.
-
-4. Directory `demos\.config` contains configuration info used to run MPyC with multiple parties. Also, Windows batch
-file `gen.bat` shows how to generate fresh key material for SSL. To generate SSL key material of your own, first run
-`pip install cryptography` (alternatively, run `pip install pyOpenSSL`, which will also install the `cryptography` package).
-
-5. To use the [Jupyter](https://jupyter.org/) notebooks `demos\*.ipynb`, you need to have Jupyter installed,
-e.g., using `pip install jupyter`. The latest version of Jupyter will come with IPython 7.x, which supports
-top-level `await`. For example, instead of `mpc.run(mpc.start())` one can now simply write `await mpc.start()` anywhere in
-a notebook cell, even outside a coroutine.
-
-6. For Python 3.8+, you also get top-level `await` by running `python -m asyncio` to launch a natively async REPL.
+and demo `ridgeregression.py` (and therefore demo `multilateration.py`) even require [Scikit-learn](https://scikit-learn.org/).\
+Try `np-run-all.sh` or `np-run-all.bat` in the `demos` directory to run all Python demos employing MPyC's secure arrays.
+Major speedups are achieved due to the reduced overhead of secure arrays and vectorized processing throughout the
+protocols.
+
+- To use the [Jupyter](https://jupyter.org/) notebooks `demos\*.ipynb`, you need to have Jupyter installed,
+e.g., using `pip install jupyter`. An interesting feature of Jupyter is the support of top-level `await`.
+For example, instead of `mpc.run(mpc.start())` you can simply use `await mpc.start()` anywhere in
+a notebook cell, even outside a coroutine.\
+For Python, you also get top-level `await` by running `python -m asyncio` to launch a natively async REPL.
 By running `python -m mpyc` instead you even get this REPL with the MPyC runtime preloaded!
 
-Copyright &copy; 2018-2021 Berry Schoenmakers
+- Directory `demos\.config` contains configuration info used to run MPyC with multiple parties.
+The file `gen.bat` shows how to generate fresh key material for SSL. To generate SSL key material of your own, first run
+`pip install cryptography` (alternatively, run `pip install pyOpenSSL`).
+
+Copyright &copy; 2018-2023 Berry Schoenmakers
```

### Comparing `mpyc-0.8/mpyc/__main__.py` & `mpyc-0.9/mpyc/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Support for natively asynchronous REPL with MPyC preloaded.
 
-To launch a natively asynch REPL (in Python 3.8+) with MPyC preloaded, run:
+To launch a natively asynch REPL with MPyC preloaded, run:
 
     python -m mpyc
 
 This causes Python's asyncio to be preloaded as well, allowing code with
 top-level await expressions to be evaluated directly (instead of using
 calls to mpc.run() or asyncio.run() in top-level code).
 
-Besides setting mpc as a handle for the MPyC runtime, also three secure
+Besides setting mpc as a handle for the MPyC runtime, also several secure
 (secret-shared) types are predefined, effectively executing the following code:
 
     from mpyc.runtime import mpc
     secint = mpc.SecInt()
     secfxp = mpc.SecFxp()
     secflt = mpc.SecFlt()
     secfld127 = mpc.SecFld(127)
@@ -47,18 +47,14 @@
 import concurrent.futures
 import inspect
 import sys
 import threading
 import types
 import warnings
 
-if __name__ == '__main__':
-    from mpyc.runtime import mpc  # NB: included here for -H --HELP for Python 3.7-
-    assert sys.version_info.minor >= 8, 'Python 3.8+ required for asyncio REPL'
-
 
 class AsyncIOInteractiveConsole(code.InteractiveConsole):
     """Adapted from asyncio.__main__.AsyncIOInteractiveConsole with minor changes only."""
 
     def __init__(self, locals, loop=None):
         super().__init__(locals)
         self.compile.compiler.flags |= ast.PyCF_ALLOW_TOP_LEVEL_AWAIT
```

### Comparing `mpyc-0.8/mpyc/asyncoro.py` & `mpyc-0.9/mpyc/asyncoro.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,111 +7,126 @@
 import struct
 import itertools
 import functools
 import typing
 from asyncio import Protocol, Future, Task
 from mpyc.sectypes import SecureObject
 
+runtime = None
+
 
 class MessageExchanger(Protocol):
     """Send and receive messages.
 
     Bidirectional connection with one of the other parties (peers).
     """
 
-    __slots__ = 'runtime', 'peer_pid', 'bytes', 'buffers', 'transport'
+    __slots__ = 'runtime', 'peer_pid', 'bytes', 'buffers', 'transport', 'nbytes_sent'
 
-    def __init__(self, runtime, peer_pid=None):
-        self.runtime = runtime
+    def __init__(self, rt, peer_pid=None):
+        """Initialize protocol for runtime rt between this party and a peer.
+
+        The connection between the two parties will be set up with one party
+        listening (as server) for the other party to connect (as client).
+        If peer_pid=None, party rt.pid starts as server and the peer start as
+        client, and the other way around otherwise. Once the connection is made,
+        the client will immediately send its pid to the server.
+        """
+        self.runtime = rt
         self.peer_pid = peer_pid
         self.bytes = bytearray()
         self.buffers = {}
         self.transport = None
+        self.nbytes_sent = 0
 
     def _key_transport_done(self):
-        self.runtime.parties[self.peer_pid].protocol = self
-        if all(p.protocol is not None for p in self.runtime.parties):
-            self.runtime.parties[self.runtime.pid].protocol.set_result(self.runtime)
+        rt = self.runtime
+        rt.parties[self.peer_pid].protocol = self
+        if all(p.protocol is not None for p in rt.parties):
+            rt.parties[rt.pid].protocol.set_result(None)
 
     def connection_made(self, transport):
         """Called when a connection is made.
 
-        If the party is a client for this connection, it sends its identity
+        If this party is a client for this connection, it sends its identity
         to the peer as well as any PRSS keys.
         """
         self.transport = transport
-        if self.peer_pid is not None:  # party is client (peer is server)
-            m = len(self.runtime.parties)
-            t = self.runtime.threshold
-            pid_keys = [self.runtime.pid.to_bytes(2, 'little')]  # send pid
-            if not self.runtime.options.no_prss:
+        if self.peer_pid is not None:  # this party is client (peer is server)
+            rt = self.runtime
+            m = len(rt.parties)
+            t = rt.threshold
+            pid_keys = [rt.pid.to_bytes(2, 'little')]  # send pid
+            if not rt.options.no_prss:
                 for subset in itertools.combinations(range(m), m - t):
-                    if subset[0] == self.runtime.pid and self.peer_pid in subset:
-                        pid_keys.append(self.runtime._prss_keys[subset])  # send PRSS keys
+                    if subset[0] == rt.pid and self.peer_pid in subset:
+                        pid_keys.append(rt._prss_keys[subset])  # send PRSS keys
             transport.writelines(pid_keys)
             self._key_transport_done()
 
     def send(self, pc, payload):
         """Send payload labeled with pc to the peer.
 
         Message format consists of three parts:
-         1. pc (8 bytes signed int)
-         2. payload_size (4 bytes unsigned int)
+         1. payload_size (4 bytes unsigned int)
+         2. pc (8 bytes signed int)
          3. payload (byte string of length payload_size).
         """
         payload_size = len(payload)
-        fmt = f'<qI{payload_size}s'
-        self.transport.write(struct.pack(fmt, pc, payload_size, payload))
+        fmt = f'<Iq{payload_size}s'
+        self.transport.write(struct.pack(fmt, payload_size, pc, payload))
+        self.nbytes_sent += 12 + payload_size
 
     def data_received(self, data):
         """Called when data is received from the peer.
 
         Received bytes are unpacked as a program counter and the payload
         (actual data). The payload is passed to the appropriate Future, if any.
 
         First message from peer is processed differently if peer is a client.
         """
         self.bytes.extend(data)
-        if self.peer_pid is None:  # peer is client (party is server)
+        if self.peer_pid is None:  # peer is client (this party is server)
             if len(self.bytes) < 2:
                 return
 
             peer_pid = int.from_bytes(self.bytes[:2], 'little')
             len_packet = 2
-            if not self.runtime.options.no_prss:
-                m = len(self.runtime.parties)
-                t = self.runtime.threshold
+            rt = self.runtime
+            if not rt.options.no_prss:
+                m = len(rt.parties)
+                t = rt.threshold
                 for subset in itertools.combinations(range(m), m - t):
-                    if subset[0] == peer_pid and self.runtime.pid in subset:
+                    if subset[0] == peer_pid and rt.pid in subset:
                         len_packet += 16
                 if len(self.bytes) < len_packet:
                     return
 
             # record new protocol peer
             self.peer_pid = peer_pid
-            if not self.runtime.options.no_prss:
+            if not rt.options.no_prss:
                 # store keys received from peer
                 len_packet = 2
                 for subset in itertools.combinations(range(m), m - t):
-                    if subset[0] == peer_pid and self.runtime.pid in subset:
-                        self.runtime._prss_keys[subset] = self.bytes[len_packet:len_packet + 16]
+                    if subset[0] == peer_pid and rt.pid in subset:
+                        rt._prss_keys[subset] = self.bytes[len_packet:len_packet + 16]
                         len_packet += 16
             del self.bytes[:len_packet]
             self._key_transport_done()
 
         while self.bytes:
-            if len(self.bytes) < 12:
+            if len(self.bytes) < 4:
                 return
 
-            pc, payload_size = struct.unpack_from('<qI', self.bytes)
+            payload_size = struct.unpack_from('<I', self.bytes)[0]
             len_packet = payload_size + 12
             if len(self.bytes) < len_packet:
                 return
 
-            payload = struct.unpack_from(f'<{payload_size}s', self.bytes, 12)[0]
+            pc, payload = struct.unpack_from(f'<q{payload_size}s', self.bytes, 4)
             del self.bytes[:len_packet]
             if pc in self.buffers:
                 self.buffers.pop(pc).set_result(payload)
             else:
                 self.buffers[pc] = payload
 
     def receive(self, pc):
@@ -122,20 +137,23 @@
             payload = self.buffers[pc] = Future(loop=self.runtime._loop)
         return payload
 
     def connection_lost(self, exc):
         """Called when the connection with the peer is lost or closed.
 
         If the connection is closed normally (during shutdown) then exc is None.
-        Otherwise, if the connection is lost unexpectedly, exc may indicate the
-        cause (but exc is None is still possible).
+        Otherwise, if the connection is lost unexpectedly, exc may indicate the cause.
         """
         if exc:
             raise exc
-        # TODO: also raise an exception if exc is None and no shutdown in progress
+
+        rt = self.runtime
+        rt.parties[self.peer_pid].protocol = None
+        if all(p.protocol is None for p in rt.parties if p.pid != rt.pid):
+            rt.parties[rt.pid].protocol.set_result(None)
 
     def close_connection(self):
         """Close connection with the peer."""
         self.transport.close()
 
 
 class _AwaitableFuture:
@@ -222,42 +240,44 @@
         assert isinstance(obj, (list, tuple)), obj
         return _SharesCounter(rt._loop, obj)
 
     return _AwaitableFuture(_get_results(obj))
 
 
 def _hop(a):  # NB: redefined in MPyC setup if mix of 32-bit/64-bit platforms enabled
-    """Simple and efficient pseudorandom program counter hop for Python 3.6+.
+    """Simple and efficient pseudorandom program counter hop.
 
     Compatible between all 64-bit platforms.
     Compatible between all 32-bit platforms.
     Not compatible between mix of 32-bit and 64-bit platforms.
     """
-    return hash(frozenset(a))
+    return hash(tuple(a))
 
 
 class _ProgramCounterWrapper:
 
     __slots__ = 'runtime', 'coro', 'pc'
 
-    def __init__(self, runtime, coro):
-        self.runtime = runtime
+    def __init__(self, rt, coro):
+        self.runtime = rt
         self.coro = coro
-        runtime._program_counter[0] += 1
-        self.pc = [_hop(runtime._program_counter), runtime._program_counter[1]+1]  # fork
+        rt._program_counter[0] += 1
+        self.pc = [_hop(rt._program_counter), rt._program_counter[1]+1]  # fork
 
     def __await__(self):
         while True:
             pc = self.runtime._program_counter
             self.runtime._program_counter = self.pc
             try:
                 val = self.coro.send(None)
-                self.pc = self.runtime._program_counter
             except StopIteration as exc:
-                return exc.value  # NB: required for Python 3.7
+                return exc.value
+
+            else:
+                self.pc = self.runtime._program_counter
             finally:
                 self.runtime._program_counter = pc
             yield val
 
 
 async def _wrap_in_coro(awaitable):
     return await awaitable
@@ -280,33 +300,43 @@
         dims = dims[1:]
         s = [_nested_list(rt, n0, dims) for _ in range(n)]
     else:
         s = [rt() for _ in range(n)]
     return s
 
 
-runtime = None
-
-
 def returnType(*args, wrap=True):
     """Define return type for MPyC coroutines.
 
     Used in first await expression in an MPyC coroutine.
     """
     rettype, *dims = args
     if isinstance(rettype, type(None)):
         rettype = None
     if rettype is not None:
         if isinstance(rettype, tuple):
             stype = rettype[0]
-            integral = rettype[1]
-            if stype.frac_length:
-                rt = lambda: stype(None, integral)
+            integral = None
+            shape = None
+            if isinstance(rettype[1], tuple):
+                shape = rettype[1]
+            elif isinstance(rettype[1], bool) and stype.frac_length:
+                integral = rettype[1]
+            if rettype[2:]:
+                shape = rettype[2]
+            if integral is not None:
+                if shape is not None:
+                    rt = lambda: stype(None, shape, integral)
+                else:
+                    rt = lambda: stype(None, integral=integral)
             else:
-                rt = stype
+                if shape is not None:
+                    rt = lambda: stype(None, shape)
+                else:
+                    rt = stype
         elif issubclass(rettype, Future):
             rt = lambda: rettype(loop=runtime._loop)
         else:
             rt = rettype
         if dims:
             rettype = _nested_list(rt, dims[0], dims[1:])
         else:
@@ -415,13 +445,13 @@
             print('Traceback (enclosing MPyC coroutine call):')
             traceback.print_stack(task.f_back)  # TODO: extend call chain
             return
 
     elif 'task' in context:
         cb = context['task']._callbacks[0]
         if isinstance(cb, tuple):
-            cb = cb[0]  # NB: drop context paramater for Python 3.7+
+            cb = cb[0]  # NB: drop context parameter
         if 'mpc_coro' in cb.__qualname__:
             if not loop.get_debug():  # Unless asyncio debug mode is enabled,
                 return  # suppress 'Task was destroyed but it is pending!' message.
 
     loop.default_exception_handler(context)
```

### Comparing `mpyc-0.8/mpyc/fingroups.py` & `mpyc-0.9/mpyc/fingroups.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 Five types of groups are currently supported, aimed mainly at applications
 in cryptography:
 
     - symmetric groups of any degree n (n>=0)
     - quadratic residue groups modulo a safe prime
     - Schnorr groups (prime-order subgroups of the multiplicative group of a finite field)
-    - elliptic curve groups (Edwards curves and Barreto-Naehrig curves)
+    - elliptic curve groups (Edwards curves, a Koblitz curve, and Barreto-Naehrig curves)
     - class groups of imaginary quadratic fields
 
 The structure of most of these groups will be trivial, preferably cyclic or even
 of prime order. Where applicable, a generator of the group (or a sufficiently
 large subgroup) is provided to accommodate discrete log and Diffie-Hellman
 hardness assumptions.
 """
@@ -160,34 +160,34 @@
         """Make finite group elements hashable (e.g., for LRU caching)."""
         return hash((type(self).__name__, self.value))
 
     def __repr__(self):
         return repr(self.value)
 
     @classmethod
-    def operation(cls, a, b):  # TODO: ",/" for positional-only arguments in Python 3.8+ (pylintrc)
+    def operation(cls, a, b, /):
         """Return a @ b."""
         raise NotImplementedError
 
     @classmethod
-    def operation2(cls, a):
+    def operation2(cls, a, /):
         """Return a @ a."""
         return cls.operation(a, a)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         """Return @-inverse of a (written ~a)."""
         raise NotImplementedError
 
     def inverse(self):  # TODO: reconsider use of instance methods
         """For convenience."""
         return type(self).inversion(self)
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         """Return a == b."""
         raise NotImplementedError
 
     @staticmethod
     def repeat(a, n):
         """Return nth @-power of a (written a^n), for any integer n."""
         cls = type(a)
@@ -226,28 +226,28 @@
         if check:
             if len(value) != self.degree or set(value) != set(range(self.degree)):
                 raise ValueError(f'valid length-{self.degree} permutation required')
 
         self.value = value
 
     @classmethod
-    def operation(cls, p, q):
+    def operation(cls, p, q, /):
         """First p then q."""
         return cls(tuple(q.value[j] for j in p.value), check=False)
 
     @classmethod
-    def inversion(cls, p):
+    def inversion(cls, p, /):
         n = len(p.value)
         q = [None] * n
         for i in range(n):
             q[p.value[i]] = i
         return cls(tuple(q), check=False)
 
     @classmethod
-    def equality(cls, p, q):
+    def equality(cls, p, q, /):
         return p.value == q.value
 
 
 @functools.lru_cache(maxsize=None)
 def SymmetricGroup(n):
     """Create type for symmetric group of degree n, n>=0."""
     name = f'Sym({n})'
@@ -285,23 +285,23 @@
 
             if value == 0 or not value.is_sqr():
                 raise ValueError('quadratic residue required')
 
         self.value = value
 
     @classmethod
-    def operation(cls, a, b):
+    def operation(cls, a, b, /):
         return cls(a.value * b.value, check=False)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         return cls(1/a.value, check=False)
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         return a.value == b.value
 
     @classmethod
     def repeat(cls, a, n):
         return cls(a.value**n, check=False)
 
     def __int__(self):
@@ -429,23 +429,23 @@
 
             if value**self.order != 1:
                 raise ValueError('subgroup elt required')
 
         self.value = value
 
     @classmethod
-    def operation(cls, a, b):
+    def operation(cls, a, b, /):
         return cls(a.value * b.value, check=False)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         return cls(1/a.value, check=False)
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         return a.value == b.value
 
     @classmethod
     def repeat(cls, a, n):
         return cls(a.value**n, check=False)
 
     def __int__(self):
@@ -511,18 +511,15 @@
     assert n == q.bit_length()
 
     p = int(p)
     q = int(q)
     if g is None:
         w = (p-1) // q
         i = 2
-        while True:
-            g = powmod(i, w, p)
-            if g != 1 and powmod(g, q, p) == 1:
-                break
+        while (g := powmod(i, w, p)) == 1:
             i += 1
         g = int(g)
     return _SchnorrGroup(p, q, g)
 
 
 @functools.lru_cache(maxsize=None)
 def _SchnorrGroup(p, q, g):
@@ -648,20 +645,20 @@
 
     __slots__ = ()
 
     _identity = (0, 1)
     oblivious = True
 
     @classmethod
-    def inversion(cls, pt):
+    def inversion(cls, pt, /):
         x, y = pt
         return cls((-x, y), check=False)
 
     @classmethod
-    def operation(cls, pt1, pt2):
+    def operation(cls, pt1, pt2, /):
         """Add Edwards points using affine coordinates (projective with z=1)."""
         # see https://hyperelliptic.org/EFD/g1p/data/edwards/projective/addition/mmadd-2007-bl
         x1, y1 = pt1
         x2, y2 = pt2
         C = x1 * x2
         D = y1 * y2
         E = cls.d * C * D
@@ -672,33 +669,33 @@
         y3 = y3 * z3_inv
         return cls((x3, y3), check=False)
 
     def normalize(self):
         return self
 
     @classmethod
-    def equality(cls, pt1, pt2):
+    def equality(cls, pt1, pt2, /):
         return pt1.value == pt2.value
 
 
 class EdwardsProjective(EdwardsCurvePoint):
     """Edwards curves with projective coordinates."""
 
     __slots__ = ()
 
     _identity = (0, 1, 1)
     oblivious = True
 
     @classmethod
-    def inversion(cls, pt):
+    def inversion(cls, pt, /):
         x, y, z = pt
         return cls((-x, y, z), check=False)
 
     @classmethod
-    def operation(cls, pt1, pt2):
+    def operation(cls, pt1, pt2, /):
         """Add Edwards points with (homogeneous) projective coordinates."""
         # see https://www.hyperelliptic.org/EFD/g1p/data/twisted/projective/addition/add-2008-bbjlp
         x1, y1, z1 = pt1
         x2, y2, z2 = pt2
         A = z1 * z2
         B = A**2
         C = x1 * x2
@@ -715,35 +712,35 @@
         cls = type(self)
         x, y, z = self
         z_inv = 1 / z
         x, y = x * z_inv, y * z_inv
         return cls((x, y, cls.field(1)), check=False)
 
     @classmethod
-    def equality(cls, pt1, pt2):
+    def equality(cls, pt1, pt2, /):
         x1, y1, z1 = pt1
         x2, y2, z2 = pt2
         return x1 * z2 == x2 * z1 and y1 * z2 == y2 * z1
 
 
 class EdwardsExtended(EdwardsCurvePoint):
     """Edwards curves with extended coordinates."""
 
     __slots__ = ()
 
     _identity = (0, 1, 1, 0)
     oblivious = True
 
     @classmethod
-    def inversion(cls, pt):
+    def inversion(cls, pt, /):
         x, y, z, t = pt
         return cls((-x, y, z, -t), check=False)
 
     @classmethod
-    def operation(cls, pt1, pt2):
+    def operation(cls, pt1, pt2, /):
         """Add (twisted a=-1) Edwards points in extended projective coordinates."""
         # see https://eprint.iacr.org/2008/522 Hisil et al., Section 4.2 for 4 processors
         x1, y1, z1, t1 = pt1
         x2, y2, z2, t2 = pt2
         r1, r2, r3, r4 = y1 - x1, y2 - x2, y1 + x1, y2 + x2
         r1, r2, r3, r4 = r1 * r2, r3 * r4, 2*cls.d * t1 * t2, 2*z1 * z2
         r1, r2, r3, r4 = r2 - r1, r4 - r3, r4 + r3, r2 + r1
@@ -754,15 +751,15 @@
         cls = type(self)
         x, y, z, _ = self
         z_inv = 1 / z
         x, y = x * z_inv, y * z_inv
         return cls((x, y, cls.field(1), x * y), check=False)
 
     @classmethod
-    def equality(cls, pt1, pt2):
+    def equality(cls, pt1, pt2, /):
         x1, y1, z1, _ = pt1
         x2, y2, z2, _ = pt2
         return x1 * z2 == x2 * z1 and y1 * z2 == y2 * z1
 
 
 class WeierstrassCurvePoint(EllipticCurvePoint):
     """Common base class for (short) Weierstrass curves."""
@@ -779,15 +776,15 @@
 
     def __init__(self, value=None, check=True):
         field = self.field
         if value is None or len(value) == 0:
             value = list(map(field, self._identity))
         elif 2 == len(value) < len(self._identity):  # convert affine to target
             value = list(value) + [field(1)]  # z = 1
-        if check:
+        if check and value:
             value = list(value)
             for i in range(len(value)):
                 if not isinstance(value[i], field):
                     value[i] = field(value[i])
             x, y = value[:2]
             z = value[2] if value[2:] else field(1)
             if z != 0:
@@ -806,23 +803,23 @@
 
     __slots__ = ()
 
     _identity = ()
     oblivious = False
 
     @classmethod
-    def inversion(cls, pt):
+    def inversion(cls, pt, /):
         if pt == cls.identity:
             return pt
 
         x, y = pt
         return cls((x, -y), check=False)
 
     @classmethod
-    def operation(cls, pt1, pt2):
+    def operation(cls, pt1, pt2, /):
         """Add Weierstrass points with affine coordinates."""
         if pt1 == cls.identity:
             return pt2
 
         if pt2 == cls.identity:
             return pt1
 
@@ -836,15 +833,15 @@
 
         r = (y1 - y2) / (x1 - x2)
         x3 = r**2 - x1 - x2
         y3 = r * (x1 - x3) - y1
         return cls((x3, y3), check=False)
 
     @classmethod
-    def operation2(cls, pt):
+    def operation2(cls, pt, /):
         """Double Weierstrass point with affine coordinates."""
         if pt == cls.identity:
             return cls.identity
 
         x, y = pt
         if y == 0:
             return cls.identity
@@ -854,33 +851,33 @@
         y2 = r * (x - x2) - y
         return cls((x2, y2), check=False)
 
     def normalize(self):
         return self
 
     @classmethod
-    def equality(cls, pt1, pt2):
+    def equality(cls, pt1, pt2, /):
         return pt1.value == pt2.value
 
 
 class WeierstrassProjective(WeierstrassCurvePoint):
     """Short Weierstrass curves with projective coordinates."""
 
     __slots__ = ()
 
     _identity = (0, 1, 0)
     oblivious = True
 
     @classmethod
-    def inversion(cls, pt):
+    def inversion(cls, pt, /):
         x, y, z = pt
         return cls((x, -y, z), check=False)
 
     @classmethod
-    def operation(cls, pt1, pt2):
+    def operation(cls, pt1, pt2, /):
         """Add Weierstrass points with projective coordinates."""
         # see https://eprint.iacr.org/2015/1060  Renes et al., Algorithm 7
         x1, y1, z1 = pt1
         x2, y2, z2 = pt2
         assert cls.a == 0
         b3 = 3*cls.b
         t0, t1, t2 = x1 * x2, y1 * y2, z1 * z2
@@ -893,15 +890,15 @@
         t1 -= t2
         x3 = t3 * t1 - t4 * y3
         y3 = t0 * y3 + t1 * z3
         z3 = t4 * z3 + t0 * t3
         return cls((x3, y3, z3), check=False)
 
     @classmethod
-    def operation2(cls, pt):
+    def operation2(cls, pt, /):
         """Double Weierstrass point with projective coordinates."""
         # see https://eprint.iacr.org/2015/1060  Renes et al., Algorithm 9
         x, y, z = pt
         t0 = y**2
         z2 = 8*t0
         t2 = 3*cls.b * z**2
         x2 = t2 * z2
@@ -919,15 +916,15 @@
             return cls.identity
 
         z_inv = 1 / z
         x, y = x * z_inv, y * z_inv
         return cls((x, y, cls.field(1)), check=False)
 
     @classmethod
-    def equality(cls, pt1, pt2):
+    def equality(cls, pt1, pt2, /):
         x1, y1, z1 = pt1
         x2, y2, z2 = pt2
         if z1 == 0 and z2 == 0:
             return True
 
         return x1 * z2 == x2 * z1 and y1 * z2 == y2 * z1
 
@@ -937,20 +934,20 @@
 
     __slots__ = ()
 
     _identity = (0, 1, 0)
     oblivious = False
 
     @classmethod
-    def inversion(cls, pt):
+    def inversion(cls, pt, /):
         x, y, z = pt
         return cls((x, -y, z), check=False)
 
     @classmethod
-    def operation(cls, pt1, pt2):
+    def operation(cls, pt1, pt2, /):
         """Add Weierstrass points with Jacobian coordinates."""
         # see https://hyperelliptic.org/EFD/g1p/data/shortw/jacobian-0/addition/add-2007-bl
         if pt1[2] == 0:
             return pt2
 
         if pt2[2] == 0:
             return pt1
@@ -974,15 +971,15 @@
         v = u1 * i
         x3 = r**2 - j - 2*v
         y3 = r * (v - x3) - 2*s1 * j
         z3 = ((z1 + z2)**2 - z1z1 - z2z2) * h
         return cls((x3, y3, z3), check=False)
 
     @classmethod
-    def operation2(cls, pt):
+    def operation2(cls, pt, /):
         """Double Weierstrass point with Jacobian coordinates."""
         # see https://hyperelliptic.org/EFD/g1p/data/shortw/jacobian-0/doubling/dbl-2009-l
         x1, y1, z1 = pt
         a = x1**2
         b = y1**2
         c = b**2
         d = 2*((x1 + b)**2 - a - c)
@@ -1001,15 +998,15 @@
 
         z_inv = 1 / z
         z_inv2 = z_inv**2
         x, y = x * z_inv2, y * z_inv * z_inv2
         return cls((x, y, cls.field(1)), check=False)
 
     @classmethod
-    def equality(cls, pt1, pt2):
+    def equality(cls, pt1, pt2, /):
         x1, y1, z1 = pt1
         x2, y2, z2 = pt2
         if z1 == 0 and z2 == 0:
             return True
 
         z12, z22 = z1**2, z2**2
         return x1 * z22 == x2 * z12 and y1 * z2 * z22 == y2 * z1 * z12
@@ -1019,18 +1016,19 @@
     """Create elliptic curve type for a selection of built-in curves.
     The default coordinates used with these curves are 'affine'.
 
     The following Edwards curves and Weierstrass curves are built-in:
 
         - 'Ed25519': see https://en.wikipedia.org/wiki/EdDSA#Ed25519
         - 'Ed448': aka "Goldilocks", see https://en.wikipedia.org/wiki/Curve448
+        - 'secp256k1': Bitcoin's Koblitz curve from https://www.secg.org/sec2-v2.pdf
         - 'BN256': Barreto-Naehrig curve, https://eprint.iacr.org/2010/186
         - 'BN256_twist': sextic twist of Barreto-Naehrig curve
 
-    Both curves can be used with 'affine' (default) and 'projective' coordinates.
+    These curves can be used with 'affine' (default) and 'projective' coordinates.
     The Edwards curves can also be used with 'extended' coordinates, and the
     Weierstrass curves with 'jacobian' coordinates.
     """
     if coordinates is None:
         coordinates = 'affine'
     return _EllipticCurve(curvename, coordinates)
 
@@ -1111,14 +1109,37 @@
             EC.b = gf('3') / xi
             x = gf([64746500191241794695844075326670126197795977525365406531717464316923369116492,
                     21167961636542580255011770066570541300993051739349375019639421053990175267184])
             y = gf([17778617556404439934652658462602675281523610326338642107814333856843981424549,
                     20666913350058776956210519119118544732556678129809273996262322366050359951122])
             base_pt = (x, y)
         EC.order = p - 6*u**2
+    elif curvename == 'secp256k1':
+        p = 2**256 - 2**32 - 2**9 - 2**8 - 2**7 - 2**6 - 2**4 - 1  # p = 3 (mod 4)
+        gf = GF(p)
+
+        name = f'E({gf.__name__}){curvename}{coordinates}'
+        if coordinates == 'jacobian':
+            base = WeierstrassJacobian
+        elif coordinates == 'affine':
+            base = WeierstrassAffine
+        elif coordinates == 'projective':
+            base = WeierstrassProjective
+        else:
+            raise ValueError('invalid coordinates')
+
+        EC = type(name, (base,), {'__slots__': ()})
+        EC.field = gf
+
+        EC.a = gf(0)
+        EC.b = gf(7)
+        x = gf(int('79BE667EF9DCBBAC55A06295CE870B07029BFCDB2DCE28D959F2815B16F81798', 16))
+        y = gf(int('483ADA7726A3C4655DA4FBFC0E1108A8FD17B448A68554199C47D08FFB10D4B8', 16))
+        base_pt = (x, y)
+        EC.order = int('FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEBAAEDCE6AF48A03BBFD25E8CD0364141', 16)
     else:
         raise ValueError('curve not supported')
 
     assert is_prime(EC.order)
     EC.curvename = curvename
     EC.field.is_signed = False  # for consistency between sectypes and regular types
     EC.is_cyclic = True  # these EC groups are cyclic (but not all EC groups are)
@@ -1185,15 +1206,15 @@
         while not (-a < b <= a <= c and (a != c or b >= 0)):  # check reduced
             # reduce
             s = (c + b) // (2*c)
             a, b, c = c, -b + 2*s*c, c*s**2 - b*s + a
         return a, b, c
 
     @classmethod
-    def operation(cls, f1, f2):  # Cohen: Algorithm 5.4.9 (NUCOMP)
+    def operation(cls, f1, f2, /):  # Cohen: Algorithm 5.4.9 (NUCOMP)
         if f1[0] < f2[0]:
             f1, f2 = f2, f1
         a1, b1, c1 = f1
         a2, b2, c2 = f2
         s = (b1 + b2) // 2
         n = b2 - s
 
@@ -1251,15 +1272,15 @@
             a3 = d * b + d1 * e * v
             b3 = Q1 + Q2 + d1 * (Q3 + Q4)
             c3 = v3 * f + d1 * g * v2
         f3 = int(a3), int(b3), int(c3)  # NB: convert from gmpy2.mpz, if gmpy2 is used for gcdext()
         return cls(cls._reduce(f3), check=False)
 
     @classmethod
-    def operation2(cls, f):  # Cohen: Algorithm 5.4.8 (NUDUPL)
+    def operation2(cls, f, /):  # Cohen: Algorithm 5.4.8 (NUDUPL)
         a, b, c = f
         d1, u, _ = gcdext(b, a)
         assert d1 == 1  # because -discriminant is prime
         A = a // d1
         B = b // d1
         C = (-c * u) % A
         C1 = A - C
@@ -1289,21 +1310,21 @@
             a2 = d**2 + d1 * e * v
             b2 = d1 * (h + v * g) + 2*d * v3
             c2 = v3**2 + d1 * g * v2
         f2 = int(a2), int(b2), int(c2)  # NB: convert from gmpy2.mpz, if gmpy2 is used for gcdext()
         return cls(cls._reduce(f2), check=False)
 
     @classmethod
-    def inversion(cls, f):
+    def inversion(cls, f, /):
         a, b, c = f
         return cls(cls._reduce((a, -b, c)), check=False)
 
     @classmethod
-    def equality(cls, a, b):
-        return a.value == b.value
+    def equality(cls, f1, f2, /):
+        return f1.value == f2.value
 
     @classmethod
     def encode(cls, m):
         """Encode message m in the first coefficient of a form."""
         D = cls.discriminant
         gap = cls.gap
         assert (m+1) * gap <= isqrt(-D)/2  # ensure M (and Z) will be reduced
```

### Comparing `mpyc-0.8/mpyc/gfpx.py` & `mpyc-0.9/mpyc/gfpx.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,18 +44,19 @@
     Invariant: last element of attribute 'value' is a nonzero integer (if 'value' nonempty).
     """
 
     __slots__ = 'value'
 
     p = None
 
-    def __init__(self, value=0):
+    def __init__(self, value=0, check=True):
         """Initialize polynomial to given value (zero polynomial, by default)."""
-        cls = type(self)
-        self.value = cls._intern(value)
+        if check:
+            value = self._intern(value)
+        self.value = value
 
     @classmethod
     def _intern(cls, a):
         # convert a to cls internal format, if possible
         a = cls._coerce(a)
         if a is NotImplemented:
             raise TypeError(f'polynomial over GF({cls.p}) expected')
@@ -84,16 +85,15 @@
                 raise ValueError('polynomial coefficients invalid or out of range')
 
             return cls._from_list(a)
 
         return NotImplemented
 
     def __int__(self):
-        cls = type(self)
-        return cls._to_int(self.value)
+        return self._to_int(self.value)
 
     def __call__(self, x):
         """Evaluate polynomial at given x."""
         p = type(self).p
         x = x % p
         y = 0
         for c in reversed(self.value):
@@ -101,16 +101,15 @@
             y += c
             y %= p
         return y
 
     def to_bytes(self, length, byteorder):
         """Return a bytes object representing a polynomial."""
         # TODO: consider coefficient-wise serialization (via numpy arrays)
-        cls = type(self)
-        return cls._to_int(self.value).to_bytes(length, byteorder)
+        return self._to_int(self.value).to_bytes(length, byteorder)
 
     @classmethod
     def _from_int(cls, a):
         p = cls.p
         neg = a < 0
         if neg:
             a = -a
@@ -299,15 +298,15 @@
                 while r and not r[-1]:
                     r.pop()
         return q, r
 
     @classmethod
     def _powmod(cls, a, n, modulus=None):
         if n == 0:
-            return 1
+            return cls._intern(1)
 
         if n < 0:
             if modulus is None:
                 raise ValueError('negative exponent')
 
             a = cls._invert(a, modulus)
             n = -n
@@ -406,20 +405,20 @@
             _a = cls._from_int(a)
             if _a[-1] != 1:  # ensure monic a
                 a = p**len(_a)
                 continue
             if cls._is_irreducible(_a):
                 break
 
-        return a
+        return _a
 
     @classmethod
     def from_terms(cls, s, x=X):
         """Convert string s with sum of powers of x to a polynomial."""
-        return cls(cls._from_terms(s, x))
+        return cls(cls._from_terms(s, x), check=False)
 
     @classmethod
     def to_terms(cls, a, x=X):
         """Convert polynomial a to a string with sum of powers of x."""
         a = cls._intern(a)
         return cls._to_terms(a, x)
 
@@ -427,283 +426,275 @@
     def deg(cls, a):
         """Degree of polynomial a (-1 if a is zero polynomial)."""
         a = cls._intern(a)
         return cls._deg(a)
 
     def degree(self):
         """Degree of polynomial (-1 for zero polynomial)."""
-        cls = type(self)
-        return cls._deg(self.value)
+        return self._deg(self.value)
 
     def __neg__(self):
         cls = type(self)
-        return cls(cls._neg(self.value))
+        return cls(cls._neg(self.value), check=False)
 
     def __pos__(self):
         cls = type(self)
-        return cls(cls._pos(self.value))
+        return cls(cls._pos(self.value), check=False)
 
     @classmethod
     def add(cls, a, b):
         """Add polynomials a and b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._add(a, b))
+        return cls(cls._add(a, b), check=False)
 
     def __add__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._add(self.value, other))
+        return cls(cls._add(self.value, other), check=False)
 
     __radd__ = __add__
 
     @classmethod
     def sub(cls, a, b):
         """Subtract polynomials a and b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._sub(a, b))
+        return cls(cls._sub(a, b), check=False)
 
     def __sub__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._sub(self.value, other))
+        return cls(cls._sub(self.value, other), check=False)
 
     def __rsub__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._sub(other, self.value))
+        return cls(cls._sub(other, self.value), check=False)
 
     @classmethod
     def mul(cls, a, b):
         """Multiply polynomials a and b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._mul(a, b))
+        return cls(cls._mul(a, b), check=False)
 
     def __mul__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._mul(self.value, other))
+        return cls(cls._mul(self.value, other), check=False)
 
     __rmul__ = __mul__
 
     @classmethod
     def lshift(cls, a, n):
         """Multiply polynomial a by X^n."""
         a = cls._intern(a)
-        return cls(cls._lshift(a, n))
+        return cls(cls._lshift(a, n), check=False)
 
     def __lshift__(self, other):
         if not isinstance(other, int):
             return NotImplemented
 
         cls = type(self)
-        return cls(cls._lshift(self.value, other))
+        return cls(cls._lshift(self.value, other), check=False)
 
     def __rlshift__(self, other):
         return NotImplemented
 
     @classmethod
     def rshift(cls, a, n):
         """Quotient for polynomial a divided by X^n, assuming a is multiple of X^n."""
         a = cls._intern(a)
-        return cls(cls._rshift(a, n))
+        return cls(cls._rshift(a, n), check=False)
 
     def __rshift__(self, other):
         if not isinstance(other, int):
             return NotImplemented
 
         cls = type(self)
-        return cls(cls._rshift(self.value, other))
+        return cls(cls._rshift(self.value, other), check=False)
 
     def __rrshift__(self, other):
         return NotImplemented
 
     def __floordiv__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._divmod(self.value, other)[0])
+        return cls(cls._divmod(self.value, other)[0], check=False)
 
     def __rfloordiv__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._divmod(other, self.value)[0])
+        return cls(cls._divmod(other, self.value)[0], check=False)
 
     @classmethod
     def mod(cls, a, b):
         """Reduce polynomial a modulo polynomial b, for nonzero b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._mod(a, b))
+        return cls(cls._mod(a, b), check=False)
 
     def __mod__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._mod(self.value, other))
+        return cls(cls._mod(self.value, other), check=False)
 
     def __rmod__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls(cls._mod(other, self.value))
+        return cls(cls._mod(other, self.value), check=False)
 
     @classmethod
     def divmod(cls, a, b):
         """Divide polynomial a by polynomial b with remainder, for nonzero b."""
         a = cls._intern(a)
         b = cls._intern(b)
         q, r = cls._divmod(a, b)
-        return cls(q), cls(r)
+        return cls(q, check=False), cls(r, check=False)
 
     def __divmod__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
         q, r = cls._divmod(self.value, other)
-        return cls(q), cls(r)
+        return cls(q, check=False), cls(r, check=False)
 
     def __rdivmod__(self, other):
         cls = type(self)
         other = cls._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
         q, r = cls._divmod(other, self.value)
-        return cls(q), cls(r)
+        return cls(q, check=False), cls(r, check=False)
 
     @classmethod
     def powmod(cls, a, n, b):
         """Polynomial a to the power of n modulo polynomial b, for nonzero b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._powmod(a, n, modulus=b))
+        return cls(cls._powmod(a, n, modulus=b), check=False)
 
     def __pow__(self, other):
         cls = type(self)
-        return cls(cls._powmod(self.value, other))
+        return cls(cls._powmod(self.value, other), check=False)
 
     @classmethod
     def gcd(cls, a, b):
         """Greatest common divisor of polynomials a and b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._gcd(a, b))
+        return cls(cls._gcd(a, b), check=False)
 
     @classmethod
     def gcdext(cls, a, b):
         """Extended GCD for polynomials a and b.
 
         Return d, s, t satisfying s a + t b = d = gcd(a,b).
         """
         a = cls._intern(a)
         b = cls._intern(b)
         d, s, t = cls._gcdext(a, b)
-        return cls(d), cls(s), cls(t)
+        return cls(d, check=False), cls(s, check=False), cls(t, check=False)
 
     @classmethod
     def invert(cls, a, b):
         """Inverse of polynomial a modulo polynomial b, for nonzero b."""
         a = cls._intern(a)
         b = cls._intern(b)
-        return cls(cls._invert(a, b))
+        return cls(cls._invert(a, b), check=False)
 
     @classmethod
     def is_irreducible(cls, a):
         """Test polynomial a for irreducibility."""
         a = cls._intern(a)
         return cls._is_irreducible(a)
 
     @classmethod
     def next_irreducible(cls, a):
         """Return lexicographically next monic irreducible polynomial > a.
 
         E.g., X < X+1 < X^2+X+1 < X^3+X+1 < X^3+X^2+1 < ... for p=2.
         """
         a = cls._intern(a)
-        return cls(cls._next_irreducible(a))
+        return cls(cls._next_irreducible(a), check=False)
 
     def __repr__(self):
-        cls = type(self)
-        return cls._to_terms(self.value)
+        return self._to_terms(self.value)
 
     def __lt__(self, other):
         """Strictly less-than comparison."""
-        cls = type(self)
-        other = cls._coerce(other)
+        other = self._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls._to_int(self.value) <= cls._to_int(other)
+        return self._to_int(self.value) <= self._to_int(other)
 
     def __le__(self, other):
         """Less-than or equal comparison."""
-        cls = type(self)
-        other = cls._coerce(other)
+        other = self._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls._to_int(self.value) < cls._to_int(other)
+        return self._to_int(self.value) < self._to_int(other)
 
     def __eq__(self, other):
         """Equality test."""
-        cls = type(self)
-        other = cls._coerce(other)
+        other = self._coerce(other)
         if other is NotImplemented:
             return False
 
         return self.value == other
 
     def __ge__(self, other):
         """Greater-than or equal comparison."""
-        cls = type(self)
-        other = cls._coerce(other)
+        other = self._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls._to_int(self.value) >= cls._to_int(other)
+        return self._to_int(self.value) >= self._to_int(other)
 
     def __gt__(self, other):
         """Strictly greater-than comparison."""
-        cls = type(self)
-        other = cls._coerce(other)
+        other = self._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
-        return cls._to_int(self.value) > cls._to_int(other)
+        return self._to_int(self.value) > self._to_int(other)
 
     def __ne__(self, other):
         """Negated equality test."""
-        cls = type(self)
-        other = cls._coerce(other)
+        other = self._coerce(other)
         if other is NotImplemented:
             return True
 
         return self.value != other
 
     def __hash__(self):
         """Make polynomials hashable (e.g., for LRU caching)."""
@@ -842,44 +833,46 @@
     def _mod(a, b):
         if b is None:  # see _powmod()
             return a
 
         if b == 0:
             raise ZeroDivisionError('division by zero polynomial')
 
-        m = BinaryPolynomial._deg(a)
-        n = BinaryPolynomial._deg(b)
+        m = a.bit_length()
+        n = b.bit_length()
         if m < n:
             return a
 
         b <<= m - n
-        for i in range(m - n + 1):
-            if (a >> m - i) & 1:
-                a ^= b
+        a ^= b
+        for i in range(m-2, n-2, -1):
             b >>= 1
+            if (a >> i) & 1:
+                a ^= b
         return a
 
     @staticmethod
     def _divmod(a, b):
         if b == 0:
             raise ZeroDivisionError('division by zero polynomial')
 
-        m = BinaryPolynomial._deg(a)
-        n = BinaryPolynomial._deg(b)
+        m = a.bit_length()
+        n = b.bit_length()
         if m < n:
             return 0, a
 
         b <<= m - n
-        q = 0
-        for i in range(m - n + 1):
+        q = 1
+        a ^= b
+        for i in range(m-2, n-2, -1):
+            b >>= 1
             q <<= 1
-            if (a >> m - i) & 1:
-                a ^= b
+            if (a >> i) & 1:
                 q ^= 1
-            b >>= 1
+                a ^= b
         return q, a
 
     @staticmethod
     def _gcd(a, b):
         while b:
             a, b = b, BinaryPolynomial._mod(a, b)
         return a
```

### Comparing `mpyc-0.8/mpyc/gmpy.py` & `mpyc-0.9/mpyc/gmpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module collects all gmpy2 functions used by MPyC.
 
 Stubs only using Python built-ins are provided in case the gmpy2 package is not available.
-A function for factoring prime powers and a function for rational reconstruction are also provided.
+Efficient functions for factoring prime powers and rational reconstruction are also provided.
 """
 
 import os
+import logging
 import math
 
 
 def factor_prime_power(x):  # TODO: move this to a separate math/number theory module?
     """Return p and d for a prime power x = p**d."""
     if x <= 1:
         raise ValueError('number not a prime power')
@@ -78,20 +79,26 @@
     raise ValueError('rational reconstruction not possible')
 
 
 try:
     if os.getenv('MPYC_NOGMPY') == '1':
         raise ImportError  # stubs will be loaded
 
-    from gmpy2 import (is_prime, next_prime, powmod, gcdext, invert,
+    from gmpy2 import (version, mpz, is_prime, next_prime, powmod, gcdext, invert,
                        legendre, jacobi, kronecker, is_square, isqrt, iroot)
+    logging.debug(f'Load gmpy2 version {version()}')
 except ImportError:
     # load stubs, if MPYC_NOGMPY is set, or if gmpy2 import fails
+    logging.debug('Load pure Python stubs for gmpy2')
     import random
 
+    def mpz(x):
+        """Return Python int(x) as stub for gmpy2's mpz(x)."""
+        return int(x)
+
     def is_prime(x, n=25):
         """Return True if x is probably prime, else False if x is
         definitely composite, performing up to n Miller-Rabin
         primality tests.
         """
         if x <= 2 or x%2 == 0:
             return x == 2
@@ -231,24 +238,15 @@
             return False
 
         y = isqrt(x)
         return x == y**2
 
     def isqrt(x):
         """Return integer square root of nonnegative x."""
-        if x == 0:
-            return x
-
-        k = (x.bit_length() - 1) // 2
-        y = 1<<k
-        for i in range(k-1, -1, -1):
-            z = y | 1<<i
-            if z**2 <= x:
-                y = z
-        return y
+        return math.isqrt(x)
 
     def iroot(x, n):
         """Return (y, b) where y is the integer nth root of x and b is True if y is exact."""
         if x == 0:
             return x, True
 
         k = (x.bit_length() - 1) // n
```

### Comparing `mpyc-0.8/mpyc/mpctools.py` & `mpyc-0.9/mpyc/mpctools.py`

 * *Files identical despite different names*

### Comparing `mpyc-0.8/mpyc/random.py` & `mpyc-0.9/mpyc/random.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,19 +53,21 @@
     Special case: if sectype is a secure finite field and
     n is equal to the order of the finite field, then the
     uniformly random output can be generated directly.
     In this case, a number is returned always.
     """
     if issubclass(sectype, sectypes.SecureFiniteField) and n == sectype.field.order:
         assert not bits, 'bits not available'
-        await runtime.returnType((sectype, True))
         return runtime._random(sectype)
 
     b = n-1
     k = b.bit_length()
+    if not n & b:  # fast path for integral powers of 2
+        return getrandbits(sectype, k, bits=bits)
+
     if bits:
         await runtime.returnType((sectype, True), k)
     else:
         await runtime.returnType((sectype, True))
     x = runtime.random_bits(sectype, k)
     h = 1
     i = k
@@ -188,25 +190,43 @@
     return z
 
 
 def shuffle(sectype, x):
     """Shuffle list x secretly in-place, and return None.
 
     Given list x may contain public or secret elements.
+    Elements of x are all numbers or all lists (of the same length) of numbers.
     """
     n = len(x)
-    if not isinstance(x[0], sectype):  # assume same type for all elts of x
-        for i in range(len(x)):
-            x[i] = sectype(x[i])
+    # assume same type for all elts of x
+    x_i_is_list = isinstance(x[0], list)
+    if not x_i_is_list:
+        # elements of x are numbers
+        if not isinstance(x[0], sectype):
+            for i in range(n):
+                x[i] = sectype(x[i])
+        for i in range(n-1):
+            u = random_unit_vector(sectype, n - i)
+            x_u = runtime.in_prod(x[i:], u)
+            d = runtime.scalar_mul(x[i] - x_u, u)
+            x[i] = x_u
+            x[i:] = runtime.vector_add(x[i:], d)
+        return
+
+    # elements of x are lists of numbers
+    for j in range(len(x[0])):
+        if not isinstance(x[0][j], sectype):
+            for i in range(n):
+                x[i][j] = sectype(x[i][j])
     for i in range(n-1):
         u = random_unit_vector(sectype, n - i)
-        x_u = runtime.in_prod(x[i:], u)
-        d = runtime.scalar_mul(x[i] - x_u, u)
+        x_u = runtime.matrix_prod([u], x[i:])[0]
+        d = runtime.matrix_prod([[a] for a in u], [runtime.vector_sub(x[i], x_u)])
         x[i] = x_u
-        x[i:] = runtime.vector_add(x[i:], d)
+        x[i:] = runtime.matrix_add(x[i:], d)
 
 
 def random_permutation(sectype, x):
     """Uniformly random permutation of given sequence x or range(x)."""
     if isinstance(x, int):
         x = range(x)
     x = list(x)
```

### Comparing `mpyc-0.8/mpyc/secgroups.py` & `mpyc-0.9/mpyc/secgroups.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """This module provides secure (secret-shared) types of finite groups in MPyC.
 
 Secure versions of all groups supported by the module mpyc.fingroups are available:
 symmetric groups, quadratic residues, elliptic curve groups, and class groups.
 """
 
-import operator
 import itertools
 import functools
 import inspect
 import asyncio
 from mpyc.finfields import FiniteFieldElement
 import mpyc.fingroups as fg
 from mpyc.thresha import _recombination_vector
@@ -144,30 +143,30 @@
 
         return secgrp.equality(self, other)
 
     def __ne__(self, other):
         return 1 - self.__eq__(other)
 
     @classmethod
-    def operation(cls, a, b):
+    def operation(cls, a, b, /):
         """Return a @ b."""
         raise NotImplementedError
 
     @classmethod
-    def operation2(cls, a):
+    def operation2(cls, a, /):
         """Return a @ a."""
         return cls.operation(a, a)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         """Return @-inverse of a (written ~a)."""
         raise NotImplementedError
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         """Return a == b."""
         raise NotImplementedError
 
     def inverse(self):
         """For ease of use."""  # instance method a.inverse()
         return type(self).inversion(self)
 
@@ -268,36 +267,46 @@
     return c
 
 
 @asyncoro.mpc_coro
 async def repeat_public_base_secret_output(a, x, secgrp):
     """Compute a^[x]->[a^x]."""
     # a in prime order group, x in Z.
-    # x is a (secure) prime field element or (secure) int.
+    # x is a secure prime field element or secure int.
     await runtime.returnType(secgrp)
+    field = x.field
     m = len(runtime.parties)
-    lambda_i = _recombination_vector(x.field, range(1, m+1), 0)[runtime.pid]
+    lambda_i = _recombination_vector(field, range(1, m+1), 0)[runtime.pid]
     x_i = await runtime.gather(x)
-    c_i = secgrp.group.repeat(a, int(lambda_i * x_i))
+    e_i = int(lambda_i * x_i)
+    if isinstance(x, SecureFiniteField) and x.subfield is not None:
+        # value of x in prime field
+        e_i %= field.characteristic
+    c_i = secgrp.group.repeat(a, e_i)
     c = runtime.input(secgrp(c_i))
     return mpyc.mpctools.reduce(secgrp.operation, c)
 
 
 @asyncoro.mpc_coro
 async def repeat_public_base_public_output(a, x) -> asyncio.Future:
     """Multi-exponentiation for given base(s) a and exponent(s) x."""
     # a is a group element, or a list of group elements.
     # x is secure number (prime field element, or integer), or a list of secure numbers.
     if not isinstance(a, list):
         a, x = [a], [x]
+    field = x[0].field
     group = type(a[0])
     m = len(runtime.parties)
-    lambda_i = _recombination_vector(x[0].field, range(1, m+1), 0)[runtime.pid]
+    lambda_i = _recombination_vector(field, range(1, m+1), 0)[runtime.pid]
     x_i = await runtime.gather(x)
     e_i = [int(lambda_i * s_i) for s_i in x_i]
+    if isinstance(x, SecureFiniteField) and x.subfield is not None:
+        # values in x in prime field
+        for j in range(len(x)):
+            e_i[j] %= field.characteristic
     c_i = functools.reduce(group.operation, map(group.repeat, a, e_i))
     c = await runtime.transfer(c_i)
     return functools.reduce(group.operation, c)
 
 
 class SecureSymmetricGroupElement(SecureFiniteGroup):
     """Common base class for secure (secret-shared) symmetric group elements."""
@@ -323,29 +332,29 @@
         super().__init__(value)
 
     def set_share(self, value):
         for a, b in zip(self.share, value):
             a.set_share(b.share)
 
     @classmethod
-    def operation(cls, p, q):
+    def operation(cls, p, q, /):
         """First p then q."""
         q = seclist(q.share)
         return cls(tuple(q[j] for j in p.share))
 
     @classmethod
-    def inversion(cls, p):
+    def inversion(cls, p, /):
         n = len(p.share)
         q = seclist(p.share)  # use p.share as dummy of the right type
         for i in range(n):
             q[p.share[i]] = i
         return cls(tuple(q))
 
     @classmethod
-    def equality(cls, p, q):  # return type is self.sectype
+    def equality(cls, p, q, /):  # return type is self.sectype
         return seclist(p.share) == seclist(q.share)
 
 
 class SecureQuadraticResidue(SecureFiniteGroup):
     """Common base class for secure (secret-shared) quadratic residues."""
 
     __slots__ = ()
@@ -359,23 +368,23 @@
             value = secfld(value)
         super().__init__(value)
 
     def set_share(self, value):
         self.share.set_share(value.share)
 
     @classmethod
-    def operation(cls, a, b):
+    def operation(cls, a, b, /):
         return cls(a.share * b.share)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         return cls(1/a.share)
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         return a.share == b.share
 
     @classmethod
     def decode(cls, M, Z, gap=128):
         return (M.share - Z.share) / gap
 
 
@@ -393,23 +402,23 @@
             value = secfld(value)
         super().__init__(value)
 
     def set_share(self, value):
         self.share.set_share(value.share)
 
     @classmethod
-    def operation(cls, a, b):
+    def operation(cls, a, b, /):
         return cls(a.share * b.share)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         return cls(1/a.share)
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         return a.share == b.share
 
     @classmethod
     def decode(cls, M, Z):
         g = cls.group.generator
         h = cls.group.identity
         x = [h]
@@ -447,21 +456,21 @@
         for a, b in zip(self.share, value):
             a.set_share(b.share)
 
     def __getitem__(self, key):  # NB:  no set_item to prevent mutability
         return self.share[key]
 
     @classmethod
-    def operation(cls, a, b):
+    def operation(cls, a, b, /):
         group = cls.group
         c = group.operation(group(a.share, check=False), group(b.share, check=False))
         return cls(c)
 
     @classmethod
-    def inversion(cls, a):
+    def inversion(cls, a, /):
         group = cls.group
         c = group.inversion(group(a.share, check=False))
         return cls(c)
 
     def normalize(self):
         cls = type(self)
         group = cls.group
@@ -474,15 +483,15 @@
             c = runtime.scalar_mul(z_inv, c)
             return cls(c + [1 - zis0])
 
         c = group(self.share, check=False).normalize()
         return cls(c)
 
     @classmethod
-    def equality(cls, a, b):
+    def equality(cls, a, b, /):
         return runtime.all(u == v for u, v in zip(a.normalize(), b.normalize()))
 
     @classmethod
     def decode(cls, M, Z, gap=256):
         return (M.normalize()[0] - Z.normalize()[0]) / gap
 
 
@@ -618,51 +627,49 @@
         a, b, c = (a > c).if_else([c, -b, a], [a, b, c])
         b = ((b < 0) * (a == c)).if_else(-b, b)
         b = (b == -a).if_else(-b, b)
         return a, b, c
 
     # See Henri Cohen's book "A Course in Computational Algebraic Number Theory", Chapter 5.
     @classmethod
-    def operation(cls, f1, f2):  # Cohen: Algorithm 5.4.7 (Shanks 1969)
+    def operation(cls, f1, f2, /):  # Cohen: Algorithm 5.4.7 (Shanks 1969)
         a1, b1, c1 = f1
         a2, b2, c2 = f2
         s = (b1 + b2)/2
-        a1, a2, b2, c2 = runtime.if_else(a1 > a2, [a2, a1, b1, c1], [a1, a2, b2, c2])
         _d, _, y1 = runtime.gcdext(a1, a2, l=type(a1).bit_length//2)
         d, x2, y2 = runtime.gcdext(s, _d, l=type(a1).bit_length//2)
         v1 = a1 / d
         v2 = a2 / d
-#        _, r = _divmod(y1*y2*(s - b2) - x2*c2, v1)
-        _, r = _divmod(y1*y2, v1)
-        _, r = _divmod(r*(s - b2) - x2*c2, v1)
+        # Set r = y1 y2 (s - b2) - x2 c2 (mod v1) in two steps:
+        r = _divmod(_divmod(y1*y2, v1)[1] * (s - b2) - x2 * c2, v1)[1]
         a3 = v1*v2
         b3 = b2 + 2*v2*r
         c3 = (b3**2 - cls.group.discriminant) / (4*a3)
         return cls(cls._reduce((a3, b3, c3)))
 
     @classmethod
-    def operation2(cls, f):
+    def operation2(cls, f, /):
         a, b, c = f  # NB: a>0, b!=0, and gcd(a,b)=1 because -discriminant is prime
         x2 = runtime.inverse(b, a, l=type(a).bit_length//2)
         _, r = _divmod(x2*c, a)
         a2 = a**2
         b2 = b - 2*a*r
         c2 = (b2**2 - cls.group.discriminant) / (4*a2)
         return cls(cls._reduce((a2, b2, c2)))
 
     @classmethod
-    def inversion(cls, f):
+    def inversion(cls, f, /):
         a, b, c = f
         b = ((b != a) * (a != c)).if_else(-b, b)
         return cls((a, b, c))
 
     @classmethod
-    def equality(cls, a, b):
-        v0 = a.share[0] == b.share[0]
-        v1 = a.share[1] == b.share[1]
+    def equality(cls, f1, f2, /):
+        v0 = f1.share[0] == f2.share[0]
+        v1 = f1.share[1] == f2.share[1]
         return v0 * v1  # TODO: optimize batch test eq. with random r in field
 
     @classmethod
     def decode(cls, M, Z):
         gap = cls.group.gap
         return (M.share[0] - Z.share[0]) / gap
```

### Comparing `mpyc-0.8/mpyc/seclists.py` & `mpyc-0.9/mpyc/seclists.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,425 +1,423 @@
-"""This module provides a secure (oblivious) alternative to Python lists.
-
-A secure list contains secret-shared numbers. Apart from hiding the contents of the
-list, however, it is also possible to hide which items are accessed and which items
-are updated. In principle, only the length of a secure list remains public.
-
-A secure list x can be cast to an ordinary list by using list(x), without affecting
-the contents of the list. Also, public access to a secure list proceeds the same as
-for ordinary Python lists, using an index or a slice.
-
-For secure (oblivious) access to a secure list, however, one uses a secret-shared
-index i, which is either a secure number or a secure unit vector. Index i must be
-compatible with the secure list x: the type of i must fit with the type of the
-elements of x and the value of i must fit with the length of list x, that is,
-0 <= i < len(x).
-
-Common usage scenarios of secure lists are supported through methods such as sort(),
-count(), and index(), or can be coded easily. For example, the frequency of values
-in a list x of secure integers (whose values are known to be between 0 and n-1)
-is computed by:
-
-    s = seclist([0]*n, secint)
-
-    for a in x: s[a] += 1
-
-Current implementation is basic, taking advantage of cheap secure dot products, as
-provided by runtime.in_prod(). Performance for modestly sized lists of lengths 10 to 1000
-should be adequate. Later: With better amortized complexity, e.g., square root ORAM.
-"""
-
-from asyncio import Future
-from mpyc.sectypes import SecureObject, SecureFixedPoint
-from mpyc.random import random_unit_vector
-from mpyc import asyncoro
-
-runtime = None
-
-
-class seclist(list):
-
-    sectype = None
-
-    def __init__(self, x=(), sectype=None):
-        """Build a secure list from the items in iterable x using the given secure type.
-
-        If no secure type is given, it is inferred from the items in x.
-
-        Invariant: all items in a secure list are of the same secure type.
-        """
-        parent = super()
-        parent.__init__(x)
-        t = len(self)
-        for a in self:
-            if isinstance(a, SecureObject):
-                t -= 1
-                if sectype is None:
-                    sectype = type(a)
-                elif sectype != type(a):
-                    raise TypeError('inconsistent sectypes')
-
-        if sectype is None:
-            raise ValueError('sectype missing')
-
-        i = 0
-        while t:
-            a = parent.__getitem__(i)
-            while isinstance(a, SecureObject):
-                i += 1
-                a = parent.__getitem__(i)
-            parent.__setitem__(i, sectype(a))
-            t -= 1
-        self.sectype = sectype
-
-    def __getitem__(self, key):
-        """Called to evaluate self[key], where key is either public or secret.
-
-        If key is a public integer (or a slice), the behavior is the same as for ordinary lists.
-        If key is a secure number or index, the value at the secret position is returned.
-        """
-        if isinstance(key, (int, slice)):
-            value = super().__getitem__(key)
-            if isinstance(key, slice):
-                value = seclist(value, self.sectype)
-            return value
-
-        if isinstance(key, self.sectype):
-            i = runtime.unit_vector(key, len(self))
-        elif isinstance(key, secindex):
-            i = [self.sectype(0)] * key.offset + key.value
-        else:
-            i = key
-        if len(i) != len(self):
-            raise IndexError('inconsistent index length')
-
-        # unary index i of proper length
-        return runtime.in_prod(list(self), i)
-
-    def __setitem__(self, key, value):
-        """Called to set self[key] = value, where key is either public or secret.
-        The type of value should fit with the type of the list.
-
-        If key is a public integer (or a slice), the behavior is the same as for ordinary lists.
-        If key is a secure number or index, the list is updated at the secret position.
-        """
-        if isinstance(key, int):
-            if not isinstance(value, self.sectype):
-                value = self.sectype(value)
-            super().__setitem__(key, value)
-            return
-
-        if isinstance(key, slice):
-            if not isinstance(value, seclist):
-                value = seclist(value, self.sectype)
-            if not issubclass(value.sectype, self.sectype):
-                raise TypeError('inconsistent sectypes')
-
-            super().__setitem__(key, value)
-            return
-
-        if not isinstance(value, self.sectype):
-            value = self.sectype(value)
-
-        n = len(self)
-        if isinstance(key, self.sectype):
-            i = runtime.unit_vector(key, n)
-        elif isinstance(key, secindex):
-            i = [self.sectype(0)] * key.offset + key.value
-        else:
-            i = key
-        if len(i) != n:
-            raise IndexError('inconsistent index length')
-
-        # unary index i of proper length
-        x = list(self)
-        x_i = runtime.in_prod(x, i)
-        x = runtime.vector_add(x, runtime.scalar_mul(value - x_i, i))
-        super().__init__(x)
-
-    def __delitem__(self, key):
-        """Called to delete self[key], where key is either public or secret.
-
-        If key is a public integer (or a slice), the behavior is the same as for ordinary lists.
-        If key is a secure number or index, the list element at the secret position is removed.
-        """
-        if isinstance(key, (int, slice)):
-            super().__delitem__(key)
-            return
-
-        n = len(self)
-        if isinstance(key, self.sectype):
-            i = runtime.unit_vector(key, n)
-        elif isinstance(key, secindex):
-            i = [self.sectype(0)] * key.offset + key.value
-        else:
-            i = key[:]
-        i.pop()
-        if len(i) != n-1:
-            raise IndexError('inconsistent index length')
-
-        # unary index i of proper length
-        for j in range(1, n-1):
-            i[j] += i[j-1]
-        # step function i
-        x = list(self)
-        x1 = x[1:]
-        x.pop()
-        delta = runtime.schur_prod(i, runtime.vector_sub(x1, x))
-        x = runtime.vector_add(x, delta)
-        super().__init__(x)
-
-    def append(self, other):
-        if not isinstance(other, self.sectype):
-            other = self.sectype(other)
-        super().append(other)
-
-    def extend(self, other):
-        if not isinstance(other, seclist):
-            other = seclist(other, self.sectype)
-        super().extend(other)
-
-    def __add__(self, other):
-        sectype = self.sectype
-        if not isinstance(other, seclist):
-            other = seclist(other, sectype)
-        elif sectype != other.sectype:
-            raise TypeError('inconsistent sectypes')
-
-        return seclist(super().__add__(other), sectype)
-
-    def __radd__(self, other):
-        return seclist(other + list(self), self.sectype)
-
-    def __iadd__(self, other):
-        self.extend(other)
-        return self
-
-    def __mul__(self, other):
-        return seclist(super().__mul__(other), self.sectype)
-
-    def __rmul__(self, other):
-        return seclist(super().__mul__(other), self.sectype)
-
-    def __imul__(self, other):
-        super().__imul__(other)
-        return self
-
-    def insert(self, key, value):
-        """Insert value before position given by key, where key is either public or secret.
-        The key should fit with the length of the list: 0 <= key <= len(self).
-        The type of value should fit with the type of the list.
-
-        If key is a public integer, the behavior is the same as for ordinary lists.
-        If key is a secure number or index, the value is inserted at the secret position.
-        """
-        if isinstance(key, int):
-            if not isinstance(value, self.sectype):
-                value = self.sectype(value)
-            super().insert(key, value)
-            return
-
-        n = len(self)
-        if isinstance(key, self.sectype):
-            i = runtime.unit_vector(key, n+1)
-        elif isinstance(key, secindex):
-            i = [self.sectype(0)] * key.offset + key.value
-        else:
-            i = key[:]
-        if len(i) != n+1:
-            raise IndexError('inconsistent index length')
-
-        # unary index i of proper length
-        zero = self.sectype(0)
-        x = list(self)
-        x.insert(0, zero)
-        x_i = runtime.in_prod(x, i)
-        y = runtime.vector_add(x, runtime.scalar_mul(value - x_i, i))
-        x.pop(0)
-        x.append(zero)
-        for j in range(1, n+1):
-            i[j] += i[j-1]
-        # step function i
-        delta = runtime.schur_prod(i, runtime.vector_sub(y, x))
-        x = runtime.vector_add(x, delta)
-        super().__init__(x)
-
-    def pop(self, key=-1):
-        """Remove and return value at position given by key, where key is either public or secret.
-
-        If key is a public integer, the behavior is the same as for ordinary lists.
-        If key is a secure number or index, the item at the secret position is removed,
-        where 0 <= key < len(self).
-        """
-        if isinstance(key, int):
-            return super().pop(key)
-
-        n = len(self)
-        if isinstance(key, self.sectype):
-            i = runtime.unit_vector(key, n)
-        elif isinstance(key, secindex):
-            i = [self.sectype(0)] * key.offset + key.value
-        else:
-            i = key
-        if len(i) != n:
-            raise IndexError('inconsistent index length')
-
-        # unary index i of proper length
-        x_i = runtime.in_prod(list(self), i)
-        self.__delitem__(i)
-        return x_i
-
-    @asyncoro.mpc_coro
-    async def remove(self, value) -> Future:
-        """Remove first occurrence of value.
-
-        Raise ValueError if value is not present.
-        """
-        i = self.find(value)
-        if await runtime.eq_public(i, -1):
-            raise ValueError('value is not in list')
-
-        self.__delitem__(i)
-
-    def copy(self):
-        return seclist(super().copy(), self.sectype)
-
-#    def random_index(self):
-#        return secindex(random_unit_vector(self.sectype, len(self)))
-
-    def __contains__(self, item):
-        """Not implemented for secure lists.
-
-        Corresponds to "item in self", which is defined as a public Boolean value in Python.
-        Instead, use seclist.contains(self, item) to get a secure Boolean result in MPyC.
-        """
-        raise NotImplementedError('use seclist.contains()')
-
-    def contains(self, item):
-        """Check if item occurs in self."""
-        return self.count(item) != 0
-
-    def count(self, value):
-        """Return the number of occurrences of value."""
-        return runtime.sum([a == value for a in list(self)])
-
-    def find(self, value):  # TODO: add optional i and j to indicate slice
-        """Return index of the first occurrence of value.
-
-        If value is not present, then index is equal to -1.
-        """
-        if not self:
-            ix = self.sectype(-1)
-        else:
-            ix = runtime.find(list(self), value, bits=False, e=-1)
-        return ix
-
-    def index(self, value):  # TODO: add optional i and j to indicate slice
-        """Return index of the first occurrence of value.
-
-        Raise ValueError if value is not present.
-        """
-        return runtime.indexOf(list(self), value, bits=False)
-
-    def sort(self, key=None, reverse=False):
-        """Sort the list in-place, similar to Python's list.sort().
-
-        See runtime.sorted() for details on key etc.
-        """
-        if len(self) < 2:
-            return
-
-        if key is None:
-            key = lambda a: a
-        runtime._sort(self, key)
-        if reverse:
-            self.reverse()
-        return
-
-    @staticmethod
-    def _norm(stype, x, x2, EQ=False):
-        n = len(x)
-        if n == 1:
-            if not EQ:
-                a = (x2[0] - x[0])/stype.field(2)
-            else:
-                a = 1 - (x2[0] + x[0])/stype.field(2)
-            if issubclass(stype, SecureFixedPoint):
-                a.integral = True  # NB: in fact, a is a bit in {0,1}
-            return a, x2[0]
-
-        lte0, nz0 = seclist._norm(stype, x[:n//2], x2[:n//2], EQ)  # low positions
-        lte1, nz1 = seclist._norm(stype, x[n//2:], x2[n//2:], EQ)  # high positions
-        lte, nz = runtime.if_else(nz0, [lte0, nz0], [lte1, nz1])
-        return lte, nz
-
-    @staticmethod
-    def _less_than(stype, x, y):
-        s = [runtime.sgn(a - b) for a, b in zip(x, y)]
-        if not s:  # x=[] or y=[]
-            return stype(bool(y))  # x < y iff y!=[]
-
-        s2 = runtime.schur_prod(s, s)
-        EQ = len(x) < len(y)
-        return seclist._norm(stype, s, s2, EQ=EQ)[0]
-
-    def __lt__(self, other):
-        return seclist._less_than(self.sectype, self, other)
-
-    def __le__(self, other):
-        return 1 - seclist._less_than(self.sectype, other, self)
-
-    def __eq__(self, other):
-        if len(self) != len(other):
-            return self.sectype(0)
-
-        return runtime.all(a == b for a, b in zip(self, other))
-
-    def __ge__(self, other):
-        return 1 - seclist._less_than(self.sectype, self, other)
-
-    def __gt__(self, other):
-        return seclist._less_than(self.sectype, other, self)
-
-    def __ne__(self, other):
-        return 1 - self.__eq__(other)
-
-
-class secindex:
-    """Provisional class to facilitate more efficient manipulation of secure indices."""
-
-    __slots__ = 'value', 'offset', 'sectype'
-
-    def __init__(self, *args, offset=0, sectype=None):
-        if sectype is not None:
-            self.value = list(*args)
-        else:
-            x = seclist(*args)
-            sectype = x.sectype  # infer sectype from elements of x
-            self.value = list(x)
-        self.offset = offset
-        self.sectype = sectype
-
-    def __add__(self, other):
-        field = self.sectype.field
-        m = len(self.value)
-        n = len(other.value)
-        i = runtime.in_prod(self.value, [field(_) for _ in range(m)])
-        j = runtime.in_prod(other.value, [field(_) for _ in range(n)])
-        k = runtime.unit_vector(i + j, m + n - 1)
-        offset = self.offset + other.offset
-        return secindex(k, offset=offset)
-
-    async def __index__(self):
-        field = self.sectype.field
-        f = self.sectype.frac_length
-        i = runtime.in_prod(self.value, [field(_) for _ in range(len(self.value))])
-        i = await runtime.output(i)
-        return self.offset + i.value >> f
-
-    def __await__(self):
-        return self.__index__().__await__()
-
-    @staticmethod
-    def random(sectype, length, offset=0):
-        n = length
-        return secindex(random_unit_vector(sectype, n), offset=offset)
+"""This module provides a secure (oblivious) alternative to Python lists.
+
+A secure list contains secret-shared numbers. Apart from hiding the contents of the
+list, however, it is also possible to hide which items are accessed and which items
+are updated. In principle, only the length of a secure list remains public.
+
+A secure list x can be cast to an ordinary list by using list(x), without affecting
+the contents of the list. Also, public access to a secure list proceeds the same as
+for ordinary Python lists, using an index or a slice.
+
+For secure (oblivious) access to a secure list, however, one uses a secret-shared
+index i, which is either a secure number or a secure unit vector. Index i must be
+compatible with the secure list x: the type of i must fit with the type of the
+elements of x and the value of i must fit with the length of list x, that is,
+0 <= i < len(x).
+
+Common usage scenarios of secure lists are supported through methods such as sort(),
+count(), and index(), or can be coded easily. For example, the frequency of values
+in a list x of secure integers (whose values are known to be between 0 and n-1)
+is computed by:
+
+    s = seclist([0]*n, secint)
+
+    for a in x: s[a] += 1
+
+Current implementation is basic, taking advantage of cheap secure dot products, as
+provided by runtime.in_prod(). Performance for modestly sized lists of lengths 10 to 1000
+should be adequate. Later: With better amortized complexity, e.g., square root ORAM.
+"""
+
+from asyncio import Future
+from mpyc.sectypes import SecureObject, SecureFixedPoint
+from mpyc.random import random_unit_vector
+from mpyc import asyncoro
+
+runtime = None
+
+
+class seclist(list):
+
+    sectype = None
+
+    def __init__(self, x=(), sectype=None):
+        """Build a secure list from the items in iterable x using the given secure type.
+
+        If no secure type is given, it is inferred from the items in x.
+
+        Invariant: all items in a secure list are of the same secure type.
+        """
+        parent = super()
+        parent.__init__(x)
+        t = len(self)
+        for a in self:
+            if isinstance(a, SecureObject):
+                t -= 1
+                if sectype is None:
+                    sectype = type(a)
+                elif sectype != type(a):
+                    raise TypeError('inconsistent sectypes')
+
+        if sectype is None:
+            raise ValueError('sectype missing')
+
+        i = 0
+        while t:
+            while isinstance(a := parent.__getitem__(i), SecureObject):
+                i += 1
+            parent.__setitem__(i, sectype(a))
+            t -= 1
+        self.sectype = sectype
+
+    def __getitem__(self, key):
+        """Called to evaluate self[key], where key is either public or secret.
+
+        If key is a public integer (or a slice), the behavior is the same as for ordinary lists.
+        If key is a secure number or index, the value at the secret position is returned.
+        """
+        if isinstance(key, (int, slice)):
+            value = super().__getitem__(key)
+            if isinstance(key, slice):
+                value = seclist(value, self.sectype)
+            return value
+
+        if isinstance(key, self.sectype):
+            i = runtime.unit_vector(key, len(self))
+        elif isinstance(key, secindex):
+            i = [self.sectype(0)] * key.offset + key.value
+        else:
+            i = key
+        if len(i) != len(self):
+            raise IndexError('inconsistent index length')
+
+        # unary index i of proper length
+        return runtime.in_prod(list(self), i)
+
+    def __setitem__(self, key, value):
+        """Called to set self[key] = value, where key is either public or secret.
+        The type of value should fit with the type of the list.
+
+        If key is a public integer (or a slice), the behavior is the same as for ordinary lists.
+        If key is a secure number or index, the list is updated at the secret position.
+        """
+        if isinstance(key, int):
+            if not isinstance(value, self.sectype):
+                value = self.sectype(value)
+            super().__setitem__(key, value)
+            return
+
+        if isinstance(key, slice):
+            if not isinstance(value, seclist):
+                value = seclist(value, self.sectype)
+            if not issubclass(value.sectype, self.sectype):
+                raise TypeError('inconsistent sectypes')
+
+            super().__setitem__(key, value)
+            return
+
+        if not isinstance(value, self.sectype):
+            value = self.sectype(value)
+
+        n = len(self)
+        if isinstance(key, self.sectype):
+            i = runtime.unit_vector(key, n)
+        elif isinstance(key, secindex):
+            i = [self.sectype(0)] * key.offset + key.value
+        else:
+            i = key
+        if len(i) != n:
+            raise IndexError('inconsistent index length')
+
+        # unary index i of proper length
+        x = list(self)
+        x_i = runtime.in_prod(x, i)
+        x = runtime.vector_add(x, runtime.scalar_mul(value - x_i, i))
+        super().__init__(x)
+
+    def __delitem__(self, key):
+        """Called to delete self[key], where key is either public or secret.
+
+        If key is a public integer (or a slice), the behavior is the same as for ordinary lists.
+        If key is a secure number or index, the list element at the secret position is removed.
+        """
+        if isinstance(key, (int, slice)):
+            super().__delitem__(key)
+            return
+
+        n = len(self)
+        if isinstance(key, self.sectype):
+            i = runtime.unit_vector(key, n)
+        elif isinstance(key, secindex):
+            i = [self.sectype(0)] * key.offset + key.value
+        else:
+            i = key[:]
+        i.pop()
+        if len(i) != n-1:
+            raise IndexError('inconsistent index length')
+
+        # unary index i of proper length
+        for j in range(1, n-1):
+            i[j] += i[j-1]
+        # step function i
+        x = list(self)
+        x1 = x[1:]
+        x.pop()
+        delta = runtime.schur_prod(i, runtime.vector_sub(x1, x))
+        x = runtime.vector_add(x, delta)
+        super().__init__(x)
+
+    def append(self, other):
+        if not isinstance(other, self.sectype):
+            other = self.sectype(other)
+        super().append(other)
+
+    def extend(self, other):
+        if not isinstance(other, seclist):
+            other = seclist(other, self.sectype)
+        super().extend(other)
+
+    def __add__(self, other):
+        sectype = self.sectype
+        if not isinstance(other, seclist):
+            other = seclist(other, sectype)
+        elif sectype != other.sectype:
+            raise TypeError('inconsistent sectypes')
+
+        return seclist(super().__add__(other), sectype)
+
+    def __radd__(self, other):
+        return seclist(other + list(self), self.sectype)
+
+    def __iadd__(self, other):
+        self.extend(other)
+        return self
+
+    def __mul__(self, other):
+        return seclist(super().__mul__(other), self.sectype)
+
+    def __rmul__(self, other):
+        return seclist(super().__mul__(other), self.sectype)
+
+    def __imul__(self, other):
+        super().__imul__(other)
+        return self
+
+    def insert(self, key, value):
+        """Insert value before position given by key, where key is either public or secret.
+        The key should fit with the length of the list: 0 <= key <= len(self).
+        The type of value should fit with the type of the list.
+
+        If key is a public integer, the behavior is the same as for ordinary lists.
+        If key is a secure number or index, the value is inserted at the secret position.
+        """
+        if isinstance(key, int):
+            if not isinstance(value, self.sectype):
+                value = self.sectype(value)
+            super().insert(key, value)
+            return
+
+        n = len(self)
+        if isinstance(key, self.sectype):
+            i = runtime.unit_vector(key, n+1)
+        elif isinstance(key, secindex):
+            i = [self.sectype(0)] * key.offset + key.value
+        else:
+            i = key[:]
+        if len(i) != n+1:
+            raise IndexError('inconsistent index length')
+
+        # unary index i of proper length
+        zero = self.sectype(0)
+        x = list(self)
+        x.insert(0, zero)
+        x_i = runtime.in_prod(x, i)
+        y = runtime.vector_add(x, runtime.scalar_mul(value - x_i, i))
+        x.pop(0)
+        x.append(zero)
+        for j in range(1, n+1):
+            i[j] += i[j-1]
+        # step function i
+        delta = runtime.schur_prod(i, runtime.vector_sub(y, x))
+        x = runtime.vector_add(x, delta)
+        super().__init__(x)
+
+    def pop(self, key=-1):
+        """Remove and return value at position given by key, where key is either public or secret.
+
+        If key is a public integer, the behavior is the same as for ordinary lists.
+        If key is a secure number or index, the item at the secret position is removed,
+        where 0 <= key < len(self).
+        """
+        if isinstance(key, int):
+            return super().pop(key)
+
+        n = len(self)
+        if isinstance(key, self.sectype):
+            i = runtime.unit_vector(key, n)
+        elif isinstance(key, secindex):
+            i = [self.sectype(0)] * key.offset + key.value
+        else:
+            i = key
+        if len(i) != n:
+            raise IndexError('inconsistent index length')
+
+        # unary index i of proper length
+        x_i = runtime.in_prod(list(self), i)
+        self.__delitem__(i)
+        return x_i
+
+    @asyncoro.mpc_coro
+    async def remove(self, value) -> Future:
+        """Remove first occurrence of value.
+
+        Raise ValueError if value is not present.
+        """
+        i = self.find(value)
+        if await runtime.eq_public(i, -1):
+            raise ValueError('value is not in list')
+
+        self.__delitem__(i)
+
+    def copy(self):
+        return seclist(super().copy(), self.sectype)
+
+#    def random_index(self):
+#        return secindex(random_unit_vector(self.sectype, len(self)))
+
+    def __contains__(self, item):
+        """Not implemented for secure lists.
+
+        Corresponds to "item in self", which is defined as a public Boolean value in Python.
+        Instead, use seclist.contains(self, item) to get a secure Boolean result in MPyC.
+        """
+        raise NotImplementedError('use seclist.contains()')
+
+    def contains(self, item):
+        """Check if item occurs in self."""
+        return self.count(item) != 0
+
+    def count(self, value):
+        """Return the number of occurrences of value."""
+        return runtime.sum([a == value for a in list(self)])
+
+    def find(self, value):  # TODO: add optional i and j to indicate slice
+        """Return index of the first occurrence of value.
+
+        If value is not present, then index is equal to -1.
+        """
+        if not self:
+            ix = self.sectype(-1)
+        else:
+            ix = runtime.find(list(self), value, bits=False, e=-1)
+        return ix
+
+    def index(self, value):  # TODO: add optional i and j to indicate slice
+        """Return index of the first occurrence of value.
+
+        Raise ValueError if value is not present.
+        """
+        return runtime.indexOf(list(self), value, bits=False)
+
+    def sort(self, key=None, reverse=False):
+        """Sort the list in-place, similar to Python's list.sort().
+
+        See runtime.sorted() for details on key etc.
+        """
+        if len(self) < 2:
+            return
+
+        if key is None:
+            key = lambda a: a
+        runtime._sort(self, key)
+        if reverse:
+            self.reverse()
+        return
+
+    @staticmethod
+    def _norm(stype, x, x2, EQ=False):
+        n = len(x)
+        if n == 1:
+            if not EQ:
+                a = (x2[0] - x[0])/stype.field(2)
+            else:
+                a = 1 - (x2[0] + x[0])/stype.field(2)
+            if issubclass(stype, SecureFixedPoint):
+                a.integral = True  # NB: in fact, a is a bit in {0,1}
+            return a, x2[0]
+
+        lte0, nz0 = seclist._norm(stype, x[:n//2], x2[:n//2], EQ)  # low positions
+        lte1, nz1 = seclist._norm(stype, x[n//2:], x2[n//2:], EQ)  # high positions
+        lte, nz = runtime.if_else(nz0, [lte0, nz0], [lte1, nz1])
+        return lte, nz
+
+    @staticmethod
+    def _less_than(stype, x, y):
+        s = [runtime.sgn(a - b) for a, b in zip(x, y)]
+        if not s:  # x=[] or y=[]
+            return stype(bool(y))  # x < y iff y!=[]
+
+        s2 = runtime.schur_prod(s, s)
+        EQ = len(x) < len(y)
+        return seclist._norm(stype, s, s2, EQ=EQ)[0]
+
+    def __lt__(self, other):
+        return seclist._less_than(self.sectype, self, other)
+
+    def __le__(self, other):
+        return 1 - seclist._less_than(self.sectype, other, self)
+
+    def __eq__(self, other):
+        if len(self) != len(other):
+            return self.sectype(0)
+
+        return runtime.all(a == b for a, b in zip(self, other))
+
+    def __ge__(self, other):
+        return 1 - seclist._less_than(self.sectype, self, other)
+
+    def __gt__(self, other):
+        return seclist._less_than(self.sectype, other, self)
+
+    def __ne__(self, other):
+        return 1 - self.__eq__(other)
+
+
+class secindex:
+    """Provisional class to facilitate more efficient manipulation of secure indices."""
+
+    __slots__ = 'value', 'offset', 'sectype'
+
+    def __init__(self, *args, offset=0, sectype=None):
+        if sectype is not None:
+            self.value = list(*args)
+        else:
+            x = seclist(*args)
+            sectype = x.sectype  # infer sectype from elements of x
+            self.value = list(x)
+        self.offset = offset
+        self.sectype = sectype
+
+    def __add__(self, other):
+        field = self.sectype.field
+        m = len(self.value)
+        n = len(other.value)
+        i = runtime.in_prod(self.value, [field(_) for _ in range(m)])
+        j = runtime.in_prod(other.value, [field(_) for _ in range(n)])
+        k = runtime.unit_vector(i + j, m + n - 1)
+        offset = self.offset + other.offset
+        return secindex(k, offset=offset)
+
+    async def __index__(self):
+        field = self.sectype.field
+        f = self.sectype.frac_length
+        i = runtime.in_prod(self.value, [field(_) for _ in range(len(self.value))])
+        i = await runtime.output(i)
+        return self.offset + i.value >> f
+
+    def __await__(self):
+        return self.__index__().__await__()
+
+    @staticmethod
+    def random(sectype, length, offset=0):
+        n = length
+        return secindex(random_unit_vector(sectype, n), offset=offset)
```

### Comparing `mpyc-0.8/mpyc/statistics.py` & `mpyc-0.9/mpyc/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,40 +375,15 @@
         x = data
     ld = len(x)
     if ld < 2:
         raise statistics.StatisticsError('must have at least two data points')
 
     sectype = type(x[0])  # all elts of x assumed of same type
     if not issubclass(sectype, SecureObject):
-        if sys.version_info.minor >= 8:
-            return statistics.quantiles(x, n=n, method=method)
-
-        data = sorted(x)
-
-        if method == 'inclusive':
-            m = ld - 1
-            result = []
-            for i in range(1, n):
-                j, delta = divmod(i * m, n)
-                interpolated = (data[j] * (n - delta) + data[j + 1] * delta) / n
-                result.append(interpolated)
-            return result
-
-        if method == 'exclusive':
-            m = ld + 1
-            result = []
-            for i in range(1, n):
-                j = i * m // n                               # rescale i to m/n
-                j = 1 if j < 1 else ld-1 if j > ld-1 else j  # clamp to 1 .. ld-1
-                delta = i*m - j*n                            # exact integer math
-                interpolated = (data[j - 1] * (n - delta) + data[j] * delta) / n
-                result.append(interpolated)
-            return result
-
-        raise ValueError(f'Unknown method: {method!r}')
+        return statistics.quantiles(x, n=n, method=method)
 
     if issubclass(sectype, SecureFixedPoint):
         div_n = lambda a: a / n
     elif issubclass(sectype, SecureInteger):
         div_n = lambda a: (a + n//2) // n
     else:
         raise TypeError('secure fixed-point or integer type required')
@@ -437,15 +412,15 @@
 
     if method == 'exclusive':
         m = ld + 1
         # Determine which kth order statistics will actually be used.
         data = {}
         for i in range(1, n):
             j = i * m // n
-            j = 1 if j < 1 else ld-1 if j > ld-1 else j
+            j = 1 if j < 1 else ld-1 if j > ld-1 else j  # clamp to 1 .. ld-1
             delta = i*m - j*n
             if n - delta:
                 data[j-1] = None
             if delta:
                 data[j] = None
         points = _quickselect(x, list(data))
         data = dict(zip(data, points))
@@ -486,15 +461,15 @@
     n = len(x)
     if not n:
         raise statistics.StatisticsError('mode requires at least one data point')
 
     if isinstance(x[0], SecureObject):
         return _mode(x, PRIV=runtime.options.sec_param//6)
 
-    return statistics.mode(x)  # NB: raises StatisticsError in Python < 3.8 if x is multimodal
+    return statistics.mode(x)
 
 
 @asyncoro.mpc_coro
 async def _mode(x, PRIV=0):
     sectype = type(x[0])  # all elts of x assumed of same type
     if not issubclass(sectype, (SecureFixedPoint, SecureInteger)):
         raise TypeError('secure fixed-point or integer type required')
```

### Comparing `mpyc-0.8/mpyc/thresha.py` & `mpyc-0.9/mpyc/thresha.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,104 +5,144 @@
 secrets without any communication, as long as the parties
 agree on a (unique) common public input for each secret.
 
 PRSS relies on parties having agreed upon the keys for a pseudorandom
 function (PRF).
 """
 
-__all__ = ['random_split', 'recombine', 'pseudorandom_share',
-           'pseudorandom_share_zero', 'PRF']
+__all__ = ['random_split', 'recombine', 'pseudorandom_share', 'pseudorandom_share_zero',
+           'np_random_split', 'np_recombine', 'np_pseudorandom_share', 'np_pseudorandom_share_0',
+           'PRF']
 
+from math import prod
 import functools
-import hashlib
+from hashlib import shake_128
 import secrets
+from mpyc.numpy import np
 
 
-def random_split(s, t, m):
+def random_split(field, s, t, m):
     """Split each secret given in s into m random Shamir shares.
 
-    The (maximum) degree for the Shamir polynomials is t, 0 <= t < n.
+    The (maximum) degree for the Shamir polynomials is t, 0 <= t < m.
     Return matrix of shares, one row per party.
     """
-    field = type(s[0])
     p = field.modulus
     order = field.order
-    T = type(p)  # T is int or gfpx.Polynomial
-    n = len(s)
-    shares = [[None] * n for _ in range(m)]
-    for h in range(n):
+    _0 = type(p)(0)  # _0 is int(0) or gfpx.Polynomial(0)
+    shares = [[None] * len(s) for _ in range(m)]
+    T_is_field = isinstance(s[0], field)  # all elts assumed of same type
+    for h, s_h in enumerate(s):
+        if T_is_field:
+            s_h = s_h.value
         c = [secrets.randbelow(order) for _ in range(t)]
         # polynomial f(X) = s[h] + c[t-1] X + c[t-2] X^2 + ... + c[0] X^t
-        for i in range(m):
-            y = 0 if T is int else T(0)
+        for i1 in range(1, m+1):
+            y = _0
             for c_j in c:
-                y += c_j
-                y *= i+1
-            shares[i][h] = (y + s[h].value) % p
+                y = (y + c_j) * i1
+            shares[i1-1][h] = (y + s_h) % p
+    return shares
+
+
+def np_random_split(field, s, t, m):
+    """Split each secret given in s into m random Shamir shares.
+
+    The (maximum) degree for the Shamir polynomials is t, 0 <= t < m.
+    Return matrix of shares, one row per party.
+    """
+    p = field.modulus
+    tp = type(p)  # int or gfpx.Polynomial
+    if isinstance(s, field.array):
+        s = s.value
+    n = len(s)
+    _randbelow = secrets.randbelow
+    order = field.order
+    C = np.fromiter((_randbelow(order) for _ in range(t * n)), dtype='O').reshape(t, n)
+    V = np.vander(np.array([tp(i) for i in range(1, m+1)], dtype='O'), N=t+1, increasing=True)
+    # NB: each entry in first column of V is a 1 of type int (also if tp is gfpx.Polynomial)
+    shares = (V @ np.concatenate((s.reshape(1, n), C))) % p
     return shares
 
 
 @functools.lru_cache(maxsize=None)
 def _recombination_vector(field, xs, x_r):
     """Compute and store a recombination vector.
 
     A recombination vector depends on the field, the x-coordinates xs
     of the shares and the x-coordinate x_r of the recombination point.
     """
     xs = [field(x).value for x in xs]
     x_r = field(x_r).value
     vector = []
     for i, x_i in enumerate(xs):
-        coefficient_d = field(1)
         coefficient_n = field(1)
+        coefficient_d = field(1)
         for j, x_j in enumerate(xs):
             if i != j:
-                coefficient_d *= (x_r - x_j)
-                coefficient_n *= (x_i - x_j)
-        vector.append((coefficient_d / coefficient_n).value)
+                coefficient_n *= (x_r - x_j)
+                coefficient_d *= (x_i - x_j)
+        vector.append((coefficient_n / coefficient_d).value)
     return vector
 
 
 def recombine(field, points, x_rs=0):
     """Recombine shares given by points into secrets.
 
     Recombination is done for x-coordinates x_rs.
     """
     xs, shares = list(zip(*points))
     if not isinstance(x_rs, list):
         x_rs = (x_rs,)
-    n = len(shares[0])
     width = len(x_rs)
-    T_is_field = isinstance(shares[0][0], field)  # all elts assumed of same type
     vector = [_recombination_vector(field, xs, x_r) for x_r in x_rs]
+
+    n = len(shares[0])
     sums = [[0] * n for _ in range(width)]
+    T_is_field = isinstance(shares[0][0], field)  # all elts assumed of same type
     for i, share_i in enumerate(shares):
         for h in range(n):
             s = share_i[h]
             if T_is_field:
                 s = s.value
             # type(s) is int or gfpx.Polynomial
             for r in range(width):
                 sums[r][h] += s * vector[r][i]
-    for r in range(width):
-        for h in range(n):
-            sums[r][h] = field(sums[r][h])
+    if T_is_field:
+        for r in range(width):
+            for h in range(n):
+                sums[r][h] = field(sums[r][h])
     if isinstance(x_rs, tuple):
-        return sums[0]
+        sums = sums[0]
+    return sums
+
+
+def np_recombine(field, points, x_rs=0):
+    """Recombine shares given by points into secrets.
 
+    Recombination is done for x-coordinates x_rs.
+    """
+    xs, shares = list(zip(*points))
+    if not isinstance(x_rs, list):
+        x_rs = (x_rs,)
+    vector = np.array([_recombination_vector(field, xs, x_r) for x_r in x_rs], dtype='O')
+    shares = field.array(shares)
+    sums = vector @ shares
+    if isinstance(x_rs, tuple):
+        sums = sums[0]
     return sums
 
 
 @functools.lru_cache(maxsize=None)
 def _f_S_i(field, m, i, S):
     """Compute and store polynomial f_S evaluated for party i.
 
     Polynomial f_S is 1 at 0 and 0 for all parties j outside S."""
     points = [(0, [1])] + [(x+1, [0]) for x in range(m) if x not in S]
-    return recombine(field, points, i+1)[0].value
+    return recombine(field, points, i+1)[0]
 
 
 def pseudorandom_share(field, m, i, prfs, uci, n):
     """Return pseudorandom Shamir shares for party i for n random numbers.
 
     The shares are based on the pseudorandom functions for party i,
     given in prfs, which maps subsets of parties to PRF instances.
@@ -116,39 +156,71 @@
         for h in range(n):
             sums[h] += prl[h] * f_S_i
     for h in range(n):
         sums[h] = field(sums[h])
     return sums
 
 
+def np_pseudorandom_share(field, m, i, prfs, uci, n):
+    """Return pseudorandom Shamir shares for party i for n random numbers.
+
+    The shares are based on the pseudorandom functions for party i,
+    given in prfs, which maps subsets of parties to PRF instances.
+    Input uci is used to evaluate the PRFs on a unique common input.
+    """
+    # sum over (m-1 choose t) subsets for degree t.
+    s = sum(prf_S(uci, (n,)) * _f_S_i(field, m, i, S)
+            for S, prf_S in prfs.items())
+    return field.array(s)
+
+
 def pseudorandom_share_zero(field, m, i, prfs, uci, n):
     """Return pseudorandom Shamir shares for party i for n sharings of 0.
 
     The shares are based on the pseudorandom functions for party i,
     given in prfs, which maps subsets of parties to PRF instances.
     Input uci is used to evaluate the PRFs on a unique common input.
     """
-    T = type(field.modulus)  # T is int or T is gfpx.Polynomial
+    _0 = type(field.modulus)(0)  # _0 is int(0) or gfpx.Polynomial(0)
+    i1 = i + 1
     sums = [0] * n
     # iterate over (m-1 choose t) subsets for degree t.
     for S, prf_S in prfs.items():
         f_S_i = _f_S_i(field, m, i, S)
         d = m - len(S)
         prl = prf_S(uci, n * d)
         for h in range(n):
-            y = 0 if T is int else T(0)
+            y = _0
             for j in range(d):
-                y += prl[h * d + j]
-                y *= i+1
+                y = (y + prl[h * d + j]) * i1
             sums[h] += y * f_S_i
     for h in range(n):
         sums[h] = field(sums[h])
     return sums
 
 
+def np_pseudorandom_share_0(field, m, i, prfs, uci, n):
+    """Return pseudorandom Shamir shares for party i for n sharings of 0.
+
+    The shares are based on the pseudorandom functions for party i,
+    given in prfs, which maps subsets of parties to PRF instances.
+    Input uci is used to evaluate the PRFs on a unique common input.
+    """
+    vtype = type(field.modulus)  # int or gfpx.Polynomial
+    d = m - len(next(iter(prfs.keys())))  # subsets all of same size m-t
+    i1s = np.array([vtype(i+1)**j for j in range(1, d+1)], dtype='O')
+    sums = vtype(0)
+    # iterate over (m-1 choose t) subsets for degree t.
+    for S, prf_S in prfs.items():
+        f_S_i = _f_S_i(field, m, i, S)
+        prl = prf_S(uci, (n, d))
+        sums += (prl @ i1s) * f_S_i
+    return field.array(sums)
+
+
 class PRF:
     """A pseudorandom function (PRF).
 
     A PRF is determined by a secret key and a public maximum.
     """
 
     def __init__(self, key, bound):
@@ -160,22 +232,35 @@
         self.key = key
         self.max = bound
         self.byte_length = ((bound - 1).bit_length() + 7) // 8
         if bound & (bound - 1):  # no power of 2
             self.byte_length += len(self.key)
 
     def __call__(self, s, n=None):
-        """Return a number or length-n list of numbers in range(self.max) for input bytes s."""
-        if n == 0:
-            return []
+        """Return pseudorandom number(s) in range(self.max) for given input bytes s.
 
+        The numbers are a deterministic function of self.key and input s.
+        If n is None, a single number is returned.
+        If n is a (nonnegative) integer, a length-n list is returned.
+        If n is a shape, a shape-n array is returned.
+        """
+        if isinstance(n, tuple):
+            shape = n
+            n = prod(shape)
+        else:
+            shape = None
         n_ = 1 if n is None else n
-        l = self.byte_length
-        if not l:
-            x = [0] * n_
+        if n_ == 0:
+            iterable = ()
+        elif not (l := self.byte_length):
+            iterable = (0 for _ in range(n_))
         else:
-            dk = hashlib.pbkdf2_hmac('sha1', self.key, s, 1, n_ * l)
+            dk = shake_128(self.key + s).digest(n_ * l)
             byteorder = 'little'
             from_bytes = int.from_bytes  # cache
             bound = self.max
-            x = [from_bytes(dk[i:i + l], byteorder) % bound for i in range(0, n_ * l, l)]
+            iterable = (from_bytes(dk[i:i + l], byteorder) % bound for i in range(0, n_ * l, l))
+        if shape is None:
+            x = list(iterable)
+        else:
+            x = np.fromiter(iterable, object, count=n_).reshape(shape)
         return x[0] if n is None else x
```

### Comparing `mpyc-0.8/mpyc.egg-info/PKG-INFO` & `mpyc-0.9/mpyc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mpyc
-Version: 0.8
-Summary: MPyC -- Secure Multiparty Computation in Python
+Version: 0.9
+Summary: MPyC for Multiparty Computation in Python
 Home-page: https://github.com/lschoe/mpyc
 Author: Berry Schoenmakers
 Author-email: berry@win.tue.nl
 License: MIT License
 Keywords: crypto,cryptography,multiparty computation,MPC,secret sharing,Shamir threshold scheme,pseudorandom secret sharing,PRSS
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -19,69 +19,69 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lschoe/mpyc/master)
 [![Travis CI](https://app.travis-ci.com/lschoe/mpyc.svg)](https://app.travis-ci.com/lschoe/mpyc)
 [![codecov](https://codecov.io/gh/lschoe/mpyc/branch/master/graph/badge.svg)](https://codecov.io/gh/lschoe/mpyc)
 [![Read the Docs](https://readthedocs.org/projects/mpyc/badge/)](https://mpyc.readthedocs.io)
 [![PyPI](https://img.shields.io/pypi/v/mpyc.svg)](https://pypi.org/project/mpyc/)
 
-# MPyC [![MPyC logo](https://raw.githubusercontent.com/lschoe/mpyc/master/images/MPyC_Logo.svg)](https://github.com/lschoe/mpyc) Secure Multiparty Computation in Python
+# MPyC [![MPyC logo](https://raw.githubusercontent.com/lschoe/mpyc/master/images/MPyC_Logo.svg)](https://github.com/lschoe/mpyc) Multiparty Computation in Python
 
 MPyC supports secure *m*-party computation tolerating a dishonest minority of up to *t* passively corrupt parties,
 where *m &ge; 1* and *0 &le; t &lt; m/2*. The underlying cryptographic protocols are based on threshold secret sharing over finite
 fields (using Shamir's threshold scheme as well as pseudorandom secret sharing).
 
 The details of the secure computation protocols are mostly transparent due to the use of sophisticated operator overloading
 combined with asynchronous evaluation of the associated protocols.
 
-See the [MPyC homepage](https://www.win.tue.nl/~berry/mpyc/) for more info and background.
+## Documentation
 
-Click the "launch binder" badge above to view the entire repository and try out the Jupyter notebooks from the `demos` directory
-in the cloud, without any install.
+[Read the Docs](https://mpyc.readthedocs.io/) for `Sphinx`-based documentation, including an overview of the `demos`.\
+[GitHub Pages](https://lschoe.github.io/mpyc/) for `pydoc`-based documentation.
 
-## Installation:
+See `demos` for Python programs and Jupyter notebooks with lots of example code. Click the "launch binder" badge above to view the entire
+repository and try out the Jupyter notebooks from the `demos` directory in the cloud, without any install.
 
-Just run: `python setup.py install` (pure Python, no dependencies).
+The [MPyC homepage](https://www.win.tue.nl/~berry/mpyc/) has some more info and background.
 
-See `demos` for Python programs and Jupyter notebooks with lots of example code.
+## Installation
 
-See [Read the Docs](https://mpyc.readthedocs.io/) for `Sphinx`-based documentation, including an overview of the `demos`,
-and [GitHub Pages](https://lschoe.github.io/mpyc/) for `pydoc`-based documentation.
+Pure Python, no dependencies. Python 3.8+ (following [NumPy's deprecation policy](https://numpy.org/neps/nep-0029-deprecation_policy.html#support-table)).
 
-## Notes:
+Run `pip install .` in the root directory (containing file `setup.py`).\
+Or, run `pip install -e .`, if you want to edit the MPyC source files.
 
-1. Python 3.6+ (Python 3.5 or lower is not sufficient).
+Use `pip install numpy` to enable support for secure NumPy arrays in MPyC, along with vectorized implementations.
 
-2. Installing package [gmpy2](https://pypi.org/project/gmpy2/) is optional, but will considerably enhance the performance of `mpyc`.
-As of December 12, 2021 with the release of gmpy2 2.1, installation has been simplified greatly:
-`pip install gmpy2` is now supported on all major Linux/MacOS/Windows platforms via prebuilt wheels.
-If you use the [conda](https://docs.conda.io/) package and environment manager, `conda install gmpy2` should do the job.
+Use `pip install gmpy2` to run MPyC with the package [gmpy2](https://pypi.org/project/gmpy2/) for considerably better performance.
 
-3. Use `run-all.sh` or `run-all.bat` in the `demos` directory to have a quick look at all pure Python demos.
+### Some Tips
+
+- Try `run-all.sh` or `run-all.bat` in the `demos` directory to have a quick look at all pure Python demos.
 Demos `bnnmnist.py` and `cnnmnist.py` require [NumPy](https://www.numpy.org/), demo `kmsurvival.py` requires
 [pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), and [lifelines](https://pypi.org/project/lifelines/),
-and demo `ridgeregression.py` (and therefore demo `multilateration.py`) even require [Scikit-learn](https://scikit-learn.org/).
-Also note the example Linux shell scripts and Windows batch files in the `docs` and `tests` directories.
-
-4. Directory `demos\.config` contains configuration info used to run MPyC with multiple parties. Also, Windows batch
-file `gen.bat` shows how to generate fresh key material for SSL. To generate SSL key material of your own, first run
-`pip install cryptography` (alternatively, run `pip install pyOpenSSL`, which will also install the `cryptography` package).
-
-5. To use the [Jupyter](https://jupyter.org/) notebooks `demos\*.ipynb`, you need to have Jupyter installed,
-e.g., using `pip install jupyter`. The latest version of Jupyter will come with IPython 7.x, which supports
-top-level `await`. For example, instead of `mpc.run(mpc.start())` one can now simply write `await mpc.start()` anywhere in
-a notebook cell, even outside a coroutine.
-
-6. For Python 3.8+, you also get top-level `await` by running `python -m asyncio` to launch a natively async REPL.
+and demo `ridgeregression.py` (and therefore demo `multilateration.py`) even require [Scikit-learn](https://scikit-learn.org/).\
+Try `np-run-all.sh` or `np-run-all.bat` in the `demos` directory to run all Python demos employing MPyC's secure arrays.
+Major speedups are achieved due to the reduced overhead of secure arrays and vectorized processing throughout the
+protocols.
+
+- To use the [Jupyter](https://jupyter.org/) notebooks `demos\*.ipynb`, you need to have Jupyter installed,
+e.g., using `pip install jupyter`. An interesting feature of Jupyter is the support of top-level `await`.
+For example, instead of `mpc.run(mpc.start())` you can simply use `await mpc.start()` anywhere in
+a notebook cell, even outside a coroutine.\
+For Python, you also get top-level `await` by running `python -m asyncio` to launch a natively async REPL.
 By running `python -m mpyc` instead you even get this REPL with the MPyC runtime preloaded!
 
-Copyright &copy; 2018-2021 Berry Schoenmakers
+- Directory `demos\.config` contains configuration info used to run MPyC with multiple parties.
+The file `gen.bat` shows how to generate fresh key material for SSL. To generate SSL key material of your own, first run
+`pip install cryptography` (alternatively, run `pip install pyOpenSSL`).
 
+Copyright &copy; 2018-2023 Berry Schoenmakers
```

### Comparing `mpyc-0.8/setup.py` & `mpyc-0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """MPyC setup script.
 
-Options:                python setup.py --help
-Install by admin/root:  python setup.py install
-Install by user:        python setup.py install --user
-Install options:        python setup.py install --help
+Run: "pip install ."
+Or:  "pip install -e ."
 """
 
 from setuptools import setup
 import mpyc
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='mpyc',
     version=mpyc.__version__,
     author='Berry Schoenmakers',
     author_email='berry@win.tue.nl',
     url='https://github.com/lschoe/mpyc',
-    description='MPyC -- Secure Multiparty Computation in Python',
+    description='MPyC for Multiparty Computation in Python',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=['crypto', 'cryptography', 'multiparty computation', 'MPC',
               'secret sharing', 'Shamir threshold scheme',
               'pseudorandom secret sharing', 'PRSS'],
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -40,9 +38,9 @@
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Distributed Computing'
     ],
     license=mpyc.__license__,
     packages=['mpyc'],
     platforms=['any'],
-    python_requires='>=3.6'
+    python_requires='>=3.8'
 )
```

