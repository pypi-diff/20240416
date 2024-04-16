# Comparing `tmp/eclsdk-1.2.1.tar.gz` & `tmp/eclsdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eclsdk-1.2.1.tar", last modified: Thu Dec  1 02:49:45 2022, max compression
+gzip compressed data, was "eclsdk-1.3.0.tar", last modified: Tue Apr 16 05:37:35 2024, max compression
```

## Comparing `eclsdk-1.2.1.tar` & `eclsdk-1.3.0.tar`

### file list

```diff
@@ -1,650 +1,654 @@
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.322734 eclsdk-1.2.1/
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1646 2022-12-01 02:49:43.000000 eclsdk-1.2.1/AUTHORS
--rw-r--r--   0 sugimo-s   (501) staff       (20)     7265 2022-12-01 02:49:43.000000 eclsdk-1.2.1/ChangeLog
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10142 2022-01-05 05:27:16.000000 eclsdk-1.2.1/LICENSE
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1915 2022-12-01 02:49:45.322854 eclsdk-1.2.1/PKG-INFO
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1057 2022-01-05 05:27:16.000000 eclsdk-1.2.1/README.rst
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)       16 2022-01-05 05:27:16.000000 eclsdk-1.2.1/babel.cfg
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.258812 eclsdk-1.2.1/ecl/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      678 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.266291 eclsdk-1.2.1/ecl/baremetal/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      932 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/baremetal_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      199 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/exceptions.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.294294 eclsdk-1.2.1/ecl/baremetal/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    24235 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/baremetal/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2974 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/availability_zone.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2381 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/baremetal/v2/chassis.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3354 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/flavor.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1968 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/keypair.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2844 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/limits.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3146 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/metadata.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2632 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/nic_physical_port.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10791 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/baremetal/v2/server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1579 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/stock.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1914 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/v2/uefi.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1910 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/baremetal/version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.297628 eclsdk-1.2.1/ecl/block_store/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1022 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/block_store_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.320303 eclsdk-1.2.1/ecl/block_store/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    12501 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      580 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      791 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      492 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/limit.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1284 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/metadata.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      921 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1110 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/type.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5664 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/block_store/v2/volume.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.325111 eclsdk-1.2.1/ecl/compute/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      930 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/compute_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.356824 eclsdk-1.2.1/ecl/compute/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    35909 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2958 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1540 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2519 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/flavor.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2496 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/image.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2196 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/keypair.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4990 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/limits.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3458 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/metadata.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2929 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13700 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      901 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/server_action.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1464 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/server_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      705 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/server_volume.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1078 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/v2/volume.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1009 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/compute/version.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11511 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connection.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.362644 eclsdk-1.2.1/ecl/connectivity/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      455 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/connectivity_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      209 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/exceptions.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.374538 eclsdk-1.2.1/ecl/connectivity/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8257 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1611 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/v1/cic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1101 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/v1/mcic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      924 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/v1/operation.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      796 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/v1/server_segment.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      519 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/connectivity/version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.379839 eclsdk-1.2.1/ecl/dedicated_hypervisor/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      978 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/dedicated_hypervisor_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      203 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/exceptions.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.395499 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9361 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1652 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/license.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3115 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/license_type.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3985 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2619 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/usage.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)      610 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/vcf.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.401060 eclsdk-1.2.1/ecl/dns/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/__init__.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)      908 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/dns_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.415511 eclsdk-1.2.1/ecl/dns/v2/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/v2/__init__.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)    10726 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/v2/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1336 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/v2/name_server.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     7046 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/v2/recordset.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4929 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/dns/v2/zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4608 2022-11-30 06:07:56.000000 eclsdk-1.2.1/ecl/exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1621 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/format.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.421609 eclsdk-1.2.1/ecl/identity/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1149 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/identity_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.431259 eclsdk-1.2.1/ecl/identity/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9868 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2079 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v2/extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1319 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v2/role.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1449 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v2/tenant.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1423 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v2/user.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.456029 eclsdk-1.2.1/ecl/identity/v3/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    32977 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1655 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/credential.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1661 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/domain.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2092 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/endpoint.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1448 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/group.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1177 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/policy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1801 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/project.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1180 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/region.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1718 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2539 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/trust.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2627 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/v3/user.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1317 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/identity/version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.458532 eclsdk-1.2.1/ecl/image/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      919 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/image_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.482188 eclsdk-1.2.1/ecl/image/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13498 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10107 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/image.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2977 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/image_copy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1456 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/license.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2328 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/member.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6062 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/schema.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1218 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/image/v2/tag.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      989 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/module_loader.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.486733 eclsdk-1.2.1/ecl/mvna/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/__init__.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)      929 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/mvna_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.524744 eclsdk-1.2.1/ecl/mvna/v1/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/__init__.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)    47073 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2149 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/base.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1447 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/certificate.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2199 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/health_monitor.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1738 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/listener.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     3811 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/load_balancer.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1628 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/operation.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2291 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/plan.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2446 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/policy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1687 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/route.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1786 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/rule.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1447 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/system_update.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1570 2022-02-18 00:42:39.000000 eclsdk-1.2.1/ecl/mvna/v1/target_group.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1030 2022-12-01 02:11:17.000000 eclsdk-1.2.1/ecl/mvna/v1/tls_policy.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.532850 eclsdk-1.2.1/ecl/network/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      218 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      938 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/network_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.619946 eclsdk-1.2.1/ecl/network/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)   113679 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/network/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1738 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/aws.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1848 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/azure.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      704 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/base.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2206 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/colocation_logical_link.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2467 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/colocation_physical_link.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      818 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/colocation_space.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2831 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/common_function.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3440 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/common_function_gateway.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2617 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/common_function_pool.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2743 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4367 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/fic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4507 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/firewall.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1864 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/firewall_action.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2397 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/firewall_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3242 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/firewall_plan.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2570 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/gcp.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3955 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/gw_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6470 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/interdc.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5422 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/internet.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4499 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/load_balancer.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1923 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/load_balancer_action.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2386 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/load_balancer_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3435 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/load_balancer_plan.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2216 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/load_balancer_syslog_server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3525 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/network.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1196 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/physical_port.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4683 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/network/v2/port.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1271 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/publicip.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2976 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/qos_option.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2326 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/network/v2/quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      843 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/reserved_address.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1718 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/static_route.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4328 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/subnet.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1460 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/tenant_connection.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4367 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/v2/vpn.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      970 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/network/version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.625807 eclsdk-1.2.1/ecl/orchestration/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      989 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/orchestration_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.642356 eclsdk-1.2.1/ecl/orchestration/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14481 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2376 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2099 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/software_config.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2768 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/software_deployment.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6767 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/stack.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1902 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/v1/template.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1006 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/orchestration/version.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8873 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/profile.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.645755 eclsdk-1.2.1/ecl/provider_connectivity/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      223 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      524 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/provider_connectivity_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.664270 eclsdk-1.2.1/ecl/provider_connectivity/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19440 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     3699 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/address_assignment.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2039 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/aws_connection.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)      514 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/base.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      590 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/exchange_point.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1090 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/operation.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2432 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/tenant_connection.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2178 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v1/tenant_connection_request.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.684144 eclsdk-1.2.1/ecl/provider_connectivity/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    23989 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     3699 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/address_assignment.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2043 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/aws_connection.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)      513 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/base.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      664 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/exchange_point.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2053 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/gcp_connection.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1567 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/operation.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2432 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/tenant_connection.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2178 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/provider_connectivity/v2/tenant_connection_request.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13437 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14235 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/proxy2.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.691892 eclsdk-1.2.1/ecl/rca/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      205 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      899 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/rca_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.698035 eclsdk-1.2.1/ecl/rca/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5139 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3065 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/v1/user.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1835 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/rca/version.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    38820 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    33671 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/resource2.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.700575 eclsdk-1.2.1/ecl/security_order/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      436 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/security_order_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.714240 eclsdk-1.2.1/ecl/security_order/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19319 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/v2/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4323 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/v2/device.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4187 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/v2/ha_device.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4005 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/v2/host_based_security.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4346 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_order/v2/waf.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.716151 eclsdk-1.2.1/ecl/security_order_v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      429 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/security_order_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.731304 eclsdk-1.2.1/ecl/security_order_v1/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19331 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/v1/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4326 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/v1/device.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4190 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/v1/ha_device.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4008 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/v1/host_based_security.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4349 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_order_v1/v1/waf.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.734244 eclsdk-1.2.1/ecl/security_portal/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_portal/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      443 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_portal/security_portal_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.741608 eclsdk-1.2.1/ecl/security_portal/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_portal/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2144 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_portal/v2/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1600 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_portal/v2/security_device.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1796 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/security_portal/v2/security_device_interface.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.744399 eclsdk-1.2.1/ecl/security_portal_v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_portal_v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      432 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_portal_v1/security_portal_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.749974 eclsdk-1.2.1/ecl/security_portal_v1/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_portal_v1/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2162 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_portal_v1/v1/_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1603 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_portal_v1/v1/security_device.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1799 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/security_portal_v1/v1/security_device_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6056 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/service_filter.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14727 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/session.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.754401 eclsdk-1.2.1/ecl/sss/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      207 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      905 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/sss/sss_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.777983 eclsdk-1.2.1/ecl/sss/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    20176 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1408 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/api_key.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2043 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/channel.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5642 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/contract.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3642 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/iam_group.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1600 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/iam_role.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1745 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/role.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3070 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/tenant.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4843 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/sss/v1/user.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.785358 eclsdk-1.2.1/ecl/storage/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      230 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      894 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/storage_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.799475 eclsdk-1.2.1/ecl/storage/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14959 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3003 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/v1/availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3485 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/v1/snapshot.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2824 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/storage/v1/storage.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3778 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/storage/v1/volume.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2961 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/v1/volume_type.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2002 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/storage/version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.802848 eclsdk-1.2.1/ecl/telemetry/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      941 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/telemetry_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.825053 eclsdk-1.2.1/ecl/telemetry/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    12262 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3530 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/alarm.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1936 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/alarm_change.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1392 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/capability.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1599 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/meter.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1796 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2714 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/sample.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2697 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/telemetry/v2/statistics.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.826268 eclsdk-1.2.1/ecl/tests/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.829369 eclsdk-1.2.1/ecl/tests/functional/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.855314 eclsdk-1.2.1/ecl/tests/functional/baremetal/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      925 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_availability_zone.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     3880 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_chassis.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2067 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_flavor.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2396 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_keypair.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      835 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_limits.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2359 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_metadata.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1881 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_nic_ports.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3465 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1630 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_server_action.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      978 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_stock.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1728 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_uefi.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1222 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/baremetal/test_version.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2575 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/base.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.857446 eclsdk-1.2.1/ecl/tests/functional/block_store/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.873165 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      434 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      233 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      264 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_limit.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1156 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_metadata.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      866 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      906 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_type.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2872 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_volume.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.873829 eclsdk-1.2.1/ecl/tests/functional/compute/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.890223 eclsdk-1.2.1/ecl/tests/functional/compute/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      430 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      993 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2019 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_flavor.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3486 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_image.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1709 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_keypair.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1023 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_limits.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2323 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9512 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1257 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_volume.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.891164 eclsdk-1.2.1/ecl/tests/functional/connectivity/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.901813 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3071 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_cic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3347 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_eic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1879 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_mcic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1936 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_meic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3682 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_operation.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.906769 eclsdk-1.2.1/ecl/tests/functional/dns/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/dns/__init__.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2373 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/dns/test_recordset.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1528 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/dns/test_zone.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.907253 eclsdk-1.2.1/ecl/tests/functional/image/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.916847 eclsdk-1.2.1/ecl/tests/functional/image/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3338 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/test_image.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2584 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/test_image_copy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      728 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/test_license.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1955 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/test_member.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2929 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/test_schema.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      880 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/image/v2/test_tag.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.917375 eclsdk-1.2.1/ecl/tests/functional/network/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.968407 eclsdk-1.2.1/ecl/tests/functional/network/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      574 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2620 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1153 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall_action.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2230 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1831 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall_plan.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2050 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_gwif.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3543 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_interdc.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3162 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_internet.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2808 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1172 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer_action.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2141 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1899 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer_plan.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1559 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_network.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1828 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_port.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1646 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_publicip.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      687 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_qos_option.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1268 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_query_string.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      654 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1109 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_reserved_address.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1996 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_staticroute.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2341 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_subnet.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1663 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/network/v2/test_vpn.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.969628 eclsdk-1.2.1/ecl/tests/functional/orchestration/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/orchestration/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.975973 eclsdk-1.2.1/ecl/tests/functional/orchestration/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/orchestration/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1038 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/orchestration/v1/hello_world.yaml
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2772 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/orchestration/v1/test_stack.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.976518 eclsdk-1.2.1/ecl/tests/functional/rca/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/rca/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.980379 eclsdk-1.2.1/ecl/tests/functional/rca/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/rca/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1591 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/rca/v1/test_user.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1209 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/rca/v1/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.980859 eclsdk-1.2.1/ecl/tests/functional/sss/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.993864 eclsdk-1.2.1/ecl/tests/functional/sss/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1041 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_api_key.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      825 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_channel.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4226 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_contract.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1342 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_role.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1349 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_tenant.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3807 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_user.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:44.994908 eclsdk-1.2.1/ecl/tests/functional/storage/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.007697 eclsdk-1.2.1/ecl/tests/functional/storage/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1040 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_av_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      850 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_version.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3119 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_virtual_storage.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4839 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_volume.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1255 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_volume_type.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.008118 eclsdk-1.2.1/ecl/tests/functional/telemetry/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.020670 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1816 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_alarm.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1587 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_alarm_change.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1122 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_capability.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      909 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1521 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_sample.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1143 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_statistics.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.060365 eclsdk-1.2.1/ecl/tests/unit/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/__init__.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.065670 eclsdk-1.2.1/ecl/tests/unit/baremetal/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1106 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/test_baremetal_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1499 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.079551 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1442 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_availability_zone.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     4131 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_charssis.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2219 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_flavor.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1565 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_keypair.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4616 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_limits.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2126 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_uefi.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1919 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/base.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.081630 eclsdk-1.2.1/ecl/tests/unit/block_store/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1106 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/test_block_store_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.091451 eclsdk-1.2.1/ecl/tests/unit/block_store/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2252 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2886 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_snapshot.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1624 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_type.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4341 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_volume.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.096615 eclsdk-1.2.1/ecl/tests/unit/compute/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1087 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/test_compute_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1531 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.125881 eclsdk-1.2.1/ecl/tests/unit/compute/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1749 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1754 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3082 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_flavor.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3489 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_image.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1554 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_keypair.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10418 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_limits.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3098 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_metadata.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9857 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11893 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_server.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1961 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_server_interface.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2375 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_volume.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.129911 eclsdk-1.2.1/ecl/tests/unit/connectivity/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      601 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/test_connectivity_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1025 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.137696 eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1624 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/test_cic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1768 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/test_mcic.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      560 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1259 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/fakes.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.143088 eclsdk-1.2.1/ecl/tests/unit/identity/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1488 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/test_identity_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2248 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.153222 eclsdk-1.2.1/ecl/tests/unit/identity/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2381 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2989 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1556 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_role.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1519 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_tenant.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1483 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_user.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.178413 eclsdk-1.2.1/ecl/tests/unit/identity/v3/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1645 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_credential.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1526 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_domain.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1706 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_endpoint.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1540 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_group.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1446 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_policy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1619 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_project.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8702 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1510 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_region.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1604 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1968 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_trust.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1881 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_user.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.181146 eclsdk-1.2.1/ecl/tests/unit/image/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/image/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1075 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/image/test_image_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.189885 eclsdk-1.2.1/ecl/tests/unit/image/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/image/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4430 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/image/v2/test_image.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1750 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/image/v2/test_member.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3811 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/image/v2/test_proxy.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.195329 eclsdk-1.2.1/ecl/tests/unit/network/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1089 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/test_network_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1447 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.216198 eclsdk-1.2.1/ecl/tests/unit/network/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1937 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_extension.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3642 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_load_balancer.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2136 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_network.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2755 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_port.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5451 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3841 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_quota.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2608 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_subnet.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1588 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/network/v2/test_vpn_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.220385 eclsdk-1.2.1/ecl/tests/unit/orchestration/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1172 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/test_orchestration_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1465 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.236139 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6948 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2451 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2034 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_software_config.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2442 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_software_deployment.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5422 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_stack.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3557 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_template.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.239725 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      648 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/test_provider_connectivity_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.248110 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/
--rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/__init__.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1480 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_address_assignment.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3778 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_proxy.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2912 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection.py
--rw-r--r--   0 sugimo-s   (501) staff       (20)     2429 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection_request.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.250682 eclsdk-1.2.1/ecl/tests/unit/sss/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1063 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/test_sss_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.263193 eclsdk-1.2.1/ecl/tests/unit/sss/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1654 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_api_key.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1960 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_channel.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3798 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_contract.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1819 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_role.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1774 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_tenant.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2891 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_user.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.267894 eclsdk-1.2.1/ecl/tests/unit/storage/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1089 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/test_storage_service.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1669 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/test_version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.278843 eclsdk-1.2.1/ecl/tests/unit/storage/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1690 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_availability_zone.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2857 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_snapshot.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3120 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_storage.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3578 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_volume.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2002 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_volume_type.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.280881 eclsdk-1.2.1/ecl/tests/unit/telemetry/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1098 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/test_telemetry_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.301763 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4137 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_alarm.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2900 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_alarm_change.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2494 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_capability.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1920 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_meter.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4060 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2262 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5344 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_sample.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3087 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_statistics.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8380 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_connection.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2046 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_exceptions.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1746 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_format.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4703 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_profile.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11767 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13714 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_proxy2.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10333 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_proxy_base.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10512 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_proxy_base2.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    53237 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_resource.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    48848 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_resource2.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1629 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_service_filter.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8190 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_session.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3139 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/tests/unit/test_utils.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2858 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/utils.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      634 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/version.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.307800 eclsdk-1.2.1/ecl/virtual_network_appliance/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1068 2022-11-30 06:07:57.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/exceptions.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.318313 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/__init__.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13177 2022-04-01 05:36:24.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/_proxy.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      720 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/base.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4591 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/operation.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5230 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/virtual_network_appliance.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1797 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/v1/virtual_network_appliance_plan.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      484 2022-01-05 05:27:16.000000 eclsdk-1.2.1/ecl/virtual_network_appliance/virtual_network_appliance_service.py
-drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-12-01 02:49:45.322470 eclsdk-1.2.1/eclsdk.egg-info/
--rw-r--r--   0 sugimo-s   (501) staff       (20)     1915 2022-12-01 02:49:43.000000 eclsdk-1.2.1/eclsdk.egg-info/PKG-INFO
--rw-r--r--   0 sugimo-s   (501) staff       (20)    20216 2022-12-01 02:49:44.000000 eclsdk-1.2.1/eclsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sugimo-s   (501) staff       (20)        1 2022-12-01 02:49:43.000000 eclsdk-1.2.1/eclsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sugimo-s   (501) staff       (20)        1 2022-02-18 04:36:41.000000 eclsdk-1.2.1/eclsdk.egg-info/not-zip-safe
--rw-r--r--   0 sugimo-s   (501) staff       (20)       46 2022-12-01 02:49:43.000000 eclsdk-1.2.1/eclsdk.egg-info/pbr.json
--rw-r--r--   0 sugimo-s   (501) staff       (20)      123 2022-12-01 02:49:43.000000 eclsdk-1.2.1/eclsdk.egg-info/requires.txt
--rw-r--r--   0 sugimo-s   (501) staff       (20)        4 2022-12-01 02:49:43.000000 eclsdk-1.2.1/eclsdk.egg-info/top_level.txt
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      404 2022-01-05 05:27:16.000000 eclsdk-1.2.1/requirements.txt
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      821 2022-12-01 02:49:45.323533 eclsdk-1.2.1/setup.cfg
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1028 2022-01-05 05:27:16.000000 eclsdk-1.2.1/setup.py
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)      648 2022-01-05 05:27:16.000000 eclsdk-1.2.1/test-requirements.txt
--rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1094 2022-01-05 05:27:16.000000 eclsdk-1.2.1/tox.ini
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.698466 eclsdk-1.3.0/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1646 2024-04-16 05:37:33.000000 eclsdk-1.3.0/AUTHORS
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     7299 2024-04-16 05:37:33.000000 eclsdk-1.3.0/ChangeLog
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10142 2022-01-05 05:27:16.000000 eclsdk-1.3.0/LICENSE
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1935 2024-04-16 05:37:35.698570 eclsdk-1.3.0/PKG-INFO
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1057 2022-01-05 05:27:16.000000 eclsdk-1.3.0/README.rst
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)       16 2022-01-05 05:27:16.000000 eclsdk-1.3.0/babel.cfg
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.158380 eclsdk-1.3.0/ecl/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      678 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.166699 eclsdk-1.3.0/ecl/baremetal/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      932 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/baremetal_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      199 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/exceptions.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.206259 eclsdk-1.3.0/ecl/baremetal/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    24676 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/baremetal/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2974 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/availability_zone.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2381 2022-04-01 05:36:24.000000 eclsdk-1.3.0/ecl/baremetal/v2/chassis.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3354 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/flavor.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1968 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/keypair.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2844 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/limits.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3146 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/metadata.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2632 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/nic_physical_port.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11176 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/baremetal/v2/server.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1579 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/stock.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1914 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/v2/uefi.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1910 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/baremetal/version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.209084 eclsdk-1.3.0/ecl/block_store/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1022 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/block_store_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.233071 eclsdk-1.3.0/ecl/block_store/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    12501 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      580 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      791 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      492 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/limit.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1284 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/metadata.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      921 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1110 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/type.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5664 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/block_store/v2/volume.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.238254 eclsdk-1.3.0/ecl/compute/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      930 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/compute_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.278794 eclsdk-1.3.0/ecl/compute/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    35909 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2958 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1540 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2519 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/flavor.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2496 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/image.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2196 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/keypair.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4990 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/limits.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3458 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/metadata.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2929 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13700 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/server.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      901 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/server_action.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1464 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/server_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      705 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/server_volume.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1078 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/v2/volume.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1009 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/compute/version.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11511 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connection.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.284812 eclsdk-1.3.0/ecl/connectivity/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      455 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/connectivity_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      209 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/exceptions.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.299255 eclsdk-1.3.0/ecl/connectivity/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8257 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/v1/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1611 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/v1/cic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1101 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/v1/mcic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      924 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/v1/operation.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      796 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/v1/server_segment.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      519 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/connectivity/version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.303948 eclsdk-1.3.0/ecl/dedicated_hypervisor/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      978 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/dedicated_hypervisor_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      203 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/exceptions.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.322570 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10766 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1652 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/license.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3115 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/license_type.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5598 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/server.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2619 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/usage.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)      610 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/vcf.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.325609 eclsdk-1.3.0/ecl/dns/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)      908 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/dns_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.338172 eclsdk-1.3.0/ecl/dns/v2/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/v2/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)    10726 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/v2/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1336 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/v2/name_server.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     7046 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/v2/recordset.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4929 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/dns/v2/zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4608 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1621 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/format.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.344622 eclsdk-1.3.0/ecl/identity/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1149 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/identity_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.361708 eclsdk-1.3.0/ecl/identity/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9868 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2079 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v2/extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1319 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v2/role.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1449 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v2/tenant.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1423 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v2/user.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.396197 eclsdk-1.3.0/ecl/identity/v3/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    32977 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1655 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/credential.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1661 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/domain.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2092 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/endpoint.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1448 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/group.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1177 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/policy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1801 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/project.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1180 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/region.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1718 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2539 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/trust.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2627 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/v3/user.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1317 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/identity/version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.399295 eclsdk-1.3.0/ecl/image/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      919 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/image_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.423476 eclsdk-1.3.0/ecl/image/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13498 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10107 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/image.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2977 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/image_copy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1456 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/license.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2328 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/member.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6062 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/schema.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1218 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/image/v2/tag.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      989 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/module_loader.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.427029 eclsdk-1.3.0/ecl/mvna/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)      929 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/mvna_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.474578 eclsdk-1.3.0/ecl/mvna/v1/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)    47565 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/mvna/v1/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2149 2022-12-01 02:11:17.000000 eclsdk-1.3.0/ecl/mvna/v1/base.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1447 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/certificate.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2199 2022-12-01 02:11:17.000000 eclsdk-1.3.0/ecl/mvna/v1/health_monitor.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1738 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/listener.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     3811 2022-12-01 02:11:17.000000 eclsdk-1.3.0/ecl/mvna/v1/load_balancer.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1628 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/operation.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2291 2022-12-01 02:11:17.000000 eclsdk-1.3.0/ecl/mvna/v1/plan.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2550 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/mvna/v1/policy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1687 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/route.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1786 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/rule.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1447 2022-12-01 02:11:17.000000 eclsdk-1.3.0/ecl/mvna/v1/system_update.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1570 2022-02-18 00:42:39.000000 eclsdk-1.3.0/ecl/mvna/v1/target_group.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1030 2022-12-01 02:11:17.000000 eclsdk-1.3.0/ecl/mvna/v1/tls_policy.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.481886 eclsdk-1.3.0/ecl/network/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      218 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      938 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/network_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.604745 eclsdk-1.3.0/ecl/network/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)   116940 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/network/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1738 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/aws.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1848 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/azure.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      704 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/base.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2206 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/colocation_logical_link.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2467 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/colocation_physical_link.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      818 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/colocation_space.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2831 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/common_function.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3440 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/common_function_gateway.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2617 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/common_function_pool.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2743 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4367 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/fic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4507 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/firewall.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1864 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/firewall_action.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2397 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/firewall_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3242 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/firewall_plan.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2570 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/gcp.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4020 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/network/v2/gw_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6470 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/interdc.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5422 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/internet.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4499 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/load_balancer.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1923 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/load_balancer_action.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2386 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/load_balancer_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3435 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/load_balancer_plan.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2216 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/load_balancer_syslog_server.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4218 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/network/v2/mec.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3525 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/network.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1196 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/physical_port.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4683 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/network/v2/port.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1271 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/publicip.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3056 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/network/v2/qos_option.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2453 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/network/v2/quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      843 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/reserved_address.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1783 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/network/v2/static_route.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4328 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/subnet.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1460 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/tenant_connection.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4367 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/v2/vpn.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      970 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/network/version.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8681 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/profile.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.610849 eclsdk-1.3.0/ecl/provider_connectivity/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      223 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      524 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/provider_connectivity_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.636346 eclsdk-1.3.0/ecl/provider_connectivity/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19440 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     3699 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/address_assignment.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2039 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/aws_connection.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)      514 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/base.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      590 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/exchange_point.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1090 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/operation.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2432 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/tenant_connection.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2178 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v1/tenant_connection_request.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.663993 eclsdk-1.3.0/ecl/provider_connectivity/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    23989 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     3699 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/address_assignment.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2043 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/aws_connection.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)      513 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/base.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      664 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/exchange_point.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2053 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/gcp_connection.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1567 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/operation.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2432 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/tenant_connection.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2178 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/provider_connectivity/v2/tenant_connection_request.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13437 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14235 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/proxy2.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.673082 eclsdk-1.3.0/ecl/rca/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      205 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      899 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/rca_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.681055 eclsdk-1.3.0/ecl/rca/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5139 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/v1/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3065 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/v1/user.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1835 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/rca/version.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    38820 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/resource.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    33671 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/resource2.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.684192 eclsdk-1.3.0/ecl/security_order/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/security_order/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      439 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/security_order_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.703776 eclsdk-1.3.0/ecl/security_order/v3/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/v3/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19319 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/v3/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4323 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/v3/device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4187 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/v3/ha_device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4005 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/v3/host_based_security.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4346 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order/v3/waf.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.707128 eclsdk-1.3.0/ecl/security_order_v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      429 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/security_order_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.728012 eclsdk-1.3.0/ecl/security_order_v1/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19331 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/v1/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4326 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/v1/device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4190 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/v1/ha_device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4008 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/v1/host_based_security.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4349 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_order_v1/v1/waf.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.731823 eclsdk-1.3.0/ecl/security_order_v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      436 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/security_order_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.749559 eclsdk-1.3.0/ecl/security_order_v2/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    19331 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/v2/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4326 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/v2/device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4190 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/v2/ha_device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4008 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/v2/host_based_security.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4349 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_order_v2/v2/waf.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.753124 eclsdk-1.3.0/ecl/security_portal/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/security_portal/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      446 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal/security_portal_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.764359 eclsdk-1.3.0/ecl/security_portal/v3/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal/v3/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2010 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal/v3/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1545 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal/v3/security_device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1741 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal/v3/security_device_interface.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.767794 eclsdk-1.3.0/ecl/security_portal_v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_portal_v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      432 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_portal_v1/security_portal_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.777286 eclsdk-1.3.0/ecl/security_portal_v1/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_portal_v1/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2162 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_portal_v1/v1/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1603 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_portal_v1/v1/security_device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1799 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/security_portal_v1/v1/security_device_interface.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.781392 eclsdk-1.3.0/ecl/security_portal_v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal_v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      443 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal_v2/security_portal_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.797300 eclsdk-1.3.0/ecl/security_portal_v2/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal_v2/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2150 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal_v2/v2/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1603 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal_v2/v2/security_device.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1799 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/security_portal_v2/v2/security_device_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     6056 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/service_filter.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14727 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/session.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.808900 eclsdk-1.3.0/ecl/sss/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      207 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1135 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/sss/sss_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.886052 eclsdk-1.3.0/ecl/sss/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    20176 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1408 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/api_key.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2043 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/channel.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5642 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/contract.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3642 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/iam_group.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1600 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/iam_role.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1745 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/role.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3070 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/tenant.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4843 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/sss/v1/user.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.898997 eclsdk-1.3.0/ecl/sss/v2/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)    23507 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/sss/v2/_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1352 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/sss/v2/service_menu.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2631 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/sss/v2/token.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.909749 eclsdk-1.3.0/ecl/storage/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      230 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      894 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/storage_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.934006 eclsdk-1.3.0/ecl/storage/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    14959 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/v1/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3003 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/v1/availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3485 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/v1/snapshot.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2824 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/storage/v1/storage.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3778 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/storage/v1/volume.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2961 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/v1/volume_type.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2002 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/storage/version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.937806 eclsdk-1.3.0/ecl/telemetry/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      941 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/telemetry_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.965762 eclsdk-1.3.0/ecl/telemetry/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    12262 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3530 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/alarm.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1936 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/alarm_change.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1392 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/capability.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1599 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/meter.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1796 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/resource.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2714 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/sample.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2697 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/telemetry/v2/statistics.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.966825 eclsdk-1.3.0/ecl/tests/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:34.971745 eclsdk-1.3.0/ecl/tests/functional/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.016005 eclsdk-1.3.0/ecl/tests/functional/baremetal/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      925 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_availability_zone.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     3880 2022-04-01 05:36:24.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_chassis.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2067 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_flavor.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2396 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_keypair.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      835 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_limits.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2359 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_metadata.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1881 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_nic_ports.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3465 2022-04-01 05:36:24.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_server.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1630 2024-04-15 02:08:27.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_server_action.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      978 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_stock.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1728 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_uefi.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1222 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/baremetal/test_version.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2575 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/base.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.017199 eclsdk-1.3.0/ecl/tests/functional/block_store/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.036475 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      434 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      233 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      264 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_limit.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1156 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_metadata.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      866 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      906 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_type.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2872 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_volume.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.037503 eclsdk-1.3.0/ecl/tests/functional/compute/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.065103 eclsdk-1.3.0/ecl/tests/functional/compute/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      430 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      993 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2019 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_flavor.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3486 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_image.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1709 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_keypair.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1023 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_limits.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2323 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9512 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_server.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1257 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_volume.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.065563 eclsdk-1.3.0/ecl/tests/functional/connectivity/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.082833 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3071 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_cic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3347 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_eic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1879 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_mcic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1936 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_meic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3682 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_operation.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.089897 eclsdk-1.3.0/ecl/tests/functional/dns/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/dns/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2373 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/dns/test_recordset.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1528 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/dns/test_zone.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.091289 eclsdk-1.3.0/ecl/tests/functional/image/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.108562 eclsdk-1.3.0/ecl/tests/functional/image/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3338 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/test_image.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2584 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/test_image_copy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      728 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/test_license.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1955 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/test_member.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2929 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/test_schema.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      880 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/image/v2/test_tag.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.109114 eclsdk-1.3.0/ecl/tests/functional/network/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.178337 eclsdk-1.3.0/ecl/tests/functional/network/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      574 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2620 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1153 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall_action.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2230 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1831 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall_plan.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2050 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_gwif.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3543 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_interdc.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3162 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_internet.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2808 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1172 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer_action.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2141 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1899 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer_plan.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1559 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_network.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1828 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_port.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1646 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_publicip.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      687 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_qos_option.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1268 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_query_string.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      654 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1109 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_reserved_address.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1996 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_staticroute.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2341 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_subnet.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1663 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/network/v2/test_vpn.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.179331 eclsdk-1.3.0/ecl/tests/functional/rca/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/rca/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.187426 eclsdk-1.3.0/ecl/tests/functional/rca/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/rca/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1591 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/rca/v1/test_user.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1209 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/rca/v1/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.188350 eclsdk-1.3.0/ecl/tests/functional/sss/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.206049 eclsdk-1.3.0/ecl/tests/functional/sss/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1041 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_api_key.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      825 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_channel.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4226 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_contract.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1342 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_role.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1349 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_tenant.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3807 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_user.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.214296 eclsdk-1.3.0/ecl/tests/functional/sss/v2/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v2/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     3456 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v2/test_service_menu.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     3093 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/functional/sss/v2/test_token.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.215256 eclsdk-1.3.0/ecl/tests/functional/storage/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.231596 eclsdk-1.3.0/ecl/tests/functional/storage/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1040 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_av_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      850 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_version.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3119 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_virtual_storage.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4839 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_volume.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1255 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_volume_type.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.232013 eclsdk-1.3.0/ecl/tests/functional/telemetry/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.252234 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1816 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_alarm.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1587 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_alarm_change.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1122 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_capability.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      909 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_resource.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1521 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_sample.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1143 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_statistics.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.305750 eclsdk-1.3.0/ecl/tests/unit/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/__init__.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.313058 eclsdk-1.3.0/ecl/tests/unit/baremetal/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1106 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/test_baremetal_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1499 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.338364 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1442 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_availability_zone.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     4131 2022-04-01 05:36:24.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_charssis.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2219 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_flavor.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1565 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_keypair.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4616 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_limits.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2126 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_uefi.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1919 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/base.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.343411 eclsdk-1.3.0/ecl/tests/unit/block_store/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1106 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/test_block_store_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.358222 eclsdk-1.3.0/ecl/tests/unit/block_store/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2252 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2886 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_snapshot.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1624 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_type.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4341 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_volume.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.365676 eclsdk-1.3.0/ecl/tests/unit/compute/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1087 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/test_compute_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1531 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.405524 eclsdk-1.3.0/ecl/tests/unit/compute/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1749 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1754 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3082 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_flavor.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3489 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_image.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1554 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_keypair.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10418 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_limits.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3098 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_metadata.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     9857 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11893 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_server.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1961 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_server_interface.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2375 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_volume.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.411833 eclsdk-1.3.0/ecl/tests/unit/connectivity/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      601 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/test_connectivity_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1025 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.422470 eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1624 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/test_cic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1768 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/test_mcic.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      560 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1259 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/fakes.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.430953 eclsdk-1.3.0/ecl/tests/unit/identity/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1488 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/test_identity_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2248 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.446215 eclsdk-1.3.0/ecl/tests/unit/identity/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2381 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2989 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1556 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_role.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1519 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_tenant.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1483 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_user.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.485377 eclsdk-1.3.0/ecl/tests/unit/identity/v3/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1645 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_credential.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1526 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_domain.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1706 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_endpoint.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1540 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_group.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1446 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_policy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1619 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_project.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8702 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1510 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_region.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1604 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1968 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_trust.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1881 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_user.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.490062 eclsdk-1.3.0/ecl/tests/unit/image/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/image/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1075 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/image/test_image_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.502087 eclsdk-1.3.0/ecl/tests/unit/image/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/image/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4430 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/image/v2/test_image.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1750 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/image/v2/test_member.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3811 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/image/v2/test_proxy.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.508827 eclsdk-1.3.0/ecl/tests/unit/network/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1089 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/test_network_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1447 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.548751 eclsdk-1.3.0/ecl/tests/unit/network/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1937 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_extension.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3642 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_load_balancer.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1765 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_mec_gateway.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2064 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_mec_interface.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1537 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_mec_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2136 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_network.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2755 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_port.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5451 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4330 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_quota.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2608 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_subnet.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1588 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/network/v2/test_vpn_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.552307 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      648 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/test_provider_connectivity_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.566252 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1480 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_address_assignment.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3778 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_proxy.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2912 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2429 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection_request.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.569152 eclsdk-1.3.0/ecl/tests/unit/sss/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1543 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/sss/test_sss_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.589736 eclsdk-1.3.0/ecl/tests/unit/sss/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1654 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_api_key.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1960 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_channel.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3798 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_contract.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1819 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_role.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1774 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_tenant.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2891 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_user.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.597340 eclsdk-1.3.0/ecl/tests/unit/sss/v2/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v2/__init__.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2472 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v2/test_service_menu.py
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     2644 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/sss/v2/test_token.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.603981 eclsdk-1.3.0/ecl/tests/unit/storage/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1089 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/test_storage_service.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1669 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/test_version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.622308 eclsdk-1.3.0/ecl/tests/unit/storage/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1690 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_availability_zone.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2857 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_snapshot.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3120 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_storage.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3578 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_volume.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2002 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_volume_type.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.625979 eclsdk-1.3.0/ecl/tests/unit/telemetry/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1098 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/test_telemetry_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.656494 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4137 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_alarm.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2900 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_alarm_change.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2494 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_capability.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1920 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_meter.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4060 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2262 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_resource.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5344 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_sample.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3087 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_statistics.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8258 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/test_connection.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2046 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_exceptions.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1746 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_format.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4480 2024-04-16 05:11:03.000000 eclsdk-1.3.0/ecl/tests/unit/test_profile.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    11767 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13714 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_proxy2.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10333 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_proxy_base.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    10512 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_proxy_base2.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    53237 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_resource.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    48848 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_resource2.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1629 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_service_filter.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     8190 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_session.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     3139 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/tests/unit/test_utils.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     2858 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/utils.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      634 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/version.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.664314 eclsdk-1.3.0/ecl/virtual_network_appliance/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1068 2024-04-15 02:10:08.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/exceptions.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.682506 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/__init__.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)    13177 2022-04-01 05:36:24.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/_proxy.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      720 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/base.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     4591 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/operation.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     5230 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/virtual_network_appliance.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1797 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/v1/virtual_network_appliance_plan.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      484 2022-01-05 05:27:16.000000 eclsdk-1.3.0/ecl/virtual_network_appliance/virtual_network_appliance_service.py
+drwxr-xr-x   0 sugimo-s   (501) staff       (20)        0 2024-04-16 05:37:35.698127 eclsdk-1.3.0/eclsdk.egg-info/
+-rw-r--r--   0 sugimo-s   (501) staff       (20)     1935 2024-04-16 05:37:33.000000 eclsdk-1.3.0/eclsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sugimo-s   (501) staff       (20)    20211 2024-04-16 05:37:33.000000 eclsdk-1.3.0/eclsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        1 2024-04-16 05:37:33.000000 eclsdk-1.3.0/eclsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        1 2022-02-18 04:36:41.000000 eclsdk-1.3.0/eclsdk.egg-info/not-zip-safe
+-rw-r--r--   0 sugimo-s   (501) staff       (20)       46 2024-04-16 05:37:33.000000 eclsdk-1.3.0/eclsdk.egg-info/pbr.json
+-rw-r--r--   0 sugimo-s   (501) staff       (20)      123 2024-04-16 05:37:33.000000 eclsdk-1.3.0/eclsdk.egg-info/requires.txt
+-rw-r--r--   0 sugimo-s   (501) staff       (20)        4 2024-04-16 05:37:33.000000 eclsdk-1.3.0/eclsdk.egg-info/top_level.txt
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      404 2022-01-05 05:27:16.000000 eclsdk-1.3.0/requirements.txt
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      821 2024-04-16 05:37:35.699995 eclsdk-1.3.0/setup.cfg
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1028 2022-01-05 05:27:16.000000 eclsdk-1.3.0/setup.py
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)      648 2022-01-05 05:27:16.000000 eclsdk-1.3.0/test-requirements.txt
+-rwxr-xr-x   0 sugimo-s   (501) staff       (20)     1094 2022-01-05 05:27:16.000000 eclsdk-1.3.0/tox.ini
```

### Comparing `eclsdk-1.2.1/AUTHORS` & `eclsdk-1.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ChangeLog` & `eclsdk-1.3.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+1.3.0
+-----
+
+* Rel/v1.3.0 (#144)
+
 1.2.1
 -----
 
 * :bookmark: IF-9049 version up (#129)
 * Add mvna get staged method (#127) (#128)
 
 1.2.0
```

### Comparing `eclsdk-1.2.1/LICENSE` & `eclsdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/PKG-INFO` & `eclsdk-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: eclsdk
-Version: 1.2.1
+Version: 1.3.0
 Summary: SDK for building applications to work with Enterprise Cloud 2.0
 Home-page: https://ecl.ntt.com
 Author: NTT Communications
 Author-email: ecl-cli-sdk@ntt.com
 License: Apache License, Version 2.0
+Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -68,7 +69,9 @@
 https://ecl.ntt.com
 
 License
 -------
 
 Apache 2.0
 
+
+
```

### Comparing `eclsdk-1.2.1/README.rst` & `eclsdk-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/__init__.py` & `eclsdk-1.3.0/ecl/__init__.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/baremetal_service.py` & `eclsdk-1.3.0/ecl/baremetal/baremetal_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/_proxy.py` & `eclsdk-1.3.0/ecl/baremetal/v2/_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,14 +452,25 @@
 
         :param string server_id: ID for the server.
         :return: :class:`~ecl.baremetal.v2.server.ServerAction`
         """
         server = _server.ServerAction()
         return server.get_management_console(self.session, server_id)
 
+    def reset_bmc(self, server_id, type):
+        """Reset the Baseboard Management Controller.
+        This request will be accepted only when the task_state is None.
+
+        :param string server_id: ID for the server.
+        :param string type: BMC reset mode.Supported values are WARM and COLD.
+        :return: ``None``
+        """
+        server = _server.ServerAction()
+        return server.reset_bmc(self.session, server_id, type)
+
     def metadata(self, server_id):
         """This API lists metadata for a specified server.
 
         :param string server_id: ID for specified server.
         :return: A list of :class:`~ecl.baremetal.v2.metadata.Metadata`
         """
         metadata = _metadata.Metadata()
@@ -547,15 +558,15 @@
         """
         chassis = _chassis.ChassisDetail if details else _chassis.Chassis
         return list(self._list(chassis))
 
     def get_chassis(self, chassis_id):
         """Gets details for a ChassisDetail associated with chassis_id.
 
-        A chassis represents base object of baremetal server. 
+        A chassis represents base object of baremetal server.
         Each chassis is assigned an unique id and has dedicated disk spaces, 
         memory capacities and cpu resources. You can create baremetal server 
         upon this object.
 
         :param string chassis_id: ID for the chassis.
         :return: :class:`~ecl.baremetal.v2.chassis.Chassis`
         """
```

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/availability_zone.py` & `eclsdk-1.3.0/ecl/baremetal/v2/availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/chassis.py` & `eclsdk-1.3.0/ecl/baremetal/v2/chassis.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/flavor.py` & `eclsdk-1.3.0/ecl/baremetal/v2/flavor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/keypair.py` & `eclsdk-1.3.0/ecl/baremetal/v2/keypair.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/limits.py` & `eclsdk-1.3.0/ecl/baremetal/v2/limits.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/metadata.py` & `eclsdk-1.3.0/ecl/baremetal/v2/metadata.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/nic_physical_port.py` & `eclsdk-1.3.0/ecl/baremetal/v2/nic_physical_port.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/server.py` & `eclsdk-1.3.0/ecl/baremetal/v2/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -250,14 +250,29 @@
             endpoint_filter=self.service,
             json=body,
             headers={"Accept": "application/json"}
         )
         self._translate_response(resp, has_body=True)
         return self
 
+    def reset_bmc(self, session, server_id, type):
+        uri = self.base_path % server_id
+        body = {
+            "bmc-reset": {
+                "type": type
+            }
+        }
+        resp = session.post(
+            uri,
+            endpoint_filter=self.service,
+            json=body
+        )
+        self._translate_response(resp, has_body=False)
+        return self
+
     @classmethod
     def find(cls, session, name_or_id, ignore_missing=False, **params):
         """Find a resource by its name or id.
 
         :param session: The session to use for making this request.
         :type session: :class:`~ecl.session.Session`
         :param name_or_id: This resource's identifier, if needed by
```

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/stock.py` & `eclsdk-1.3.0/ecl/baremetal/v2/stock.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/v2/uefi.py` & `eclsdk-1.3.0/ecl/baremetal/v2/uefi.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/baremetal/version.py` & `eclsdk-1.3.0/ecl/baremetal/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/block_store_service.py` & `eclsdk-1.3.0/ecl/block_store/block_store_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/_proxy.py` & `eclsdk-1.3.0/ecl/block_store/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/availability_zone.py` & `eclsdk-1.3.0/ecl/block_store/v2/availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/extension.py` & `eclsdk-1.3.0/ecl/block_store/v2/extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/metadata.py` & `eclsdk-1.3.0/ecl/block_store/v2/metadata.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/quota.py` & `eclsdk-1.3.0/ecl/block_store/v2/quota.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/type.py` & `eclsdk-1.3.0/ecl/block_store/v2/type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/block_store/v2/volume.py` & `eclsdk-1.3.0/ecl/block_store/v2/volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/compute_service.py` & `eclsdk-1.3.0/ecl/compute/compute_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/_proxy.py` & `eclsdk-1.3.0/ecl/compute/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/availability_zone.py` & `eclsdk-1.3.0/ecl/compute/v2/availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/extension.py` & `eclsdk-1.3.0/ecl/compute/v2/extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/flavor.py` & `eclsdk-1.3.0/ecl/compute/v2/flavor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/image.py` & `eclsdk-1.3.0/ecl/compute/v2/image.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/keypair.py` & `eclsdk-1.3.0/ecl/compute/v2/keypair.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/limits.py` & `eclsdk-1.3.0/ecl/compute/v2/limits.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/metadata.py` & `eclsdk-1.3.0/ecl/compute/v2/metadata.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/quota.py` & `eclsdk-1.3.0/ecl/compute/v2/quota.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/server.py` & `eclsdk-1.3.0/ecl/compute/v2/server.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/server_action.py` & `eclsdk-1.3.0/ecl/compute/v2/server_action.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/server_interface.py` & `eclsdk-1.3.0/ecl/compute/v2/server_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/server_volume.py` & `eclsdk-1.3.0/ecl/compute/v2/server_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/v2/volume.py` & `eclsdk-1.3.0/ecl/compute/v2/volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/compute/version.py` & `eclsdk-1.3.0/ecl/compute/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connection.py` & `eclsdk-1.3.0/ecl/connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connectivity/v1/_proxy.py` & `eclsdk-1.3.0/ecl/connectivity/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connectivity/v1/cic.py` & `eclsdk-1.3.0/ecl/connectivity/v1/cic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connectivity/v1/mcic.py` & `eclsdk-1.3.0/ecl/connectivity/v1/mcic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connectivity/v1/operation.py` & `eclsdk-1.3.0/ecl/connectivity/v1/operation.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connectivity/v1/server_segment.py` & `eclsdk-1.3.0/ecl/connectivity/v1/server_segment.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/connectivity/version.py` & `eclsdk-1.3.0/ecl/connectivity/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/dedicated_hypervisor_service.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/dedicated_hypervisor_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/_proxy.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/_proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,14 +82,27 @@
             body["description"] = description
         if availability_zone:
             body["availability_zone"] = availability_zone
         if metadata:
             body["metadata"] = metadata
         return self._create(_server.Server, **body)
 
+    def update_server(self, server_id, name):
+        """
+        Updates the editable attributes of the specified baremetal server.
+
+        :param string server_id: ID for the server.
+        :param string name: Name of your Dedicated Hypervisor/Baremetal server
+            as a string.
+        :return: The results of server update.
+        :rtype: :class:`~ecl.dedicated_hypervisor.v1.server.Server`
+        """
+        body = {"name": name}
+        return self._update(_server.Server, server_id, **body)
+
     def delete_server(self, server_id, ignore_missing=False):
         """
         Deletes a specified Dedicated Hypervisor server.
         You can delete server when specified server status is
         ACTIVE or ERROR status.
 
         :param string server_id: ID for the server.
@@ -223,7 +236,31 @@
 
     def sddcs(self, **query):
         return list(self._list(_vcf.Sddc, **query))
 
 
     def delete_sddc(self, sddc_id, ignore_missing=False):
         return self._delete(_vcf.Sddc, sddc_id, ignore_missing=ignore_missing)
+
+    def get_cfgw_connection(self, server_id):
+        """
+        Shows the connection status between your Dedicated Hypervisor and
+        common function gateway network.
+
+        :param string server_id: ID for the server.
+        :return: One :class:`~ecl.dedicated_hypervisor.v1.server.CFGWConnection`
+        instance.
+        """
+        cfgw = _server.CFGWConnection()
+        return cfgw.get_cfgw_connection(self.session, server_id)
+
+    def update_cfgw_connection(self, server_id):
+        """
+        Updates the connection status between your Dedicated Hypervisor and
+        common function gateway network.
+
+        :param string server_id: ID for the server.
+        :return: One :class:`~ecl.dedicated_hypervisor.v1.server.CFGWConnection`
+        instance.
+        """
+        cfgw = _server.CFGWConnection()
+        return cfgw.update_cfgw_connection(self.session, server_id)
```

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/license.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/license.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/license_type.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/license_type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/server.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     base_path = '/servers'
     service = dedicated_hypervisor_service.DedicatedHypervisorService()
 
     # Capabilities
     allow_list = True
     allow_get = True
     allow_create = True
+    allow_update = True
     allow_delete = True
 
     _query_mapping = resource2.QueryParameters("image", "flavor", "name",
                                                "status",
                                                changes_since="changes-since")
 
     # Properties
@@ -54,14 +55,16 @@
     admin_pass = resource2.Body('adminPass')
     #: Status of the Dedicated Hypervisor instance.
     status = resource2.Body('status')
     #: detail of baremetal server.
     baremetal_server = resource2.Body('baremetal_server')
     #: Server's availability zone.
     availability_zone = resource2.Body('availability_zone')
+    #: Connection between the server and common function gateway network is established or not.
+    cfgw_connection_status = resource2.Body('cfgw_connection_status')
 
 
 class ServerDetail(Server):
     base_path = '/servers/detail'
 
     # capabilities
     allow_list = True
@@ -93,26 +96,70 @@
         uri = self.base_path % server_id
         params = {}
         params["license_types"] = license_types
         if vm_id:
             params["vm_id"] = vm_id
         if vm_name:
             params["vm_name"] = vm_name
-        body = { "add-license-to-vm": params }
+        body = {"add-license-to-vm": params}
         resp = session.post(
             uri,
             endpoint_filter=self.service,
             json=body
         )
         self._translate_response(resp, has_body=True)
         return self
 
     def get_add_license_job(self, session, server_id, job_id):
         uri = self.base_path % server_id
-        body = { "get-result-for-add-license-to-vm": { "job_id": job_id } }
+        body = {"get-result-for-add-license-to-vm": {"job_id": job_id}}
         resp = session.post(
             uri,
             endpoint_filter=self.service,
             json=body
         )
         self._translate_response(resp, has_body=True)
         return self
+
+
+class CFGWConnection(Server):
+    resource_key = "server"
+    base_path = '/servers/%s/cfgw_connection'
+
+    id = resource2.Body('id')
+    cfgw_connection = resource2.Body('cfgw_connection')
+
+    def get_cfgw_connection(self, session, server_id):
+        """
+        Shows the connection status between your Dedicated Hypervisor and
+        common function gateway network.
+
+        :param session: The session to use for making this request.
+        :param string server_id: ID for the server.
+        :return: One :class:`~ecl.dedicated_hypervisor.v1.server.CFGWConnection`
+            instance.
+        """
+        uri = self.base_path % server_id
+        resp = session.get(
+            uri,
+            endpoint_filter=self.service
+        )
+        self._translate_response(resp)
+        return self
+
+    def update_cfgw_connection(self, session, server_id):
+        """
+        Updates the connection status between your Dedicated Hypervisor and
+        common function gateway network.
+
+        :param session: The session to use for making this request.
+        :param string server_id: ID for the server.
+        :return: One :class:`~ecl.dedicated_hypervisor.v1.server.CFGWConnection`
+            instance.
+        """
+        uri = self.base_path % server_id
+        resp = session.post(
+            uri,
+            endpoint_filter=self.service
+        )
+        self._translate_response(resp)
+        return self
```

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/usage.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/usage.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dedicated_hypervisor/v1/vcf.py` & `eclsdk-1.3.0/ecl/dedicated_hypervisor/v1/vcf.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dns/dns_service.py` & `eclsdk-1.3.0/ecl/dns/dns_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dns/v2/_proxy.py` & `eclsdk-1.3.0/ecl/dns/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dns/v2/name_server.py` & `eclsdk-1.3.0/ecl/dns/v2/name_server.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dns/v2/recordset.py` & `eclsdk-1.3.0/ecl/dns/v2/recordset.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/dns/v2/zone.py` & `eclsdk-1.3.0/ecl/dns/v2/zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/exceptions.py` & `eclsdk-1.3.0/ecl/exceptions.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/format.py` & `eclsdk-1.3.0/ecl/format.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/identity_service.py` & `eclsdk-1.3.0/ecl/identity/identity_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v2/_proxy.py` & `eclsdk-1.3.0/ecl/identity/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v2/extension.py` & `eclsdk-1.3.0/ecl/identity/v2/extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v2/role.py` & `eclsdk-1.3.0/ecl/identity/v2/role.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v2/tenant.py` & `eclsdk-1.3.0/ecl/identity/v2/tenant.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v2/user.py` & `eclsdk-1.3.0/ecl/identity/v2/user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/_proxy.py` & `eclsdk-1.3.0/ecl/identity/v3/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/credential.py` & `eclsdk-1.3.0/ecl/identity/v3/credential.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/domain.py` & `eclsdk-1.3.0/ecl/identity/v3/domain.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/endpoint.py` & `eclsdk-1.3.0/ecl/identity/v3/endpoint.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/group.py` & `eclsdk-1.3.0/ecl/identity/v3/group.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/policy.py` & `eclsdk-1.3.0/ecl/identity/v3/policy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/project.py` & `eclsdk-1.3.0/ecl/identity/v3/project.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/region.py` & `eclsdk-1.3.0/ecl/identity/v3/region.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/service.py` & `eclsdk-1.3.0/ecl/identity/v3/service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/trust.py` & `eclsdk-1.3.0/ecl/identity/v3/trust.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/v3/user.py` & `eclsdk-1.3.0/ecl/identity/v3/user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/identity/version.py` & `eclsdk-1.3.0/ecl/identity/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/image_service.py` & `eclsdk-1.3.0/ecl/image/image_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/_proxy.py` & `eclsdk-1.3.0/ecl/image/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/image.py` & `eclsdk-1.3.0/ecl/image/v2/image.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/image_copy.py` & `eclsdk-1.3.0/ecl/image/v2/image_copy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/license.py` & `eclsdk-1.3.0/ecl/image/v2/license.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/member.py` & `eclsdk-1.3.0/ecl/image/v2/member.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/schema.py` & `eclsdk-1.3.0/ecl/image/v2/schema.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/image/v2/tag.py` & `eclsdk-1.3.0/ecl/image/v2/tag.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/module_loader.py` & `eclsdk-1.3.0/ecl/module_loader.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/mvna_service.py` & `eclsdk-1.3.0/ecl/mvna/mvna_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/_proxy.py` & `eclsdk-1.3.0/ecl/mvna/v1/_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -709,28 +709,29 @@
     def policies(self, **params):
         """List Policies."""
         return list(self._list(_policy.Policy, paginated=False, **params))
 
     def create_policy(self, health_monitor_id, listener_id,
                       default_target_group_id, load_balancer_id,
                       name=None, description=None, tags=None, algorithm=None,
-                      persistence=None, sorry_page_url=None, source_nat=None,
-                      certificate_id=None, tls_policy_id=None
+                      persistence=None, idle_timeout=None, sorry_page_url=None,
+                      source_nat=None, certificate_id=None, tls_policy_id=None
                       ):
         """Create Policy.
 
         :param string health_monitor_id: Health Monitor ID of Policy
         :param string listener_id: Listener ID of Policy
         :param string default_target_group_id: Default Target Group ID
         :param string load_balancer_id: Load Balancer ID
         :param string name: Name of Policy
         :param string description: Description of Policy
         :param dict tags: Tags of Policy
         :param string algorithm: Algorithm of Policy
         :param string persistence: Persistence of Policy
+        :param integer idle_timeout: Idle Timeout of Policy
         :param string sorry_page_url: Sorry page URL
         :param string source_nat: Source NAT
         :param string certificate_id: Certificate ID
         :param string tls_policy_id: TLS Policy ID
         :return: Policy
         """
         body = {
@@ -745,14 +746,16 @@
             body["description"] = description
         if tags is not None:
             body["tags"] = tags
         if algorithm is not None:
             body["algorithm"] = algorithm
         if persistence is not None:
             body["persistence"] = persistence
+        if idle_timeout is not None:
+            body["idle_timeout"] = idle_timeout
         if sorry_page_url is not None:
             body["sorry_page_url"] = sorry_page_url
         if source_nat is not None:
             body["source_nat"] = source_nat
         if certificate_id is not None:
             body["certificate_id"] = certificate_id
         if tls_policy_id is not None:
@@ -794,40 +797,43 @@
                     attempting to delete a nonexistent policy.
         :return: None
         """
         self._delete(_policy.Policy, policy_id, ignore_missing=ignore_missing)
 
     def create_staged_policy_configuration(self, policy_id,
                                            algorithm=None, persistence=None,
-                                           sorry_page_url=None, source_nat=None,
-                                           certificate_id=None,
+                                           idle_timeout=None, sorry_page_url=None,
+                                           source_nat=None, certificate_id=None,
                                            health_monitor_id=None,
                                            listener_id=None,
                                            default_target_group_id=None,
                                            tls_policy_id=None
                                            ):
         """Create Staged Policy Configuration.
 
         :param string policy_id: ID of Policy
         :param string algorithm: Algorithm of Policy
         :param string persistence: Persistence of Policy
+        :param integer idle_timeout: Idle Timeout of Policy
         :param string sorry_page_url: Sorry page URL
         :param string source_nat: Source NAT
         :param string certificate_id: Certificate ID
         :param string health_monitor_id: Health Monitor ID of Policy
         :param string listener_id: Listener ID of Policy
         :param string default_target_group_id: Default Target Group ID
         :param string tls_policy_id: TLS Policy ID
         :return: Policy
         """
         body = {}
         if algorithm is not None:
             body["algorithm"] = algorithm
         if persistence is not None:
             body["persistence"] = persistence
+        if idle_timeout is not None:
+            body["idle_timeout"] = idle_timeout
         if sorry_page_url is not None:
             body["sorry_page_url"] = sorry_page_url
         if source_nat is not None:
             body["source_nat"] = source_nat
         if certificate_id is not None:
             body["certificate_id"] = certificate_id
         if health_monitor_id is not None:
@@ -850,40 +856,43 @@
         :return: Policy
         """
         policy = _policy.Policy()
         return policy.get_staged_configuration_resource(self.session, policy_id)
 
     def update_staged_policy_configuration(self, policy_id,
                                            algorithm=None, persistence=None,
-                                           sorry_page_url=None, source_nat=None,
-                                           certificate_id=None,
+                                           idle_timeout=None, sorry_page_url=None,
+                                           source_nat=None, certificate_id=None,
                                            health_monitor_id=None,
                                            listener_id=None,
                                            default_target_group_id=None,
                                            tls_policy_id=None
                                            ):
         """Update Staged Policy Configuration.
 
         :param string policy_id: ID of Policy
         :param string algorithm: Algorithm of Policy
         :param string persistence: Persistence of Policy
+        :param integer idle_timeout: Idle Timeout of Policy
         :param string sorry_page_url: Sorry page URL
         :param string source_nat: Source NAT
         :param string certificate_id: Certificate ID
         :param string health_monitor_id: Health Monitor ID of Policy
         :param string listener_id: Listener ID of Policy
         :param string default_target_group_id: Default Target Group ID
         :param string tls_policy_id: TLS Policy ID
         :return: Policy
         """
         body = {}
         if algorithm is not None:
             body["algorithm"] = algorithm
         if persistence is not None:
             body["persistence"] = persistence
+        if idle_timeout is not None:
+            body["idle_timeout"] = idle_timeout
         if sorry_page_url is not None:
             body["sorry_page_url"] = sorry_page_url
         if source_nat is not None:
             body["source_nat"] = source_nat
         if certificate_id is not None:
             body["certificate_id"] = certificate_id
         if health_monitor_id is not None:
```

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/base.py` & `eclsdk-1.3.0/ecl/mvna/v1/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/certificate.py` & `eclsdk-1.3.0/ecl/mvna/v1/certificate.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/health_monitor.py` & `eclsdk-1.3.0/ecl/mvna/v1/health_monitor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/listener.py` & `eclsdk-1.3.0/ecl/mvna/v1/listener.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/load_balancer.py` & `eclsdk-1.3.0/ecl/mvna/v1/load_balancer.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/operation.py` & `eclsdk-1.3.0/ecl/mvna/v1/operation.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/plan.py` & `eclsdk-1.3.0/ecl/mvna/v1/plan.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/policy.py` & `eclsdk-1.3.0/ecl/mvna/v1/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         "id",
         "name",
         "description",
         "configuration_status",
         "operation_status",
         "algorithm",
         "persistence",
+        "idle_timeout",
         "sorry_page_url",
         "source_nat",
         "certificate_id",
         "health_monitor_id",
         "listener_id",
         "default_target_group_id",
         "tls_policy_id",
@@ -50,14 +51,16 @@
     configuration_status = resource2.Body('configuration_status')
     #: Operation status of policy
     operation_status = resource2.Body('operation_status')
     #: Algorithm of policy
     algorithm = resource2.Body('algorithm')
     #: persistence of policy
     persistence = resource2.Body('persistence')
+    #: Idle Timeout of policy
+    idle_timeout = resource2.Body('idle_timeout')
 
     #: Sorry page URL of policy
     sorry_page_url = resource2.Body('sorry_page_url')
     #: Source NAT of policy
     source_nat = resource2.Body('source_nat')
     #: Certificate ID of policy
     certificate_id = resource2.Body('certificate_id')
```

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/route.py` & `eclsdk-1.3.0/ecl/mvna/v1/route.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/rule.py` & `eclsdk-1.3.0/ecl/mvna/v1/rule.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/system_update.py` & `eclsdk-1.3.0/ecl/mvna/v1/system_update.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/target_group.py` & `eclsdk-1.3.0/ecl/mvna/v1/target_group.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/mvna/v1/tls_policy.py` & `eclsdk-1.3.0/ecl/mvna/v1/tls_policy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/network_service.py` & `eclsdk-1.3.0/ecl/network/network_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/_proxy.py` & `eclsdk-1.3.0/ecl/network/v2/_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ecl.network.v2 import vpn as _vpn
 from ecl.network.v2 import interdc as _interdc
 from ecl.network.v2 import aws as _aws
 from ecl.network.v2 import gcp as _gcp
 from ecl.network.v2 import tenant_connection as _tenant_connection
 from ecl.network.v2 import azure as _azure
 from ecl.network.v2 import fic as _fic
+from ecl.network.v2 import mec as _mec
 
 from ecl import proxy2
 
 
 class Proxy(proxy2.BaseProxy):
 
     def create_network(self, admin_state_up=None, description=None,
@@ -1280,14 +1281,15 @@
 
     def create_gateway_interface(self, service_type, network_id, netmask,
                                  primary_ipv4, secondary_ipv4, gw_vipv4, vrid,
                                  name=None, description=None,
                                  primary_ipv6=None, secondary_ipv6=None,
                                  gw_vipv6=None, interdc_gw_id=None,
                                  internet_gw_id=None,
+                                 mec_gw_id=None,
                                  vpn_gw_id=None, aws_gw_id=None, gcp_gw_id=None,
                                  azure_gw_id=None, fic_gw_id=None, tenant_id=None):
         """Create a Gateway Interface from parameters
 
         :param string service_type: service type of gateway interface to create
         :param string network_id: network ID of gateway interface to create
         :param int netmask: netmask of gateway interface to create
@@ -1298,14 +1300,15 @@
         :param string name: name of gateway interface to create
         :param string description: description of gateway interface to create
         :param IPv6 primary_ipv6: primary IPv6 of gateway interface to create
         :param IPv6 secondary_ipv6: secondary IPv6 of gateway interface to create
         :param IPv6 gw_vipv6: gateway virtual IPv6 of gateway interface to create
         :param string interdc_gw_id: InterDC Gateway ID of gateway interface to create
         :param string internet_gw_id: Internet Gateway ID of gateway interface to create
+        :param string mec_gw_id: MEC Gateway ID of gateway interface to create
         :param string vpn_gw_id: VPN Gateway ID of gateway interface to create
         :param string fic_gw_id: FIC Gateway ID of gateway interface to create
         :param string tenant_id: tenant ID of gateway interface to create
 
         :returns: The results of GatewayInterface creation
         :rtype: One :class:`~ecl.network.v2.gwif.GatewayInterface`
         """
@@ -1328,14 +1331,16 @@
             body.update({"secondary_ipv6": secondary_ipv6})
         if gw_vipv6:
             body.update({"gw_vipv6": gw_vipv6})
         if interdc_gw_id:
             body.update({"interdc_gw_id": interdc_gw_id})
         if internet_gw_id:
             body.update({"internet_gw_id": internet_gw_id})
+        if mec_gw_id:
+            body.update({"mec_gw_id": mec_gw_id})
         if vpn_gw_id:
             body.update({"vpn_gw_id": vpn_gw_id})
         if aws_gw_id:
             body.update({"aws_gw_id": aws_gw_id})
         if gcp_gw_id:
             body.update({"gcp_gw_id": gcp_gw_id})
         if azure_gw_id:
@@ -1411,25 +1416,26 @@
         :raises: :class:`~ecl.exceptions.ResourceNotFound`
                  when no resource can be found.
         """
         return self._get(_static_route.StaticRoute, static_route)
 
     def create_static_route(self, service_type, destination, nexthop,
                             name=None, description=None,interdc_gw_id=None,
-                            internet_gw_id=None, vpn_gw_id=None, aws_gw_id=None,
+                            internet_gw_id=None, mec_gw_id=None, vpn_gw_id=None, aws_gw_id=None,
                             gcp_gw_id=None, azure_gw_id=None, fic_gw_id=None, tenant_id=None):
         """Create a Static Route
 
         :param service_type: service type of static route to create
         :param destination: destination of static route to create
         :param nexthop: next hop of static route to create
         :param name: name of static route to create
         :param description: description of static route to create
         :param interdc_gw_id: InterDC Gateway ID of static route to create
         :param internet_gw_id: Internet Gateway ID of static route to create
+        :param mec_gw_id: MEC Gateway ID of static route to create
         :param vpn_gw_id: VPN Gateway ID of static route to create
         :param fic_gw_id: FIC Gateway ID of static route to create
         :param tenant_id: tenant ID of static route to create
 
         :return: The results of StaticRoute creation
         :rtype:  One :class:`~ecl.network.v2.staticroute.StaticRoute`
         """
@@ -1442,14 +1448,16 @@
             body.update({"name": name})
         if description:
             body.update({"description": description})
         if interdc_gw_id:
             body.update({"interdc_gw_id": interdc_gw_id})
         if internet_gw_id:
             body.update({"internet_gw_id": internet_gw_id})
+        if mec_gw_id:
+            body.update({"mec_gw_id": mec_gw_id})
         if vpn_gw_id:
             body.update({"vpn_gw_id": vpn_gw_id})
         if aws_gw_id:
             body.update({"aws_gw_id": aws_gw_id})
         if gcp_gw_id:
             body.update({"gcp_gw_id": gcp_gw_id})
         if azure_gw_id:
@@ -2585,7 +2593,85 @@
                        :class:`~ecl.network.v2.fic.FICInterface` instance.
 
         :returns: One :class:`~ecl.network.v2.fic.FICInterface`
         :raises: :class:`~ecl.exceptions.ResourceNotFound`
                  when no resource can be found.
         """
         return self._get(_fic.FICInterface, fic_interface)
+
+    def mec_services(self, **query):
+        """Return a list of MEC Service
+
+        :returns: A list of MEC Service objects
+        """
+        return list(self._list(_mec.MECService, paginated=False,
+                               **query))
+
+    def get_mec_service(self, mec_service):
+
+        """Get a single MEC Service
+
+        :param mec_service: The value can be the ID of a MEC Service or a
+                       :class:`~ecl.network.v2.mec.MECService` instance.
+
+        :returns: One :class:`~ecl.network.v2.mec.MECService`
+        :raises: :class:`~ecl.exceptions.ResourceNotFound`
+                 when no resource can be found.
+        """
+        return self._get(_mec.MECService, mec_service)
+
+    def mec_gateways(self, **query):
+        """Return a list of MEC Gateways
+
+        :param query: Query parameters to select results
+
+        :returns: A list of MEC Gateway objects
+        """
+        return list(self._list(_mec.MECGateway, paginated=False, **query))
+
+    def get_mec_gateway(self, mec_gateway):
+
+        """Get a single MEC Gateway
+
+        :param mec_gateway: The value can be the ID of a MEC Gateway or a
+                       :class:`~ecl.network.v2.mec.MECGateway` instance.
+
+        :returns: One :class:`~ecl.network.v2.mec.MECGateway`
+        :raises: :class:`~ecl.exceptions.ResourceNotFound`
+                 when no resource can be found.
+        """
+        return self._get(_mec.MECGateway, mec_gateway)
+
+    def find_mec_gateway(self, name_or_id, ignore_missing=False):
+        """Find a single mec_gateway
+
+        :param name_or_id: The name or ID of a mec_gateway.
+        :param bool ignore_missing: When set to ``False``
+                    :class:`~ecl.exceptions.ResourceNotFound` will be
+                    raised when the resource does not exist.
+                    When set to ``True``, None will be returned when
+                    attempting to find a nonexistent resource.
+        :returns: One :class:`~ecl.network.v2.mec.MECGateway` or None
+        """
+        return self._find(_mec.MECGateway,
+                          name_or_id, ignore_missing=ignore_missing)
+
+    def mec_interfaces(self, **query):
+        """Return a list of MEC Interface
+
+        :returns: A list of MEC Interface objects
+        """
+        return list(self._list(_mec.MECInterface, paginated=False,
+                               *query))
+
+    def get_mec_interface(self, mec_interface):
+
+        """Get a single MEC Gateway
+
+        :param mec_interface: The value can be the ID of a MEC Interface or a
+                       :class:`~ecl.network.v2.mec.MECInterface` instance.
+
+        :returns: One :class:`~ecl.network.v2.mec.MECInterface`
+        :raises: :class:`~ecl.exceptions.ResourceNotFound`
+                 when no resource can be found.
+        """
+        return self._get(_mec.MECInterface, mec_interface)
```

### Comparing `eclsdk-1.2.1/ecl/network/v2/aws.py` & `eclsdk-1.3.0/ecl/network/v2/aws.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/azure.py` & `eclsdk-1.3.0/ecl/network/v2/azure.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/base.py` & `eclsdk-1.3.0/ecl/network/v2/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/colocation_logical_link.py` & `eclsdk-1.3.0/ecl/network/v2/colocation_logical_link.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/colocation_physical_link.py` & `eclsdk-1.3.0/ecl/network/v2/colocation_physical_link.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/colocation_space.py` & `eclsdk-1.3.0/ecl/network/v2/colocation_space.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/common_function.py` & `eclsdk-1.3.0/ecl/network/v2/common_function.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/common_function_gateway.py` & `eclsdk-1.3.0/ecl/network/v2/common_function_gateway.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/common_function_pool.py` & `eclsdk-1.3.0/ecl/network/v2/common_function_pool.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/extension.py` & `eclsdk-1.3.0/ecl/network/v2/extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/fic.py` & `eclsdk-1.3.0/ecl/network/v2/fic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/firewall.py` & `eclsdk-1.3.0/ecl/network/v2/firewall.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/firewall_action.py` & `eclsdk-1.3.0/ecl/network/v2/firewall_action.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/firewall_interface.py` & `eclsdk-1.3.0/ecl/network/v2/firewall_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/firewall_plan.py` & `eclsdk-1.3.0/ecl/network/v2/firewall_plan.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/gcp.py` & `eclsdk-1.3.0/ecl/network/v2/gcp.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/gw_interface.py` & `eclsdk-1.3.0/ecl/network/v2/gw_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     resources_key = "gw_interfaces"
     service = network_service.NetworkService("v2.0")
     base_path = '/' + service.version + '/gw_interfaces'
 
     _query_mapping = resource2.QueryParameters(
         "description", "gw_vipv4", "gw_vipv6",
         "id", "interdc_gw_id", "internet_gw_id",
+        "mec_gw_id",
         "name", "netmask", "network_id",
         "primary_ipv4", "primary_ipv6",
         "secondary_ipv4", "secondary_ipv6",
         "service_type", "vpn_gw_id",
         "status", "tenant_id", "vrid",
         "sort_key", "sort_dir", "aws_gw_id",
         "azure_gw_id", "gcp_gw_id", "fic_gw_id",
@@ -34,14 +35,15 @@
 
     description = resource2.Body("description")
     gw_vipv4 = resource2.Body("gw_vipv4")
     gw_vipv6 = resource2.Body("gw_vipv6")
     id = resource2.Body("id")
     interdc_gw_id = resource2.Body("interdc_gw_id")
     internet_gw_id = resource2.Body("internet_gw_id")
+    mec_gw_id = resource2.Body("mec_gw_id")
     name = resource2.Body("name")
     netmask = resource2.Body("netmask")
     network_id = resource2.Body("network_id")
     primary_ipv4 = resource2.Body("primary_ipv4")
     primary_ipv6 = resource2.Body("primary_ipv6")
     secondary_ipv4 = resource2.Body("secondary_ipv4")
     secondary_ipv6 = resource2.Body("secondary_ipv6")
```

### Comparing `eclsdk-1.2.1/ecl/network/v2/interdc.py` & `eclsdk-1.3.0/ecl/network/v2/interdc.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/internet.py` & `eclsdk-1.3.0/ecl/network/v2/internet.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/load_balancer.py` & `eclsdk-1.3.0/ecl/network/v2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/load_balancer_action.py` & `eclsdk-1.3.0/ecl/network/v2/load_balancer_action.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/load_balancer_interface.py` & `eclsdk-1.3.0/ecl/network/v2/load_balancer_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/load_balancer_plan.py` & `eclsdk-1.3.0/ecl/network/v2/load_balancer_plan.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/load_balancer_syslog_server.py` & `eclsdk-1.3.0/ecl/network/v2/load_balancer_syslog_server.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/network.py` & `eclsdk-1.3.0/ecl/network/v2/network.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/physical_port.py` & `eclsdk-1.3.0/ecl/network/v2/physical_port.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/port.py` & `eclsdk-1.3.0/ecl/network/v2/port.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/publicip.py` & `eclsdk-1.3.0/ecl/network/v2/publicip.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/qos_option.py` & `eclsdk-1.3.0/ecl/network/v2/qos_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,28 @@
     base_path = '/' + service.version + '/qos_options'
 
     allow_list = True
     allow_get = True
 
     _query_mapping = resource2.QueryParameters(
         "description", "bandwidth", "name",
-        "status", "qos_type", "service_type",
+        "status", "qos_type", "mec_service_id",
+        "service_type",
         "interdc_service_id", "internet_service_id",
         "vpn_service_id", "sort_key", "sort_dir",
         "fic_service_id",
     )
 
     description = resource2.Body("description")
     bandwidth = resource2.Body("bandwidth")
     id = resource2.Body("id")
     name = resource2.Body("name")
     status = resource2.Body("status")
     qos_type = resource2.Body("qos_type")
+    mec_service_id = resource2.Body("mec_service_id")
     service_type = resource2.Body("service_type")
     interdc_service_id = resource2.Body("interdc_service_id")
     internet_service_id = resource2.Body("internet_service_id")
     vpn_service_id = resource2.Body("vpn_service_id")
     fic_service_id = resource2.Body("fic_service_id")
 
     @classmethod
```

### Comparing `eclsdk-1.2.1/ecl/network/v2/quota.py` & `eclsdk-1.3.0/ecl/network/v2/quota.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # Properties
     #: The maximum amount of colocation logical link you can have. *Type: int*
     colocation_logical_link = resource2.Body('colocation_logical_link', type=int)
     #: The maximum amount of common function gateway you can create. *Type: int*
     common_function_gateway = resource2.Body('common_function_gateway', type=int)
     #: The maximum amount of fic gateway you can create. *Type: int*
     fic_gateway = resource2.Body('fic_gateway', type=int)
+    #: The maximum amount of mec gateway you can create. *Type: int*
+    mec_gateway = resource2.Body('mec_gateway', type=int)
     #: The maximum amount of firewall you can create. *Type: int*
     firewall = resource2.Body('firewall', type=int)
     #: ID of quota
     id = resource2.Body("id")
     #: The maximum amount of interdc gateway you can create. *Type: int*
     interdc_gateway = resource2.Body('interdc_gateway', type=int)
     #: The maximum amount of internet gateway you can create. *Type: int*
```

### Comparing `eclsdk-1.2.1/ecl/network/v2/reserved_address.py` & `eclsdk-1.3.0/ecl/network/v2/reserved_address.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/static_route.py` & `eclsdk-1.3.0/ecl/network/v2/static_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,24 +18,26 @@
     allow_create = True
     allow_delete = True
     allow_update = True
 
     _query_mapping = resource2.QueryParameters(
         "description", "id", "destination",
         "name", "interdc_gw_id", "internet_gw_id",
+        "mec_gw_id",
         "nexthop", "service_type", "status", "tenant_id",
         "vpn_gw_id", "sort_key", "sort_dir", "aws_gw_id",
         "azure_gw_id", "gcp_gw_id", "fic_gw_id",
     )
 
     description = resource2.Body("description")
     destination = resource2.Body("destination")
     id = resource2.Body("id")
     interdc_gw_id = resource2.Body("interdc_gw_id")
     internet_gw_id = resource2.Body("internet_gw_id")
+    mec_gw_id = resource2.Body("mec_gw_id")
     name = resource2.Body("name")
     nexthop = resource2.Body("nexthop")
     service_type = resource2.Body("service_type")
     status = resource2.Body("status")
     tenant_id = resource2.Body("tenant_id")
     vpn_gw_id = resource2.Body("vpn_gw_id")
     aws_gw_id = resource2.Body("aws_gw_id")
```

### Comparing `eclsdk-1.2.1/ecl/network/v2/subnet.py` & `eclsdk-1.3.0/ecl/network/v2/subnet.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/tenant_connection.py` & `eclsdk-1.3.0/ecl/network/v2/tenant_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/v2/vpn.py` & `eclsdk-1.3.0/ecl/network/v2/vpn.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/network/version.py` & `eclsdk-1.3.0/ecl/network/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/orchestration/orchestration_service.py` & `eclsdk-1.3.0/ecl/rca/rca_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from ecl import service_filter
 
 
-class OrchestrationService(service_filter.ServiceFilter):
-    """The orchestration service."""
+class RcaService(service_filter.ServiceFilter):
+    """RCA service"""
 
     valid_versions = [service_filter.ValidVersion('v1')]
 
     def __init__(self, version=None):
-        """Create an orchestration service."""
-        super(OrchestrationService, self).__init__(
-            service_type='orchestration',
-            version=version,
-            requires_project_id=True,
-        )
+        """Create a RCA service"""
+        super(RcaService, self).__init__(service_type='rca',
+                                         version=version)
```

### Comparing `eclsdk-1.2.1/ecl/orchestration/v1/software_deployment.py` & `eclsdk-1.3.0/ecl/telemetry/v2/statistics.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,59 +6,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from ecl.orchestration import orchestration_service
-from ecl import resource2 as resource
+from ecl import resource
+from ecl.telemetry import telemetry_service
 
 
-class SoftwareDeployment(resource.Resource):
-    resource_key = 'software_deployment'
-    resources_key = 'software_deployments'
-    base_path = '/software_deployments'
-    service = orchestration_service.OrchestrationService()
+class Statistics(resource.Resource):
+    """.. caution:: This API is a work in progress and is subject to change."""
+    id_attribute = 'meter_name'
+    resource_key = 'statistics'
+    base_path = '/meters/%(meter_name)s/statistics'
+    service = telemetry_service.TelemetryService()
 
-    # capabilities
-    allow_create = True
+    # Supported Operations
     allow_list = True
-    allow_get = True
-    allow_delete = True
-    allow_update = True
+
+    # Path Parameter
+    meter_name = resource.prop('meter_name')
 
     # Properties
-    #: The stack action that triggers this deployment resource.
-    action = resource.Body('action')
-    #: The UUID of the software config resource that runs when applying to the
-    #: server.
-    config_id = resource.Body('config_id')
-    #: A map containing the names and values of all inputs to the config.
-    input_values = resource.Body('input_values', type=dict)
-    #: A map containing the names and values from the deployment.
-    output_values = resource.Body('output_values', type=dict)
-    #: The UUID of the compute server to which the configuration applies.
-    server_id = resource.Body('server_id')
-    #: The ID of the authentication project which can also perform operations
-    #: on this deployment.
-    stack_user_project_id = resource.Body('stack_user_project_id')
-    #: Current status of the software deployment.
-    status = resource.Body('status')
-    #: Error description for the last status change.
-    status_reason = resource.Body('status_reason')
-    #: The date and time when the software deployment resource was created.
-    created_at = resource.Body('creation_time')
-    #: The date and time when the software deployment resource was created.
-    updated_at = resource.Body('updated_time')
-
-    def create(self, session):
-        # This overrides the default behavior of resource creation because
-        # heat doesn't accept resource_key in its request.
-        return super(SoftwareDeployment, self).create(
-            session, prepend_key=False)
-
-    def update(self, session):
-        # This overrides the default behavior of resource creation because
-        # heat doesn't accept resource_key in its request.
-        return super(SoftwareDeployment, self).update(
-            session, prepend_key=False)
+    #: The selectable aggregate value(s)
+    aggregate = resource.prop('aggregate')
+    #: The average of all of the volume values seen in the data
+    avg = resource.prop('avg')
+    #: The number of samples seen
+    count = resource.prop('count')
+    #: The difference, in seconds, between the oldest and newest timestamp
+    duration = resource.prop('duration')
+    #: UTC date and time of the oldest timestamp, or the query end time.
+    duration_end_at = resource.prop('duration_end')
+    #: UTC date and time of the earliest timestamp, or the query start time.
+    duration_start_at = resource.prop('duration_start')
+    #: Dictionary of field names for group, if groupby statistics are requested
+    group_by = resource.prop('groupby')
+    #: The maximum volume seen in the data
+    max = resource.prop('max')
+    #: The minimum volume seen in the data
+    min = resource.prop('min')
+    #: The difference, in seconds, between the period start and end
+    period = resource.prop('period')
+    #: UTC date and time of the period end.
+    period_end_at = resource.prop('period_end')
+    #: UTC date and time of the period start.
+    period_start_at = resource.prop('period_start')
+    #: The total of all of the volume values seen in the data
+    sum = resource.prop('sum')
+    #: The unit type of the data set
+    unit = resource.prop('unit')
+
+    @classmethod
+    def list(cls, session, limit=None, marker=None, path_args=None,
+             paginated=False, **params):
+        url = cls._get_url(path_args)
+        resp = session.get(url, endpoint_filter=cls.service, params=params)
+        for stat in resp.json():
+            yield cls.existing(**stat)
```

### Comparing `eclsdk-1.2.1/ecl/orchestration/v1/template.py` & `eclsdk-1.3.0/ecl/telemetry/v2/sample.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,47 +6,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from six.moves.urllib import parse
+from ecl import resource
+from ecl.telemetry import telemetry_service
 
-from ecl.orchestration import orchestration_service
-from ecl import resource2 as resource
 
-
-class Template(resource.Resource):
-    service = orchestration_service.OrchestrationService()
-
-    # capabilities
-    allow_create = False
-    allow_list = False
-    allow_retrieve = False
-    allow_delete = False
-    allow_update = False
+class Sample(resource.Resource):
+    """.. caution:: This API is a work in progress and is subject to change."""
+    id_attribute = 'sample_id'
+    base_path = '/meters/%(counter_name)s'
+    service = telemetry_service.TelemetryService()
+
+    # Supported Operations
+    allow_create = True
+    allow_list = True
 
     # Properties
-    #: The description specified in the template
-    description = resource.Body('Description')
-    #: Key and value pairs that contain template parameters
-    parameters = resource.Body('Parameters', type=dict)
-    #: A list of parameter groups each contains a lsit of parameter names.
-    parameter_groups = resource.Body('ParameterGroups', type=list)
-
-    def validate(self, session, template, environment=None, template_url=None,
-                 ignore_errors=None):
-        url = '/validate'
-
-        body = {'template': template}
-        if environment is not None:
-            body['environment'] = environment
-        if template_url is not None:
-            body['template_url'] = template_url
-        if ignore_errors:
-            qry = parse.urlencode({'ignore_errors': ignore_errors})
-            url = '?'.join([url, qry])
-
-        resp = session.post(url, endpoint_filter=self.service, json=body)
-        self._translate_response(resp)
+    #: The meter name this sample is for
+    counter_name = resource.prop('meter', alias='counter_name')
+    #: When the sample has been generated.
+    generated_at = resource.prop('timestamp')
+    #: Arbitrary metadata associated with the sample
+    metadata = resource.prop('metadata', alias='resource_metadata')
+    #: The ID of the project this sample was taken for
+    project_id = resource.prop('project_id')
+    #: When the sample has been recorded.
+    recorded_at = resource.prop('recorded_at')
+    #: The ID of the resource this sample was taken for
+    resource_id = resource.prop('resource_id')
+    #: The name of the source that identifies where the sample comes from
+    source = resource.prop('source')
+    #: The meter type
+    type = resource.prop('type', alias='counter_type')
+    #: The unit of measure
+    unit = resource.prop('unit', alias='counter_unit')
+    #: The ID of the user this sample was taken for
+    user_id = resource.prop('user_id')
+    #: The metered value
+    volume = resource.prop('volume', alias='counter_volume')
+
+    @classmethod
+    def list(cls, session, limit=None, marker=None, path_args=None,
+             paginated=False, **params):
+        url = cls._get_url(path_args)
+        resp = session.get(url, endpoint_filter=cls.service, params=params)
+        for item in resp.json():
+            yield cls.existing(**item)
+
+    def create(self, session):
+        url = self._get_url(self)
+        # telemetry expects a list of samples
+        attrs = self._attrs.copy()
+        attrs.pop('meter', None)
+        resp = session.post(url, endpoint_filter=self.service,
+                            json=[attrs])
+        resp = resp.json()
+        self.update_attrs(**resp.pop())
+        self._reset_dirty()
         return self
```

### Comparing `eclsdk-1.2.1/ecl/orchestration/version.py` & `eclsdk-1.3.0/ecl/telemetry/telemetry_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,25 +6,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from ecl.orchestration import orchestration_service
-from ecl import resource
+from ecl import service_filter
 
 
-class Version(resource.Resource):
-    resource_key = 'version'
-    resources_key = 'versions'
-    base_path = '/'
-    service = orchestration_service.OrchestrationService(
-        version=orchestration_service.OrchestrationService.UNVERSIONED
-    )
+class TelemetryService(service_filter.ServiceFilter):
+    """The telemetry service."""
 
-    # capabilities
-    allow_list = True
+    valid_versions = [service_filter.ValidVersion('v2')]
 
-    # Properties
-    links = resource.prop('links')
-    status = resource.prop('status')
+    def __init__(self, version=None):
+        """Create a telemetry service."""
+        super(TelemetryService, self).__init__(service_type='metering',
+                                               version=version)
```

### Comparing `eclsdk-1.2.1/ecl/profile.py` & `eclsdk-1.3.0/ecl/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 The resulting preference print out would look something like::
 
     service_type=compute,region=zion,service_name=matrix
     service_type=network,region=zion
     service_type=image,region=zion
     service_type=metering,region=zion
-    service_type=orchestration,region=zion
     service_type=identity,region=zion,version=v3
 """
 
 import copy
 import logging
 import six
 
@@ -59,23 +58,22 @@
 from ecl.connectivity import connectivity_service
 from ecl.dedicated_hypervisor import dedicated_hypervisor_service
 from ecl import exceptions
 from ecl.identity import identity_service
 from ecl.image import image_service
 from ecl import module_loader
 from ecl.network import network_service
-from ecl.orchestration import orchestration_service
 from ecl.provider_connectivity import provider_connectivity_service
 from ecl.rca import rca_service
 from ecl.storage import storage_service
 from ecl.security_order import security_order_service
 from ecl.security_portal import security_portal_service
-## This section will be deleted if MSS v1 API is not available
-from ecl.security_order_v1 import security_order_service as security_order_service_v1
-from ecl.security_portal_v1 import security_portal_service as security_portal_service_v1
+## This section will be deleted if MSS v2 API is not available
+from ecl.security_order_v2 import security_order_service as security_order_service_v2
+from ecl.security_portal_v2 import security_portal_service as security_portal_service_v2
 ## end of the section
 from ecl.sss import sss_service
 from ecl.telemetry import telemetry_service
 from ecl.dns import dns_service
 from ecl.virtual_network_appliance import virtual_network_appliance_service
 from ecl.mvna import mvna_service
 
@@ -104,30 +102,28 @@
         self._add_service(
             connectivity_service.ConnectivityService(version="v1"))
         self._add_service(identity_service.IdentityService(version="v3"))
         self._add_service(image_service.ImageService(version="v2"))
         self._add_service(network_service.NetworkService(version="v2"))
         self._add_service(sss_service.SssService(version="v1"))
         self._add_service(
-            orchestration_service.OrchestrationService(version="v1"))
-        self._add_service(
             provider_connectivity_service.ProviderConnectivityService(
                 version="v2"))
         self._add_service(telemetry_service.TelemetryService(version="v2"))
         self._add_service(block_store_service.BlockStoreService(version="v2"))
         self._add_service(storage_service.StorageService(version="v1"))
         self._add_service(
-            security_order_service.SecurityOrderService(version="v2"))
+            security_order_service.SecurityOrderService(version="v3"))
         self._add_service(
-            security_portal_service.SecurityPortalService(version="v2"))
-        ## This section will be deleted if MSS v1 API is not available
+            security_portal_service.SecurityPortalService(version="v3"))
+        ## This section will be deleted if MSS v2 API is not available
         self._add_service(
-            security_order_service_v1.SecurityOrderService(version="v1"))
+            security_order_service_v2.SecurityOrderService(version="v2"))
         self._add_service(
-            security_portal_service_v1.SecurityPortalService(version="v1"))
+            security_portal_service_v2.SecurityPortalService(version="v2"))
         ## end of the section
         self._add_service(rca_service.RcaService(version="v1"))
         self._add_service(baremetal_service.BaremetalService(version="v2"))
         self._add_service(
             dedicated_hypervisor_service.DedicatedHypervisorService(
                 version="v1"))
         self._add_service(dns_service.DnsService(version="v2"))
