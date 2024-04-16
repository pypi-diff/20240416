# Comparing `tmp/deadline-0.47.2.tar.gz` & `tmp/deadline-0.47.3.tar.gz`

## Comparing `deadline-0.47.2.tar` & `deadline-0.47.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.47.2/THIRD_PARTY_LICENSES
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.2/_version.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/__main__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/_version.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/exceptions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/py.typed
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/__init__.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_list_apis.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_loginout.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_queue_parameters.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_session.py
--rw-r--r--   0        0        0    17160 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_submit_job_bundle.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_telemetry.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/__init__.py
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_common.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_deadline_cli.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_deadline_web_url.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/deadline_cli_main.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/deadline_dev_gui_main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/_sigint_handler.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/auth_group.py
--rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/bundle_group.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/config_group.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/farm_group.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/fleet_group.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/handle_web_url_command.py
--rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/job_group.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/queue_group.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/worker_group.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/config/__init__.py
--rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/config/config_file.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/_yaml.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/adaptors.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/job_template.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/loader.py
--rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/parameters.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/submission.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/cli_job_submitter.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/deadline_authentication_status.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dev_application.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/job_bundle_submitter.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dataclasses/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/_types.py
--rw-r--r--   0        0        0    34201 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_config_dialog.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_login_dialog.py
--rw-r--r--   0        0        0    25968 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/deadline_logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/info.svg
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/cli_job_settings_tab.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
--rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/host_requirements_tab.py
--rw-r--r--   0        0        0    14402 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/job_attachments_tab.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
--rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/openjd_parameters_widget.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/path_widgets.py
--rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/shared_job_settings_tab.py
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/spinbox_widgets.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/README.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_utils.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_version.py
--rw-r--r--   0        0        0    26842 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_sync.py
--rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/download.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/exceptions.py
--rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/models.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/os_file_permission.py
--rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/progress_tracker.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/py.typed
--rw-r--r--   0        0        0    51260 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/upload.py
--rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/vfs.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/aws_clients.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/aws_config.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/deadline.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_windows/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_windows/file.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/_canonical_json.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/base_manifest.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/decode.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/manifest_model.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/versions.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/__init__.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/cache_db.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/hash_cache.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/s3_check_cache.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.2/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.47.2/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.47.2/NOTICE
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.47.2/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.47.2/hatch.toml
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 deadline-0.47.2/pyproject.toml
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 deadline-0.47.2/PKG-INFO
+-rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.47.3/THIRD_PARTY_LICENSES
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.3/_version.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/__main__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/_version.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/exceptions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/py.typed
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/__init__.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_list_apis.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_loginout.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_queue_parameters.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_session.py
+-rw-r--r--   0        0        0    17160 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_submit_job_bundle.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/api/_telemetry.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/__init__.py
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_common.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_deadline_cli.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_deadline_web_url.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/deadline_cli_main.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/deadline_dev_gui_main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/_sigint_handler.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/auth_group.py
+-rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/bundle_group.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/config_group.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/farm_group.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/fleet_group.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/handle_web_url_command.py
+-rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/job_group.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/queue_group.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/cli/_groups/worker_group.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/config/__init__.py
+-rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/config/config_file.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/_yaml.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/adaptors.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/job_template.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/loader.py
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/parameters.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/job_bundle/submission.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/cli_job_submitter.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/deadline_authentication_status.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dev_application.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/job_bundle_submitter.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dataclasses/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/_types.py
+-rw-r--r--   0        0        0    34201 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_config_dialog.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_login_dialog.py
+-rw-r--r--   0        0        0    26025 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/deadline_logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/info.svg
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/cli_job_settings_tab.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
+-rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/host_requirements_tab.py
+-rw-r--r--   0        0        0    14402 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/job_attachments_tab.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
+-rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/openjd_parameters_widget.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/path_widgets.py
+-rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/shared_job_settings_tab.py
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/client/ui/widgets/spinbox_widgets.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/README.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/__init__.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_utils.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_version.py
+-rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_sync.py
+-rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/download.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/exceptions.py
+-rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/models.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/os_file_permission.py
+-rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/progress_tracker.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/py.typed
+-rw-r--r--   0        0        0    52783 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/upload.py
+-rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/vfs.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/__init__.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/aws_clients.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/aws_config.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_aws/deadline.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_windows/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/_windows/file.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/_canonical_json.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/base_manifest.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/decode.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/manifest_model.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/versions.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/__init__.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/cache_db.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/hash_cache.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.47.3/src/deadline/job_attachments/caches/s3_check_cache.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.47.3/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.47.3/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.47.3/NOTICE
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.47.3/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.47.3/hatch.toml
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 deadline-0.47.3/pyproject.toml
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 deadline-0.47.3/PKG-INFO
```

### Comparing `deadline-0.47.2/THIRD_PARTY_LICENSES` & `deadline-0.47.3/THIRD_PARTY_LICENSES`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/exceptions.py` & `deadline-0.47.3/src/deadline/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/__init__.py` & `deadline-0.47.3/src/deadline/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/_list_apis.py` & `deadline-0.47.3/src/deadline/client/api/_list_apis.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/_loginout.py` & `deadline-0.47.3/src/deadline/client/api/_loginout.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/_queue_parameters.py` & `deadline-0.47.3/src/deadline/client/api/_queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/_session.py` & `deadline-0.47.3/src/deadline/client/api/_session.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/_submit_job_bundle.py` & `deadline-0.47.3/src/deadline/client/api/_submit_job_bundle.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/api/_telemetry.py` & `deadline-0.47.3/src/deadline/client/api/_telemetry.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_common.py` & `deadline-0.47.3/src/deadline/client/cli/_common.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_deadline_cli.py` & `deadline-0.47.3/src/deadline/client/cli/_deadline_cli.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_deadline_web_url.py` & `deadline-0.47.3/src/deadline/client/cli/_deadline_web_url.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/deadline_dev_gui_main.py` & `deadline-0.47.3/src/deadline/client/cli/deadline_dev_gui_main.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/_sigint_handler.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/_sigint_handler.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/auth_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/auth_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/bundle_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/bundle_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/config_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/config_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/farm_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/farm_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/fleet_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/fleet_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/handle_web_url_command.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/handle_web_url_command.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/job_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/job_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/queue_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/queue_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/cli/_groups/worker_group.py` & `deadline-0.47.3/src/deadline/client/cli/_groups/worker_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/config/__init__.py` & `deadline-0.47.3/src/deadline/client/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/config/config_file.py` & `deadline-0.47.3/src/deadline/client/config/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/__init__.py` & `deadline-0.47.3/src/deadline/client/job_bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/_yaml.py` & `deadline-0.47.3/src/deadline/client/job_bundle/_yaml.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/adaptors.py` & `deadline-0.47.3/src/deadline/client/job_bundle/adaptors.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/job_template.py` & `deadline-0.47.3/src/deadline/client/job_bundle/job_template.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/loader.py` & `deadline-0.47.3/src/deadline/client/job_bundle/loader.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/parameters.py` & `deadline-0.47.3/src/deadline/client/job_bundle/parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/job_bundle/submission.py` & `deadline-0.47.3/src/deadline/client/job_bundle/submission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/__init__.py` & `deadline-0.47.3/src/deadline/client/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/cli_job_submitter.py` & `deadline-0.47.3/src/deadline/client/ui/cli_job_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/deadline_authentication_status.py` & `deadline-0.47.3/src/deadline/client/ui/deadline_authentication_status.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/dev_application.py` & `deadline-0.47.3/src/deadline/client/ui/dev_application.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/job_bundle_submitter.py` & `deadline-0.47.3/src/deadline/client/ui/job_bundle_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/dataclasses/__init__.py` & `deadline-0.47.3/src/deadline/client/ui/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_config_dialog.py` & `deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_config_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_login_dialog.py` & `deadline-0.47.3/src/deadline/client/ui/dialogs/deadline_login_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py` & `deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,14 +335,15 @@
             # This thread is only started if self._asset_manager is set.
             upload_summary, attachment_settings = cast(
                 S3AssetManager, self._asset_manager
             ).upload_assets(
                 manifests=manifests,
                 on_uploading_assets=_update_upload_progress,
                 s3_check_cache_dir=config_file.get_cache_directory(),
+                manifest_write_dir=self._job_bundle_dir,
             )
 
             logger.info("Finished uploading job attachments files.")
 
             self.upload_thread_succeeded.emit(upload_summary, attachment_settings.to_dict())
         except AssetSyncCancelledError as e:
             # If it wasn't canceled, send the exception to the dialog
```

