# Comparing `tmp/rucio-clients-34.1.0.tar.gz` & `tmp/rucio_clients-34.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-clients-34.1.0.tar", last modified: Tue Apr  2 13:57:09 2024, max compression
+gzip compressed data, was "rucio_clients-34.2.0.tar", last modified: Tue Apr 16 10:35:08 2024, max compression
```

## Comparing `rucio-clients-34.1.0.tar` & `rucio_clients-34.2.0.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.809292 rucio-clients-34.1.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio-clients-34.1.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-clients-34.1.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-clients-34.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-02 13:57:06.000000 rucio-clients-34.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2024-04-02 13:57:09.809292 rucio-clients-34.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-04-02 11:45:19.000000 rucio-clients-34.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.757292 rucio-clients-34.1.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127075 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)   133531 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/bin/rucio-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.758292 rucio-clients-34.1.0/etc/
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-clients-34.1.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-clients-34.1.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-03-13 10:19:28.000000 rucio-clients-34.1.0/etc/rucio.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.754292 rucio-clients-34.1.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.759292 rucio-clients-34.1.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.766292 rucio-clients-34.1.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16353 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    47057 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86065 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27124 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12682 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46563 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.771292 rucio-clients-34.1.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2234 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24282 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     3300 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6291 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/didtype.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45297 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6056 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.774292 rucio-clients-34.1.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5152 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18523 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15885 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5069 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79094 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.774292 rucio-clients-34.1.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.780292 rucio-clients-34.1.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7198 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29093 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9680 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3409 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10394 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22650 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15256 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14651 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17467 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8127 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22166 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12567 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/rse/rsemanager.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-02 11:50:17.000000 rucio-clients-34.1.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1549 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.807292 rucio-clients-34.1.0/lib/rucio_clients.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5205 2024-04-02 13:57:09.000000 rucio-clients-34.1.0/lib/rucio_clients.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-clients-34.1.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-03-19 15:04:29.000000 rucio-clients-34.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-02 13:57:09.810292 rucio-clients-34.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-02 13:57:06.000000 rucio-clients-34.1.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.806292 rucio-clients-34.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     6929 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio-clients-34.1.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio-clients-34.1.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:09.806292 rucio-clients-34.1.0/tools/
--rw-r--r--   0 root         (0) root         (0)     6163 2024-03-21 13:32:51.000000 rucio-clients-34.1.0/tools/merge_rucio_configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.421055 rucio_clients-34.2.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio_clients-34.2.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-16 10:35:04.000000 rucio_clients-34.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-16 10:35:08.421055 rucio_clients-34.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-16 07:53:27.000000 rucio_clients-34.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.385055 rucio_clients-34.2.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127117 2024-04-09 08:44:02.000000 rucio_clients-34.2.0/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)   133531 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/bin/rucio-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.386055 rucio_clients-34.2.0/etc/
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-03-13 10:19:28.000000 rucio_clients-34.2.0/etc/rucio.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.383055 rucio_clients-34.2.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.387055 rucio_clients-34.2.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.391055 rucio_clients-34.2.0/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16353 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    47980 2024-04-08 15:35:56.000000 rucio_clients-34.2.0/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    86092 2024-04-08 15:35:57.000000 rucio_clients-34.2.0/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27124 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12682 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46563 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.394055 rucio_clients-34.2.0/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24284 2024-04-08 15:14:19.000000 rucio_clients-34.2.0/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6291 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/didtype.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45297 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6056 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.396055 rucio_clients-34.2.0/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5152 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    18523 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/cms.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)    15885 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/lsst.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5069 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79128 2024-04-08 15:14:19.000000 rucio_clients-34.2.0/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.396055 rucio_clients-34.2.0/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.400055 rucio_clients-34.2.0/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29093 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9680 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10394 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    22650 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14651 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17467 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8127 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22166 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12567 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37238 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/rsemanager.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-16 07:53:37.000000 rucio_clients-34.2.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-08 15:22:52.000000 rucio_clients-34.2.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.419055 rucio_clients-34.2.0/lib/rucio_clients.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5205 2024-04-16 10:35:08.000000 rucio_clients-34.2.0/lib/rucio_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio_clients-34.2.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-04-16 07:53:27.000000 rucio_clients-34.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-16 10:35:08.423055 rucio_clients-34.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-16 10:35:04.000000 rucio_clients-34.2.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.419055 rucio_clients-34.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-04-08 15:14:19.000000 rucio_clients-34.2.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.419055 rucio_clients-34.2.0/tools/
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tools/merge_rucio_configs.py
```

### Comparing `rucio-clients-34.1.0/AUTHORS.rst` & `rucio_clients-34.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/LICENSE` & `rucio_clients-34.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/MANIFEST.in` & `rucio_clients-34.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/PKG-INFO` & `rucio_clients-34.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-clients
-Version: 34.1.0
+Version: 34.2.0
 Summary: Rucio Client Lite Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-clients-34.1.0/README.rst` & `rucio_clients-34.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/bin/rucio` & `rucio_clients-34.2.0/bin/rucio`

 * *Files 0% similar despite different names*

```diff
@@ -1147,15 +1147,15 @@
     %(prog)s set_metadata [options] <field1=value1 field2=value2 ...>
 
     Set data identifier metadata
     """
     client = get_client(args)
     value = args.value
     if args.key == 'lifetime':
-        value = float(args.value)
+        value = None if args.value.lower() == 'none' else float(args.value)
     scope, name = get_scope(args.did, client)
     client.set_metadata(scope=scope, name=name, key=args.key, value=value)
     return SUCCESS
 
 
 @exception_handler
 def delete_metadata(args):
```

### Comparing `rucio-clients-34.1.0/bin/rucio-admin` & `rucio_clients-34.2.0/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/etc/rse-accounts.cfg.template` & `rucio_clients-34.2.0/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/etc/rucio.cfg.atlas.client.template` & `rucio_clients-34.2.0/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/etc/rucio.cfg.template` & `rucio_clients-34.2.0/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/__init__.py` & `rucio_clients-34.2.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/alembicrevision.py` & `rucio_clients-34.2.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/__init__.py` & `rucio_clients-34.2.0/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/accountclient.py` & `rucio_clients-34.2.0/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/accountlimitclient.py` & `rucio_clients-34.2.0/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/baseclient.py` & `rucio_clients-34.2.0/lib/rucio/client/baseclient.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,32 +15,35 @@
 '''
  Client class for callers of the Rucio system
 '''
 
 import errno
 import getpass
 import os
-import random
+import secrets
 import sys
 import time
 from configparser import NoOptionError, NoSectionError
+from logging import Logger
 from os import environ, fdopen, geteuid, makedirs, path
 from shutil import move
 from tempfile import mkstemp
+from typing import Any, Generator, Optional
 from urllib.parse import urlparse
 
+import requests
 from dogpile.cache import make_region
 from requests import Response, Session
 from requests.exceptions import ConnectionError
 from requests.status_codes import codes
 
 from rucio import version
 from rucio.common import exception
 from rucio.common.config import config_get, config_get_bool, config_get_int
-from rucio.common.exception import CannotAuthenticate, ClientProtocolNotSupported, MissingClientParameter, MissingModuleException, NoAuthInformation, ServerConnectionException
+from rucio.common.exception import CannotAuthenticate, ClientProtocolNotSupported, ConfigNotFound, MissingClientParameter, MissingModuleException, NoAuthInformation, ServerConnectionException
 from rucio.common.extra import import_extras
 from rucio.common.utils import build_url, get_tmp_dir, my_key_generator, parse_response, setup_logger, ssh_sign
 
 EXTRA_MODULES = import_extras(['requests_kerberos'])
 
 if EXTRA_MODULES['requests_kerberos']:
     from requests_kerberos import HTTPKerberosAuth  # pylint: disable=import-error
@@ -60,27 +63,37 @@
 def choice(hosts):
     """
     Select randomly a host
 
     :param hosts: Lost of hosts
     :return: A randomly selected host.
     """
-    return random.choice(hosts)
+    return secrets.choice(hosts)
 
 
 class BaseClient:
 
     """Main client class for accessing Rucio resources. Handles the authentication."""
 
     AUTH_RETRIES, REQUEST_RETRIES = 2, 3
     TOKEN_PATH_PREFIX = get_tmp_dir() + '/.rucio_'
     TOKEN_PREFIX = 'auth_token_'
     TOKEN_EXP_PREFIX = 'auth_token_exp_'
 
-    def __init__(self, rucio_host=None, auth_host=None, account=None, ca_cert=None, auth_type=None, creds=None, timeout=600, user_agent='rucio-clients', vo=None, logger=None):
+    def __init__(self,
+                 rucio_host: Optional[str] = None,
+                 auth_host: Optional[str] = None,
+                 account: Optional[str] = None,
+                 ca_cert: Optional[str] = None,
+                 auth_type: Optional[str] = None,
+                 creds: Optional[dict[str, Any]] = None,
+                 timeout: Optional[int] = 600,
+                 user_agent: Optional[str] = 'rucio-clients',
+                 vo: Optional[str] = None,
+                 logger: Logger = LOG) -> None:
         """
         Constructor of the BaseClient.
         :param rucio_host: The address of the rucio server, if None it is read from the config file.
         :param rucio_port: The port of the rucio server, if None it is read from the config file.
         :param auth_host: The address of the rucio authentication server, if None it is read from the config file.
         :param auth_port: The port of the rucio authentication server, if None it is read from the config file.
         :param account: The account to authenticate to rucio.
