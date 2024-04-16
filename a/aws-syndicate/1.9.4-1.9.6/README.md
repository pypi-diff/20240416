# Comparing `tmp/aws-syndicate-1.9.4.tar.gz` & `tmp/aws-syndicate-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-syndicate-1.9.4.tar", last modified: Tue Dec 19 11:03:09 2023, max compression
+gzip compressed data, was "aws-syndicate-1.9.6.tar", last modified: Mon Jan  8 13:58:08 2024, max compression
```

## Comparing `aws-syndicate-1.9.4.tar` & `aws-syndicate-1.9.6.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.711065 aws-syndicate-1.9.4/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11357 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/LICENSE
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    14485 2023-12-19 11:03:09.711065 aws-syndicate-1.9.4/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13485 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/README.md
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.711065 aws-syndicate-1.9.4/aws_syndicate.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    14485 2023-12-19 11:03:09.000000 aws-syndicate-1.9.4/aws_syndicate.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9951 2023-12-19 11:03:09.000000 aws-syndicate-1.9.4/aws_syndicate.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-12-19 11:03:09.000000 aws-syndicate-1.9.4/aws_syndicate.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       64 2023-12-19 11:03:09.000000 aws-syndicate-1.9.4/aws_syndicate.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      183 2023-12-19 11:03:09.000000 aws-syndicate-1.9.4/aws_syndicate.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       10 2023-12-19 11:03:09.000000 aws-syndicate-1.9.4/aws_syndicate.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       79 2023-12-19 11:03:09.711065 aws-syndicate-1.9.4/setup.cfg
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2204 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/setup.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.671064 aws-syndicate-1.9.4/syndicate/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.671064 aws-syndicate-1.9.4/syndicate/commons/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/commons/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3311 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/commons/log_helper.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.675064 aws-syndicate-1.9.4/syndicate/connection/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8404 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    33977 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/api_gateway_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8718 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/application_autoscaling_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9549 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/batch_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20973 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/cloud_watch_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2553 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/cloudfront_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6834 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/cognito_identity_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5475 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/cognito_identity_provider_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4167 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/dax_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5893 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/documentdb_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    44385 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/dynamo_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15840 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/ec2_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6820 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/elastic_beanstalk_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1793 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/eventbridge_scheduler_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/firehose_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3486 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/helper.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25713 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/iam_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2849 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/kinesis_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3215 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/kms_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30172 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/lambda_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2059 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/resource_groups_tagging_api_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16776 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/s3_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3047 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/ses_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9513 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/sns_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6186 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/sqs_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4686 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/step_functions_connection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3305 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/connection/sts_connection.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.679065 aws-syndicate-1.9.4/syndicate/core/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9293 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.679065 aws-syndicate-1.9.4/syndicate/core/build/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2103 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/artifact_processor.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12106 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/bundle_processor.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27226 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/deployment_processor.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1768 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/helper.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22965 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/meta_processor.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9261 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/profiler_processor.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.679065 aws-syndicate-1.9.4/syndicate/core/build/runtime/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      602 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/runtime/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1772 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/runtime/java.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4624 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/runtime/nodejs.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15997 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/runtime/python.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.683065 aws-syndicate-1.9.4/syndicate/core/build/validator/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      967 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/validator/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14908 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/validator/batch_compenv_validator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14128 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/validator/batch_jobdef_validator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8926 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/validator/dynamodb_validator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2681 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/validator/lambda_validator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2268 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/validator/mapping.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11367 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/build/warmup_processor.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.683065 aws-syndicate-1.9.4/syndicate/core/conf/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/conf/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4866 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/conf/bucket_view.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6235 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/conf/generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16495 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/conf/processor.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15070 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/conf/validator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4866 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/constants.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2787 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/decorators.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.683065 aws-syndicate-1.9.4/syndicate/core/generators/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2096 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16888 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/contents.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.687065 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3547 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7114 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/api_gateway_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9797 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/base_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1387 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/batch_compenv_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      633 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/batch_jobdef_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2001 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/batch_jobqueue_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1559 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cloudwatch_alarm_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1213 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cloudwatch_event_rule_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      447 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cognito_federated_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1290 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cognito_user_pool_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      598 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/dax_cluster_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1505 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/docdb_cluster_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1513 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/docdb_instance_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3699 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/dynamodb_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      836 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/ec2_instance_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      293 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/eventbridge_rule_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      855 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/iam_policy_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2119 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/iam_role_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      331 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/kinesis_stream_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      586 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/s3_bucket_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      845 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/sns_application_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      341 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/sns_topic_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1117 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/sqs_queue_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      281 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/step_function_activity_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      651 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/step_function_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1445 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/web_socket_api_gateway_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14499 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/lambda_function.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4642 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/project.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2023 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/generators/tests.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.691065 aws-syndicate-1.9.4/syndicate/core/groups/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      697 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/groups/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8240 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/groups/generate.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    41096 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/groups/meta.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1701 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/groups/tags.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    35179 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/handlers.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21809 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/helper.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.691065 aws-syndicate-1.9.4/syndicate/core/project_state/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      602 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/project_state/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17715 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/project_state/project_state.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6922 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/project_state/status_processor.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2169 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/project_state/sync_processor.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.699065 aws-syndicate-1.9.4/syndicate/core/resources/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2546 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/abstract_external_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40873 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/api_gateway_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1649 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/base_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8094 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/batch_compenv_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4130 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/batch_jobdef_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3074 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/batch_jobqueue_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3673 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/cloud_watch_alarm_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7850 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/cloud_watch_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4207 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/cognito_identity_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7131 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/cognito_user_pool_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4083 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/dax_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4470 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/docdb_cluster_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3380 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/docdb_instance_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17302 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/dynamo_db_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9744 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/ebs_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8121 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/ec2_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5800 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/eventbridge_scheduler_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2921 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/firehose_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4042 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/group_tagging_api_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6208 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/helper.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14761 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/iam_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2880 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/kinesis_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    46532 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/lambda_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12784 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/processors_mapping.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13837 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/resources_provider.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7281 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/s3_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12204 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/sns_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6501 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/sqs_resource.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9113 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/resources/step_functions_resource.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.699065 aws-syndicate-1.9.4/syndicate/core/transform/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5061 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/build_meta_transformer.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.699065 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2711 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/cf_transform_utils.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6113 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/cloudformation_transformer.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.703065 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23992 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_api_gateway_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4239 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_batch_compenv_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4594 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_batch_job_defeinition.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1762 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_batch_job_queue_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1888 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_alarm_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4120 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_rule_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2506 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_cognito_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9892 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_dynamodb_table_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1086 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_iam_managed_policy_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4371 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_iam_role_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1173 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_kinesis_stream_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17045 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_lambda_function_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1637 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_lambda_layer_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1065 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_resource_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6121 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_s3_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1009 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_sns_application_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3537 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_sns_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4533 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_sqs_converter.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.703065 aws-syndicate-1.9.4/syndicate/core/transform/terraform/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:03:09.707065 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    29869 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_api_gateway_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6856 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_batch_compenv_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3101 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_batch_jobdef_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2009 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_batch_jobqueue_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3327 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_cloud_watch_alram_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4378 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_cloud_watch_rule_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3866 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_cognito_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12327 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_dynamo_db_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1291 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_iam_policy_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3093 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_iam_role_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1260 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_kinesis_stream_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    24116 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_lambda_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2544 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_lambda_layer_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1058 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_resource_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3297 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_s3_bucket_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1918 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_sns_app_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5408 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_sns_topic_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9561 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_sqs_converter.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19233 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/terraform_template.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7241 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/terraform_transformer.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1543 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/tf_helper.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      884 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/tf_resource_name_builder.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4335 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/terraform/tf_resource_reference_builder.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2603 2023-12-19 11:02:18.000000 aws-syndicate-1.9.4/syndicate/core/transform/transform_processor.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.895956 aws-syndicate-1.9.6/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11357 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/LICENSE
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    14453 2024-01-08 13:58:08.895956 aws-syndicate-1.9.6/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13485 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/README.md
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.895956 aws-syndicate-1.9.6/aws_syndicate.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    14453 2024-01-08 13:58:08.000000 aws-syndicate-1.9.6/aws_syndicate.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9951 2024-01-08 13:58:08.000000 aws-syndicate-1.9.6/aws_syndicate.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2024-01-08 13:58:08.000000 aws-syndicate-1.9.6/aws_syndicate.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       64 2024-01-08 13:58:08.000000 aws-syndicate-1.9.6/aws_syndicate.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      166 2024-01-08 13:58:08.000000 aws-syndicate-1.9.6/aws_syndicate.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       10 2024-01-08 13:58:08.000000 aws-syndicate-1.9.6/aws_syndicate.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       79 2024-01-08 13:58:08.895956 aws-syndicate-1.9.6/setup.cfg
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2176 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/setup.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.851955 aws-syndicate-1.9.6/syndicate/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/__init__.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.851955 aws-syndicate-1.9.6/syndicate/commons/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/commons/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3311 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/commons/log_helper.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.859955 aws-syndicate-1.9.6/syndicate/connection/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8404 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    33977 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/api_gateway_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8718 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/application_autoscaling_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9549 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/batch_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20973 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/cloud_watch_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2553 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/cloudfront_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6834 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/cognito_identity_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5475 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/cognito_identity_provider_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4167 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/dax_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5893 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/documentdb_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    44385 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/dynamo_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15840 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/ec2_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6820 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/elastic_beanstalk_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1793 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/eventbridge_scheduler_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2453 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/firehose_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3486 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/helper.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25713 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/iam_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2849 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/kinesis_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3215 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/kms_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30172 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/lambda_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2059 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/resource_groups_tagging_api_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16776 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/s3_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3047 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/ses_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9513 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/sns_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6186 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/sqs_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4686 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/step_functions_connection.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3305 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/connection/sts_connection.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.859955 aws-syndicate-1.9.6/syndicate/core/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9293 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/__init__.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.863955 aws-syndicate-1.9.6/syndicate/core/build/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2103 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/artifact_processor.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12106 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/bundle_processor.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27226 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/deployment_processor.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1768 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/helper.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22965 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/meta_processor.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9261 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/profiler_processor.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.863955 aws-syndicate-1.9.6/syndicate/core/build/runtime/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      602 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/runtime/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1772 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/runtime/java.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4624 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/runtime/nodejs.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15997 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/runtime/python.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.863955 aws-syndicate-1.9.6/syndicate/core/build/validator/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      967 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/validator/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14908 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/validator/batch_compenv_validator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14128 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/validator/batch_jobdef_validator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8926 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/validator/dynamodb_validator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2681 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/validator/lambda_validator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2268 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/validator/mapping.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11367 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/build/warmup_processor.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.867956 aws-syndicate-1.9.6/syndicate/core/conf/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/conf/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4866 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/conf/bucket_view.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6235 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/conf/generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14741 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/conf/processor.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15070 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/conf/validator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4866 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/constants.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2787 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/decorators.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.867956 aws-syndicate-1.9.6/syndicate/core/generators/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2096 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16888 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/contents.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.871955 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3547 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7114 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/api_gateway_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9797 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/base_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1387 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/batch_compenv_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      633 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/batch_jobdef_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2001 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/batch_jobqueue_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1559 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cloudwatch_alarm_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1213 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cloudwatch_event_rule_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      447 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cognito_federated_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1290 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cognito_user_pool_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      598 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/dax_cluster_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1505 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/docdb_cluster_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1513 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/docdb_instance_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3699 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/dynamodb_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      836 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/ec2_instance_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      293 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/eventbridge_rule_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      855 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/iam_policy_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2119 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/iam_role_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      331 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/kinesis_stream_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      586 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/s3_bucket_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      845 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/sns_application_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      341 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/sns_topic_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1117 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/sqs_queue_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      281 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/step_function_activity_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      651 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/step_function_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1445 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/web_socket_api_gateway_generator.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14499 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/lambda_function.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4642 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/project.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2023 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/generators/tests.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.875956 aws-syndicate-1.9.6/syndicate/core/groups/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      697 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/groups/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8240 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/groups/generate.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    41096 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/groups/meta.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1701 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/groups/tags.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    35179 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/handlers.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21811 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/helper.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.875956 aws-syndicate-1.9.6/syndicate/core/project_state/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      602 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/project_state/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17715 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/project_state/project_state.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6922 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/project_state/status_processor.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2169 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/project_state/sync_processor.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.883956 aws-syndicate-1.9.6/syndicate/core/resources/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2546 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/abstract_external_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40873 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/api_gateway_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1649 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/base_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8094 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/batch_compenv_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4130 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/batch_jobdef_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3074 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/batch_jobqueue_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3673 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/cloud_watch_alarm_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7850 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/cloud_watch_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4207 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/cognito_identity_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7131 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/cognito_user_pool_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4083 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/dax_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4470 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/docdb_cluster_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3380 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/docdb_instance_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17302 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/dynamo_db_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9744 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/ebs_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8121 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/ec2_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5800 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/eventbridge_scheduler_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2921 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/firehose_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4042 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/group_tagging_api_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6208 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/helper.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14761 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/iam_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2880 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/kinesis_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    46532 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/lambda_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12784 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/processors_mapping.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13837 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/resources_provider.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7281 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/s3_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12204 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/sns_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6501 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/sqs_resource.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9113 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/resources/step_functions_resource.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.883956 aws-syndicate-1.9.6/syndicate/core/transform/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5061 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/build_meta_transformer.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.883956 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2711 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/cf_transform_utils.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6113 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/cloudformation_transformer.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.887956 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      603 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23992 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_api_gateway_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4239 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_batch_compenv_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4594 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_batch_job_defeinition.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1762 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_batch_job_queue_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1888 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_alarm_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4120 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_rule_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2506 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_cognito_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9892 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_dynamodb_table_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1086 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_iam_managed_policy_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4371 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_iam_role_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1173 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_kinesis_stream_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17045 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_lambda_function_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1637 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_lambda_layer_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1065 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_resource_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6121 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_s3_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1009 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_sns_application_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3537 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_sns_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4533 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_sqs_converter.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.891956 aws-syndicate-1.9.6/syndicate/core/transform/terraform/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/__init__.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:58:08.895956 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    29869 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_api_gateway_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6856 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_batch_compenv_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3101 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_batch_jobdef_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2009 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_batch_jobqueue_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3327 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_cloud_watch_alram_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4378 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_cloud_watch_rule_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3866 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_cognito_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12327 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_dynamo_db_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1291 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_iam_policy_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3093 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_iam_role_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1260 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_kinesis_stream_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    24116 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_lambda_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2544 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_lambda_layer_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1058 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_resource_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3297 2024-01-08 13:57:16.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_s3_bucket_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1918 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_sns_app_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5408 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_sns_topic_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9561 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_sqs_converter.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19233 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/terraform_template.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7241 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/terraform_transformer.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1543 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/tf_helper.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      884 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/tf_resource_name_builder.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4335 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/terraform/tf_resource_reference_builder.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2603 2024-01-08 13:57:17.000000 aws-syndicate-1.9.6/syndicate/core/transform/transform_processor.py
```

### Comparing `aws-syndicate-1.9.4/LICENSE` & `aws-syndicate-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/PKG-INFO` & `aws-syndicate-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-syndicate
-Version: 1.9.4
+Version: 1.9.6
 Summary: AWS-syndicate is an Amazon Web Services deployment framework written in Python, which allows to easily deploy serverless applications using resource descriptions.
 Home-page: https://github.com/epam/aws-syndicate
 Author: EPAM Systems
 Author-email: support@syndicate.team
 Keywords: AWS,SERVERLESS,CLOUD,LAMBDA,DEPLOY
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==7.1.2
 Requires-Dist: botocore==1.29.80
 Requires-Dist: boto3==1.26.80