### Comparing `deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py` & `deadline-0.47.3/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/resources/deadline_logo.svg` & `deadline-0.47.3/src/deadline/client/ui/resources/deadline_logo.svg`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/resources/blender_example_bundle/template.yaml` & `deadline-0.47.3/src/deadline/client/ui/resources/blender_example_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/resources/cli_job_bundle/template.yaml` & `deadline-0.47.3/src/deadline/client/ui/resources/cli_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml` & `deadline-0.47.3/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/cli_job_settings_tab.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/cli_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/host_requirements_tab.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/host_requirements_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/job_attachments_tab.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/job_attachments_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/job_bundle_settings_tab.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/job_bundle_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/openjd_parameters_widget.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/openjd_parameters_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/path_widgets.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/path_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/shared_job_settings_tab.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/shared_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/client/ui/widgets/spinbox_widgets.py` & `deadline-0.47.3/src/deadline/client/ui/widgets/spinbox_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/README.md` & `deadline-0.47.3/src/deadline/job_attachments/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 When making a job submission, the job attachments library makes a snapshot of all of the files included in the submission. The contents of each file are hashed, and the files are uploaded to the S3 bucket associated with the queue you are submitting to. This way, if the files haven't changed since a previous submission, the hash will be the same and the files will not be re-uploaded. 
 
 These snapshots are encapsulated in one or more [`asset_manifests`](asset_manifests). Asset manifests include the local file path and associated hash of every file included in the submission, plus some metadata such as the file size and last modified time. Asset manifests are uploaded to your job attachments S3 bucket alongside your files.
 
 When starting work, the worker downloads the manifest associated with your job, and recreates the file structure of your submission locally, either downloading all files at once, or as needed if using the [virtual][vfs] job attachments filesystem type. When a task completes, the worker creates a new manifest for any outputs that were specified in the job submission, and uploads the manifest and the outputs back to your S3 bucket.
 
