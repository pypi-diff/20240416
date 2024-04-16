# Comparing `tmp/PyProfQueue-0.1.8.tar.gz` & `tmp/PyProfQueue-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.8.tar", last modified: Tue Apr 16 09:35:01 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.9.tar", last modified: Tue Apr 16 10:31:23 2024, max compression
```

## Comparing `PyProfQueue-0.1.8.tar` & `PyProfQueue-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.8/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.8/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      864 2024-04-16 09:23:13.000000 PyProfQueue-0.1.8/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5627 2024-04-16 09:23:45.000000 PyProfQueue-0.1.8/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    39120 2024-04-16 08:37:35.000000 PyProfQueue-0.1.8/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.8/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4689 2024-04-11 12:23:42.000000 PyProfQueue-0.1.8/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-16 09:33:12.000000 PyProfQueue-0.1.8/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 10:31:23.501277 PyProfQueue-0.1.9/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5779 2024-04-16 10:31:23.501277 PyProfQueue-0.1.9/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 10:31:23.501277 PyProfQueue-0.1.9/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.9/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 10:31:23.501277 PyProfQueue-0.1.9/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.9/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      864 2024-04-16 09:23:13.000000 PyProfQueue-0.1.9/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5627 2024-04-16 09:23:45.000000 PyProfQueue-0.1.9/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    39238 2024-04-16 10:31:11.000000 PyProfQueue-0.1.9/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.9/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 10:31:23.501277 PyProfQueue-0.1.9/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5779 2024-04-16 10:31:23.000000 PyProfQueue-0.1.9/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-16 10:31:23.000000 PyProfQueue-0.1.9/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-16 10:31:23.000000 PyProfQueue-0.1.9/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-16 10:31:23.000000 PyProfQueue-0.1.9/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-16 10:31:23.000000 PyProfQueue-0.1.9/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5079 2024-04-16 10:31:11.000000 PyProfQueue-0.1.9/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-16 10:31:23.501277 PyProfQueue-0.1.9/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-16 10:31:11.000000 PyProfQueue-0.1.9/setup.py
```

### Comparing `PyProfQueue-0.1.8/PKG-INFO` & `PyProfQueue-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -27,43 +27,47 @@
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
                             likwid: bool = False,
                             likwid_req: list = None,
                             prometheus: bool = False,
+                            prometheus_ip: str = None, 
                             prometheus_req: list = None
                             )   
 ```
 - queue_system: The intended target queue system
 - work_script: The bash script which contains the queue options and work to be done
 - read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
 if different from queue_system
 - queue_options(Optional): Any queue options to add or override when compared to the work_script 
 - likwid (Optional: defaults to False): Bool to determine if likwid should be used
 - likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
 - prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
+- prometheus_ip (Optional: defaults to None): IP address of pre-existing Prometheus instance, not providing an 
+address will default to launching prometheus with the address 'http://localhost:9090'
 - prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
 
 The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
   - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
   - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
   - likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 For example, loading the likwid module:
 ```
 likwid_req = ['module load likwid']
 ```
-- **add_prometheus**(prometheus_req: list, prometheus_output: str ='./')
+- **add_prometheus**(prometheus_req: list, prometheus_ip: str ='./')
   - Adds necessary initiation to use measure computing resource usage
   - This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
   - prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
 prometheus.
-It is necessary to at least add the following entry:
+  - prometheus_ip is a string which is the ip-address of a pre-existing prometheus instance, if it exists.
+It is necessary to at least add the following entry unless prometheus_ip is provided:
 ``` 
 prometheus_req = [
     'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
 ]
 ```
 
 - **change_options**(queue_options: dict)
```

### Comparing `PyProfQueue-0.1.8/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.9/PyProfQueue/data/likwid_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.8/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.1.9/PyProfQueue/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.8/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.1.9/PyProfQueue/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.8/PyProfQueue/script.py` & `PyProfQueue-0.1.9/PyProfQueue/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,17 +181,19 @@
 
     def add_likwid(self, likwid_req):
         self.likwid = True
         self.likwid_file = impresources.files(data) / "likwid_commands.txt"
         self.likwid_initEndSplit = -1
         self.likwid_req = likwid_req
 