```

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/provider_connectivity_service.py` & `eclsdk-1.3.0/ecl/provider_connectivity/provider_connectivity_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/_proxy.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/address_assignment.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/address_assignment.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/aws_connection.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/aws_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/base.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/exchange_point.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/exchange_point.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/operation.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/operation.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/tenant_connection.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/tenant_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v1/tenant_connection_request.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v1/tenant_connection_request.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/_proxy.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/address_assignment.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/address_assignment.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/aws_connection.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/aws_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/base.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/exchange_point.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/exchange_point.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/gcp_connection.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/gcp_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/operation.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/operation.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/tenant_connection.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/tenant_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/provider_connectivity/v2/tenant_connection_request.py` & `eclsdk-1.3.0/ecl/provider_connectivity/v2/tenant_connection_request.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/proxy.py` & `eclsdk-1.3.0/ecl/proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/proxy2.py` & `eclsdk-1.3.0/ecl/proxy2.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/rca/rca_service.py` & `eclsdk-1.3.0/ecl/storage/storage_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from ecl import service_filter
 
 
-class RcaService(service_filter.ServiceFilter):
-    """RCA service"""
+class StorageService(service_filter.ServiceFilter):
+    """storage service."""
 
-    valid_versions = [service_filter.ValidVersion('v1')]
+    valid_versions = [service_filter.ValidVersion('v1', path='v1.0')]
 
     def __init__(self, version=None):
-        """Create a RCA service"""
-        super(RcaService, self).__init__(service_type='rca',
-                                         version=version)
+        """Create a storage service."""
+        super(StorageService, self).__init__(service_type='storage', version=version)
```