@@ -90,17 +103,16 @@
         :param creds: Dictionary with credentials needed for authentication.
         :param user_agent: Indicates the client.
         :param vo: The VO to authenticate into.
         :param logger: Logger object to use. If None, use the default LOG created by the module
         """
 
         self.host = rucio_host
-        self.list_hosts = []
         self.auth_host = auth_host
-        self.logger = logger or LOG
+        self.logger = logger
         self.session = Session()
         self.user_agent = "%s/%s" % (user_agent, version.version_string())  # e.g. "rucio-clients/0.2.13"
         sys.argv[0] = sys.argv[0].split('/')[-1]
         self.script_id = '::'.join(sys.argv[0:2])
         if self.script_id == '':  # Python interpreter used
             self.script_id = 'python'
         try:
@@ -109,118 +121,34 @@
             if self.auth_host is None:
                 self.auth_host = config_get('client', 'auth_host')
         except (NoOptionError, NoSectionError) as error:
             raise MissingClientParameter('Section client and Option \'%s\' cannot be found in config file' % error.args[0])
 
         try:
             self.trace_host = config_get('trace', 'trace_host')
-        except (NoOptionError, NoSectionError):
+        except (NoOptionError, NoSectionError, ConfigNotFound):
             self.trace_host = self.host
             self.logger.debug('No trace_host passed. Using rucio_host instead')
 
+        self.list_hosts = [self.host]
         self.account = account
         self.vo = vo
         self.ca_cert = ca_cert
-        self.auth_type = auth_type
-        self.creds = creds
-        self.auth_token = None
-        self.auth_token_file_path = config_get('client', 'auth_token_file_path', False, None)
+        self.auth_token = ""
         self.headers = {}
         self.timeout = timeout
         self.request_retries = self.REQUEST_RETRIES
         self.token_exp_epoch = None
-        self.token_exp_epoch_file = None
         self.auth_oidc_refresh_active = config_get_bool('client', 'auth_oidc_refresh_active', False, False)
+
         # defining how many minutes before token expires, oidc refresh (if active) should start
         self.auth_oidc_refresh_before_exp = config_get_int('client', 'auth_oidc_refresh_before_exp', False, 20)
 
-        if auth_type is None:
-            self.logger.debug('No auth_type passed. Trying to get it from the environment variable RUCIO_AUTH_TYPE and config file.')
-            if 'RUCIO_AUTH_TYPE' in environ:
-                if environ['RUCIO_AUTH_TYPE'] not in ['userpass', 'x509', 'x509_proxy', 'gss', 'ssh', 'saml', 'oidc']:
-                    raise MissingClientParameter('Possible RUCIO_AUTH_TYPE values: userpass, x509, x509_proxy, gss, ssh, saml, oidc, vs. ' + environ['RUCIO_AUTH_TYPE'])
-                self.auth_type = environ['RUCIO_AUTH_TYPE']
-            else:
-                try:
-                    self.auth_type = config_get('client', 'auth_type')
-                except (NoOptionError, NoSectionError) as error:
-                    raise MissingClientParameter('Option \'%s\' cannot be found in config file' % error.args[0])
-
-        if self.auth_type == 'oidc':
-            if not self.creds:
-                self.creds = {}
-            # if there are defautl values, check if rucio.cfg does not specify them, otherwise put default
-            if 'oidc_refresh_lifetime' not in self.creds or self.creds['oidc_refresh_lifetime'] is None:
-                self.creds['oidc_refresh_lifetime'] = config_get('client', 'oidc_refresh_lifetime', False, None)
-            if 'oidc_issuer' not in self.creds or self.creds['oidc_issuer'] is None:
-                self.creds['oidc_issuer'] = config_get('client', 'oidc_issuer', False, None)
-            if 'oidc_audience' not in self.creds or self.creds['oidc_audience'] is None:
-                self.creds['oidc_audience'] = config_get('client', 'oidc_audience', False, None)
-            if 'oidc_auto' not in self.creds or self.creds['oidc_auto'] is False:
-                self.creds['oidc_auto'] = config_get_bool('client', 'oidc_auto', False, False)
-            if self.creds['oidc_auto']:
-                if 'oidc_username' not in self.creds or self.creds['oidc_username'] is None:
-                    self.creds['oidc_username'] = config_get('client', 'oidc_username', False, None)
-                if 'oidc_password' not in self.creds or self.creds['oidc_password'] is None:
-                    self.creds['oidc_password'] = config_get('client', 'oidc_password', False, None)
-            if 'oidc_scope' not in self.creds or self.creds['oidc_scope'] == 'openid profile':
-                self.creds['oidc_scope'] = config_get('client', 'oidc_scope', False, 'openid profile')
-            if 'oidc_polling' not in self.creds or self.creds['oidc_polling'] is False:
-                self.creds['oidc_polling'] = config_get_bool('client', 'oidc_polling', False, False)
-
-        if not self.creds:
-            self.logger.debug('No creds passed. Trying to get it from the config file.')
-            self.creds = {}
-            try:
-                if self.auth_type in ['userpass', 'saml']:
-                    self.creds['username'] = config_get('client', 'username')
-                    self.creds['password'] = config_get('client', 'password')
-                elif self.auth_type == 'x509':
-                    if "RUCIO_CLIENT_CERT" in environ:
-                        client_cert = environ["RUCIO_CLIENT_CERT"]
-                    else:
-                        client_cert = config_get('client', 'client_cert')
-                    self.creds['client_cert'] = path.abspath(path.expanduser(path.expandvars(client_cert)))
-                    if not path.exists(self.creds['client_cert']):
-                        raise MissingClientParameter('X.509 client certificate not found: %s' % self.creds['client_cert'])
-
-                    if "RUCIO_CLIENT_KEY" in environ:
-                        client_key = environ["RUCIO_CLIENT_KEY"]
-                    else:
-                        client_key = config_get('client', 'client_key')
-                    self.creds['client_key'] = path.abspath(path.expanduser(path.expandvars(client_key)))
-                    if not path.exists(self.creds['client_key']):
-                        raise MissingClientParameter('X.509 client key not found: %s' % self.creds['client_key'])
-                    else:
-                        perms = oct(os.stat(self.creds['client_key']).st_mode)[-3:]
-                        if perms not in ['400', '600']:
-                            raise CannotAuthenticate('X.509 authentication selected, but private key (%s) permissions are liberal (required: 400 or 600, found: %s)' % (self.creds['client_key'], perms))
-
-                elif self.auth_type == 'x509_proxy':
-                    try:
-                        self.creds['client_proxy'] = path.abspath(path.expanduser(path.expandvars(config_get('client', 'client_x509_proxy'))))
-                    except NoOptionError:
-                        # Recreate the classic GSI logic for locating the proxy:
-                        # - $X509_USER_PROXY, if it is set.
-                        # - /tmp/x509up_u`id -u` otherwise.
-                        # If neither exists (at this point, we don't care if it exists but is invalid), then rethrow
-                        if 'X509_USER_PROXY' in environ:
-                            self.creds['client_proxy'] = environ['X509_USER_PROXY']
-                        else:
-                            fname = '/tmp/x509up_u%d' % geteuid()
-                            if path.exists(fname):
-                                self.creds['client_proxy'] = fname
-                            else:
-                                raise MissingClientParameter('Cannot find a valid X509 proxy; not in %s, $X509_USER_PROXY not set, and '
-                                                             '\'x509_proxy\' not set in the configuration file.' % fname)
-                elif self.auth_type == 'ssh':
-                    self.creds['ssh_private_key'] = path.abspath(path.expanduser(path.expandvars(config_get('client', 'ssh_private_key'))))
-            except (NoOptionError, NoSectionError) as error:
-                if error.args[0] != 'client_key':
-                    raise MissingClientParameter('Option \'%s\' cannot be found in config file' % error.args[0])
+        self.auth_type = self._get_auth_type(auth_type)
+        self.creds = self._get_creds(creds)
 
         rucio_scheme = urlparse(self.host).scheme
         auth_scheme = urlparse(self.auth_host).scheme
 
         if rucio_scheme != 'http' and rucio_scheme != 'https':
             raise ClientProtocolNotSupported('\'%s\' not supported' % rucio_scheme)
 
@@ -234,16 +162,14 @@
                 self.logger.debug('HTTPS is required, but no ca_cert was passed and X509_CERT_DIR is not defined. Trying to get it from the config file.')
                 try:
                     self.ca_cert = path.expandvars(config_get('client', 'ca_cert'))
                 except (NoOptionError, NoSectionError):
                     self.logger.debug('No ca_cert found in configuration. Falling back to Mozilla default CA bundle (certifi).')
                     self.ca_cert = True
 
-        self.list_hosts = [self.host]
-
         if account is None:
             self.logger.debug('No account passed. Trying to get it from the RUCIO_ACCOUNT environment variable or the config file.')
             try:
                 self.account = environ['RUCIO_ACCOUNT']
             except KeyError:
                 try:
                     self.account = config_get('client', 'account')
@@ -258,38 +184,134 @@
                 self.logger.debug('No VO found. Trying to get it from the config file.')
                 try:
                     self.vo = config_get('client', 'vo')
                 except (NoOptionError, NoSectionError):
                     self.logger.debug('No VO found. Using default VO.')
                     self.vo = 'def'
 
-        token_filename_suffix = "for_default_account" if self.account is None else "for_account_" + self.account
+        self.auth_token_file_path, self.token_exp_epoch_file, self.token_file, self.token_path = self._get_auth_tokens()
+        self.__authenticate()
 
+        try:
+            self.request_retries = config_get_int('client', 'request_retries')
+        except (NoOptionError, ConfigNotFound):
+            self.logger.debug('request_retries not specified in config file. Taking default.')
+        except ValueError:
+            self.logger.debug('request_retries must be an integer. Taking default.')
+
+    def _get_auth_tokens(self) -> tuple[Optional[str], str, str, str]:
         # if token file path is defined in the rucio.cfg file, use that file. Currently this prevents authenticating as another user or VO.
-        if self.auth_token_file_path:
-            self.token_file = self.auth_token_file_path
-            self.token_path = '/'.join(self.token_file.split('/')[:-1])
+        auth_token_file_path = config_get('client', 'auth_token_file_path', False, None)
+        token_filename_suffix = "for_default_account" if self.account is None else "for_account_" + self.account
+
+        if auth_token_file_path:
+            token_file = auth_token_file_path
+            token_path = '/'.join(auth_token_file_path.split('/')[:-1])
+
         else:
-            self.token_path = self.TOKEN_PATH_PREFIX + getpass.getuser()
+            token_path = self.TOKEN_PATH_PREFIX + getpass.getuser()
             if self.vo != 'def':
-                self.token_path += '@%s' % self.vo
-            self.token_file = self.token_path + '/' + self.TOKEN_PREFIX + token_filename_suffix
+                token_path += '@%s' % self.vo
 
-        self.token_exp_epoch_file = self.token_path + '/' + self.TOKEN_EXP_PREFIX + token_filename_suffix
+            token_file = token_path + '/' + self.TOKEN_PREFIX + token_filename_suffix
 
-        self.__authenticate()
+        token_exp_epoch_file = token_path + '/' + self.TOKEN_EXP_PREFIX + token_filename_suffix
+        return auth_token_file_path, token_exp_epoch_file, token_file, token_path
 
-        try:
-            self.request_retries = config_get_int('client', 'request_retries')
-        except (NoOptionError, RuntimeError):
-            LOG.debug('request_retries not specified in config file. Taking default.')
-        except ValueError:
-            self.logger.debug('request_retries must be an integer. Taking default.')
+    def _get_auth_type(self, auth_type: Optional[str]) -> str:
+        if auth_type is None:
+            self.logger.debug('No auth_type passed. Trying to get it from the environment variable RUCIO_AUTH_TYPE and config file.')
+            if 'RUCIO_AUTH_TYPE' in environ:
+                if environ['RUCIO_AUTH_TYPE'] not in ['userpass', 'x509', 'x509_proxy', 'gss', 'ssh', 'saml', 'oidc']:
+                    raise MissingClientParameter('Possible RUCIO_AUTH_TYPE values: userpass, x509, x509_proxy, gss, ssh, saml, oidc, vs. ' + environ['RUCIO_AUTH_TYPE'])
+                auth_type = environ['RUCIO_AUTH_TYPE']
+            else:
+                try:
+                    auth_type = config_get('client', 'auth_type')
+                except (NoOptionError, NoSectionError) as error:
+                    raise MissingClientParameter('Option \'%s\' cannot be found in config file' % error.args[0])
+        return auth_type
+
+    def _get_creds(self, creds: Optional[dict[str, Any]]) -> dict[str, Any]:
+        if self.auth_type == 'oidc':
+            if not creds:
+                creds = {}
+            # if there are defautl values, check if rucio.cfg does not specify them, otherwise put default
+            if 'oidc_refresh_lifetime' not in creds or creds['oidc_refresh_lifetime'] is None:
+                creds['oidc_refresh_lifetime'] = config_get('client', 'oidc_refresh_lifetime', False, None)
+            if 'oidc_issuer' not in creds or creds['oidc_issuer'] is None:
+                creds['oidc_issuer'] = config_get('client', 'oidc_issuer', False, None)
+            if 'oidc_audience' not in creds or creds['oidc_audience'] is None:
+                creds['oidc_audience'] = config_get('client', 'oidc_audience', False, None)
+            if 'oidc_auto' not in creds or creds['oidc_auto'] is False:
+                creds['oidc_auto'] = config_get_bool('client', 'oidc_auto', False, False)
+            if creds['oidc_auto']:
+                if 'oidc_username' not in creds or creds['oidc_username'] is None:
+                    creds['oidc_username'] = config_get('client', 'oidc_username', False, None)
+                if 'oidc_password' not in creds or creds['oidc_password'] is None:
+                    creds['oidc_password'] = config_get('client', 'oidc_password', False, None)
+            if 'oidc_scope' not in creds or creds['oidc_scope'] == 'openid profile':
+                creds['oidc_scope'] = config_get('client', 'oidc_scope', False, 'openid profile')
+            if 'oidc_polling' not in creds or creds['oidc_polling'] is False:
+                creds['oidc_polling'] = config_get_bool('client', 'oidc_polling', False, False)
+
+        if creds is None:
+            self.logger.debug('No creds passed. Trying to get it from the config file.')
+            creds = {}
+            try:
+                if self.auth_type in ['userpass', 'saml']:
+                    creds['username'] = config_get('client', 'username')
+                    creds['password'] = config_get('client', 'password')
+                elif self.auth_type == 'x509':
+                    if "RUCIO_CLIENT_CERT" in environ:
+                        client_cert = environ["RUCIO_CLIENT_CERT"]
+                    else:
+                        client_cert = config_get('client', 'client_cert')
+                    creds['client_cert'] = path.abspath(path.expanduser(path.expandvars(client_cert)))
+                    if not path.exists(creds['client_cert']):
+                        raise MissingClientParameter('X.509 client certificate not found: %s' % creds['client_cert'])
+
+                    if "RUCIO_CLIENT_KEY" in environ:
+                        client_key = environ["RUCIO_CLIENT_KEY"]
+                    else:
+                        client_key = config_get('client', 'client_key')
+                    creds['client_key'] = path.abspath(path.expanduser(path.expandvars(client_key)))
+                    if not path.exists(creds['client_key']):
+                        raise MissingClientParameter('X.509 client key not found: %s' % creds['client_key'])
+                    else:
+                        perms = oct(os.stat(creds['client_key']).st_mode)[-3:]
+                        if perms not in ['400', '600']:
+                            raise CannotAuthenticate('X.509 authentication selected, but private key (%s) permissions are liberal (required: 400 or 600, found: %s)' % (creds['client_key'], perms))
+
+                elif self.auth_type == 'x509_proxy':
+                    try:
+                        creds['client_proxy'] = path.abspath(path.expanduser(path.expandvars(config_get('client', 'client_x509_proxy'))))
+                    except NoOptionError:
+                        # Recreate the classic GSI logic for locating the proxy:
+                        # - $X509_USER_PROXY, if it is set.
+                        # - /tmp/x509up_u`id -u` otherwise.
+                        # If neither exists (at this point, we don't care if it exists but is invalid), then rethrow
+                        if 'X509_USER_PROXY' in environ:
+                            creds['client_proxy'] = environ['X509_USER_PROXY']
+                        else:
+                            fname = '/tmp/x509up_u%d' % geteuid()
+                            if path.exists(fname):
+                                creds['client_proxy'] = fname
+                            else:
+                                raise MissingClientParameter(
+                                    'Cannot find a valid X509 proxy; not in %s, $X509_USER_PROXY not set, and '
+                                    '\'x509_proxy\' not set in the configuration file.' % fname)
+                elif self.auth_type == 'ssh':
+                    creds['ssh_private_key'] = path.abspath(path.expanduser(path.expandvars(config_get('client', 'ssh_private_key'))))
+            except (NoOptionError, NoSectionError) as error:
+                if error.args[0] != 'client_key':
+                    raise MissingClientParameter('Option \'%s\' cannot be found in config file' % error.args[0])
+        return creds
 
-    def _get_exception(self, headers, status_code=None, data=None):
+    def _get_exception(self, headers: dict[str, str], status_code: Optional[int] = None, data=None) -> tuple[type[exception.RucioException], str]:
         """
         Helper method to parse an error string send by the server and transform it into the corresponding rucio exception.
 
         :param headers: The http response header containing the Rucio exception details.
         :param status_code: The http status code.
         :param data: The data with the ExceptionMessage.
 
