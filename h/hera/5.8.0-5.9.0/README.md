# Comparing `tmp/hera-5.8.0.tar.gz` & `tmp/hera-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera-5.8.0.tar", max compression
+gzip compressed data, was "hera-5.9.0.tar", max compression
```

## Comparing `hera-5.8.0.tar` & `hera-5.9.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1066 2023-10-24 16:39:48.923639 hera-5.8.0/LICENSE
--rw-r--r--   0        0        0     7951 2023-10-24 16:39:48.923639 hera-5.8.0/README.md
--rw-r--r--   0        0        0     3778 2023-10-24 16:40:11.563557 hera-5.8.0/pyproject.toml
--rw-r--r--   0        0        0      523 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/__init__.py
--rw-r--r--   0        0        0      300 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/_version.py
--rw-r--r--   0        0        0     1669 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/auth/__init__.py
--rw-r--r--   0        0        0       19 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3262 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1403 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      278 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      622 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   108238 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.963639 hera-5.8.0/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   150080 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    32048 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   130758 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1706 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3092 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22481 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      208 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1438 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    28683 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/events/service.py
--rw-r--r--   0        0        0     2870 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/exceptions/__init__.py
--rw-r--r--   0        0        0      282 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12024 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/py.typed
--rw-r--r--   0        0        0      294 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      962 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     6574 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0     1287 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4735 2023-10-24 16:39:48.967639 hera-5.8.0/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     3990 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/_context.py
--rw-r--r--   0        0        0     4741 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/_inspect.py
--rw-r--r--   0        0        0    54241 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32887 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0     1587 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/archive.py
--rw-r--r--   0        0        0    13690 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3769 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/cluster_workflow_template.py
--rw-r--r--   0        0        0     3924 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/container.py
--rw-r--r--   0        0        0     7709 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     9680 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     3126 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2919 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/data.py
--rw-r--r--   0        0        0     7886 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1572 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      686 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2679 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0     5001 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/metrics.py
--rw-r--r--   0        0        0     6908 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1403 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      278 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      622 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   108238 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   150080 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    32048 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.971639 hera-5.8.0/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   130758 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1706 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3092 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22481 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0       75 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      208 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1438 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      902 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4672 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1816 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     3898 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5542 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     2851 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0    12916 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    30323 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/script.py
--rw-r--r--   0        0        0    53667 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/service.py
--rw-r--r--   0        0        0     6793 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3370 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0     7345 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/task.py
--rw-r--r--   0        0        0      129 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     3476 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2615 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    21504 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    23321 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0     1113 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     7457 2023-10-24 16:39:48.975638 hera-5.8.0/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 hera-5.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-10-26 13:51:15.748113 hera-5.9.0/LICENSE
+-rw-r--r--   0        0        0     7951 2023-10-26 13:51:15.748113 hera-5.9.0/README.md
+-rw-r--r--   0        0        0     3778 2023-10-26 13:51:36.856759 hera-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0      523 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/__init__.py
+-rw-r--r--   0        0        0      300 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/_version.py
+-rw-r--r--   0        0        0     1669 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/auth/__init__.py
+-rw-r--r--   0        0        0       19 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3262 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1403 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      278 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      622 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   108238 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.792115 hera-5.9.0/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   150080 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    32048 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   130758 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1706 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3092 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22481 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      208 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1438 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    28683 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/events/service.py
+-rw-r--r--   0        0        0     2870 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/exceptions/__init__.py
+-rw-r--r--   0        0        0      282 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12024 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/py.typed
+-rw-r--r--   0        0        0      294 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      962 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     6574 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0     1287 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4735 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     3990 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0     4741 2023-10-26 13:51:15.796115 hera-5.9.0/src/hera/workflows/_inspect.py
+-rw-r--r--   0        0        0    54241 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32887 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0     1587 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0    14060 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3769 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/cluster_workflow_template.py
+-rw-r--r--   0        0        0     3924 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     7709 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     9680 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     3126 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2919 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     7886 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1572 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      686 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2679 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0     5001 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/metrics.py
+-rw-r--r--   0        0        0     6908 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1403 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      278 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      622 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   108238 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.800115 hera-5.9.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   150080 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    32048 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   130758 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1706 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3092 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22481 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0       75 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      208 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1438 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      902 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4672 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1816 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     3898 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5542 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     2851 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0    12916 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    30323 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    53667 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     6793 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3370 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0     7345 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/task.py
+-rw-r--r--   0        0        0      129 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     3476 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2615 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    21504 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    23321 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0     1113 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     7457 2023-10-26 13:51:15.804115 hera-5.9.0/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 hera-5.9.0/PKG-INFO
```

### Comparing `hera-5.8.0/LICENSE` & `hera-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/README.md` & `hera-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/pyproject.toml` & `hera-5.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera"  # project-name
 # The version is automatically substituted by the CI
