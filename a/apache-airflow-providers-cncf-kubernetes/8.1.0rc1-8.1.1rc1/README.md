# Comparing `tmp/apache_airflow_providers_cncf_kubernetes-8.1.0rc1.tar.gz` & `tmp/apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.1.0rc1.tar", last modified: Tue Apr  9 12:20:31 2024, max compression
+gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar", last modified: Tue Apr 16 07:37:35 2024, max compression
```

## Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1.tar` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3341 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/LICENSE
--rw-r--r--   0        0        0     1590 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
--rw-r--r--   0        0        0     4094 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/callbacks.py
--rw-r--r--   0        0        0      787 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0        0        0     5780 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0        0        0      787 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
--rw-r--r--   0        0        0    34132 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
--rw-r--r--   0        0        0     1673 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
--rw-r--r--   0        0        0    23564 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
--rw-r--r--   0        0        0    10014 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
--rw-r--r--   0        0        0    17733 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0        0        0    31558 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0        0        0     2101 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py
--rw-r--r--   0        0        0     5329 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kube_client.py
--rw-r--r--   0        0        0     5225 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kube_config.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
--rw-r--r--   0        0        0     2567 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
--rw-r--r--   0        0        0     6410 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
--rw-r--r--   0        0        0      787 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0        0        0    15370 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
--rw-r--r--   0        0        0    21432 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/job.py
--rw-r--r--   0        0        0     1269 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0        0        0    50239 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0        0        0     7151 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0        0        0    13262 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0        0        0    24490 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py
--rw-r--r--   0        0        0    11994 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0        0        0    12009 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
--rw-r--r--   0        0        0     2256 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
--rw-r--r--   0        0        0     2442 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
--rw-r--r--   0        0        0     3020 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
--rw-r--r--   0        0        0     1741 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0        0        0     3460 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
--rw-r--r--   0        0        0     1873 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
--rw-r--r--   0        0        0     1464 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
--rw-r--r--   0        0        0     1494 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
--rw-r--r--   0        0        0     5209 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/secret.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0        0        0     5552 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
--rw-r--r--   0        0        0     2968 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py
--rw-r--r--   0        0        0      785 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py
--rw-r--r--   0        0        0     1266 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0        0        0    13519 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
--rw-r--r--   0        0        0      863 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0        0        0     5195 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0        0        0     1928 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
--rw-r--r--   0        0        0    33322 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0        0        0     2519 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
--rw-r--r--   0        0        0     3178 2024-04-09 12:20:31.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3341 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/LICENSE
+-rw-r--r--   0        0        0     1590 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0        0        0     3967 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+-rw-r--r--   0        0        0     4094 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/callbacks.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0        0        0     5780 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0        0        0    34132 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0        0        0     1673 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0        0        0    23564 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0        0        0    10014 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0        0        0    17754 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0        0        0    31558 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0        0        0     2101 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0        0        0     5329 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0        0        0     5225 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_config.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0        0        0     2567 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
+-rw-r--r--   0        0        0     6410 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0        0        0    15370 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
+-rw-r--r--   0        0        0    21432 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/job.py
+-rw-r--r--   0        0        0     1269 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0    50268 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0        0        0     7151 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0        0        0    13262 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0        0        0    24490 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0        0        0    11994 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0        0        0    12009 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0        0        0     2256 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
+-rw-r--r--   0        0        0     2442 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
+-rw-r--r--   0        0        0     3020 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
+-rw-r--r--   0        0        0     1741 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0        0        0     3460 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
+-rw-r--r--   0        0        0     1873 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
+-rw-r--r--   0        0        0     1464 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
+-rw-r--r--   0        0        0     1494 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
+-rw-r--r--   0        0        0     5209 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/secret.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0        0        0     5552 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0        0        0     2968 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/job.py
+-rw-r--r--   0        0        0     1266 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0        0        0    13519 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+-rw-r--r--   0        0        0      863 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0        0        0     5195 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0        0        0     1928 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
+-rw-r--r--   0        0        0    33444 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0        0        0     2519 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+-rw-r--r--   0        0        0     3178 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/README.rst` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.1.0.rc1``
+Release: ``8.1.1.rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
@@ -78,8 +78,8 @@
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=28.1.0,<=29.0.0``
 ``kubernetes_asyncio``  ``>=28.1.0,<=29.0.0``
 ``google-re2``          ``>=1.0``
 ======================  =====================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/LICENSE` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "8.1.0"
