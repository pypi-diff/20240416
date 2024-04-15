# Comparing `tmp/flwr_nightly-1.9.0.dev20240412.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240412.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240414.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240412.tar` & `flwr_nightly-1.9.0.dev20240414.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0        0        0    11358 2024-04-12 23:05:12.128890 flwr_nightly-1.9.0.dev20240412/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-12 23:05:12.128890 flwr_nightly-1.9.0.dev20240412/README.md
--rw-r--r--   0        0        0     5863 2024-04-12 23:05:28.604737 flwr_nightly-1.9.0.dev20240412/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     2215 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0     4675 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/flower_toml.py
--rw-r--r--   0        0        0      789 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5300 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0      668 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      269 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/flower.toml.tpl
--rw-r--r--   0        0        0      390 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      459 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      438 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4153 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1187 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    26193 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8717 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     8560 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-12 23:05:12.544886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    14482 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     1006 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2273 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     3016 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7782 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-12 23:05:12.548886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     4356 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     7571 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     9042 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2491 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24302 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5271 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3496 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7344 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      820 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0    10106 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0     4586 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5592 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-12 23:05:12.552886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4761 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3036 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3273 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     6734 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0     9586 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    23985 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     6058 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15685 2024-04-12 23:05:12.556886 flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15257 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240412/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-14 23:34:02.582474 flwr_nightly-1.9.0.dev20240414/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-14 23:34:02.582474 flwr_nightly-1.9.0.dev20240414/README.md
+-rw-r--r--   0        0        0     5863 2024-04-14 23:34:21.637594 flwr_nightly-1.9.0.dev20240414/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     2215 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0     4675 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/flower_toml.py
+-rw-r--r--   0        0        0      789 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5300 2024-04-14 23:34:02.998473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      269 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/flower.toml.tpl
+-rw-r--r--   0        0        0      390 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      459 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      438 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4153 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1187 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    26193 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8717 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     8560 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    14482 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     1006 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-14 23:34:03.002473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     3016 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7782 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24302 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3496 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7344 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      820 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0    10106 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0     4586 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-14 23:34:03.006473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5592 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4761 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3473 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0     9586 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    23985 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6058 2024-04-14 23:34:03.010473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15685 2024-04-14 23:34:03.014473 flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15257 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240414/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240412/LICENSE` & `flwr_nightly-1.9.0.dev20240414/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/README.md` & `flwr_nightly-1.9.0.dev20240414/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/pyproject.toml` & `flwr_nightly-1.9.0.dev20240414/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0-dev20240412"
+version = "1.9.0-dev20240414"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/flower_toml.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/flower_toml.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from flwr.proto import node_pb2 as flwr_dot_proto_dot_node__pb2
 from flwr.proto import task_pb2 as flwr_dot_proto_dot_task__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66lwr/proto/fleet.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x15\x66lwr/proto/task.proto\"*\n\x11\x43reateNodeRequest\x12\x15\n\rping_interval\x18\x01 \x01(\x01\"4\n\x12\x43reateNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"3\n\x11\x44\x65leteNodeRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"\x14\n\x12\x44\x65leteNodeResponse\"D\n\x0bPingRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x15\n\rping_interval\x18\x02 \x01(\x01\"\x1f\n\x0cPingResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"F\n\x12PullTaskInsRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x10\n\x08task_ids\x18\x02 \x03(\t\"k\n\x13PullTaskInsResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12*\n\rtask_ins_list\x18\x02 \x03(\x0b\x32\x13.flwr.proto.TaskIns\"@\n\x12PushTaskResRequest\x12*\n\rtask_res_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.TaskRes\"\xae\x01\n\x13PushTaskResResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12=\n\x07results\x18\x02 \x03(\x0b\x32,.flwr.proto.PushTaskResResponse.ResultsEntry\x1a.\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"\x1e\n\tReconnect\x12\x11\n\treconnect\x18\x01 \x01(\x04\x32\x86\x03\n\x05\x46leet\x12M\n\nCreateNode\x12\x1d.flwr.proto.CreateNodeRequest\x1a\x1e.flwr.proto.CreateNodeResponse\"\x00\x12M\n\nDeleteNode\x12\x1d.flwr.proto.DeleteNodeRequest\x1a\x1e.flwr.proto.DeleteNodeResponse\"\x00\x12;\n\x04Ping\x12\x17.flwr.proto.PingRequest\x1a\x18.flwr.proto.PingResponse\"\x00\x12P\n\x0bPullTaskIns\x12\x1e.flwr.proto.PullTaskInsRequest\x1a\x1f.flwr.proto.PullTaskInsResponse\"\x00\x12P\n\x0bPushTaskRes\x12\x1e.flwr.proto.PushTaskResRequest\x1a\x1f.flwr.proto.PushTaskResResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66lwr/proto/fleet.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x15\x66lwr/proto/task.proto\"*\n\x11\x43reateNodeRequest\x12\x15\n\rping_interval\x18\x01 \x01(\x01\"4\n\x12\x43reateNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"3\n\x11\x44\x65leteNodeRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"\x14\n\x12\x44\x65leteNodeResponse\"D\n\x0bPingRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x15\n\rping_interval\x18\x02 \x01(\x01\"\x1f\n\x0cPingResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"F\n\x12PullTaskInsRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x10\n\x08task_ids\x18\x02 \x03(\t\"k\n\x13PullTaskInsResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12*\n\rtask_ins_list\x18\x02 \x03(\x0b\x32\x13.flwr.proto.TaskIns\"@\n\x12PushTaskResRequest\x12*\n\rtask_res_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.TaskRes\"\xae\x01\n\x13PushTaskResResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12=\n\x07results\x18\x02 \x03(\x0b\x32,.flwr.proto.PushTaskResResponse.ResultsEntry\x1a.\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\":\n\x03Run\x12\x0e\n\x06run_id\x18\x01 \x01(\x12\x12\x0e\n\x06\x66\x61\x62_id\x18\x02 \x01(\t\x12\x13\n\x0b\x66\x61\x62_version\x18\x03 \x01(\t\"\x1f\n\rGetRunRequest\x12\x0e\n\x06run_id\x18\x01 \x01(\x12\".\n\x0eGetRunResponse\x12\x1c\n\x03run\x18\x01 \x01(\x0b\x32\x0f.flwr.proto.Run\"\x1e\n\tReconnect\x12\x11\n\treconnect\x18\x01 \x01(\x04\x32\xc9\x03\n\x05\x46leet\x12M\n\nCreateNode\x12\x1d.flwr.proto.CreateNodeRequest\x1a\x1e.flwr.proto.CreateNodeResponse\"\x00\x12M\n\nDeleteNode\x12\x1d.flwr.proto.DeleteNodeRequest\x1a\x1e.flwr.proto.DeleteNodeResponse\"\x00\x12;\n\x04Ping\x12\x17.flwr.proto.PingRequest\x1a\x18.flwr.proto.PingResponse\"\x00\x12P\n\x0bPullTaskIns\x12\x1e.flwr.proto.PullTaskInsRequest\x1a\x1f.flwr.proto.PullTaskInsResponse\"\x00\x12P\n\x0bPushTaskRes\x12\x1e.flwr.proto.PushTaskResRequest\x1a\x1f.flwr.proto.PushTaskResResponse\"\x00\x12\x41\n\x06GetRun\x12\x19.flwr.proto.GetRunRequest\x1a\x1a.flwr.proto.GetRunResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flwr.proto.fleet_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._options = None
@@ -43,12 +43,18 @@
   _globals['_PULLTASKINSRESPONSE']._serialized_end=539
   _globals['_PUSHTASKRESREQUEST']._serialized_start=541
   _globals['_PUSHTASKRESREQUEST']._serialized_end=605
   _globals['_PUSHTASKRESRESPONSE']._serialized_start=608
   _globals['_PUSHTASKRESRESPONSE']._serialized_end=782
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_start=736
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_end=782
-  _globals['_RECONNECT']._serialized_start=784
-  _globals['_RECONNECT']._serialized_end=814
-  _globals['_FLEET']._serialized_start=817
-  _globals['_FLEET']._serialized_end=1207
+  _globals['_RUN']._serialized_start=784
+  _globals['_RUN']._serialized_end=842
+  _globals['_GETRUNREQUEST']._serialized_start=844
+  _globals['_GETRUNREQUEST']._serialized_end=875
+  _globals['_GETRUNRESPONSE']._serialized_start=877
+  _globals['_GETRUNRESPONSE']._serialized_end=923
+  _globals['_RECONNECT']._serialized_start=925
+  _globals['_RECONNECT']._serialized_end=955
+  _globals['_FLEET']._serialized_start=958
+  _globals['_FLEET']._serialized_end=1415
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -160,14 +160,56 @@
         reconnect: typing.Optional[global___Reconnect] = ...,
         results: typing.Optional[typing.Mapping[typing.Text, builtins.int]] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["reconnect",b"reconnect"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["reconnect",b"reconnect","results",b"results"]) -> None: ...
 global___PushTaskResResponse = PushTaskResResponse
 
+class Run(google.protobuf.message.Message):
+    """GetRun messages"""
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    RUN_ID_FIELD_NUMBER: builtins.int
+    FAB_ID_FIELD_NUMBER: builtins.int
+    FAB_VERSION_FIELD_NUMBER: builtins.int
+    run_id: builtins.int
+    fab_id: typing.Text
+    fab_version: typing.Text
+    def __init__(self,
+        *,
+        run_id: builtins.int = ...,
+        fab_id: typing.Text = ...,
+        fab_version: typing.Text = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["fab_id",b"fab_id","fab_version",b"fab_version","run_id",b"run_id"]) -> None: ...
+global___Run = Run
+
+class GetRunRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    RUN_ID_FIELD_NUMBER: builtins.int
+    run_id: builtins.int
+    def __init__(self,
+        *,
+        run_id: builtins.int = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["run_id",b"run_id"]) -> None: ...
+global___GetRunRequest = GetRunRequest
+
+class GetRunResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    RUN_FIELD_NUMBER: builtins.int
+    @property
+    def run(self) -> global___Run: ...
+    def __init__(self,
+        *,
+        run: typing.Optional[global___Run] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["run",b"run"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["run",b"run"]) -> None: ...
+global___GetRunResponse = GetRunResponse
+
 class Reconnect(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     RECONNECT_FIELD_NUMBER: builtins.int
     reconnect: builtins.int
     def __init__(self,
         *,
         reconnect: builtins.int = ...,
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,19 @@
                 response_deserializer=flwr_dot_proto_dot_fleet__pb2.PullTaskInsResponse.FromString,
                 )
         self.PushTaskRes = channel.unary_unary(
                 '/flwr.proto.Fleet/PushTaskRes',
                 request_serializer=flwr_dot_proto_dot_fleet__pb2.PushTaskResRequest.SerializeToString,
                 response_deserializer=flwr_dot_proto_dot_fleet__pb2.PushTaskResResponse.FromString,
                 )
+        self.GetRun = channel.unary_unary(
+                '/flwr.proto.Fleet/GetRun',
+                request_serializer=flwr_dot_proto_dot_fleet__pb2.GetRunRequest.SerializeToString,
+                response_deserializer=flwr_dot_proto_dot_fleet__pb2.GetRunResponse.FromString,
+                )
 
 
 class FleetServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateNode(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -76,14 +81,20 @@
 
         HTTP API path: /api/v1/fleet/push-task-res
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetRun(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_FleetServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateNode': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateNode,
                     request_deserializer=flwr_dot_proto_dot_fleet__pb2.CreateNodeRequest.FromString,
                     response_serializer=flwr_dot_proto_dot_fleet__pb2.CreateNodeResponse.SerializeToString,
@@ -104,14 +115,19 @@
                     response_serializer=flwr_dot_proto_dot_fleet__pb2.PullTaskInsResponse.SerializeToString,
             ),
             'PushTaskRes': grpc.unary_unary_rpc_method_handler(
                     servicer.PushTaskRes,
                     request_deserializer=flwr_dot_proto_dot_fleet__pb2.PushTaskResRequest.FromString,
                     response_serializer=flwr_dot_proto_dot_fleet__pb2.PushTaskResResponse.SerializeToString,
             ),
+            'GetRun': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetRun,
+                    request_deserializer=flwr_dot_proto_dot_fleet__pb2.GetRunRequest.FromString,
+                    response_serializer=flwr_dot_proto_dot_fleet__pb2.GetRunResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'flwr.proto.Fleet', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -198,7 +214,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/flwr.proto.Fleet/PushTaskRes',
             flwr_dot_proto_dot_fleet__pb2.PushTaskResRequest.SerializeToString,
             flwr_dot_proto_dot_fleet__pb2.PushTaskResResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetRun(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/flwr.proto.Fleet/GetRun',
+            flwr_dot_proto_dot_fleet__pb2.GetRunRequest.SerializeToString,
+            flwr_dot_proto_dot_fleet__pb2.GetRunResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         flwr.proto.fleet_pb2.PushTaskResRequest,
         flwr.proto.fleet_pb2.PushTaskResResponse]
     """Complete one or more tasks, if possible
 
     HTTP API path: /api/v1/fleet/push-task-res
     """
 
+    GetRun: grpc.UnaryUnaryMultiCallable[
+        flwr.proto.fleet_pb2.GetRunRequest,
+        flwr.proto.fleet_pb2.GetRunResponse]
+
 
 class FleetServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def CreateNode(self,
         request: flwr.proto.fleet_pb2.CreateNodeRequest,
         context: grpc.ServicerContext,
     ) -> flwr.proto.fleet_pb2.CreateNodeResponse: ...
@@ -74,9 +78,15 @@
     ) -> flwr.proto.fleet_pb2.PushTaskResResponse:
         """Complete one or more tasks, if possible
 
         HTTP API path: /api/v1/fleet/push-task-res
         """
         pass
 
+    @abc.abstractmethod
+    def GetRun(self,
+        request: flwr.proto.fleet_pb2.GetRunRequest,
+        context: grpc.ServicerContext,
+    ) -> flwr.proto.fleet_pb2.GetRunResponse: ...
+
 
 def add_FleetServicer_to_server(servicer: FleetServicer, server: grpc.Server) -> None: ...
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from flwr.common.logger import log
 from flwr.proto import fleet_pb2_grpc  # pylint: disable=E0611
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     CreateNodeResponse,
     DeleteNodeRequest,
     DeleteNodeResponse,
+    GetRunRequest,
+    GetRunResponse,
     PingRequest,
     PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
@@ -86,7 +88,17 @@
     ) -> PushTaskResResponse:
         """Push TaskRes."""
         log(INFO, "FleetServicer.PushTaskRes")
         return message_handler.push_task_res(
             request=request,
             state=self.state_factory.state(),
         )
+
+    def GetRun(
+        self, request: GetRunRequest, context: grpc.ServicerContext
+    ) -> GetRunResponse:
+        """Get run information."""
+        log(INFO, "FleetServicer.GetRun")
+        return message_handler.get_run(
+            request=request,
+            state=self.state_factory.state(),
+        )
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from uuid import UUID
 
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     CreateNodeResponse,
     DeleteNodeRequest,
     DeleteNodeResponse,
+    GetRunRequest,
+    GetRunResponse,
     PingRequest,
     PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
     Reconnect,
@@ -97,7 +99,14 @@
 
     # Build response
     response = PushTaskResResponse(
         reconnect=Reconnect(reconnect=5),
         results={str(task_id): 0},
     )
     return response
+
+
+def get_run(
+    request: GetRunRequest, state: State  # pylint: disable=W0613
+) -> GetRunResponse:
+    """Get run information."""
+    return GetRunResponse()
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import sys
 
 from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
+    GetRunRequest,
     PingRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 from flwr.server.superlink.fleet.message_handler import message_handler
 from flwr.server.superlink.state import State
 
@@ -175,20 +176,49 @@
     return Response(
         status_code=200,
         content=ping_response_bytes,
         headers={"Content-Type": "application/protobuf"},
     )
 
 
+async def get_run(request: Request) -> Response:
+    """GetRun."""
+    _check_headers(request.headers)
+
+    # Get the request body as raw bytes
+    get_run_request_bytes: bytes = await request.body()
+
+    # Deserialize ProtoBuf
+    get_run_request_proto = GetRunRequest()
+    get_run_request_proto.ParseFromString(get_run_request_bytes)
+
+    # Get state from app
+    state: State = app.state.STATE_FACTORY.state()
+
+    # Handle message
+    get_run_response_proto = message_handler.get_run(
+        request=get_run_request_proto, state=state
+    )
+
+    # Return serialized ProtoBuf
+    get_run_response_bytes = get_run_response_proto.SerializeToString()
+    return Response(
+        status_code=200,
+        content=get_run_response_bytes,
+        headers={"Content-Type": "application/protobuf"},
+    )
+
+
 routes = [
     Route("/api/v0/fleet/create-node", create_node, methods=["POST"]),
     Route("/api/v0/fleet/delete-node", delete_node, methods=["POST"]),
     Route("/api/v0/fleet/pull-task-ins", pull_task_ins, methods=["POST"]),
     Route("/api/v0/fleet/push-task-res", push_task_res, methods=["POST"]),
     Route("/api/v0/fleet/ping", ping, methods=["POST"]),
+    Route("/api/v0/fleet/get-run", get_run, methods=["POST"]),
 ]
 
 app: Starlette = Starlette(
     debug=False,
     routes=routes,
 )
```

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240414/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240412/PKG-INFO` & `flwr_nightly-1.9.0.dev20240414/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240412
+Version: 1.9.0.dev20240414
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240412 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240414 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