-Requires-Dist: configobj==5.0.8
 Requires-Dist: tqdm==4.65.2
 Requires-Dist: colorama==0.4.5
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests-aws-sign==0.1.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: troposphere==4.1.0
```

### Comparing `aws-syndicate-1.9.4/README.md` & `aws-syndicate-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/aws_syndicate.egg-info/PKG-INFO` & `aws-syndicate-1.9.6/aws_syndicate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-syndicate
-Version: 1.9.4
+Version: 1.9.6
 Summary: AWS-syndicate is an Amazon Web Services deployment framework written in Python, which allows to easily deploy serverless applications using resource descriptions.
 Home-page: https://github.com/epam/aws-syndicate
 Author: EPAM Systems
 Author-email: support@syndicate.team
 Keywords: AWS,SERVERLESS,CLOUD,LAMBDA,DEPLOY
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==7.1.2
 Requires-Dist: botocore==1.29.80
 Requires-Dist: boto3==1.26.80
-Requires-Dist: configobj==5.0.8
 Requires-Dist: tqdm==4.65.2
 Requires-Dist: colorama==0.4.5
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests-aws-sign==0.1.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: troposphere==4.1.0
```

### Comparing `aws-syndicate-1.9.4/aws_syndicate.egg-info/SOURCES.txt` & `aws-syndicate-1.9.6/aws_syndicate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/setup.py` & `aws-syndicate-1.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='aws-syndicate',
-    version='1.9.4',
+    version='1.9.6',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'click==7.1.2',
         'botocore==1.29.80',
         'boto3==1.26.80',
