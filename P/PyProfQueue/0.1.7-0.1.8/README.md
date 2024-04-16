# Comparing `tmp/PyProfQueue-0.1.7.tar.gz` & `tmp/PyProfQueue-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.7.tar", last modified: Mon Apr 15 10:54:41 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.8.tar", last modified: Tue Apr 16 09:35:01 2024, max compression
```

## Comparing `PyProfQueue-0.1.7.tar` & `PyProfQueue-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.194335 PyProfQueue-0.1.7/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.7/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.7/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      811 2024-04-10 13:27:21.000000 PyProfQueue-0.1.7/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5801 2024-04-12 10:47:29.000000 PyProfQueue-0.1.7/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    37533 2024-04-15 10:52:27.000000 PyProfQueue-0.1.7/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.7/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-15 10:54:41.000000 PyProfQueue-0.1.7/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4689 2024-04-11 12:23:42.000000 PyProfQueue-0.1.7/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-15 10:54:41.198335 PyProfQueue-0.1.7/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-15 10:54:32.000000 PyProfQueue-0.1.7/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.8/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.8/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      864 2024-04-16 09:23:13.000000 PyProfQueue-0.1.8/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5627 2024-04-16 09:23:45.000000 PyProfQueue-0.1.8/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    39120 2024-04-16 08:37:35.000000 PyProfQueue-0.1.8/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.8/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-16 09:35:01.000000 PyProfQueue-0.1.8/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4689 2024-04-11 12:23:42.000000 PyProfQueue-0.1.8/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-16 09:35:01.061648 PyProfQueue-0.1.8/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-16 09:33:12.000000 PyProfQueue-0.1.8/setup.py
```

### Comparing `PyProfQueue-0.1.7/PKG-INFO` & `PyProfQueue-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1.7/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.8/PyProfQueue/data/likwid_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.7/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.1.8/PyProfQueue/data/prometheus_commands.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 mkdir ${PROMETHEUS_RUNNING_DIR}
-
+# *=*
 ${PROMETHEUS_SOFTWARE}/node_exporter/node_exporter > /dev/null 2>&1 &
 export NODE_PID=$!
 ${PROMETHEUS_SOFTWARE}/prometheus --config.file=${PROMETHEUS_SOFTWARE}/prometheus.yml --storage.tsdb.path=${PROMETHEUS_RUNNING_DIR}/data > /dev/null 2>&1 &
 export PROMETHEUS_PID=$!
-
+# *=*
 export START_TIME=$(date +%s)
 sleep 15
 # *=*
 sleep 15
 export END_TIME=$(date +%s)
 export DURATION=$((${END_TIME} - ${START_TIME}))
 export START=$(date -d @${START_TIME} -u +"%Y-%m-%d %H:%M:%S")
 export END=$(date -d @${END_TIME} -u +"%Y-%m-%d %H:%M:%S")
-${PROMETHEUS_PYTHON} ${PROFILE_SCRAPE}/read_prometheus.py "${START}" "${END}" "${PROMETHEUS_RUNNING_DIR}"
+${PROMETHEUS_PYTHON} ${PROFILE_SCRAPE}/read_prometheus.py -o "${PROMETHEUS_RUNNING_DIR}" -s "${START}" -e "${END}" -i "${PROMETHEUS_IP}"
+# *=*
 sleep 1
 kill -TERM ${NODE_PID}
 kill -TERM ${PROMETHEUS_PID}
+# *=*
 echo 'Run time: '$((${DURATION}/60/60))':'$((${DURATION}/60%60 ))':'$((${DURATION}%60))
```

### Comparing `PyProfQueue-0.1.7/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.1.8/PyProfQueue/data/read_prometheus.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import pandas as pd
 import numpy as np
 
 parser = argparse.ArgumentParser(description="Just an example")
 parser.add_argument("-o", "--output", type=str, help="output path where data should be stored")
 parser.add_argument("-s", "--start_time", type=str, help="start time of the code")
 parser.add_argument("-e", "--end_time", type=str, help="end time of the code")
-parser.add_argument("-p", "--pre_prometheus", type=bool, default=False,
-                    help="Toggle for a Pre-Existing Prometheus instance")
 parser.add_argument("-i", "--ip_address", type=str, default="http://localhost:9090",
                     help="IP address of the Prometheus instance")
 args = parser.parse_args()
 
 
 def check_options():
     global args
@@ -46,15 +44,14 @@
 def prometheus_scrape(connection: PromqlHttpApi, command: str, begin: datetime, end: datetime,
                       given_name: str, name_convention: str = None, step: str = '10s'):
     queue_results = connection.query_range(command, start=begin, end=end, step=step)()['result']
     queue_dict = {}
     for result in queue_results:
         if name_convention is not None:
             key_name = given_name + ' ' + result['metric'][name_convention]
-            print(key_name)
         else:
             key_name = given_name
         queue_dict[key_name] = np.array([[float(x[0]), float(x[1])] for x in result['values']])
     return queue_dict
 
 
 def pandas_merge(dictionary: dict, dataframe: pd.DataFrame = None):
