# Comparing `tmp/ten99policy-1.0.4.tar.gz` & `tmp/ten99policy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ten99policy-1.0.4.tar", last modified: Mon Dec 26 18:22:19 2022, max compression
+gzip compressed data, was "ten99policy-1.0.5.tar", last modified: Tue Apr 16 20:16:31 2024, max compression
```

## Comparing `ten99policy-1.0.4.tar` & `ten99policy-1.0.5.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.271217 ten99policy-1.0.4/
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.249936 ten99policy-1.0.4/.circleci/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2971 2022-06-14 14:49:57.000000 ten99policy-1.0.4/.circleci/config.yml
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      386 2022-06-14 14:49:57.000000 ten99policy-1.0.4/.codeclimate.yml
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      252 2022-06-14 14:49:57.000000 ten99policy-1.0.4/.editorconfig
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      366 2022-06-16 06:33:50.000000 ten99policy-1.0.4/.flake8
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      667 2022-06-14 14:49:57.000000 ten99policy-1.0.4/.gitignore
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2022-06-16 06:45:19.000000 ten99policy-1.0.4/LICENSE
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1482 2022-12-26 18:22:19.271323 ten99policy-1.0.4/PKG-INFO
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     3469 2022-06-16 06:46:37.000000 ten99policy-1.0.4/README.md
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        6 2022-12-26 18:22:00.000000 ten99policy-1.0.4/VERSION
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.257573 ten99policy-1.0.4/examples/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1915 2022-12-25 22:04:06.000000 ten99policy-1.0.4/examples/contractors.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1889 2022-07-21 17:45:39.000000 ten99policy-1.0.4/examples/entities.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      673 2022-12-25 22:04:06.000000 ten99policy-1.0.4/examples/events.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1204 2022-11-02 16:58:51.000000 ten99policy-1.0.4/examples/insurance_application_sessions.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1718 2022-07-21 17:45:39.000000 ten99policy-1.0.4/examples/invoices.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1696 2022-07-21 17:45:39.000000 ten99policy-1.0.4/examples/jobs.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1576 2022-07-21 17:45:39.000000 ten99policy-1.0.4/examples/policies.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1311 2022-07-21 17:45:39.000000 ten99policy-1.0.4/examples/quotes.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1123 2022-12-25 22:04:06.000000 ten99policy-1.0.4/requirements.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      102 2022-12-26 18:22:19.271594 ten99policy-1.0.4/setup.cfg
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2060 2022-06-16 06:46:58.000000 ten99policy-1.0.4/setup.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.259142 ten99policy-1.0.4/ten99policy/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      476 2022-12-25 22:03:41.000000 ten99policy-1.0.4/ten99policy/__init__.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    11491 2022-12-25 22:04:11.000000 ten99policy-1.0.4/ten99policy/api_requestor.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.261973 ten99policy-1.0.4/ten99policy/api_resources/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      788 2022-12-25 22:04:11.000000 ten99policy-1.0.4/ten99policy/api_resources/__init__.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.263273 ten99policy-1.0.4/ten99policy/api_resources/abstract/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      799 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/__init__.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     3093 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      869 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2081 2022-06-16 06:33:37.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/custom_method.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      634 2022-06-16 06:33:37.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1062 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     4418 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      883 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      900 2022-06-16 06:33:37.000000 ten99policy-1.0.4/ten99policy/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-12-25 21:21:42.000000 ten99policy-1.0.4/ten99policy/api_resources/assignments.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/contractors.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/entities.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      594 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/error_object.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      138 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/events.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      264 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/insurance_application_sessions.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/invoices.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      420 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/jobs.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     5800 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/api_resources/list_object.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/policies.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      330 2022-06-16 06:30:18.000000 ten99policy-1.0.4/ten99policy/api_resources/quotes.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     3999 2022-06-16 06:45:08.000000 ten99policy-1.0.4/ten99policy/error.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    24625 2022-06-16 06:45:08.000000 ten99policy-1.0.4/ten99policy/http_client.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     2775 2022-06-16 06:30:17.000000 ten99policy-1.0.4/ten99policy/multipart_data_generator.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      570 2022-06-16 06:33:37.000000 ten99policy-1.0.4/ten99policy/object_classes.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    32463 2022-06-14 14:49:57.000000 ten99policy-1.0.4/ten99policy/six.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)    12243 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/ten99policy_object.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      998 2022-06-16 06:35:38.000000 ten99policy-1.0.4/ten99policy/ten99policy_response.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     6972 2022-12-25 22:04:06.000000 ten99policy-1.0.4/ten99policy/util.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)       18 2022-12-26 18:22:15.000000 ten99policy-1.0.4/ten99policy/version.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.260205 ten99policy-1.0.4/ten99policy.egg-info/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1482 2022-12-26 18:22:19.000000 ten99policy-1.0.4/ten99policy.egg-info/PKG-INFO
--rw-r--r--   0 cfkarakulak   (501) staff       (20)     1922 2022-12-26 18:22:19.000000 ten99policy-1.0.4/ten99policy.egg-info/SOURCES.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2022-12-26 18:22:19.000000 ten99policy-1.0.4/ten99policy.egg-info/dependency_links.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2022-08-04 07:33:51.000000 ten99policy-1.0.4/ten99policy.egg-info/not-zip-safe
--rw-r--r--   0 cfkarakulak   (501) staff       (20)       95 2022-12-26 18:22:19.000000 ten99policy-1.0.4/ten99policy.egg-info/requires.txt
--rw-r--r--   0 cfkarakulak   (501) staff       (20)       12 2022-12-26 18:22:19.000000 ten99policy-1.0.4/ten99policy.egg-info/top_level.txt
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.263410 ten99policy-1.0.4/tests/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.4/tests/__init__.py
-drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2022-12-26 18:22:19.271005 ten99policy-1.0.4/tests/api_resources/
--rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.4/tests/api_resources/__init__.py
--rw-r--r--   0 cfkarakulak   (501) staff       (20)      404 2022-06-16 06:30:17.000000 ten99policy-1.0.4/tests/api_resources/test_customer.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.163683 ten99policy-1.0.5/
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.149122 ten99policy-1.0.5/.circleci/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2971 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.circleci/config.yml
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      386 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.codeclimate.yml
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      252 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.editorconfig
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      366 2022-06-16 06:33:50.000000 ten99policy-1.0.5/.flake8
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      667 2022-06-14 14:49:57.000000 ten99policy-1.0.5/.gitignore
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2022-06-16 06:45:19.000000 ten99policy-1.0.5/LICENSE
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1584 2024-04-16 20:16:31.163595 ten99policy-1.0.5/PKG-INFO
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     3469 2022-06-16 06:46:37.000000 ten99policy-1.0.5/README.md
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        6 2024-04-16 20:15:21.000000 ten99policy-1.0.5/VERSION
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.151175 ten99policy-1.0.5/examples/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1640 2022-12-26 18:25:47.000000 ten99policy-1.0.5/examples/assignments.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      633 2024-04-16 12:38:39.000000 ten99policy-1.0.5/examples/contractors.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1889 2022-07-21 17:45:39.000000 ten99policy-1.0.5/examples/entities.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      673 2022-12-25 22:04:06.000000 ten99policy-1.0.5/examples/events.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1204 2022-11-02 16:58:51.000000 ten99policy-1.0.5/examples/insurance_application_sessions.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1718 2022-07-21 17:45:39.000000 ten99policy-1.0.5/examples/invoices.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1693 2023-03-26 18:07:20.000000 ten99policy-1.0.5/examples/jobs.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1576 2022-07-21 17:45:39.000000 ten99policy-1.0.5/examples/policies.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1331 2023-02-28 10:16:19.000000 ten99policy-1.0.5/examples/quotes.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1106 2024-04-16 12:23:08.000000 ten99policy-1.0.5/requirements.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      102 2024-04-16 20:16:31.163970 ten99policy-1.0.5/setup.cfg
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2060 2022-06-16 06:46:58.000000 ten99policy-1.0.5/setup.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.154145 ten99policy-1.0.5/ten99policy/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      476 2022-12-25 22:03:41.000000 ten99policy-1.0.5/ten99policy/__init__.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    11598 2024-04-16 12:37:14.000000 ten99policy-1.0.5/ten99policy/api_requestor.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.160902 ten99policy-1.0.5/ten99policy/api_resources/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      788 2022-12-26 18:25:47.000000 ten99policy-1.0.5/ten99policy/api_resources/__init__.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.162540 ten99policy-1.0.5/ten99policy/api_resources/abstract/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      799 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/__init__.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     3093 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      869 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2081 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/custom_method.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      634 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1062 2024-04-16 12:23:13.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     4418 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      883 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      900 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-12-26 18:25:47.000000 ten99policy-1.0.5/ten99policy/api_resources/assignments.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      434 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/contractors.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/entities.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      594 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/error_object.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      138 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/events.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      264 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/insurance_application_sessions.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/invoices.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      420 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/jobs.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     5800 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/api_resources/list_object.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      428 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/policies.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      330 2022-06-16 06:30:18.000000 ten99policy-1.0.5/ten99policy/api_resources/quotes.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     3999 2022-06-16 06:45:08.000000 ten99policy-1.0.5/ten99policy/error.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    24625 2022-06-16 06:45:08.000000 ten99policy-1.0.5/ten99policy/http_client.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     2775 2022-06-16 06:30:17.000000 ten99policy-1.0.5/ten99policy/multipart_data_generator.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      570 2022-06-16 06:33:37.000000 ten99policy-1.0.5/ten99policy/object_classes.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    32463 2022-06-14 14:49:57.000000 ten99policy-1.0.5/ten99policy/six.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)    12243 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/ten99policy_object.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      998 2022-06-16 06:35:38.000000 ten99policy-1.0.5/ten99policy/ten99policy_response.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     6972 2022-12-25 22:04:06.000000 ten99policy-1.0.5/ten99policy/util.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)       18 2024-04-16 20:15:33.000000 ten99policy-1.0.5/ten99policy/version.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.163240 ten99policy-1.0.5/ten99policy.egg-info/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1584 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/PKG-INFO
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)     1946 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/SOURCES.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/dependency_links.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        1 2022-08-04 07:33:51.000000 ten99policy-1.0.5/ten99policy.egg-info/not-zip-safe
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)       95 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/requires.txt
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)       12 2024-04-16 20:16:31.000000 ten99policy-1.0.5/ten99policy.egg-info/top_level.txt
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.162779 ten99policy-1.0.5/tests/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.5/tests/__init__.py
+drwxr-xr-x   0 cfkarakulak   (501) staff       (20)        0 2024-04-16 20:16:31.163018 ten99policy-1.0.5/tests/api_resources/
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)        0 2022-06-14 14:49:57.000000 ten99policy-1.0.5/tests/api_resources/__init__.py
+-rw-r--r--   0 cfkarakulak   (501) staff       (20)      404 2022-06-16 06:30:17.000000 ten99policy-1.0.5/tests/api_resources/test_customer.py
```

### Comparing `ten99policy-1.0.4/.circleci/config.yml` & `ten99policy-1.0.5/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/.gitignore` & `ten99policy-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/LICENSE` & `ten99policy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/PKG-INFO` & `ten99policy-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: ten99policy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python bindings for the ten99policy API
 Home-page: https://github.com/1099policy/1099policy-client-python
 Author: Ray Ventura
 Author-email: support@1099policy.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/1099policy/1099policy-client-python/issues
 Project-URL: Documentation, https://1099policy.com/docs/api/?lang=python
 Project-URL: Source Code, https://github.com/1099policy/1099policy-client-python
