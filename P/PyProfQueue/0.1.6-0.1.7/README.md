# Comparing `tmp/PyProfQueue-0.1.6.tar.gz` & `tmp/PyProfQueue-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.6.tar", last modified: Fri Apr 12 13:25:49 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.7.tar", last modified: Mon Apr 15 10:54:41 2024, max compression
```

## Comparing `PyProfQueue-0.1.6.tar` & `PyProfQueue-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 13:25:49.798168 PyProfQueue-0.1.6/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-12 13:25:49.798168 PyProfQueue-0.1.6/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 13:25:49.798168 PyProfQueue-0.1.6/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.6/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 13:25:49.798168 PyProfQueue-0.1.6/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.6/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      811 2024-04-10 13:27:21.000000 PyProfQueue-0.1.6/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5801 2024-04-12 10:47:29.000000 PyProfQueue-0.1.6/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    37555 2024-04-12 13:00:53.000000 PyProfQueue-0.1.6/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.6/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 13:25:49.798168 PyProfQueue-0.1.6/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-12 13:25:49.000000 PyProfQueue-0.1.6/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-12 13:25:49.000000 PyProfQueue-0.1.6/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-12 13:25:49.000000 PyProfQueue-0.1.6/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-12 13:25:49.000000 PyProfQueue-0.1.6/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-12 13:25:49.000000 PyProfQueue-0.1.6/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4689 2024-04-11 12:23:42.000000 PyProfQueue-0.1.6/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-12 13:25:49.798168 PyProfQueue-0.1.6/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-12 12:59:36.000000 PyProfQueue-0.1.6/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.194335 PyProfQueue-0.1.7/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.7/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.7/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      811 2024-04-10 13:27:21.000000 PyProfQueue-0.1.7/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5801 2024-04-12 10:47:29.000000 PyProfQueue-0.1.7/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    37533 2024-04-15 10:52:27.000000 PyProfQueue-0.1.7/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.7/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4689 2024-04-11 12:23:42.000000 PyProfQueue-0.1.7/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-15 10:54:32.000000 PyProfQueue-0.1.7/setup.py
```

### Comparing `PyProfQueue-0.1.6/PKG-INFO` & `PyProfQueue-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1.6/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.7/PyProfQueue/data/likwid_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.6/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.1.7/PyProfQueue/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.6/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.1.7/PyProfQueue/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.6/PyProfQueue/script.py` & `PyProfQueue-0.1.7/PyProfQueue/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,16 +759,15 @@
             if self.queue_system is not None:
                 self.add_options(profilefile)
 
             profilefile.write('export WORKING_DIR={}\n'.format(self.work_dir))
             profilefile.write('if [ ! -d  "${WORKING_DIR}" ]; then\n')
             profilefile.write('  mkdir ${WORKING_DIR}\n')
             profilefile.write('fi\n')
-            if self.queue_system is None:
-                profilefile.write('cd ${WORKING_DIR}\n')
+            profilefile.write('cd ${WORKING_DIR}\n')
             profilefile.write('\n')
 
             if self.likwid:
                 self.init_likwid(profilefile)
 
             if self.prometheus:
                 self.init_prometheus(profilefile)
@@ -786,15 +785,15 @@
 
         return
 
     def add_options(self, profilefile):
         to_write = [a for a in dir(self.obj_options) if not a.startswith('__') and
                     not callable(getattr(self.obj_options, a))]
         for option in to_write:
-            if option is not None:
+            if option is not None and option != 'workdir':
                 profilefile.write(self.option_start + self.option_converter(option) +
                                   self.obj_options.__getattribute__(option) + '\n')
         profilefile.write('\n')
 
     def run_work(self, profilefile, bash_options=['']):
         profilefile.write('bash {} {}\n'.format(self.tmp_work_script,
                                                 ' '.join(str(x) for x in bash_options)))
```

### Comparing `PyProfQueue-0.1.6/PyProfQueue/submission.py` & `PyProfQueue-0.1.7/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.6/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.1.7/PyProfQueue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1.6/ReadMe.md` & `PyProfQueue-0.1.7/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.6/setup.py` & `PyProfQueue-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.6',
+    version='0.1.7',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