### Comparing `eclsdk-1.2.1/ecl/rca/v1/_proxy.py` & `eclsdk-1.3.0/ecl/rca/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/rca/v1/user.py` & `eclsdk-1.3.0/ecl/rca/v1/user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/rca/version.py` & `eclsdk-1.3.0/ecl/rca/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/resource.py` & `eclsdk-1.3.0/ecl/resource.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/resource2.py` & `eclsdk-1.3.0/ecl/resource2.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order/v2/_proxy.py` & `eclsdk-1.3.0/ecl/security_order_v2/v2/_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from ecl.security_order.v2 import device as _fgs
-from ecl.security_order.v2 import ha_device as _fgha
-from ecl.security_order.v2 import waf as _fgwaf
-from ecl.security_order.v2 import host_based_security as _hbs
+from ecl.security_order_v2.v2 import device as _fgs
+from ecl.security_order_v2.v2 import ha_device as _fgha
+from ecl.security_order_v2.v2 import waf as _fgwaf
+from ecl.security_order_v2.v2 import host_based_security as _hbs
 from ecl import proxy2
 
 
 class Proxy(proxy2.BaseProxy):
 
     def devices(self, locale=None):
         """List Managed Firwall/UTM devices of single constitution.
```

### Comparing `eclsdk-1.2.1/ecl/security_order/v2/device.py` & `eclsdk-1.3.0/ecl/security_order/v3/device.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order/v2/ha_device.py` & `eclsdk-1.3.0/ecl/security_order/v3/ha_device.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order/v2/host_based_security.py` & `eclsdk-1.3.0/ecl/security_order/v3/host_based_security.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order/v2/waf.py` & `eclsdk-1.3.0/ecl/security_order/v3/waf.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order_v1/v1/_proxy.py` & `eclsdk-1.3.0/ecl/security_order_v1/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order_v1/v1/device.py` & `eclsdk-1.3.0/ecl/security_order_v1/v1/device.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order_v1/v1/ha_device.py` & `eclsdk-1.3.0/ecl/security_order_v1/v1/ha_device.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order_v1/v1/host_based_security.py` & `eclsdk-1.3.0/ecl/security_order_v1/v1/host_based_security.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_order_v1/v1/waf.py` & `eclsdk-1.3.0/ecl/security_order_v1/v1/waf.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_portal/v2/_proxy.py` & `eclsdk-1.3.0/ecl/security_portal_v2/v2/_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
-from ecl.security_portal.v2 import security_device as _sd
-from ecl.security_portal.v2 import security_device_interface as _sdi
+from ecl.security_portal_v2.v2 import security_device as _sd
+from ecl.security_portal_v2.v2 import security_device_interface as _sdi
 from ecl import proxy2
 
 
 class Proxy(proxy2.BaseProxy):
     def security_devices(self):
         """Listing security devices associated with specific tenant.