-        'configobj==5.0.8',
         'tqdm==4.65.2',
         'colorama==0.4.5',
         'pyyaml==6.0.1',
         'requests-aws-sign==0.1.6',
         'requests==2.31.0',
         'tabulate==0.9.0',
         'troposphere==4.1.0'
```

### Comparing `aws-syndicate-1.9.4/syndicate/__init__.py` & `aws-syndicate-1.9.6/syndicate/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/commons/__init__.py` & `aws-syndicate-1.9.6/syndicate/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/commons/log_helper.py` & `aws-syndicate-1.9.6/syndicate/commons/log_helper.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/__init__.py` & `aws-syndicate-1.9.6/syndicate/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/api_gateway_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/api_gateway_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/application_autoscaling_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/application_autoscaling_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/batch_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/batch_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/cloud_watch_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/cloud_watch_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/cloudfront_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/cloudfront_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/cognito_identity_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/cognito_identity_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/cognito_identity_provider_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/cognito_identity_provider_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/dax_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/dax_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/documentdb_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/documentdb_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/dynamo_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/dynamo_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/ec2_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/ec2_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/elastic_beanstalk_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/elastic_beanstalk_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/eventbridge_scheduler_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/eventbridge_scheduler_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/firehose_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/firehose_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/helper.py` & `aws-syndicate-1.9.6/syndicate/connection/helper.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/iam_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/iam_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/kinesis_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/kinesis_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/kms_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/kms_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/lambda_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/lambda_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/resource_groups_tagging_api_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/resource_groups_tagging_api_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/s3_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/s3_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/ses_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/ses_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/sns_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/sns_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/sqs_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/sqs_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/step_functions_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/step_functions_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/connection/sts_connection.py` & `aws-syndicate-1.9.6/syndicate/connection/sts_connection.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/artifact_processor.py` & `aws-syndicate-1.9.6/syndicate/core/build/artifact_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/bundle_processor.py` & `aws-syndicate-1.9.6/syndicate/core/build/bundle_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/deployment_processor.py` & `aws-syndicate-1.9.6/syndicate/core/build/deployment_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/helper.py` & `aws-syndicate-1.9.6/syndicate/core/build/helper.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/meta_processor.py` & `aws-syndicate-1.9.6/syndicate/core/build/meta_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/profiler_processor.py` & `aws-syndicate-1.9.6/syndicate/core/build/profiler_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/runtime/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/build/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/runtime/java.py` & `aws-syndicate-1.9.6/syndicate/core/build/runtime/java.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/runtime/nodejs.py` & `aws-syndicate-1.9.6/syndicate/core/build/runtime/nodejs.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/runtime/python.py` & `aws-syndicate-1.9.6/syndicate/core/build/runtime/python.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/validator/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/build/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/validator/batch_compenv_validator.py` & `aws-syndicate-1.9.6/syndicate/core/build/validator/batch_compenv_validator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/validator/batch_jobdef_validator.py` & `aws-syndicate-1.9.6/syndicate/core/build/validator/batch_jobdef_validator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/validator/dynamodb_validator.py` & `aws-syndicate-1.9.6/syndicate/core/build/validator/dynamodb_validator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/validator/lambda_validator.py` & `aws-syndicate-1.9.6/syndicate/core/build/validator/lambda_validator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/validator/mapping.py` & `aws-syndicate-1.9.6/syndicate/core/build/validator/mapping.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/build/warmup_processor.py` & `aws-syndicate-1.9.6/syndicate/core/build/warmup_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/conf/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/conf/bucket_view.py` & `aws-syndicate-1.9.6/syndicate/core/conf/bucket_view.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/conf/generator.py` & `aws-syndicate-1.9.6/syndicate/core/conf/generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/conf/processor.py` & `aws-syndicate-1.9.6/syndicate/core/conf/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,121 +10,59 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 import os
+from configparser import ConfigParser
+from datetime import datetime
+from typing import Union
 
 import yaml
