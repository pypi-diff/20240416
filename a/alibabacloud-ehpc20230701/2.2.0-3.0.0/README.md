# Comparing `tmp/alibabacloud_ehpc20230701-2.2.0.tar.gz` & `tmp/alibabacloud_ehpc20230701-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ehpc20230701-2.2.0.tar", last modified: Fri Mar 15 17:10:17 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ehpc20230701-3.0.0.tar", last modified: Tue Apr 16 03:01:01 2024, max compression
```

## Comparing `alibabacloud_ehpc20230701-2.2.0.tar` & `alibabacloud_ehpc20230701-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2438 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35815 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701/client.py
--rw-r--r--   0 root         (0) root         (0)   124286 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2438 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-03-15 17:10:17.000000 alibabacloud_ehpc20230701-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43481 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/client.py
+-rw-r--r--   0 root         (0) root         (0)   139430 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/setup.py
```

### Comparing `alibabacloud_ehpc20230701-2.2.0/ChangeLog.md` & `alibabacloud_ehpc20230701-3.0.0/ChangeLog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-03-15 Version: 2.2.0
+- Support API ListExecutors.
+- Update API DeleteJobs: add param ExecutorIds.
+
+
 2024-03-13 Version: 2.1.0
 - Support API ListJobExecutors.
 - Update API AddImage: delete param Action.
 - Update API AddImage: delete param RegionId.
 - Update API CreateJob: update param Tasks.
 - Update API GetImage: delete param Action.
 - Update API GetImage: delete param RegionId.
```

### Comparing `alibabacloud_ehpc20230701-2.2.0/LICENSE` & `alibabacloud_ehpc20230701-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20230701-2.2.0/PKG-INFO` & `alibabacloud_ehpc20230701-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ehpc20230701
-Version: 2.2.0
+Version: 3.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20230701) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20230701-2.2.0/README-CN.md` & `alibabacloud_ehpc20230701-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20230701-2.2.0/README.md` & `alibabacloud_ehpc20230701-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701/client.py` & `alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -315,14 +315,190 @@
     async def delete_jobs_async(
         self,
         request: ehpc20230701_models.DeleteJobsRequest,
     ) -> ehpc20230701_models.DeleteJobsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_jobs_with_options_async(request, runtime)
 