+Manifest files are written to a `manifests` directory within each job bundle that is added to the job history if submitted through the GUI (default: `~/.deadline/job_history`). A corresponding `manifest_s3_mapping` file is created alongside manifests, which specifies each local manifest file with the S3 manifest path in the submitted job's job attachments metadata.
+
 [vfs]: https://docs.aws.amazon.com/deadline-cloud/latest/userguide/storage-virtual.html
 
 ## Local Cache Files
 
 In order to further improve submission time, there are currently two local [`caches`](caches), which are simple SQLite databases that cache file information locally. These include:
 
 1. [`Hash Cache`](caches/hash_cache.py): a cache recording a file name and corresponding hash of its contents at a specific time. If a file does not exist in the hash cache, or its last modified time is later than the time in the cache, the file will be hashed and the cache updated.
```

### Comparing `deadline-0.47.2/src/deadline/job_attachments/_utils.py` & `deadline-0.47.3/src/deadline/job_attachments/_utils.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_sync.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 """ Module for File Attachment synching """
 from __future__ import annotations
 import os
+import shutil
 import sys
 import time
 from io import BytesIO
 from logging import Logger, LoggerAdapter, getLogger
 from math import trunc
 from pathlib import Path, PurePosixPath
 from typing import Any, Callable, DefaultDict, Dict, List, Optional, Tuple, Type, Union
