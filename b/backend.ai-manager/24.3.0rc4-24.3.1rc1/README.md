# Comparing `tmp/backend.ai-manager-24.3.0rc4.tar.gz` & `tmp/backend.ai-manager-24.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:02 2024, max compression
+gzip compressed data, was "backend.ai-manager-24.3.1rc1.tar", last modified: Tue Apr 16 17:08:34 2024, max compression
```

## Comparing `backend.ai-manager-24.3.0rc4.tar` & `backend.ai-manager-24.3.1rc1.tar`

### file list

```diff
@@ -1,293 +1,296 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.469383 backend.ai-manager-24.3.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-05 03:40:02.465383 backend.ai-manager-24.3.0rc4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.389383 backend.ai-manager-24.3.0rc4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.389383 backend.ai-manager-24.3.0rc4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.397383 backend.ai-manager-24.3.0rc4/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/agent_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.405383 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41681 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (127)    37072 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    43070 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    90344 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    32952 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   133871 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.405383 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    34463 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.409383 backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.413383 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.417383 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.449383 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/857b763b8618_add_groups_per_user_image_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/97d8c7aa5e96_add_agent_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ae7d4cd92aa7_add_endpoint_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (127)    29365 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d04592473df7_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e812d42bc34f_remove_unique_constraint_of_endpoints_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (127)    50166 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    33902 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    67131 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/gql_relay.py
--rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    37155 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    52925 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.449383 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24189 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/resource_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    57462 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    56384 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    80293 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.453383 backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   172351 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.453383 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72808 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    36027 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.461383 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1851 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/bai-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   413294 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/graphiql.min.css
--r-xr-xr-x   0 runner    (1001) docker     (127)  3122938 2024-04-05 03:39:46.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/graphiql.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   131882 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/react-dom.production.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/react.production.min.js
--r-xr-xr-x   0 runner    (1001) docker     (127)   870146 2024-04-05 03:39:46.000000 backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/spec-viewer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.465383 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:02.000000 backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:02.469383 backend.ai-manager-24.3.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-05 03:40:00.000000 backend.ai-manager-24.3.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.719063 backend.ai-manager-24.3.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-16 17:08:34.719063 backend.ai-manager-24.3.1rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.651064 backend.ai-manager-24.3.1rc1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.651064 backend.ai-manager-24.3.1rc1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.659064 backend.ai-manager-24.3.1rc1/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/agent_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.663064 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41681 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37072 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43070 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90779 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32952 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133871 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.667064 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34463 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.667064 backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21077 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.675064 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.675064 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.675064 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/revision_history/
+-rw-r--r--   0 runner    (1001) docker     (127)    31967 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/revision_history/23.09.10.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.703064 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/857b763b8618_add_groups_per_user_image_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/97d8c7aa5e96_add_agent_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ae7d4cd92aa7_add_endpoint_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29365 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d04592473df7_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/dddf9be580f5_sync_kernelssessionname_to_real_session_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e812d42bc34f_remove_unique_constraint_of_endpoints_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50166 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33902 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68057 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/gql_relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40691 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53041 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.707064 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24189 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/resource_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57462 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56384 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80293 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.707064 backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   172351 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.707064 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72808 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36027 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.715063 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1851 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/bai-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   413294 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/graphiql.min.css
+-r-xr-xr-x   0 runner    (1001) docker     (127)  3122938 2024-04-16 17:08:31.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/graphiql.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   131882 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/react-dom.production.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/react.production.min.js
+-r-xr-xr-x   0 runner    (1001) docker     (127)   870146 2024-04-16 17:08:31.000000 backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/spec-viewer.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:34.719063 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17750 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-16 17:08:34.000000 backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:08:34.719063 backend.ai-manager-24.3.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-16 17:08:33.000000 backend.ai-manager-24.3.1rc1/setup.py
```

### Comparing `backend.ai-manager-24.3.0rc4/PKG-INFO` & `backend.ai-manager-24.3.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -21,51 +21,51 @@
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: PyJWT~=2.0
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: SQLAlchemy[postgresql_asyncpg]~=1.4.40
 Requires-Dist: aiodataloader-ng~=0.2.1
 Requires-Dist: aiodocker~=0.21.0
-Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp_cors~=0.7
 Requires-Dist: aiohttp_sse>=2.0
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
-Requires-Dist: alembic~=1.12.0
+Requires-Dist: alembic~=1.13.1
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-cli==24.03.0rc4
-Requires-Dist: backend.ai-common==24.03.0rc4
-Requires-Dist: backend.ai-plugin==24.03.0rc4
+Requires-Dist: backend.ai-cli==24.03.1rc1
+Requires-Dist: backend.ai-common==24.03.1rc1
+Requires-Dist: backend.ai-plugin==24.03.1rc1
 Requires-Dist: bcrypt>=4.1.2
 Requires-Dist: callosum~=1.0.3
 Requires-Dist: click~=8.1.7
 Requires-Dist: cryptography>=2.8
