# Comparing `tmp/cs2solutions-0.6.2.tar.gz` & `tmp/cs2solutions-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2solutions-0.6.2.tar", last modified: Mon Apr 15 20:00:15 2024, max compression
+gzip compressed data, was "cs2solutions-0.6.3.tar", last modified: Mon Apr 15 20:04:28 2024, max compression
```

## Comparing `cs2solutions-0.6.2.tar` & `cs2solutions-0.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 20:00:15.742913 cs2solutions-0.6.2/
--rw-rw-rw-   0        0        0    35823 2024-02-17 10:04:18.000000 cs2solutions-0.6.2/LICENSE
--rw-rw-rw-   0        0        0    42995 2024-04-15 20:00:15.741948 cs2solutions-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      727 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/README.md
--rw-rw-rw-   0        0        0     1265 2024-04-15 20:00:09.000000 cs2solutions-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 20:00:15.742913 cs2solutions-0.6.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 20:00:15.715517 cs2solutions-0.6.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:00:15.728956 cs2solutions-0.6.2/src/cs2solutions/
--rw-rw-rw-   0        0        0      141 2024-04-15 19:58:24.000000 cs2solutions-0.6.2/src/cs2solutions/__init__.py
--rw-rw-rw-   0        0        0     7065 2024-03-10 22:19:53.000000 cs2solutions-0.6.2/src/cs2solutions/aircraft.py
--rw-rw-rw-   0        0        0        0 2024-03-16 10:08:22.000000 cs2solutions-0.6.2/src/cs2solutions/cs.py
--rw-rw-rw-   0        0        0     6142 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/src/cs2solutions/cs2bot.py
--rw-rw-rw-   0        0        0    11149 2024-03-16 10:15:26.000000 cs2solutions-0.6.2/src/cs2solutions/decomp.py
--rw-rw-rw-   0        0        0    21713 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/src/cs2solutions/discretization.py
--rw-rw-rw-   0        0        0     8843 2024-03-16 10:12:07.000000 cs2solutions-0.6.2/src/cs2solutions/duckiebot.py
--rw-rw-rw-   0        0        0     7967 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/src/cs2solutions/intro.py
--rw-rw-rw-   0        0        0    13919 2024-04-15 19:59:56.000000 cs2solutions-0.6.2/src/cs2solutions/intromimo.py
--rw-rw-rw-   0        0        0    11049 2024-03-16 10:11:41.000000 cs2solutions-0.6.2/src/cs2solutions/lqrfeedback.py
--rw-rw-rw-   0        0        0    13739 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/src/cs2solutions/morse.py
--rw-rw-rw-   0        0        0       93 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/src/cs2solutions/plot.py
--rw-rw-rw-   0        0        0       68 2024-02-21 18:21:30.000000 cs2solutions-0.6.2/src/cs2solutions/test.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:00:15.740949 cs2solutions-0.6.2/src/cs2solutions.egg-info/
--rw-rw-rw-   0        0        0    42995 2024-04-15 20:00:15.000000 cs2solutions-0.6.2/src/cs2solutions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2024-04-15 20:00:15.000000 cs2solutions-0.6.2/src/cs2solutions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 20:00:15.000000 cs2solutions-0.6.2/src/cs2solutions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-15 20:00:15.000000 cs2solutions-0.6.2/src/cs2solutions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-15 20:00:15.000000 cs2solutions-0.6.2/src/cs2solutions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 20:04:28.201442 cs2solutions-0.6.3/
+-rw-rw-rw-   0        0        0    35823 2024-02-17 10:04:18.000000 cs2solutions-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0    42995 2024-04-15 20:04:28.200442 cs2solutions-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/README.md
+-rw-rw-rw-   0        0        0     1265 2024-04-15 20:04:16.000000 cs2solutions-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 20:04:28.201442 cs2solutions-0.6.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 20:04:28.179616 cs2solutions-0.6.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:04:28.187616 cs2solutions-0.6.3/src/cs2solutions/
+-rw-rw-rw-   0        0        0      141 2024-04-15 19:58:24.000000 cs2solutions-0.6.3/src/cs2solutions/__init__.py
+-rw-rw-rw-   0        0        0     7065 2024-03-10 22:19:53.000000 cs2solutions-0.6.3/src/cs2solutions/aircraft.py
+-rw-rw-rw-   0        0        0        0 2024-03-16 10:08:22.000000 cs2solutions-0.6.3/src/cs2solutions/cs.py
+-rw-rw-rw-   0        0        0     6142 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/src/cs2solutions/cs2bot.py
+-rw-rw-rw-   0        0        0    11149 2024-03-16 10:15:26.000000 cs2solutions-0.6.3/src/cs2solutions/decomp.py
+-rw-rw-rw-   0        0        0    21713 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/src/cs2solutions/discretization.py
+-rw-rw-rw-   0        0        0     8843 2024-03-16 10:12:07.000000 cs2solutions-0.6.3/src/cs2solutions/duckiebot.py
+-rw-rw-rw-   0        0        0     7967 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/src/cs2solutions/intro.py
+-rw-rw-rw-   0        0        0    13919 2024-04-15 19:59:56.000000 cs2solutions-0.6.3/src/cs2solutions/intromimo.py
+-rw-rw-rw-   0        0        0    11049 2024-03-16 10:11:41.000000 cs2solutions-0.6.3/src/cs2solutions/lqrfeedback.py
+-rw-rw-rw-   0        0        0    13739 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/src/cs2solutions/morse.py
+-rw-rw-rw-   0        0        0       93 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/src/cs2solutions/plot.py
+-rw-rw-rw-   0        0        0       68 2024-02-21 18:21:30.000000 cs2solutions-0.6.3/src/cs2solutions/test.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:04:28.199442 cs2solutions-0.6.3/src/cs2solutions.egg-info/
+-rw-rw-rw-   0        0        0    42995 2024-04-15 20:04:28.000000 cs2solutions-0.6.3/src/cs2solutions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2024-04-15 20:04:28.000000 cs2solutions-0.6.3/src/cs2solutions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 20:04:28.000000 cs2solutions-0.6.3/src/cs2solutions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-15 20:04:28.000000 cs2solutions-0.6.3/src/cs2solutions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 20:04:28.000000 cs2solutions-0.6.3/src/cs2solutions.egg-info/top_level.txt
```

### Comparing `cs2solutions-0.6.2/LICENSE` & `cs2solutions-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/PKG-INFO` & `cs2solutions-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.6.2
+Version: 0.6.3
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `cs2solutions-0.6.2/README.md` & `cs2solutions-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/pyproject.toml` & `cs2solutions-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/solutions"]
 
 [project]
 name = "cs2solutions"
-version = "0.6.2"
+version = "0.6.3"
 dependencies =[
     "control",
     "matplotlib",
     "numpy",
     "scipy"
 ]
 requires-python = ">=3.9"
```

### Comparing `cs2solutions-0.6.2/src/cs2solutions/aircraft.py` & `cs2solutions-0.6.3/src/cs2solutions/aircraft.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/cs2bot.py` & `cs2solutions-0.6.3/src/cs2solutions/cs2bot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/decomp.py` & `cs2solutions-0.6.3/src/cs2solutions/decomp.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/discretization.py` & `cs2solutions-0.6.3/src/cs2solutions/discretization.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/duckiebot.py` & `cs2solutions-0.6.3/src/cs2solutions/duckiebot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/intro.py` & `cs2solutions-0.6.3/src/cs2solutions/intro.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/intromimo.py` & `cs2solutions-0.6.3/src/cs2solutions/intromimo.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/lqrfeedback.py` & `cs2solutions-0.6.3/src/cs2solutions/lqrfeedback.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions/morse.py` & `cs2solutions-0.6.3/src/cs2solutions/morse.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.2/src/cs2solutions.egg-info/PKG-INFO` & `cs2solutions-0.6.3/src/cs2solutions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.6.2
+Version: 0.6.3
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `cs2solutions-0.6.2/src/cs2solutions.egg-info/SOURCES.txt` & `cs2solutions-0.6.3/src/cs2solutions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