```

### Comparing `PyProfQueue-0.1.7/PyProfQueue/script.py` & `PyProfQueue-0.1.8/PyProfQueue/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,30 +67,30 @@
                                     queue_options={'user': 'user_name'})
     """
     def __init__(self, queue_system: str,
                  work_script: str,
                  read_queue_system: str = None,
                  queue_options: dict = None,
                  likwid: bool = False, likwid_req: list = None,
-                 prometheus: bool = False, prometheus_req: list = None):
-        if True: # If statement added to allow for the collapse of the initiation of variables
+                 prometheus: bool = False, prometheus_ip: str = None, prometheus_req: list = None):
+        if True:  # If statement added to allow for the collapse of the initiation of variables
             self.queue_system = queue_system
             self.work_script = work_script
             self.tmp_work_script = None
             self.tmp_profile_script = None
             self.works = None
             self.work_dir = None
             self.likwid = likwid
             self.likwid_file = None
             self.likwid_initEndSplit = None
             self.likwid_req = None
             self.prometheus = prometheus
+            self.prometheus_ip = prometheus_ip
             self.prometheus_file = None
             self.prometheus_initEndSplit = None
-            self.prometheus_location = None
             self.read_queue_system = read_queue_system
 
         if self.likwid:
             self.add_likwid(likwid_req)
         if self.prometheus:
             self.add_prometheus(prometheus_req)
 
@@ -184,30 +184,31 @@
         self.likwid_file = impresources.files(data) / "likwid_commands.txt"
         self.likwid_initEndSplit = -1
         self.likwid_req = likwid_req
 
     def add_prometheus(self, prometheus_req):
         contains_ps = False
         contains_pp = False
-        for req in prometheus_req:
-            if 'PROMETHEUS_SOFTWARE' in req:
-                contains_ps = True
-                continue
-            if 'PROMETHEUS_PYTHON' in req:
-                contains_pp = True
-                continue
-            else:
-                prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
-                contains_pp = True
-                continue
+        if prometheus_req is not None:
+            for req in prometheus_req:
+                if 'PROMETHEUS_SOFTWARE' in req:
+                    contains_ps = True
+                    continue
+                if 'PROMETHEUS_PYTHON' in req:
+                    contains_pp = True
+                    continue
+                else:
+                    prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
+                    contains_pp = True
+                    continue
+        else:
+            prometheus_req = []
         if not contains_pp:
             prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
-            contains_pp = True
-
-        if not contains_ps or not contains_pp:
+        if not contains_ps and self.prometheus_ip is None:
             exit('When requesting prometheus profiling, prometheus_req must include "export PROMETHEUS_SOFTWARE=".')
         self.prometheus = True
         self.prometheus_file = impresources.files(data) / "prometheus_commands.txt"
         self.prometheus_initEndSplit = -1
         self.prometheus_req = prometheus_req
 
     def option_pass(self):
@@ -829,30 +830,65 @@
                 profilefile.write(line)
         profilefile.write('# Likwid final steps done\n')
         profilefile.write('\n')
         return
 
     def init_prometheus(self, profilefile):
         profilefile.write('# Prometheus initialisation declarations\n')
+        if self.prometheus_ip is None:
+            profilefile.write("export PROMETHEUS_IP=http://localhost:9090\n")
+        else:
+            profilefile.write("export PROMETHEUS_IP={}\n".format(self.prometheus_ip))
         for i in self.prometheus_req:
             profilefile.write(i)
             profilefile.write('\n')
         profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
         scrape_path = str(impresources.path(data, 'read_prometheus.py'))[:-19]
         profilefile.write('export PROFILE_SCRAPE={}\n'.format(scrape_path))
         profilefile.write('\n')
+        final_init_indicator = 2
+        if self.prometheus_ip is None:
+            read_indicators = [0, 1, 2]
+        else:
+            read_indicators = [0, 2]
+        indicator = 0
         with open(self.prometheus_file, 'r') as prometheus_file:
             for number, line in enumerate(prometheus_file):
-                if line == '# *=*\n':
+                if line == '# *=*\n' and indicator >= final_init_indicator:
                     self.prometheus_initEndSplit = number + 1
                     break
-                profilefile.write(line)
+                elif line == '# *=*\n':
+                    indicator += 1
+                    continue
+                if indicator in read_indicators:
+                    profilefile.write(line)
+        print(indicator)
+        print(self.prometheus_initEndSplit)
         profilefile.write('# Prometheus initialisation done\n')
         profilefile.write('\n')
 
     def end_prometheus(self, profilefile):
         profilefile.write('# Prometheus final steps declarations\n')
+        if self.prometheus_ip is None:
+            read_indicators = [0, 1, 2]
+        else:
+            read_indicators = [0, 2]
+        indicator = 0
         with open(self.prometheus_file, 'r') as prometheus_file:
             for line in itertools.islice(prometheus_file, self.prometheus_initEndSplit, None):
-                profilefile.write(line)
+                if line == '# *=*\n':
+                    indicator += 1
+                    continue
+                if indicator in read_indicators:
+                    profilefile.write(line)
         profilefile.write('# Prometheus final steps done\n')
         profilefile.write('\n')
+
+    def existing_init_prometheus(self, profilefile):
+        profilefile.write('# Prometheus initialisation for scraping existing instance')
+        for i in self.prometheus_req:
+            profilefile.write(i)
+            profilefile.write('\n')
+        profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
+
+    def existing_end_prometheus(self, profilefile):
+        profilefile.write('# Prometheus final steps for scraping existing instance')
```

### Comparing `PyProfQueue-0.1.7/PyProfQueue/submission.py` & `PyProfQueue-0.1.8/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.7/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.1.8/PyProfQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1.7/ReadMe.md` & `PyProfQueue-0.1.8/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.7/setup.py` & `PyProfQueue-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.7',
+    version='0.1.8',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