@@ -312,15 +334,15 @@
             exc_msg = headers['ExceptionMessage']
 
         if hasattr(exception, exc_cls):
             return getattr(exception, exc_cls), exc_msg
         else:
             return exception.RucioException, "%s: %s" % (exc_cls, exc_msg)
 
-    def _load_json_data(self, response):
+    def _load_json_data(self, response: requests.Response) -> Generator[Any, Any, Any]:
         """
         Helper method to correctly load json data based on the content type of the http response.
 
         :param response: the response received from the server.
         """
         if 'content-type' in response.headers and response.headers['content-type'] == 'application/x-json-stream':
             for line in response.iter_lines():
@@ -328,21 +350,21 @@
                     yield parse_response(line)
         elif 'content-type' in response.headers and response.headers['content-type'] == 'application/json':
             yield parse_response(response.text)
         else:  # Exception ?
             if response.text:
                 yield response.text
 
-    def _reduce_data(self, data, maxlen=132):
+    def _reduce_data(self, data, maxlen: int = 132) -> str:
         text = data if isinstance(data, str) else data.decode("utf-8")
         if len(text) > maxlen:
             text = "%s ... %s" % (text[:maxlen - 15], text[-10:])
         return text
 
-    def _back_off(self, retry_number, reason):
+    def _back_off(self, retry_number: int, reason: str) -> None:
         """
         Sleep a certain amount of time which increases with the retry count
         :param retry_number: the retry iteration
         :param reason: the reason to backoff which will be shown to the user
         """
         sleep_time = min(MAX_RETRY_BACK_OFF_SECONDS, 0.25 * 2 ** retry_number)
         self.logger.warning("Waiting {}s due to reason: {} ".format(sleep_time, reason))
