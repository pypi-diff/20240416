# Comparing `tmp/waitcondition-hook-for-aws-fargate-task-1.0.2.tar.gz` & `tmp/waitcondition-hook-for-aws-fargate-task-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waitcondition-hook-for-aws-fargate-task-1.0.2.tar", last modified: Mon Mar 11 03:58:00 2024, max compression
+gzip compressed data, was "waitcondition-hook-for-aws-fargate-task-1.0.3.tar", last modified: Mon Apr 15 11:44:16 2024, max compression
```

## Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2.tar` & `waitcondition-hook-for-aws-fargate-task-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:58:00.957266 waitcondition-hook-for-aws-fargate-task-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-11 03:58:00.957266 waitcondition-hook-for-aws-fargate-task-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 03:58:00.957266 waitcondition-hook-for-aws-fargate-task-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:58:00.953266 waitcondition-hook-for-aws-fargate-task-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:58:00.957266 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:58:00.957266 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23999 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 03:57:50.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 03:58:00.957266 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-11 03:58:00.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-11 03:58:00.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 03:58:00.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-11 03:58:00.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-11 03:58:00.000000 waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.283397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47992 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:44:04.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:44:16.287397 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 11:44:16.000000 waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/top_level.txt
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/LICENSE` & `waitcondition-hook-for-aws-fargate-task-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/PKG-INFO` & `waitcondition-hook-for-aws-fargate-task-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waitcondition-hook-for-aws-fargate-task
-Version: 1.0.2
+Version: 1.0.3
 Summary: AWS CDK Construct that run a Fargate task. Stack will process only when Fargate task executed successfully and all containers exit with code 0, otherwise rollback
 Home-page: https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Author: Amazon.com, Inc. or its affiliates. All Rights Reserved.<fanhongy@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,19 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Waitcondition Hook for AWS Fargate task
 
-This module will create an ECS cluster and run a Fargate task as you defined. It will pause the CloudFormation Stack until the Fargate task is complete and success.
+WaitCondition hook for AWS Fargate tasks is a AWS CDK Construct that helps builders to run a AWS Fargate task with one or multiple container embedded into a CloudFormation lifecycle. You can use this construct add dependency between resources and the AWS Fargate task execution result (eg. Database migration, image build and packing, invoking third party/on-prem API). waitcondition-hook-for-aws-fargate-task construct will also handle the failure of the task, and rollback the CloudFormation stack after.
+
+## Target architecture
+
+![Workflow](./image/workflow.png)
 
 ## Usage:
 
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { RemovalPolicy } from 'aws-cdk-lib';
 import { Vpc } from 'aws-cdk-lib/aws-ec2';
@@ -37,35 +41,34 @@
 import { Construct } from 'constructs';
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
-
+        // Define the VPC
+        const vpc = Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
-        // import exiting ecr repo
+        // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
         });
         // Create the Fargate runner
         const myFargateRunner = new FargateRunner(this, 'MyRunner', {
             fargateTaskDef: taskDefinition,
             timeout: `${60 * 5}`,
             vpc: vpc,
         });
         // Create the SQS queue
         const myQueue = new Queue(this, 'MyQueue', {});
-
         // Add dependency
         myQueue.node.addDependency(myFargateRunner);
-
     }
 }
 const app = new cdk.App();
 
 const env = {
     account: process.env.CDK_DEFAULT_ACCOUNT,
     region: process.env.CDK_DEFAULT_REGION,
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/README.md` & `waitcondition-hook-for-aws-fargate-task-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Waitcondition Hook for AWS Fargate task
 
-This module will create an ECS cluster and run a Fargate task as you defined. It will pause the CloudFormation Stack until the Fargate task is complete and success.
+WaitCondition hook for AWS Fargate tasks is a AWS CDK Construct that helps builders to run a AWS Fargate task with one or multiple container embedded into a CloudFormation lifecycle. You can use this construct add dependency between resources and the AWS Fargate task execution result (eg. Database migration, image build and packing, invoking third party/on-prem API). waitcondition-hook-for-aws-fargate-task construct will also handle the failure of the task, and rollback the CloudFormation stack after.
+
+## Target architecture
+
+![Workflow](./image/workflow.png)
 
 ## Usage:
 
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { RemovalPolicy } from 'aws-cdk-lib';
 import { Vpc } from 'aws-cdk-lib/aws-ec2';
@@ -14,35 +18,34 @@
 import { Construct } from 'constructs';
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
-
+        // Define the VPC
+        const vpc = Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
-        // import exiting ecr repo
+        // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
         });
         // Create the Fargate runner
         const myFargateRunner = new FargateRunner(this, 'MyRunner', {
             fargateTaskDef: taskDefinition,
             timeout: `${60 * 5}`,
             vpc: vpc,
         });
         // Create the SQS queue
         const myQueue = new Queue(this, 'MyQueue', {});
-
         // Add dependency
         myQueue.node.addDependency(myFargateRunner);
-
     }
 }
 const app = new cdk.App();
 
 const env = {
     account: process.env.CDK_DEFAULT_ACCOUNT,
     region: process.env.CDK_DEFAULT_REGION,
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/setup.py` & `waitcondition-hook-for-aws-fargate-task-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "waitcondition-hook-for-aws-fargate-task",
-    "version": "1.0.2",
+    "version": "1.0.3",
     "description": "AWS CDK Construct that run a Fargate task. Stack will process only when Fargate task executed successfully and all containers exit with code 0, otherwise rollback",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon.com, Inc. or its affiliates. All Rights Reserved.<fanhongy@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "waitcondition-hook-for-aws-fargate-task",
         "waitcondition-hook-for-aws-fargate-task._jsii"
     ],
     "package_data": {
         "waitcondition-hook-for-aws-fargate-task._jsii": [
-            "waitcondition-hook-for-aws-fargate-task@1.0.2.jsii.tgz"
+            "waitcondition-hook-for-aws-fargate-task@1.0.3.jsii.tgz"
         ],
         "waitcondition-hook-for-aws-fargate-task": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.109.0, <3.0.0",
+        "aws-cdk-lib>=2.137.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.93.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition-hook-for-aws-fargate-task/__init__.py` & `waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition-hook-for-aws-fargate-task/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 '''
 # Waitcondition Hook for AWS Fargate task
 
-This module will create an ECS cluster and run a Fargate task as you defined. It will pause the CloudFormation Stack until the Fargate task is complete and success.
+WaitCondition hook for AWS Fargate tasks is a AWS CDK Construct that helps builders to run a AWS Fargate task with one or multiple container embedded into a CloudFormation lifecycle. You can use this construct add dependency between resources and the AWS Fargate task execution result (eg. Database migration, image build and packing, invoking third party/on-prem API). waitcondition-hook-for-aws-fargate-task construct will also handle the failure of the task, and rollback the CloudFormation stack after.
+
+## Target architecture
+
+![Workflow](./image/workflow.png)
 
 ## Usage:
 
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { RemovalPolicy } from 'aws-cdk-lib';
 import { Vpc } from 'aws-cdk-lib/aws-ec2';
@@ -15,35 +19,34 @@
 import { Construct } from 'constructs';
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
-
+        // Define the VPC
+        const vpc = Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
-        // import exiting ecr repo
+        // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
         });
         // Create the Fargate runner
         const myFargateRunner = new FargateRunner(this, 'MyRunner', {
             fargateTaskDef: taskDefinition,
             timeout: `${60 * 5}`,
             vpc: vpc,
         });
         // Create the SQS queue
         const myQueue = new Queue(this, 'MyQueue', {});
-
         // Add dependency
         myQueue.node.addDependency(myFargateRunner);
-
     }
 }
 const app = new cdk.App();
 
 const env = {
     account: process.env.CDK_DEFAULT_ACCOUNT,
     region: process.env.CDK_DEFAULT_REGION,
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO` & `waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waitcondition-hook-for-aws-fargate-task
-Version: 1.0.2
+Version: 1.0.3
 Summary: AWS CDK Construct that run a Fargate task. Stack will process only when Fargate task executed successfully and all containers exit with code 0, otherwise rollback
 Home-page: https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Author: Amazon.com, Inc. or its affiliates. All Rights Reserved.<fanhongy@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/waitcondition-hook-for-aws-fargate-task.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,19 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Waitcondition Hook for AWS Fargate task
 
-This module will create an ECS cluster and run a Fargate task as you defined. It will pause the CloudFormation Stack until the Fargate task is complete and success.
+WaitCondition hook for AWS Fargate tasks is a AWS CDK Construct that helps builders to run a AWS Fargate task with one or multiple container embedded into a CloudFormation lifecycle. You can use this construct add dependency between resources and the AWS Fargate task execution result (eg. Database migration, image build and packing, invoking third party/on-prem API). waitcondition-hook-for-aws-fargate-task construct will also handle the failure of the task, and rollback the CloudFormation stack after.
+
+## Target architecture
+
+![Workflow](./image/workflow.png)
 
 ## Usage:
 
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { RemovalPolicy } from 'aws-cdk-lib';
 import { Vpc } from 'aws-cdk-lib/aws-ec2';
@@ -37,35 +41,34 @@
 import { Construct } from 'constructs';
 import { FargateRunner } from 'waitcondition-hook-for-aws-fargate-task';
 import { Queue } from 'aws-cdk-lib/aws-sqs';
 
 export class FargateRunnerTestStack extends cdk.Stack {
     constructor(scope: Construct, id: string, props?: cdk.StackProps) {
         super(scope, id, props);
-
+        // Define the VPC
+        const vpc = Vpc(this, 'MyVpc')
         // Define the Fargate Task
         const taskDefinition = new ecs.FargateTaskDefinition(this, 'MyTask', {});
-        // import exiting ecr repo
+        // Import exiting ecr repo
         const repo = ecr.Repository.fromRepositoryName(this, 'MyRepo', 'RepoName');
         // Add a container to the task
         taskDefinition.addContainer('MyContainer', {
             image: ecs.ContainerImage.fromEcrRepository(repo),
         });
         // Create the Fargate runner
         const myFargateRunner = new FargateRunner(this, 'MyRunner', {
             fargateTaskDef: taskDefinition,
             timeout: `${60 * 5}`,
             vpc: vpc,
         });
         // Create the SQS queue
         const myQueue = new Queue(this, 'MyQueue', {});
-
         // Add dependency
         myQueue.node.addDependency(myFargateRunner);
-
     }
 }
 const app = new cdk.App();
 
 const env = {
     account: process.env.CDK_DEFAULT_ACCOUNT,
     region: process.env.CDK_DEFAULT_REGION,
```

### Comparing `waitcondition-hook-for-aws-fargate-task-1.0.2/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt` & `waitcondition-hook-for-aws-fargate-task-1.0.3/src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt`

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
-src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.2.jsii.tgz
+src/waitcondition-hook-for-aws-fargate-task/_jsii/waitcondition-hook-for-aws-fargate-task@1.0.3.jsii.tgz
 src/waitcondition_hook_for_aws_fargate_task.egg-info/PKG-INFO
 src/waitcondition_hook_for_aws_fargate_task.egg-info/SOURCES.txt
 src/waitcondition_hook_for_aws_fargate_task.egg-info/dependency_links.txt
 src/waitcondition_hook_for_aws_fargate_task.egg-info/requires.txt
 src/waitcondition_hook_for_aws_fargate_task.egg-info/top_level.txt
```