-from configobj import ConfigObj
-from validate import Validator, VdtTypeError
 
 from syndicate.commons.log_helper import get_logger
+from syndicate.core.conf.bucket_view import \
+    AbstractBucketView, AbstractViewDigest
 from syndicate.core.conf.validator import \
     (PROJECT_PATH_CFG, REGION_CFG, DEPLOY_TARGET_BUCKET_CFG,
      ACCOUNT_ID_CFG, PROJECTS_MAPPING_CFG, AWS_ACCESS_KEY_ID_CFG,
      RESOURCES_PREFIX_CFG, RESOURCES_SUFFIX_CFG, AWS_SECRET_ACCESS_KEY_CFG,
      ALL_REGIONS, ALLOWED_RUNTIME_LANGUAGES, ConfigValidator,
      USE_TEMP_CREDS_CFG, SERIAL_NUMBER_CFG,
      TEMP_AWS_ACCESS_KEY_ID_CFG, TEMP_AWS_SECRET_ACCESS_KEY_CFG,
      TEMP_AWS_SESSION_TOKEN_CFG, EXPIRATION_CFG, TAGS_CFG,
      IAM_PERMISSIONS_BOUNDARY_CFG, LAMBDAS_ALIASES_NAME_CFG,
      AWS_SESSION_TOKEN_CFG, EXTENDED_PREFIX_MODE_CFG)
 from syndicate.core.constants import (DEFAULT_SEP, IAM_POLICY, IAM_ROLE,
                                       S3_BUCKET_TYPE)
 