-    def add_prometheus(self, prometheus_req):
+    def add_prometheus(self, prometheus_req: list, prometheus_ip: str = None):
         contains_ps = False
         contains_pp = False
+        if prometheus_ip is not None:
+            self.prometheus_ip = prometheus_ip
         if prometheus_req is not None:
             for req in prometheus_req:
                 if 'PROMETHEUS_SOFTWARE' in req:
                     contains_ps = True
                     continue
                 if 'PROMETHEUS_PYTHON' in req:
                     contains_pp = True
```

### Comparing `PyProfQueue-0.1.8/PyProfQueue/submission.py` & `PyProfQueue-0.1.9/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.8/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.1.9/PyProfQueue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -27,43 +27,47 @@
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
                             likwid: bool = False,
                             likwid_req: list = None,
                             prometheus: bool = False,
+                            prometheus_ip: str = None, 
                             prometheus_req: list = None
                             )   
 ```
 - queue_system: The intended target queue system
 - work_script: The bash script which contains the queue options and work to be done
 - read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
 if different from queue_system
 - queue_options(Optional): Any queue options to add or override when compared to the work_script 
 - likwid (Optional: defaults to False): Bool to determine if likwid should be used
 - likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
 - prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
+- prometheus_ip (Optional: defaults to None): IP address of pre-existing Prometheus instance, not providing an 
+address will default to launching prometheus with the address 'http://localhost:9090'
 - prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
 
 The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
   - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
   - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
   - likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 For example, loading the likwid module:
 ```
 likwid_req = ['module load likwid']
 ```
-- **add_prometheus**(prometheus_req: list, prometheus_output: str ='./')
+- **add_prometheus**(prometheus_req: list, prometheus_ip: str ='./')
   - Adds necessary initiation to use measure computing resource usage
   - This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
   - prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
 prometheus.
-It is necessary to at least add the following entry:
+  - prometheus_ip is a string which is the ip-address of a pre-existing prometheus instance, if it exists.
+It is necessary to at least add the following entry unless prometheus_ip is provided:
 ``` 
 prometheus_req = [
     'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
 ]
 ```
 
 - **change_options**(queue_options: dict)
```

### Comparing `PyProfQueue-0.1.8/ReadMe.md` & `PyProfQueue-0.1.9/ReadMe.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,43 +8,47 @@
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
                             likwid: bool = False,
                             likwid_req: list = None,
                             prometheus: bool = False,
+                            prometheus_ip: str = None, 
                             prometheus_req: list = None
                             )   
 ```
 - queue_system: The intended target queue system
 - work_script: The bash script which contains the queue options and work to be done
 - read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
 if different from queue_system
 - queue_options(Optional): Any queue options to add or override when compared to the work_script 
 - likwid (Optional: defaults to False): Bool to determine if likwid should be used
 - likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
 - prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
+- prometheus_ip (Optional: defaults to None): IP address of pre-existing Prometheus instance, not providing an 
+address will default to launching prometheus with the address 'http://localhost:9090'
 - prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
 
 The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
   - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
   - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
   - likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 For example, loading the likwid module:
 ```
 likwid_req = ['module load likwid']
 ```
-- **add_prometheus**(prometheus_req: list, prometheus_output: str ='./')
+- **add_prometheus**(prometheus_req: list, prometheus_ip: str ='./')
   - Adds necessary initiation to use measure computing resource usage
   - This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
   - prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
 prometheus.
-It is necessary to at least add the following entry:
+  - prometheus_ip is a string which is the ip-address of a pre-existing prometheus instance, if it exists.
+It is necessary to at least add the following entry unless prometheus_ip is provided:
 ``` 
 prometheus_req = [
     'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
 ]
 ```
 
 - **change_options**(queue_options: dict)
```

### Comparing `PyProfQueue-0.1.8/setup.py` & `PyProfQueue-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.8',
+    version='0.1.9',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