```

### Comparing `eclsdk-1.2.1/ecl/security_portal/v2/security_device.py` & `eclsdk-1.3.0/ecl/security_portal_v2/v2/security_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from ecl.security_portal import security_portal_service
+from ecl.security_portal_v2 import security_portal_service
 from ecl import resource2
 from ecl import exceptions
 from ecl import utils
 
 
 class SecurityDevice(resource2.Resource):
     resource_key = "device"
```

### Comparing `eclsdk-1.2.1/ecl/security_portal/v2/security_device_interface.py` & `eclsdk-1.3.0/ecl/security_portal_v2/v2/security_device_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from ecl.security_portal import security_portal_service
+from ecl.security_portal_v2 import security_portal_service
 from ecl import resource2
 from ecl import exceptions
 from ecl import utils
 
 
 class SecurityDeviceInterface(resource2.Resource):
     resource_key = "device_interface"
```

### Comparing `eclsdk-1.2.1/ecl/security_portal_v1/v1/_proxy.py` & `eclsdk-1.3.0/ecl/security_portal_v1/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_portal_v1/v1/security_device.py` & `eclsdk-1.3.0/ecl/security_portal_v1/v1/security_device.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/security_portal_v1/v1/security_device_interface.py` & `eclsdk-1.3.0/ecl/security_portal_v1/v1/security_device_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/service_filter.py` & `eclsdk-1.3.0/ecl/service_filter.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/session.py` & `eclsdk-1.3.0/ecl/session.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/sss_service.py` & `eclsdk-1.3.0/ecl/sss/sss_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,11 +14,20 @@
 
 
 class SssService(service_filter.ServiceFilter):
     """The SSS service."""
 
     valid_versions = [service_filter.ValidVersion('v1')]
 