-from syndicate.core.conf.bucket_view import \
-    AbstractBucketView, AbstractViewDigest
-from typing import Union
-
 CONFIG_FILE_NAME = 'syndicate.yml'
 ALIASES_FILE_NAME = 'syndicate_aliases.yml'
 
 LEGACY_CONFIG_FILE_NAME = 'sdct.conf'
 LEGACY_ALIASES_FILE_NAME = 'sdct_aliases.conf'
-DEFAULT_SECTION_NAME = 'default'
 
 _LOG = get_logger('core.conf.config_holder')
 
 GLOBAL_AWS_SERVICES = {IAM_ROLE, IAM_POLICY, S3_BUCKET_TYPE}
 
-REQUIRED_PARAMETERS = {
-    PROJECT_PATH_CFG: 'string(min=1)',
-    REGION_CFG: "region_func",
-    DEPLOY_TARGET_BUCKET_CFG: 'string(min=3, max=63)',
-    ACCOUNT_ID_CFG: 'account_func',
-    PROJECTS_MAPPING_CFG: 'project_func'
-}
-
-ALL_CONFIG_PARAMETERS = [
-    AWS_ACCESS_KEY_ID_CFG, AWS_SECRET_ACCESS_KEY_CFG,
-    RESOURCES_PREFIX_CFG, RESOURCES_SUFFIX_CFG,
-    TEMP_AWS_ACCESS_KEY_ID_CFG, TEMP_AWS_SECRET_ACCESS_KEY_CFG,
-    TEMP_AWS_SESSION_TOKEN_CFG, EXPIRATION_CFG
-]
-ALL_CONFIG_PARAMETERS.extend(REQUIRED_PARAMETERS.keys())
-
-ERROR_MESSAGE_MAPPING = {
-    PROJECT_PATH_CFG: 'cannot be empty',
-    REGION_CFG: "is invalid. Valid options: " + str(ALL_REGIONS),
-    DEPLOY_TARGET_BUCKET_CFG: 'length must be between 3 and 63 characters',
-    ACCOUNT_ID_CFG: 'must be 12-digit number',
-    PROJECTS_MAPPING_CFG: "must be as a mapping of runtime language to "
-                          "project path. Allowed runtime language values: "
-                          + str(ALLOWED_RUNTIME_LANGUAGES),
-    RESOURCES_PREFIX_CFG: 'length must be less than or equal to 5',
-    RESOURCES_SUFFIX_CFG: 'length must be less than or equal to 5'
-}
-
-
-def _region(value):
-    value = value.lower()
-    if not isinstance(value, str):
-        raise VdtTypeError(value)
-    if value not in ALL_REGIONS:
-        raise VdtTypeError(value)
-    return value
-
-
-def _account(value):
-    if len(value) != 12:
-        raise VdtTypeError(value)
-    try:
-        int(value)
-    except:
-        raise VdtTypeError(value)
-    return value
-
-
-def _project_mapping(value):
-    if value is '' or None:
-        return ''  # valid case if you have no projects to build
-    mappings = value.split(';')
-    for mapping in mappings:
-        items = mapping.split(':')
-        if len(items) != 2:
-            raise VdtTypeError(value)
-        if items[0] not in ALLOWED_RUNTIME_LANGUAGES:
-            raise VdtTypeError(value)
-    return value
-
 
 class ConfigHolder:
     def __init__(self, dir_path):
         con_path_yml = os.path.join(dir_path, CONFIG_FILE_NAME)
         con_path_yaml = os.path.join(dir_path,
                                      CONFIG_FILE_NAME.replace('yml', 'yaml'))
         con_path = con_path_yml if \
             os.path.exists(con_path_yml) else con_path_yaml
         self._config_path = con_path
         if os.path.isfile(con_path):
             self._init_yaml_config(dir_path=dir_path, con_path=con_path)
         else:
