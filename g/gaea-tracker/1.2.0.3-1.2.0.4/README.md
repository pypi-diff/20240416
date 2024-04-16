# Comparing `tmp/gaea_tracker-1.2.0.3-py3-none-any.whl.zip` & `tmp/gaea_tracker-1.2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5831 bytes, number of entries: 8
--rw-r--r--  2.0 unx      213 b- defN 24-Apr-09 06:22 gaea_tracker/__init__.py
--rw-r--r--  2.0 unx     1654 b- defN 24-Apr-09 06:22 gaea_tracker/aim_tracker.py
--rw-r--r--  2.0 unx     7577 b- defN 24-Apr-09 06:22 gaea_tracker/experiment_tracker.py
--rw-r--r--  2.0 unx     1459 b- defN 24-Apr-09 06:22 gaea_tracker/mlflow_tracker.py
--rw-r--r--  2.0 unx     1745 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/RECORD
-8 files, 13421 bytes uncompressed, 4659 bytes compressed:  65.3%
+Zip file size: 5897 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-16 05:21 gaea_tracker/__init__.py
+-rw-r--r--  2.0 unx     1654 b- defN 24-Apr-16 05:21 gaea_tracker/aim_tracker.py
+-rw-r--r--  2.0 unx     7798 b- defN 24-Apr-16 05:21 gaea_tracker/experiment_tracker.py
+-rw-r--r--  2.0 unx     1459 b- defN 24-Apr-16 05:21 gaea_tracker/mlflow_tracker.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-16 05:21 gaea_tracker-1.2.0.4.dist-info/RECORD
+8 files, 13642 bytes uncompressed, 4725 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gaea_tracker/experiment_tracker.py
 Comment: 
 
 Filename: gaea_tracker/mlflow_tracker.py
 Comment: 
 
-Filename: gaea_tracker-1.2.0.3.dist-info/METADATA
+Filename: gaea_tracker-1.2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: gaea_tracker-1.2.0.3.dist-info/WHEEL
+Filename: gaea_tracker-1.2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_tracker-1.2.0.3.dist-info/top_level.txt
+Filename: gaea_tracker-1.2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_tracker-1.2.0.3.dist-info/RECORD
+Filename: gaea_tracker-1.2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gaea_tracker/experiment_tracker.py

```diff
@@ -6,14 +6,15 @@
 @Description   :
 """
 import os
 from typing import Dict, List
 import json
 from jsonschema import validate
 import yaml
+import bcelogger
 
 from windmillclient.client.windmill_client import WindmillClient
 from windmilltrainingv1.client.training_api_job import parse_job_name
 from windmilltrainingv1.client.training_api_project import parse_project_name
 
 
 class ExperimentTracker(object):
@@ -127,46 +128,50 @@
         """
         self._project_name = name
 
     def _update_run_id(self, run_id: str, name: str):
         """
         Update the run id.
         """
-        job_instance = parse_job_name(name)
-        workspace_id = job_instance.workspace_id
-        project_name = job_instance.project_name
-        local_name = job_instance.local_name
+        job = parse_job_name(name)
+        workspace_id = job.workspace_id
+        project_name = job.project_name
+        local_name = job.local_name
         response = self.windmill_client.get_job(workspace_id=workspace_id,
                                                 project_name=project_name,
                                                 local_name=local_name)
         experiment_runs = response.experimentRuns
         if experiment_runs is None:
             experiment_runs = {}
+        bcelogger.info(f"Job kind is {self.job_kind} and run id is {run_id}")
         experiment_runs.update({self.job_kind: run_id})
         self.windmill_client.update_job(workspace_id=workspace_id,
                                         project_name=project_name,
                                         display_name=response.displayName,
                                         local_name=local_name,
                                         experiment_runs=experiment_runs)
+        bcelogger.info(f"Update job {name} run id to {run_id}")
 
     def _get_windmill_job(self):
         """
         Get windmill job.
         """
-        project_instance = parse_project_name(self.project_name)
-        workspace_id, project_name = project_instance.workspace_id, project_instance.local_name
+        bcelogger.info(f"Project name is {self.project_name}")
+        project = parse_project_name(self.project_name)
+        workspace_id, project_name = project.workspace_id, project.local_name
         if "PF_RUN_ID" in os.environ and "PF_STEP_NAME" in os.environ:
             paddleflow_run_id = os.environ["PF_RUN_ID"]
             self._job_kind = os.environ["PF_STEP_NAME"]
             self._work_dir = os.environ["PF_WORK_DIR"]
             self._extra_work_dir = os.environ.get("PF_EXTRA_WORK_DIR")
             response = self.windmill_client.get_job(workspace_id=workspace_id,
                                                     project_name=project_name,
                                                     local_name=paddleflow_run_id,
                                                     naming_kind="runID")
+            bcelogger.info(f"Get job response is {response}")
             assert response.name is not None, \
                 f"The job name is empty, " \
                 f"please check your request workspace_id={workspace_id} project_name={project_name} " \
                 f"local_name={paddleflow_run_id} naming_kind=runID, " \
                 f"response is {response}"
             name = response.name
             self.config_param = {"org_id": response.orgID, "project_name": response.projectName}
```

## Comparing `gaea_tracker-1.2.0.3.dist-info/METADATA` & `gaea_tracker-1.2.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaea-tracker
-Version: 1.2.0.3
+Version: 1.2.0.4
 Summary: A common tracker library.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gaea_tracker-1.2.0.3.dist-info/RECORD` & `gaea_tracker-1.2.0.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gaea_tracker/__init__.py,sha256=W_LJdwsPO-i_I_labqmA9UtINpc16H_xrUMtH3BgJrg,213
 gaea_tracker/aim_tracker.py,sha256=B8WcwJPQC6hKy-NMeZOYY6rQ4-cER_2j0zrxdPcNlxQ,1654
-gaea_tracker/experiment_tracker.py,sha256=ztxoWQCK9EdQ0Qzos7N7K4SI1gY4k1k96kE3y1I9NpY,7577
+gaea_tracker/experiment_tracker.py,sha256=QojIx4sZjL6Trlla3rtqFObeCE8F-cfzmxMcTuXN3wk,7798
 gaea_tracker/mlflow_tracker.py,sha256=iSHBX25D1K5Ss1Jnhyq_2q9KAeizhOz_LTXIVcU3OXE,1459
-gaea_tracker-1.2.0.3.dist-info/METADATA,sha256=EyDfKdAHc8f8qB96ytQLPvUspvnLGCAOYaH4E5DDvwk,1745
-gaea_tracker-1.2.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gaea_tracker-1.2.0.3.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
-gaea_tracker-1.2.0.3.dist-info/RECORD,,
+gaea_tracker-1.2.0.4.dist-info/METADATA,sha256=sXqEtgpKRW1QeufuDVlNzqB58LyNO1q5VCbAvELJHhU,1745
+gaea_tracker-1.2.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gaea_tracker-1.2.0.4.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
+gaea_tracker-1.2.0.4.dist-info/RECORD,,
```