-    def __init__(self, version=None):
+    def __init__(self, **kwargs):
         """Create a SSS service."""
-        super(SssService, self).__init__(service_type='sss',
-                                         version=version)
+        super(SssService, self).__init__(service_type='sssv2',
+                                         **kwargs)
+
+
+class SssAdminService(SssService):
+    """The SSS service. (Admin Endpoint)"""
+
+    def __init__(self, **kwargs):
+        kwargs['interface'] = service_filter.ServiceFilter.ADMIN
+        super(SssAdminService, self).__init__(**kwargs)
+
```

### Comparing `eclsdk-1.2.1/ecl/sss/v1/_proxy.py` & `eclsdk-1.3.0/ecl/sss/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/api_key.py` & `eclsdk-1.3.0/ecl/sss/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/channel.py` & `eclsdk-1.3.0/ecl/sss/v1/channel.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/contract.py` & `eclsdk-1.3.0/ecl/sss/v1/contract.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/iam_group.py` & `eclsdk-1.3.0/ecl/sss/v1/iam_group.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/iam_role.py` & `eclsdk-1.3.0/ecl/sss/v1/iam_role.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/role.py` & `eclsdk-1.3.0/ecl/sss/v1/role.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/tenant.py` & `eclsdk-1.3.0/ecl/sss/v1/tenant.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/sss/v1/user.py` & `eclsdk-1.3.0/ecl/sss/v1/user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/storage_service.py` & `eclsdk-1.3.0/ecl/sss/v2/service_menu.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from ecl import service_filter
+from ecl import resource2
+from ecl.sss import sss_service
 
 
-class StorageService(service_filter.ServiceFilter):
-    """storage service."""
+class ServiceMenu(resource2.Resource):
+    service = sss_service.SssAdminService()
 