-Requires-Dist: etcd-client-py==0.2.4
+Requires-Dist: etcd-client-py==0.3.0
 Requires-Dist: graphene~=3.3.0
 Requires-Dist: lark~=1.1.5
 Requires-Dist: more-itertools~=8.13.0
 Requires-Dist: msgpack>=1.0.5rc1
 Requires-Dist: multidict>=6.0
-Requires-Dist: pydantic~=2.4.2
+Requires-Dist: pydantic~=2.6.4
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: pyzmq~=25.1.2
 Requires-Dist: redis[hiredis]==4.5.5
 Requires-Dist: setproctitle~=1.3.2
 Requires-Dist: tabulate~=0.8.9
 Requires-Dist: tenacity>=8.0
 Requires-Dist: trafaret~=2.1
 Requires-Dist: types-PyYAML
 Requires-Dist: types-aiofiles
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-redis
 Requires-Dist: types-six
 Requires-Dist: types-tabulate
-Requires-Dist: typing_extensions~=4.3
+Requires-Dist: typing_extensions~=4.11
 Requires-Dist: uvloop~=0.19.0; sys_platform != "Windows"
 Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Manager with API Gateway
 ===================================
 
 Package Structure
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/agent_cache.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/agent_cache.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/acl.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/admin.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/auth.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/context.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/etcd.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/events.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/image.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/logs.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/manager.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/resource.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/service.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/session.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1152,23 +1152,30 @@
             new_image_ref: ImageRef = ImageRef(
                 new_canonical,
                 architecture=base_image_ref.architecture,
                 known_registries=["*"],
                 is_local=base_image_ref.is_local,
             )
 
+            image_labels = {
+                "ai.backend.customized-image.owner": f"{params.image_visibility.value}:{image_owner_id}",
+                "ai.backend.customized-image.name": params.image_name,
+                "ai.backend.customized-image.id": customized_image_id,
+            }
+            match params.image_visibility:
+                case CustomizedImageVisibilityScope.USER:
+                    image_labels["ai.backend.customized-image.user.email"] = request["user"][
+                        "email"
+                    ]
+
             # commit image with new tag set
             resp = await root_ctx.registry.commit_session(
                 session,
                 new_image_ref,
-                extra_labels={
-                    "ai.backend.customized-image.owner": f"{params.image_visibility.value}:{image_owner_id}",
-                    "ai.backend.customized-image.name": params.image_name,
-                    "ai.backend.customized-image.id": customized_image_id,
-                },
+                extra_labels=image_labels,
             )
             async for event, _ in background_task_manager.poll_bgtask_event(
                 uuid.UUID(resp["bgtask_id"])
             ):
                 match event:
                     case BgtaskDoneEvent():
                         await reporter.update(increment=1, message="Committed image")
@@ -1311,18 +1318,21 @@
     async with root_ctx.db.begin_session() as db_sess:
         compute_session = await SessionRow.get_session(
             db_sess,
             session_name,
             owner_access_key,
             allow_stale=True,
             for_update=True,
+            kernel_loading_strategy=KernelLoadingStrategy.ALL_KERNELS,
         )
         if compute_session.status != SessionStatus.RUNNING:
             raise InvalidAPIParameters("Can't change name of not running session")
         compute_session.name = new_name
+        for kernel in compute_session.kernels:
+            kernel.session_name = new_name
         await db_sess.commit()
 
     return web.Response(status=204)
 
 
 @server_status_required(READ_ALLOWED)
 @auth_required
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/session_template.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/spec.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/spec.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/stream.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import aiotools
 import attrs
 import trafaret as t
 import zmq
 import zmq.asyncio
 from aiohttp import web
 from aiotools import adefer, apartial
-from etcd_client import GRpcStatusCode, GRpcStatusError
+from etcd_client import GRPCStatusCode, GRPCStatusError
 
 from ai.backend.common import redis_helper
 from ai.backend.common import validators as tx
 from ai.backend.common.events import KernelTerminatingEvent
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import AccessKey, AgentId, KernelId, SessionId
 from ai.backend.manager.idle import AppStreamingStatus
@@ -696,18 +696,18 @@
     try:
         while True:
             try:
                 no_packet_timeout: timedelta = tx.TimeDuration().check(
                     await shared_config.etcd.get("config/idle/app-streaming-packet-timeout")
                     or "5m",
                 )
