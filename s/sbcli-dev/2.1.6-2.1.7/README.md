# Comparing `tmp/sbcli_dev-2.1.6.zip` & `tmp/sbcli_dev-2.1.7.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 178247 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/setup.cfg
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/pyproject.toml
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/README.md
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/setup.py
--rw-r--r--  2.0 unx      148 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/env_var
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     5073 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx    76437 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     5098 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     8654 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_web/static/tst.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/
--rw-r--r--  2.0 unx     6213 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    21428 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     1440 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx    63525 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/snode_client.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/db_config_single.sh
--rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx    13535 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1427 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    10787 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    46637 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4817 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     6372 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     4971 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2218 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-16 15:37 sbcli_dev-2.1.6/simplyblock_core/models/lvol_model.py
-144 files, 985068 bytes uncompressed, 152111 bytes compressed:  84.6%
+Zip file size: 178140 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/setup.cfg
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/pyproject.toml
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/README.md
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/setup.py
+-rw-r--r--  2.0 unx      148 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/env_var
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     5073 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx    76437 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     8169 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     8654 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_web/static/tst.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/
+-rw-r--r--  2.0 unx     7387 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx    21428 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1440 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx    61755 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/snode_client.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/db_config_single.sh
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx    13535 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1427 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    46084 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     6372 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     7218 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     3252 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-16 17:00 sbcli_dev-2.1.7/simplyblock_core/models/lvol_model.py
+144 files, 983566 bytes uncompressed, 152004 bytes compressed:  84.5%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli_dev-2.1.6/
+Filename: sbcli_dev-2.1.7/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_cli/
+Filename: sbcli_dev-2.1.7/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/
+Filename: sbcli_dev-2.1.7/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/
+Filename: sbcli_dev-2.1.7/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/setup.cfg
+Filename: sbcli_dev-2.1.7/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.1.6/pyproject.toml
+Filename: sbcli_dev-2.1.7/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/README.md
+Filename: sbcli_dev-2.1.7/README.md
 Comment: 
 
-Filename: sbcli_dev-2.1.6/setup.py
+Filename: sbcli_dev-2.1.7/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/env_var
+Filename: sbcli_dev-2.1.7/env_var
 Comment: 
 
-Filename: sbcli_dev-2.1.6/PKG-INFO
+Filename: sbcli_dev-2.1.7/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.1.6/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.1.7/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.1.7/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_cli/main.py
+Filename: sbcli_dev-2.1.7/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/templates/
+Filename: sbcli_dev-2.1.7/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/app.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/utils.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.1.7/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.1.7/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/constants.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/utils.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/capacity_collector.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.1.6/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.1.7/simplyblock_core/models/lvol_model.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.1.6/README.md` & `sbcli_dev-2.1.7/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/setup.py` & `sbcli_dev-2.1.7/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/PKG-INFO` & `sbcli_dev-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.1.6
+Version: 2.1.7
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.1.6/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.1.7/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.1.7/sbcli_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.1.6
+Version: 2.1.7
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.1.6/simplyblock_cli/cli.py` & `sbcli_dev-2.1.7/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.1.7/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/app.py` & `sbcli_dev-2.1.7/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/node_webapp.py` & `sbcli_dev-2.1.7/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.1.7/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/snode_app.py` & `sbcli_dev-2.1.7/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/node_utils.py` & `sbcli_dev-2.1.7/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/utils.py` & `sbcli_dev-2.1.7/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.1.7/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.1.7/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.1.7/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.1.7/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/static/delete.py` & `sbcli_dev-2.1.7/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_web/static/deploy.py` & `sbcli_dev-2.1.7/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/distr_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/distr_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding=utf-8
 import datetime
 import logging
 import re
 
+from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.kv_store import DBController
 
 logger = logging.getLogger()
 
 
 def send_node_status_event(node_id, node_status):
@@ -65,25 +66,22 @@
         node.write_to_db(db_controller.kv_store)
 
 
 def get_distr_cluster_map(snodes, target_node):
     map_cluster = {}
     map_prob = []
     for snode in snodes:
-        if snode.status not in [snode.STATUS_ONLINE, snode.STATUS_RESTARTING]:
-            logger.debug(f"Node is not online: {snode.get_id()}, status: {snode.status}")
-            continue
         dev_map = {}
         dev_w_map = []
         node_w = 0
-
         for i, dev in enumerate(snode.nvme_devices):
             logger.debug(f"Device: {dev.get_id()}, status: {dev.status}")
