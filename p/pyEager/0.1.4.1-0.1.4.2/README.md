# Comparing `tmp/pyEager-0.1.4.1.tar.gz` & `tmp/pyEager-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEager-0.1.4.1.tar", last modified: Wed Sep  6 14:31:54 2023, max compression
+gzip compressed data, was "pyEager-0.1.4.2.tar", last modified: Tue Apr 16 16:10:03 2024, max compression
```

## Comparing `pyEager-0.1.4.1.tar` & `pyEager-0.1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-09-06 14:31:54.457104 pyEager-0.1.4.1/
--rw-r--r--   0 lamnidis   (506) staff       (20)     1071 2023-08-02 14:15:47.000000 pyEager-0.1.4.1/LICENSE.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)     2909 2023-09-06 14:31:54.457253 pyEager-0.1.4.1/PKG-INFO
--rw-r--r--   0 lamnidis   (506) staff       (20)     2018 2023-09-06 14:15:20.000000 pyEager-0.1.4.1/README.md
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-09-06 14:31:54.455683 pyEager-0.1.4.1/pyEager/
--rw-r--r--   0 lamnidis   (506) staff       (20)      446 2023-09-06 14:29:19.000000 pyEager-0.1.4.1/pyEager/__init__.py
--rw-r--r--   0 lamnidis   (506) staff       (20)    10314 2023-09-06 14:08:40.000000 pyEager-0.1.4.1/pyEager/parsers.py
--rw-r--r--   0 lamnidis   (506) staff       (20)     2929 2023-08-03 12:59:09.000000 pyEager-0.1.4.1/pyEager/wrappers.py
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-09-06 14:31:54.456912 pyEager-0.1.4.1/pyEager.egg-info/
--rw-r--r--   0 lamnidis   (506) staff       (20)     2909 2023-09-06 14:31:53.000000 pyEager-0.1.4.1/pyEager.egg-info/PKG-INFO
--rw-r--r--   0 lamnidis   (506) staff       (20)      253 2023-09-06 14:31:54.000000 pyEager-0.1.4.1/pyEager.egg-info/SOURCES.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        1 2023-09-06 14:31:54.000000 pyEager-0.1.4.1/pyEager.egg-info/dependency_links.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        7 2023-09-06 14:31:54.000000 pyEager-0.1.4.1/pyEager.egg-info/requires.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        8 2023-09-06 14:31:54.000000 pyEager-0.1.4.1/pyEager.egg-info/top_level.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)       79 2023-09-06 14:31:54.457721 pyEager-0.1.4.1/setup.cfg
--rw-r--r--   0 lamnidis   (506) staff       (20)     1249 2023-09-06 14:29:26.000000 pyEager-0.1.4.1/setup.py
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2024-04-16 16:10:03.754480 pyEager-0.1.4.2/
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1071 2023-08-02 14:15:47.000000 pyEager-0.1.4.2/LICENSE.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2912 2024-04-16 16:10:03.754273 pyEager-0.1.4.2/PKG-INFO
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2018 2023-09-06 14:15:20.000000 pyEager-0.1.4.2/README.md
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2024-04-16 16:10:03.751410 pyEager-0.1.4.2/pyEager/
+-rw-r--r--   0 lamnidis   (506) staff       (20)      446 2023-09-06 14:29:19.000000 pyEager-0.1.4.2/pyEager/__init__.py
+-rw-r--r--   0 lamnidis   (506) staff       (20)    10368 2024-04-16 16:08:54.000000 pyEager-0.1.4.2/pyEager/parsers.py
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2929 2023-08-03 12:59:09.000000 pyEager-0.1.4.2/pyEager/wrappers.py
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2024-04-16 16:10:03.753726 pyEager-0.1.4.2/pyEager.egg-info/
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2912 2024-04-16 16:10:03.000000 pyEager-0.1.4.2/pyEager.egg-info/PKG-INFO
+-rw-r--r--   0 lamnidis   (506) staff       (20)      253 2024-04-16 16:10:03.000000 pyEager-0.1.4.2/pyEager.egg-info/SOURCES.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        1 2024-04-16 16:10:03.000000 pyEager-0.1.4.2/pyEager.egg-info/dependency_links.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        7 2024-04-16 16:10:03.000000 pyEager-0.1.4.2/pyEager.egg-info/requires.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        8 2024-04-16 16:10:03.000000 pyEager-0.1.4.2/pyEager.egg-info/top_level.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)       79 2024-04-16 16:10:03.755118 pyEager-0.1.4.2/setup.cfg
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1249 2024-04-16 16:09:59.000000 pyEager-0.1.4.2/setup.py
```

### Comparing `pyEager-0.1.4.1/LICENSE.txt` & `pyEager-0.1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.4.1/PKG-INFO` & `pyEager-0.1.4.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyEager
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: A simple package to read in eager results.
 Home-page: https://github.com/TCLamnidis/pyEager
-Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.4.1.tar.gz
+Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.4.2.tar.gz
 Author: Thiseas C. Lamnidis
 Author-email: thisseass@gmail.com
 License: MIT
 Keywords: python,pandas,nf-core,eager,nf-core/eager,ancient DNA
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 License-File: LICENSE.txt
+Requires-Dist: pandas
 
 # pyEager
 
 A simple package to read in eager results.
 
 ## Available functions
 
@@ -47,8 +47,7 @@
 ## Usage
 
 <!-- TODO Add usage examples -->
 
 ## License
 
 [MIT](LICENSE.txt)
-
```

### Comparing `pyEager-0.1.4.1/README.md` & `pyEager-0.1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.4.1/pyEager/parsers.py` & `pyEager-0.1.4.2/pyEager/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,16 +251,18 @@
             return row["initial_bam_name"]
         ## Additional merge
         elif row["additional_merge"]:
             return f"{row['Sample_Name']}_libmerged_add.bam"
 
     ## Get sex determination BAM name
     def sexdet_bam_name(row):
-        return row["additional_bam_name"].replace(
-            ".bam", f"_{row['Strandedness']}strand.bam"
+        return (
+            row["additional_bam_name"]
+            .replace(".bam", f"_{row['Strandedness']}strand.bam")
+            .replace("_udgnone_", "_")
         )
 
     ## Add columns with inferred BAM names
     tsv_data["initial_bam_name"] = tsv_data.apply(
         initial_bam_name, axis=1, run_trim_bam=run_trim_bam
     )
     tsv_data["additional_bam_name"] = tsv_data.apply(additional_bam_name, axis=1)
```

### Comparing `pyEager-0.1.4.1/pyEager/wrappers.py` & `pyEager-0.1.4.2/pyEager/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.4.1/pyEager.egg-info/PKG-INFO` & `pyEager-0.1.4.2/pyEager.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyEager
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: A simple package to read in eager results.
 Home-page: https://github.com/TCLamnidis/pyEager
-Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.4.1.tar.gz
+Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.4.2.tar.gz
 Author: Thiseas C. Lamnidis
 Author-email: thisseass@gmail.com
 License: MIT
 Keywords: python,pandas,nf-core,eager,nf-core/eager,ancient DNA
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 License-File: LICENSE.txt
+Requires-Dist: pandas
 
 # pyEager
 
 A simple package to read in eager results.
 
 ## Available functions
 
@@ -47,8 +47,7 @@
 ## Usage
 
 <!-- TODO Add usage examples -->
 
 ## License
 
 [MIT](LICENSE.txt)
-
```

### Comparing `pyEager-0.1.4.1/setup.py` & `pyEager-0.1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from distutils.core import setup
 
-VERSION = "0.1.4.1"
+VERSION = "0.1.4.2"
 setup(
     name="pyEager",
     packages=["pyEager"],
     version=VERSION,
     license="MIT",
     description="A simple package to read in eager results.",
     long_description=open("README.md").read(),
```