-    valid_versions = [service_filter.ValidVersion('v1', path='v1.0')]
+    # Properties
+    #: User id. format is ecid[0-9]{10}.
+    user_id = resource2.Body('user_id')
+    #: Category information of service menu
+    categories = resource2.Body('categories')
 
-    def __init__(self, version=None):
-        """Create a storage service."""
-        super(StorageService, self).__init__(service_type='storage', version=version)
+    def get_user_service_menu(self, session, user_id):
+        """Get menu of services available to user.
+
+        :param session: The session to use for making this request.
+        :param user_id: ID of a user
+        :return: :class:`~ecl.sss.v2.service_menu.ServiceMenu`
+        """
+        url = '/users/%s/service-menus' % user_id
+        resp = session.get(url, endpoint_filter=self.service)
+        self._translate_response(resp, has_body=True)
+        return self
```

### Comparing `eclsdk-1.2.1/ecl/storage/v1/_proxy.py` & `eclsdk-1.3.0/ecl/storage/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/v1/availability_zone.py` & `eclsdk-1.3.0/ecl/storage/v1/availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/v1/snapshot.py` & `eclsdk-1.3.0/ecl/storage/v1/snapshot.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/v1/storage.py` & `eclsdk-1.3.0/ecl/storage/v1/storage.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/v1/volume.py` & `eclsdk-1.3.0/ecl/storage/v1/volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/v1/volume_type.py` & `eclsdk-1.3.0/ecl/storage/v1/volume_type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/storage/version.py` & `eclsdk-1.3.0/ecl/storage/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/telemetry/telemetry_service.py` & `eclsdk-1.3.0/ecl/telemetry/v2/capability.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from ecl import service_filter
+import six
 
+from ecl import resource
+from ecl.telemetry import telemetry_service
 
-class TelemetryService(service_filter.ServiceFilter):
-    """The telemetry service."""
 
-    valid_versions = [service_filter.ValidVersion('v2')]
+class Capability(resource.Resource):
+    """.. caution:: This API is a work in progress and is subject to change."""
+    resource_key = 'capability'
+    resources_key = 'capabilities'
+    base_path = '/capabilities'
+    service = telemetry_service.TelemetryService()
 
-    def __init__(self, version=None):
-        """Create a telemetry service."""
-        super(TelemetryService, self).__init__(service_type='metering',
-                                               version=version)
+    # Supported Operations
+    allow_list = True
+
+    # Properties
+    is_enabled = resource.prop('enabled', type=bool)
+
+    @classmethod
+    def list(cls, session, limit=None, marker=None, path_args=None,
+             paginated=False, **params):
+        resp = session.get(cls.base_path, endpoint_filter=cls.service,
+                           params=params)
+        resp = resp.json()
+        for key, value in six.iteritems(resp['api']):
+            yield cls.existing(id=key, enabled=value)
```

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/_proxy.py` & `eclsdk-1.3.0/ecl/telemetry/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/alarm.py` & `eclsdk-1.3.0/ecl/telemetry/v2/alarm.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/alarm_change.py` & `eclsdk-1.3.0/ecl/telemetry/v2/alarm_change.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/capability.py` & `eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_alarm_change.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,34 +6,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import six
+import unittest
+import uuid
 
-from ecl import resource
-from ecl.telemetry import telemetry_service
+from ecl.tests.functional import base
 
 
-class Capability(resource.Resource):
-    """.. caution:: This API is a work in progress and is subject to change."""
-    resource_key = 'capability'
-    resources_key = 'capabilities'
-    base_path = '/capabilities'
-    service = telemetry_service.TelemetryService()
+@unittest.skip("bug/1524468")
+@unittest.skipUnless(base.service_exists(service_type="metering"),
+                     "Metering service does not exist")
+class TestAlarmChange(base.BaseFunctionalTest):
 
-    # Supported Operations
-    allow_list = True
+    NAME = uuid.uuid4().hex
+    alarm = None
 
-    # Properties
-    is_enabled = resource.prop('enabled', type=bool)
+    @classmethod
+    def setUpClass(cls):
+        super(TestAlarmChange, cls).setUpClass()
+        meter = next(cls.conn.telemetry.meters())
+        alarm = cls.conn.telemetry.create_alarm(
+            name=cls.NAME,
+            type='threshold',
+            threshold_rule={
+                'meter_name': meter.name,
+                'threshold': 1.1,
+            },
+        )
+        cls.alarm = alarm
 
     @classmethod
-    def list(cls, session, limit=None, marker=None, path_args=None,
-             paginated=False, **params):
-        resp = session.get(cls.base_path, endpoint_filter=cls.service,
-                           params=params)
-        resp = resp.json()
-        for key, value in six.iteritems(resp['api']):
-            yield cls.existing(id=key, enabled=value)
+    def tearDownClass(cls):
+        cls.conn.telemetry.delete_alarm(cls.alarm, ignore_missing=False)
+
+    def test_list(self):
+        change = next(self.conn.telemetry.alarm_changes(self.alarm))
+        self.assertEqual(self.alarm.id, change.alarm_id)
+        self.assertEqual('creation', change.type)
```

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/meter.py` & `eclsdk-1.3.0/ecl/telemetry/v2/meter.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/resource.py` & `eclsdk-1.3.0/ecl/telemetry/v2/resource.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/telemetry/v2/sample.py` & `eclsdk-1.3.0/ecl/sss/v2/token.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,64 +6,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from ecl import resource
-from ecl.telemetry import telemetry_service
+from ecl import resource2
+from ecl.sss import sss_service
 
 
-class Sample(resource.Resource):
-    """.. caution:: This API is a work in progress and is subject to change."""
-    id_attribute = 'sample_id'
-    base_path = '/meters/%(counter_name)s'
-    service = telemetry_service.TelemetryService()
+class Token(resource2.Resource):
+    resources_key = None
+    resource_key = 'token'
+    base_path = '/tokens/users'
+    service = sss_service.SssAdminService()
 
-    # Supported Operations
+    # Capabilities
     allow_create = True
-    allow_list = True
 
     # Properties
-    #: The meter name this sample is for
-    counter_name = resource.prop('meter', alias='counter_name')
-    #: When the sample has been generated.
-    generated_at = resource.prop('timestamp')
-    #: Arbitrary metadata associated with the sample
-    metadata = resource.prop('metadata', alias='resource_metadata')
-    #: The ID of the project this sample was taken for
-    project_id = resource.prop('project_id')
-    #: When the sample has been recorded.
-    recorded_at = resource.prop('recorded_at')
-    #: The ID of the resource this sample was taken for
-    resource_id = resource.prop('resource_id')
-    #: The name of the source that identifies where the sample comes from
-    source = resource.prop('source')
-    #: The meter type
-    type = resource.prop('type', alias='counter_type')
-    #: The unit of measure
-    unit = resource.prop('unit', alias='counter_unit')
-    #: The ID of the user this sample was taken for
-    user_id = resource.prop('user_id')
-    #: The metered value
-    volume = resource.prop('volume', alias='counter_volume')
-
-    @classmethod
-    def list(cls, session, limit=None, marker=None, path_args=None,
-             paginated=False, **params):
-        url = cls._get_url(path_args)
-        resp = session.get(url, endpoint_filter=cls.service, params=params)
-        for item in resp.json():
-            yield cls.existing(**item)
-
-    def create(self, session):
-        url = self._get_url(self)
-        # telemetry expects a list of samples
-        attrs = self._attrs.copy()
-        attrs.pop('meter', None)
-        resp = session.post(url, endpoint_filter=self.service,
-                            json=[attrs])
-        resp = resp.json()
-        self.update_attrs(**resp.pop())
-        self._reset_dirty()
+    #: The authentication method.
+    methods = resource2.Body('methods')
+    #: A user object.
+    user = resource2.Body('user')
+    #: The date and time when the token was issued.
+    issued_at = resource2.Body('issued_at')
+    #: The date and time when the token expires.
+    expires_at = resource2.Body('expires_at')
+    #: A list of audit IDs.
+    audit_ids = resource2.Body('audit_ids')
+    #: A project object including the id, name and domain object representing
+    #: the project the token is scoped to.
+    project = resource2.Body('project')
+    # Whether a project is acting as a domain.
+    is_domain = resource2.Body('is_domain')
+    #: A list of role objects.
+    roles = resource2.Body('roles')
+    #: A catalog object.
+    catalog = resource2.Body('catalog')
+    #: The authentication token. An authentication response returns
+    #: the token ID in this header rather than in the response body.
+    subject_token = resource2.Header('X-Subject-Token')
+
+    def get_user_token_by_admin(self, session, user_id,
+                                tenant_id=None, no_catalog=True):
+        """Obtain a user token by SSS on behalf
+
+        :param session: The session to use for making this request.
+        :type session: :class:`~ecl.session.Session`
+        :param user_id: ID of a user
+        :param tenant_id: ID of a tenant
+        :param bool no_catalog: Exclude the service catalog from the response.
+        :return: :class:`~ecl.sss.v2.token.Token`
+        """
+        url = '%s/%s' % (self.base_path, user_id)
+        if no_catalog:
+            url += '?nocatalog=true'
+        body = {"tenant_id": tenant_id} if tenant_id else {}
+
+        resp = session.post(url, endpoint_filter=self.service, json=body)
+        self._translate_response(resp, has_body=True)
         return self
```

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_availability_zone.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_chassis.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_chassis.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_flavor.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_flavor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_keypair.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_keypair.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_limits.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_limits.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_metadata.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_metadata.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_nic_ports.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_nic_ports.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_server.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_server.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_server_action.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_server_action.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_stock.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_stock.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_uefi.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_uefi.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/baremetal/test_version.py` & `eclsdk-1.3.0/ecl/tests/functional/baremetal/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/base.py` & `eclsdk-1.3.0/ecl/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_metadata.py` & `eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_metadata.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_quota.py` & `eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_quota.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_type.py` & `eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/block_store/v2/test_volume.py` & `eclsdk-1.3.0/ecl/tests/functional/block_store/v2/test_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_extension.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_flavor.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_flavor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_image.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_image.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_keypair.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_keypair.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_limits.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_quota.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_quota.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_server.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_server.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/compute/v2/test_volume.py` & `eclsdk-1.3.0/ecl/tests/functional/compute/v2/test_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_cic.py` & `eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_cic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_eic.py` & `eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_eic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_mcic.py` & `eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_mcic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_meic.py` & `eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_meic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/connectivity/v1/test_operation.py` & `eclsdk-1.3.0/ecl/tests/functional/connectivity/v1/test_operation.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/dns/test_recordset.py` & `eclsdk-1.3.0/ecl/tests/functional/dns/test_recordset.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/dns/test_zone.py` & `eclsdk-1.3.0/ecl/tests/functional/dns/test_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/image/v2/test_image.py` & `eclsdk-1.3.0/ecl/tests/functional/image/v2/test_image.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/image/v2/test_image_copy.py` & `eclsdk-1.3.0/ecl/tests/functional/image/v2/test_image_copy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/image/v2/test_license.py` & `eclsdk-1.3.0/ecl/tests/functional/image/v2/test_license.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/image/v2/test_member.py` & `eclsdk-1.3.0/ecl/tests/functional/image/v2/test_member.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/image/v2/test_schema.py` & `eclsdk-1.3.0/ecl/tests/functional/image/v2/test_schema.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/image/v2/test_tag.py` & `eclsdk-1.3.0/ecl/tests/functional/image/v2/test_tag.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_extension.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall_action.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall_action.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall_interface.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_firewall_plan.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_firewall_plan.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_gwif.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_gwif.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_interdc.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_interdc.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_internet.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_internet.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer_action.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer_action.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer_interface.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_load_balancer_plan.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_load_balancer_plan.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_network.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_network.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_port.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_port.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_publicip.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_publicip.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_qos_option.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_qos_option.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_query_string.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_query_string.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_quota.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_quota.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_reserved_address.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_reserved_address.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_staticroute.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_staticroute.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_subnet.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_subnet.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/network/v2/test_vpn.py` & `eclsdk-1.3.0/ecl/tests/functional/network/v2/test_vpn.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/rca/v1/test_user.py` & `eclsdk-1.3.0/ecl/tests/functional/rca/v1/test_user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/rca/v1/test_version.py` & `eclsdk-1.3.0/ecl/tests/functional/rca/v1/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_api_key.py` & `eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_api_key.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_channel.py` & `eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_channel.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_contract.py` & `eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_contract.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_role.py` & `eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_role.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_tenant.py` & `eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_tenant.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/sss/v1/test_user.py` & `eclsdk-1.3.0/ecl/tests/functional/sss/v1/test_user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_av_zone.py` & `eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_av_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_version.py` & `eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_virtual_storage.py` & `eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_virtual_storage.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_volume.py` & `eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/storage/v1/test_volume_type.py` & `eclsdk-1.3.0/ecl/tests/functional/storage/v1/test_volume_type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_alarm.py` & `eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_alarm.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_alarm_change.py` & `eclsdk-1.3.0/ecl/tests/unit/fakes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,37 @@
+# Copyright 2010-2011 OpenStack Foundation
+# Copyright (c) 2013 Hewlett-Packard Development Company, L.P.
+#
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import unittest
-import uuid
+import mock
+
+
+class FakeTransport(mock.Mock):
+    RESPONSE = mock.Mock('200 OK')
+
+    def __init__(self):
+        super(FakeTransport, self).__init__()
+        self.request = mock.Mock()
+        self.request.return_value = self.RESPONSE
 
-from ecl.tests.functional import base
 
+class FakeAuthenticator(mock.Mock):
+    TOKEN = 'fake_token'
+    ENDPOINT = 'http://www.example.com/endpoint'
 
-@unittest.skip("bug/1524468")
-@unittest.skipUnless(base.service_exists(service_type="metering"),
-                     "Metering service does not exist")
-class TestAlarmChange(base.BaseFunctionalTest):
-
-    NAME = uuid.uuid4().hex
-    alarm = None
-
-    @classmethod
-    def setUpClass(cls):
-        super(TestAlarmChange, cls).setUpClass()
-        meter = next(cls.conn.telemetry.meters())
-        alarm = cls.conn.telemetry.create_alarm(
-            name=cls.NAME,
-            type='threshold',
-            threshold_rule={
-                'meter_name': meter.name,
-                'threshold': 1.1,
-            },
-        )
-        cls.alarm = alarm
-
-    @classmethod
-    def tearDownClass(cls):
-        cls.conn.telemetry.delete_alarm(cls.alarm, ignore_missing=False)
-
-    def test_list(self):
-        change = next(self.conn.telemetry.alarm_changes(self.alarm))
-        self.assertEqual(self.alarm.id, change.alarm_id)
-        self.assertEqual('creation', change.type)
+    def __init__(self):
+        super(FakeAuthenticator, self).__init__()
+        self.get_token = mock.Mock()
+        self.get_token.return_value = self.TOKEN
+        self.get_endpoint = mock.Mock()
+        self.get_endpoint.return_value = self.ENDPOINT
```

### Comparing `eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_capability.py` & `eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_capability.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_resource.py` & `eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_resource.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_sample.py` & `eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_sample.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/functional/telemetry/v2/test_statistics.py` & `eclsdk-1.3.0/ecl/tests/functional/telemetry/v2/test_statistics.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/test_baremetal_service.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/test_baremetal_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_availability_zone.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_charssis.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_charssis.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_flavor.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_flavor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_keypair.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_keypair.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_limits.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/baremetal/v2/test_uefi.py` & `eclsdk-1.3.0/ecl/tests/unit/baremetal/v2/test_uefi.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/base.py` & `eclsdk-1.3.0/ecl/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/block_store/test_block_store_service.py` & `eclsdk-1.3.0/ecl/tests/unit/block_store/test_block_store_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_snapshot.py` & `eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_type.py` & `eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/block_store/v2/test_volume.py` & `eclsdk-1.3.0/ecl/tests/unit/block_store/v2/test_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/test_compute_service.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/test_compute_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_availability_zone.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_extension.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_flavor.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_flavor.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_image.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_image.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_keypair.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_keypair.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_limits.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_metadata.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_metadata.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_server.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_server.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_server_interface.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_server_interface.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/compute/v2/test_volume.py` & `eclsdk-1.3.0/ecl/tests/unit/compute/v2/test_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/connectivity/test_connectivity_service.py` & `eclsdk-1.3.0/ecl/tests/unit/connectivity/test_connectivity_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/connectivity/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/connectivity/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/test_cic.py` & `eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/test_cic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/test_mcic.py` & `eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/test_mcic.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/connectivity/v1/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/connectivity/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/test_identity_service.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/test_identity_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_extension.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_role.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_role.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_tenant.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_tenant.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v2/test_user.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v2/test_user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_credential.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_credential.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_domain.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_domain.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_endpoint.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_group.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_group.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_policy.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_policy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_project.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_project.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_region.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_region.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_service.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_trust.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_trust.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/identity/v3/test_user.py` & `eclsdk-1.3.0/ecl/tests/unit/identity/v3/test_user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/image/test_image_service.py` & `eclsdk-1.3.0/ecl/tests/unit/image/test_image_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/image/v2/test_image.py` & `eclsdk-1.3.0/ecl/tests/unit/image/v2/test_image.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/image/v2/test_member.py` & `eclsdk-1.3.0/ecl/tests/unit/image/v2/test_member.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/image/v2/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/image/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/test_network_service.py` & `eclsdk-1.3.0/ecl/tests/unit/network/test_network_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/network/test_version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_extension.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_extension.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_load_balancer.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_load_balancer.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_network.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_network.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_port.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_port.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_quota.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_quota.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     "interdc_gateway": 1,
     "internet_gateway": 1,
     "load_balancer": 2,
     "network": 2,
     "port": 30,
     "subnet": 5,
     "tenant_id": IDENTIFIER,
-    "vpn_gateway": 1
+    "vpn_gateway": 1,
+    "security_group": 1,
+    "fic_gateway": 1,
+    "mec_gateway": 1
 }
 
 
 
 class TestQuota(testtools.TestCase):
 
     def test_basic(self):
@@ -56,14 +59,17 @@
         self.assertEqual(EXAMPLE['interdc_gateway'], sot.internet_gateway)
         self.assertEqual(EXAMPLE['load_balancer'], sot.load_balancer)
         self.assertEqual(EXAMPLE['network'], sot.networks)
         self.assertEqual(EXAMPLE['port'], sot.ports)
         self.assertEqual(EXAMPLE['subnet'], sot.subnets)
         self.assertEqual(EXAMPLE['tenant_id'], sot.project_id)
         self.assertEqual(EXAMPLE['vpn_gateway'], sot.vpn_gateway)