@@ -429,15 +451,15 @@
             else:
                 break
 
         if result is None:
             raise ServerConnectionException
         return result
 
-    def __get_token_userpass(self):
+    def __get_token_userpass(self) -> bool:
         """
         Sends a request to get an auth token from the server and stores it as a class attribute. Uses username/password.
 
         :returns: True if the token was successfully received. False otherwise.
         """
 
         headers = {'X-Rucio-Username': self.creds['username'],
@@ -465,15 +487,15 @@
                                                    status_code=result.status_code,
                                                    data=result.content)
             raise exc_cls(exc_msg)
 
         self.auth_token = result.headers['x-rucio-auth-token']
         return True
 
-    def __refresh_token_OIDC(self):
+    def __refresh_token_OIDC(self) -> bool:
         """
         Checks if there is active refresh token and if so returns
         either active token with expiration timestamp or requests a new
         refresh and returns new access token with new expiration timestamp
         and saves these in the token directory.
 
         :returns: True if the token was successfully received. False otherwise.
@@ -519,15 +541,15 @@
                            \ntoken or a token with no refresh token in Rucio DB")
                 return False
         else:
             print("Rucio Client did not succeed to contact the \
                    \nRucio Auth Server when attempting token refresh.")
             return False
 
-    def __get_token_OIDC(self):
+    def __get_token_OIDC(self) -> bool:
         """
         First authenticates the user via a Identity Provider server
         (with user's username & password), by specifying oidc_scope,
         user agrees to share the relevant information with Rucio.
         If all proceeds well, an access token is requested from the Identity Provider.
         Access Tokens are not stored in Rucio DB.
         Refresh Tokens are granted only in case no valid access token exists in user's
@@ -643,15 +665,15 @@
             file_d, file_n = mkstemp(dir=self.token_path)
             with fdopen(file_d, "w") as f_exp_epoch:
                 f_exp_epoch.write(str(self.token_exp_epoch))
             move(file_n, self.token_exp_epoch_file)
             self.__refresh_token_OIDC()
         return True
 
-    def __get_token_x509(self):
+    def __get_token_x509(self) -> bool:
         """
         Sends a request to get an auth token from the server and stores it as a class attribute. Uses x509 authentication.
 
         :returns: True if the token was successfully received. False otherwise.
         """
         client_cert = None
         client_key = None
@@ -660,15 +682,15 @@
             client_cert = self.creds['client_cert']
             if 'client_key' in self.creds:
                 client_key = self.creds['client_key']
         elif self.auth_type == 'x509_proxy':
             url = build_url(self.auth_host, path='auth/x509_proxy')
             client_cert = self.creds['client_proxy']
 
-        if not path.exists(client_cert):
+        if (client_cert is not None) and not (path.exists(client_cert)):
             self.logger.error('given client cert (%s) doesn\'t exist' % client_cert)
             return False
         if client_key is not None and not path.exists(client_key):
             self.logger.error('given client key (%s) doesn\'t exist' % client_key)
 
         if client_key is None:
             cert = client_cert
@@ -688,15 +710,15 @@
                                                    status_code=result.status_code,
                                                    data=result.content)
             raise exc_cls(exc_msg)
 
         self.auth_token = result.headers['x-rucio-auth-token']
         return True
 