-            except GRpcStatusError as e:
+            except GRPCStatusError as e:
                 err_detail = e.args[0]
 
-                if err_detail["code"] == GRpcStatusCode.Unavailable:
+                if err_detail["code"] == GRPCStatusCode.Unavailable:
                     log.warning(
                         "stream_conn_tracker_gc(): error while connecting to Etcd server,"
                         " retrying..."
                     )
                 else:
                     raise e
             async with app_ctx.conn_tracker_lock:
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/types.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/utils.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/agent.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/api.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/api.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/context.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/gql.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/image.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/cli/redis.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/cli/redis.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/config.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/harbor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import json
 import logging
 import urllib.parse
 from typing import Any, AsyncIterator, Mapping, Optional, cast
 
 import aiohttp
+import aiohttp.client_exceptions
 import aiotools
 import yarl
 
-from ai.backend.common.docker import arch_name_aliases
+from ai.backend.common.docker import ImageRef, arch_name_aliases
 from ai.backend.common.docker import login as registry_login
 from ai.backend.common.logging import BraceStyleAdapter
 
 from .base import (
     BaseContainerRegistry,
     concurrency_sema,
     progress_reporter,
@@ -121,14 +122,53 @@
                             "digest": config_digest,
                         },
                     }
         await self._read_manifest(image, tag, manifest)
 
 
 class HarborRegistry_v2(BaseContainerRegistry):
+    async def untag(
+        self,
+        image: ImageRef,
+    ) -> None:
+        project, repository = image.name.split("/", maxsplit=1)
+        base_url = (
+            self.registry_url
+            / "api"
+            / "v2.0"
+            / "projects"
+            / project
+            / "repositories"
+            / repository
+            / "artifacts"
+            / image.tag
+        )
+        username = self.registry_info["username"]
+        if username is not None:
+            self.credentials["username"] = username
+        password = self.registry_info["password"]
+        if password is not None:
+            self.credentials["password"] = password
+
+        async with self.prepare_client_session() as (url, sess):
+            rqst_args = {}
+            if self.credentials:
+                rqst_args["auth"] = aiohttp.BasicAuth(
+                    self.credentials["username"],
+                    self.credentials["password"],
+                )
+
+            async with sess.delete(base_url, allow_redirects=False, **rqst_args) as resp:
+                try:
+                    resp.raise_for_status()
+                except aiohttp.client_exceptions.ClientError:
+                    content = await resp.json()
+                    log.warn("response body: {}", content)
+                    raise
+
     async def fetch_repositories(
         self,
         sess: aiohttp.ClientSession,
     ) -> AsyncIterator[str]:
         api_url = self.registry_url / "api" / "v2.0"
         registry_projects = self.registry_info["project"]
         rqst_args = {}
@@ -193,15 +233,15 @@
                     body = await resp.json()
                     for image_info in body:
                         skip_reason: Optional[str] = None
                         tag = image_info["digest"]
                         try:
                             if not image_info["tags"] or len(image_info["tags"]) == 0:
                                 skip_reason = "no tag"
-                                return
+                                continue
                             tag = image_info["tags"][0]["name"]
                             match image_info["manifest_media_type"]:
                                 case self.MEDIA_TYPE_OCI_INDEX:
                                     await self._process_oci_index(
                                         tg, sess, rqst_args, image, image_info
                                     )
                                 case self.MEDIA_TYPE_DOCKER_MANIFEST_LIST:
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/container_registry/local.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/defs.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/defs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/exceptions.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/idle.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/idle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/__init__.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/acl.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/agent.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/857b763b8618_add_groups_per_user_image_storage.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/857b763b8618_add_groups_per_user_image_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/base.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/domain.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/etcd.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/gql.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/gql.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,18 +67,20 @@
     AliasImage,
     ClearImages,
     DealiasImage,
     ForgetImage,
     ForgetImageById,
     Image,
     ImageLoadFilter,
+    ImageNode,
     ModifyImage,
     PreloadImage,
     RescanImages,
     UnloadImage,
+    UntagImageFromRegistry,
 )
 from .kernel import (
     ComputeContainer,
     ComputeContainerList,
     LegacyComputeSession,
     LegacyComputeSessionList,
 )
@@ -201,14 +203,15 @@
     # admin only
     rescan_images = RescanImages.Field()
     preload_image = PreloadImage.Field()
     unload_image = UnloadImage.Field()
     modify_image = ModifyImage.Field()
     forget_image_by_id = ForgetImageById.Field(description="Added since 24.03.0")
     forget_image = ForgetImage.Field()