-version = "5.8.0"
+version = "5.9.0"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera-5.8.0/src/hera/__init__.py` & `hera-5.9.0/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/auth/__init__.py` & `hera-5.9.0/src/hera/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/__init__.py` & `hera-5.9.0/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/eventsource.py` & `hera-5.9.0/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/eventsource.pyi` & `hera-5.9.0/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/grpc/gateway/runtime.py` & `hera-5.9.0/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera-5.9.0/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.9.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.9.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.9.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/k8s/api/core/v1.py` & `hera-5.9.0/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera-5.9.0/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera-5.9.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.9.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/sensor.py` & `hera-5.9.0/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/models/sensor.pyi` & `hera-5.9.0/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/events/service.py` & `hera-5.9.0/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/exceptions/__init__.py` & `hera-5.9.0/src/hera/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/expr/_node.py` & `hera-5.9.0/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/expr/_sprig.py` & `hera-5.9.0/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/shared/_base_model.py` & `hera-5.9.0/src/hera/shared/_base_model.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/shared/_global_config.py` & `hera-5.9.0/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/shared/serialization.py` & `hera-5.9.0/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/__init__.py` & `hera-5.9.0/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/_context.py` & `hera-5.9.0/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/_inspect.py` & `hera-5.9.0/src/hera/workflows/_inspect.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/_mixins.py` & `hera-5.9.0/src/hera/workflows/_mixins.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/_unparse.py` & `hera-5.9.0/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/archive.py` & `hera-5.9.0/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/artifact.py` & `hera-5.9.0/src/hera/workflows/artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     """allows the specification of an artifact from a subpath within the main source."""
 
     loader: Optional[ArtifactLoader] = None
     """used for input Artifact annotations for determining how to load the data.
 
     Note: A loader value of 'None' must be used with an underlying type of 'str' or Path-like class."""
 
+    optional: Optional[bool] = None
+    """whether the Artifact is optional. For an input Artifact, this means it may possibly not
+    exist at the specified path during the template's runtime. For an output Artifact, it may
+    possibly not be generated during the step/task and available as an output to subsequent steps/tasks."""
+
     output: bool = False
     """used to specify artifact as an output in function signature annotations"""
 
     def _check_name(self):
         if not self.name:
             raise ValueError("name cannot be `None` or empty when used")
 
@@ -110,14 +115,15 @@
             archive_logs=self.archive_logs,
             artifact_gc=self.artifact_gc,
             deleted=self.deleted,
             from_=self.from_,
             from_expression=self.from_expression,
             global_name=self.global_name,
             mode=self.mode,
+            optional=self.optional,
             path=self.path,
             recurse_mode=self.recurse_mode,
             sub_path=self.sub_path,
         )
 
     def _build_artifact_paths(self) -> _ModelArtifactPaths:
         self._check_name()
```

### Comparing `hera-5.8.0/src/hera/workflows/cluster_workflow_template.py` & `hera-5.9.0/src/hera/workflows/cluster_workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/container.py` & `hera-5.9.0/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/container_set.py` & `hera-5.9.0/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/cron_workflow.py` & `hera-5.9.0/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/dag.py` & `hera-5.9.0/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/data.py` & `hera-5.9.0/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/env.py` & `hera-5.9.0/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/env_from.py` & `hera-5.9.0/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/exceptions.py` & `hera-5.9.0/src/hera/workflows/exceptions.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/http_template.py` & `hera-5.9.0/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/metrics.py` & `hera-5.9.0/src/hera/workflows/metrics.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/__init__.py` & `hera-5.9.0/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/eventsource.py` & `hera-5.9.0/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/eventsource.pyi` & `hera-5.9.0/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera-5.9.0/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera-5.9.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.9.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.9.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.9.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera-5.9.0/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera-5.9.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera-5.9.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.9.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/sensor.py` & `hera-5.9.0/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/models/sensor.pyi` & `hera-5.9.0/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/operator.py` & `hera-5.9.0/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/parameter.py` & `hera-5.9.0/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/protocol.py` & `hera-5.9.0/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/resource.py` & `hera-5.9.0/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/resources.py` & `hera-5.9.0/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/retry_strategy.py` & `hera-5.9.0/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/runner.py` & `hera-5.9.0/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/script.py` & `hera-5.9.0/src/hera/workflows/script.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/service.py` & `hera-5.9.0/src/hera/workflows/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/steps.py` & `hera-5.9.0/src/hera/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/suspend.py` & `hera-5.9.0/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/task.py` & `hera-5.9.0/src/hera/workflows/task.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/user_container.py` & `hera-5.9.0/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/validators.py` & `hera-5.9.0/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/volume.py` & `hera-5.9.0/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/workflow.py` & `hera-5.9.0/src/hera/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/workflow_status.py` & `hera-5.9.0/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/src/hera/workflows/workflow_template.py` & `hera-5.9.0/src/hera/workflows/workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.8.0/PKG-INFO` & `hera-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera
-Version: 5.8.0
+Version: 5.9.0
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
```