-            if dev.status == "JM_DEV":
+            if dev.status == NVMeDevice.STATUS_JM:
                 continue
+
             dev_w = int(dev.size/(1024*1024*1024)) or 1
             node_w += dev_w
             name = None
             if snode.get_id() == target_node.get_id():
                 name = dev.alceml_bdev
             else:
                 for dev2 in target_node.remote_devices:
@@ -166,8 +164,43 @@
                 else:
                     data["Results"] = "failed"
                     passed = False
             else:
                 data["Results"] = "not found"
                 passed = False
             results.append(data)
-    return results, passed
+    return results, passed
+
+
+def send_cluster_map_to_node(node):
+    db_controller = DBController()
+    snodes = db_controller.get_storage_nodes()
+    rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+    cluster_map_data = get_distr_cluster_map(snodes, node)
+    cluster_map_data['UUID_node_target'] = node.get_id()
+    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    if not ret:
+        logger.error("Failed to send cluster map")
+        logger.info(cluster_map_data)
+        return False
+    return True
+
+
+def send_cluster_map_add_node(snode):
+    db_controller = DBController()
+    snodes = db_controller.get_storage_nodes()
+    for node in snodes:
+        if node.status != node.STATUS_ONLINE:
+            continue
+        logger.info(f"Sending to: {node.get_id()}")
+        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+
+        cluster_map_data = get_distr_cluster_map([snode], node)
+        cl_map = {
+            "map_cluster": cluster_map_data['map_cluster'],
+            "map_prob": cluster_map_data['map_prob']}
+        ret = rpc_client.distr_add_nodes(cl_map)
+        if not ret:
+            logger.error("Failed to send cluster map")
+            logger.info(cl_map)
+            return False
+    return True
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/pci_utils.py` & `sbcli_dev-2.1.7/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/rpc_client.py` & `sbcli_dev-2.1.7/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/constants.py` & `sbcli_dev-2.1.7/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.1.7/simplyblock_core/storage_node_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -538,31 +538,21 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
@@ -683,31 +673,21 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
@@ -948,31 +928,21 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending node event update")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     logger.info("Sending devices event updates")
     for dev in snode.nvme_devices:
         if dev.status != "online":
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/cnode_client.py` & `sbcli_dev-2.1.7/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.1.7/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.1.7/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.1.7/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/utils.py` & `sbcli_dev-2.1.7/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/kv_store.py` & `sbcli_dev-2.1.7/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/snode_client.py` & `sbcli_dev-2.1.7/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.1.7/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.1.7/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.1.7/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.1.7/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.1.7/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.1.7/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.1.7/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.1.7/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.1.7/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/snapshot_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,17 @@
         base_name, new_vuid, lvol.ndcs, lvol.npcs, num_blocks,
         lvol.distr_bs, lvol_controller.get_jm_names(snode), lvol.distr_chunk_bs,
         None, None, lvol.distr_page_size)
     if not ret:
         logger.error("Failed to create Distr bdev")
         return False, "Failed to create Distr bdev"
 
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     ret = rpc_client.ultra21_lvol_bmap_init(
         base_name, num_blocks, lvol.distr_bs, int(lvol.distr_page_size / lvol.distr_bs), num_blocks * 10)
     if not ret:
         return False, "Failed to init distr bdev"
 
     logger.info("Creating Snapshot bdev")
@@ -229,18 +228,17 @@
         logger.error("Failed to create Distr bdev")
         return False, "Failed to create Distr bdev"
     if ret == "?":
         logger.error(f"Failed to create Distr bdev, ret={ret}")
         # return False
 
     logger.info("Sending cluster map to the lvol")
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     logger.info("Creating clone bdev")
     block_len = lvol.distr_bs
     page_len = int(lvol.distr_page_size / lvol.distr_bs)
     max_num_blocks = num_blocks * 10
     ret = rpc_client.ultra21_lvol_bmap_init(name, num_blocks, block_len, page_len, max_num_blocks)
     if not ret:
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/lvol_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -709,19 +709,18 @@
         ret = None
 
         if type == "bdev_distr":
             params['jm_names'] = get_jm_names(snode)
             params['ha_comm_addrs'] = ha_comm_addrs
             params['ha_inode_self'] = ha_inode_self
             ret = rpc_client.bdev_distrib_create(**params)
