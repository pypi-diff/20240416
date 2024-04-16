# Comparing `tmp/sbcli-jm-2.1.3.zip` & `tmp/sbcli_jm-3.0.0.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 177697 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/setup.cfg
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/pyproject.toml
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/README.md
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/setup.py
--rw-r--r--  2.0 unx      148 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/env_var
--rw-r--r--  2.0 unx     1128 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/PKG-INFO
--rw-r--r--  2.0 unx    76437 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     5078 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     8654 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_web/static/tst.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/
--rw-r--r--  2.0 unx     6262 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    21428 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     1440 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx    63525 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/snode_client.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/db_config_single.sh
--rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx    13535 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1427 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    10787 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    46637 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4817 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     6372 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     4963 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2218 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     5067 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/requires.txt
--rw-r--r--  2.0 unx     1128 b- defN 24-Apr-06 20:39 sbcli-jm-2.1.3/sbcli_jm.egg-info/PKG-INFO
-144 files, 984094 bytes uncompressed, 151863 bytes compressed:  84.6%
+Zip file size: 177896 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/setup.cfg
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/pyproject.toml
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/README.md
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/setup.py
+-rw-r--r--  2.0 unx      147 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/env_var
+-rw-r--r--  2.0 unx     1128 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/PKG-INFO
+-rw-r--r--  2.0 unx    76335 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     8169 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     8654 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/tst.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/
+-rw-r--r--  2.0 unx     6199 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx    21410 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1440 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx    64162 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/snode_client.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_single.sh
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx    13535 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1427 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    10787 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    46637 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     6372 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     7218 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     3222 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     5067 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1128 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/PKG-INFO
+144 files, 985536 bytes uncompressed, 152062 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli-jm-2.1.3/
+Filename: sbcli_jm-3.0.0/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_cli/
+Filename: sbcli_jm-3.0.0/simplyblock_cli/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/
+Filename: sbcli_jm-3.0.0/simplyblock_web/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/
+Filename: sbcli_jm-3.0.0/simplyblock_core/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/setup.cfg
+Filename: sbcli_jm-3.0.0/setup.cfg
 Comment: 
 
-Filename: sbcli-jm-2.1.3/pyproject.toml
+Filename: sbcli_jm-3.0.0/pyproject.toml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/README.md
+Filename: sbcli_jm-3.0.0/README.md
 Comment: 
 
-Filename: sbcli-jm-2.1.3/setup.py
+Filename: sbcli_jm-3.0.0/setup.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/env_var
+Filename: sbcli_jm-3.0.0/env_var
 Comment: 
 
-Filename: sbcli-jm-2.1.3/PKG-INFO
+Filename: sbcli_jm-3.0.0/PKG-INFO
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_cli/cli.py
+Filename: sbcli_jm-3.0.0/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_cli/main.py
+Filename: sbcli_jm-3.0.0/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/templates/
+Filename: sbcli_jm-3.0.0/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/app.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/node_webapp.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/caching_node_app.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/snode_app.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/node_utils.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/utils.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/auth_middleware.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_jm-3.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/csi.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/rpac.yaml
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/delete.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/deploy.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/is_up.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/list_deps.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_web/static/tst.py
+Filename: sbcli_jm-3.0.0/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/distr_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/pci_utils.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/shell_utils.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/rpc_client.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/constants.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/storage_node_ops.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/cnode_client.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/compute_node_ops.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/cluster_ops.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/utils.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/kv_store.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/snode_client.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/device_events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/capacity_collector.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/install_service.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/device_monitor.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/remove_service.sh
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/health_check_service.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/service_template.service
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/global_settings.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/cluster.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/caching_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/pool.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/events.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/iface.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/base_model.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/__init__.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/stats.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/nvme_device.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/storage_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/port_stat.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/snapshot.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/compute_node.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/simplyblock_core/models/lvol_model.py
+Filename: sbcli_jm-3.0.0/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/top_level.txt
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/SOURCES.txt
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/dependency_links.txt
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/entry_points.txt
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/requires.txt
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli-jm-2.1.3/sbcli_jm.egg-info/PKG-INFO
+Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli-jm-2.1.3/README.md` & `sbcli_jm-3.0.0/README.md`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/setup.py` & `sbcli_jm-3.0.0/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/PKG-INFO` & `sbcli_jm-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-jm
-Version: 2.1.3
+Version: 3.0.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-jm-2.1.3/simplyblock_cli/cli.py` & `sbcli_jm-3.0.0/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         # sub_command.add_argument("ifname", help='Management interface name')
         # sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
 
         sub_command = self.add_sub_command(subparser, "add-node", 'Add storage node by ip')
         sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
         sub_command.add_argument("node_ip", help='IP of storage node to add')
         sub_command.add_argument("ifname", help='Management interface name')
-        sub_command.add_argument("--jm-pcie", help='JM device address', dest='jm_pcie')
         sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G', dest='spdk_mem')
         sub_command.add_argument("--dev-split", help='Split nvme devices by this factor, can be 2 or more',
                                  dest='dev_split', type=int, default=1)
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
@@ -801,15 +800,15 @@
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 out = storage_ops.add_node(
                     cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, dev_split, spdk_image, spdk_debug,
-                    small_pool_count, large_pool_count, small_bufsize, large_bufsize, args.jm_pcie)
+                    small_pool_count, large_pool_count, small_bufsize, large_bufsize)
                 return out
 
             elif sub_command == "list":
                 ret = storage_ops.list_storage_nodes(self.db_store, args.json)
 
             elif sub_command == "remove":
                 ret = storage_ops.remove_storage_node(args.node_id, args.force_remove, args.force_migrate)
```