-    def __get_token_ssh(self):
+    def __get_token_ssh(self) -> bool:
         """
         Sends a request to get an auth token from the server and stores it as a class attribute. Uses SSH key exchange authentication.
 
         :returns: True if the token was successfully received. False otherwise.
         """
         headers = {}
 
@@ -744,15 +766,15 @@
                                                    status_code=result.status_code,
                                                    data=result.content)
             raise exc_cls(exc_msg)
 
         self.auth_token = result.headers['x-rucio-auth-token']
         return True
 
-    def __get_token_gss(self):
+    def __get_token_gss(self) -> bool:
         """
         Sends a request to get an auth token from the server and stores it as a class attribute. Uses Kerberos authentication.
 
         :returns: True if the token was successfully received. False otherwise.
         """
         if not EXTRA_MODULES['requests_kerberos']:
             raise MissingModuleException('The requests-kerberos module is not installed.')
@@ -770,15 +792,15 @@
                                                    status_code=result.status_code,
                                                    data=result.content)
             raise exc_cls(exc_msg)
 
         self.auth_token = result.headers['x-rucio-auth-token']
         return True
 
-    def __get_token_saml(self):
+    def __get_token_saml(self) -> bool:
         """
         Sends a request to get an auth token from the server and stores it as a class attribute. Uses saml authentication.
 
         :returns: True if the token was successfully received. False otherwise.
         """
         userpass = {'username': self.creds['username'], 'password': self.creds['password']}
         url = build_url(self.auth_host, path='auth/saml')
@@ -800,15 +822,15 @@
                                                    status_code=result.status_code,
                                                    data=result.content)
             raise exc_cls(exc_msg)
 
         self.auth_token = result.headers['X-Rucio-Auth-Token']
         return True
 
-    def __get_token(self):
+    def __get_token(self) -> None:
         """
         Calls the corresponding method to receive an auth token depending on the auth type. To be used if a 401 - Unauthorized error is received.
         """
 
         self.logger.debug('get a new token')
         for retry in range(self.AUTH_RETRIES + 1):
             if self.auth_type == 'userpass':