-
-            snodes = db_controller.get_storage_nodes()
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-            cluster_map_data['UUID_node_target'] = snode.get_id()
-            rpc_client.distr_send_cluster_map(cluster_map_data)
+            if ret:
+                ret = distr_controller.send_cluster_map_to_node(snode)
+                if not ret:
+                    return False, "Failed to send cluster map"
 
         elif type == "bmap_init":
             ret = rpc_client.ultra21_lvol_bmap_init(**params)
 
         elif type == "ultra_lvol":
             ret = rpc_client.ultra21_lvol_mount_lvol(**params)
 
@@ -783,18 +782,17 @@
 
     logger.info("Add BDev to subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(lvol.nqn, lvol.top_bdev, lvol.uuid, lvol.guid)
     if not ret:
         return False, "Failed to add bdev to subsystem"
 
     logger.info("Sending cluster map to LVol")
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     spdk_mem_info_after = rpc_client.ultra21_util_get_malloc_stats()
     logger.debug("ultra21_util_get_malloc_stats:")
     logger.debug(spdk_mem_info_after)
 
     diff = {}
     for key in spdk_mem_info_after.keys():
@@ -1271,21 +1269,15 @@
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
 
     snode = db_controller.get_storage_node_by_id(lvol.node_id)
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    logger.info(f"Sending to: {snode.get_id()}")
-    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-    return ret
+    return distr_controller.send_cluster_map_to_node(snode)
 
 
 def get_cluster_map(lvol_id):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.1.7/simplyblock_core/controllers/health_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         logger.error("node not found")
         return False
 
     if snode.status in [StorageNode.STATUS_OFFLINE, StorageNode.STATUS_REMOVED]:
         logger.info(f"Skipping ,node status is {snode.status}")
         return True
 
-    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_UNRECOGNIZED]:
+    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_FAILED]:
         logger.info(f"Skipping ,device status is {device.status}")
         return True
 
     passed = True
     try:
         rpc_client = RPCClient(
             snode.mgmt_ip, snode.rpc_port,
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.1.7/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.1.7/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/capacity_collector.py` & `sbcli_dev-2.1.7/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.1.7/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/__init__.py` & `sbcli_dev-2.1.7/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.1.7/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.1.7/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.1.7/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.1.7/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.1.7/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.1.7/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.1.7/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.1.7/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.1.7/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.1.7/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.1.7/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/cluster.py` & `sbcli_dev-2.1.7/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.1.7/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/pool.py` & `sbcli_dev-2.1.7/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/events.py` & `sbcli_dev-2.1.7/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/iface.py` & `sbcli_dev-2.1.7/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/base_model.py` & `sbcli_dev-2.1.7/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/stats.py` & `sbcli_dev-2.1.7/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.1.7/simplyblock_core/models/nvme_device.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
     STATUS_JM = "JM_DEV"
+
     STATUS_ONLINE = 'online'
-    STATUS_AVAILABLE = 'available'
     STATUS_UNAVAILABLE = 'unavailable'
-    STATUS_READONLY = 'read_only'
-    STATUS_OVERLOADED = 'overloaded'
-    STATUS_FAILED = 'failed'
     STATUS_REMOVED = 'removed'
-    STATUS_RESETTING = 'resetting'
-    STATUS_UNRECOGNIZED = 'unrecognized'
+    STATUS_FAILED = 'failed'
+    STATUS_READONLY = 'read_only'
 
     attributes = {
         "uuid": {"type": str, 'default': ""},
         "device_name": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
         "sequential_number": {"type": int, 'default': 0},
         "partitions_count": {"type": int, 'default': 0},
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.1.7/simplyblock_core/models/storage_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 
 class StorageNode(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
     STATUS_SUSPENDED = 'suspended'
-    STATUS_IN_CREATION = 'in_creation'
     STATUS_IN_SHUTDOWN = 'in_shutdown'
-    STATUS_RESTARTING = 'restarting'
-    STATUS_UNREACHABLE = 'unreachable'
     STATUS_REMOVED = 'removed'
+    STATUS_RESTARTING = 'in_restart'
+
+    STATUS_IN_CREATION = 'in_restart'  # 'in_creation'
+    STATUS_UNREACHABLE = 'offline'  # 'unreachable'
 
     STATUS_CODE_MAP = {
         STATUS_ONLINE: 0,
         STATUS_OFFLINE: 1,
         STATUS_SUSPENDED: 2,
         STATUS_REMOVED: 3,
```

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.1.7/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.1.7/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.1.7/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.1.7/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.1.6/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.1.7/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