## Comparing `sbcli-jm-2.1.3/simplyblock_web/caching_node_app_k8s.py` & `sbcli_jm-3.0.0/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/app.py` & `sbcli_jm-3.0.0/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/node_webapp.py` & `sbcli_jm-3.0.0/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/caching_node_app.py` & `sbcli_jm-3.0.0/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/snode_app.py` & `sbcli_jm-3.0.0/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/node_utils.py` & `sbcli_jm-3.0.0/simplyblock_web/node_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         logger.error(err)
         return []
     data = json.loads(out)
     logger.debug("nvme list:")
     logger.debug(data)
 
     devices = []
-    if data and 'Devices' in data:
+    if data and 'Devices' in data and data['Devices']:
         for dev in data['Devices'][0]['Subsystems']:
             if 'Controllers' in dev and dev['Controllers']:
                 controller = dev['Controllers'][0]
                 namespace = None
                 if "Namespaces" in dev and dev['Namespaces']:
                     namespace = dev['Namespaces'][0]
                 elif controller and controller["Namespaces"]:
```

## Comparing `sbcli-jm-2.1.3/simplyblock_web/utils.py` & `sbcli_jm-3.0.0/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/auth_middleware.py` & `sbcli_jm-3.0.0/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_jm-3.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files 10% similar despite different names*

```diff
@@ -27,30 +27,61 @@
             path: /lib/modules
         - name: dev-vol
           hostPath:
             path: /dev
         - name: hugepage
           emptyDir:
             medium: HugePages
+        - name: script-volume
+          emptyDir: {}
+        - name: script-config
+          configMap:
+            name: caching-node-restart-script-cm
+      initContainers:
+        - name: copy-script
+          image: busybox
+          command: ["sh", "-c", "cp /config/restart_script.py /script/restart_script.py"]
+          volumeMounts:
+            - name: script-volume
+              mountPath: /script
+            - name: script-config
+              mountPath: /config
       containers:
       - name: spdk-container
         image: {{ SPDK_IMAGE }}
         imagePullPolicy: "Always"
         command: ["/root/scripts/run_spdk_tgt.sh", "{{ SPDK_CPU_MASK }}", "{{ SPDK_MEM }}"]
+        lifecycle:
+          postStart:
+            exec:
+              command: ["/usr/bin/python3", "/script/restart_script.py"]
+        env:
+          - name: SPDKCSI_SECRET
+            valueFrom:
+              secretKeyRef:
+                name: spdkcsi-secret
+                key: secret.json
+          - name: CLUSTER_CONFIG
+            valueFrom:
+              configMapKeyRef:
+                name: spdkcsi-cm
+                key: config.json
         securityContext:
           privileged: true
         volumeMounts:
         - name: socket-dir
           mountPath: /var/tmp
         - name: host-sys
           mountPath: /sys
         - name: host-modules
           mountPath: /lib/modules
         - name: dev-vol
           mountPath: /dev
+        - name: script-volume
+          mountPath: /script
         resources:
           limits:
             hugepages-2Mi: 2Gi
             memory: 1024Mi
           requests:
             memory: 1024Mi
```

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/snode_ops.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/csi.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_device.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_jm-3.0.0/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/static/delete.py` & `sbcli_jm-3.0.0/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_web/static/deploy.py` & `sbcli_jm-3.0.0/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/distr_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/distr_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             logger.debug(f"Node is not online: {snode.get_id()}, status: {snode.status}")
             continue
         dev_map = {}
         dev_w_map = []
         node_w = 0
 
         for i, dev in enumerate(snode.nvme_devices):
