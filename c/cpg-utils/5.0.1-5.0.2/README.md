# Comparing `tmp/cpg-utils-5.0.1.tar.gz` & `tmp/cpg-utils-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-5.0.1.tar", last modified: Sun Apr 14 10:00:04 2024, max compression
+gzip compressed data, was "cpg-utils-5.0.2.tar", last modified: Mon Apr 15 21:48:02 2024, max compression
```

## Comparing `cpg-utils-5.0.1.tar` & `cpg-utils-5.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:00:04.535262 cpg-utils-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-14 10:00:04.535262 cpg-utils-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:00:04.531262 cpg-utils-5.0.1/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/cpg_utils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:00:04.535262 cpg-utils-5.0.1/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-14 10:00:04.000000 cpg-utils-5.0.1/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 10:00:04.000000 cpg-utils-5.0.1/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:00:04.000000 cpg-utils-5.0.1/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 10:00:04.000000 cpg-utils-5.0.1/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 10:00:04.000000 cpg-utils-5.0.1/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:00:04.535262 cpg-utils-5.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:00:04.535262 cpg-utils-5.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/test/test_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 10:00:03.000000 cpg-utils-5.0.1/test/test_doctests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 21:48:02.000000 cpg-utils-5.0.2/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:48:02.262892 cpg-utils-5.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-15 21:47:59.000000 cpg-utils-5.0.2/test/test_doctests.py
```

### Comparing `cpg-utils-5.0.1/LICENSE` & `cpg-utils-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/PKG-INFO` & `cpg-utils-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.1
+Version: 5.0.2
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.1/README.md` & `cpg-utils-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/__init__.py` & `cpg-utils-5.0.2/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/cloud.py` & `cpg-utils-5.0.2/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.2/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/config.py` & `cpg-utils-5.0.2/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/constants.py` & `cpg-utils-5.0.2/cpg_utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 
 
 CROMWELL_AUDIENCE = os.getenv('CROMWELL_AUDIENCE', DEFAULT_CROMWELL_AUDIENCE)
 CROMWELL_URL = os.getenv('CROMWELL_URL', DEFAULT_CROMWELL_URL)
 
 
-class AnsiiColors:
+class AnsiColors:
     """
     Lookup table: https://en.wikipedia.org/wiki/ANSI_escape_code#3/4_bit
     """
 
     BRIGHTMAGENTA = '\033[95m'  # Bright magenta
     BRIGHTBLUE = '\033[94m'  # Bright blue
     BRIGHTGREEN = '\033[92m'  # Bright green
```

### Comparing `cpg-utils-5.0.1/cpg_utils/cromwell.py` & `cpg-utils-5.0.2/cpg_utils/cromwell.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/cromwell_model.py` & `cpg-utils-5.0.2/cpg_utils/cromwell_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import Enum
 from textwrap import indent
 
 import datetime
 
 from tabulate import tabulate
 
-from cpg_utils.constants import AnsiiColors
+from cpg_utils.constants import AnsiColors
 
 
 class ExecutionStatus(Enum):
     preparing = 'preparing'
     starting = 'starting'
     in_progress = 'inprogress'
     running = 'running'
@@ -37,25 +37,25 @@
             ExecutionStatus.failed: '!',
             ExecutionStatus.retryablefailure: '~!',
         }
 
     @property
     def _colors(self):
         return {
-            ExecutionStatus.done: AnsiiColors.BRIGHTGREEN,
-            ExecutionStatus.succeeded: AnsiiColors.BRIGHTGREEN,
-            ExecutionStatus.failed: AnsiiColors.BRIGHTRED,
-            ExecutionStatus.retryablefailure: AnsiiColors.BRIGHTBLUE,
+            ExecutionStatus.done: AnsiColors.BRIGHTGREEN,
+            ExecutionStatus.succeeded: AnsiColors.BRIGHTGREEN,
+            ExecutionStatus.failed: AnsiColors.BRIGHTRED,
+            ExecutionStatus.retryablefailure: AnsiColors.BRIGHTBLUE,
         }
 
     def symbol(self):
         return self._symbols.get(self, '?')
 
     def color(self):