+    untag_image_from_registry = UntagImageFromRegistry.Field(description="Added in 24.03.1")
     alias_image = AliasImage.Field()
     dealias_image = DealiasImage.Field()
     clear_images = ClearImages.Field()
 
     # super-admin only
     create_keypair_resource_policy = CreateKeyPairResourcePolicy.Field()
     modify_keypair_resource_policy = ModifyKeyPairResourcePolicy.Field()
@@ -342,25 +345,26 @@
                 f"Added since 24.03.0. Available values: {', '.join([p.name for p in ProjectType])}"
             ),
         ),
     )
 
     image = graphene.Field(
         Image,
-        reference=graphene.String(required=True),
+        id=graphene.String(description="Added in 24.03.1"),
+        reference=graphene.String(),
         architecture=graphene.String(default_value=DEFAULT_IMAGE_ARCH),
     )
 
     images = graphene.List(
         Image,
         is_installed=graphene.Boolean(),
         is_operation=graphene.Boolean(),
     )
 
-    customized_images = graphene.List(Image, description="Added since 24.03.0")
+    customized_images = graphene.List(ImageNode, description="Added since 24.03.1")
 
     user = graphene.Field(
         User,
         domain_name=graphene.String(),
         email=graphene.String(),
     )
 
@@ -999,21 +1003,31 @@
             type=[ProjectType[t] for t in type],
         )
 
     @staticmethod
     async def resolve_image(
         root: Any,
         info: graphene.ResolveInfo,
-        reference: str,
-        architecture: str,
+        *,
+        id: str | None = None,
+        reference: str | None = None,
+        architecture: str | None = None,
     ) -> Image:
+        """Loads image information by its ID or reference information. Either ID or reference/architecture pair must be provided."""
         ctx: GraphQueryContext = info.context
         client_role = ctx.user["role"]
         client_domain = ctx.user["domain_name"]
-        item = await Image.load_item(info.context, reference, architecture)
+        if id:
+            item = await Image.load_item_by_id(info.context, uuid.UUID(id))
+        else:
+            if not (reference and architecture):
+                raise InvalidAPIParameters(
+                    "reference/architecture and id can't be omitted at the same time!"
+                )
+            item = await Image.load_item(info.context, reference, architecture)
         if client_role == UserRole.SUPERADMIN:
             pass
         elif client_role in (UserRole.ADMIN, UserRole.USER):
             items = await Image.filter_allowed(info.context, [item], client_domain)
             if not items:
                 raise ImageNotFound
             item = items[0]
@@ -1021,30 +1035,30 @@
             raise InvalidAPIParameters("Unknown client role")
         return item
 
     @staticmethod
     async def resolve_customized_images(
         root: Any,
         info: graphene.ResolveInfo,
-    ) -> Sequence[Image]:
+    ) -> Sequence[ImageNode]:
         ctx: GraphQueryContext = info.context
         client_role = ctx.user["role"]
         client_domain = ctx.user["domain_name"]
         items = await Image.load_all(ctx, filters=set((ImageLoadFilter.CUSTOMIZED_ONLY,)))
         if client_role == UserRole.SUPERADMIN:
             pass
         elif client_role in (UserRole.ADMIN, UserRole.USER):
             items = await Image.filter_allowed(
                 info.context,
                 items,
                 client_domain,
             )
         else:
             raise InvalidAPIParameters("Unknown client role")
-        return items
+        return [ImageNode.from_legacy_image(i) for i in items]
 
     @staticmethod
     async def resolve_images(
         root: Any,
         info: graphene.ResolveInfo,
         *,
         is_installed=None,
@@ -1743,23 +1757,31 @@
         return ComputeContainerList(items, total_count)
 
     @staticmethod
     @scoped_query(autofill_user=False, user_key="access_key")
     async def resolve_compute_container(
         root: Any,
         info: graphene.ResolveInfo,
-        container_id: str,
+        id: str,
+        *,
+        domain_name: str | None = None,
+        access_key: AccessKey | None = None,
     ) -> ComputeContainer:
         # We need to check the group membership of the designated kernel,
         # but practically a user cannot guess the IDs of kernels launched
         # by other users and in other groups.
         # Let's just protect the domain/user boundary here.
         graph_ctx: GraphQueryContext = info.context
-        loader = graph_ctx.dataloader_manager.get_loader(graph_ctx, "ComputeContainer.detail")
-        return await loader.load(container_id)
+        loader = graph_ctx.dataloader_manager.get_loader(
+            graph_ctx,
+            "ComputeContainer.detail",
+            domain_name=domain_name,
+            access_key=access_key,
+        )
+        return await loader.load(id)
 
     @staticmethod
     @scoped_query(autofill_user=False, user_key="access_key")
     async def resolve_compute_session_list(
         root: Any,
         info: graphene.ResolveInfo,
         limit: int,
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/gql_relay.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/gql_relay.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/group.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/image.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     "ImageAliasRow",
     "ImageLoadFilter",
     "ImageRow",
     "Image",
     "PreloadImage",
     "RescanImages",
     "ForgetImage",
+    "ForgetImageById",
+    "UntagImageFromRegistry",
     "ModifyImage",
     "AliasImage",
     "DealiasImage",
     "ClearImages",
 )
 
 
@@ -613,14 +615,27 @@
         graph_ctx: GraphQueryContext,
         image_refs: Sequence[ImageRef],
     ) -> Sequence[Optional[Image]]:
         image_names = [x.canonical for x in image_refs]
         return await cls.batch_load_by_canonical(graph_ctx, image_names)
 
     @classmethod
