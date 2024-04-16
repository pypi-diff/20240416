# Comparing `tmp/ereg-0.0.8-py3-none-any.whl.zip` & `tmp/ereg-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20675 bytes, number of entries: 16
+Zip file size: 20869 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      171 b- defN 80-Jan-01 00:00 ereg/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ereg/cli/__init__.py
 -rw-r--r--  2.0 unx     4031 b- defN 80-Jan-01 00:00 ereg/cli/run.py
 -rw-r--r--  2.0 unx     3617 b- defN 80-Jan-01 00:00 ereg/configurations/default_rigid.yaml
 -rw-r--r--  2.0 unx     3600 b- defN 80-Jan-01 00:00 ereg/configurations/sample_config.yaml
 -rw-r--r--  2.0 unx     1575 b- defN 80-Jan-01 00:00 ereg/functional.py
 -rw-r--r--  2.0 unx    33997 b- defN 80-Jan-01 00:00 ereg/registration.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ereg/utils/__init__.py
 -rw-r--r--  2.0 unx      793 b- defN 80-Jan-01 00:00 ereg/utils/citation_reminder.py
 -rw-r--r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 ereg/utils/io.py
 -rw-r--r--  2.0 unx      866 b- defN 80-Jan-01 00:00 ereg/utils/metrics.py
--rw-r--r--  2.0 unx    11356 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     5874 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 ereg-0.0.8.dist-info/RECORD
-16 files, 68582 bytes uncompressed, 18633 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx    11356 b- defN 80-Jan-01 00:00 ereg-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6421 b- defN 80-Jan-01 00:00 ereg-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ereg-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 ereg-0.0.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 ereg-0.0.9.dist-info/RECORD
+16 files, 69129 bytes uncompressed, 18827 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: ereg/utils/io.py
 Comment: 
 
 Filename: ereg/utils/metrics.py
 Comment: 
 
-Filename: ereg-0.0.8.dist-info/LICENSE
+Filename: ereg-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: ereg-0.0.8.dist-info/METADATA
+Filename: ereg-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: ereg-0.0.8.dist-info/WHEEL
+Filename: ereg-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: ereg-0.0.8.dist-info/entry_points.txt
+Filename: ereg-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ereg-0.0.8.dist-info/RECORD
+Filename: ereg-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ereg-0.0.8.dist-info/LICENSE` & `ereg-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ereg-0.0.8.dist-info/METADATA` & `ereg-0.0.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eReg
-Version: 0.0.8
+Version: 0.0.9
 Summary: efficient, pythonic cross-platform image registrations
 Home-page: https://github.com/BrainLesion/eReg
 Author: Sarthak Pati
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,21 +17,25 @@
 Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Documentation, https://eReg.readthedocs.io/
 Project-URL: Repository, https://github.com/BrainLesion/eReg
 Description-Content-Type: text/markdown
 
+[![PyPI version preprocessing](https://badge.fury.io/py/eReg.svg)](https://pypi.python.org/pypi/eReg/)
+[![Documentation Status](https://readthedocs.org/projects/ereg/badge/?version=latest)](http://ereg.readthedocs.io/?badge=latest)
+[![tests](https://github.com/BrainLesion/eReg/actions/workflows/tests.yml/badge.svg)](https://github.com/BrainLesion/eReg/actions/workflows/tests.yml)
+
 # eReg - A Simple Registration Tool
+**eReg** is a robust, fast and user-friendly registration tool that can be used in clinical environments without the need for virtualization or containerization technologies. It supports most platforms across various hardware configurations.
 
 ## Need
-
 Because of security concerns, users in clinical environments do not have access to virtualization and containerization technologies such as Docker and Singularity. This becomes a problem, because most research code (especially for image registration) is built around the need to have access to these technologies. Alternatively, some tools only work on a Linux environment, or they need specific hardware resources (such as a DL accelerator card), which are not always available in clinical settings.
 
-**eReg** is a simple registration tool that can be used in clinical environments without the need for virtualization or containerization technologies. It supports most platforms across various hardware configurations.
+
 
 ## Installation
 
 With a Python 3.8+ environment, you can install **eReg** from [pypi.org](https://pypi.org/project/eReg/).
 
 1. Create a virtual environment
 
@@ -75,15 +79,15 @@
   -c , --config        The configuration file to use.
   -tff , --transfile   Registration transform file; if provided, will use this transform instead of computing a new one or will save. Defaults to None.
   -lf , --log_file     The log file to write to. Defaults to None.
   -gt , --gt           The ground truth image.
 ```
 
 ### Pythonic Interface
-The `ereg` package provides two Python interfaces, an object-oriented interface, as well as convenience functions.
+The `ereg` package provides two Python interfaces, an object-oriented interface, as well as convenience functions. A [Jupyter notebook tutorial](https://github.com/BrainLesion/tutorials/tree/main/eReg) is available to illustrate usage of the Python API.
 
 #### Object-Oriented Interface
 
 The `register` method represents the core-of the object-oriented interface:
 
 ```python
 from ereg.registration import RegistrationClass
```

## Comparing `ereg-0.0.8.dist-info/RECORD` & `ereg-0.0.9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 ereg/configurations/sample_config.yaml,sha256=v_KqDOlNjmzqcaO5rfv8sM9cP_4upjwU2wY89nmq7ck,3600
 ereg/functional.py,sha256=VO2WYCc1-cQ9d17t8hF3t0wrJvsirWszBtEsFBW8fCM,1575
 ereg/registration.py,sha256=VvcldvSzemBlwB4PIkCMxQoCtg7TQF2NT99eNyQTo08,33997
 ereg/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ereg/utils/citation_reminder.py,sha256=JV1Ey0StYPCnsBpPx4yXSCfbnaAK2kxI1gLlHLNZ5Bs,793
 ereg/utils/io.py,sha256=946FhtfQJaF_5uziQ-FrEYUW5-WpaH6FGgV6FeYrEzU,1296
 ereg/utils/metrics.py,sha256=HzUctS0r_Tv7bdSo_7nhFiam0adWCsNpX_1yjibHhzo,866
-ereg-0.0.8.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-ereg-0.0.8.dist-info/METADATA,sha256=fKGdr2dAfb_tNAw9IUrZVlwBPBDG6f4BrcqcnCLAJGo,5874
-ereg-0.0.8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-ereg-0.0.8.dist-info/entry_points.txt,sha256=1W3fHbgIIvRc178p2ovIAzyoURXHluISleo29PEHcsw,69
-ereg-0.0.8.dist-info/RECORD,,
+ereg-0.0.9.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+ereg-0.0.9.dist-info/METADATA,sha256=FepkG-Jb18vmECoFiSduYtj9JL152R1tX8cLOP37wLs,6421
+ereg-0.0.9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+ereg-0.0.9.dist-info/entry_points.txt,sha256=1W3fHbgIIvRc178p2ovIAzyoURXHluISleo29PEHcsw,69
+ereg-0.0.9.dist-info/RECORD,,
```