+__version__ = "8.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/callbacks.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/callbacks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1712665231,
+        "source-date-epoch": 1713253055,
         "versions": [
+            "8.1.1",
             "8.1.0",
             "8.0.1",
             "8.0.0",
             "7.14.0",
             "7.13.0",
             "7.12.0",
             "7.11.0",
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kube_client.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kube_config.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/job.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,15 +787,16 @@
                 pod=pod,
                 container_name=self.base_container_name,
                 follow=follow,
                 since_seconds=since_seconds,
             )
             for raw_line in logs:
                 line = raw_line.decode("utf-8", errors="backslashreplace").rstrip("\n")
-                self.log.info("Container logs: %s", line)
+                if line:
+                    self.log.info("Container logs: %s", line)
         except HTTPError as e:
             self.log.warning(
                 "Reading of logs interrupted with error %r; will retry. "
                 "Set log level to DEBUG for traceback.",
                 e,
             )
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,16 @@
                                 for line in progress_callback_lines:
                                     if self._progress_callback:
                                         self._progress_callback(line)
                                     if self._callbacks:
                                         self._callbacks.progress_callback(
                                             line=line, client=self._client, mode=ExecutionMode.SYNC
                                         )
-                                self.log.info("[%s] %s", container_name, message_to_log)
+                                if message_to_log is not None:
+                                    self.log.info("[%s] %s", container_name, message_to_log)
                                 last_captured_timestamp = message_timestamp
                                 message_to_log = message
                                 message_timestamp = line_timestamp
                                 progress_callback_lines = [line]
                         else:  # continuation of the previous log line
                             message_to_log = f"{message_to_log}\n{message}"
                             progress_callback_lines.append(line)
@@ -477,15 +478,16 @@
                     for line in progress_callback_lines:
                         if self._progress_callback:
                             self._progress_callback(line)
                         if self._callbacks:
                             self._callbacks.progress_callback(
                                 line=line, client=self._client, mode=ExecutionMode.SYNC
                             )
-                    self.log.info("[%s] %s", container_name, message_to_log)
+                    if message_to_log is not None:
+                        self.log.info("[%s] %s", container_name, message_to_log)
                     last_captured_timestamp = message_timestamp
             except TimeoutError as e:
                 # in case of timeout, increment return time by 2 seconds to avoid
                 # duplicate log entries
                 if val := (last_captured_timestamp or since_time):
                     return val.add(seconds=2), e
             except HTTPError as e:
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/pyproject.toml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-cncf-kubernetes"
-version = "8.1.0.rc1"
+version = "8.1.1.rc1"
 description = "Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -62,16 +62,16 @@
     "cryptography>=2.0.0",
     "google-re2>=1.0",
     "kubernetes>=28.1.0,<=29.0.0",
     "kubernetes_asyncio>=28.1.0,<=29.0.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.0rc1/PKG-INFO` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 8.1.0rc1
+Version: 8.1.1rc1
 Summary: Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow
 Keywords: airflow-provider,cncf.kubernetes,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,16 +25,16 @@
 Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: asgiref>=3.5.2
 Requires-Dist: cryptography>=2.0.0
 Requires-Dist: google-re2>=1.0
 Requires-Dist: kubernetes>=28.1.0,<=29.0.0
 Requires-Dist: kubernetes_asyncio>=28.1.0,<=29.0.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -76,28 +76,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.1.0.rc1``
+Release: ``8.1.1.rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
@@ -116,8 +116,8 @@
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=28.1.0,<=29.0.0``
 ``kubernetes_asyncio``  ``>=28.1.0,<=29.0.0``
 ``google-re2``          ``>=1.0``
 ======================  =====================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/changelog.html>`_.
```

