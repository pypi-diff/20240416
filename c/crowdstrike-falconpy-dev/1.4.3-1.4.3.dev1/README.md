# Comparing `tmp/crowdstrike-falconpy-dev-1.4.3.tar.gz` & `tmp/crowdstrike-falconpy-dev-1.4.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdstrike-falconpy-dev-1.4.3.tar", last modified: Tue Apr 16 15:26:24 2024, max compression
+gzip compressed data, was "crowdstrike-falconpy-dev-1.4.3.dev1.tar", last modified: Fri Mar 22 16:48:25 2024, max compression
```

## Comparing `crowdstrike-falconpy-dev-1.4.3.tar` & `crowdstrike-falconpy-dev-1.4.3.dev1.tar`

### file list

```diff
@@ -1,334 +1,335 @@
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.863851 crowdstrike-falconpy-dev-1.4.3/
--rw-r--r--   0 jhiller    (501) staff       (20)     5042 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/AUTHORS.md
--rw-r--r--   0 jhiller    (501) staff       (20)     1211 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/LICENSE
--rw-r--r--   0 jhiller    (501) staff       (20)    22424 2024-04-16 15:26:24.863181 crowdstrike-falconpy-dev-1.4.3/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)    18806 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/README.md
--rw-r--r--   0 jhiller    (501) staff       (20)     7201 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/dev_setup.py
--rw-r--r--   0 jhiller    (501) staff       (20)       38 2024-04-16 15:26:24.863977 crowdstrike-falconpy-dev-1.4.3/setup.cfg
--rw-r--r--   0 jhiller    (501) staff       (20)     4441 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/setup.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.670254 crowdstrike-falconpy-dev-1.4.3/src/
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.861173 crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/
--rw-r--r--   0 jhiller    (501) staff       (20)    22424 2024-04-16 15:26:24.000000 crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)    12164 2024-04-16 15:26:24.000000 crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        1 2024-04-16 15:26:24.000000 crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/dependency_links.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       83 2024-04-16 15:26:24.000000 crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/requires.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       12 2024-04-16 15:26:24.000000 crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/top_level.txt
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.723949 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/
--rw-r--r--   0 jhiller    (501) staff       (20)    13510 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.728537 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/
--rw-r--r--   0 jhiller    (501) staff       (20)     2095 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11118 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5455 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_behavior.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2191 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_connection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3585 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2345 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_payloads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2112 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_validator.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.731712 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/
--rw-r--r--   0 jhiller    (501) staff       (20)     2047 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3926 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_base_falcon_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5890 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_bearer_token.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25370 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_falcon_interface.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4243 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_interface_config.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9922 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_uber_interface.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.732307 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_constant/
--rw-r--r--   0 jhiller    (501) staff       (20)     2992 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_constant/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.774853 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/
--rw-r--r--   0 jhiller    (501) staff       (20)    11139 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12076 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6740 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4669 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_cloud_snapshots.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4362 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_configuration_assessment.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2288 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_configuration_assessment_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3594 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7317 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_detections.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10475 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_images.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6442 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_packages.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11812 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38587 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13510 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7519 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_custom_storage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18026 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6461 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10667 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24288 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5926 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_drift_indicators.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3167 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15182 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7270 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15282 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4046 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)    33101 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23284 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10068 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10302 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_foundry_logscale.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9015 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10749 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3793 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5259 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_image_assessment_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8063 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6228 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27079 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4594 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15921 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13543 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    49145 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5796 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7157 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4457 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2377 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20908 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3602 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13571 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3569 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9960 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_prevention_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4808 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4165 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24958 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17733 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3335 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_real_time_response_audit.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18257 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4096 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9925 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11743 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3808 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8651 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15935 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sensor_update_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4678 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4669 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8488 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4885 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4250 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_unidentified_containers.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16740 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14871 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_workflows.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6063 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.783647 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/
--rw-r--r--   0 jhiller    (501) staff       (20)     4788 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13253 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5506 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24312 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4070 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23308 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3510 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2290 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6252 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15695 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2201 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3044 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_mapping.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13826 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13735 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15033 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4120 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3832 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1945 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.785374 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/
--rw-r--r--   0 jhiller    (501) staff       (20)     1871 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2124 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2063 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/_container_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2218 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/_token_fail_reason.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.786598 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/
--rw-r--r--   0 jhiller    (501) staff       (20)     2869 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6071 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/_exceptions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5936 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/_warnings.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.787671 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_log/
--rw-r--r--   0 jhiller    (501) staff       (20)     1744 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_log/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3563 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_log/_facility.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.803463 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/
--rw-r--r--   0 jhiller    (501) staff       (20)     6763 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2691 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3624 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3735 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_cloud_snapshots.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8983 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7709 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4974 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2790 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6181 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_device_control_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3666 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_falconx.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6540 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15938 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_firewall.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3701 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_foundry.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7429 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_generic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4290 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4625 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5808 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7508 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5577 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3774 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2866 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4506 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3118 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4309 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8001 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2615 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_response_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2433 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4519 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6410 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_workflows.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.808123 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/
--rw-r--r--   0 jhiller    (501) staff       (20)     4301 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/__base_resource.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2186 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4464 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_base_dictionary.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1825 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_errors.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2684 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_expanded_result.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3302 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_headers.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3476 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2489 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_resources.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4320 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_response_component.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17269 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_result.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.809470 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/
--rw-r--r--   0 jhiller    (501) staff       (20)     1827 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11888 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/_base_service_class.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15099 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/_service_class.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.812147 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/
--rw-r--r--   0 jhiller    (501) staff       (20)     3325 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4842 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38784 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_functions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2839 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_service.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7243 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_uber.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3534 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_version.py
--rw-r--r--   0 jhiller    (501) staff       (20)    29278 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/alerts.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.813990 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/
--rw-r--r--   0 jhiller    (501) staff       (20)     2297 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10307 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/_advanced.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22357 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/_legacy.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15947 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11442 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/cloud_snapshots.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6121 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/configuration_assessment.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4007 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/configuration_assessment_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6517 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13752 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_detections.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17955 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_images.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10060 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_packages.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20248 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)    71956 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34208 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15743 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/custom_storage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35915 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10057 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/debug.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15758 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    29552 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    26025 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10441 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/drift_indicators.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5973 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    56069 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18125 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    28300 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8668 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)    55691 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    79369 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20297 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18682 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/foundry_logscale.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18869 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    29375 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10700 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16858 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/image_assessment_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13868 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13625 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    39639 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10663 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    40962 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14032 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    95881 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16367 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23565 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10056 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5166 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    45042 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9353 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    36525 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13881 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20718 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14372 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9493 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43159 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27814 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4685 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/real_time_response_audit.py
--rw-r--r--   0 jhiller    (501) staff       (20)    45859 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7687 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19891 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22121 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6764 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16863 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38364 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9899 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8333 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10652 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9791 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7700 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/unidentified_containers.py
--rw-r--r--   0 jhiller    (501) staff       (20)    39354 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    30725 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/workflows.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8311 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/src/falconpydev/zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-04-16 15:26:24.860524 crowdstrike-falconpy-dev-1.4.3/tests/
--rw-r--r--   0 jhiller    (501) staff       (20)     3747 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6020 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_api_request.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13934 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_authentications.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11321 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_authorization.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9513 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2250 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_cloud_snapshots.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1187 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_configuration_assessment.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1031 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_configuration_assessment_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1189 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_container_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1641 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_container_detections.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1980 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_container_images.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1512 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_container_packages.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2333 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_container_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8916 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4540 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2608 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_custom_storage.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6223 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5675 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8245 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3156 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1523 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_drift_indicators.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4468 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4500 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4105 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3949 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1200 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4805 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19281 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4175 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2198 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_foundry_logscale.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5816 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12282 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3089 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2400 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_image_assessment_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4104 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4309 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3655 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3483 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5129 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2171 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6609 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4394 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5649 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2494 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1071 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3486 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8135 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2075 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6603 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2021 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3137 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6962 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6933 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1229 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_real_time_response_audit.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6646 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1580 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4476 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23298 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_result_object.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6794 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1449 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5691 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9177 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2369 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14230 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_service_class.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2962 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3904 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1826 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4701 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_timeout.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14727 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_uber.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14776 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_uber_api_complete.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1274 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_unidentified_containers.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8529 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2873 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_workflows.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3383 2024-04-16 15:26:23.000000 crowdstrike-falconpy-dev-1.4.3/tests/test_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.193488 crowdstrike-falconpy-dev-1.4.3.dev1/
+-rw-r--r--   0 jhiller    (501) staff       (20)     5042 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/AUTHORS.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     1211 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/LICENSE
+-rw-r--r--   0 jhiller    (501) staff       (20)    22055 2024-03-22 16:48:25.192945 crowdstrike-falconpy-dev-1.4.3.dev1/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)    18806 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/README.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     7151 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/dev_setup.py
+-rw-r--r--   0 jhiller    (501) staff       (20)       38 2024-03-22 16:48:25.193621 crowdstrike-falconpy-dev-1.4.3.dev1/setup.cfg
+-rw-r--r--   0 jhiller    (501) staff       (20)     4441 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/setup.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:24.884852 crowdstrike-falconpy-dev-1.4.3.dev1/src/
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:24.893914 crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/
+-rw-r--r--   0 jhiller    (501) staff       (20)    22055 2024-03-22 16:48:24.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)    12198 2024-03-22 16:48:24.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        1 2024-03-22 16:48:24.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       83 2024-03-22 16:48:24.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/requires.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       12 2024-03-22 16:48:24.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/top_level.txt
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:24.960665 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/
+-rw-r--r--   0 jhiller    (501) staff       (20)    13510 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:24.967808 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2095 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11118 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5455 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_behavior.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2191 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_connection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3585 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2345 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_payloads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2112 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_validator.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:24.973386 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2047 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3926 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_base_falcon_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5890 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_bearer_token.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22680 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_falcon_interface.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4243 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_interface_config.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9922 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_uber_interface.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:24.974256 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_constant/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2992 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_constant/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.033185 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/
+-rw-r--r--   0 jhiller    (501) staff       (20)    11139 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12076 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6740 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4669 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_cloud_snapshots.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4362 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_configuration_assessment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2288 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_configuration_assessment_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3594 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7317 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_detections.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10486 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_images.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6442 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_packages.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11812 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38268 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13510 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7519 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_custom_storage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17727 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6461 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10667 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24288 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5926 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_drift_indicators.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3167 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15182 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7270 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15282 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4046 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    33045 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23284 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10068 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10302 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_foundry_logscale.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9015 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10749 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3793 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5259 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_image_assessment_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8063 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6228 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27079 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4594 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15921 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13543 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    49085 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5796 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7141 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4457 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2377 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20908 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3602 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13571 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3569 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9960 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_prevention_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4808 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4165 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24958 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17733 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3335 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_real_time_response_audit.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18257 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4096 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9925 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11743 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3808 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8651 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15935 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sensor_update_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4678 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4669 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8488 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4885 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4250 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_unidentified_containers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16740 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14871 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_workflows.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6063 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.045715 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4788 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13253 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5506 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24312 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4070 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23308 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3510 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2290 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6252 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15695 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2201 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3044 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_mapping.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13826 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13735 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15033 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4120 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3832 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1945 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.048907 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1871 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2124 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2063 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/_container_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2218 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/_token_fail_reason.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.051226 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2869 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6071 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/_exceptions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5936 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/_warnings.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.052731 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_log/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1744 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_log/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3563 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_log/_facility.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.100181 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/
+-rw-r--r--   0 jhiller    (501) staff       (20)     6763 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2691 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3624 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3735 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_cloud_snapshots.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8983 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7709 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4974 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2790 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6181 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_device_control_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3666 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_falconx.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6252 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15938 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_firewall.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3701 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_foundry.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7429 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_generic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4290 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4625 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5808 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7508 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5577 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3774 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2866 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4506 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3118 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4309 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8001 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2615 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_response_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2433 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4519 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6410 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_workflows.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.114683 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4301 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/__base_resource.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2186 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4464 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_base_dictionary.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1825 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_errors.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2684 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_expanded_result.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3302 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_headers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3476 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2489 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_resources.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4320 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_response_component.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17269 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_result.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.117569 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1827 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11888 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/_base_service_class.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14366 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/_service_class.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.125140 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/
+-rw-r--r--   0 jhiller    (501) staff       (20)     3265 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3076 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38470 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_functions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2839 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_service.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7243 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_uber.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3539 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_version.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29278 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/alerts.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.130086 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2297 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10307 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/_advanced.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22357 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/_legacy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15947 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11442 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/cloud_snapshots.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6121 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/configuration_assessment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4007 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/configuration_assessment_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6517 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13752 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_detections.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17955 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_images.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10060 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_packages.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20248 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    69217 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34208 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15743 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/custom_storage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    33273 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10057 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/debug.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15758 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29552 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    26025 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10441 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/drift_indicators.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5973 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    56069 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18125 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    28300 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8668 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    53063 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    79369 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20297 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18682 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/foundry_logscale.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18869 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29375 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10700 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16858 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/image_assessment_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13868 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13625 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    39639 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10663 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    40962 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14032 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    95749 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16367 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23565 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10056 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5166 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    45042 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9353 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    36525 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13881 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20718 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14372 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9493 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43159 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27814 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4685 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/real_time_response_audit.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    45859 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7687 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    19891 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22121 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6764 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16863 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38364 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9899 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8333 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10652 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9791 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7700 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/unidentified_containers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    39354 2024-03-22 16:46:39.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    30306 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/workflows.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8311 2024-03-22 16:46:38.000000 crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2024-03-22 16:48:25.192007 crowdstrike-falconpy-dev-1.4.3.dev1/tests/
+-rw-r--r--   0 jhiller    (501) staff       (20)     3747 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6020 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_api_request.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14980 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_authentications.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11321 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_authorization.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9513 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2250 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_cloud_snapshots.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1187 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_configuration_assessment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1031 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_configuration_assessment_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1189 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1640 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_detections.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1980 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_images.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1507 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_packages.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2328 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8812 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4540 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2608 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_custom_storage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6119 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5675 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8245 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3156 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1518 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_drift_indicators.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4468 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1481 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_exposure_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4500 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4105 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3949 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1200 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4805 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    19281 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4175 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2198 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_foundry_logscale.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5816 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12282 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3089 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2400 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_image_assessment_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4104 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4309 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3655 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3483 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5129 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2171 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6609 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4394 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5649 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2494 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1071 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3486 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8135 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2075 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6603 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2021 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3137 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6962 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6933 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1229 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_real_time_response_audit.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6646 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1580 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4476 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23459 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_result_object.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6794 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1449 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5691 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9177 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2369 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14230 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_service_class.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2962 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3904 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1826 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4701 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_timeout.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14653 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_uber.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14776 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_uber_api_complete.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1269 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_unidentified_containers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8529 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2642 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_workflows.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1907 2024-03-22 16:46:35.000000 crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_zero_trust_assessment.py
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/AUTHORS.md` & `crowdstrike-falconpy-dev-1.4.3.dev1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/LICENSE` & `crowdstrike-falconpy-dev-1.4.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/PKG-INFO` & `crowdstrike-falconpy-dev-1.4.3.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy-dev
-Version: 1.4.3
+Version: 1.4.3.dev1
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
@@ -23,35 +23,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: requests
-Requires-Dist: urllib3
-Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: pydocstyle; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: bandit; extra == "dev"
 
 ![CrowdStrike FalconPy](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png)
 
 [![CrowdStrike Subreddit](https://img.shields.io/badge/-r%2Fcrowdstrike-white?logo=reddit&labelColor=gray&link=https%3A%2F%2Freddit.com%2Fr%2Fcrowdstrike)](https://reddit.com/r/crowdstrike)<br/>
 
 # FalconPy - The CrowdStrike Falcon SDK for Python
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/README.md` & `crowdstrike-falconpy-dev-1.4.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/dev_setup.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/dev_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Framework :: Flake8",
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Topic :: Security",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: System :: Systems Administration",
         "Topic :: Utilities"
     ],
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/setup.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy-dev
-Version: 1.4.3
+Version: 1.4.3.dev1
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
@@ -23,35 +23,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: requests
-Requires-Dist: urllib3
-Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: pydocstyle; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: bandit; extra == "dev"
 
 ![CrowdStrike FalconPy](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png)
 
 [![CrowdStrike Subreddit](https://img.shields.io/badge/-r%2Fcrowdstrike-white?logo=reddit&labelColor=gray&link=https%3A%2F%2Freddit.com%2Fr%2Fcrowdstrike)](https://reddit.com/r/crowdstrike)<br/>
 
 # FalconPy - The CrowdStrike Falcon SDK for Python
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -256,14 +256,15 @@
 tests/test_custom_storage.py
 tests/test_d4c_registration.py
 tests/test_detects.py
 tests/test_device_control_policies.py
 tests/test_discover.py
 tests/test_drift_indicators.py
 tests/test_event_streams.py
+tests/test_exposure_management.py
 tests/test_falcon_complete_dashboard.py
 tests/test_falcon_container.py
 tests/test_falconx_sandbox.py
 tests/test_fdr.py
 tests/test_filevantage.py
 tests/test_firewall_management.py
 tests/test_firewall_policies.py
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_behavior.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_behavior.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_connection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_connection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_meta.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_payloads.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_payloads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_api_request/_request_validator.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_api_request/_request_validator.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_base_falcon_auth.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_base_falcon_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_bearer_token.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_bearer_token.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_falcon_interface.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_falcon_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,41 +38,44 @@
 
 For more information, please refer to <https://unlicense.org>
 """
 import time
 import os
 import warnings
 from contextvars import copy_context
+from json import loads
+try:
+    from simplejson import JSONDecodeError
+except (ImportError, ModuleNotFoundError):  # Support import as a module
+    from json.decoder import JSONDecodeError
 from logging import Logger, getLogger
 from typing import Dict, Optional, Union
 from ._base_falcon_auth import BaseFalconAuth
 from ._bearer_token import BearerToken
 from .._log import LogFacility
 from .._constant import MIN_TOKEN_RENEW_WINDOW, MAX_TOKEN_RENEW_WINDOW
 from ._interface_config import InterfaceConfiguration
 from .._enum import TokenFailReason
 from .._util import (
     autodiscover_region,
-    confirm_base_url,
     perform_request,
     log_class_startup,
     login_payloads,
-    logout_payloads,
-    review_provided_credentials
+    logout_payloads
     )
-from .._error import InvalidCredentials, NoAuthenticationMechanism
+from .._error import InvalidCredentials, NoAuthenticationMechanism, InvalidCredentialFormat
 
 
-# pylint: disable=R0902,R0904
+# pylint: disable=R0902
 class FalconInterface(BaseFalconAuth):
     """Standard Falcon API interface used by Service Classes."""
 
-    # _______  _____  __   _ _______ _______  ______ _     _ _______ _______  _____   ______
-    # |       |     | | \  | |______    |    |_____/ |     | |          |    |     | |_____/
-    # |_____  |_____| |  \_| ______|    |    |    \_ |_____| |_____     |    |_____| |    \_
+    # ____ ____ _  _ ____ ___ ____ _  _ ____ ___ ____ ____
+    # |    |  | |\ | [__   |  |__/ |  | |     |  |  | |__/
+    # |___ |__| | \| ___]  |  |  \ |__| |___  |  |__| |  \
     #
     # The default constructor for all authentication objects. Ingests provided credentials
     # and sets the necessary class attributes based upon the authentication detail received.
     # pylint: disable=R0912,R0913,R0914
     def __init__(self,
                  access_token: Optional[Union[str, bool]] = False,
                  base_url: Optional[str] = "https://api.crowdstrike.com",
@@ -93,98 +96,77 @@
                  ) -> "FalconInterface":
         """Construct an instance of the FalconInterface class."""
         # Set the pythonic behavior mode.
         self._pythonic: bool = False
         if isinstance(pythonic, bool):
             self._pythonic = pythonic
 
+        # The default credential dictionary, where the client_id and client_secret are stored.
+        self._creds = {}
+
+        # Set up an empty Bearer Token container
+        self._token: BearerToken = BearerToken()
+
         # Setup our configuration object using the provided keywords.
         self._config: InterfaceConfiguration = InterfaceConfiguration(base_url=base_url,
                                                                       proxy=proxy,
                                                                       timeout=timeout,
                                                                       user_agent=user_agent,
                                                                       ssl_verify=ssl_verify
                                                                       )            # \ o /
         # ____ _  _ ___ _  _ ____ _  _ ___ _ ____ ____ ___ _ ____ _  _                 |
         # |__| |  |  |  |__| |___ |\ |  |  | |    |__|  |  | |  | |\ |                / \
         # |  | |__|  |  |  | |___ | \|  |  | |___ |  |  |  | |__| | \|
-        #
-        # Assume no credentials or tokens are provided.
-        # A NoAuthenticationMechanism warning will be generated if a
-        # valid authentication mechanism is not specified or detected.
-        #
-        # Then try to authenticate in the following order:
-        #    1. Direct
-        #    2. Credential
-        #    3. Token (Legacy)
-        #    4. Context (Foundry)
-        #    5. Environment
-        #
-        # Remaining authentication checks are skipped once a successful mechanism has been determined.
-        #
-        # Object Authentication is handled within the ServiceClass object and leverages the existing
-        # authentication used for the underlying authentication object attribute.
+        # Direct Authentication
+        if client_id and client_secret and not creds:
+            creds = {
+                "client_id": client_id,
+                "client_secret": client_secret
+            }
+            # You must pass member_cid the same way you pass client_id / secret.
+            # If you use a creds dictionary, pass the member_cid there instead.
+            if member_cid:
+                creds["member_cid"] = member_cid
+        elif not creds:
+            creds = {}
+        # Credential Authentication (also powers Direct Authentication).
+        if isinstance(creds, str):
+            try:
+                # Try and clean up any attempts to provide the dictionary as a string
+                self._creds: Dict[str, str] = loads(creds.replace("'", "\""))
+            except (TypeError, JSONDecodeError) as bad_cred_format:
+                raise InvalidCredentialFormat from bad_cred_format
+        elif isinstance(creds, dict):
+            self._creds: Dict[str, str] = creds
+        else:
+            raise InvalidCredentialFormat
 
-        # Set up an empty Bearer Token container.
-        self._token: BearerToken = BearerToken()
+        # Legacy (Token) Authentication (fallback)
+        if access_token:
+            # Store this non-refreshable token, assuming it was just generated.
+            self._token: BearerToken = BearerToken(access_token, 1799, 201)
+
+        # Foundry authentication
+        ctx = copy_context()
+        for cvar in ctx.values():
+            try:
+                self._token: BearerToken = BearerToken(cvar.access_token, 1799, 201)
+                break
+            except AttributeError:
+                pass
 
-        # ___  _ ____ ____ ____ ___    ____ _  _ ___     ____ ____ ____ ___  ____ _  _ ___ _ ____ _
-        # |  \ | |__/ |___ |     |     |__| |\ | |  \    |    |__/ |___ |  \ |___ |\ |  |  | |__| |
-        # |__/ | |  \ |___ |___  |     |  | | \| |__/    |___ |  \ |___ |__/ |___ | \|  |  | |  | |___
-        #
-        # Direct Authentication checks provided values and return a creds dictionary based upon the contents.
-        # Authorization is derived from the bearer token generated using the provided credentials.
-        self._creds, self._auth_style = review_provided_credentials(client_id, client_secret, creds, member_cid)
-
-        # ___ ____ _  _ ____ _  _
-        #  |  |  | |_/  |___ |\ |
-        #  |  |__| | \_ |___ | \|
-        #
-        # Token (Legacy) Authentication
-        # Authorization is derived from the provided bearer token.
-        # A login event is unnecessary when using this authentication mechanism.
-        if not self.cred_format_valid:
-            if access_token:
-                # Store this non-refreshable token, assuming it was just generated.
-                self._token: BearerToken = BearerToken(access_token, 1799, 201)
-                self._auth_style = "TOKEN"
-
-        # ____ ____ _  _ ___ ____ _  _ ___
-        # |    |  | |\ |  |  |___  \/   |
-        # |___ |__| | \|  |  |___ _/\_  |
-        #
-        # Context Authentication searches the current running context for
-        # an object containing a bearer token as an attribute or property.
-        # Authorization is derived from the discovered bearer token.
-        # A login event is unnecessary when using this authentication mechanism.
-        if not self.cred_format_valid and not self.token_value:
-            for cvar in copy_context().values():
-                try:
-                    # Any object is acceptable as long as it has an attribute or property named "access_token".
-                    self._token: BearerToken = BearerToken(cvar.access_token, 1799, 201)
-                    # Attempt to retrieve the cloud region from the same object.
-                    # Fall back to our previously set default on failure.
-                    try:
-                        if cvar.cs_cloud:
-                            self._config.base_url = confirm_base_url(cvar.cs_cloud)
-                    except AttributeError:
-                        pass
-                    self._auth_style = "CONTEXT"
-                    break
-                except AttributeError:
-                    pass
-
-        # ____ _  _ _  _ _ ____ ____ _  _ _  _ ____ _  _ ___
-        # |___ |\ | |  | | |__/ |  | |\ | |\/| |___ |\ |  |
-        # |___ | \|  \/  | |  \ |__| | \| |  | |___ | \|  |
-        #
-        # Environment Authentication searches the current environment for variables containing credentials.
-        # Authorization is derived from the bearer token generated using the discovered credentials.
-        # Developers may customize which variable names are searched by leveraging the environment keyword (dictionary).
+        # Set the token renewal window, ignored when using Legacy Authentication.
+        self.renew_window: int = max(min(renew_window, MAX_TOKEN_RENEW_WINDOW),
+                                     MIN_TOKEN_RENEW_WINDOW
+                                     )
+
+        # Environment Authentication
+        # User configuration environment keys
         self._environment = environment if environment else {}
+        # When credentials are not provided, attempt to retrieve them from the environment.
         if not self.cred_format_valid and not self.token_value:
             # Both variables must be present within the running environment.
             if os.getenv(f"{self.env_prefix}{self.env_key}") and os.getenv(f"{self.env_prefix}{self.env_secret}"):
                 api_id = os.getenv(f"{self.env_prefix}{self.env_key}") \
                     if "client_id" not in self.creds else self.creds["client_id"]
                 api_sec = os.getenv(f"{self.env_prefix}{self.env_secret}") \
                     if "client_secret" not in self.creds else self.creds["client_secret"]
@@ -192,25 +174,15 @@
                 self._creds = {
                     "client_id": api_id,
                     "client_secret": api_sec
                 }
                 # Provide member_cid for MSSP environment authentication scenarios. Issue #1105.
                 if member_cid:
                     self._creds["member_cid"] = member_cid
-                self._auth_style = "ENVIRONMENT"
-
-        # Set the token renewal window, ignored when using Legacy or Context Authentication.
-        self.renew_window: int = max(min(renew_window, MAX_TOKEN_RENEW_WINDOW),
-                                     MIN_TOKEN_RENEW_WINDOW
-                                     )
 
-        # _    ____ ____ ____ _ _  _ ____
-        # |    |  | | __ | __ | |\ | | __
-        # |___ |__| |__] |__] | | \| |__]
-        #
         # Log the creation of this object if debugging is enabled.
         # Starting with v1.3.0 minimal Python native logging is available. In order to reduce
         # potential impacts to developer configurations, this facility is extremely limited
         # and not implemented by default. (Meaning logs are not generated.)
         # To enable logging, pass the keyword "debug" with a value of True to the constructor.
         if debug:
             # Ignored when debugging is disabled.
@@ -224,33 +196,26 @@
                                                  )
             # Log the startup of this class.
             log_class_startup(self, self.log)
         else:
             # Set up an empty log facility
             self._log: LogFacility = LogFacility()
 
-        # _  _ ____ _    _ ___  ____ ___ ____
-        # |  | |__| |    | |  \ |__|  |  |___
-        #  \/  |  | |___ | |__/ |  |  |  |___
-        #
-        # Validation occurs after the logging object is created.
         try:
-            # Check to see if we have a valid authentication mechanism configured.
             if not self.cred_format_valid and not self.token_value:
                 raise NoAuthenticationMechanism
         except NoAuthenticationMechanism as no_auth_mechanism:
-            # Warn appropriately if we do not.
             if pythonic:
                 warnings.warn(no_auth_mechanism.message, NoAuthenticationMechanism, stacklevel=2)
             if self.log:
                 self.log.warning(no_auth_mechanism.message)
 
-    #  _______ _______ _______ _     _  _____  ______  _______
-    #  |  |  | |______    |    |_____| |     | |     \ |______
-    #  |  |  | |______    |    |     | |_____| |_____/ ______|
+    # _  _ ____ ___ _  _ ____ ___  ____
+    # |\/| |___  |  |__| |  | |  \ [__
+    # |  | |___  |  |  | |__| |__/ ___]
     #
     # The generic login and logout handlers are provided here and leverage private methods
     # to perform the operation. These private methods can be overridden to provide individual
     # login and logout functionality to different inheriting class types.
     def login(self) -> Union[dict, bool]:
         """Login to the Falcon API by requesting a new token."""
         return self._login_handler()
@@ -342,17 +307,17 @@
         except InvalidCredentials as bad_creds:
             returned = bad_creds.result
             if self.log:
                 self.log.error(bad_creds.message)
 
         return returned
 
-    #  _____   ______  _____   _____  _______  ______ _______ _____ _______ _______
-    # |_____] |_____/ |     | |_____] |______ |_____/    |      |   |______ |______
-    # |       |    \_ |_____| |       |______ |    \_    |    __|__ |______ ______|
+    # ___  ____ ____ ___  ____ ____ ___ _ ____ ____
+    # |__] |__/ |  | |__] |___ |__/  |  | |___ [__
+    # |    |  \ |__| |    |___ |  \  |  | |___ ___]
     #
     # These properties are present in all FalconInterface derivatives.
     @property
     def creds(self) -> Dict[str, str]:
         """Return the current credential dictionary."""
         return self._creds
 
@@ -370,55 +335,55 @@
         if not isinstance(value, InterfaceConfiguration):
             raise ValueError
         self._config = value
 
     @property
     def base_url(self) -> str:
         """Return the base URL for this interface from the configuration object."""
-        return self.config.base_url
+        return self._config.base_url
 
     @base_url.setter
     def base_url(self, value):
-        self.config.base_url = value
+        self._config.base_url = value
 
     @property
     def ssl_verify(self) -> bool:
         """Return the SSL verification setting from the configuration object."""
-        return self.config.ssl_verify
+        return self._config.ssl_verify
 
     @ssl_verify.setter
     def ssl_verify(self, value: bool):
-        self.config.ssl_verify = value
+        self._config.ssl_verify = value
 
     @property
     def proxy(self) -> Dict[str, str]:
         """Return the current proxy setting."""
-        return self.config.proxy
+        return self._config.proxy
 
     @proxy.setter
     def proxy(self, value: Dict[str, str]):
-        self.config.proxy = value
+        self._config.proxy = value
 
     @property
     def user_agent(self) -> str:
         """Return the current user agent setting."""
-        return self.config.user_agent
+        return self._config.user_agent
 
     @user_agent.setter
     def user_agent(self, value: str):
-        self.config.user_agent = value
+        self._config.user_agent = value
 
     @property
     def timeout(self) -> Union[int, tuple]:
         """Return the current timeout setting."""
-        return self.config.timeout
+        return self._config.timeout
 
     @timeout.setter
     def timeout(self, value: Union[int, tuple]):
-        self.config.timeout = value
+        self._config.timeout = value
 
     @property
     def debug_record_count(self) -> int:
         """Return the current debug record count setting."""
         return self.log_facility.debug_record_count
 
     @debug_record_count.setter
@@ -495,24 +460,14 @@
         """Return the current value setting."""
         return self.bearer_token.value
 
     @token_value.setter
     def token_value(self, value: str):
         self.bearer_token.value = value
 
-    @property
-    def pythonic(self) -> bool:
-        """Return a boolean if we are in a pythonic mode."""
-        return self._pythonic
-
-    @pythonic.setter
-    def pythonic(self, value: bool):
-        """Enable or disable pythonic mode."""
-        self._pythonic = value
-
     # All properties defined here are by design IMMUTABLE.
     @property
     def refreshable(self) -> bool:
         """Return a boolean if this interface can automatically refresh tokens when they expire."""
         return self.cred_format_valid
 
     @property
@@ -556,25 +511,30 @@
 
     @property
     def debug(self) -> bool:
         """Return a boolean if we are in a debug mode."""
         return bool(self.log)
 
     @property
+    def pythonic(self) -> bool:
+        """Return a boolean if we are in a pythonic mode."""
+        return self._pythonic
+
+    @pythonic.setter
+    def pythonic(self, value: bool):
+        """Enable or disable pythonic mode."""
+        self._pythonic = value
+
+    @property
     def env_prefix(self) -> str:
         """Return the environment prefix."""
         return self._environment.get("prefix", "FALCON_")
 
     @property
     def env_key(self) -> str:
         """Return the environment API key name."""
         return self._environment.get("id_name", "CLIENT_ID")
 
     @property
     def env_secret(self) -> str:
         """Return the environment API key secret."""
         return self._environment.get("secret_name", "CLIENT_SECRET")
-
-    @property
-    def auth_style(self) -> str:
-        """Return the authentication mechanism used to instantiate this object."""
-        return self._auth_style
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_interface_config.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_interface_config.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_auth_object/_uber_interface.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_auth_object/_uber_interface.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_constant/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_constant/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_cloud_snapshots.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_cloud_snapshots.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_configuration_assessment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_configuration_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_configuration_assessment_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_configuration_assessment_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_detections.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_detections.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_images.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,18 +245,18 @@
         "type": "integer",
         "description": "The offset from where to begin.",
         "name": "offset",
         "in": "query"
       },
       {
         "type": "string",
-        "description": "The fields to sort the records on. Supported columns:  [base_os cid detections "
-        "firstScanned first_seen highest_cps_current_rating highest_detection_severity highest_vulnerability_severity "
-        "image_digest image_id last_seen layers_with_vulnerabilities packages registry repository tag "
-        "vulnerabilities]",
+        "description": "The fields to sort the records on. Supported columns:  [base_os cid containers "
+        "detections firstScanned first_seen highest_cps_current_rating highest_detection_severity "
+        "highest_vulnerability_severity image_digest image_id last_seen layers_with_vulnerabilities packages registry "
+        "repository tag vulnerabilities]",
         "name": "sort",
         "in": "query"
       }
     ]
   ],
   [
     "CombinedImageIssuesSummary",
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_packages.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_packages.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_container_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_container_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_cspm_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_cspm_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -764,28 +764,14 @@
         "description": "Service Account ID",
         "name": "id",
         "in": "query"
       }
     ]
   ],
   [
-    "UpdateCSPMGCPServiceAccountsExt",
-    "PATCH",
-    "/cloud-connect-cspm-gcp/entities/service-accounts/v1",
-    "Patches the service account key for external clients.",
-    "cspm_registration",
-    [
-      {
-        "name": "body",
-        "in": "body",
-        "required": True
-      }
-    ]
-  ],
-  [
     "ValidateCSPMGCPServiceAccountExt",
     "POST",
     "/cloud-connect-cspm-gcp/entities/service-accounts/validate/v1",
     "Validates credentials for a service account",
     "cspm_registration",
     [
       {
@@ -1171,18 +1157,18 @@
     "GET",
     "/detects/queries/iom/v2",
     "Get list of active misconfiguration ids - including custom policy detections in addition to default policy detections.",
     "cspm_registration",
     [
       {
         "type": "string",
-        "description": "use_current_scan_ids - *use this to get records for latest scans (ignored when "
-        "next_token is set)*\naccount_name\naccount_id\nagent_id\nattack_types\nazure_subscription_id\ncloud_provider\n "
-        "cloud_service_keyword\ncustom_policy_id\nis_managed\npolicy_id\npolicy_type\nresource_id\nregion\nstatus\nscan "
-        "_time\nseverity\nseverity_string\n",
+        "description": "Available filters: use_current_scan_ids - *use this to get records for latest scans*\n "
+        "account_name\naccount_id\nagent_id\nattack_types\nazure_subscription_id\ncloud_provider\ncloud_service_keyword "
+        "\ncustom_policy_id\nis_managed\npolicy_id\npolicy_type\nresource_id\nregion\nstatus\nscan_time\nseverity\nseve "
+        "rity_string\n",
         "name": "filter",
         "in": "query"
       },
       {
         "type": "string",
         "default": "timestamp|desc",
         "description": "account_name\naccount_id\nattack_types\nazure_subscription_id\ncloud_provider\ncloud_s "
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_custom_ioa.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_custom_storage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_custom_storage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_d4c_registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,28 +538,14 @@
         "description": "Service Account ID",
         "name": "id",
         "in": "query"
       }
     ]
   ],
   [
-    "UpdateD4CGCPServiceAccountsExt",
-    "PATCH",
-    "/cloud-connect-gcp/entities/service-accounts/v1",
-    "Patches the service account key for external clients.",
-    "d4c_registration",
-    [
-      {
-        "name": "body",
-        "in": "body",
-        "required": True
-      }
-    ]
-  ],
-  [
     "GetD4CGCPUserScriptsAttachment",
     "GET",
     "/cloud-connect-gcp/entities/user-scripts-download/v1",
     "Return a script for customer to run in their cloud environment to grant us access to their GCP "
     "environment as a downloadable attachment",
     "d4c_registration",
     [
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_detects.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_device_control_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_discover.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_drift_indicators.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_drift_indicators.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_event_streams.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_falcon_container.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_fdr.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_filevantage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_filevantage.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,18 +441,18 @@
         " performed by specific users that will be monitored.\n\n * `exclude_users` represents the changes performed by "
         " specific users that will `NOT` be monitored.\n\n * `include_processes` represents the changes performed by "
         "specific processes that will be monitored.\n\n * `exclude_processes` represents the changes performed by "
         "specific processes that will be `NOT` monitored.\n\n * `content_files` represents the files whose content will "
         " be monitored. Listed files must match the file include pattern and not match the file exclude pattern\n\n * "
         "`content_registry_values` represents the registry values whose content will be monitored. Listed registry "
         "values must match the registry include pattern and not match the registry exclude pattern\n\n * "
-        "`enable_content_capture`\n\n * `enable_hash_capture`\n\nFile system directory monitoring:\n\n * "
-        "`watch_delete_directory_changes`\n\n * `watch_create_directory_changes`\n\n * "
-        "`watch_rename_directory_changes`\n\n * `watch_attributes_directory_changes` (`macOS` is not supported at this "
-        "time)\n\n * `watch_permissions_directory_changes` (`macOS` is not supported at this time)\n\nFile system file "
+        "`enable_content_capture`\n\nFile system directory monitoring:\n\n * `watch_delete_directory_changes`\n\n * "
+        "`watch_create_directory_changes`\n\n * `watch_rename_directory_changes`\n\n * "
+        "`watch_attributes_directory_changes` (`macOS` is not supported at this time)\n\n * "
+        "`watch_permissions_directory_changes` (`macOS` is not supported at this time)\n\nFile system file "
         "monitoring:\n\n * `watch_rename_file_changes`\n\n * `watch_write_file_changes`\n\n * "
         "`watch_create_file_changes`\n\n * `watch_delete_file_changes`\n\n * `watch_attributes_file_changes` (`macOS` "
         "is not supported at this time)\n\n * `watch_permissions_file_changes` (`macOS` is not supported at this "
         "time)\n\nWindows registry key and value monitoring: \n\n * `watch_create_key_changes`\n\n * "
         "`watch_delete_key_changes`\n\n * `watch_rename_key_changes`\n\n * `watch_set_value_changes`\n\n * "
         "`watch_permissions_key_changes`\n\n * `watch_delete_value_changes`\n\n * `watch_create_file_changes`",
         "name": "body",
@@ -484,18 +484,18 @@
         " represents the changes performed by specific users that will be monitored.\n\n * `exclude_users` represents "
         "the changes performed by specific users that will `NOT` be monitored.\n\n * `include_processes` represents the "
         " changes performed by specific processes that will be monitored.\n\n * `exclude_processes` represents the "
         "changes performed by specific processes that will be `NOT` monitored.\n\n * `content_files` represents the "
         "files that will be monitored. Listed files must match the file include pattern and not match the file exclude "
         "pattern\n\n * `content_registry_values` represents the registry values whose content will be monitored. Listed "
         " registry values must match the registry include pattern and not match the registry exclude pattern\n\n * "
-        "`enable_content_capture`\n\n * `enable_hash_capture`\n\nFile system directory monitoring:\n\n * "
-        "`watch_delete_directory_changes`\n\n * `watch_create_directory_changes`\n\n * "
-        "`watch_rename_directory_changes`\n\n * `watch_attributes_directory_changes` (`macOS` is not supported at this "
-        "time)\n\n * `watch_permissions_directory_changes` (`macOS` is not supported at this time)\n\nFile system file "
+        "`enable_content_capture`\n\nFile system directory monitoring:\n\n * `watch_delete_directory_changes`\n\n * "
+        "`watch_create_directory_changes`\n\n * `watch_rename_directory_changes`\n\n * "
+        "`watch_attributes_directory_changes` (`macOS` is not supported at this time)\n\n * "
+        "`watch_permissions_directory_changes` (`macOS` is not supported at this time)\n\nFile system file "
         "monitoring:\n\n * `watch_rename_file_changes`\n\n * `watch_write_file_changes`\n\n * "
         "`watch_create_file_changes`\n\n * `watch_delete_file_changes`\n\n * `watch_attributes_file_changes` (`macOS` "
         "is not supported at this time)\n\n * `watch_permissions_file_changes` (`macOS` is not supported at this "
         "time)\n\nWindows registry key and value monitoring: \n\n * `watch_create_key_changes`\n\n * "
         "`watch_delete_key_changes`\n\n * `watch_rename_key_changes`\n\n * `watch_set_value_changes`\n\n * "
         "`watch_delete_value_changes`\n\n * `watch_create_file_changes`",
         "name": "body",
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_firewall_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_firewall_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_foundry_logscale.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_foundry_logscale.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_host_group.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_hosts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_identity_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_image_assessment_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_image_assessment_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_incidents.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_installation_tokens.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_intel.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ioc.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_iocs.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_kubernetes_protection.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     "Bucket clusters by kubernetes version",
     "kubernetes_protection",
     [
       {
         "type": "string",
         "description": "Retrieve count of Kubernetes clusters that match a query in Falcon Query Language "
         "(FQL). Supported filters:  access,agent_status,cid,cloud_account_id,cloud_name,cloud_region,cluster_id,cluster"
-        "_name,cluster_status,container_count,iar_coverage,kubernetes_version,last_seen, management_status, node_count,"
-        "pod_count, tags",
+        "_name,cluster_status,container_count,kubernetes_version,last_seen, management_status, node_count, pod_count, "
+        "tags",
         "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
     "ReadClustersByStatusCount",
@@ -71,16 +71,16 @@
     "Bucket clusters by status",
     "kubernetes_protection",
     [
       {
         "type": "string",
         "description": "Retrieve count of Kubernetes clusters that match a query in Falcon Query Language "
         "(FQL). Supported filters:  access,agent_status,cid,cloud_account_id,cloud_name,cloud_region,cluster_id,cluster"
-        "_name,cluster_status,container_count,iar_coverage,kubernetes_version,last_seen, management_status, node_count,"
-        "pod_count, tags",
+        "_name,cluster_status,container_count,kubernetes_version,last_seen, management_status, node_count, pod_count, "
+        "tags",
         "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
     "ReadClusterCount",
@@ -89,16 +89,16 @@
     "Retrieve cluster counts",
     "kubernetes_protection",
     [
       {
         "type": "string",
         "description": "Retrieve count of Kubernetes clusters that match a query in Falcon Query Language "
         "(FQL). Supported filters:  access,agent_status,cid,cloud_account_id,cloud_name,cloud_region,cluster_id,cluster"
-        "_name,cluster_status,container_count,iar_coverage,kubernetes_version,last_seen, management_status, node_count,"
-        "pod_count, tags",
+        "_name,cluster_status,container_count,kubernetes_version,last_seen, management_status, node_count, pod_count, "
+        "tags",
         "name": "filter",
         "in": "query"
       }
     ]
   ],
   [
     "ReadContainersByDateRangeCount",
@@ -666,16 +666,15 @@
     "Retrieve kubernetes clusters identified by the provided filter criteria",
     "kubernetes_protection",
     [
       {
         "type": "string",
         "description": "Search Kubernetes clusters using a query in Falcon Query Language (FQL). Supported "
         "filters:  access,agent_status,cid,cloud_account_id,cloud_name,cloud_region,cluster_id,cluster_name,cluster_sta"
-        "tus,container_count,iar_coverage,kubernetes_version,last_seen, management_status, node_count, pod_count, "
-        "tags",
+        "tus,container_count,kubernetes_version,last_seen, management_status, node_count, pod_count, tags",
         "name": "filter",
         "in": "query"
       },
       {
         "type": "integer",
         "description": "The upper-bound on the number of records to retrieve.",
         "name": "limit",
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_malquery.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_message_center.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_message_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,16 +192,16 @@
         "type": "integer",
         "description": "The maximum records to return. [1-500]",
         "name": "limit",
         "in": "query"
       },
       {
         "enum": [
-          "activity.created_time.asc",
-          "activity.created_time.desc"
+          "activity.type.asc",
+          "activity.type.desc"
         ],
         "type": "string",
         "description": "The property to sort on, followed by a dot (.), followed by the sort direction, either "
         "\"asc\" or \"desc\".",
         "name": "sort",
         "in": "query"
       },
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ml_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_mssp.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_oauth2.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_ods.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_prevention_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_prevention_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_quarantine.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_quick_scan.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_real_time_response.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_real_time_response_audit.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_real_time_response_audit.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_recon.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_report_executions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_response_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sample_uploads.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sensor_download.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sensor_update_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sensor_update_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_unidentified_containers.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_unidentified_containers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_user_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_workflows.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_workflows.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/_zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_custom_ioa.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_discover.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_fdr.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_firewall_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_hosts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_identity_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_installation_tokens.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_ioc.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_iocs.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_mapping.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_mapping.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_ods.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_real_time_response.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_report_executions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/_base_url.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/_container_base_url.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/_container_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_enum/_token_fail_reason.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_enum/_token_fail_reason.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/_exceptions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/_exceptions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_error/_warnings.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_error/_warnings.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_log/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_log/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_log/_facility.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_log/_facility.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_cloud_snapshots.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_cloud_snapshots.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_container.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_cspm_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_detects.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_device_control_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_device_control_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_falconx.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_falconx.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_filevantage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_filevantage.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,14 @@
         "exclude": "string",
         "exclude_processes": "string",
         "exclude_users": "string",
         "id": "string",
         "include": "string",
         "include_processes": "string",
         "include_users": "string",
-        "content_files": "string",
-        "content_registry_values": "string",
-        "enable_content_capture": boolean,
-        "enable_hash_capture": boolean,
         "modified_timestamp": "string",
         "path": "string",
         "precedence": integer,
         "rule_group_id": "string",
         "severity": "string",
         "type": "string",
         "watch_attributes_directory_changes": boolean,
@@ -146,25 +142,23 @@
         "watch_write_file_changes": boolean
     }
     """
     returned = {}
     keys = ["created_timestamp", "depth", "description", "exclude", "exclude_processes",
             "exclude_users", "id", "include", "include_processes", "include_users",
             "modified_timestamp", "path", "rule_group_id", "severity", "type",
-            "content_files", "content_registry_values"
             ]
     bool_int_keys = ["watch_attributes_directory_changes", "watch_attributes_file_changes",
                      "watch_create_directory_changes", "watch_create_file_changes",
                      "watch_create_key_changes", "watch_delete_directory_changes",
                      "watch_delete_file_changes", "watch_delete_key_changes",
                      "watch_delete_value_changes", "watch_permissions_directory_changes",
                      "watch_permissions_file_changes", "watch_rename_directory_changes",
                      "watch_rename_file_changes", "watch_rename_key_changes",
-                     "watch_set_value_changes", "watch_write_file_changes", "precedence",
-                     "enable_content_capture", "enable_hash_capture"
+                     "watch_set_value_changes", "watch_write_file_changes", "precedence"
                      ]
     for key in keys:
         if passed_keywords.get(key, None):
             returned[key] = passed_keywords.get(key, None)
     for key in bool_int_keys:
         if passed_keywords.get(key, None) is not None:
             returned[key] = passed_keywords.get(key, None)
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_firewall.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_firewall.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_foundry.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_foundry.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_generic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_generic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_host_group.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_incidents.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_ioa.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_ioc.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_malquery.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_message_center.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_mssp.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_ods.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_prevention_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_real_time_response.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_recon.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_reports.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_response_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_response_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_sample_uploads.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_sensor_update_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_payload/_workflows.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_payload/_workflows.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/__base_resource.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/__base_resource.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_base_dictionary.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_base_dictionary.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_errors.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_errors.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_expanded_result.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_expanded_result.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_headers.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_headers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_meta.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_resources.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_resources.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_response_component.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_response_component.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_result/_result.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_result/_result.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/_base_service_class.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/_base_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_service_class/_service_class.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_service_class/_service_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     # |___ |__| | \| ___]  |  |  \ |__| |___  |  |__| |  \
     #
     # Override the default auth_object class to be our extended Service Class
     # object (OAuth2). Implement extended headers and payload validation and
     # provide a solution for maintaining instantiated class specific properties.
     #
     def __init__(self: "ServiceClass",
-                 auth_object: Optional[Union[FalconInterface, OAuth2]] = None,
+                 auth_object: Optional[FalconInterface or OAuth2] = None,
                  default_auth_object_class: Optional[Type[FalconInterface]] = OAuth2,
                  **kwargs
                  ):
         """Service Class base constructor.
 
         Instantiates the object, ingests authorization, and initializes attributes.
 
@@ -171,19 +171,14 @@
                 setattr(self, f"_override_{item}", kwargs.get(item))
 
         # Service Classes automatically log themselves in upon instantiation
         # if no authentication status is present.
         if not self.token_status:
             self.login()
 
-        # Detect if object authentication is being used to instantiate this class.
-        self._override_auth_style: str = None
-        if isinstance(auth_object, FalconInterface):
-            self.auth_style = "OBJECT"
-
         # Log the creation of this Service Class if debugging is enabled.
         if self.log:
             log_class_startup(self, self.log)
 
     # _  _ ____ ___ _  _ ____ ___  ____
     # |\/| |___  |  |__| |  | |  \ [__
     # |  | |___  |  |  | |__| |__/ ___]
@@ -322,29 +317,14 @@
         return returned
 
     @user_agent.setter
     def user_agent(self, value: int):
         """Allow the user_agent to be changed for this instance of the class."""
         self._override_user_agent = value
 
-    @property
-    def auth_style(self) -> str:
-        """Return the authentication mechanism used for instantiating this class."""
-        if self._override_auth_style:
-            returned = self._override_auth_style
-        else:
-            returned = self.auth_object.auth_style
-
-        return returned
-
-    @auth_style.setter
-    def auth_style(self, value: str):
-        """Allow the authentication mechanism to be specified per instance of the class."""
-        self._override_auth_style = value
-
     # Override the headers read only property to inject our ext_headers.
     # The Uber Class accomplishes this functionality differently.
     @property
     def headers(self) -> Dict[str, str]:
         """Provide a complete set of request headers."""
         return {
             ** self.auth_object.auth_headers,
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from ._auth import login_payloads, logout_payloads, review_provided_credentials
+from ._auth import login_payloads, logout_payloads
 from ._functions import (
     validate_payload,
     generate_b64cred,
     handle_single_argument,
     force_default,
     service_request,
     perform_request,
@@ -73,9 +73,9 @@
            "handle_container_operations", "uber_request_keywords", "autodiscover_region",
            "validate_payload", "generate_b64cred", "handle_single_argument", "force_default",
            "service_request", "perform_request", "generate_error_result", "generate_ok_result",
            "get_default", "args_to_params", "process_service_request", "confirm_base_url",
            "confirm_base_region", "return_preferred_default", "base_url_regions",
            "_ALLOWED_METHODS", "login_payloads", "logout_payloads", "sanitize_dictionary",
            "calc_content_return", "log_class_startup", "service_override_payload",
-           "deprecated_operation", "deprecated_class", "review_provided_credentials"
+           "deprecated_operation", "deprecated_class"
            ]
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_auth.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/mobile_enrollment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Internal authentication utilities library.
+"""Falcon Mobile Enrollment API Interface Class.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -31,89 +31,94 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from typing import Dict, Optional
-from json import loads
-try:
-    from simplejson import JSONDecodeError
-except (ImportError, ModuleNotFoundError):  # Support import as a module
-    from json.decoder import JSONDecodeError
-from ._functions import generate_b64cred
-from .._endpoint._oauth2 import _oauth2_endpoints as AuthEndpoints
-from .._error import InvalidCredentialFormat
-
-
-def login_payloads(creds: dict, base: str):
-    """Craft the necessary payloads to generate a token.
-
-    This method is intentionally generic and does not necessarily need to
-    be used to generate the token currently being used for other API operations.
-    """
-    op_id = "oauth2AccessToken"
-    target = f"{base}{[ep[2] for ep in AuthEndpoints if op_id in ep[0]][0]}"
-    data = {
-        'client_id': creds['client_id'],
-        'client_secret': creds['client_secret']
-    }
-    if "member_cid" in creds:
-        data["member_cid"] = creds["member_cid"]
-
-    return op_id, target, data
-
-
-def logout_payloads(creds: dict, base: str, token_val: str, client_id: str = None):
-    """Craft the necessary payloads to revoke a token.
-
-    This method is intentionally generic and does not necessarily need to
-    be used to revoke the token currently being used for other API operations.
+from typing import Dict, Union
+from ._util import process_service_request, force_default
+from ._service_class import ServiceClass
+from ._endpoint._mobile_enrollment import _mobile_enrollment_endpoints as Endpoints
+
+
+class MobileEnrollment(ServiceClass):
+    """This class represents the CrowdStrike Falcon Mobile Enrollment service collection.
+
+    The only requirement to instantiate an instance of this class is one of the following:
+    - valid API credentials provided as the keywords `client_id` and `client_secret`
+    - a `creds` dictionary containing valid credentials within the client_id and client_secret keys
+
+          {
+              "client_id": "CLIENT_ID_HERE",
+              "client_secret": "CLIENT_SECRET_HERE"
+          }
+    - an `auth_object` containing a valid instance of the authentication service class (OAuth2)
+    - a valid token provided by the token method of the authentication service class (OAuth2.token)
     """
-    op_id = "oauth2RevokeToken"
-    target = f"{base}{[ep[2] for ep in AuthEndpoints if op_id in ep[0]][0]}"
-    b64cred = generate_b64cred(creds["client_id"], creds["client_secret"])
-    headers = {"Authorization": f"basic {b64cred}"}
-    data = {"token": f"{token_val}"}
-    if client_id:
-        data["client_id"] = client_id
-
-    return op_id, target, data, headers
-
-
-def review_provided_credentials(cid: Optional[str] = None,
-                                csec: Optional[str] = None,
-                                cdict: Optional[Dict[str, str]] = None,
-                                mcid: Optional[str] = None
-                                ):
-    """Review the provided credential values and create a valid credential dictionary."""
-    returned = {}
-    returned_style = None
-    if cid and csec and not cdict:
-        cdict = {
-            "client_id": cid,
-            "client_secret": csec
-        }
-        # You must pass member_cid the same way you pass client_id / secret.
-        # If you use a creds dictionary, pass the member_cid there instead.
-        if mcid:
-            cdict["member_cid"] = mcid
-        returned_style = "DIRECT"
-    elif not cdict:
-        cdict = {}
-    # Credential Authentication (also powers Direct Authentication).
-    if isinstance(cdict, str):
-        try:
-            # Try and clean up any attempts to provide the dictionary as a string
-            returned: Dict[str, str] = loads(cdict.replace("'", "\""))
-            returned_style = "CREDENTIAL"
-        except (TypeError, JSONDecodeError) as bad_cred_format:
-            raise InvalidCredentialFormat from bad_cred_format
-    elif isinstance(cdict, dict):
-        returned: Dict[str, str] = cdict
-        if not returned_style:
-            returned_style = "CREDENTIAL"
-    else:
-        raise InvalidCredentialFormat
 
-    return returned, returned_style
+    @force_default(defaults=["body", "parameters"], default_types=["dict", "dict"])
+    def device_enroll(self: object, body: dict = None, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Trigger on-boarding process for a mobile device.
+
+        HTTP Method: POST
+
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/mobile-enrollment/RequestDeviceEnrollmentV3
+
+        Keyword arguments
+        ----
+        action_name : str
+            Action to perform. String. Allowed values: enroll, re-enroll.
+        body : str
+            Full body payload, not required if using `email_addresses` and `expires_at` keywords.
+                {
+                    "email_addresses": [
+                        "string"
+                    ],
+                    "expires_at": "2022-08-07T02:37:16.797Z"
+                }
+        email_addresses : str or list[str] (required)
+            Email addresses to use for enrollment. String or list of strings.
+        expires_at : str (required)
+            Date enrollment expires. UTC date format.
+        filter : str
+            FQL filter.
+        parameters : str
+            Full parameters payload, not required if using `action_name` keyword.
+
+        Arguments
+        ----
+        This method only supports keywords for providing arguments.
+
+        Returns
+        ----
+        dict
+            Dictionary containing API response.
+        """
+        if not body:
+            provided = kwargs.get("email_addresses", None)
+            if provided:
+                if isinstance(provided, str):
+                    provided = provided.split(",")
+                body["email_addresses"] = provided
+            if kwargs.get("expires_at", None):
+                body["expires_at"] = kwargs.get("expires_at", None)
+
+        return process_service_request(
+            calling_object=self,
+            endpoints=Endpoints,
+            operation_id="RequestDeviceEnrollmentV3",
+            body=body,
+            keywords=kwargs,
+            params=parameters
+            )
+
+    # This method name aligns to the operation ID in the API but
+    # does not conform to snake_case / PEP8 and is defined here for
+    # backwards compatibility / ease of use purposes
+    RequestDeviceEnrollmentV3 = device_enroll
+
+
+# The legacy name for this class does not conform to PascalCase / PEP8
+# It is defined here for backwards compatibility purposes only.
+Mobile_Enrollment = MobileEnrollment  # pylint: disable=C0103
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_functions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,23 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-from __future__ import annotations
 import base64
 import functools
 from warnings import warn
 from json import loads
 try:
     from simplejson import JSONDecodeError
 except (ImportError, ModuleNotFoundError):  # Support import as a module
     from json.decoder import JSONDecodeError
-from typing import Dict, Any, Union, Optional, List, TYPE_CHECKING
+from typing import Dict, Any, Union, Optional, List
 from copy import deepcopy
 from logging import Logger
 import requests
 import urllib3
 from urllib3.exceptions import InsecureRequestWarning
 from .._api_request import APIRequest
 from .._endpoint import operation_deprecation_mapping
@@ -72,20 +71,14 @@
     InvalidBaseURL,
     SSLDisabledWarning,
     UnnecessaryEncodingUsed,
     DeprecatedOperation,
     DeprecatedClass
     )
 from .._result import Result
-if TYPE_CHECKING:  # pragma: no cover
-    from .._auth_object import FalconInterface
-    from .._service_class import ServiceClass
-    from ..api_complete import APIHarness, APIHarnessV2
-    from ..oauth2 import OAuth2
-
 urllib3.disable_warnings(InsecureRequestWarning)
 
 
 def validate_payload(validator: Dict[str, Any],
                      payload: Dict[str, Union[str, int, dict, list, bytes]],
                      required: Optional[List[str]] = None
                      ) -> bool:
@@ -199,15 +192,17 @@
             except (SDKError, InvalidMethod) as bad_sdk_command:
                 created = bad_sdk_command.result
             return created
         return factory
     return wrapper
 
 
-def service_request(caller: ServiceClass = None, **kwargs) -> Union[Dict[str, Union[int, dict, list]], bytes]:
+# Caller is a derivitive of ServiceClass below, but we cannot type it until after
+# support for Python 3.6 is dropped due to the circular reference it would cause.
+def service_request(caller=None, **kwargs) -> Union[Dict[str, Union[int, dict, list]], bytes]:
     """Prepare and then perform the request (Service Classes only).
 
     Inbound caller argument should be a ServiceClass class or derivative.
     """
     if caller:
         # EAFP
         try:
@@ -609,16 +604,16 @@
                 returned_payload[element.__name__] = payload[element]
             else:
                 returned_payload[element] = payload[element]
 
     return returned_payload
 
 
-def process_service_request(calling_object: ServiceClass,  # pylint: disable=R0914 # (19/15)
-                            endpoints: List[List[Union[str, List[Dict[str, Any]]]]],
+def process_service_request(calling_object,  # pylint: disable=R0914 # (19/15)
+                            endpoints: list,
                             operation_id: str,
                             **kwargs
                             ) -> dict:
     """Perform a request originating from a service class module.
 
     Calculate the target_url based upon the provided operation ID and endpoint list.
 
@@ -818,20 +813,18 @@
                                                                         )):]
         if "Authorization" in cleaned:
             cleaned["Authorization"] = "Bearer REDACTED"
 
     return cleaned
 
 
-def log_class_startup(interface: Union[FalconInterface, ServiceClass, APIHarness, APIHarnessV2, OAuth2],
-                      log_device: Logger
-                      ):
+# Python 3.6 compatibility warning: Cannot properly type the interface.
+def log_class_startup(interface, log_device: Logger):
     """Log the startup of one of our interface or Service Classes."""
     log_device.debug("CREATED: %s interface class", interface.__class__.__name__)
-    log_device.debug("AUTH: Configured for %s Authentication", interface.auth_style.title())
     log_device.debug("CONFIG: Base URL set to %s", interface.base_url)
     log_device.debug("CONFIG: SSL verification is set to %s", str(interface.ssl_verify))
     log_device.debug("CONFIG: Timeout set to %s seconds", str(interface.timeout))
     log_device.debug("CONFIG: Proxy dictionary: %s", str(interface.proxy))
     log_device.debug("CONFIG: User-Agent string set to: %s", interface.user_agent)
     log_device.debug("CONFIG: Token renewal window set to %s seconds",
                      str(interface.renew_window)
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_service.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_service.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_util/_uber.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_util/_uber.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/_version.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-_VERSION = '1.4.3'
+_VERSION = '1.4.3.dev1'
 _MAINTAINER = 'Joshua Hiller'
 _AUTHOR = 'CrowdStrike'
 _AUTHOR_EMAIL = 'falconpy@crowdstrike.com'
 _CREDITS = 'CrowdStrike'
 _DESCRIPTION = "The CrowdStrike Falcon SDK for Python 3"
 _TITLE = "crowdstrike-falconpy"
 _PROJECT_URL = "https://github.com/CrowdStrike/falconpy"
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/__init__.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/_advanced.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/_advanced.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/api_complete/_legacy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/api_complete/_legacy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/cloud_snapshots.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/cloud_snapshots.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/configuration_assessment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/configuration_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/configuration_assessment_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/configuration_assessment_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_detections.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_detections.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_images.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_images.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_packages.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_packages.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/container_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/container_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/cspm_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/cspm_registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -229,15 +229,14 @@
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
             operation_id="PatchCSPMAwsAccount",
             body=body
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
     def get_aws_console_setup_urls(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve setup URLs for the AWS console.
 
         Returns a URL for customers to visit in their cloud environment
         to grant access to CrowdStrike.
 
         Keyword arguments:
@@ -259,15 +258,14 @@
             calling_object=self,
             endpoints=Endpoints,
             operation_id="GetCSPMAwsConsoleSetupURLs",
             keywords=kwargs,
             params=parameters
             )
 
-    @force_default(defaults=["parameters"], default_types=["dict"])
     def get_aws_account_scripts_attachment(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
         """Retrieve AWS account scripts.
 
         Return a script for customers to run in their cloud environment
         to grant access to CrowdStrike for their AWS environment.
 
         Keyword arguments:
@@ -1001,72 +999,14 @@
             calling_object=self,
             endpoints=Endpoints,
             operation_id="GetCSPMGCPServiceAccountsExt",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "id")
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def update_gcp_service_account(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Update a GCP service account.
-
-        Keyword arguments:
-        body -- full body payload, not required if using other keywords.
-                {
-                    "resources": [
-                        {
-                            "client_email": "string",
-                            "client_id": "string",
-                            "private_key": "string",
-                            "private_key_id": "string",
-                            "project_id": "string",
-                            "service_account_conditions": [
-                                {
-                                    "feature": "string",
-                                    "is_visible": boolean,
-                                    "last_transition": "UTC date string",
-                                    "message": "string",
-                                    "reason": "string",
-                                    "status": "string",
-                                    "type": "string"
-                                }
-                            ],
-                            "service_account_id": 0
-                        }
-                    ]
-                }
-        client_email -- Client email associated with the service account. String.
-        client_id -- GCP Client ID. String.
-        private_key -- GCP private key. String.
-        private_key_id -- GCP private key ID. String.
-        project_id -- GCP project ID. String.
-        resources -- List of GCP service accounts to validate. List of dictionaries.
-                     Overrides other keywords except for body.
-        service_account_conditions -- GCP service account conditions. List of dictionaries.
-        service_account_id -- GCP service account ID. Integer.
-
-        This method only supports keywords for providing arguments.
-
-        Returns: dict object containing API response.
-
-        HTTP Method: PATCH
-
-        Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/cspm-registration/UpdateCSPMGCPServiceAccountsExt
-        """
-        if not body:
-            body = cspm_service_account_validate_payload(passed_keywords=kwargs)
-
-        return process_service_request(
-            calling_object=self,
-            endpoints=Endpoints,
-            operation_id="UpdateCSPMGCPServiceAccountsExt",
-            body=body
-            )
-
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_gcp_user_scripts_attachment(self: object,
                                         *args,
                                         parameters: dict = None,
                                         **kwargs
                                         ) -> Dict[str, Union[int, dict]]:
         """Retrieve GCP user script attachment.
@@ -1635,15 +1575,14 @@
     CreateCSPMGCPAccount = create_gcp_account
     DeleteCSPMGCPAccount = delete_gcp_account
     UpdateCSPMGCPAccount = update_gcp_account
     ConnectCSPMGCPAccount = connect_gcp_account
     GetCSPMGCPValidateAccountsExt = validate_gcp_account
     ValidateCSPMGCPServiceAccountExt = validate_gcp_service_account
     GetCSPMGCPServiceAccountsExt = get_gcp_service_account
-    UpdateCSPMGCPServiceAccountsExt = update_gcp_service_account
     GetCSPMGCPUserScriptsAttachment = get_gcp_user_scripts_attachment
     GetBehaviorDetections = get_behavior_detections
     GetConfigurationDetections = get_configuration_detections
     GetConfigurationDetectionEntities = get_configuration_detection_entities
     GetConfigurationDetectionIDsV2 = get_configuration_detection_ids_v2
     GetIOAEvents = get_ioa_events
     GetIOAUsers = get_ioa_users
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/custom_ioa.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/custom_storage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/custom_storage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/d4c_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/d4c_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 For more information, please refer to <https://unlicense.org>
 """
 from typing import Dict, Union
 from ._util import force_default, process_service_request, handle_single_argument
 from ._payload import (
     azure_registration_payload,
     aws_d4c_registration_payload,
-    gcp_registration_payload,
-    cspm_service_account_validate_payload
+    gcp_registration_payload
     )
 from ._service_class import ServiceClass
 from ._endpoint._d4c_registration import _d4c_registration_endpoints as Endpoints
 
 
 class D4CRegistration(ServiceClass):
     """The only requirement to instantiate an instance of this class is one of the following.
@@ -574,72 +573,14 @@
             calling_object=self,
             endpoints=Endpoints,
             operation_id="GetD4CGCPServiceAccountsExt",
             keywords=kwargs,
             params=handle_single_argument(args, parameters, "id")
             )
 
-    @force_default(defaults=["body"], default_types=["dict"])
-    def update_gcp_service_account(self: object, body: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Update a GCP service account.
-
-        Keyword arguments:
-        body -- full body payload, not required if using other keywords.
-                {
-                    "resources": [
-                        {
-                            "client_email": "string",
-                            "client_id": "string",
-                            "private_key": "string",
-                            "private_key_id": "string",
-                            "project_id": "string",
-                            "service_account_conditions": [
-                                {
-                                    "feature": "string",
-                                    "is_visible": boolean,
-                                    "last_transition": "UTC date string",
-                                    "message": "string",
-                                    "reason": "string",
-                                    "status": "string",
-                                    "type": "string"
-                                }
-                            ],
-                            "service_account_id": 0
-                        }
-                    ]
-                }
-        client_email -- Client email associated with the service account. String.
-        client_id -- GCP Client ID. String.
-        private_key -- GCP private key. String.
-        private_key_id -- GCP private key ID. String.
-        project_id -- GCP project ID. String.
-        resources -- List of GCP service accounts to validate. List of dictionaries.
-                     Overrides other keywords except for body.
-        service_account_conditions -- GCP service account conditions. List of dictionaries.
-        service_account_id -- GCP service account ID. Integer.
-
-        This method only supports keywords for providing arguments.
-
-        Returns: dict object containing API response.
-
-        HTTP Method: PATCH
-
-        Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/d4c-registration/UpdateD4CGCPServiceAccountsExt
-        """
-        if not body:
-            body = cspm_service_account_validate_payload(passed_keywords=kwargs)
-
-        return process_service_request(
-            calling_object=self,
-            endpoints=Endpoints,
-            operation_id="UpdateD4CGCPServiceAccountsExt",
-            body=body
-            )
-
     @force_default(defaults=["parameters"], default_types=["dict"])
     def get_gcp_user_scripts_attachment_v2(self: object,
                                            *args,
                                            parameters: dict = None,
                                            **kwargs
                                            ) -> Dict[str, Union[int, dict]]:
         """Retrieve GCP user script attachment.
@@ -826,15 +767,14 @@
     GetD4CCGPAccount = get_gcp_account
     CreateCSPMGCPAccount = create_gcp_account
     CreateD4CGCPAccount = create_gcp_account
     DeleteD4CGCPAccount = delete_gcp_account
     ConnectD4CGCPAccount = connect_gcp_account
     GetD4CGCPUserScriptsAttachment = get_gcp_user_scripts_attachment_v2
     GetD4CGCPServiceAccountsExt = get_gcp_service_account
-    UpdateD4CGCPServiceAccountsExt = update_gcp_service_account
     GetCSPMGCPUserScriptsAttachment = get_gcp_user_scripts_attachment
     GetCSPMGCPUserScripts = get_gcp_user_scripts
     GetD4CGCPUserScripts = get_gcp_user_scripts
     GetHorizonD4CScripts = get_aws_horizon_scripts
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/debug.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/debug.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/detects.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/device_control_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/discover.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/drift_indicators.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/drift_indicators.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/event_streams.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/falcon_container.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/fdr.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/filevantage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/filevantage.py`

 * *Files 4% similar despite different names*

```diff
@@ -553,40 +553,36 @@
                    "exclude": "string",
                    "exclude_processes": "string",
                    "exclude_users": "string",
                    "id": "string",
                    "include": "string",
                    "include_processes": "string",
                    "include_users": "string",
-                   "content_files": "string",
-                   "content_registry_values": "string",
-                   "enable_content_capture": boolean,
-                   "enable_hash_capture": boolean,
                    "modified_timestamp": "string",
                    "path": "string",
                    "precedence": 0,
                    "rule_group_id": "string",
                    "severity": "string",
                    "type": "string",
-                   "watch_attributes_directory_changes": boolean,
-                   "watch_attributes_file_changes": boolean,
-                   "watch_create_directory_changes": boolean,
-                   "watch_create_file_changes": boolean,
-                   "watch_create_key_changes": boolean,
-                   "watch_delete_directory_changes": boolean,
-                   "watch_delete_file_changes": boolean,
-                   "watch_delete_key_changes": boolean,
-                   "watch_delete_value_changes": boolean,
-                   "watch_permissions_directory_changes": boolean,
-                   "watch_permissions_file_changes": boolean,
-                   "watch_rename_directory_changes": boolean,
-                   "watch_rename_file_changes": boolean,
-                   "watch_rename_key_changes": boolean,
-                   "watch_set_value_changes": boolean,
-                   "watch_write_file_changes": boolean
+                   "watch_attributes_directory_changes": true,
+                   "watch_attributes_file_changes": true,
+                   "watch_create_directory_changes": true,
+                   "watch_create_file_changes": true,
+                   "watch_create_key_changes": true,
+                   "watch_delete_directory_changes": true,
+                   "watch_delete_file_changes": true,
+                   "watch_delete_key_changes": true,
+                   "watch_delete_value_changes": true,
+                   "watch_permissions_directory_changes": true,
+                   "watch_permissions_file_changes": true,
+                   "watch_rename_directory_changes": true,
+                   "watch_rename_file_changes": true,
+                   "watch_rename_key_changes": true,
+                   "watch_set_value_changes": true,
+                   "watch_write_file_changes": true
                }
         description -- The rule description. (String, 0-500 characters.)
         rule_group_id -- Group ID containing the group configuration. (String)
         path -- the file system or registry path to monitor. (String, 1-250 characters)
                 All paths must end with the path separator, e.g. c:\windows\ /usr/bin/
         severity -- to categorize change events produced by this rule. (String)
                     Allowed values: Low, Medium, High or Critical
@@ -600,46 +596,33 @@
                    Allowed rule group configuration is based on the type of rule
                    the rule group is added to.
         exclude -- the files, directories, registry keys, or registry values that will NOT be monitored. (String).
                    Falcon GLOB syntax is supported.
                    Allowed rule group configuration is based on the type of rule
                    the rule group is added to.
         include_users -- the changes performed by specific users that will be monitored. (String).
-                         Falcon GLOB syntax is supported.
-                         macOS is not supported at this time.
-                         Allowed rule group configuration is based on the type of rule
-                         the rule group is added to.
+                   Falcon GLOB syntax is supported.
+                   macOS is not supported at this time.
+                   Allowed rule group configuration is based on the type of rule
+                   the rule group is added to.
         exclude_users -- the changes performed by specific users that will NOT be monitored. (String).
-                         Falcon GLOB syntax is supported.
-                         macOS is not supported at this time.
-                         Allowed rule group configuration is based on the type of rule
-                         the rule group is added to.
+                   Falcon GLOB syntax is supported.
+                   macOS is not supported at this time.
+                   Allowed rule group configuration is based on the type of rule
+                   the rule group is added to.
         include_processes -- the changes performed by specific processes that will be monitored. (String).
-                             Falcon GLOB syntax is supported.
-                             macOS is not supported at this time.
-                             Allowed rule group configuration is based on the type of rule
-                             the rule group is added to.
+                   Falcon GLOB syntax is supported.
+                   macOS is not supported at this time.
+                   Allowed rule group configuration is based on the type of rule
+                   the rule group is added to.
         exclude_users -- the changes performed by specific processes that will be NOT monitored. (String).
                          Falcon GLOB syntax is supported.
                          macOS is not supported at this time.
                          Allowed rule group configuration is based on the type of rule
                          the rule group is added to.
-        exclude_processes -- the changes performed by the specific processes that will NOT be monitored. (String).
-                             Falcon GLOB syntax is supported.
-                             macOS is not supported at this time.
-                             Allowed rule group configuration is based on the type of rule
-                             the rule group is added to.
-        content_files -- the files whose content will be monitored. (String).
-                         Listed files must match the file include pattern
-                         and not match the file exclude pattern.
-        content_registry_values -- the registry values whose content will be monitored. (String).
-                                   Listed registry values must match the registry include pattern
-                                   and not match the registry exclude pattern.
-        enable_content_capture -- Enable content capturing. Boolean.
-        enable_hash_capture -- Enable hash capturing. Boolean.
         watch_delete_directory_changes -- File system directory monitoring. Boolean.
         watch_create_directory_changes -- File system directory monitoring. Boolean.
         watch_rename_directory_changes -- File system directory monitoring. Boolean.
         watch_attributes_directory_changes -- File system directory monitoring. Boolean.
                                               macOS is not supported at this time.
         watch_permissions_directory_changes -- File system directory monitoring. Boolean.
                                                macOS is not supported at this time.
@@ -722,40 +705,36 @@
                    "exclude": "string",
                    "exclude_processes": "string",
                    "exclude_users": "string",
                    "id": "string",
                    "include": "string",
                    "include_processes": "string",
                    "include_users": "string",
-                   "content_files": "string",
-                   "content_registry_values": "string",
-                   "enable_content_capture": boolean,
-                   "enable_hash_capture": boolean,
                    "modified_timestamp": "string",
                    "path": "string",
                    "precedence": 0,
                    "rule_group_id": "string",
                    "severity": "string",
                    "type": "string",
-                   "watch_attributes_directory_changes": boolean,
-                   "watch_attributes_file_changes": boolean,
-                   "watch_create_directory_changes": boolean,
-                   "watch_create_file_changes": boolean,
-                   "watch_create_key_changes": boolean,
-                   "watch_delete_directory_changes": boolean,
-                   "watch_delete_file_changes": boolean,
-                   "watch_delete_key_changes": boolean,
-                   "watch_delete_value_changes": boolean,
-                   "watch_permissions_directory_changes": boolean,
-                   "watch_permissions_file_changes": boolean,
-                   "watch_rename_directory_changes": boolean,
-                   "watch_rename_file_changes": boolean,
-                   "watch_rename_key_changes": boolean,
-                   "watch_set_value_changes": boolean,
-                   "watch_write_file_changes": boolean
+                   "watch_attributes_directory_changes": true,
+                   "watch_attributes_file_changes": true,
+                   "watch_create_directory_changes": true,
+                   "watch_create_file_changes": true,
+                   "watch_create_key_changes": true,
+                   "watch_delete_directory_changes": true,
+                   "watch_delete_file_changes": true,
+                   "watch_delete_key_changes": true,
+                   "watch_delete_value_changes": true,
+                   "watch_permissions_directory_changes": true,
+                   "watch_permissions_file_changes": true,
+                   "watch_rename_directory_changes": true,
+                   "watch_rename_file_changes": true,
+                   "watch_rename_key_changes": true,
+                   "watch_set_value_changes": true,
+                   "watch_write_file_changes": true
                }
         description -- The rule description. (String, 0-500 characters.)
         id -- ID of the rule to be updated. (String)
         rule_group_id -- Group ID containing the group configuration. (String)
         path -- the file system or registry path to monitor. (String, 1-250 characters)
                 All paths must end with the path separator, e.g. c:\windows\ /usr/bin/
         severity -- to categorize change events produced by this rule. (String)
@@ -789,27 +768,14 @@
                    Allowed rule group configuration is based on the type of rule
                    the rule group is added to.
         exclude_users -- the changes performed by specific processes that will be NOT monitored. (String).
                          Falcon GLOB syntax is supported.
                          macOS is not supported at this time.
                          Allowed rule group configuration is based on the type of rule
                          the rule group is added to.
-        exclude_processes -- the changes performed by the specific processes that will NOT be monitored. (String).
-                             Falcon GLOB syntax is supported.
-                             macOS is not supported at this time.
-                             Allowed rule group configuration is based on the type of rule
-                             the rule group is added to.
-        content_files -- the files whose content will be monitored. (String).
-                         Listed files must match the file include pattern
-                         and not match the file exclude pattern.
-        content_registry_values -- the registry values whose content will be monitored. (String).
-                                   Listed registry values must match the registry include pattern
-                                   and not match the registry exclude pattern.
-        enable_content_capture -- Enable content capturing. Boolean.
-        enable_hash_capture -- Enable hash capturing. Boolean.
         watch_delete_directory_changes -- File system directory monitoring. Boolean.
         watch_create_directory_changes -- File system directory monitoring. Boolean.
         watch_rename_directory_changes -- File system directory monitoring. Boolean.
         watch_attributes_directory_changes -- File system directory monitoring. Boolean.
                                               macOS is not supported at this time.
         watch_permissions_directory_changes -- File system directory monitoring. Boolean.
                                                macOS is not supported at this time.
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/firewall_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/firewall_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/foundry_logscale.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/foundry_logscale.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/host_group.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/hosts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/identity_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/image_assessment_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/image_assessment_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/incidents.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/installation_tokens.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/intel.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ioc.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/iocs.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/kubernetes_protection.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
                     agent_status            container_count
                     cid                     kubernetes_version
                     cloud_account_id        last_seen
                     cloud_name              management_status
                     cloud_region            node_count
                     cluster_id              pod_count
                     cluster_name            tags
-                    iar_coverage
         parameters -- Full parameters payload dictionary. Not required if using other keywords.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'filter'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
@@ -124,15 +123,14 @@
                     agent_status            container_count
                     cid                     kubernetes_version
                     cloud_account_id        last_seen
                     cloud_name              management_status
                     cloud_region            node_count
                     cluster_id              pod_count
                     cluster_name            tags
-                    iar_coverage
         parameters -- Full parameters payload dictionary. Not required if using other keywords.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'filter'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
@@ -160,15 +158,14 @@
                     agent_status            container_count
                     cid                     kubernetes_version
                     cloud_account_id        last_seen
                     cloud_name              management_status
                     cloud_region            node_count
                     cluster_id              pod_count
                     cluster_name            tags
-                    iar_coverage
         parameters -- Full parameters payload dictionary. Not required if using other keywords.
 
         Arguments: When not specified, the first argument to this method is assumed to be 'filter'.
                    All others are ignored.
 
         Returns: dict object containing API response.
 
@@ -1211,15 +1208,14 @@
                     agent_status        container_count
                     cid                 kubernetes_version
                     cloud_account_id    last_seen
                     cloud_name          management_status
                     cloud_region        node_count
                     cluster_id          pod_count
                     cluster_name        tags
-                    iar_coverage
         limit -- The upper-bound on the number of records to retrieve. Integer.
         offset -- The offset from where to begin. Integer.
         sort -- Field to sort results by. String.
         parameters -- Full parameters payload dictionary. Not required if using other keywords.
 
         This method only supports keywords for providing arguments.
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/malquery.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/message_center.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ml_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/real_time_response_audit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Falcon Mobile Enrollment API Interface Class.
+"""CrowdStrike Falcon Real Time Response Audit API interface class.
 
  _______                        __ _______ __        __ __
 |   _   .----.-----.--.--.--.--|  |   _   |  |_.----|__|  |--.-----.
 |.  1___|   _|  _  |  |  |  |  _  |   1___|   _|   _|  |    <|  -__|
 |.  |___|__| |_____|________|_____|____   |____|__| |__|__|__|_____|
 |:  1   |                         |:  1   |
 |::.. . |   CROWDSTRIKE FALCON    |::.. . |    FalconPy
@@ -32,93 +32,68 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 from typing import Dict, Union
-from ._util import process_service_request, force_default
+from ._util import force_default, process_service_request
 from ._service_class import ServiceClass
-from ._endpoint._mobile_enrollment import _mobile_enrollment_endpoints as Endpoints
+from ._endpoint._real_time_response_audit import _real_time_response_audit_endpoints as Endpoints
 
 
-class MobileEnrollment(ServiceClass):
-    """This class represents the CrowdStrike Falcon Mobile Enrollment service collection.
+class RealTimeResponseAudit(ServiceClass):
+    """The only requirement to instantiate an instance of this class is one of the following.
 
-    The only requirement to instantiate an instance of this class is one of the following:
-    - valid API credentials provided as the keywords `client_id` and `client_secret`
-    - a `creds` dictionary containing valid credentials within the client_id and client_secret keys
-
-          {
-              "client_id": "CLIENT_ID_HERE",
-              "client_secret": "CLIENT_SECRET_HERE"
-          }
-    - an `auth_object` containing a valid instance of the authentication service class (OAuth2)
-    - a valid token provided by the token method of the authentication service class (OAuth2.token)
+    - a valid client_id and client_secret provided as keywords.
+    - a credential dictionary with client_id and client_secret containing valid API credentials
+      {
+          "client_id": "CLIENT_ID_HERE",
+          "client_secret": "CLIENT_SECRET_HERE"
+      }
+    - a previously-authenticated instance of the authentication service class (oauth2.py)
+    - a valid token provided by the authentication service class (oauth2.py)
     """
 
-    @force_default(defaults=["body", "parameters"], default_types=["dict", "dict"])
-    def device_enroll(self: object, body: dict = None, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
-        """Trigger on-boarding process for a mobile device.
+    @force_default(defaults=["parameters"], default_types=["dict"])
+    def audit_sessions(self: object, parameters: dict = None, **kwargs) -> Dict[str, Union[int, dict]]:
+        """Get all the RTR sessions created for a customer during a specified time period.
+
+        Keyword arguments:
+        filter -- The filter expression that should be used to limit the results. FQL syntax.
+        limit -- The maximum number of sessions to return in this response. Integer.
+                 Use with the offset parameter to manage pagination of results.
+        offset -- Starting index of overall result set from which to return ids.
+                  Use with the limit parameter to manage pagination of results.
+        parameters - full parameters payload, not required if using other keywords.
+        sort -- The property to sort by. FQL syntax (e.g. date_created|asc).
+                Available sort fields: created_at, updated_at, deleted_at
+        with_command_info -- Retrieve sessions with command information included. By default
+                             sessions are returned without command information which includes
+                             cloud request IDs and log fields.
 
-        HTTP Method: POST
-
-        Swagger URL
-        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/mobile-enrollment/RequestDeviceEnrollmentV3
+        This method only supports keywords for providing arguments.
 
-        Keyword arguments
-        ----
-        action_name : str
-            Action to perform. String. Allowed values: enroll, re-enroll.
-        body : str
-            Full body payload, not required if using `email_addresses` and `expires_at` keywords.
-                {
-                    "email_addresses": [
-                        "string"
-                    ],
-                    "expires_at": "2022-08-07T02:37:16.797Z"
-                }
-        email_addresses : str or list[str] (required)
-            Email addresses to use for enrollment. String or list of strings.
-        expires_at : str (required)
-            Date enrollment expires. UTC date format.
-        filter : str
-            FQL filter.
-        parameters : str
-            Full parameters payload, not required if using `action_name` keyword.
+        Returns: dict object containing API response.
 
-        Arguments
-        ----
-        This method only supports keywords for providing arguments.
+        HTTP Method: GET
 
-        Returns
-        ----
-        dict
-            Dictionary containing API response.
+        Swagger URL
+        https://assets.falcon.crowdstrike.com/support/api/swagger.html#/real-time-response-audit/RTRAuditSessions
         """
-        if not body:
-            provided = kwargs.get("email_addresses", None)
-            if provided:
-                if isinstance(provided, str):
-                    provided = provided.split(",")
-                body["email_addresses"] = provided
-            if kwargs.get("expires_at", None):
-                body["expires_at"] = kwargs.get("expires_at", None)
-
         return process_service_request(
             calling_object=self,
             endpoints=Endpoints,
-            operation_id="RequestDeviceEnrollmentV3",
-            body=body,
+            operation_id="RTRAuditSessions",
             keywords=kwargs,
             params=parameters
             )
 
-    # This method name aligns to the operation ID in the API but
-    # does not conform to snake_case / PEP8 and is defined here for
+    # These method names align to the operation IDs in the API but
+    # do not conform to snake_case / PEP8 and are defined here for
     # backwards compatibility / ease of use purposes
-    RequestDeviceEnrollmentV3 = device_enroll
+    RTRAuditSessions = audit_sessions
 
 
 # The legacy name for this class does not conform to PascalCase / PEP8
 # It is defined here for backwards compatibility purposes only.
-Mobile_Enrollment = MobileEnrollment  # pylint: disable=C0103
+Real_Time_Response_Audit = RealTimeResponseAudit  # pylint: disable=C0103
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/mssp.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/oauth2.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/ods.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/prevention_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/quarantine.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/quick_scan.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/real_time_response.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/recon.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/report_executions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/response_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sample_uploads.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/scheduled_reports.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sensor_download.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sensor_update_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/unidentified_containers.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/unidentified_containers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/user_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/workflows.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,31 +169,22 @@
 
         HTTP Method: POST
 
         Swagger URL
         https://assets.falcon.crowdstrike.com/support/api/swagger.html#/workflows/WorkflowDefinitionsImport
         """
         data_file = kwargs.get("data_file", None)
-        content_type = "application/x-yaml"
-        # Create a multipart form payload for our upload file
-        try:
-            with open(data_file, "r", encoding="utf-8") as yaml_file:
-                file_data = yaml_file.read()
-                file_extended = {"name": "yaml_upload", "data_file": file_data, "type": content_type}
-        except FileNotFoundError:
-            data_file = None
-
-        if data_file and file_data:
+        if data_file:
             returned = process_service_request(
                         calling_object=self,
                         endpoints=Endpoints,
                         operation_id="WorkflowDefinitionsImport",
                         keywords=kwargs,
                         params=parameters,
-                        files=file_extended
+                        data=data_file
                         )
         else:
             returned = generate_error_result("You must provide a workflow file in YAML format to import.")
 
         return returned
 
     @force_default(defaults=["body", "parameters"], default_types=["dict", "dict"])
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/src/falconpydev/zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/src/falconpydev/zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_api_request.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_api_request.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_authentications.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_authentications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,59 @@
 # test_authentications.py
 # Tests different service class authentication styles
 import os
 import sys
 import pytest
+# from datetime import datetime
+# from logging import (
+#     getLogger,
+#     basicConfig,
+#     DEBUG,
+#     WARNING,
+#     ERROR,
+#     INFO,
+#     )
+from logging.handlers import RotatingFileHandler
+from contextvars import ContextVar, copy_context
+from typing import Dict
 # Authentication via the test_authorization.py
 from tests import test_authorization as Authorization
 # Import our sibling src folder into the path
 sys.path.append(os.path.abspath('src'))
 # Classes to test - manually imported from sibling folder
 from falconpy import (
     ZeroTrustAssessment,
+    CloudConnectAWS,
     OAuth2,
     APIHarness,
     version,
     InvalidCredentialFormat,
     Hosts,
     Detects
     )
+from dataclasses import field, dataclass
 from falconpy._util import confirm_base_region
 from falconpy._version import _TITLE, _VERSION
 
 auth = Authorization.TestAuthorization()
 auth.serviceAuth()
 AllowedResponses = [200, 401, 403, 429]
 _DEBUG = os.getenv("FALCONPY_UNIT_TEST_DEBUG", None)
 if _DEBUG:
     _DEBUG = True
 
+@dataclass
+class FoundryRequest:
+    access_token: str = field(default='')
+    body: Dict[str, any] = field(default_factory=lambda: {})
+    context: Dict[str, any] = field(default_factory=lambda: {})
+    method: str = field(default='')
+    params: Dict[str, any] = field(default_factory=lambda: {})
+    url: str = field(default='')
+
 
 class TestAuthentications:
 
     def serviceAny_TestCredentialAuthFailure(self):
         bad_falcon = ZeroTrustAssessment(creds={"client_id": "This", "client_secret": "WontWork"}, debug=_DEBUG)
         # Check the service class login code path at the same time
         bad_falcon.login()
@@ -322,23 +345,31 @@
     @pytest.mark.skipif(auth.authorization.base_url == "https://api.laggar.gcw.crowdstrike.com",
                         reason="Test unsupported in GovCloud"
                         )
     def test_string_credentials_dictionary(self):
         key = auth.config["falcon_client_id"]
         the_other_bit = auth.config["falcon_client_secret"]
         test_string = "{" + f"'client_id': '{key}', 'client_secret': '{the_other_bit}'" + "}"
-        test_object = Hosts(creds=test_string, debug=_DEBUG)
+        test_object = Hosts(creds=test_string)
         test_object.login()
         assert bool(test_object.authenticated())
 
     def test_bad_credentials_dictionary(self):
         _success = False
         test = "Bob"
         try:
             test_object = Hosts(creds=test)
         except InvalidCredentialFormat:
             test = 2
             try:
-                test_object = Hosts(creds=test, debug=_DEBUG)
+                test_object = Hosts(creds=test)
             except InvalidCredentialFormat:
                 _success = True
         assert _success
+
+    def test_foundry_authentication(self):
+        request_context = ContextVar("request", default=FoundryRequest())
+        req: FoundryRequest = request_context.get()
+        req.access_token = auth.authorization.token()["body"]["access_token"]
+        request_context.set(req)
+        hosts = Hosts(pythonic=True)
+        assert bool(hosts.query_devices_by_filter_scroll(limit=1).status_code == 200)
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_authorization.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_cloud_snapshots.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_cloud_snapshots.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_configuration_assessment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_configuration_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_configuration_assessment_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_configuration_assessment_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_container_alerts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_container_detections.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_detections.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 sys.path.append(os.path.abspath('src'))
 # Classes to test - manually imported from sibling folder
 from falconpy import ContainerDetections
 
 auth = Authorization.TestAuthorization()
 config = auth.getConfigObject()
 falcon = ContainerDetections(auth_object=config)
-AllowedResponses = [200, 201, 207, 400, 403, 404, 429]
+AllowedResponses = [200, 201, 207, 400, 404, 429]
 
 
 class TestContainerDetections:
     def test_all_code_paths(self):
         error_checks = True
         tests = {
             "ReadDetectionsCountBySeverity": falcon.read_detection_counts_by_severity("cid:'1234567890'"),
@@ -30,10 +30,10 @@
             "GetRuntimeDetectionsCombinedV2": falcon.search_runtime_detections(limit=1, filter="cid:'1234567'"),
             "ReadDetections": falcon.read_detections(limit=1, filter="cid:'1234567890'"),
             "SearchDetections": falcon.search_detections(filter="cid:'1234567890'", limit=1)
         }
         for key in tests:
             if tests[key]["status_code"] not in AllowedResponses:
                 error_checks = False
-                print(key)
-                print(tests[key])
+                # print(key)
+                # print(tests[key])
         assert error_checks
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_container_images.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_images.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_container_packages.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 sys.path.append(os.path.abspath('src'))
 # Classes to test - manually imported from sibling folder
 from falconpy import ContainerPackages
 
 auth = Authorization.TestAuthorization()
 config = auth.getConfigObject()
 falcon = ContainerPackages(auth_object=config)
-AllowedResponses = [200, 201, 207, 400, 403, 404, 429]
+AllowedResponses = [200, 201, 207, 400, 404, 429]
 
 
 class TestContainerPackages:
     def test_all_code_paths(self):
         error_checks = True
         tests = {
             "ReadPackagesCountByZeroDay": falcon.read_zero_day_counts(filter="cid:'12345678901234567890123456789012'"),
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_container_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_container_vulnerabilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 sys.path.append(os.path.abspath('src'))
 # Classes to test - manually imported from sibling folder
 from falconpy import ContainerVulnerabilities
 
 auth = Authorization.TestAuthorization()
 config = auth.getConfigObject()
 falcon = ContainerVulnerabilities(auth_object=config)
-AllowedResponses = [200, 201, 207, 400, 403, 404, 429]
+AllowedResponses = [200, 201, 207, 400, 404, 429]
 
 
 class TestContainerVulnerabilities:
     def test_all_code_paths(self):
         error_checks = True
         tests = {
             "ReadCombinedVulnerabilities": falcon.read_combined_vulnerabilities(filter="cid:'12345678901234567890123456789012'"),
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_cspm_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_cspm_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,14 @@
             "GetConfigurationDetectionIdsV2": falcon.get_configuration_detection_ids_v2(),
             "GetCSPMPoliciesDetails": falcon.get_policy_details(),
             "GetGCPAccount": falcon.get_gcp_account(ids="12345678", scan_type="dry"),
             "CreateGCPAccount": falcon.create_gcp_account(parent_id="whatever", parent_type="shiny"),
             "DeleteD4CGCPAccount": falcon.delete_gcp_account("1234567"),
             "ConnectD4CGCPAccount": falcon.connect_gcp_account(client_id="123456", parent_id="123456"),
             "GetD4CGCPServiceAccoutnExt": falcon.get_gcp_service_account(id="12345678"),
-            "UpdateCSPMGCPServiceAccountsExt": falcon.update_gcp_service_account(service_account_id=2),
             "GetD4CGCPUserScriptsAttachmentV2": falcon.get_gcp_user_scripts_attachment(ids="12345678"),
             "UpdateGCP": falcon.update_gcp_account(environment="temperate", parent_id="1234567"),
             "GetMgmt": falcon.get_azure_management_group(tenant_id="1234567"),
             "CreateMgmt": falcon.create_azure_management_group(default_subscription_id="bob", tenant_id="1234567"),
             "DeleteAzureManagementGroup": falcon.delete_azure_management_group("whatever_tenant_ID"),
             "UpdateAzure": falcon.update_azure_account(environment="chilly", subscription_id="banana"),
             "ValidateGCPAccount": falcon.validate_gcp_account("whatever_account_id"),
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_custom_ioa.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_custom_storage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_custom_storage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_d4c_registration.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_d4c_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,15 @@
             "GetD4CAwsConsoleSetupURLs": falcon.get_aws_console_setup("us-east-2"),
             "GetD4CAwsAccountScriptsAttachment": falcon.get_aws_account_scripts("123456789"),
             "GetHorizonD4CScripts": falcon.get_aws_horizon_scripts(organization_id="123456789"),
             "GetDiscoverCloudAzureTenantIDs": falcon.get_azure_tenant_ids(),
             "DeleteD4CGCPAccount": falcon.delete_gcp_account("1234567"),
             "ConnectD4CGCPAccount": falcon.connect_gcp_account(client_id="123456", parent_id="123456"),
             "GetD4CGCPServiceAccoutnExt": falcon.get_gcp_service_account(id="12345678"),
-            "GetD4CGCPUserScriptsAttachmentV2": falcon.get_gcp_user_scripts_attachment_v2(ids="12345678"),
-            "UpdateD4CGCPServiceAccountsExt": falcon.update_gcp_service_account(service_account_id=2),
+            "GetD4CGCPUserScriptsAttachmentV2": falcon.get_gcp_user_scripts_attachment_v2(ids="12345678")
         }
         for key in tests:
             if tests[key]["status_code"] != 500:
                 error_checks = False
 
             # print(f"{key} processed with a {tests[key]} response")
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_detects.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_device_control_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_discover.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_drift_indicators.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_drift_indicators.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 sys.path.append(os.path.abspath('src'))
 # Classes to test - manually imported from sibling folder
 from falconpy import DriftIndicators
 
 auth = Authorization.TestAuthorization()
 config = auth.getConfigObject()
 falcon = DriftIndicators(auth_object=config)
-AllowedResponses = [200, 201, 207, 400, 403, 404, 429]
+AllowedResponses = [200, 201, 207, 400, 404, 429]
 
 
 class TestDriftIndicators:
     def test_all_code_paths(self):
         error_checks = True
         tests = {
             "GetDriftIndicatorsValuesByDate": falcon.get_drift_indicators_by_date(filter="cid:'12345678901234567890123456789012'"),
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_event_streams.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_falcon_container.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_fdr.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_filevantage.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_firewall_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_firewall_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_foundry_logscale.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_foundry_logscale.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_host_group.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_hosts.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_identity_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_image_assessment_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_image_assessment_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_incidents.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_installation_tokens.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_intel.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_ioc.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_iocs.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_malquery.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_message_center.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_ml_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_mssp.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_ods.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_prevention_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_quarantine.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_quick_scan.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_real_time_response.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_real_time_response_audit.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_real_time_response_audit.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_recon.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_report_executions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_response_policies.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_result_object.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_result_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -748,16 +748,19 @@
                 hosts.query_devices_by_filter_scroll(filter="hostname%3A%27falconpy%27")
             except APIError:
                 _success = True
             hosts = Hosts(auth_object=hosts, pythonic=False)
             hosts.query_devices_by_filter_scroll(filter="hostname%3A%27falconpy%27")
             assert _success
 
+    @pytest.mark.skipif(config.base_url == "https://api.laggar.gcw.crowdstrike.com",
+                        reason="Unit testing unavailable on US-GOV-1"
+                        )
     @not_supported
-    @pytest.mark.skipif(config.base_url != "https://api.crowdstrike.com", reason="This unit test is only supported in US-1.")
+    @pytest.mark.skipif("us-1" not in config.base_url, reason="This unit test is only supported in US-1.")
     def test_pythonic_deprecation_warnings(self):
         _success = False
         with pytest.warns(SDKDeprecationWarning):
             warnings.warn(SDKDeprecationWarning(message="This is a generic deprecation warning", code=187))
         with pytest.warns(DeprecatedClass):
             warnings.warn(DeprecatedClass(code=187))
         with pytest.warns(DeprecatedOperation):
@@ -770,8 +773,8 @@
 
         with pytest.warns(DeprecatedOperation):
             try:
                 old_discover.get_aws_settings()
                 _success = True
             except:
                 pass
-        assert _success
+        assert _success
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_sample_uploads.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_sensor_download.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_sensor_update_policy.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_service_class.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_timeout.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_uber.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_uber.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,17 +355,16 @@
                     and falcon.headers()
                     and falcon.token
                     )
 
     def test_uber_deprecated_attributes(self):
         _success = False
         falcon.token_renew_window = 180
-        if falcon.authenticated() and not falcon.token_expired():
-            if falcon.token_renew_window == 180:
-                _success = True
+        if falcon.token_renew_window == 180:
+            _success = True
         assert _success
 
     def test_uber_properties(self):
         # Force a new object so we can flip the debug flag
         temp_falcon = APIHarnessV2(access_token=falcon.token_value,
                                  base_url=config["falcon_base_url"],
                                  debug=True
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_uber_api_complete.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_uber_api_complete.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_unidentified_containers.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_unidentified_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 sys.path.append(os.path.abspath('src'))
 # Classes to test - manually imported from sibling folder
 from falconpy import UnidentifiedContainers
 
 auth = Authorization.TestAuthorization()
 config = auth.getConfigObject()
 falcon = UnidentifiedContainers(auth_object=config)
-AllowedResponses = [200, 201, 207, 400, 403, 404, 429]
+AllowedResponses = [200, 201, 207, 400, 404, 429]
 
 
 class TestUnidentifiedContainers:
     def test_all_code_paths(self):
         error_checks = True
         tests = {
             "ReadUnidentifiedContainersByDateRangeCount": falcon.read_count_by_date_range("cluster_name:'bob'"),
```

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_user_management.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.4.3/tests/test_workflows.py` & `crowdstrike-falconpy-dev-1.4.3.dev1/tests/test_workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,15 @@
             "WorkflowSystemDefinitionsDeProvision" : falcon.deprovision(definition_id="12345", deprovision_all=True),
             "WorkflowSystemDefinitionsPromote" : falcon.promote(customer_definition_id="12345", activities={}),
             "WorkflowSystemDefinitionsProvision" : falcon.provision(name="FalconPyTesting", configuration=[{}]),
             "WorkflowDefinitionsCombined": falcon.search_definitions(),
             "WorkflowExecutionsCombined": falcon.search_executions(),
             "WorkflowDefinitionsExport": falcon.export_definition(),
             "WorkflowDefinitionsImport": falcon.import_definition(validate_only=True, data_file="this_will_415"),
-            "WorkflowDefinitionsImport2": falcon.import_definition(validate_only=True, file_data="this_will_500"),
-            "WorkflowDefinitionsImport3": falcon.import_definition(validate_only=True, data_file="not_here.yml"),
-            "WorkflowDefinitionsImport4": falcon.import_definition(validate_only=True, data_file="tests/test.yml"),
+            "WorkflowDefinitionsImport": falcon.import_definition(validate_only=True, file_data="this_will_500"),
             "WorkflowDefinitionsUpdate": falcon.update_definition(change_log="testing"),
             "WorkflowGetHumanInputV1": falcon.get_human_input(ids="1234567"),
             "WorkflowUpdateHumanInputV1": falcon.update_human_input(input="whatever", note="whatever"),
         }
         for key in tests:
             if tests[key]["status_code"] not in AllowedResponses:
                 error_checks = False
```

