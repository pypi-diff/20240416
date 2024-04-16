# Comparing `tmp/waitcondition-hook-for-aws-fargate-task-1.0.3.tar.gz` & `tmp/waitcondition-hook-for-aws-fargate-task-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waitcondition-hook-for-aws-fargate-task-1.0.3.tar", last modified: Mon Apr 15 11:44:16 2024, max compression
+gzip compressed data, was "waitcondition-hook-for-aws-fargate-task-1.0.4.tar", last modified: Tue Apr 16 01:39:34 2024, max compression
```

## Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3.tar` & `waitcondition-hook-for-aws-fargate-task-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.283397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47992 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:39:34.492999 waitcondition-hook-for-aws-fargate-task-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-16 01:39:34.492999 waitcondition-hook-for-aws-fargate-task-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:39:34.492999 waitcondition-hook-for-aws-fargate-task-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:39:34.488999 waitcondition-hook-for-aws-fargate-task-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:39:34.488999 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:39:34.488999 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47998 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:39:22.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:39:34.492999 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-16 01:39:34.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-16 01:39:34.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:39:34.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 01:39:34.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-16 01:39:34.000000 waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/top_level.txt
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/LICENSE` & `waitcondition-hook-for-aws-fargate-task-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/PKG-INFO` & `waitcondition-hook-for-aws-fargate-task-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waitcondition-hook-for-aws-fargate-task
-Version: 1.0.3
+Version: 1.0.4
 Summary: AWS CDK Construct that run a Fargate task. Stack will process only when Fargate task executed successfully and all containers exit with code 0, otherwise rollback
 Home-page: https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Author: Amazon.com, Inc. or its affiliates. All Rights Reserved.<fanhongy@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
         // Define the VPC
-        const vpc = Vpc(this, 'MyVpc')
+        const vpc = new Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
         // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/README.md` & `waitcondition-hook-for-aws-fargate-task-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
         // Define the VPC
-        const vpc = Vpc(this, 'MyVpc')
+        const vpc = new Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
         // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/setup.py` & `waitcondition-hook-for-aws-fargate-task-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "waitcondition-hook-for-aws-fargate-task",
-    "version": "1.0.3",
+    "version": "1.0.4",
     "description": "AWS CDK Construct that run a Fargate task. Stack will process only when Fargate task executed successfully and all containers exit with code 0, otherwise rollback",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon.com, Inc. or its affiliates. All Rights Reserved.<fanhongy@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "waitcondition-hook-for-aws-fargate-task",
         "waitcondition-hook-for-aws-fargate-task._jsii"
     ],
     "package_data": {
         "waitcondition-hook-for-aws-fargate-task._jsii": [
-            "waitcondition-hook-for-aws-fargate-task@1.0.3.jsii.tgz"
+            "waitcondition-hook-for-aws-fargate-task@1.0.4.jsii.tgz"
         ],
         "waitcondition-hook-for-aws-fargate-task": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/__init__.py` & `waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition-hook-for-aws-fargate-task/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
         // Define the VPC
-        const vpc = Vpc(this, 'MyVpc')
+        const vpc = new Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
         // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO` & `waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waitcondition-hook-for-aws-fargate-task
-Version: 1.0.3
+Version: 1.0.4
 Summary: AWS CDK Construct that run a Fargate task. Stack will process only when Fargate task executed successfully and all containers exit with code 0, otherwise rollback
 Home-page: https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Author: Amazon.com, Inc. or its affiliates. All Rights Reserved.<fanhongy@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
         // Define the VPC
-        const vpc = Vpc(this, 'MyVpc')
+        const vpc = new Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
         // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt` & `waitcondition-hook-for-aws-fargate-task-1.0.4/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/waitcondition-hook-for-aws-fargate-task/__init__.py
 src/waitcondition-hook-for-aws-fargate-task/py.typed
 src/waitcondition-hook-for-aws-fargate-task/_jsii/__init__.py
-src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.3.jsii.tgz
+src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.4.jsii.tgz
 src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO
 src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt
 src/waitcondition_hook_for_aws_fargate_task.egg-info/dependency_links.txt
 src/waitcondition_hook_for_aws_fargate_task.egg-info/requires.txt
 src/waitcondition_hook_for_aws_fargate_task.egg-info/top_level.txt
```