+    async def load_item_by_id(
+        cls,
+        ctx: GraphQueryContext,
+        id: UUID,
+    ) -> Image:
+        async with ctx.db.begin_readonly_session() as session:
+            row = await ImageRow.get(session, id, load_aliases=True)
+            if not row:
+                raise ImageNotFound
+
+            return await cls.from_row(ctx, row)
+
+    @classmethod
     async def load_item(
         cls,
         ctx: GraphQueryContext,
         reference: str,
         architecture: str,
     ) -> Image:
         try:
@@ -745,14 +760,31 @@
                 )
                 for k, v in row.resources.items()
             ],
             supported_accelerators=(row.accelerators or "").split(","),
         )
 
     @classmethod
+    def from_legacy_image(cls, row: Image) -> ImageNode:
+        return cls(
+            id=row.id,
+            name=row.name,
+            humanized_name=row.humanized_name,
+            tag=row.tag,
+            registry=row.registry,
+            architecture=row.architecture,
+            is_local=row.is_local,
+            digest=row.digest,
+            labels=row.labels,
+            size_bytes=row.size_bytes,
+            resource_limits=row.resource_limits,
+            supported_accelerators=row.supported_accelerators,
+        )
+
+    @classmethod
     async def get_node(cls, info: graphene.ResolveInfo, id: str) -> ImageNode:
         graph_ctx: GraphQueryContext = info.context
 
         _, image_id = AsyncNode.resolve_global_id(info, id)
         query = sa.select(ImageRow).where(ImageRow.id == image_id)
         async with graph_ctx.db.begin_readonly_session() as db_session:
             image_row = await db_session.scalar(query)
@@ -842,45 +874,50 @@
     )
 
     class Arguments:
         image_id = graphene.String(required=True)
 
     ok = graphene.Boolean()
     msg = graphene.String()
+    image = graphene.Field(ImageNode, description="Added since 24.03.1.")
 
     @staticmethod
     async def mutate(
         root: Any,
         info: graphene.ResolveInfo,
         image_id: str,
     ) -> ForgetImageById:
+        _, raw_image_id = AsyncNode.resolve_global_id(info, image_id)
+        if not raw_image_id:
+            raw_image_id = image_id
+
+        try:
+            _image_id = UUID(raw_image_id)
+        except ValueError:
+            raise ObjectNotFound("image")
+
         log.info("forget image {0} by API request", image_id)
         ctx: GraphQueryContext = info.context
         client_role = ctx.user["role"]
 
         async with ctx.db.begin_session() as session:
-            try:
-                _image_id = UUID(image_id)
-            except ValueError:
-                raise ObjectNotFound("image")
-
             image_row = await ImageRow.get(session, _image_id)
             if not image_row:
                 raise ObjectNotFound("image")
             if client_role != UserRole.SUPERADMIN:
                 customized_image_owner = (image_row.labels or {}).get(
                     "ai.backend.customized-image.owner"
                 )
                 if (
                     not customized_image_owner
                     or customized_image_owner != f"user:{ctx.user['uuid']}"
                 ):
                     return ForgetImageById(ok=False, msg="Forbidden")
             await session.delete(image_row)