@@ -842,15 +864,15 @@
                 self.__write_token()
                 self.headers['X-Rucio-Auth-Token'] = self.auth_token
                 break
 
         if self.auth_token is None:
             raise CannotAuthenticate('cannot get an auth token from server')
 
-    def __read_token(self):
+    def __read_token(self) -> bool:
         """
         Checks if a local token file exists and reads the token from it.
 
         :return: True if a token could be read. False if no file exists.
         """
         if not path.exists(self.token_file):
             return False
@@ -864,15 +886,15 @@
         except Exception:
             raise
         if self.auth_oidc_refresh_active and self.auth_type == 'oidc':
             self.__refresh_token_OIDC()
         self.logger.debug('got token from file')
         return True
 
-    def __write_token(self):
+    def __write_token(self) -> None:
         """
         Write the current auth_token to the local token file.
         """
         # check if rucio temp directory is there. If not create it with permissions only for the current user
         if not path.isdir(self.token_path):
             try:
                 self.logger.debug('rucio token folder \'%s\' not found. Create it.' % self.token_path)
@@ -891,15 +913,15 @@
                     f_exp_epoch.write(str(self.token_exp_epoch))
                 move(file_n, self.token_exp_epoch_file)
         except OSError as error:
             print("I/O error({0}): {1}".format(error.errno, error.strerror))
         except Exception:
             raise
 
-    def __authenticate(self):
+    def __authenticate(self) -> None:
         """
         Main method for authentication. It first tries to read a locally saved token. If not available it requests a new one.
         """
         if self.auth_type == 'userpass':
             if self.creds['username'] is None or self.creds['password'] is None:
                 raise NoAuthInformation('No username or password passed')
         elif self.auth_type == 'oidc':
```

### Comparing `rucio-clients-34.1.0/lib/rucio/client/client.py` & `rucio_clients-34.2.0/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/configclient.py` & `rucio_clients-34.2.0/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/credentialclient.py` & `rucio_clients-34.2.0/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/didclient.py` & `rucio_clients-34.2.0/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/diracclient.py` & `rucio_clients-34.2.0/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/downloadclient.py` & `rucio_clients-34.2.0/lib/rucio/client/downloadclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import copy
 import enum
 import itertools
 import logging
 import os
 import random
+import secrets
 import shutil
 import signal
 import subprocess
 import time
 from queue import Empty, Queue, deque
 from threading import Thread
 
@@ -758,15 +759,15 @@
         :raises NoFilesDownloaded: if no files could be downloaded
         :raises NotAllFilesDownloaded: if not all files could be downloaded
         :raises RucioException: if something went wrong during the download (e.g. aria2c could not be started)
         """
         logger = self.logger
         trace_custom_fields['uuid'] = generate_uuid()
 
-        rpc_secret = '%x' % (random.getrandbits(64))
+        rpc_secret = '%x' % (secrets.randbits(64))
         rpc_auth = 'token:%s' % rpc_secret
         rpcproc, aria_rpc = self._start_aria2c_rpc(rpc_secret)
 
         for item in items:
             item['force_scheme'] = ['https', 'davs']
             item['no_resolve_archives'] = True
 
@@ -819,15 +820,15 @@
               '--connect-timeout=5 '\
               '--rpc-listen-port=%d'
 
         logger(logging.INFO, 'Starting aria2c rpc server...')
 
         # trying up to 3 random ports
         for attempt in range(3):
-            port = random.randint(1024, 65534)
+            port = random.randint(1024, 65534)  # noqa: S311
             logger(logging.DEBUG, 'Trying to start rpc server on port: %d' % port)
             try:
                 to_exec = cmd % (os.getpid(), rpc_secret, port)
                 logger(logging.DEBUG, to_exec)
                 rpcproc = subprocess.Popen(
                     cmd,
                     shell=True,
```

### Comparing `rucio-clients-34.1.0/lib/rucio/client/exportclient.py` & `rucio_clients-34.2.0/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/fileclient.py` & `rucio_clients-34.2.0/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/importclient.py` & `rucio_clients-34.2.0/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/lifetimeclient.py` & `rucio_clients-34.2.0/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/lockclient.py` & `rucio_clients-34.2.0/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/metaconventionsclient.py` & `rucio_clients-34.2.0/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/pingclient.py` & `rucio_clients-34.2.0/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/replicaclient.py` & `rucio_clients-34.2.0/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/requestclient.py` & `rucio_clients-34.2.0/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/rseclient.py` & `rucio_clients-34.2.0/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/ruleclient.py` & `rucio_clients-34.2.0/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/scopeclient.py` & `rucio_clients-34.2.0/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/subscriptionclient.py` & `rucio_clients-34.2.0/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/touchclient.py` & `rucio_clients-34.2.0/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/client/uploadclient.py` & `rucio_clients-34.2.0/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/__init__.py` & `rucio_clients-34.2.0/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/cache.py` & `rucio_clients-34.2.0/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/config.py` & `rucio_clients-34.2.0/lib/rucio/common/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,20 +184,20 @@
 
     :raises NoOptionError
     :raises NoSectionError
     :raises RuntimeError
     """
     try:
         return convert_type_fnc(get_config().get(section, option))
-    except (configparser.NoOptionError, configparser.NoSectionError, RuntimeError) as err:
+    except (configparser.NoOptionError, configparser.NoSectionError, ConfigNotFound) as err:
         try:
             legacy_config = get_legacy_config(section, option)
             if legacy_config is not None:
                 return convert_type_fnc(legacy_config)
-        except RuntimeError:
+        except ConfigNotFound:
             pass
 
         from rucio.common.utils import is_client
         client_mode = is_client()
 
         if not client_mode and check_config_table:
             try:
@@ -725,15 +725,15 @@
 
 
 def get_lfn2pfn_algorithm_default():
     """Returns the default algorithm name for LFN2PFN translation for this server."""
     default_lfn2pfn = "hash"
     try:
         default_lfn2pfn = config_get('policy', 'lfn2pfn_algorithm_default')
-    except (configparser.NoOptionError, configparser.NoSectionError, RuntimeError):
+    except (configparser.NoOptionError, configparser.NoSectionError, ConfigNotFound, RuntimeError):
         pass
     return default_lfn2pfn
 
 
 def get_rse_credentials(path_to_credentials_file: Optional[Union[str, os.PathLike]] = None):
     """ Returns credentials for RSEs. """
 
@@ -781,15 +781,17 @@
 
         if 'RUCIO_CONFIG' in os.environ:
             self.configfile = os.environ['RUCIO_CONFIG']
         else:
             configs = [os.path.join(confdir, 'rucio.cfg') for confdir in get_config_dirs()]
             self.configfile = next(iter(filter(os.path.exists, configs)), None)
             if self.configfile is None:
-                raise RuntimeError('Could not load Rucio configuration file. '
-                                   'Rucio looked in the following paths for a configuration file, in order:'
-                                   '\n\t' + '\n\t'.join(configs))
+                raise ConfigNotFound(
+                    'Could not load Rucio configuration file. '
+                    'Rucio looked in the following paths for a configuration file, in order:'
+                    '\n\t' + '\n\t'.join(configs))
 
         if not self.parser.read(self.configfile) == [self.configfile]:
-            raise RuntimeError('Could not load Rucio configuration file. '
-                               'Rucio tried loading the following configuration file:'
-                               '\n\t' + self.configfile)
+            raise ConfigNotFound(
+                'Could not load Rucio configuration file. '
+                'Rucio tried loading the following configuration file:'
+                '\n\t' + self.configfile)
```

### Comparing `rucio-clients-34.1.0/lib/rucio/common/constants.py` & `rucio_clients-34.2.0/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/constraints.py` & `rucio_clients-34.2.0/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/didtype.py` & `rucio_clients-34.2.0/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/exception.py` & `rucio_clients-34.2.0/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/extra.py` & `rucio_clients-34.2.0/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/logging.py` & `rucio_clients-34.2.0/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/pcache.py` & `rucio_clients-34.2.0/lib/rucio/common/pcache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/plugins.py` & `rucio_clients-34.2.0/lib/rucio/common/plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/policy.py` & `rucio_clients-34.2.0/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/__init__.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/atlas.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/belleii.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/cms.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/domatpc.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/escape.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/generic.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/icecube.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/schema/lsst.py` & `rucio_clients-34.2.0/lib/rucio/common/schema/lsst.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/stomp_utils.py` & `rucio_clients-34.2.0/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/stopwatch.py` & `rucio_clients-34.2.0/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/test_rucio_server.py` & `rucio_clients-34.2.0/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/types.py` & `rucio_clients-34.2.0/lib/rucio/common/types.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/common/utils.py` & `rucio_clients-34.2.0/lib/rucio/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from urllib.parse import parse_qsl, quote, urlencode, urlparse, urlunparse
 from uuid import uuid4 as uuid
 from xml.etree import ElementTree
 
 import requests
 
 from rucio.common.config import config_get, config_has_section
-from rucio.common.exception import DIDFilterSyntaxError, DuplicateCriteriaInDIDFilter, InputValidationError, InvalidType, MetalinkJsonParsingError, MissingModuleException, PolicyPackageVersionError, RucioException
+from rucio.common.exception import ConfigNotFound, DIDFilterSyntaxError, DuplicateCriteriaInDIDFilter, InputValidationError, InvalidType, MetalinkJsonParsingError, MissingModuleException, PolicyPackageVersionError, RucioException
 from rucio.common.extra import import_extras
 from rucio.common.plugins import PolicyPackageAlgorithms
 from rucio.common.types import InternalAccount, InternalScope
 
 EXTRA_MODULES = import_extras(['paramiko'])
 
 if EXTRA_MODULES['paramiko']:
@@ -143,27 +143,27 @@
         if isinstance(params, str):
             complete_url += quote(params)
         else:
             complete_url += urlencode(params, doseq=doseq)
     return complete_url
 
 
-def all_oidc_req_claims_present(scope, audience, required_scope, required_audience, sepatator=" "):
+def all_oidc_req_claims_present(scope, audience, required_scope, required_audience, separator=" "):
     """
     Checks if both of the following statements are true:
     - all items in required_scope are present in scope string
     - all items in required_audience are present in audience
     returns false otherwise. audience and scope must be both strings
     or both lists. Similarly for required_* variables.
     If this condition is satisfied, False is returned.
     :params scope: list of strings or one string where items are separated by a separator input variable
     :params audience: list of strings or one string where items are separated by a separator input variable
     :params required_scope: list of strings or one string where items are separated by a separator input variable
     :params required_audience: list of strings or one string where items are separated by a separator input variable
-    :params sepatator: separator string, space by default
+    :params separator: separator string, space by default
     :returns : True or False
     """
     if not scope:
         scope = ""
     if not audience:
         audience = ""
     if not required_scope:
@@ -179,32 +179,32 @@
         req_audience_present = all(elem in audience for elem in required_audience)
         return req_scope_present and req_audience_present
     elif (isinstance(scope, str) and isinstance(audience, str) and isinstance(required_scope, str) and isinstance(required_audience, str)):
         scope = str(scope)
         audience = str(audience)
         required_scope = str(required_scope)
         required_audience = str(required_audience)
-        req_scope_present = all(elem in scope.split(sepatator) for elem in required_scope.split(sepatator))
-        req_audience_present = all(elem in audience.split(sepatator) for elem in required_audience.split(sepatator))
+        req_scope_present = all(elem in scope.split(separator) for elem in required_scope.split(separator))
+        req_audience_present = all(elem in audience.split(separator) for elem in required_audience.split(separator))
         return req_scope_present and req_audience_present
     elif (isinstance(scope, list) and isinstance(audience, list) and isinstance(required_scope, str) and isinstance(required_audience, str)):
         scope = [str(it) for it in scope]
         audience = [str(it) for it in audience]
         required_scope = str(required_scope)
         required_audience = str(required_audience)
-        req_scope_present = all(elem in scope for elem in required_scope.split(sepatator))
-        req_audience_present = all(elem in audience for elem in required_audience.split(sepatator))
+        req_scope_present = all(elem in scope for elem in required_scope.split(separator))
+        req_audience_present = all(elem in audience for elem in required_audience.split(separator))
         return req_scope_present and req_audience_present
     elif (isinstance(scope, str) and isinstance(audience, str) and isinstance(required_scope, list) and isinstance(required_audience, list)):
         scope = str(scope)
         audience = str(audience)
         required_scope = [str(it) for it in required_scope]
         required_audience = [str(it) for it in required_audience]
-        req_scope_present = all(elem in scope.split(sepatator) for elem in required_scope)
-        req_audience_present = all(elem in audience.split(sepatator) for elem in required_audience)
+        req_scope_present = all(elem in scope.split(separator) for elem in required_scope)
+        req_audience_present = all(elem in audience.split(separator) for elem in required_audience)
         return req_scope_present and req_audience_present
     else:
         return False
 
 
 def generate_uuid():
     return str(uuid()).replace('-', '').lower()
@@ -1840,15 +1840,15 @@
         try:
             if config_has_section('database'):
                 client_mode = False
             elif config_has_section('client'):
                 client_mode = True
             else:
                 client_mode = False
-        except RuntimeError:
+        except (RuntimeError, ConfigNotFound):
             # If no configuration file is found the default value should be True
             client_mode = True
     else:
         if os.environ['RUCIO_CLIENT_MODE']:
             client_mode = True
         else:
             client_mode = False