-        return self._colors.get(self, AnsiiColors.RESET)
+        return self._colors.get(self, AnsiColors.RESET)
 
     def is_finished(self):
         _finished_states = {
             ExecutionStatus.done,
             ExecutionStatus.succeeded,
             ExecutionStatus.failed,
             ExecutionStatus.retryablefailure,
@@ -292,15 +292,15 @@
         if self.attempt is not None and self.attempt > 1:
             name += f' (attempt {self.attempt})'
 
         symbol = self.executionStatus.symbol() if self.executionStatus else '?'
         color, rcol = '', ''
         if not monochrome:
             color = self.executionStatus.color() if self.executionStatus else ''
-            rcol = AnsiiColors.RESET
+            rcol = AnsiColors.RESET
 
         extras_str = "".join("\n" + indent(e, '  ') for e in extras)
         return f'{color}[{symbol}] {name} ({duration_str}){extras_str}{rcol}'
 
 
 def unwrap_caused_by(failures: list):
     inner_failures = []
@@ -325,15 +325,15 @@
         )
 
     collapsed_status = collapse_status_of_calls(calls)
     status = collapsed_status.symbol() if collapsed_status else '?'
     color, rcol = '', ''
     if not monochrome:
         color = collapsed_status.color() if collapsed_status else ''
-        rcol = AnsiiColors.RESET
+        rcol = AnsiColors.RESET
     inner_calls = ''
 
     if len(calls) > 1 and not expand_completed:
         name += f' ({len(calls)} jobs)'
 
     if len(calls) > 0:
         starts = [c.start for c in calls if c.start is not None]
```

### Comparing `cpg-utils-5.0.1/cpg_utils/dataproc.py` & `cpg-utils-5.0.2/cpg_utils/dataproc.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/git.py` & `cpg-utils-5.0.2/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/hail_batch.py` & `cpg-utils-5.0.2/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/membership.py` & `cpg-utils-5.0.2/cpg_utils/membership.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils/slack.py` & `cpg-utils-5.0.2/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.2/cpg_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.1
+Version: 5.0.2
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.1/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.2/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/pyproject.toml` & `cpg-utils-5.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/setup.py` & `cpg-utils-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='5.0.1',
+    version='5.0.2',
     description='Library of convenience functions specific to the CPG',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     package_data={
```

### Comparing `cpg-utils-5.0.1/test/test_config.py` & `cpg-utils-5.0.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.1/test/test_cromwell.py` & `cpg-utils-5.0.2/test/test_cromwell.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import unittest
 from unittest.mock import MagicMock, patch
 
 from cpg_utils.cromwell import run_cromwell_workflow
+from cpg_utils.cromwell_model import WorkflowMetadataModel
 
 
 class TestCromwellWrapper(unittest.TestCase):
 
     @patch('cpg_utils.config.get_config')
     @patch('cpg_utils.cromwell.read_secret')
     def test_workflow_options(
@@ -82,7 +83,48 @@
             wf_options['final_workflow_log_dir'],
             'test://analysis-bucket/cromwell_logs/output-prefix',
         )
         self.assertEqual(
             wf_options['final_workflow_outputs_dir'],
             'test://default-bucket/output-prefix',
         )
+
+    def test_cromwell_status_format(self):
+        """
+        Check parsing some basic cromwell metadata, and formatting it for display
+        """
+        model = WorkflowMetadataModel.parse(
+            {
+                'id': '<mocked-id>',
+                'submission': '2021-07-09T09:46:00.000Z',
+                'start': '2021-07-09T09:47:00.000Z',
+                'end': '2021-07-09T09:48:00.000Z',
+                'calls': {
+                    'wf.print': [
+                        {
+                            'name': 'print',
+                            'executionStatus': 'succeeded',
+                            'start': '2021-07-09T09:47:00.000Z',
+                            'end': '2021-07-09T09:48:00.000Z',
+                        },
+                    ],
+                },
+            },
+        )
+        resp = model.display(expand_completed=True, monochrome=True)
+
+        status_str = """
+-----------  ------------------------
+Workflow ID  <mocked-id>
+Name
+Status       preparing
+Submitted    2021-07-09T09:46:00.000Z
+Start        2021-07-09T09:47:00.000Z
+End          2021-07-09T09:48:00.000Z
+Duration     1m:0s
+Walltime     2m:0s
+-----------  ------------------------
+Jobs:
+  [#] print (1m:0s)
+"""
+
+        self.assertEqual(status_str.strip(), resp.strip())
```