-Description: UNKNOWN
 Keywords: ten99policy api insurance
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -26,7 +24,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests>=2.20; python_version >= "3.0"
+Requires-Dist: requests[security]>=2.20; python_version < "3.0"
```

### Comparing `ten99policy-1.0.4/README.md` & `ten99policy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/examples/entities.py` & `ten99policy-1.0.5/examples/entities.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/examples/events.py` & `ten99policy-1.0.5/examples/events.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/examples/insurance_application_sessions.py` & `ten99policy-1.0.5/examples/insurance_application_sessions.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/examples/invoices.py` & `ten99policy-1.0.5/examples/invoices.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/examples/jobs.py` & `ten99policy-1.0.5/examples/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 resource = ten99policy.Jobs.create(
     name="Truck driver",
     description="Requires a truck",
     duration_hours=20,
     wage=100,
     years_experience=20,
     wage_type="flatfee",
-    entity_id="en_FwZfQRe4aW",
+    entity="en_FwZfQRe4aW",
     category_code="jc_MTqpkbkp6G"
 )
 
 # -----------------------------------------------------------------------------------*/
 # Updating a job (replace xxx with an existing job id)
 #-----------------------------------------------------------------------------------*/
```

### Comparing `ten99policy-1.0.4/examples/policies.py` & `ten99policy-1.0.5/examples/policies.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/examples/quotes.py` & `ten99policy-1.0.5/examples/quotes.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -----------------------------------------------------------------------------------*/
 # Creating a quote
 #-----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Quotes.create(
     job_id="jb_jsb9KEcTpc",
     contractor_id="cn_yJBbMeq9QA",