```

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/__init__.py` & `rucio_clients-34.2.0/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/__init__.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/cache.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/dummy.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/gfal.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/globus.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/http_cache.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/mock.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/ngarc.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/posix.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/protocol.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/rclone.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/rfio.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/srm.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/ssh.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/storm.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/storm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/webdav.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/protocols/xrootd.py` & `rucio_clients-34.2.0/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/rse/rsemanager.py` & `rucio_clients-34.2.0/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/lib/rucio/version.py` & `rucio_clients-34.2.0/lib/rucio/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,25 @@
                     'final': False,
                     'revno': 0}
 
 RUCIO_VERSION = [VERSION_INFO['version'], ]
 FINAL = VERSION_INFO['final']   # This becomes true at Release Candidate time
 
 
-def canonical_version_string():
+def canonical_version_string() -> str:
     """ Get the canonical string """
     return '.'.join(filter(None, RUCIO_VERSION))
 
 
-def version_string():
+def version_string() -> str:
     """ Get the version string """
     return canonical_version_string()
 
 
-def vcs_version_string():
+def vcs_version_string() -> str:
     """ Get the VCS version string """
     return "%s:%s" % (VERSION_INFO['branch_nick'], VERSION_INFO['revision_id'])
 
 
-def version_string_with_vcs():
+def version_string_with_vcs() -> str:
     """ Get the version string with VCS """
     return "%s-%s" % (canonical_version_string(), vcs_version_string())
```

### Comparing `rucio-clients-34.1.0/lib/rucio_clients.egg-info/SOURCES.txt` & `rucio_clients-34.2.0/lib/rucio_clients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/pylintrc` & `rucio_clients-34.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/pyproject.toml` & `rucio_clients-34.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/requirements.txt` & `rucio_clients-34.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/setup.py` & `rucio_clients-34.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/setuputil.py` & `rucio_clients-34.2.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_abacus_account.py` & `rucio_clients-34.2.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_abacus_collection_replica.py` & `rucio_clients-34.2.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_abacus_rse.py` & `rucio_clients-34.2.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_account.py` & `rucio_clients-34.2.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_account_limits.py` & `rucio_clients-34.2.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_api_external_representation.py` & `rucio_clients-34.2.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_archive.py` & `rucio_clients-34.2.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_auditor.py` & `rucio_clients-34.2.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_auditor_hdfs.py` & `rucio_clients-34.2.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_auditor_srmdumps.py` & `rucio_clients-34.2.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_authentication.py` & `rucio_clients-34.2.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_automatix.py` & `rucio_clients-34.2.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_bad_replica.py` & `rucio_clients-34.2.0/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_bb8.py` & `rucio_clients-34.2.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_belleii.py` & `rucio_clients-34.2.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_bin_rucio.py` & `rucio_clients-34.2.0/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_boolean.py` & `rucio_clients-34.2.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_common_types.py` & `rucio_clients-34.2.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_config.py` & `rucio_clients-34.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_conveyor.py` & `rucio_clients-34.2.0/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_conveyor_submitter.py` & `rucio_clients-34.2.0/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_counter.py` & `rucio_clients-34.2.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_credential.py` & `rucio_clients-34.2.0/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_curl.py` & `rucio_clients-34.2.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_daemons.py` & `rucio_clients-34.2.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_dataset_replicas.py` & `rucio_clients-34.2.0/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_db.py` & `rucio_clients-34.2.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_did.py` & `rucio_clients-34.2.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_did_meta_plugins.py` & `rucio_clients-34.2.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_didtype.py` & `rucio_clients-34.2.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_download.py` & `rucio_clients-34.2.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_dumper.py` & `rucio_clients-34.2.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_dumper_consistency.py` & `rucio_clients-34.2.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_dumper_data_model.py` & `rucio_clients-34.2.0/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_dumper_path_parsing.py` & `rucio_clients-34.2.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_filter_engine.py` & `rucio_clients-34.2.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_heartbeat.py` & `rucio_clients-34.2.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_hermes.py` & `rucio_clients-34.2.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_identity.py` & `rucio_clients-34.2.0/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_impl_upload_download.py` & `rucio_clients-34.2.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_import_export.py` & `rucio_clients-34.2.0/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_judge_cleaner.py` & `rucio_clients-34.2.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_judge_evaluator.py` & `rucio_clients-34.2.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_judge_injector.py` & `rucio_clients-34.2.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_judge_repairer.py` & `rucio_clients-34.2.0/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_lifetime.py` & `rucio_clients-34.2.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_message.py` & `rucio_clients-34.2.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_meta_conventions.py` & `rucio_clients-34.2.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_meta_did.py` & `rucio_clients-34.2.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_module_import.py` & `rucio_clients-34.2.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_monitor.py` & `rucio_clients-34.2.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_multi_vo.py` & `rucio_clients-34.2.0/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_naming_convention.py` & `rucio_clients-34.2.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_oauthmanager.py` & `rucio_clients-34.2.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_oidc.py` & `rucio_clients-34.2.0/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_permission.py` & `rucio_clients-34.2.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_pfns.py` & `rucio_clients-34.2.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_ping.py` & `rucio_clients-34.2.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_preparer.py` & `rucio_clients-34.2.0/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_qos.py` & `rucio_clients-34.2.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_quarantined_replica.py` & `rucio_clients-34.2.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_reaper.py` & `rucio_clients-34.2.0/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_redirect.py` & `rucio_clients-34.2.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_replica.py` & `rucio_clients-34.2.0/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_replica_recoverer.py` & `rucio_clients-34.2.0/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_replica_sorting.py` & `rucio_clients-34.2.0/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_request.py` & `rucio_clients-34.2.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_root_proxy.py` & `rucio_clients-34.2.0/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse.py` & `rucio_clients-34.2.0/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_expression_parser.py` & `rucio_clients-34.2.0/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_lfn2path.py` & `rucio_clients-34.2.0/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_gfal2.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_posix.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_rclone.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_rsync.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_srm.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_ssh.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_webdav.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_protocol_xrootd.py` & `rucio_clients-34.2.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rse_selector.py` & `rucio_clients-34.2.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rucio_server.py` & `rucio_clients-34.2.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_rule.py` & `rucio_clients-34.2.0/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_schema_cms.py` & `rucio_clients-34.2.0/tests/test_schema_cms.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_scope.py` & `rucio_clients-34.2.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_subscription.py` & `rucio_clients-34.2.0/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_throttler.py` & `rucio_clients-34.2.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_tpc.py` & `rucio_clients-34.2.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_trace.py` & `rucio_clients-34.2.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_transfer.py` & `rucio_clients-34.2.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_transfer_plugins.py` & `rucio_clients-34.2.0/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_undertaker.py` & `rucio_clients-34.2.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_upload.py` & `rucio_clients-34.2.0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tests/test_utils.py` & `rucio_clients-34.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-34.1.0/tools/merge_rucio_configs.py` & `rucio_clients-34.2.0/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