-            if dev.status != "online":
-                logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
+            logger.debug(f"Device: {dev.get_id()}, status: {dev.status}")
+            if dev.status == "JM_DEV":
                 continue
             dev_w = int(dev.size/(1024*1024*1024)) or 1
             node_w += dev_w
             name = None
             if snode.get_id() == target_node.get_id():
                 name = dev.alceml_bdev
             else:
@@ -91,22 +91,21 @@
                         name = dev2.remote_bdev
                         break
             if not name:
                 continue
             dev_map[dev.cluster_device_order] = {
                 "UUID": dev.get_id(),
                 "bdev_name": name,
-                "status": "online"}
+                "status": dev.status}
             dev_w_map.append({
                 "weight": dev_w,
                 "id": dev.cluster_device_order})
         map_cluster[snode.get_id()] = {
-                # "availability_group": 0,
-                "status": "online",
-                "devices": dev_map}
+            "status": snode.status,
+            "devices": dev_map}
         map_prob.append({
             "weight": node_w,
             "items": dev_w_map
         })
     cl_map = {
         "name": "",
         "UUID_node_target": "",
```

## Comparing `sbcli-jm-2.1.3/simplyblock_core/pci_utils.py` & `sbcli_jm-3.0.0/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/rpc_client.py` & `sbcli_jm-3.0.0/simplyblock_core/rpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         params = {"name": uuid}
         return self._request("bdev_get_iostat", params)
 
     def bdev_raid_create(self, name, bdevs_list):
         params = {
             "name": name,
             "raid_level": "0",
-            "strip_size_kb": 4 * len(bdevs_list),
+            "strip_size_kb": 4,
             "base_bdevs": bdevs_list
         }
         return self._request("bdev_raid_create", params)
 
     def bdev_set_qos_limit(self, name, rw_ios_per_sec, rw_mbytes_per_sec, r_mbytes_per_sec, w_mbytes_per_sec):
         params = {
             "name": name
```

## Comparing `sbcli-jm-2.1.3/simplyblock_core/constants.py` & `sbcli_jm-3.0.0/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/storage_node_ops.py` & `sbcli_jm-3.0.0/simplyblock_core/storage_node_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,46 +212,46 @@
 def _prepare_cluster_devices(snode, after_restart=False):
     db_controller = DBController()
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
+    jm_nvme_bdevs = []
     for index, nvme in enumerate(snode.nvme_devices):
-        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE, NVMeDevice.STATUS_JM]:
+        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
             logger.debug(f"Device is not online or unavailable: {nvme.get_id()}, status: {nvme.status}")
             continue
 
+        ret = rpc_client.bdev_split(nvme.nvme_bdev, 10)
+        if not ret:
+            logger.error(f"Failed to split nvme bdev: {nvme.nvme_bdev}")
+            return False
+        jm_nvme_bdevs.append(f"{nvme.nvme_bdev}p0")
+        ret = rpc_client.bdev_raid_create(f"raid_{nvme.nvme_bdev}", [f"{nvme.nvme_bdev}p{i}" for i in range(1,10)])
+        if not ret:
+            logger.error(f"Failed to create raid_{nvme.nvme_bdev}")
+            return False
         test_name = f"{nvme.nvme_bdev}_test"
         # create testing bdev
-        ret = rpc_client.bdev_passtest_create(test_name, nvme.nvme_bdev)
-
+        ret = rpc_client.bdev_passtest_create(test_name, f"raid_{nvme.nvme_bdev}")
+        if not ret:
+            logger.error(f"Failed to create passtest bdev {test_name}")
+            return False
         alceml_id = nvme.get_id()
         alceml_name = f"alceml_{alceml_id}"
         logger.info(f"adding {alceml_name}")
         pba_init_mode = 3
         if after_restart:
             pba_init_mode = 2
         ret = rpc_client.bdev_alceml_create(alceml_name, test_name, alceml_id, pba_init_mode=pba_init_mode)
         if not ret:
             logger.error(f"Failed to create alceml bdev: {alceml_name}")
             return False
 
-        # create jm
-        if nvme.jm_bdev:
-            ret = rpc_client.bdev_jm_create(nvme.jm_bdev, alceml_name)
-            if not ret:
-                logger.error(f"Failed to create JM bdev: {snode.nvme_devices[0].jm_bdev}")
-                return False
-            nvme.testing_bdev = test_name
-            nvme.alceml_bdev = alceml_name
-            nvme.io_error = True
-            nvme.status = NVMeDevice.STATUS_JM
-            continue
-
         # add pass through
         pt_name = f"{alceml_name}_PT"
         ret = rpc_client.bdev_PT_NoExcl_create(pt_name, alceml_name)
         if not ret:
             logger.error(f"Failed to create pt noexcl bdev: {pt_name}")
             return False
 
@@ -284,14 +284,34 @@
         nvme.alceml_bdev = alceml_name
         nvme.pt_bdev = pt_name
         nvme.nvmf_nqn = subsystem_nqn
         nvme.nvmf_ip = IP
         nvme.nvmf_port = 4420
         nvme.io_error = False
         nvme.status = NVMeDevice.STATUS_ONLINE
+
+    if jm_nvme_bdevs:
+        ret = rpc_client.bdev_raid_create(f"raid_jm_{snode.get_id()}", jm_nvme_bdevs)
+        if not ret:
+            logger.error(f"Failed to create raid_jm_{snode.get_id()}")
+            return False
+        alceml_name = f"alceml_jm_{snode.get_id()}"
+        pba_init_mode = 3
+        if after_restart:
+            pba_init_mode = 2
+        ret = rpc_client.bdev_alceml_create(alceml_name, f"raid_jm_{snode.get_id()}", str(uuid.uuid4()), pba_init_mode=pba_init_mode)
+        if not ret:
+            logger.error(f"Failed to create alceml bdev: {alceml_name}")
+            return False
+
+        ret = rpc_client.bdev_jm_create(f"jm_{snode.get_id()}", alceml_name)
+        if not ret:
+            logger.error(f"Failed to create jm_{snode.get_id()}")
+            return False
+
     snode.write_to_db(db_controller.kv_store)
     return True
 
 
 def _connect_to_remote_devs(this_node):
     db_controller = DBController()
 
@@ -318,15 +338,15 @@
             dev.remote_bdev = f"{name}n1"
             remote_devices.append(dev)
     return remote_devices
 
 
 def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask,
              spdk_mem, dev_split=1, spdk_image=None, spdk_debug=False,
-             small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0, jm_device_pcie=None):
+             small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
@@ -476,28 +496,21 @@
                 dev_dict['nvme_bdev'] = pt
                 dev_dict['size'] = int(dev.size / dev_split)
                 new_devices.append(NVMeDevice(dev_dict))
         snode.nvme_devices = new_devices
     else:
         snode.nvme_devices = nvme_devs
 