+        self.assertEqual(EXAMPLE['security_group'], sot.security_group)
+        self.assertEqual(EXAMPLE['fic_gateway'], sot.fic_gateway)
+        self.assertEqual(EXAMPLE['mec_gateway'], sot.mec_gateway)
 
 class TestQuotaDefault(testtools.TestCase):
 
     def test_basic(self):
         default = quota.QuotaDefault()
         self.assertEqual('quota', default.resource_key)
         self.assertEqual('quotas', default.resources_key)
@@ -85,7 +91,10 @@
         self.assertEqual(EXAMPLE['interdc_gateway'], default.internet_gateway)
         self.assertEqual(EXAMPLE['load_balancer'], default.load_balancer)
         self.assertEqual(EXAMPLE['network'], default.networks)
         self.assertEqual(EXAMPLE['port'], default.ports)
         self.assertEqual(EXAMPLE['subnet'], default.subnets)
         self.assertEqual(EXAMPLE['tenant_id'], default.project_id)
         self.assertEqual(EXAMPLE['vpn_gateway'], default.vpn_gateway)
+        self.assertEqual(EXAMPLE['security_group'], default.security_group)
+        self.assertEqual(EXAMPLE['fic_gateway'], default.fic_gateway)
+        self.assertEqual(EXAMPLE['mec_gateway'], default.mec_gateway)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_subnet.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_subnet.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/network/v2/test_vpn_service.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_vpn_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/orchestration/test_orchestration_service.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/test_telemetry_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import testtools
 
-from ecl.orchestration import orchestration_service
+from ecl.telemetry import telemetry_service
 
 
-class TestOrchestrationService(testtools.TestCase):
+class TestTelemetryService(testtools.TestCase):
 
     def test_service(self):
-        sot = orchestration_service.OrchestrationService()
-        self.assertEqual('orchestration', sot.service_type)
+        sot = telemetry_service.TelemetryService()
+        self.assertEqual('metering', sot.service_type)
         self.assertEqual('public', sot.interface)
         self.assertIsNone(sot.region)
         self.assertIsNone(sot.service_name)
         self.assertEqual(1, len(sot.valid_versions))
-        self.assertEqual('v1', sot.valid_versions[0].module)
-        self.assertEqual('v1', sot.valid_versions[0].path)
-        self.assertTrue(sot.requires_project_id)
+        self.assertEqual('v2', sot.valid_versions[0].module)
+        self.assertEqual('v2', sot.valid_versions[0].path)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/orchestration/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/test_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import testtools
 
-from ecl.orchestration import version
+from ecl.storage import version
 
-IDENTIFIER = 'IDENTIFIER'
+IDENTIFIER = 'v1.0'
 EXAMPLE = {
     'id': IDENTIFIER,
-    'links': '2',
-    'status': '3',
+    'media-types': {
+        'base': 'application/json',
+        'type': 'application/vnd.openstack.volume+json;version=1'
+    },
+    'updated': '2012-01-04T11:33:21Z',
+    'status': 'CURRENT'
 }
 
 
 class TestVersion(testtools.TestCase):
 
     def test_basic(self):
         sot = version.Version()
         self.assertEqual('version', sot.resource_key)
         self.assertEqual('versions', sot.resources_key)
         self.assertEqual('/', sot.base_path)
-        self.assertEqual('orchestration', sot.service.service_type)
+        self.assertEqual('storage', sot.service.service_type)
         self.assertFalse(sot.allow_create)
-        self.assertFalse(sot.allow_retrieve)
+        self.assertTrue(sot.allow_get)
         self.assertFalse(sot.allow_update)
         self.assertFalse(sot.allow_delete)
         self.assertTrue(sot.allow_list)
 
     def test_make_it(self):
-        sot = version.Version(EXAMPLE)
+        sot = version.Version(**EXAMPLE)
         self.assertEqual(EXAMPLE['id'], sot.id)
-        self.assertEqual(EXAMPLE['links'], sot.links)
+        self.assertEqual(EXAMPLE['media-types'], sot.media_types)
+        self.assertEqual(EXAMPLE['updated'], sot.updated)
         self.assertEqual(EXAMPLE['status'], sot.status)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_resource.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_resource.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,58 +8,51 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import testtools
 
-from ecl.orchestration.v1 import resource
+from ecl.telemetry.v2 import resource
 
-
-FAKE_ID = '32e39358-2422-4ad0-a1b5-dd60696bf564'
-FAKE_NAME = 'test_stack'
-FAKE = {
-    'links': [{
-        'href': 'http://res_link',
-        'rel': 'self'
-    }, {
-        'href': 'http://stack_link',
-        'rel': 'stack'
-    }],
-    'logical_resource_id': 'the_resource',
-    'name': 'the_resource',
-    'physical_resource_id': '9f38ab5a-37c8-4e40-9702-ce27fc5f6954',
-    'required_by': [],
-    'resource_type': 'OS::Heat::FakeResource',
-    'status': 'CREATE_COMPLETE',
-    'status_reason': 'state changed',
-    'updated_time': '2015-03-09T12:15:57.233772',
+IDENTIFIER = 'IDENTIFIER'
+LINKS = [{'href': 'first_uri', 'rel': 'label 1', },
+         {'href': 'other_uri', 'rel': 'label', }, ]
+EXAMPLE = {
+    'resource_id': IDENTIFIER,
+    'first_sample_timestamp': '2015-03-09T12:15:57.233772',
+    'last_sample_timestamp': '2015-03-09T12:15:57.233772',
+    'links': LINKS,
+    'metadata': {'name_one': '1', 'name_two': '2', },
+    'project_id': '123',
+    'source': 'abc',
+    'user_id': '789'
 }
 
 
 class TestResource(testtools.TestCase):
 
     def test_basic(self):
-        sot = resource.Resource()
-        self.assertEqual('resource', sot.resource_key)
-        self.assertEqual('resources', sot.resources_key)
-        self.assertEqual('/stacks/%(stack_name)s/%(stack_id)s/resources',
-                         sot.base_path)
-        self.assertEqual('orchestration', sot.service.service_type)
+        sot = resource.Resource(EXAMPLE)
+        self.assertIsNone(sot.resource_key)
+        self.assertIsNone(sot.resources_key)
+        self.assertEqual('/resources', sot.base_path)
+        self.assertEqual('metering', sot.service.service_type)
         self.assertFalse(sot.allow_create)
-        self.assertFalse(sot.allow_retrieve)
+        self.assertTrue(sot.allow_retrieve)
         self.assertFalse(sot.allow_update)
         self.assertFalse(sot.allow_delete)
         self.assertTrue(sot.allow_list)
 
     def test_make_it(self):
-        sot = resource.Resource(**FAKE)
-        self.assertEqual(FAKE['links'], sot.links)
-        self.assertEqual(FAKE['logical_resource_id'], sot.logical_resource_id)
-        self.assertEqual(FAKE['name'], sot.name)
-        self.assertEqual(FAKE['physical_resource_id'],
-                         sot.physical_resource_id)
-        self.assertEqual(FAKE['required_by'], sot.required_by)
-        self.assertEqual(FAKE['resource_type'], sot.resource_type)
-        self.assertEqual(FAKE['status'], sot.status)
-        self.assertEqual(FAKE['status_reason'], sot.status_reason)
-        self.assertEqual(FAKE['updated_time'], sot.updated_at)
+        sot = resource.Resource(EXAMPLE)
+        self.assertEqual(EXAMPLE['resource_id'], sot.id)
+        self.assertEqual(EXAMPLE['first_sample_timestamp'],
+                         sot.first_sample_at)
+        self.assertEqual(EXAMPLE['last_sample_timestamp'],
+                         sot.last_sample_at)
+        self.assertEqual(EXAMPLE['links'], sot.links)
+        self.assertEqual(EXAMPLE['metadata'], sot.metadata)
+        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
+        self.assertEqual(EXAMPLE['resource_id'], sot.resource_id)
+        self.assertEqual(EXAMPLE['source'], sot.source)
+        self.assertEqual(EXAMPLE['user_id'], sot.user_id)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/orchestration/v1/test_software_config.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/test_sss_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,48 +8,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import testtools
 
-from ecl.orchestration.v1 import software_config
+from ecl.sss import sss_service
 
 
-FAKE_ID = 'ce8ae86c-9810-4cb1-8888-7fb53bc523bf'
-FAKE_NAME = 'test_software_config'
-FAKE = {
-    'id': FAKE_ID,
-    'name': FAKE_NAME,
-    'config': 'fake config',
-    'creation_time': '2015-03-09T12:15:57',
-    'group': 'fake group',
-    'inputs': [{'foo': 'bar'}],
-    'outputs': [{'baz': 'zoo'}],
-    'options': {'key': 'value'},
-}
-
-
-class TestSoftwareConfig(testtools.TestCase):
-
-    def test_basic(self):
-        sot = software_config.SoftwareConfig()
-        self.assertEqual('software_config', sot.resource_key)
-        self.assertEqual('software_configs', sot.resources_key)
-        self.assertEqual('/software_configs', sot.base_path)
-        self.assertEqual('orchestration', sot.service.service_type)
-        self.assertTrue(sot.allow_create)
-        self.assertTrue(sot.allow_get)
-        self.assertFalse(sot.allow_update)
-        self.assertTrue(sot.allow_delete)
-        self.assertTrue(sot.allow_list)
-
-    def test_make_it(self):
-        sot = software_config.SoftwareConfig(**FAKE)
-        self.assertEqual(FAKE_ID, sot.id)
-        self.assertEqual(FAKE_NAME, sot.name)
-        self.assertEqual(FAKE['config'], sot.config)
-        self.assertEqual(FAKE['creation_time'], sot.created_at)
-        self.assertEqual(FAKE['group'], sot.group)
-        self.assertEqual(FAKE['inputs'], sot.inputs)
-        self.assertEqual(FAKE['outputs'], sot.outputs)
-        self.assertEqual(FAKE['options'], sot.options)
+class TestSSSService(testtools.TestCase):
+
+    def test_service(self):
+        sot = sss_service.SssService()
+        self.assertEqual('sssv2', sot.service_type)
+        self.assertEqual('public', sot.interface)
+        self.assertIsNone(sot.region)
+        self.assertIsNone(sot.service_name)
+        self.assertEqual(1, len(sot.valid_versions))
+        self.assertEqual('v2', sot.valid_versions[0].module)
+        self.assertEqual('v2', sot.valid_versions[0].path)
+
+
+class TestSSSAdminService(testtools.TestCase):
+
+    def test_service(self):
+        sot = sss_service.SssAdminService()
+        self.assertEqual('sssv2', sot.service_type)
+        self.assertEqual('admin', sot.interface)
+        self.assertIsNone(sot.region)
+        self.assertIsNone(sot.service_name)
+        self.assertEqual(1, len(sot.valid_versions))
+        self.assertEqual('v2', sot.valid_versions[0].module)
+        self.assertEqual('v2', sot.valid_versions[0].path)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/test_provider_connectivity_service.py` & `eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/test_provider_connectivity_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_address_assignment.py` & `eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_address_assignment.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection.py` & `eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection_request.py` & `eclsdk-1.3.0/ecl/tests/unit/provider_connectivity/v1/test_tenant_connection_request.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_api_key.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_api_key.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_channel.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_channel.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_contract.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_contract.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_role.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_role.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_tenant.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_tenant.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/sss/v1/test_user.py` & `eclsdk-1.3.0/ecl/tests/unit/sss/v1/test_user.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/test_storage_service.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/test_storage_service.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/test_version.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_mec_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,41 +8,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import testtools
 
-from ecl.storage import version
+from ecl.network.v2 import mec
 
-IDENTIFIER = 'v1.0'
 EXAMPLE = {
-    'id': IDENTIFIER,
-    'media-types': {
-        'base': 'application/json',
-        'type': 'application/vnd.openstack.volume+json;version=1'
-    },
-    'updated': '2012-01-04T11:33:21Z',
-    'status': 'CURRENT'
+    "description": "Example service 1 description.",
+    "id": "id12345678900",
+    "name": "Example port 1",
+    "tenant_id": "IDENTIFIER",
+    "zone": "Name",
 }
 
 
-class TestVersion(testtools.TestCase):
+class TestPort(testtools.TestCase):
 
     def test_basic(self):
-        sot = version.Version()
-        self.assertEqual('version', sot.resource_key)
-        self.assertEqual('versions', sot.resources_key)
-        self.assertEqual('/', sot.base_path)
-        self.assertEqual('storage', sot.service.service_type)
-        self.assertFalse(sot.allow_create)
+        sot = mec.MECService()
+        self.assertEqual('mec_service', sot.resource_key)
+        self.assertEqual('mec_services', sot.resources_key)
+        self.assertEqual('/v2.0/mec_services', sot.base_path)
+        self.assertEqual('network', sot.service.service_type)
         self.assertTrue(sot.allow_get)
-        self.assertFalse(sot.allow_update)
-        self.assertFalse(sot.allow_delete)
         self.assertTrue(sot.allow_list)
 
     def test_make_it(self):
-        sot = version.Version(**EXAMPLE)
+        sot = mec.MECService(**EXAMPLE)
+        self.assertEqual(EXAMPLE['description'], sot.description)
         self.assertEqual(EXAMPLE['id'], sot.id)
-        self.assertEqual(EXAMPLE['media-types'], sot.media_types)
-        self.assertEqual(EXAMPLE['updated'], sot.updated)
-        self.assertEqual(EXAMPLE['status'], sot.status)
+        self.assertEqual(EXAMPLE['name'], sot.name)
+        self.assertEqual(EXAMPLE['zone'], sot.zone)
+        self.assertEqual(EXAMPLE['tenant_id'], sot.tenant_id)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_availability_zone.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_snapshot.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_storage.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_storage.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_volume.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_volume.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/storage/v1/test_volume_type.py` & `eclsdk-1.3.0/ecl/tests/unit/storage/v1/test_volume_type.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_alarm.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_alarm.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_alarm_change.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_alarm_change.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_capability.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_capability.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_meter.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_meter.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_resource.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_statistics.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,53 +6,77 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+import mock
 import testtools
 
-from ecl.telemetry.v2 import resource
+from ecl.telemetry.v2 import statistics
 
-IDENTIFIER = 'IDENTIFIER'
-LINKS = [{'href': 'first_uri', 'rel': 'label 1', },
-         {'href': 'other_uri', 'rel': 'label', }, ]
 EXAMPLE = {
-    'resource_id': IDENTIFIER,
-    'first_sample_timestamp': '2015-03-09T12:15:57.233772',
-    'last_sample_timestamp': '2015-03-09T12:15:57.233772',
-    'links': LINKS,
-    'metadata': {'name_one': '1', 'name_two': '2', },
-    'project_id': '123',
-    'source': 'abc',
-    'user_id': '789'
+    'aggregate': '1',
+    'avg': '2',
+    'count': '3',
+    'duration': '4',
+    'duration_end': '2015-03-09T12:45:00.000000',
+    'duration_start': '2015-03-09T12:15:00.000000',
+    'groupby': '7',
+    'max': '8',
+    'min': '9',
+    'period': '10',
+    'period_end': '2015-03-09T12:45:00.000000',
+    'period_start': '2015-03-09T12:15:00.000000',
+    'sum': '13',
+    'unit': '14',
 }
 
 
-class TestResource(testtools.TestCase):
+class TestStatistics(testtools.TestCase):
 
     def test_basic(self):
-        sot = resource.Resource(EXAMPLE)
-        self.assertIsNone(sot.resource_key)
+        sot = statistics.Statistics()
+        self.assertEqual('statistics', sot.resource_key)
         self.assertIsNone(sot.resources_key)
-        self.assertEqual('/resources', sot.base_path)
+        self.assertEqual('/meters/%(meter_name)s/statistics', sot.base_path)
         self.assertEqual('metering', sot.service.service_type)
         self.assertFalse(sot.allow_create)
-        self.assertTrue(sot.allow_retrieve)
+        self.assertFalse(sot.allow_retrieve)
         self.assertFalse(sot.allow_update)
         self.assertFalse(sot.allow_delete)
         self.assertTrue(sot.allow_list)
 
     def test_make_it(self):
-        sot = resource.Resource(EXAMPLE)
-        self.assertEqual(EXAMPLE['resource_id'], sot.id)
-        self.assertEqual(EXAMPLE['first_sample_timestamp'],
-                         sot.first_sample_at)
-        self.assertEqual(EXAMPLE['last_sample_timestamp'],
-                         sot.last_sample_at)
-        self.assertEqual(EXAMPLE['links'], sot.links)
-        self.assertEqual(EXAMPLE['metadata'], sot.metadata)
-        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
-        self.assertEqual(EXAMPLE['resource_id'], sot.resource_id)
-        self.assertEqual(EXAMPLE['source'], sot.source)
-        self.assertEqual(EXAMPLE['user_id'], sot.user_id)
+        sot = statistics.Statistics(EXAMPLE)
+        self.assertIsNone(sot.id)
+        self.assertEqual(EXAMPLE['aggregate'], sot.aggregate)
+        self.assertEqual(EXAMPLE['avg'], sot.avg)
+        self.assertEqual(EXAMPLE['count'], sot.count)
+        self.assertEqual(EXAMPLE['duration'], sot.duration)
+        self.assertEqual(EXAMPLE['duration_end'], sot.duration_end_at)
+        self.assertEqual(EXAMPLE['duration_start'], sot.duration_start_at)
+        self.assertEqual(EXAMPLE['groupby'], sot.group_by)
+        self.assertEqual(EXAMPLE['max'], sot.max)
+        self.assertEqual(EXAMPLE['min'], sot.min)
+        self.assertEqual(EXAMPLE['period'], sot.period)
+        self.assertEqual(EXAMPLE['period_end'], sot.period_end_at)
+        self.assertEqual(EXAMPLE['period_start'], sot.period_start_at)
+        self.assertEqual(EXAMPLE['sum'], sot.sum)
+        self.assertEqual(EXAMPLE['unit'], sot.unit)
+
+    def test_list(self):
+        sess = mock.Mock()
+        resp = mock.Mock()
+        resp.json = mock.Mock(return_value=[EXAMPLE])
+        sess.get = mock.Mock(return_value=resp)
+
+        args = {'meter_name': 'example'}
+        reply = statistics.Statistics.list(sess, path_args=args)
+
+        url = '/meters/example/statistics'
+        stat = next(reply)
+        sess.get.assert_called_with(url, endpoint_filter=stat.service,
+                                    params={})
+        self.assertEqual(EXAMPLE, stat)
+        self.assertRaises(StopIteration, next, reply)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_sample.py` & `eclsdk-1.3.0/ecl/tests/unit/telemetry/v2/test_sample.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/telemetry/v2/test_statistics.py` & `eclsdk-1.3.0/ecl/tests/unit/network/v2/test_mec_gateway.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,77 +6,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import mock
 import testtools
 
-from ecl.telemetry.v2 import statistics
+from ecl.network.v2 import mec
 
 EXAMPLE = {
-    'aggregate': '1',
-    'avg': '2',
-    'count': '3',
-    'duration': '4',
-    'duration_end': '2015-03-09T12:45:00.000000',
-    'duration_start': '2015-03-09T12:15:00.000000',
-    'groupby': '7',
-    'max': '8',
-    'min': '9',
-    'period': '10',
-    'period_end': '2015-03-09T12:45:00.000000',
-    'period_start': '2015-03-09T12:15:00.000000',
-    'sum': '13',
-    'unit': '14',
+    "description": "Example gateway 1 description.",
+    "id": "id12345678900",
+    "name": "Example port 1",
+    "qos_option_id": "qosid12345678",
+    "tenant_id": "IDENTIFIER",
+    "status": "ACTIVE",
+    "mec_service_id": "mecsid12345678",
 }
 
 
-class TestStatistics(testtools.TestCase):
+class TestPort(testtools.TestCase):
 
     def test_basic(self):
-        sot = statistics.Statistics()
-        self.assertEqual('statistics', sot.resource_key)
-        self.assertIsNone(sot.resources_key)
-        self.assertEqual('/meters/%(meter_name)s/statistics', sot.base_path)
-        self.assertEqual('metering', sot.service.service_type)
-        self.assertFalse(sot.allow_create)
-        self.assertFalse(sot.allow_retrieve)
-        self.assertFalse(sot.allow_update)
-        self.assertFalse(sot.allow_delete)
+        sot = mec.MECGateway()
+        self.assertEqual('mec_gateway', sot.resource_key)
+        self.assertEqual('mec_gateways', sot.resources_key)
+        self.assertEqual('/v2.0/mec_gateways', sot.base_path)
+        self.assertEqual('network', sot.service.service_type)
+        self.assertTrue(sot.allow_get)
         self.assertTrue(sot.allow_list)
 
     def test_make_it(self):
-        sot = statistics.Statistics(EXAMPLE)
-        self.assertIsNone(sot.id)
-        self.assertEqual(EXAMPLE['aggregate'], sot.aggregate)
-        self.assertEqual(EXAMPLE['avg'], sot.avg)
-        self.assertEqual(EXAMPLE['count'], sot.count)
-        self.assertEqual(EXAMPLE['duration'], sot.duration)
-        self.assertEqual(EXAMPLE['duration_end'], sot.duration_end_at)
-        self.assertEqual(EXAMPLE['duration_start'], sot.duration_start_at)
-        self.assertEqual(EXAMPLE['groupby'], sot.group_by)
-        self.assertEqual(EXAMPLE['max'], sot.max)
-        self.assertEqual(EXAMPLE['min'], sot.min)
-        self.assertEqual(EXAMPLE['period'], sot.period)
-        self.assertEqual(EXAMPLE['period_end'], sot.period_end_at)
-        self.assertEqual(EXAMPLE['period_start'], sot.period_start_at)
-        self.assertEqual(EXAMPLE['sum'], sot.sum)
-        self.assertEqual(EXAMPLE['unit'], sot.unit)
-
-    def test_list(self):
-        sess = mock.Mock()
-        resp = mock.Mock()
-        resp.json = mock.Mock(return_value=[EXAMPLE])
-        sess.get = mock.Mock(return_value=resp)
-
-        args = {'meter_name': 'example'}
-        reply = statistics.Statistics.list(sess, path_args=args)
-
-        url = '/meters/example/statistics'
-        stat = next(reply)
-        sess.get.assert_called_with(url, endpoint_filter=stat.service,
-                                    params={})
-        self.assertEqual(EXAMPLE, stat)
-        self.assertRaises(StopIteration, next, reply)
+        sot = mec.MECGateway(**EXAMPLE)
+        self.assertEqual(EXAMPLE['description'], sot.description)
+        self.assertEqual(EXAMPLE['id'], sot.id)
+        self.assertEqual(EXAMPLE['name'], sot.name)
+        self.assertEqual(EXAMPLE['qos_option_id'], sot.qos_option_id)
+        self.assertEqual(EXAMPLE['status'], sot.status)
+        self.assertEqual(EXAMPLE['tenant_id'], sot.tenant_id)
+        self.assertEqual(EXAMPLE['mec_service_id'], sot.mec_service_id)
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_connection.py` & `eclsdk-1.3.0/ecl/tests/unit/test_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,14 @@
                          conn.identity.__class__.__module__)
         self.assertEqual('ecl.image.v2._proxy',
                          conn.image.__class__.__module__)
         self.assertEqual('ecl.network.v2._proxy',
                          conn.network.__class__.__module__)
         self.assertEqual('ecl.rca.v1._proxy',
                          conn.rca.__class__.__module__)