-            self._init_ini_config(dir_path=dir_path)
+            self._init_conf_config(dir_path=dir_path)
 
     def _assert_no_errors(self, errors: list):
         if errors:
             raise AssertionError(f'The following error occurred '
                                  f'while {self._config_path} '
                                  f'parsing: {errors}')
 
@@ -142,30 +80,34 @@
             dir_path, ALIASES_FILE_NAME.replace('yml', 'yaml'))
         aliases_path = aliases_path_yml \
             if os.path.exists(aliases_path_yml) else aliases_path_yaml
         aliases_content = load_yaml_file_content(file_path=aliases_path)
         self._aliases = aliases_content
         self._aliases.update(self.default_aliases)
 
-    def _init_ini_config(self, dir_path):
+    def _init_conf_config(self, dir_path):
         con_path = os.path.join(dir_path, LEGACY_CONFIG_FILE_NAME)
         if not os.path.isfile(con_path):
             raise AssertionError(
                 'sdct.conf does not exist inside %s folder' % dir_path)
+
         self._config_path = con_path
-        self._config_dict = ConfigObj(con_path,
-                                      configspec=REQUIRED_PARAMETERS)
-        self._validate_ini()
+        self._config_dict = load_conf_file_content(self._config_path)
+
+        validator = ConfigValidator(self._config_dict)
+        errors = validator.validate()
+        self._assert_no_errors(errors)
+
         alias_path = os.path.join(dir_path, LEGACY_ALIASES_FILE_NAME)
         if not os.path.exists(alias_path):
             _LOG.warn('sdct_aliases.conf does not exist '
                       'inside %s folder' % dir_path)
-        else:
-            self._aliases = ConfigObj(alias_path)
-            self._aliases.update(self.default_aliases)
+
+        self._aliases = load_conf_file_content(alias_path)
+        self._aliases.update(self.default_aliases)
 
     def set_temp_credentials_to_config(self, temp_aws_access_key_id,
                                        temp_aws_secret_access_key,
                                        temp_aws_session_token,
                                        expiration):
         content_to_update = {
             TEMP_AWS_ACCESS_KEY_ID_CFG: temp_aws_access_key_id,
@@ -174,55 +116,14 @@
             EXPIRATION_CFG: expiration
         }
         update_file_content(
             file_path=self._config_path,
             content=content_to_update
         )
 
-    def _validate_ini(self):
-        # building a validator
-        validator = Validator({
-            'region_func': _region,
-            'account_func': _account,
-            'project_func': _project_mapping
-        })
-        # validate
-        param_valid_dict = self._config_dict.validate(validator=validator)
-        if not param_valid_dict:
-            raise Exception(f'Error while parsing {self._config_path}')
-        # check non-required parameters
-        prefix_value = self._config_dict.get(RESOURCES_PREFIX_CFG)
-        if prefix_value:
-            if len(prefix_value) > 5:
-                if not isinstance(param_valid_dict, dict):
-                    param_valid_dict = {RESOURCES_PREFIX_CFG: False}
-                else:
-                    param_valid_dict[RESOURCES_PREFIX_CFG] = False
-
-        suffix_value = self._config_dict.get(RESOURCES_SUFFIX_CFG)
-        if suffix_value:
-            if len(suffix_value) > 5:
-                if not isinstance(param_valid_dict, dict):
-                    param_valid_dict = {RESOURCES_SUFFIX_CFG: False}
-                else:
-                    param_valid_dict[RESOURCES_SUFFIX_CFG] = False
-
-        # processing results
-        if isinstance(param_valid_dict, dict):
-            messages = ''
-            for key, value in param_valid_dict.items():
-                if not value:
-                    messages += '\n{0} {1}'.format(key,
-                                                   ERROR_MESSAGE_MAPPING[key])
-
-            if messages:
-                raise Exception('Configuration is invalid. ' + messages)
-        tags = self._config_dict.get(TAGS_CFG) or {}
-        self._assert_no_errors(ConfigValidator.validate_tags(TAGS_CFG, tags))
-
     def _resolve_variable(self, variable_name):
         return self._config_dict.get(variable_name)
 
     def _resolve_aliases(self, variable_name):
         return self._aliases.get(variable_name)
 
     def _prepare_bucket_view(self) -> Union[None, AbstractBucketView]:
@@ -245,15 +146,16 @@
             _LOG.warn('No viewing complement has been found.')
         except AbstractBucketView.BucketViewRuntimeError:
             _LOG.warn('Viewing complement set-up has failed.')
 
         del self.deploy_target_bucket_view
         return None
 