-    coverage_type="general"
+    coverage_type=["general", "workers-comp"],
 )
 
 # -----------------------------------------------------------------------------------*/
 # Updating a quote (replace xxx with an existing quote id)
 #-----------------------------------------------------------------------------------*/
 
 resource = ten99policy.Quotes.modify('qt_C9Z2DmfHSF',
@@ -27,8 +27,8 @@
 
 resource = ten99policy.Quotes.list()
 
 # -----------------------------------------------------------------------------------*/
 # Retrieving a quote (replace xxx with an existing quote id)
 #-----------------------------------------------------------------------------------*/
 
-resource = ten99policy.Quotes.retrieve('qt_C9Z2DmfHSF')
+resource = ten99policy.Quotes.retrieve('qt_C9Z2DmfHSF')
```

### Comparing `ten99policy-1.0.4/requirements.txt` & `ten99policy-1.0.5/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 clikit==0.6.2
 colorama==0.4.4
 coverage==6.3
 crashtest==0.3.1
 cryptography==37.0.2
 distlib==0.3.4
 docutils==0.16
-dotty-dict==1.3.0
+dotty_dict==1.3.0
 exceptionite==2.2.5
 filelock==3.7.0
 hashids==1.3.1
 hfilesize==0.1.0
 hupper==1.10.3
 idna==3.3
 inflection==0.5.1
 iniconfig==1.1.1
 Jinja2==3.1.2
 jmespath==1.0.1
 MarkupSafe==2.1.1
-masonite==4.13.0
 mock==4.0.3
 mypy-extensions==0.4.3
 packaging==21.3
 pastel==0.2.1
 pathspec==0.9.0
 pbr==5.9.0
 pendulum==2.1.2
@@ -43,15 +42,15 @@
 PyJWT==2.4.0
 pylev==1.4.0
 pyparsing==3.0.7
 pytest==6.2.5
 python-dateutil==2.8.2
 python-dotenv==0.15.0
 pytzdata==2020.1
-PyYAML==5.4.1
+PyYAML==5.3.1
 requests==2.27.1
 requests-file==1.5.1
 rsa==4.7.2
 s3transfer==0.6.0
 setuptools-scm==6.4.2
 six==1.16.0
 stevedore==3.5.0
```

### Comparing `ten99policy-1.0.4/setup.py` & `ten99policy-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_requestor.py` & `ten99policy-1.0.5/ten99policy/api_requestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import calendar
 import datetime
 import json
 import platform
 import time
 import uuid
 import warnings
+import urllib.parse
 from collections import OrderedDict
 
 import ten99policy
 from ten99policy import error, http_client, version, util, six
 from ten99policy.multipart_data_generator import MultipartDataGenerator
 from ten99policy.six.moves.urllib.parse import urlsplit, urlunsplit
 from ten99policy.ten99policy_response import Ten99PolicyResponse, Ten99PolicyStreamResponse
@@ -53,19 +54,19 @@
                 yield (subkey, subvalue)
         elif isinstance(value, datetime.datetime):
             yield (key, _encode_datetime(value))
         else:
             yield (key, util.utf8(value))
 
 
-def _build_api_url(url, query):
+def _build_api_url(url, query, query_string=None):
     scheme, netloc, path, base_query, fragment = urlsplit(url)
 
-    if base_query:
-        query = "%s&%s" % (base_query, query)
+    if base_query and query_string:
+        query = "%s&%s" % (base_query, query_string)
 
     return urlunsplit((scheme, netloc, path, query, fragment))
 
 
 class APIRequestor(object):
     def __init__(
         self,
@@ -222,15 +223,16 @@
         # encoded_params = json.dumps(dict(_api_encode(params or {})))
         # encoded_params = encoded_params.replace("%5B", "[").replace("%5D", "]")
 
         encoded_params = json.dumps(params)
 
         if method == "get" or method == "delete":
             if params:
-                abs_url = _build_api_url(abs_url, encoded_params)
+                data = urllib.parse.urlencode(params)
+                abs_url = _build_api_url(abs_url, data)
             post_data = None
         elif method == "post" or method == "put" or method == "patch":
             if (
                 supplied_headers is not None
                 and supplied_headers.get("Content-Type")
                 == "multipart/form-data"
             ):
```

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/__init__.py` & `ten99policy-1.0.5/ten99policy/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/__init__.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/api_resource.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/createable_api_resource.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/custom_method.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/deletable_api_resource.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/listable_api_resource.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/nested_resource_class_methods.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/singleton_api_resource.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/abstract/updateable_api_resource.py` & `ten99policy-1.0.5/ten99policy/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/error_object.py` & `ten99policy-1.0.5/ten99policy/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/api_resources/list_object.py` & `ten99policy-1.0.5/ten99policy/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/error.py` & `ten99policy-1.0.5/ten99policy/error.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/http_client.py` & `ten99policy-1.0.5/ten99policy/http_client.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/multipart_data_generator.py` & `ten99policy-1.0.5/ten99policy/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/object_classes.py` & `ten99policy-1.0.5/ten99policy/object_classes.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/six.py` & `ten99policy-1.0.5/ten99policy/six.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/ten99policy_object.py` & `ten99policy-1.0.5/ten99policy/ten99policy_object.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/ten99policy_response.py` & `ten99policy-1.0.5/ten99policy/ten99policy_response.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy/util.py` & `ten99policy-1.0.5/ten99policy/util.py`

 * *Files identical despite different names*

### Comparing `ten99policy-1.0.4/ten99policy.egg-info/PKG-INFO` & `ten99policy-1.0.5/ten99policy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: ten99policy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python bindings for the ten99policy API
 Home-page: https://github.com/1099policy/1099policy-client-python
 Author: Ray Ventura
 Author-email: support@1099policy.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/1099policy/1099policy-client-python/issues
 Project-URL: Documentation, https://1099policy.com/docs/api/?lang=python
 Project-URL: Source Code, https://github.com/1099policy/1099policy-client-python
-Description: UNKNOWN
 Keywords: ten99policy api insurance
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -26,7 +24,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests>=2.20; python_version >= "3.0"
+Requires-Dist: requests[security]>=2.20; python_version < "3.0"
```

### Comparing `ten99policy-1.0.4/ten99policy.egg-info/SOURCES.txt` & `ten99policy-1.0.5/ten99policy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 LICENSE
 README.md
 VERSION
 requirements.txt
 setup.cfg
 setup.py
 .circleci/config.yml
+examples/assignments.py
 examples/contractors.py
 examples/entities.py
 examples/events.py
 examples/insurance_application_sessions.py
 examples/invoices.py
 examples/jobs.py
 examples/policies.py
```