-        self.assertEqual('ecl.orchestration.v1._proxy',
-                         conn.orchestration.__class__.__module__)
         self.assertEqual('ecl.telemetry.v2._proxy',
                          conn.telemetry.__class__.__module__)
         self.assertEqual('ecl.sss.v1._proxy',
                          conn.sss.__class__.__module__)
 
     def _prepare_test_config(self):
         # Create a temporary directory where our test config will live
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_exceptions.py` & `eclsdk-1.3.0/ecl/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_format.py` & `eclsdk-1.3.0/ecl/tests/unit/test_format.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_profile.py` & `eclsdk-1.3.0/ecl/tests/unit/test_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             'compute', 
             'dedicated-hypervisor',
             'identity',
             'image',
             'interconnectivity',
             'metering',
             'network',
-            'orchestration',
             'rca',
             'sss',
             'storage',
             'volumev2',
             ]
         self.assertEqual(expected, prof.service_keys)
 
@@ -41,15 +40,14 @@
         self.assertEqual('v2', prof.get_filter('compute').version)
         self.assertEqual('v1', prof.get_filter('dedicated-hypervisor').version)
         self.assertEqual('v3', prof.get_filter('identity').version)
         self.assertEqual('v2', prof.get_filter('image').version)
         self.assertEqual('v1', prof.get_filter('interconnectivity').version)
         self.assertEqual('v2', prof.get_filter('metering').version)
         self.assertEqual('v2', prof.get_filter('network').version)
-        self.assertEqual('v1', prof.get_filter('orchestration').version)
         self.assertEqual('v1', prof.get_filter('rca').version)
         self.assertEqual('v1', prof.get_filter('sss').version)
         self.assertEqual('v1', prof.get_filter('storage').version)
         self.assertEqual('v2', prof.get_filter('volumev2').version)
 
     def test_set(self):
         prof = profile.Profile()
@@ -65,16 +63,14 @@
         self.assertEqual('v5', prof.get_filter('image').version)
         prof.set_version('interconnectivity', 'v9')
         self.assertEqual('v9', prof.get_filter('interconnectivity').version)
         prof.set_version('metering', 'v6')
         self.assertEqual('v6', prof.get_filter('metering').version)
         prof.set_version('network', 'v7')
         self.assertEqual('v7', prof.get_filter('network').version)
-        prof.set_version('orchestration', 'v8')
-        self.assertEqual('v8', prof.get_filter('orchestration').version)
         prof.set_version('rca', 'v9')
         self.assertEqual('v9', prof.get_filter('rca').version)
         prof.set_version('sss', 'v10')
         self.assertEqual('v10', prof.get_filter('sss').version)
         prof.set_version('storage', 'v11')
         self.assertEqual('v11', prof.get_filter('storage').version)
         prof.set_version('volumev2', 'v12')
```

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_proxy.py` & `eclsdk-1.3.0/ecl/tests/unit/test_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_proxy2.py` & `eclsdk-1.3.0/ecl/tests/unit/test_proxy2.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_proxy_base.py` & `eclsdk-1.3.0/ecl/tests/unit/test_proxy_base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_proxy_base2.py` & `eclsdk-1.3.0/ecl/tests/unit/test_proxy_base2.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_resource.py` & `eclsdk-1.3.0/ecl/tests/unit/test_resource.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_resource2.py` & `eclsdk-1.3.0/ecl/tests/unit/test_resource2.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_service_filter.py` & `eclsdk-1.3.0/ecl/tests/unit/test_service_filter.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_session.py` & `eclsdk-1.3.0/ecl/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/tests/unit/test_utils.py` & `eclsdk-1.3.0/ecl/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/utils.py` & `eclsdk-1.3.0/ecl/utils.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/version.py` & `eclsdk-1.3.0/ecl/version.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/virtual_network_appliance/exceptions.py` & `eclsdk-1.3.0/ecl/virtual_network_appliance/exceptions.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/virtual_network_appliance/v1/_proxy.py` & `eclsdk-1.3.0/ecl/virtual_network_appliance/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/virtual_network_appliance/v1/base.py` & `eclsdk-1.3.0/ecl/virtual_network_appliance/v1/base.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/virtual_network_appliance/v1/operation.py` & `eclsdk-1.3.0/ecl/virtual_network_appliance/v1/operation.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/virtual_network_appliance/v1/virtual_network_appliance.py` & `eclsdk-1.3.0/ecl/virtual_network_appliance/v1/virtual_network_appliance.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/ecl/virtual_network_appliance/v1/virtual_network_appliance_plan.py` & `eclsdk-1.3.0/ecl/virtual_network_appliance/v1/virtual_network_appliance_plan.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/eclsdk.egg-info/PKG-INFO` & `eclsdk-1.3.0/eclsdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: eclsdk
-Version: 1.2.1
+Version: 1.3.0
 Summary: SDK for building applications to work with Enterprise Cloud 2.0
 Home-page: https://ecl.ntt.com
 Author: NTT Communications
 Author-email: ecl-cli-sdk@ntt.com
 License: Apache License, Version 2.0
+Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -68,7 +69,9 @@
 https://ecl.ntt.com
 
 License
 -------
 
 Apache 2.0
 
+
+
```

### Comparing `eclsdk-1.2.1/eclsdk.egg-info/SOURCES.txt` & `eclsdk-1.3.0/eclsdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -168,35 +168,26 @@
 ecl/network/v2/interdc.py
 ecl/network/v2/internet.py
 ecl/network/v2/load_balancer.py
 ecl/network/v2/load_balancer_action.py
 ecl/network/v2/load_balancer_interface.py
 ecl/network/v2/load_balancer_plan.py
 ecl/network/v2/load_balancer_syslog_server.py
+ecl/network/v2/mec.py
 ecl/network/v2/network.py
 ecl/network/v2/physical_port.py
 ecl/network/v2/port.py
 ecl/network/v2/publicip.py
 ecl/network/v2/qos_option.py
 ecl/network/v2/quota.py
 ecl/network/v2/reserved_address.py
 ecl/network/v2/static_route.py
 ecl/network/v2/subnet.py
 ecl/network/v2/tenant_connection.py
 ecl/network/v2/vpn.py
-ecl/orchestration/__init__.py
-ecl/orchestration/orchestration_service.py
-ecl/orchestration/version.py
-ecl/orchestration/v1/__init__.py
-ecl/orchestration/v1/_proxy.py
-ecl/orchestration/v1/resource.py
-ecl/orchestration/v1/software_config.py
-ecl/orchestration/v1/software_deployment.py
-ecl/orchestration/v1/stack.py
-ecl/orchestration/v1/template.py
 ecl/provider_connectivity/__init__.py
 ecl/provider_connectivity/exceptions.py
 ecl/provider_connectivity/provider_connectivity_service.py
 ecl/provider_connectivity/v1/__init__.py
 ecl/provider_connectivity/v1/_proxy.py
 ecl/provider_connectivity/v1/address_assignment.py
 ecl/provider_connectivity/v1/aws_connection.py
@@ -220,53 +211,70 @@
 ecl/rca/rca_service.py
 ecl/rca/version.py
 ecl/rca/v1/__init__.py
 ecl/rca/v1/_proxy.py
 ecl/rca/v1/user.py
 ecl/security_order/__init__.py
 ecl/security_order/security_order_service.py
-ecl/security_order/v2/__init__.py
-ecl/security_order/v2/_proxy.py
-ecl/security_order/v2/device.py
-ecl/security_order/v2/ha_device.py
-ecl/security_order/v2/host_based_security.py
-ecl/security_order/v2/waf.py
+ecl/security_order/v3/__init__.py
+ecl/security_order/v3/_proxy.py
+ecl/security_order/v3/device.py
+ecl/security_order/v3/ha_device.py
+ecl/security_order/v3/host_based_security.py
+ecl/security_order/v3/waf.py
 ecl/security_order_v1/__init__.py
 ecl/security_order_v1/security_order_service.py
 ecl/security_order_v1/v1/__init__.py
 ecl/security_order_v1/v1/_proxy.py
 ecl/security_order_v1/v1/device.py
 ecl/security_order_v1/v1/ha_device.py
 ecl/security_order_v1/v1/host_based_security.py
 ecl/security_order_v1/v1/waf.py
+ecl/security_order_v2/__init__.py
+ecl/security_order_v2/security_order_service.py
+ecl/security_order_v2/v2/__init__.py
+ecl/security_order_v2/v2/_proxy.py
+ecl/security_order_v2/v2/device.py
+ecl/security_order_v2/v2/ha_device.py
+ecl/security_order_v2/v2/host_based_security.py
+ecl/security_order_v2/v2/waf.py
 ecl/security_portal/__init__.py
 ecl/security_portal/security_portal_service.py
-ecl/security_portal/v2/__init__.py
-ecl/security_portal/v2/_proxy.py
-ecl/security_portal/v2/security_device.py
-ecl/security_portal/v2/security_device_interface.py
+ecl/security_portal/v3/__init__.py
+ecl/security_portal/v3/_proxy.py
+ecl/security_portal/v3/security_device.py
+ecl/security_portal/v3/security_device_interface.py
 ecl/security_portal_v1/__init__.py
 ecl/security_portal_v1/security_portal_service.py
 ecl/security_portal_v1/v1/__init__.py
 ecl/security_portal_v1/v1/_proxy.py
 ecl/security_portal_v1/v1/security_device.py
 ecl/security_portal_v1/v1/security_device_interface.py
+ecl/security_portal_v2/__init__.py
+ecl/security_portal_v2/security_portal_service.py
+ecl/security_portal_v2/v2/__init__.py
+ecl/security_portal_v2/v2/_proxy.py
+ecl/security_portal_v2/v2/security_device.py
+ecl/security_portal_v2/v2/security_device_interface.py
 ecl/sss/__init__.py
 ecl/sss/exceptions.py
 ecl/sss/sss_service.py
 ecl/sss/v1/__init__.py
 ecl/sss/v1/_proxy.py
 ecl/sss/v1/api_key.py
 ecl/sss/v1/channel.py
 ecl/sss/v1/contract.py
 ecl/sss/v1/iam_group.py
 ecl/sss/v1/iam_role.py
 ecl/sss/v1/role.py
 ecl/sss/v1/tenant.py
 ecl/sss/v1/user.py
+ecl/sss/v2/_proxy.py
+ecl/sss/v2/service_menu.py
+ecl/sss/v2/token.py
 ecl/storage/__init__.py
 ecl/storage/exceptions.py
 ecl/storage/storage_service.py
 ecl/storage/version.py
 ecl/storage/v1/__init__.py
 ecl/storage/v1/_proxy.py
 ecl/storage/v1/availability_zone.py
@@ -359,30 +367,29 @@
 ecl/tests/functional/network/v2/test_qos_option.py
 ecl/tests/functional/network/v2/test_query_string.py
 ecl/tests/functional/network/v2/test_quota.py
 ecl/tests/functional/network/v2/test_reserved_address.py
 ecl/tests/functional/network/v2/test_staticroute.py
 ecl/tests/functional/network/v2/test_subnet.py
 ecl/tests/functional/network/v2/test_vpn.py
-ecl/tests/functional/orchestration/__init__.py
-ecl/tests/functional/orchestration/v1/__init__.py
-ecl/tests/functional/orchestration/v1/hello_world.yaml
-ecl/tests/functional/orchestration/v1/test_stack.py
 ecl/tests/functional/rca/__init__.py
 ecl/tests/functional/rca/v1/__init__.py
 ecl/tests/functional/rca/v1/test_user.py
 ecl/tests/functional/rca/v1/test_version.py
 ecl/tests/functional/sss/__init__.py
 ecl/tests/functional/sss/v1/__init__.py
 ecl/tests/functional/sss/v1/test_api_key.py
 ecl/tests/functional/sss/v1/test_channel.py
 ecl/tests/functional/sss/v1/test_contract.py
 ecl/tests/functional/sss/v1/test_role.py
 ecl/tests/functional/sss/v1/test_tenant.py
 ecl/tests/functional/sss/v1/test_user.py
+ecl/tests/functional/sss/v2/__init__.py
+ecl/tests/functional/sss/v2/test_service_menu.py
+ecl/tests/functional/sss/v2/test_token.py
 ecl/tests/functional/storage/__init__.py
 ecl/tests/functional/storage/v1/__init__.py
 ecl/tests/functional/storage/v1/test_av_zone.py
 ecl/tests/functional/storage/v1/test_version.py
 ecl/tests/functional/storage/v1/test_virtual_storage.py
 ecl/tests/functional/storage/v1/test_volume.py
 ecl/tests/functional/storage/v1/test_volume_type.py
@@ -478,30 +485,23 @@
 ecl/tests/unit/image/v2/test_proxy.py
 ecl/tests/unit/network/__init__.py
 ecl/tests/unit/network/test_network_service.py
 ecl/tests/unit/network/test_version.py
 ecl/tests/unit/network/v2/__init__.py
 ecl/tests/unit/network/v2/test_extension.py
 ecl/tests/unit/network/v2/test_load_balancer.py
+ecl/tests/unit/network/v2/test_mec_gateway.py
+ecl/tests/unit/network/v2/test_mec_interface.py
+ecl/tests/unit/network/v2/test_mec_service.py
 ecl/tests/unit/network/v2/test_network.py
 ecl/tests/unit/network/v2/test_port.py
 ecl/tests/unit/network/v2/test_proxy.py
 ecl/tests/unit/network/v2/test_quota.py
 ecl/tests/unit/network/v2/test_subnet.py
 ecl/tests/unit/network/v2/test_vpn_service.py
-ecl/tests/unit/orchestration/__init__.py
-ecl/tests/unit/orchestration/test_orchestration_service.py
-ecl/tests/unit/orchestration/test_version.py
-ecl/tests/unit/orchestration/v1/__init__.py
-ecl/tests/unit/orchestration/v1/test_proxy.py
-ecl/tests/unit/orchestration/v1/test_resource.py
-ecl/tests/unit/orchestration/v1/test_software_config.py
-ecl/tests/unit/orchestration/v1/test_software_deployment.py
-ecl/tests/unit/orchestration/v1/test_stack.py
-ecl/tests/unit/orchestration/v1/test_template.py
 ecl/tests/unit/provider_connectivity/__init__.py
 ecl/tests/unit/provider_connectivity/test_provider_connectivity_service.py
 ecl/tests/unit/provider_connectivity/v1/__init__.py
 ecl/tests/unit/provider_connectivity/v1/test_address_assignment.py
 ecl/tests/unit/provider_connectivity/v1/test_proxy.py
 ecl/tests/unit/provider_connectivity/v1/test_tenant_connection.py
 ecl/tests/unit/provider_connectivity/v1/test_tenant_connection_request.py
@@ -510,14 +510,17 @@
 ecl/tests/unit/sss/v1/__init__.py
 ecl/tests/unit/sss/v1/test_api_key.py
 ecl/tests/unit/sss/v1/test_channel.py
 ecl/tests/unit/sss/v1/test_contract.py
 ecl/tests/unit/sss/v1/test_role.py
 ecl/tests/unit/sss/v1/test_tenant.py
 ecl/tests/unit/sss/v1/test_user.py
+ecl/tests/unit/sss/v2/__init__.py
+ecl/tests/unit/sss/v2/test_service_menu.py
+ecl/tests/unit/sss/v2/test_token.py
 ecl/tests/unit/storage/__init__.py
 ecl/tests/unit/storage/test_storage_service.py
 ecl/tests/unit/storage/test_version.py
 ecl/tests/unit/storage/v1/__init__.py
 ecl/tests/unit/storage/v1/test_availability_zone.py
 ecl/tests/unit/storage/v1/test_snapshot.py
 ecl/tests/unit/storage/v1/test_storage.py
```

### Comparing `eclsdk-1.2.1/setup.cfg` & `eclsdk-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eclsdk
-version = 1.2.1
+version = 1.3.0
 summary = SDK for building applications to work with Enterprise Cloud 2.0
 description-file = 
 	README.rst
 license = Apache License, Version 2.0
 author = NTT Communications
 author-email = ecl-cli-sdk@ntt.com
 home-page = https://ecl.ntt.com
```

### Comparing `eclsdk-1.2.1/setup.py` & `eclsdk-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/test-requirements.txt` & `eclsdk-1.3.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `eclsdk-1.2.1/tox.ini` & `eclsdk-1.3.0/tox.ini`

 * *Files identical despite different names*