-    jm_index = 0
     # Set device cluster order
     dev_order = get_next_cluster_device_order(db_controller)
     for index, nvme in enumerate(snode.nvme_devices):
         nvme.cluster_device_order = dev_order
         dev_order += 1
-        if jm_device_pcie and nvme.pcie_address == jm_device_pcie:
-            jm_index = index
         device_events.device_create(nvme)
 
-    # create jm
-    logger.info(f"Using device for JM: {snode.nvme_devices[jm_index].get_id()}")
-    snode.nvme_devices[jm_index].jm_bdev = f"jm_{snode.get_id()}"
-
     # save object
     snode.write_to_db(db_controller.kv_store)
 
     # prepare devices
     ret = _prepare_cluster_devices(snode)
     if not ret:
         logger.error("Failed to prepare cluster devices")
@@ -1553,25 +1566,25 @@
         ifname = "eth0"
 
     dev_ip = utils.get_iface_ip(ifname)
     if not dev_ip:
         logger.error(f"Error getting interface ip: {ifname}")
         return False
 
-    logger.info(f"Node IP: {dev_ip}")
-    ret = scripts.configure_docker(dev_ip)
-
     logger.info("NVMe SSD devices found on node:")
     stream = os.popen("lspci -Dnn | grep -i nvme")
     for l in stream.readlines():
         logger.info(l.strip())
 
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
 
+    logger.info(f"Node IP: {dev_ip}")
+    ret = scripts.configure_docker(dev_ip)
+
     node_docker = docker.DockerClient(base_url=f"tcp://{dev_ip}:2375", version="auto", timeout=60 * 5)
     # create the api container
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
         if node.attrs["Name"] == "/SNodeAPI":
             logger.info("SNodeAPI container found, removing...")
             node.stop()
@@ -1604,15 +1617,14 @@
 
 
 def deploy_cleaner():
     scripts.deploy_cleaner()
     return True
 
 
-
 def get_host_secret(node_id):
     db_controller = DBController()
     node = db_controller.get_storage_node_by_id(node_id)
     if not node:
         logger.error("node not found")
         return False
 
@@ -1625,15 +1637,15 @@
     if not node:
         logger.error("node not found")
         return False
 
     return node.ctrl_secret
 
 
-def health_checkk(node_id):
+def health_check(node_id):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error("node not found")
         return False
 
     try:
@@ -1772,8 +1784,8 @@
 
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
     data = snode.get_clean_dict()