-    def _resolve_bucket_view_attribute(self, attribute_name: str, default=None):
+    def _resolve_bucket_view_attribute(self, attribute_name: str,
+                                       default=None):
         """
         Retrieves bucket view value respectively to a provided attribute name.
         """
         if not isinstance(attribute_name, str):
             raise KeyError('Name of an attribute must be a string.')
         view = self.deploy_target_bucket_view
         if view and not view.raw:
@@ -434,32 +336,97 @@
         return False
 
 
 def path_resolver(path):
     return path.replace('\\', DEFAULT_SEP).replace('//', DEFAULT_SEP)
 
 
+def str_to_bool(val):
+    if isinstance(val, str):
+        if val.lower() == 'true':
+            return True
+        elif val.lower() == 'false':
+            return False
+    return val
+
+
+def str_to_datetime(val):
+    if isinstance(val, str):
+        if ' ' in val:
+            val = val.replace(' ', 'T')
+        return datetime.fromisoformat(val)
+    return val
+
+
+def add_default_section(file_path):
+    with open(file_path, 'r+') as f:
+        lines = f.readlines()
+        lines = [line for line in lines if line.strip() != '']
+
+        first_line = lines[0]
+        f.seek(0)
+        if '[default]' not in first_line:
+            rest_of_file = f.read()
+            f.seek(0)
+            f.write('[default]\n' + rest_of_file)
+
+
 def load_yaml_file_content(file_path):
     if not os.path.isfile(file_path):
         raise AssertionError(f'There is no file by path: {file_path}')
     with open(file_path, 'r') as yaml_file:
         return yaml.load(yaml_file, Loader=yaml.FullLoader)
 
 
+def load_conf_file_content(file_path):
+    if not os.path.isfile(file_path):
+        raise AssertionError(f'There is no file by path: {file_path}')
+
+    add_default_section(file_path)
+
+    config = ConfigParser()
+    config.read(file_path)
+    config_dict = {}
+
+    for section in config.sections():
+        if section == 'tags':
+            config_dict[section] = dict(config[section])
+        else:
+            section_dict = {
+                k: str_to_bool(v) if k != 'expiration' else str_to_datetime(v)
+                for k, v in dict(config[section]).items()}
+            config_dict.update(section_dict)
+
+    return config_dict
+
+
 def update_file_content(file_path, content):
     if file_path.endswith('.yaml') or file_path.endswith('.yml'):
         update_yaml_file_content(file_path=file_path, content=content)
     elif file_path.endswith('.conf'):
-        update_ini_file_content(file_path=file_path, content=content)
+        update_conf_file_content(file_path=file_path, content=content)
 
 
 def update_yaml_file_content(file_path, content):
     file_content = load_yaml_file_content(file_path=file_path)
     file_content.update(content)
     with open(file_path, 'w') as yaml_file:
         yaml.dump(file_content, yaml_file, default_flow_style=False)
 
 
-def update_ini_file_content(file_path, content):
-    config = ConfigObj(file_path, configspec=REQUIRED_PARAMETERS)
-    config.update(content)
-    config.write()
+def update_conf_file_content(file_path, content):
+    file_content = load_conf_file_content(file_path)
+    file_content.update(content)
+
+    config = ConfigParser()
+    for key, val in file_content.items():
+        if type(val) is dict:
+            config.add_section(key)
+            for sub_key, sub_val in val.items():
+                config.set(key, sub_key, str(sub_val))
+        else:
+            if not config.has_section('default'):
+                config.add_section('default')
+            config.set('default', key, str(val))
+
+    with open(file_path, 'w') as f:
+        config.write(f)
```

### Comparing `aws-syndicate-1.9.4/syndicate/core/conf/validator.py` & `aws-syndicate-1.9.6/syndicate/core/conf/validator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/constants.py` & `aws-syndicate-1.9.6/syndicate/core/constants.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/decorators.py` & `aws-syndicate-1.9.6/syndicate/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/contents.py` & `aws-syndicate-1.9.6/syndicate/core/generators/contents.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/api_gateway_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/api_gateway_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/base_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/base_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/batch_compenv_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/batch_compenv_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/batch_jobdef_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/batch_jobdef_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/batch_jobqueue_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/batch_jobqueue_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cloudwatch_alarm_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cloudwatch_alarm_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cloudwatch_event_rule_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cloudwatch_event_rule_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/cognito_user_pool_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/cognito_user_pool_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/dax_cluster_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/dax_cluster_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/docdb_cluster_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/docdb_cluster_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/docdb_instance_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/docdb_instance_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/dynamodb_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/dynamodb_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/ec2_instance_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/ec2_instance_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/iam_policy_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/iam_policy_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/iam_role_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/iam_role_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/s3_bucket_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/s3_bucket_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/sns_application_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/sns_application_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/sqs_queue_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/sqs_queue_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/step_function_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/step_function_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/deployment_resources/web_socket_api_gateway_generator.py` & `aws-syndicate-1.9.6/syndicate/core/generators/deployment_resources/web_socket_api_gateway_generator.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/lambda_function.py` & `aws-syndicate-1.9.6/syndicate/core/generators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/project.py` & `aws-syndicate-1.9.6/syndicate/core/generators/project.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/generators/tests.py` & `aws-syndicate-1.9.6/syndicate/core/generators/tests.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/groups/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/groups/generate.py` & `aws-syndicate-1.9.6/syndicate/core/groups/generate.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/groups/meta.py` & `aws-syndicate-1.9.6/syndicate/core/groups/meta.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/groups/tags.py` & `aws-syndicate-1.9.6/syndicate/core/groups/tags.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/handlers.py` & `aws-syndicate-1.9.6/syndicate/core/handlers.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/helper.py` & `aws-syndicate-1.9.6/syndicate/core/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,15 +574,15 @@
                       f"parameter: '{param.name}'")
     return value
 
 
 def check_lambda_name(value):
     """Validates lambda's name"""
     _LOG.info(f"Validating lambda name: '{value}'")