+    def describe_job_metric_data_with_options(
+        self,
+        tmp_req: ehpc20230701_models.DescribeJobMetricDataRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ehpc20230701_models.DescribeJobMetricDataShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.array_index):
+            request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.array_index_shrink):
+            query['ArrayIndex'] = request.array_index_shrink
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        if not UtilClient.is_unset(request.metric_name):
+            query['MetricName'] = request.metric_name
+        if not UtilClient.is_unset(request.task_name):
+            query['TaskName'] = request.task_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeJobMetricData',
+            version='2023-07-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ehpc20230701_models.DescribeJobMetricDataResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_job_metric_data_with_options_async(
+        self,
+        tmp_req: ehpc20230701_models.DescribeJobMetricDataRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ehpc20230701_models.DescribeJobMetricDataShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.array_index):
+            request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.array_index_shrink):
+            query['ArrayIndex'] = request.array_index_shrink
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        if not UtilClient.is_unset(request.metric_name):
+            query['MetricName'] = request.metric_name
+        if not UtilClient.is_unset(request.task_name):
+            query['TaskName'] = request.task_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeJobMetricData',
+            version='2023-07-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ehpc20230701_models.DescribeJobMetricDataResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_job_metric_data(
+        self,
+        request: ehpc20230701_models.DescribeJobMetricDataRequest,
+    ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_job_metric_data_with_options(request, runtime)
+
+    async def describe_job_metric_data_async(
+        self,
+        request: ehpc20230701_models.DescribeJobMetricDataRequest,
+    ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_job_metric_data_with_options_async(request, runtime)
+
+    def describe_job_metric_last_with_options(
+        self,
+        tmp_req: ehpc20230701_models.DescribeJobMetricLastRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ehpc20230701_models.DescribeJobMetricLastShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.array_index):
+            request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.array_index_shrink):
+            query['ArrayIndex'] = request.array_index_shrink
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        if not UtilClient.is_unset(request.task_name):
+            query['TaskName'] = request.task_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeJobMetricLast',
+            version='2023-07-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ehpc20230701_models.DescribeJobMetricLastResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_job_metric_last_with_options_async(
+        self,
+        tmp_req: ehpc20230701_models.DescribeJobMetricLastRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        UtilClient.validate_model(tmp_req)
+        request = ehpc20230701_models.DescribeJobMetricLastShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.array_index):
+            request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.array_index_shrink):
+            query['ArrayIndex'] = request.array_index_shrink
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        if not UtilClient.is_unset(request.task_name):
+            query['TaskName'] = request.task_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeJobMetricLast',
+            version='2023-07-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ehpc20230701_models.DescribeJobMetricLastResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_job_metric_last(
+        self,
+        request: ehpc20230701_models.DescribeJobMetricLastRequest,
+    ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_job_metric_last_with_options(request, runtime)
+
+    async def describe_job_metric_last_async(
+        self,
+        request: ehpc20230701_models.DescribeJobMetricLastRequest,
+    ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_job_metric_last_with_options_async(request, runtime)
+
     def get_image_with_options(
         self,
         request: ehpc20230701_models.GetImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.GetImageResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701/models.py` & `alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,14 +1098,100 @@
                 temp_model = CreateJobRequestTasksTaskSpecResourceDisks()
                 self.disks.append(temp_model.from_map(k))
         if m.get('Memory') is not None:
             self.memory = m.get('Memory')
         return self
 
 
+class CreateJobRequestTasksTaskSpecTaskExecutorContainerEnvironmentVars(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        value: str = None,
+    ):
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateJobRequestTasksTaskSpecTaskExecutorContainer(TeaModel):
+    def __init__(
+        self,
+        command: List[str] = None,
+        environment_vars: List[CreateJobRequestTasksTaskSpecTaskExecutorContainerEnvironmentVars] = None,
+        image: str = None,
+        working_dir: str = None,
+    ):
+        self.command = command
+        self.environment_vars = environment_vars
+        self.image = image
+        self.working_dir = working_dir
+
+    def validate(self):
+        if self.environment_vars:
+            for k in self.environment_vars:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.command is not None:
+            result['Command'] = self.command
+        result['EnvironmentVars'] = []
+        if self.environment_vars is not None:
+            for k in self.environment_vars:
+                result['EnvironmentVars'].append(k.to_map() if k else None)
+        if self.image is not None:
+            result['Image'] = self.image
+        if self.working_dir is not None:
+            result['WorkingDir'] = self.working_dir
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Command') is not None:
+            self.command = m.get('Command')
+        self.environment_vars = []
+        if m.get('EnvironmentVars') is not None:
+            for k in m.get('EnvironmentVars'):
+                temp_model = CreateJobRequestTasksTaskSpecTaskExecutorContainerEnvironmentVars()
+                self.environment_vars.append(temp_model.from_map(k))
+        if m.get('Image') is not None:
+            self.image = m.get('Image')
+        if m.get('WorkingDir') is not None:
+            self.working_dir = m.get('WorkingDir')
+        return self
+
+
 class CreateJobRequestTasksTaskSpecTaskExecutorVM(TeaModel):
     def __init__(
         self,
         image: str = None,
         prolog_script: str = None,
         script: str = None,
     ):
@@ -1140,81 +1226,144 @@
             self.script = m.get('Script')
         return self
 
 
 class CreateJobRequestTasksTaskSpecTaskExecutor(TeaModel):
     def __init__(
         self,
+        container: CreateJobRequestTasksTaskSpecTaskExecutorContainer = None,
         vm: CreateJobRequestTasksTaskSpecTaskExecutorVM = None,
     ):
+        self.container = container
         self.vm = vm
 
     def validate(self):
+        if self.container:
+            self.container.validate()
         if self.vm:
             self.vm.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.container is not None:
+            result['Container'] = self.container.to_map()
         if self.vm is not None:
             result['VM'] = self.vm.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Container') is not None:
+            temp_model = CreateJobRequestTasksTaskSpecTaskExecutorContainer()
+            self.container = temp_model.from_map(m['Container'])
         if m.get('VM') is not None:
             temp_model = CreateJobRequestTasksTaskSpecTaskExecutorVM()
             self.vm = temp_model.from_map(m['VM'])
         return self
 
 
+class CreateJobRequestTasksTaskSpecVolumeMount(TeaModel):
+    def __init__(
+        self,
+        mount_options: str = None,
+        mount_path: str = None,
+        volume_driver: str = None,
+    ):
+        self.mount_options = mount_options
+        self.mount_path = mount_path
+        self.volume_driver = volume_driver
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mount_options is not None:
+            result['MountOptions'] = self.mount_options
+        if self.mount_path is not None:
+            result['MountPath'] = self.mount_path
+        if self.volume_driver is not None:
+            result['VolumeDriver'] = self.volume_driver
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MountOptions') is not None:
+            self.mount_options = m.get('MountOptions')
+        if m.get('MountPath') is not None:
+            self.mount_path = m.get('MountPath')
+        if m.get('VolumeDriver') is not None:
+            self.volume_driver = m.get('VolumeDriver')
+        return self
+
+
 class CreateJobRequestTasksTaskSpec(TeaModel):
     def __init__(
         self,
         resource: CreateJobRequestTasksTaskSpecResource = None,
         task_executor: List[CreateJobRequestTasksTaskSpecTaskExecutor] = None,
+        volume_mount: List[CreateJobRequestTasksTaskSpecVolumeMount] = None,
     ):
         self.resource = resource
         self.task_executor = task_executor
+        self.volume_mount = volume_mount
 
     def validate(self):
         if self.resource:
             self.resource.validate()
         if self.task_executor:
             for k in self.task_executor:
                 if k:
                     k.validate()
+        if self.volume_mount:
+            for k in self.volume_mount:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.resource is not None:
             result['Resource'] = self.resource.to_map()
         result['TaskExecutor'] = []
         if self.task_executor is not None:
             for k in self.task_executor:
                 result['TaskExecutor'].append(k.to_map() if k else None)
+        result['VolumeMount'] = []
+        if self.volume_mount is not None:
+            for k in self.volume_mount:
+                result['VolumeMount'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Resource') is not None:
             temp_model = CreateJobRequestTasksTaskSpecResource()
             self.resource = temp_model.from_map(m['Resource'])
         self.task_executor = []
         if m.get('TaskExecutor') is not None:
             for k in m.get('TaskExecutor'):
                 temp_model = CreateJobRequestTasksTaskSpecTaskExecutor()
                 self.task_executor.append(temp_model.from_map(k))
+        self.volume_mount = []
+        if m.get('VolumeMount') is not None:
+            for k in m.get('VolumeMount'):
+                temp_model = CreateJobRequestTasksTaskSpecVolumeMount()
+                self.volume_mount.append(temp_model.from_map(k))
         return self
 
 
 class CreateJobRequestTasks(TeaModel):
     def __init__(
         self,
         executor_policy: CreateJobRequestTasksExecutorPolicy = None,
@@ -1653,14 +1802,377 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteJobsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeJobMetricDataRequest(TeaModel):
+    def __init__(
+        self,
+        array_index: List[int] = None,
+        job_id: str = None,
+        metric_name: str = None,
+        task_name: str = None,
+    ):
+        self.array_index = array_index
+        self.job_id = job_id
+        self.metric_name = metric_name
+        self.task_name = task_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.array_index is not None:
+            result['ArrayIndex'] = self.array_index
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.metric_name is not None:
+            result['MetricName'] = self.metric_name
+        if self.task_name is not None:
+            result['TaskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArrayIndex') is not None:
+            self.array_index = m.get('ArrayIndex')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('MetricName') is not None:
+            self.metric_name = m.get('MetricName')
+        if m.get('TaskName') is not None:
+            self.task_name = m.get('TaskName')
+        return self
+
+
+class DescribeJobMetricDataShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        array_index_shrink: str = None,
+        job_id: str = None,
+        metric_name: str = None,
+        task_name: str = None,
+    ):
+        self.array_index_shrink = array_index_shrink
+        self.job_id = job_id
+        self.metric_name = metric_name
+        self.task_name = task_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.array_index_shrink is not None:
+            result['ArrayIndex'] = self.array_index_shrink
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.metric_name is not None:
+            result['MetricName'] = self.metric_name
+        if self.task_name is not None:
+            result['TaskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArrayIndex') is not None:
+            self.array_index_shrink = m.get('ArrayIndex')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('MetricName') is not None:
+            self.metric_name = m.get('MetricName')
+        if m.get('TaskName') is not None:
+            self.task_name = m.get('TaskName')
+        return self
+
+
+class DescribeJobMetricDataResponseBody(TeaModel):
+    def __init__(
+        self,
+        data_points: str = None,
+        period: int = None,
+        request_id: str = None,
+    ):
+        self.data_points = data_points
+        self.period = period
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_points is not None:
+            result['DataPoints'] = self.data_points
+        if self.period is not None:
+            result['Period'] = self.period
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataPoints') is not None:
+            self.data_points = m.get('DataPoints')
+        if m.get('Period') is not None:
+            self.period = m.get('Period')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeJobMetricDataResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeJobMetricDataResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeJobMetricDataResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeJobMetricLastRequest(TeaModel):
+    def __init__(
+        self,
+        array_index: List[int] = None,
+        job_id: str = None,
+        task_name: str = None,
+    ):
+        self.array_index = array_index
+        self.job_id = job_id
+        self.task_name = task_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.array_index is not None:
+            result['ArrayIndex'] = self.array_index
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.task_name is not None:
+            result['TaskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArrayIndex') is not None:
+            self.array_index = m.get('ArrayIndex')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('TaskName') is not None:
+            self.task_name = m.get('TaskName')
+        return self
+
+
+class DescribeJobMetricLastShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        array_index_shrink: str = None,
+        job_id: str = None,
+        task_name: str = None,
+    ):
+        self.array_index_shrink = array_index_shrink
+        self.job_id = job_id
+        self.task_name = task_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.array_index_shrink is not None:
+            result['ArrayIndex'] = self.array_index_shrink
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.task_name is not None:
+            result['TaskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArrayIndex') is not None:
+            self.array_index_shrink = m.get('ArrayIndex')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('TaskName') is not None:
+            self.task_name = m.get('TaskName')
+        return self
+
+
+class DescribeJobMetricLastResponseBodyMetrics(TeaModel):
+    def __init__(
+        self,
+        array_index: int = None,
+        metric: str = None,
+    ):
+        self.array_index = array_index
+        self.metric = metric
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.array_index is not None:
+            result['ArrayIndex'] = self.array_index
+        if self.metric is not None:
+            result['Metric'] = self.metric
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArrayIndex') is not None:
+            self.array_index = m.get('ArrayIndex')
+        if m.get('Metric') is not None:
+            self.metric = m.get('Metric')
+        return self
+
+
+class DescribeJobMetricLastResponseBody(TeaModel):
+    def __init__(
+        self,
+        metrics: List[DescribeJobMetricLastResponseBodyMetrics] = None,
+        request_id: str = None,
+    ):
+        self.metrics = metrics
+        self.request_id = request_id
+
+    def validate(self):
+        if self.metrics:
+            for k in self.metrics:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Metrics'] = []
+        if self.metrics is not None:
+            for k in self.metrics:
+                result['Metrics'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.metrics = []
+        if m.get('Metrics') is not None:
+            for k in m.get('Metrics'):
+                temp_model = DescribeJobMetricLastResponseBodyMetrics()
+                self.metrics.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeJobMetricLastResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeJobMetricLastResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeJobMetricLastResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetImageRequest(TeaModel):
     def __init__(
         self,
         image_id: str = None,
     ):
         self.image_id = image_id
 
@@ -2841,27 +3353,23 @@
         return self
 
 
 class ListExecutorsResponseBody(TeaModel):
     def __init__(
         self,
         executors: List[ListExecutorsResponseBodyExecutors] = None,
-        job_id: str = None,
         page_number: str = None,
         page_size: str = None,
         request_id: str = None,
-        task_name: str = None,
         total_count: str = None,
     ):
         self.executors = executors
-        self.job_id = job_id
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
-        self.task_name = task_name
         self.total_count = total_count
 
     def validate(self):
         if self.executors:
             for k in self.executors:
                 if k:
                     k.validate()
@@ -2872,45 +3380,37 @@
             return _map
 
         result = dict()
         result['Executors'] = []
         if self.executors is not None:
             for k in self.executors:
                 result['Executors'].append(k.to_map() if k else None)
-        if self.job_id is not None:
-            result['JobId'] = self.job_id
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.task_name is not None:
-            result['TaskName'] = self.task_name
         if self.total_count is not None:
             result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.executors = []
         if m.get('Executors') is not None:
             for k in m.get('Executors'):
                 temp_model = ListExecutorsResponseBodyExecutors()
                 self.executors.append(temp_model.from_map(k))
-        if m.get('JobId') is not None:
-            self.job_id = m.get('JobId')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('TaskName') is not None:
-            self.task_name = m.get('TaskName')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class ListExecutorsResponse(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_ehpc20230701-2.2.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO` & `alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ehpc20230701
-Version: 2.2.0
+Version: 3.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20230701) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20230701-2.2.0/setup.py` & `alibabacloud_ehpc20230701-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ehpc20230701.
 
-Created on 15/03/2024
+Created on 16/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ehpc20230701"
 NAME = "alibabacloud_ehpc20230701" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elastic High Performance Computing (20230701) SDK Library for Python"
```