-    return json.dumps(data, indent=2)
+    return json.dumps(data, indent=2)
```

## Comparing `sbcli-jm-2.1.3/simplyblock_core/cnode_client.py` & `sbcli_jm-3.0.0/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/compute_node_ops.py` & `sbcli_jm-3.0.0/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/cluster_ops.py` & `sbcli_jm-3.0.0/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/mgmt_node_ops.py` & `sbcli_jm-3.0.0/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/utils.py` & `sbcli_jm-3.0.0/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/kv_store.py` & `sbcli_jm-3.0.0/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/snode_client.py` & `sbcli_jm-3.0.0/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_jm-3.0.0/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/install_deps.sh` & `sbcli_jm-3.0.0/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/__init__.py` & `sbcli_jm-3.0.0/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/haproxy.cfg` & `sbcli_jm-3.0.0/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_jm-3.0.0/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_jm-3.0.0/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_jm-3.0.0/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/device_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/cluster_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/lvol_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/pool_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/snapshot_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/storage_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/mgmt_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/events_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/lvol_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/pool_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/device_events.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/controllers/health_controller.py` & `sbcli_jm-3.0.0/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_jm-3.0.0/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/log_agg_service.py` & `sbcli_jm-3.0.0/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/capacity_collector.py` & `sbcli_jm-3.0.0/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/port_stat_collector.py` & `sbcli_jm-3.0.0/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/__init__.py` & `sbcli_jm-3.0.0/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/install_service.sh` & `sbcli_jm-3.0.0/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_jm-3.0.0/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/device_monitor.py` & `sbcli_jm-3.0.0/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/storage_node_monitor.py` & `sbcli_jm-3.0.0/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/lvol_monitor.py` & `sbcli_jm-3.0.0/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/distr_event_collector.py` & `sbcli_jm-3.0.0/simplyblock_core/services/distr_event_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,18 +39,18 @@
             for dev in node.nvme_devices:
                 if dev.cluster_device_order == storage_id:
                     if dev.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
                         logger.info(f"The storage device is not online, skipping. status: {dev.status}")
                         event.status = 'skipped'
                         return
 
-                    if node.get_id() != node_id:
-                        logger.info(f"The storage device is remote, skipping")
-                        event.status = 'skipped-remote'
-                        return
+                    # if node.get_id() != node_id:
+                    #     logger.info(f"The storage device is remote, skipping")
+                    #     event.status = 'skipped-remote'
+                    #     return
 
                     device_id = dev.get_id()
                     break
 
         if not device_id:
             logger.info(f"Device not found!, storage id: {storage_id} from node: {node_id}")
             event.status = 'device_not_found'
```

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/health_check_service.py` & `sbcli_jm-3.0.0/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/caching_node_monitor.py` & `sbcli_jm-3.0.0/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/cap_monitor.py` & `sbcli_jm-3.0.0/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_jm-3.0.0/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/global_settings.py` & `sbcli_jm-3.0.0/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/cluster.py` & `sbcli_jm-3.0.0/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/caching_node.py` & `sbcli_jm-3.0.0/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/pool.py` & `sbcli_jm-3.0.0/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/events.py` & `sbcli_jm-3.0.0/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/iface.py` & `sbcli_jm-3.0.0/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/base_model.py` & `sbcli_jm-3.0.0/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/stats.py` & `sbcli_jm-3.0.0/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/nvme_device.py` & `sbcli_jm-3.0.0/simplyblock_core/models/nvme_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import List
 
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
-    STATUS_JM = "JM_DEV"
     STATUS_ONLINE = 'online'
     STATUS_AVAILABLE = 'available'
     STATUS_UNAVAILABLE = 'unavailable'
     STATUS_READONLY = 'read_only'
     STATUS_OVERLOADED = 'overloaded'
     STATUS_FAILED = 'failed'
     STATUS_REMOVED = 'removed'
```

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/storage_node.py` & `sbcli_jm-3.0.0/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/port_stat.py` & `sbcli_jm-3.0.0/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/mgmt_node.py` & `sbcli_jm-3.0.0/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/snapshot.py` & `sbcli_jm-3.0.0/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/compute_node.py` & `sbcli_jm-3.0.0/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/simplyblock_core/models/lvol_model.py` & `sbcli_jm-3.0.0/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/sbcli_jm.egg-info/SOURCES.txt` & `sbcli_jm-3.0.0/sbcli_jm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli-jm-2.1.3/sbcli_jm.egg-info/PKG-INFO` & `sbcli_jm-3.0.0/sbcli_jm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-jm
-Version: 2.1.3
+Version: 3.0.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