-    invalid_character = re.search('[^0-9a-zA-Z\-]', value)
+    invalid_character = re.search('[^0-9a-zA-Z\-\_]', value)
     error = None
     if not 3 <= len(value) <= 63:
         error = f'lambda name \'{value}\' length must be between 3 and 63 characters'
     elif invalid_character:
         error = f'lambda name \'{value}\' contains invalid characters: ' \
                 f'{invalid_character.group()}'
     elif value.startswith('-'):
```

### Comparing `aws-syndicate-1.9.4/syndicate/core/project_state/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/project_state/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/project_state/project_state.py` & `aws-syndicate-1.9.6/syndicate/core/project_state/project_state.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/project_state/status_processor.py` & `aws-syndicate-1.9.6/syndicate/core/project_state/status_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/project_state/sync_processor.py` & `aws-syndicate-1.9.6/syndicate/core/project_state/sync_processor.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/abstract_external_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/abstract_external_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/api_gateway_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/api_gateway_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/base_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/base_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/batch_compenv_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/batch_compenv_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/batch_jobdef_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/batch_jobdef_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/batch_jobqueue_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/batch_jobqueue_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/cloud_watch_alarm_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/cloud_watch_alarm_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/cloud_watch_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/cloud_watch_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/cognito_identity_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/cognito_identity_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/cognito_user_pool_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/cognito_user_pool_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/dax_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/dax_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/docdb_cluster_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/docdb_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/docdb_instance_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/docdb_instance_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/dynamo_db_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/dynamo_db_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/ebs_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/ebs_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/ec2_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/ec2_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/eventbridge_scheduler_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/eventbridge_scheduler_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/firehose_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/firehose_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/group_tagging_api_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/group_tagging_api_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/helper.py` & `aws-syndicate-1.9.6/syndicate/core/resources/helper.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/iam_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/iam_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/kinesis_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/kinesis_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/lambda_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/lambda_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/processors_mapping.py` & `aws-syndicate-1.9.6/syndicate/core/resources/processors_mapping.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/resources_provider.py` & `aws-syndicate-1.9.6/syndicate/core/resources/resources_provider.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/s3_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/s3_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/sns_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/sns_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/sqs_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/sqs_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/resources/step_functions_resource.py` & `aws-syndicate-1.9.6/syndicate/core/resources/step_functions_resource.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/build_meta_transformer.py` & `aws-syndicate-1.9.6/syndicate/core/transform/build_meta_transformer.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/cf_transform_utils.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/cf_transform_utils.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/cloudformation_transformer.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/cloudformation_transformer.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/__init__.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_api_gateway_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_api_gateway_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_batch_compenv_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_batch_compenv_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_batch_job_defeinition.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_batch_job_defeinition.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_batch_job_queue_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_batch_job_queue_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_alarm_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_alarm_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_rule_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_cloudwatch_rule_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_cognito_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_cognito_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_dynamodb_table_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_dynamodb_table_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_iam_managed_policy_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_iam_managed_policy_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_iam_role_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_iam_role_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_kinesis_stream_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_kinesis_stream_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_lambda_function_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_lambda_function_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_lambda_layer_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_lambda_layer_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_resource_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_resource_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_s3_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_s3_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_sns_application_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_sns_application_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_sns_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_sns_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/cloudformation/converter/cf_sqs_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/cloudformation/converter/cf_sqs_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_api_gateway_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_api_gateway_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_batch_compenv_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_batch_compenv_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_batch_jobdef_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_batch_jobdef_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_batch_jobqueue_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_batch_jobqueue_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_cloud_watch_alram_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_cloud_watch_alram_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_cloud_watch_rule_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_cloud_watch_rule_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_cognito_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_cognito_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_dynamo_db_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_dynamo_db_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_iam_policy_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_iam_policy_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_iam_role_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_iam_role_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_kinesis_stream_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_kinesis_stream_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_lambda_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_lambda_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_lambda_layer_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_lambda_layer_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_resource_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_resource_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_s3_bucket_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_s3_bucket_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_sns_app_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_sns_app_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_sns_topic_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_sns_topic_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/converter/tf_sqs_converter.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/converter/tf_sqs_converter.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/terraform_template.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/terraform_template.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/terraform_transformer.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/terraform_transformer.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/tf_helper.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/tf_helper.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/tf_resource_name_builder.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/tf_resource_name_builder.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/terraform/tf_resource_reference_builder.py` & `aws-syndicate-1.9.6/syndicate/core/transform/terraform/tf_resource_reference_builder.py`

 * *Files identical despite different names*

### Comparing `aws-syndicate-1.9.4/syndicate/core/transform/transform_processor.py` & `aws-syndicate-1.9.6/syndicate/core/transform/transform_processor.py`

 * *Files identical despite different names*