-        return ForgetImageById(ok=True, msg="")
+            return ForgetImageById(ok=True, msg="", image=ImageNode.from_row(image_row))
 
 
 class ForgetImage(graphene.Mutation):
     allowed_roles = (
         UserRole.SUPERADMIN,
         UserRole.ADMIN,
         UserRole.USER,
@@ -888,14 +925,15 @@
 
     class Arguments:
         reference = graphene.String(required=True)
         architecture = graphene.String(default_value=DEFAULT_IMAGE_ARCH)
 
     ok = graphene.Boolean()
     msg = graphene.String()
+    image = graphene.Field(ImageNode, description="Added since 24.03.1.")
 
     @staticmethod
     async def mutate(
         root: Any,
         info: graphene.ResolveInfo,
         reference: str,
         architecture: str,
@@ -918,15 +956,78 @@
                 )
                 if (
                     not customized_image_owner
                     or customized_image_owner != f"user:{ctx.user['uuid']}"
                 ):
                     return ForgetImage(ok=False, msg="Forbidden")
             await session.delete(image_row)
-        return ForgetImage(ok=True, msg="")
+            return ForgetImage(ok=True, msg="", image=ImageNode.from_row(image_row))
+
+
+class UntagImageFromRegistry(graphene.Mutation):
+    """Added in 24.03.1"""
+
+    allowed_roles = (
+        UserRole.SUPERADMIN,
+        UserRole.ADMIN,
+        UserRole.USER,
+    )
+
+    class Arguments:
+        image_id = graphene.String(required=True)
+
+    ok = graphene.Boolean()
+    msg = graphene.String()
+    image = graphene.Field(ImageNode, description="Added since 24.03.1.")
+
+    @staticmethod
+    async def mutate(
+        root: Any,
+        info: graphene.ResolveInfo,
+        image_id: str,
+    ) -> UntagImageFromRegistry:
+        from ai.backend.manager.container_registry.harbor import HarborRegistry_v2
+
+        _, raw_image_id = AsyncNode.resolve_global_id(info, image_id)
+        if not raw_image_id:
+            raw_image_id = image_id
+
+        try:
+            _image_id = UUID(raw_image_id)
+        except ValueError:
+            raise ObjectNotFound("image")
+
+        log.info("remove image from registry {0} by API request", str(_image_id))
+        ctx: GraphQueryContext = info.context
+        client_role = ctx.user["role"]
+
+        async with ctx.db.begin_readonly_session() as session:
+            image_row = await ImageRow.get(session, _image_id)
+            if not image_row:
+                raise ImageNotFound
+            if client_role != UserRole.SUPERADMIN:
+                customized_image_owner = (image_row.labels or {}).get(
+                    "ai.backend.customized-image.owner"
+                )
+                if (
+                    not customized_image_owner
+                    or customized_image_owner != f"user:{ctx.user['uuid']}"
+                ):
+                    return UntagImageFromRegistry(ok=False, msg="Forbidden")
+
+            registry_info = await ctx.shared_config.get_container_registry(
+                image_row.image_ref.registry
+            )
+            if registry_info.get("type", "") != "harbor2":
+                raise NotImplementedError("This feature is only supported for Harbor 2 registries")
+
+        scanner = HarborRegistry_v2(ctx.db, image_row.image_ref.registry, registry_info)
+        await scanner.untag(image_row.image_ref)
+
+        return UntagImageFromRegistry(ok=True, msg="", image=ImageNode.from_row(image_row))
 
 
 class AliasImage(graphene.Mutation):
     allowed_roles = (UserRole.SUPERADMIN,)
 
     class Arguments:
         alias = graphene.String(required=True)
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/kernel.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -788,14 +788,15 @@
     class Meta:
         interfaces = (Item,)
 
     # identity
     idx = graphene.Int()  # legacy
     role = graphene.String()  # legacy
     hostname = graphene.String()  # legacy
+    kernel_id = graphene.UUID(description="Added in 24.03.1.")
     cluster_idx = graphene.Int()
     local_rank = graphene.Int()
     cluster_role = graphene.String()
     cluster_hostname = graphene.String()
     session_id = graphene.UUID()  # owner session
 
     # image
@@ -835,14 +836,15 @@
             hide_agents = False
         else:
             hide_agents = ctx.local_config["manager"]["hide-agents"]
         status_history = row.status_history or {}
         return {
             # identity
             "id": row.id,
+            "kernel_id": row.id,
             "idx": row.cluster_idx,
             "role": row.cluster_role,
             "hostname": row.cluster_hostname,
             "cluster_idx": row.cluster_idx,
             "local_rank": row.local_rank,
             "cluster_role": row.cluster_role,
             "cluster_hostname": row.cluster_hostname,
@@ -1000,16 +1002,16 @@
             qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         if order is not None:
             qoparser = QueryOrderParser(cls._queryorder_colmap)
             query = qoparser.append_ordering(query, order)
         else:
             query = query.order_by(*DEFAULT_KERNEL_ORDERING)
-        async with ctx.db.begin_readonly_session() as conn:
-            return [cls.from_row(ctx, r) async for r in (await conn.stream(query))]
+        async with ctx.db.begin_readonly_session() as db_session:
+            return [cls.from_row(ctx, r) async for r in (await db_session.stream_scalars(query))]
 
     @classmethod
     async def batch_load_by_session(
         cls,
         ctx: GraphQueryContext,
         session_ids: Sequence[SessionId],
     ) -> Sequence[Sequence[ComputeContainer]]:
```

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/keypair.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/__init__.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/ordering.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/resource_usage.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/resource_usage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/routing.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/session.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/session_template.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/storage.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/user.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/utils.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/models/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/openapi.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/openapi.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/pglock.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/registry.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/dispatcher.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/predicates.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/server.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/types.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/utils.py` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/bai-icon.svg` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/bai-icon.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/graphiql.min.css` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/graphiql.min.css`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/graphiql.min.js` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/graphiql.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/react-dom.production.min.js` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/react-dom.production.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/react.production.min.js` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/react.production.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/ai/backend/manager/vendor/spec-viewer.js` & `backend.ai-manager-24.3.1rc1/ai/backend/manager/vendor/spec-viewer.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -21,51 +21,51 @@
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: PyJWT~=2.0
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: SQLAlchemy[postgresql_asyncpg]~=1.4.40
 Requires-Dist: aiodataloader-ng~=0.2.1
 Requires-Dist: aiodocker~=0.21.0
-Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp_cors~=0.7
 Requires-Dist: aiohttp_sse>=2.0
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
-Requires-Dist: alembic~=1.12.0
+Requires-Dist: alembic~=1.13.1
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-cli==24.03.0rc4
-Requires-Dist: backend.ai-common==24.03.0rc4
-Requires-Dist: backend.ai-plugin==24.03.0rc4
+Requires-Dist: backend.ai-cli==24.03.1rc1
+Requires-Dist: backend.ai-common==24.03.1rc1
+Requires-Dist: backend.ai-plugin==24.03.1rc1
 Requires-Dist: bcrypt>=4.1.2
 Requires-Dist: callosum~=1.0.3
 Requires-Dist: click~=8.1.7
 Requires-Dist: cryptography>=2.8
-Requires-Dist: etcd-client-py==0.2.4
+Requires-Dist: etcd-client-py==0.3.0
 Requires-Dist: graphene~=3.3.0
 Requires-Dist: lark~=1.1.5
 Requires-Dist: more-itertools~=8.13.0
 Requires-Dist: msgpack>=1.0.5rc1
 Requires-Dist: multidict>=6.0
-Requires-Dist: pydantic~=2.4.2
+Requires-Dist: pydantic~=2.6.4
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: pyzmq~=25.1.2
 Requires-Dist: redis[hiredis]==4.5.5
 Requires-Dist: setproctitle~=1.3.2
 Requires-Dist: tabulate~=0.8.9
 Requires-Dist: tenacity>=8.0
 Requires-Dist: trafaret~=2.1
 Requires-Dist: types-PyYAML
 Requires-Dist: types-aiofiles
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-redis
 Requires-Dist: types-six
 Requires-Dist: types-tabulate
-Requires-Dist: typing_extensions~=4.3
+Requires-Dist: typing_extensions~=4.11
 Requires-Dist: uvloop~=0.19.0; sys_platform != "Windows"
 Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Manager with API Gateway
 ===================================
 
 Package Structure
```

### Comparing `backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 ai/backend/manager/models/storage.py
 ai/backend/manager/models/user.py
 ai/backend/manager/models/utils.py
 ai/backend/manager/models/vfolder.py
 ai/backend/manager/models/alembic/__init__.py
 ai/backend/manager/models/alembic/env.py
 ai/backend/manager/models/alembic/script.py.mako
+ai/backend/manager/models/alembic/revision_history/23.09.10.json
 ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
 ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
 ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py
 ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
 ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
 ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
 ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
@@ -223,14 +224,15 @@
 ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
 ai/backend/manager/models/alembic/versions/d643752544de_.py
 ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
 ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
 ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
 ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
 ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+ai/backend/manager/models/alembic/versions/dddf9be580f5_sync_kernelssessionname_to_real_session_.py
 ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
 ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
 ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
 ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
 ai/backend/manager/models/alembic/versions/e812d42bc34f_remove_unique_constraint_of_endpoints_.py
 ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
 ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
```

### Comparing `backend.ai-manager-24.3.0rc4/backend.ai_manager.egg-info/requires.txt` & `backend.ai-manager-24.3.1rc1/backend.ai_manager.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 PyJWT~=2.0
 PyYAML~=6.0
 SQLAlchemy[postgresql_asyncpg]~=1.4.40
 aiodataloader-ng~=0.2.1
 aiodocker~=0.21.0
-aiofiles~=0.8.0
+aiofiles~=23.2.1
 aiohttp_cors~=0.7
 aiohttp_sse>=2.0
 aiohttp~=3.9.1
 aiomonitor~=0.7.0
 aiotools~=1.7.0
-alembic~=1.12.0
+alembic~=1.13.1
 async_timeout~=4.0
 attrs>=20.3
-backend.ai-cli==24.03.0rc4
-backend.ai-common==24.03.0rc4
-backend.ai-plugin==24.03.0rc4
+backend.ai-cli==24.03.1rc1
+backend.ai-common==24.03.1rc1
+backend.ai-plugin==24.03.1rc1
 bcrypt>=4.1.2
 callosum~=1.0.3
 click~=8.1.7
 cryptography>=2.8
-etcd-client-py==0.2.4
+etcd-client-py==0.3.0
 graphene~=3.3.0
 lark~=1.1.5
 more-itertools~=8.13.0
 msgpack>=1.0.5rc1
 multidict>=6.0
-pydantic~=2.4.2
+pydantic~=2.6.4
 python-dateutil>=2.8
 pyzmq~=25.1.2
 redis[hiredis]==4.5.5
 setproctitle~=1.3.2
 tabulate~=0.8.9
 tenacity>=8.0
 trafaret~=2.1
 types-PyYAML
 types-aiofiles
 types-python-dateutil
 types-redis
 types-six
 types-tabulate
-typing_extensions~=4.3
+typing_extensions~=4.11
 yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 [:sys_platform != "Windows"]
 uvloop~=0.19.0
```

### Comparing `backend.ai-manager-24.3.0rc4/backend_shim.py` & `backend.ai-manager-24.3.1rc1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc4/setup.py` & `backend.ai-manager-24.3.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,54 +37,54 @@
     },
     'install_requires': (
         'PyJWT~=2.0',
         'PyYAML~=6.0',
         'SQLAlchemy[postgresql_asyncpg]~=1.4.40',
         'aiodataloader-ng~=0.2.1',
         'aiodocker~=0.21.0',
-        'aiofiles~=0.8.0',
+        'aiofiles~=23.2.1',
         'aiohttp_cors~=0.7',
         'aiohttp_sse>=2.0',
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
-        'alembic~=1.12.0',
+        'alembic~=1.13.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==24.03.0rc4
+        """backend.ai-cli==24.03.1rc1
 """,
-        """backend.ai-common==24.03.0rc4
+        """backend.ai-common==24.03.1rc1
 """,
-        """backend.ai-plugin==24.03.0rc4
+        """backend.ai-plugin==24.03.1rc1
 """,
         'bcrypt>=4.1.2',
         'callosum~=1.0.3',
         'click~=8.1.7',
         'cryptography>=2.8',
-        'etcd-client-py==0.2.4',
+        'etcd-client-py==0.3.0',
         'graphene~=3.3.0',
         'lark~=1.1.5',
         'more-itertools~=8.13.0',
         'msgpack>=1.0.5rc1',
         'multidict>=6.0',
-        'pydantic~=2.4.2',
+        'pydantic~=2.6.4',
         'python-dateutil>=2.8',
         'pyzmq~=25.1.2',
         'redis[hiredis]==4.5.5',
         'setproctitle~=1.3.2',
         'tabulate~=0.8.9',
         'tenacity>=8.0',
         'trafaret~=2.1',
         'types-PyYAML',
         'types-aiofiles',
         'types-python-dateutil',
         'types-redis',
         'types-six',
         'types-tabulate',
-        'typing_extensions~=4.3',
+        'typing_extensions~=4.11',
         'uvloop~=0.19.0; sys_platform != "Windows"',
         'yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2',
     ),
     'license': 'LGPLv3',
     'long_description': """Backend.AI Manager with API Gateway
 ===================================
 
@@ -357,14 +357,15 @@
             'VERSION',
             'py.typed',
         ),
         'ai.backend.manager.api': (
             'py.typed',
         ),
         'ai.backend.manager.models.alembic': (
+            'revision_history/23.09.10.json',
             'script.py.mako',
         ),
         'ai.backend.manager.vendor': (
             '__init__.py',
             'bai-icon.svg',
             'graphiql.min.css',
             'graphiql.min.js',
@@ -388,11 +389,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc4
+    'version': """24.03.1rc1
 """,
     'zip_safe': False,
 })
```