@@ -333,14 +334,27 @@
         # (in microseconds). This is used to later determine which files have been modified or
         # newly created during the session and need to be uploaded as output.
         for local_root, merged_manifest in merged_manifests_by_root.items():
             for manifest_path in merged_manifest.paths:
                 abs_path = str(Path(local_root) / manifest_path.path)
                 self.synced_assets_mtime[abs_path] = Path(abs_path).stat().st_mtime_ns
 
+    def _ensure_disk_capacity(self, session_dir: Path, total_input_bytes: int) -> None:
+        """
+        Raises an AssetSyncError if the given input bytes is larger than the available disk space.
+        """
+        disk_free: int = shutil.disk_usage(session_dir).free
+        if total_input_bytes > disk_free:
+            input_size_readable = _human_readable_file_size(total_input_bytes)
+            disk_free_readable = _human_readable_file_size(disk_free)
+            raise AssetSyncError(
+                "Error occurred while attempting to sync input files: "
+                f"Total file size required for download ({input_size_readable}) is larger than available disk space ({disk_free_readable})"
+            )
+
     def sync_inputs(
         self,
         s3_settings: Optional[JobAttachmentS3Settings],
         attachments: Optional[Attachments],
         queue_id: str,
         job_id: str,
         session_dir: Path,
@@ -443,22 +457,24 @@
                 for root, manifests in manifests_by_root.items():
                     dir_name = _get_unique_dest_dir_name(root)
                     local_root = str(session_dir.joinpath(dir_name))
                     grouped_manifests_by_root[local_root].extend(manifests)
 
         # Merge the manifests in each root into a single manifest
         merged_manifests_by_root: dict[str, BaseAssetManifest] = dict()
+        total_input_size: int = 0
         for root, manifests in grouped_manifests_by_root.items():
             merged_manifest = merge_asset_manifests(manifests)
 
             if merged_manifest:
                 merged_manifests_by_root[root] = merged_manifest
+                total_input_size += merged_manifest.totalSize  # type: ignore[attr-defined]
 
         # Download
-
+        # Virtual Download Flow
         if (
             attachments.fileSystem == JobAttachmentsFileSystem.VIRTUAL.value
             and sys.platform != "win32"
             and fs_permission_settings is not None
             and os_env_vars is not None
             and "AWS_PROFILE" in os_env_vars
             and isinstance(fs_permission_settings, PosixFileSystemPermissionSettings)
@@ -478,14 +494,16 @@
                 self._record_attachment_mtimes(merged_manifests_by_root)
                 return (summary_statistics, list(pathmapping_rules.values()))
             except VFSExecutableMissingError:
                 logger.error(
                     f"Virtual File System not found, falling back to {JobAttachmentsFileSystem.COPIED} for JobAttachmentsFileSystem."
                 )
 
+        # Copied Download flow
+        self._ensure_disk_capacity(session_dir, total_input_size)
         try:
             download_summary_statistics = download_files_from_manifests(
                 s3_bucket=s3_settings.s3BucketName,
                 manifests_by_root=merged_manifests_by_root,
                 cas_prefix=s3_settings.full_cas_prefix(),
                 fs_permission_settings=fs_permission_settings,
                 session=self.session,
@@ -540,37 +558,42 @@
             return SummaryStatistics()
 
         all_output_files: List[OutputFile] = []
 
         storage_profiles_source_paths = list(storage_profiles_path_mapping_rules.keys())
 
         for manifest_properties in attachments.manifests:
+            session_root = session_dir
             local_root: Path = Path()
             if (
                 len(storage_profiles_path_mapping_rules) > 0
                 and manifest_properties.fileSystemLocationName
             ):
                 if manifest_properties.rootPath in storage_profiles_source_paths:
                     local_root = Path(
                         storage_profiles_path_mapping_rules[manifest_properties.rootPath]
                     )
+                    # We use session_root to filter out any files resolved to a location outside
+                    # of that directory. If storage profile's path mapping rules are available,
+                    # we can consider the session_root to be the mapped-storage profile path.
+                    session_root = local_root
                 else:
                     raise AssetSyncError(
                         "Error occurred while attempting to sync output files: "
                         f"No path mapping rule found for the source path {manifest_properties.rootPath}"
                     )
             else:
                 dir_name: str = _get_unique_dest_dir_name(manifest_properties.rootPath)
                 local_root = session_dir.joinpath(dir_name)
 
             output_files: List[OutputFile] = self._get_output_files(
                 manifest_properties,
                 s3_settings,
                 local_root,
-                session_dir,
+                session_root,
             )
             if output_files:
                 output_manifest = self._generate_output_manifest(output_files)
                 session_action_id_with_time_stamp = (
                     f"{_float_to_iso_datetime_string(start_time)}_{session_action_id}"
                 )
                 full_output_prefix = s3_settings.full_output_prefix(
```

### Comparing `deadline-0.47.2/src/deadline/job_attachments/download.py` & `deadline-0.47.3/src/deadline/job_attachments/download.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/exceptions.py` & `deadline-0.47.3/src/deadline/job_attachments/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/models.py` & `deadline-0.47.3/src/deadline/job_attachments/models.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/os_file_permission.py` & `deadline-0.47.3/src/deadline/job_attachments/os_file_permission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/progress_tracker.py` & `deadline-0.47.3/src/deadline/job_attachments/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/upload.py` & `deadline-0.47.3/src/deadline/job_attachments/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         job_attachment_settings: JobAttachmentS3Settings,
         manifest: BaseAssetManifest,
         partial_manifest_prefix: str,
         source_root: Path,
         file_system_location_name: Optional[str] = None,
         progress_tracker: Optional[ProgressTracker] = None,
         s3_check_cache_dir: Optional[str] = None,
+        manifest_write_dir: Optional[str] = None,
     ) -> tuple[str, str]:
         """
         Uploads assets based off of an asset manifest, uploads the asset manifest.
 
         Args:
             manifest: The asset manifest to upload.
             partial_manifest_prefix: The (partial) key prefix to use for uploading the manifest
@@ -156,23 +157,14 @@
             source_root: The local root path of the assets.
             job_attachment_settings: The settings for the job attachment configured in Queue.
             progress_tracker: Optional progress tracker to track progress.
 
         Returns:
             A tuple of (the partial key for the manifest on S3, the hash of input manifest).
         """
-        # Upload assets
-        self.upload_input_files(
-            manifest,
-            job_attachment_settings.s3BucketName,
-            source_root,
-            job_attachment_settings.full_cas_prefix(),
-            progress_tracker,
-            s3_check_cache_dir,
-        )
 
         # Upload asset manifest
         hash_alg = manifest.get_default_hash_alg()
         manifest_bytes = manifest.encode().encode("utf-8")
         manifest_name_prefix = hash_data(
             f"{file_system_location_name or ''}{str(source_root)}".encode(), hash_alg
         )
@@ -183,22 +175,61 @@
         else:
             partial_manifest_key = manifest_name
 
         full_manifest_key = job_attachment_settings.add_root_and_manifest_folder_prefix(
             partial_manifest_key
         )
 
+        if manifest_write_dir:
+            self._write_local_manifest(
+                manifest_write_dir, manifest_name, full_manifest_key, manifest
+            )
+
         self.upload_bytes_to_s3(
             bytes=BytesIO(manifest_bytes),
             bucket=job_attachment_settings.s3BucketName,
             key=full_manifest_key,
         )
 
+        # Upload assets
+        self.upload_input_files(
+            manifest,
+            job_attachment_settings.s3BucketName,
+            source_root,
+            job_attachment_settings.full_cas_prefix(),
+            progress_tracker,
+            s3_check_cache_dir,
+        )
+
         return (partial_manifest_key, hash_data(manifest_bytes, hash_alg))
 
+    def _write_local_manifest(
+        self,
+        manifest_write_dir: str,
+        manifest_name: str,
+        full_manifest_key: str,
+        manifest: BaseAssetManifest,
+    ) -> None:
+        """
+        Writes a manifest file locally in a 'manifests' sub-directory.
+        Also creates/appends to a file mapping the local manifest name to the full S3 key in the same directory.
+        """
+        local_manifest_file = Path(manifest_write_dir, "manifests", manifest_name)
+        logger.info(f"Creating local manifest file: {local_manifest_file}\n")
+        local_manifest_file.parent.mkdir(parents=True, exist_ok=True)
+        with open(local_manifest_file, "w") as file:
+            file.write(manifest.encode())
+
+        # Create or append to an existing mapping file. We use this since path lengths can go beyond the
+        # file name length limit on Windows if we were to create the full S3 key path locally.
+        manifest_map_file = Path(manifest_write_dir, "manifests", "manifest_s3_mapping")
+        mapping = {"local_file": manifest_name, "s3_key": full_manifest_key}
+        with open(manifest_map_file, "a") as mapping_file:
+            mapping_file.write(f"{mapping}\n")
+
     def upload_input_files(
         self,
         manifest: BaseAssetManifest,
         s3_bucket: str,
         source_root: Path,
         s3_cas_prefix: str,
         progress_tracker: Optional[ProgressTracker] = None,
@@ -1128,14 +1159,15 @@
         return (progress_tracker.get_summary_statistics(), asset_root_manifests)
 
     def upload_assets(
         self,
         manifests: list[AssetRootManifest],
         on_uploading_assets: Optional[Callable[[Any], bool]] = None,
         s3_check_cache_dir: Optional[str] = None,
+        manifest_write_dir: Optional[str] = None,
     ) -> tuple[SummaryStatistics, Attachments]:
         """
         Uploads all the files for provided manifests and manifests themselves to S3.
 
         Args:
             manifests: a list of manifests that contain assets to be uploaded
             on_uploading_assets: a callback to be called to periodically report progress to the caller.
@@ -1178,14 +1210,15 @@
                     partial_manifest_prefix=self.job_attachment_settings.partial_manifest_prefix(
                         self.farm_id, self.queue_id
                     ),
                     source_root=Path(asset_root_manifest.root_path),
                     file_system_location_name=asset_root_manifest.file_system_location_name,
                     progress_tracker=progress_tracker,
                     s3_check_cache_dir=s3_check_cache_dir,
+                    manifest_write_dir=manifest_write_dir,
                 )
                 manifest_properties.inputManifestPath = partial_manifest_key
                 manifest_properties.inputManifestHash = asset_manifest_hash
 
             manifest_properties_list.append(manifest_properties)
 
             logger.debug("Asset manifests - locations in S3:")
```

### Comparing `deadline-0.47.2/src/deadline/job_attachments/vfs.py` & `deadline-0.47.3/src/deadline/job_attachments/vfs.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/_aws/aws_clients.py` & `deadline-0.47.3/src/deadline/job_attachments/_aws/aws_clients.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/_aws/deadline.py` & `deadline-0.47.3/src/deadline/job_attachments/_aws/deadline.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/_windows/file.py` & `deadline-0.47.3/src/deadline/job_attachments/_windows/file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/__init__.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/_canonical_json.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/_canonical_json.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/base_manifest.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/base_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/decode.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/decode.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/hash_algorithms.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/manifest_model.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/manifest_model.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py` & `deadline-0.47.3/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/caches/cache_db.py` & `deadline-0.47.3/src/deadline/job_attachments/caches/cache_db.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/caches/hash_cache.py` & `deadline-0.47.3/src/deadline/job_attachments/caches/hash_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/src/deadline/job_attachments/caches/s3_check_cache.py` & `deadline-0.47.3/src/deadline/job_attachments/caches/s3_check_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/LICENSE` & `deadline-0.47.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/README.md` & `deadline-0.47.3/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/hatch.toml` & `deadline-0.47.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/pyproject.toml` & `deadline-0.47.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.2/PKG-INFO` & `deadline-0.47.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline
-Version: 0.47.2
+Version: 0.47.3
 Summary: Multi-purpose library and command line tool that implements functionality to support applications using AWS Deadline Cloud.
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

