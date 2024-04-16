# Comparing `tmp/rucio-34.1.0.tar.gz` & `tmp/rucio-34.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-34.1.0.tar", last modified: Tue Apr  2 13:57:05 2024, max compression
+gzip compressed data, was "rucio-34.2.0.tar", last modified: Tue Apr 16 10:35:03 2024, max compression
```

## Comparing `rucio-34.1.0.tar` & `rucio-34.2.0.tar`

### file list

```diff
@@ -1,650 +1,650 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.199252 rucio-34.1.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio-34.1.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.1.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      934 2024-04-02 13:57:01.000000 rucio-34.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2799 2024-04-02 13:57:05.199252 rucio-34.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-04-02 11:45:19.000000 rucio-34.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.069251 rucio-34.1.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127075 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)     2820 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-abacus-account
--rwxr-xr-x   0 root         (0) root         (0)     1823 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-abacus-collection-replica
--rwxr-xr-x   0 root         (0) root         (0)     2567 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-abacus-rse
--rwxr-xr-x   0 root         (0) root         (0)   133531 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-admin
--rwxr-xr-x   0 root         (0) root         (0)     3185 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-atropos
--rwxr-xr-x   0 root         (0) root         (0)     5849 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-auditor
--rwxr-xr-x   0 root         (0) root         (0)     2008 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-automatix
--rwxr-xr-x   0 root         (0) root         (0)     3103 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-bb8
--rwxr-xr-x   0 root         (0) root         (0)     6100 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-c3po
--rwxr-xr-x   0 root         (0) root         (0)     5063 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-cache-client
--rwxr-xr-x   0 root         (0) root         (0)     1362 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-cache-consumer
--rwxr-xr-x   0 root         (0) root         (0)     2346 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-finisher
--rwxr-xr-x   0 root         (0) root         (0)     2839 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-poller
--rwxr-xr-x   0 root         (0) root         (0)     1759 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-preparer
--rwxr-xr-x   0 root         (0) root         (0)     1682 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-receiver
--rwxr-xr-x   0 root         (0) root         (0)     3385 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-stager
--rwxr-xr-x   0 root         (0) root         (0)     6750 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-submitter
--rwxr-xr-x   0 root         (0) root         (0)     3859 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-conveyor-throttler
--rwxr-xr-x   0 root         (0) root         (0)     2546 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-dark-reaper
--rwxr-xr-x   0 root         (0) root         (0)     6463 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-dumper
--rwxr-xr-x   0 root         (0) root         (0)     1414 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-follower
--rwxr-xr-x   0 root         (0) root         (0)     1987 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-hermes
--rwxr-xr-x   0 root         (0) root         (0)     4649 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-judge-cleaner
--rwxr-xr-x   0 root         (0) root         (0)     7470 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-judge-evaluator
--rwxr-xr-x   0 root         (0) root         (0)     1671 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-judge-injector
--rwxr-xr-x   0 root         (0) root         (0)     1675 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-judge-repairer
--rwxr-xr-x   0 root         (0) root         (0)     1782 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-kronos
--rwxr-xr-x   0 root         (0) root         (0)     2260 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-minos
--rwxr-xr-x   0 root         (0) root         (0)     1997 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-minos-temporary-expiration
--rwxr-xr-x   0 root         (0) root         (0)     5625 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-necromancer
--rwxr-xr-x   0 root         (0) root         (0)     2788 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-oauth-manager
--rwxr-xr-x   0 root         (0) root         (0)     4070 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-reaper
--rwxr-xr-x   0 root         (0) root         (0)    18989 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-replica-recoverer
--rwxr-xr-x   0 root         (0) root         (0)     2351 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-rse-decommissioner
--rwxr-xr-x   0 root         (0) root         (0)     3920 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-storage-consistency-actions
--rwxr-xr-x   0 root         (0) root         (0)     3364 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-transmogrifier
--rwxr-xr-x   0 root         (0) root         (0)     2720 2024-03-21 13:32:52.000000 rucio-34.1.0/bin/rucio-undertaker
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.071251 rucio-34.1.0/etc/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/alembic.ini.template
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/alembic_offline.ini.template
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/globus-config.yml.template
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/ldap.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.073251 rucio-34.1.0/etc/mail_templates/
--rw-r--r--   0 root         (0) root         (0)     1210 2024-03-13 10:19:28.000000 rucio-34.1.0/etc/mail_templates/rule_approval_request.tmpl
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/mail_templates/rule_approved_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/mail_templates/rule_approved_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/mail_templates/rule_denied_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/mail_templates/rule_denied_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/mail_templates/rule_ok_notification.tmpl
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.1.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-03-13 10:19:28.000000 rucio-34.1.0/etc/rucio.cfg.template
--rw-r--r--   0 root         (0) root         (0)     7477 2024-03-13 10:19:28.000000 rucio-34.1.0/etc/rucio_multi_vo.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.047251 rucio-34.1.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.074251 rucio-34.1.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.080251 rucio-34.1.0/lib/rucio/api/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9292 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/account.py
--rw-r--r--   0 root         (0) root         (0)    11395 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    12890 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/authentication.py
--rw-r--r--   0 root         (0) root         (0)     8654 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/config.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/credential.py
--rw-r--r--   0 root         (0) root         (0)    28937 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/did.py
--rw-r--r--   0 root         (0) root         (0)     3206 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/exporter.py
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     6830 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/importer.py
--rw-r--r--   0 root         (0) root         (0)     3685 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/lock.py
--rw-r--r--   0 root         (0) root         (0)     3573 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/permission.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    22398 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/replica.py
--rw-r--r--   0 root         (0) root         (0)    10550 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/request.py
--rw-r--r--   0 root         (0) root         (0)    23582 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/rse.py
--rw-r--r--   0 root         (0) root         (0)    15938 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/rule.py
--rw-r--r--   0 root         (0) root         (0)     3003 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/scope.py
--rw-r--r--   0 root         (0) root         (0)    10537 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4559 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/api/vo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.087251 rucio-34.1.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16353 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    47057 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86065 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27124 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12682 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46563 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.092251 rucio-34.1.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2234 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24282 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     3300 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6291 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/didtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.093251 rucio-34.1.0/lib/rucio/common/dumper/
--rw-r--r--   0 root         (0) root         (0)     9151 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/dumper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16073 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/dumper/consistency.py
--rw-r--r--   0 root         (0) root         (0)     9687 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/dumper/data_models.py
--rw-r--r--   0 root         (0) root         (0)     1923 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/dumper/path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45297 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6056 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.096251 rucio-34.1.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5152 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18523 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15885 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5069 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79094 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.108251 rucio-34.1.0/lib/rucio/core/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14952 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/account.py
--rw-r--r--   0 root         (0) root         (0)     6293 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/account_counter.py
--rw-r--r--   0 root         (0) root         (0)    14278 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    19785 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/authentication.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/config.py
--rw-r--r--   0 root         (0) root         (0)     8161 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/credential.py
--rw-r--r--   0 root         (0) root         (0)   125614 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.110252 rucio-34.1.0/lib/rucio/core/did_meta_plugins/
--rw-r--r--   0 root         (0) root         (0)    11733 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17475 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
--rw-r--r--   0 root         (0) root         (0)     4078 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
--rw-r--r--   0 root         (0) root         (0)    29313 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     9245 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/json_meta.py
--rw-r--r--   0 root         (0) root         (0)     7453 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
--rw-r--r--   0 root         (0) root         (0)    13727 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
--rw-r--r--   0 root         (0) root         (0)     9406 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/dirac.py
--rw-r--r--   0 root         (0) root         (0)     5695 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/distance.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/exporter.py
--rw-r--r--   0 root         (0) root         (0)    10340 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    11836 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/identity.py
--rw-r--r--   0 root         (0) root         (0)    13839 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/importer.py
--rw-r--r--   0 root         (0) root         (0)    15235 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)    22807 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/lock.py
--rw-r--r--   0 root         (0) root         (0)     9693 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/message.py
--rw-r--r--   0 root         (0) root         (0)     8691 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)    15768 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/monitor.py
--rw-r--r--   0 root         (0) root         (0)     5395 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/naming_convention.py
--rw-r--r--   0 root         (0) root         (0)     4890 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/nongrid_trace.py
--rw-r--r--   0 root         (0) root         (0)    69762 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/oidc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.112252 rucio-34.1.0/lib/rucio/core/permission/
--rw-r--r--   0 root         (0) root         (0)     3910 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55427 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/atlas.py
--rw-r--r--   0 root         (0) root         (0)    46908 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/belleii.py
--rw-r--r--   0 root         (0) root         (0)    46757 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/cms.py
--rw-r--r--   0 root         (0) root         (0)    43104 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/escape.py
--rw-r--r--   0 root         (0) root         (0)    45307 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/generic.py
--rw-r--r--   0 root         (0) root         (0)    45853 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/permission/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     8029 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)   177307 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/core/replica.py
--rw-r--r--   0 root         (0) root         (0)    15420 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/replica_sorter.py
--rw-r--r--   0 root         (0) root         (0)   116242 2024-04-02 11:36:32.000000 rucio-34.1.0/lib/rucio/core/request.py
--rw-r--r--   0 root         (0) root         (0)    67929 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/rse.py
--rw-r--r--   0 root         (0) root         (0)     5510 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/rse_counter.py
--rw-r--r--   0 root         (0) root         (0)    15369 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)    13932 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/core/rse_selector.py
--rw-r--r--   0 root         (0) root         (0)   208340 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/rule.py
--rw-r--r--   0 root         (0) root         (0)    92255 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/rule_grouping.py
--rw-r--r--   0 root         (0) root         (0)     5364 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/scope.py
--rw-r--r--   0 root         (0) root         (0)    15232 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/subscription.py
--rw-r--r--   0 root         (0) root         (0)    18667 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/topology.py
--rw-r--r--   0 root         (0) root         (0)    13107 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/trace.py
--rw-r--r--   0 root         (0) root         (0)    64150 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/transfer.py
--rw-r--r--   0 root         (0) root         (0)     5507 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/vo.py
--rw-r--r--   0 root         (0) root         (0)     5070 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/core/volatile_replica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.112252 rucio-34.1.0/lib/rucio/daemons/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.113252 rucio-34.1.0/lib/rucio/daemons/abacus/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/abacus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3736 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/abacus/account.py
--rw-r--r--   0 root         (0) root         (0)     3856 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/abacus/collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/abacus/rse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.114251 rucio-34.1.0/lib/rucio/daemons/atropos/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/atropos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10559 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/atropos/atropos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.115252 rucio-34.1.0/lib/rucio/daemons/auditor/
--rw-r--r--   0 root         (0) root         (0)     9998 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/auditor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2865 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/auditor/hdfs.py
--rw-r--r--   0 root         (0) root         (0)     8616 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/auditor/srmdumps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.115252 rucio-34.1.0/lib/rucio/daemons/automatix/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/automatix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9914 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/automatix/automatix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.116252 rucio-34.1.0/lib/rucio/daemons/badreplicas/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/badreplicas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15768 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/badreplicas/minos.py
--rw-r--r--   0 root         (0) root         (0)     8626 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
--rw-r--r--   0 root         (0) root         (0)     9892 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/badreplicas/necromancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.118252 rucio-34.1.0/lib/rucio/daemons/bb8/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/bb8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13071 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/bb8/bb8.py
--rw-r--r--   0 root         (0) root         (0)    26597 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/bb8/common.py
--rw-r--r--   0 root         (0) root         (0)     6644 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
--rw-r--r--   0 root         (0) root         (0)     6522 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.118252 rucio-34.1.0/lib/rucio/daemons/c3po/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.120252 rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4571 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/simple.py
--rw-r--r--   0 root         (0) root         (0)     4651 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
--rw-r--r--   0 root         (0) root         (0)    12151 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
--rw-r--r--   0 root         (0) root         (0)    15009 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/c3po.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.121252 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3261 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/agis.py
--rw-r--r--   0 root         (0) root         (0)     2094 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/free_space.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
--rw-r--r--   0 root         (0) root         (0)     1338 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/mock_did.py
--rw-r--r--   0 root         (0) root         (0)     2068 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3818 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/collectors/workload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.123252 rucio-34.1.0/lib/rucio/daemons/c3po/utils/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1386 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1523 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/utils/expiring_list.py
--rw-r--r--   0 root         (0) root         (0)     2440 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/utils/popularity.py
--rw-r--r--   0 root         (0) root         (0)     2087 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/c3po/utils/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.123252 rucio-34.1.0/lib/rucio/daemons/cache/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.1.0/lib/rucio/daemons/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6744 2024-03-13 10:19:28.000000 rucio-34.1.0/lib/rucio/daemons/cache/consumer.py
--rw-r--r--   0 root         (0) root         (0)    14947 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.126252 rucio-34.1.0/lib/rucio/daemons/conveyor/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25768 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/common.py
--rw-r--r--   0 root         (0) root         (0)    23644 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/finisher.py
--rw-r--r--   0 root         (0) root         (0)    16242 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/poller.py
--rw-r--r--   0 root         (0) root         (0)     7462 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/preparer.py
--rw-r--r--   0 root         (0) root         (0)     8289 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/receiver.py
--rw-r--r--   0 root         (0) root         (0)     3827 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/stager.py
--rw-r--r--   0 root         (0) root         (0)    16333 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/submitter.py
--rw-r--r--   0 root         (0) root         (0)    20351 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/conveyor/throttler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.127252 rucio-34.1.0/lib/rucio/daemons/follower/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/follower/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3355 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/follower/follower.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.127252 rucio-34.1.0/lib/rucio/daemons/hermes/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/hermes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26436 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/hermes/hermes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.129252 rucio-34.1.0/lib/rucio/daemons/judge/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5758 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/judge/cleaner.py
--rw-r--r--   0 root         (0) root         (0)     7156 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/judge/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     6352 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/judge/injector.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/judge/repairer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.129252 rucio-34.1.0/lib/rucio/daemons/oauthmanager/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/oauthmanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8815 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.130252 rucio-34.1.0/lib/rucio/daemons/reaper/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/reaper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11222 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/reaper/dark_reaper.py
--rw-r--r--   0 root         (0) root         (0)    35532 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/reaper/reaper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.131252 rucio-34.1.0/lib/rucio/daemons/replicarecoverer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/replicarecoverer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    33150 2024-04-02 11:24:52.000000 rucio-34.1.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.131252 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2671 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.132252 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/
--rw-r--r--   0 root         (0) root         (0)      863 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
--rw-r--r--   0 root         (0) root         (0)    16231 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
--rw-r--r--   0 root         (0) root         (0)     2927 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
--rw-r--r--   0 root         (0) root         (0)    10358 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.133252 rucio-34.1.0/lib/rucio/daemons/storage/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.133252 rucio-34.1.0/lib/rucio/daemons/storage/consistency/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/storage/consistency/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29563 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/storage/consistency/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.134252 rucio-34.1.0/lib/rucio/daemons/tracer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/tracer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23764 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/tracer/kronos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.134252 rucio-34.1.0/lib/rucio/daemons/transmogrifier/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/transmogrifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30528 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.135252 rucio-34.1.0/lib/rucio/daemons/undertaker/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/undertaker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/daemons/undertaker/undertaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.135252 rucio-34.1.0/lib/rucio/db/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.137252 rucio-34.1.0/lib/rucio/db/sqla/
--rw-r--r--   0 root         (0) root         (0)     2130 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4151 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.138252 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3545 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.163252 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/
--rw-r--r--   0 root         (0) root         (0)     3340 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
--rw-r--r--   0 root         (0) root         (0)     1533 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     5272 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
--rw-r--r--   0 root         (0) root         (0)     1548 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
--rw-r--r--   0 root         (0) root         (0)     2816 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1260 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
--rw-r--r--   0 root         (0) root         (0)     1678 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
--rw-r--r--   0 root         (0) root         (0)     2675 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
--rw-r--r--   0 root         (0) root         (0)     8494 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
--rw-r--r--   0 root         (0) root         (0)     3277 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3782 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
--rw-r--r--   0 root         (0) root         (0)     4360 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
--rw-r--r--   0 root         (0) root         (0)     2781 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
--rw-r--r--   0 root         (0) root         (0)     2297 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     2274 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
--rw-r--r--   0 root         (0) root         (0)     2206 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
--rw-r--r--   0 root         (0) root         (0)     2837 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
--rw-r--r--   0 root         (0) root         (0)     1554 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
--rw-r--r--   0 root         (0) root         (0)     3882 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3997 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2817 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     7527 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2396 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     3592 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     2777 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     1644 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
--rw-r--r--   0 root         (0) root         (0)     2424 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
--rw-r--r--   0 root         (0) root         (0)     1598 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     1526 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
--rw-r--r--   0 root         (0) root         (0)     2363 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     6101 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
--rw-r--r--   0 root         (0) root         (0)     1969 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
--rw-r--r--   0 root         (0) root         (0)     5023 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
--rw-r--r--   0 root         (0) root         (0)     3568 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
--rw-r--r--   0 root         (0) root         (0)     1661 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
--rw-r--r--   0 root         (0) root         (0)     1715 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
--rw-r--r--   0 root         (0) root         (0)     3118 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1749 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
--rw-r--r--   0 root         (0) root         (0)     5038 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
--rw-r--r--   0 root         (0) root         (0)     3689 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
--rw-r--r--   0 root         (0) root         (0)     2614 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
--rw-r--r--   0 root         (0) root         (0)     3117 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
--rw-r--r--   0 root         (0) root         (0)     5836 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
--rw-r--r--   0 root         (0) root         (0)     1348 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
--rw-r--r--   0 root         (0) root         (0)     7344 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
--rw-r--r--   0 root         (0) root         (0)     2934 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
--rw-r--r--   0 root         (0) root         (0)     2784 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     9561 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1594 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
--rw-r--r--   0 root         (0) root         (0)     5263 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
--rw-r--r--   0 root         (0) root         (0)     2947 2024-03-21 13:32:52.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
--rw-r--r--   0 root         (0) root         (0)     1949 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
--rw-r--r--   0 root         (0) root         (0)     1110 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
--rw-r--r--   0 root         (0) root         (0)     1599 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
--rw-r--r--   0 root         (0) root         (0)   112135 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/models.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/sautils.py
--rw-r--r--   0 root         (0) root         (0)    17773 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/session.py
--rw-r--r--   0 root         (0) root         (0)     6088 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/types.py
--rw-r--r--   0 root         (0) root         (0)    21427 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/db/sqla/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.164252 rucio-34.1.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.167252 rucio-34.1.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7198 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29093 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9680 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3409 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10394 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22650 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15256 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14651 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17467 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8127 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22166 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12567 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.167252 rucio-34.1.0/lib/rucio/tests/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7837 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/tests/common_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.169252 rucio-34.1.0/lib/rucio/transfertool/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8299 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     1711 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/bittorrent_driver.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
--rw-r--r--   0 root         (0) root         (0)    72072 2024-04-02 11:45:21.000000 rucio-34.1.0/lib/rucio/transfertool/fts3.py
--rw-r--r--   0 root         (0) root         (0)     6136 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/fts3_plugins.py
--rw-r--r--   0 root         (0) root         (0)     7656 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/globus.py
--rw-r--r--   0 root         (0) root         (0)     8411 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/globus_library.py
--rw-r--r--   0 root         (0) root         (0)     2859 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/mock.py
--rw-r--r--   0 root         (0) root         (0)     7753 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/transfertool/transfertool.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-02 11:50:17.000000 rucio-34.1.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1549 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.169252 rucio-34.1.0/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.170252 rucio-34.1.0/lib/rucio/web/rest/
--rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.170252 rucio-34.1.0/lib/rucio/web/rest/flaskapi/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.176252 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
--rw-r--r--   0 root         (0) root         (0)    36983 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
--rw-r--r--   0 root         (0) root         (0)     3344 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/archives.py
--rw-r--r--   0 root         (0) root         (0)    61575 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/auth.py
--rw-r--r--   0 root         (0) root         (0)    16147 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/common.py
--rw-r--r--   0 root         (0) root         (0)    10143 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/config.py
--rw-r--r--   0 root         (0) root         (0)     7718 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
--rw-r--r--   0 root         (0) root         (0)    80863 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/dids.py
--rw-r--r--   0 root         (0) root         (0)     4706 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2656 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/export.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     7894 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/identities.py
--rw-r--r--   0 root         (0) root         (0)     5257 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/import.py
--rw-r--r--   0 root         (0) root         (0)    12007 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12990 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/locks.py
--rw-r--r--   0 root         (0) root         (0)     2861 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/main.py
--rw-r--r--   0 root         (0) root         (0)     7784 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
--rw-r--r--   0 root         (0) root         (0)     3096 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/ping.py
--rw-r--r--   0 root         (0) root         (0)    13331 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
--rw-r--r--   0 root         (0) root         (0)    72710 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
--rw-r--r--   0 root         (0) root         (0)    41600 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/requests.py
--rw-r--r--   0 root         (0) root         (0)    81945 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/rses.py
--rw-r--r--   0 root         (0) root         (0)    31870 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/rules.py
--rw-r--r--   0 root         (0) root         (0)     5068 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
--rw-r--r--   0 root         (0) root         (0)    24149 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.177252 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/templates/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
--rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
--rw-r--r--   0 root         (0) root         (0)     3213 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/traces.py
--rw-r--r--   0 root         (0) root         (0)     9154 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/vos.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/main.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1010 2024-03-21 13:32:51.000000 rucio-34.1.0/lib/rucio/web/rest/ping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.194252 rucio-34.1.0/lib/rucio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25997 2024-04-02 13:57:05.000000 rucio-34.1.0/lib/rucio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-34.1.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio-34.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-03-19 15:04:29.000000 rucio-34.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-02 13:57:05.199252 rucio-34.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-02 13:57:01.000000 rucio-34.1.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio-34.1.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.194252 rucio-34.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     6929 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio-34.1.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio-34.1.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio-34.1.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:05.194252 rucio-34.1.0/tools/
--rwxr-xr-x   0 root         (0) root         (0)     1259 2024-03-21 13:32:51.000000 rucio-34.1.0/tools/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     6163 2024-03-21 13:32:51.000000 rucio-34.1.0/tools/merge_rucio_configs.py
--rwxr-xr-x   0 root         (0) root         (0)     1351 2024-03-21 13:32:51.000000 rucio-34.1.0/tools/reset_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.839003 rucio-34.2.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio-34.2.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.2.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-16 10:34:59.000000 rucio-34.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2799 2024-04-16 10:35:03.839003 rucio-34.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-16 07:53:27.000000 rucio-34.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.696002 rucio-34.2.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127117 2024-04-09 08:44:02.000000 rucio-34.2.0/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)     2820 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-abacus-account
+-rwxr-xr-x   0 root         (0) root         (0)     1823 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-abacus-collection-replica
+-rwxr-xr-x   0 root         (0) root         (0)     2567 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-abacus-rse
+-rwxr-xr-x   0 root         (0) root         (0)   133531 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-admin
+-rwxr-xr-x   0 root         (0) root         (0)     3185 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-atropos
+-rwxr-xr-x   0 root         (0) root         (0)     5849 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-auditor
+-rwxr-xr-x   0 root         (0) root         (0)     2008 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-automatix
+-rwxr-xr-x   0 root         (0) root         (0)     3103 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-bb8
+-rwxr-xr-x   0 root         (0) root         (0)     6100 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-c3po
+-rwxr-xr-x   0 root         (0) root         (0)     5060 2024-04-08 15:35:56.000000 rucio-34.2.0/bin/rucio-cache-client
+-rwxr-xr-x   0 root         (0) root         (0)     1362 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-cache-consumer
+-rwxr-xr-x   0 root         (0) root         (0)     2346 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-finisher
+-rwxr-xr-x   0 root         (0) root         (0)     2839 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-poller
+-rwxr-xr-x   0 root         (0) root         (0)     1759 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-preparer
+-rwxr-xr-x   0 root         (0) root         (0)     1682 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-receiver
+-rwxr-xr-x   0 root         (0) root         (0)     3385 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-stager
+-rwxr-xr-x   0 root         (0) root         (0)     6750 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-submitter
+-rwxr-xr-x   0 root         (0) root         (0)     3859 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-throttler
+-rwxr-xr-x   0 root         (0) root         (0)     2546 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-dark-reaper
+-rwxr-xr-x   0 root         (0) root         (0)     6463 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-dumper
+-rwxr-xr-x   0 root         (0) root         (0)     1414 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-follower
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-hermes
+-rwxr-xr-x   0 root         (0) root         (0)     4649 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-cleaner
+-rwxr-xr-x   0 root         (0) root         (0)     7470 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-evaluator
+-rwxr-xr-x   0 root         (0) root         (0)     1671 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-injector
+-rwxr-xr-x   0 root         (0) root         (0)     1675 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-repairer
+-rwxr-xr-x   0 root         (0) root         (0)     1782 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-kronos
+-rwxr-xr-x   0 root         (0) root         (0)     2260 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-minos
+-rwxr-xr-x   0 root         (0) root         (0)     1997 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-minos-temporary-expiration
+-rwxr-xr-x   0 root         (0) root         (0)     5625 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-necromancer
+-rwxr-xr-x   0 root         (0) root         (0)     2788 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-oauth-manager
+-rwxr-xr-x   0 root         (0) root         (0)     4070 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-reaper
+-rwxr-xr-x   0 root         (0) root         (0)    18989 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-replica-recoverer
+-rwxr-xr-x   0 root         (0) root         (0)     2351 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-rse-decommissioner
+-rwxr-xr-x   0 root         (0) root         (0)     3920 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-storage-consistency-actions
+-rwxr-xr-x   0 root         (0) root         (0)     3364 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-transmogrifier
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-undertaker
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.698001 rucio-34.2.0/etc/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/alembic.ini.template
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/alembic_offline.ini.template
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/globus-config.yml.template
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/ldap.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.700002 rucio-34.2.0/etc/mail_templates/
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-03-13 10:19:28.000000 rucio-34.2.0/etc/mail_templates/rule_approval_request.tmpl
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_approved_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_approved_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_denied_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_denied_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_ok_notification.tmpl
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-03-13 10:19:28.000000 rucio-34.2.0/etc/rucio.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-03-13 10:19:28.000000 rucio-34.2.0/etc/rucio_multi_vo.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.674001 rucio-34.2.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.701002 rucio-34.2.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.708002 rucio-34.2.0/lib/rucio/api/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9292 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/account.py
+-rw-r--r--   0 root         (0) root         (0)    11395 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     8654 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/config.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/credential.py
+-rw-r--r--   0 root         (0) root         (0)    28937 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/did.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/exporter.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/importer.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/lock.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/permission.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    22398 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/replica.py
+-rw-r--r--   0 root         (0) root         (0)    10550 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/request.py
+-rw-r--r--   0 root         (0) root         (0)    23582 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/rse.py
+-rw-r--r--   0 root         (0) root         (0)    15938 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/rule.py
+-rw-r--r--   0 root         (0) root         (0)     3003 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/scope.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4559 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/vo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.715002 rucio-34.2.0/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16353 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    47980 2024-04-08 15:35:56.000000 rucio-34.2.0/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    86092 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27124 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12682 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46563 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.719002 rucio-34.2.0/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24284 2024-04-08 15:14:19.000000 rucio-34.2.0/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6291 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/didtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.721002 rucio-34.2.0/lib/rucio/common/dumper/
+-rw-r--r--   0 root         (0) root         (0)     9762 2024-04-10 15:37:02.000000 rucio-34.2.0/lib/rucio/common/dumper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15982 2024-04-08 15:35:56.000000 rucio-34.2.0/lib/rucio/common/dumper/consistency.py
+-rw-r--r--   0 root         (0) root         (0)     9687 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/dumper/data_models.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/dumper/path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45297 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6056 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.723002 rucio-34.2.0/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5152 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    18523 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/cms.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)    15885 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/lsst.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5069 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79128 2024-04-08 15:14:19.000000 rucio-34.2.0/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.737002 rucio-34.2.0/lib/rucio/core/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14952 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/account.py
+-rw-r--r--   0 root         (0) root         (0)     6293 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/account_counter.py
+-rw-r--r--   0 root         (0) root         (0)    14278 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    19785 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/config.py
+-rw-r--r--   0 root         (0) root         (0)     8161 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/credential.py
+-rw-r--r--   0 root         (0) root         (0)   125614 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.739002 rucio-34.2.0/lib/rucio/core/did_meta_plugins/
+-rw-r--r--   0 root         (0) root         (0)    11733 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17475 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4078 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     9245 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/json_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7453 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
+-rw-r--r--   0 root         (0) root         (0)     9406 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/distance.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/exporter.py
+-rw-r--r--   0 root         (0) root         (0)    10340 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    11836 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/identity.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2024-04-09 11:14:59.000000 rucio-34.2.0/lib/rucio/core/importer.py
+-rw-r--r--   0 root         (0) root         (0)    15235 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)    22807 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/lock.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)    15768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/nongrid_trace.py
+-rw-r--r--   0 root         (0) root         (0)    69761 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/oidc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.742002 rucio-34.2.0/lib/rucio/core/permission/
+-rw-r--r--   0 root         (0) root         (0)     3910 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55427 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    46908 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    46757 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/cms.py
+-rw-r--r--   0 root         (0) root         (0)    43104 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/escape.py
+-rw-r--r--   0 root         (0) root         (0)    45307 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/generic.py
+-rw-r--r--   0 root         (0) root         (0)    45853 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     8029 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)   177321 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/replica.py
+-rw-r--r--   0 root         (0) root         (0)    15420 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/replica_sorter.py
+-rw-r--r--   0 root         (0) root         (0)   116256 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/request.py
+-rw-r--r--   0 root         (0) root         (0)    67929 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rse.py
+-rw-r--r--   0 root         (0) root         (0)     5510 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rse_counter.py
+-rw-r--r--   0 root         (0) root         (0)    15369 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)    13946 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)   208340 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rule.py
+-rw-r--r--   0 root         (0) root         (0)    92255 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rule_grouping.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/scope.py
+-rw-r--r--   0 root         (0) root         (0)    15232 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    18667 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/topology.py
+-rw-r--r--   0 root         (0) root         (0)    13107 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/trace.py
+-rw-r--r--   0 root         (0) root         (0)    64150 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     5613 2024-04-08 15:24:34.000000 rucio-34.2.0/lib/rucio/core/vo.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/volatile_replica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.742002 rucio-34.2.0/lib/rucio/daemons/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.743002 rucio-34.2.0/lib/rucio/daemons/abacus/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/account.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/rse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.744002 rucio-34.2.0/lib/rucio/daemons/atropos/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/atropos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10574 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/atropos/atropos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.745002 rucio-34.2.0/lib/rucio/daemons/auditor/
+-rw-r--r--   0 root         (0) root         (0)     9998 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/auditor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/auditor/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)    10248 2024-04-10 15:37:02.000000 rucio-34.2.0/lib/rucio/daemons/auditor/srmdumps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.745002 rucio-34.2.0/lib/rucio/daemons/automatix/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/automatix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/automatix/automatix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.746002 rucio-34.2.0/lib/rucio/daemons/badreplicas/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/minos.py
+-rw-r--r--   0 root         (0) root         (0)     8626 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
+-rw-r--r--   0 root         (0) root         (0)     9892 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/necromancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.748002 rucio-34.2.0/lib/rucio/daemons/bb8/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13071 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/bb8.py
+-rw-r--r--   0 root         (0) root         (0)    26597 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/common.py
+-rw-r--r--   0 root         (0) root         (0)     6644 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
+-rw-r--r--   0 root         (0) root         (0)     6522 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.748002 rucio-34.2.0/lib/rucio/daemons/c3po/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.750002 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/simple.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
+-rw-r--r--   0 root         (0) root         (0)    12151 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
+-rw-r--r--   0 root         (0) root         (0)    15009 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/c3po.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.751002 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/agis.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/free_space.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/mock_did.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.753002 rucio-34.2.0/lib/rucio/daemons/c3po/utils/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_list.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/popularity.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.753002 rucio-34.2.0/lib/rucio/daemons/cache/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.2.0/lib/rucio/daemons/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6744 2024-03-13 10:19:28.000000 rucio-34.2.0/lib/rucio/daemons/cache/consumer.py
+-rw-r--r--   0 root         (0) root         (0)    14947 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.756002 rucio-34.2.0/lib/rucio/daemons/conveyor/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/common.py
+-rw-r--r--   0 root         (0) root         (0)    23644 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/finisher.py
+-rw-r--r--   0 root         (0) root         (0)    16242 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/poller.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/preparer.py
+-rw-r--r--   0 root         (0) root         (0)     8289 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/stager.py
+-rw-r--r--   0 root         (0) root         (0)    16333 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/submitter.py
+-rw-r--r--   0 root         (0) root         (0)    20351 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/throttler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.757002 rucio-34.2.0/lib/rucio/daemons/follower/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/follower/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/follower/follower.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.757002 rucio-34.2.0/lib/rucio/daemons/hermes/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/hermes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26436 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/hermes/hermes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.759002 rucio-34.2.0/lib/rucio/daemons/judge/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5772 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/cleaner.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     6394 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/injector.py
+-rw-r--r--   0 root         (0) root         (0)     5310 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/repairer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.759002 rucio-34.2.0/lib/rucio/daemons/oauthmanager/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/oauthmanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.760002 rucio-34.2.0/lib/rucio/daemons/reaper/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/reaper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/reaper/dark_reaper.py
+-rw-r--r--   0 root         (0) root         (0)    35532 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/reaper/reaper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.760002 rucio-34.2.0/lib/rucio/daemons/replicarecoverer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/replicarecoverer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    33150 2024-04-05 14:57:55.000000 rucio-34.2.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.761002 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.763002 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/
+-rw-r--r--   0 root         (0) root         (0)      863 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    16231 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.763002 rucio-34.2.0/lib/rucio/daemons/storage/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.763002 rucio-34.2.0/lib/rucio/daemons/storage/consistency/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/storage/consistency/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29563 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/storage/consistency/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.764002 rucio-34.2.0/lib/rucio/daemons/tracer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/tracer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23764 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/tracer/kronos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.765002 rucio-34.2.0/lib/rucio/daemons/transmogrifier/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/transmogrifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30528 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.765002 rucio-34.2.0/lib/rucio/daemons/undertaker/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/undertaker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/undertaker/undertaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.766002 rucio-34.2.0/lib/rucio/db/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.769002 rucio-34.2.0/lib/rucio/db/sqla/
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.769002 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.801003 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/
+-rw-r--r--   0 root         (0) root         (0)     3340 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
+-rw-r--r--   0 root         (0) root         (0)     8494 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
+-rw-r--r--   0 root         (0) root         (0)     3882 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     6101 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     9561 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
+-rw-r--r--   0 root         (0) root         (0)   112135 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/models.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/sautils.py
+-rw-r--r--   0 root         (0) root         (0)    17773 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/session.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/types.py
+-rw-r--r--   0 root         (0) root         (0)    21427 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.801003 rucio-34.2.0/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.805003 rucio-34.2.0/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29093 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9680 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10394 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    22650 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14651 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17467 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8127 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22166 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12567 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37238 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.805003 rucio-34.2.0/lib/rucio/tests/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8879 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/tests/common_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.807003 rucio-34.2.0/lib/rucio/transfertool/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8299 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
+-rw-r--r--   0 root         (0) root         (0)    72072 2024-04-02 11:45:21.000000 rucio-34.2.0/lib/rucio/transfertool/fts3.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/fts3_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     7656 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/globus.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/globus_library.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7753 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/transfertool.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-16 07:53:37.000000 rucio-34.2.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-08 15:22:52.000000 rucio-34.2.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.807003 rucio-34.2.0/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.808003 rucio-34.2.0/lib/rucio/web/rest/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.808003 rucio-34.2.0/lib/rucio/web/rest/flaskapi/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.814003 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
+-rw-r--r--   0 root         (0) root         (0)    36983 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/archives.py
+-rw-r--r--   0 root         (0) root         (0)    61575 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/auth.py
+-rw-r--r--   0 root         (0) root         (0)    16147 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/common.py
+-rw-r--r--   0 root         (0) root         (0)    10143 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/config.py
+-rw-r--r--   0 root         (0) root         (0)     7718 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    80863 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dids.py
+-rw-r--r--   0 root         (0) root         (0)     4706 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/export.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     7894 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/identities.py
+-rw-r--r--   0 root         (0) root         (0)     5257 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/import.py
+-rw-r--r--   0 root         (0) root         (0)    12007 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12990 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/locks.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/main.py
+-rw-r--r--   0 root         (0) root         (0)     7784 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/ping.py
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
+-rw-r--r--   0 root         (0) root         (0)    72710 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
+-rw-r--r--   0 root         (0) root         (0)    41600 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/requests.py
+-rw-r--r--   0 root         (0) root         (0)    81945 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rses.py
+-rw-r--r--   0 root         (0) root         (0)    31870 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rules.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
+-rw-r--r--   0 root         (0) root         (0)    24149 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.815003 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/traces.py
+-rw-r--r--   0 root         (0) root         (0)     9154 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/vos.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/main.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/ping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.834003 rucio-34.2.0/lib/rucio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25997 2024-04-16 10:35:03.000000 rucio-34.2.0/lib/rucio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-34.2.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio-34.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-04-16 07:53:27.000000 rucio-34.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-16 10:35:03.840003 rucio-34.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-16 10:34:59.000000 rucio-34.2.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio-34.2.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.833003 rucio-34.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-04-08 15:14:19.000000 rucio-34.2.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.834003 rucio-34.2.0/tools/
+-rwxr-xr-x   0 root         (0) root         (0)     1259 2024-03-21 13:32:51.000000 rucio-34.2.0/tools/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-03-21 13:32:51.000000 rucio-34.2.0/tools/merge_rucio_configs.py
+-rwxr-xr-x   0 root         (0) root         (0)     1351 2024-03-21 13:32:51.000000 rucio-34.2.0/tools/reset_database.py
```

### Comparing `rucio-34.1.0/AUTHORS.rst` & `rucio-34.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/LICENSE` & `rucio-34.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/MANIFEST.in` & `rucio-34.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/PKG-INFO` & `rucio-34.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio
-Version: 34.1.0
+Version: 34.2.0
 Summary: Rucio Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-34.1.0/README.rst` & `rucio-34.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio` & `rucio-34.2.0/bin/rucio`

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

### Comparing `rucio-34.1.0/bin/rucio-abacus-account` & `rucio-34.2.0/bin/rucio-abacus-account`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-abacus-collection-replica` & `rucio-34.2.0/bin/rucio-abacus-collection-replica`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-abacus-rse` & `rucio-34.2.0/bin/rucio-abacus-rse`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-admin` & `rucio-34.2.0/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-atropos` & `rucio-34.2.0/bin/rucio-atropos`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-auditor` & `rucio-34.2.0/bin/rucio-auditor`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-automatix` & `rucio-34.2.0/bin/rucio-automatix`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-bb8` & `rucio-34.2.0/bin/rucio-bb8`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-c3po` & `rucio-34.2.0/bin/rucio-c3po`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-cache-client` & `rucio-34.2.0/bin/rucio-cache-client`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
     Rucio Cache client.
 """
 
 import argparse
 import json
 import os
-import random
+import secrets
 import ssl
 import sys
 
 import stomp
 from jsonschema import validate
 
 from rucio.client.didclient import DIDClient
@@ -75,15 +75,15 @@
         validate_files(payload["files"])
     else:
         validate(payload, get_schema_value('CACHE_DELETE_REPLICAS'))
     conn = stomp.Connection([(args.broker, args.port)])
     conn.set_ssl(key_file=args.ssl_key_file, cert_file=args.ssl_cert_file, ssl_version=ssl.PROTOCOL_TLSv1)
 
     conn.connect()
-    message = {'id': int(random.random() * 1000), 'payload': payload}
+    message = {'id': secrets.randbelow(1001), 'payload': payload}
     conn.send(destination=args.destination, body=json.dumps(message), id='rucio-cache-messaging', ack='auto', headers={'vo': 'atlas'})
     conn.disconnect()
 
 
 def get_parser():
     """
     Returns the argparse parser.
```

### Comparing `rucio-34.1.0/bin/rucio-cache-consumer` & `rucio-34.2.0/bin/rucio-cache-consumer`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-finisher` & `rucio-34.2.0/bin/rucio-conveyor-finisher`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-poller` & `rucio-34.2.0/bin/rucio-conveyor-poller`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-preparer` & `rucio-34.2.0/bin/rucio-conveyor-preparer`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-receiver` & `rucio-34.2.0/bin/rucio-conveyor-receiver`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-stager` & `rucio-34.2.0/bin/rucio-conveyor-stager`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-submitter` & `rucio-34.2.0/bin/rucio-conveyor-submitter`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-conveyor-throttler` & `rucio-34.2.0/bin/rucio-conveyor-throttler`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-dark-reaper` & `rucio-34.2.0/bin/rucio-dark-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-dumper` & `rucio-34.2.0/bin/rucio-dumper`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-follower` & `rucio-34.2.0/bin/rucio-follower`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-hermes` & `rucio-34.2.0/bin/rucio-hermes`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-judge-cleaner` & `rucio-34.2.0/bin/rucio-judge-cleaner`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-judge-evaluator` & `rucio-34.2.0/bin/rucio-judge-evaluator`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-judge-injector` & `rucio-34.2.0/bin/rucio-judge-injector`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-judge-repairer` & `rucio-34.2.0/bin/rucio-judge-repairer`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-kronos` & `rucio-34.2.0/bin/rucio-kronos`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-minos` & `rucio-34.2.0/bin/rucio-minos`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-minos-temporary-expiration` & `rucio-34.2.0/bin/rucio-minos-temporary-expiration`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-necromancer` & `rucio-34.2.0/bin/rucio-necromancer`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-oauth-manager` & `rucio-34.2.0/bin/rucio-oauth-manager`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-reaper` & `rucio-34.2.0/bin/rucio-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-replica-recoverer` & `rucio-34.2.0/bin/rucio-replica-recoverer`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-rse-decommissioner` & `rucio-34.2.0/bin/rucio-rse-decommissioner`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-storage-consistency-actions` & `rucio-34.2.0/bin/rucio-storage-consistency-actions`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-transmogrifier` & `rucio-34.2.0/bin/rucio-transmogrifier`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/bin/rucio-undertaker` & `rucio-34.2.0/bin/rucio-undertaker`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/alembic.ini.template` & `rucio-34.2.0/etc/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/alembic_offline.ini.template` & `rucio-34.2.0/etc/alembic_offline.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/ldap.cfg.template` & `rucio-34.2.0/etc/ldap.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/mail_templates/rule_approval_request.tmpl` & `rucio-34.2.0/etc/mail_templates/rule_approval_request.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/mail_templates/rule_ok_notification.tmpl` & `rucio-34.2.0/etc/mail_templates/rule_ok_notification.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/rse-accounts.cfg.template` & `rucio-34.2.0/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/rucio.cfg.atlas.client.template` & `rucio-34.2.0/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/rucio.cfg.template` & `rucio-34.2.0/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/etc/rucio_multi_vo.cfg.template` & `rucio-34.2.0/etc/rucio_multi_vo.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/__init__.py` & `rucio-34.2.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/alembicrevision.py` & `rucio-34.2.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/__init__.py` & `rucio-34.2.0/lib/rucio/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/account.py` & `rucio-34.2.0/lib/rucio/api/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/account_limit.py` & `rucio-34.2.0/lib/rucio/api/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/authentication.py` & `rucio-34.2.0/lib/rucio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/config.py` & `rucio-34.2.0/lib/rucio/api/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/credential.py` & `rucio-34.2.0/lib/rucio/api/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/did.py` & `rucio-34.2.0/lib/rucio/api/did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/dirac.py` & `rucio-34.2.0/lib/rucio/api/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/exporter.py` & `rucio-34.2.0/lib/rucio/api/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/heartbeat.py` & `rucio-34.2.0/lib/rucio/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/identity.py` & `rucio-34.2.0/lib/rucio/api/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/importer.py` & `rucio-34.2.0/lib/rucio/api/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/lifetime_exception.py` & `rucio-34.2.0/lib/rucio/api/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/lock.py` & `rucio-34.2.0/lib/rucio/api/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/meta_conventions.py` & `rucio-34.2.0/lib/rucio/api/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/permission.py` & `rucio-34.2.0/lib/rucio/api/permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/quarantined_replica.py` & `rucio-34.2.0/lib/rucio/api/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/replica.py` & `rucio-34.2.0/lib/rucio/api/replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/request.py` & `rucio-34.2.0/lib/rucio/api/request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/rse.py` & `rucio-34.2.0/lib/rucio/api/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/rule.py` & `rucio-34.2.0/lib/rucio/api/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/scope.py` & `rucio-34.2.0/lib/rucio/api/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/subscription.py` & `rucio-34.2.0/lib/rucio/api/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/api/vo.py` & `rucio-34.2.0/lib/rucio/api/vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/__init__.py` & `rucio-34.2.0/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/accountclient.py` & `rucio-34.2.0/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/accountlimitclient.py` & `rucio-34.2.0/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/baseclient.py` & `rucio-34.2.0/lib/rucio/client/baseclient.py`

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

### Comparing `rucio-34.1.0/lib/rucio/client/client.py` & `rucio-34.2.0/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/configclient.py` & `rucio-34.2.0/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/credentialclient.py` & `rucio-34.2.0/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/didclient.py` & `rucio-34.2.0/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/diracclient.py` & `rucio-34.2.0/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/downloadclient.py` & `rucio-34.2.0/lib/rucio/client/downloadclient.py`

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

### Comparing `rucio-34.1.0/lib/rucio/client/exportclient.py` & `rucio-34.2.0/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/fileclient.py` & `rucio-34.2.0/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/importclient.py` & `rucio-34.2.0/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/lifetimeclient.py` & `rucio-34.2.0/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/lockclient.py` & `rucio-34.2.0/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/metaconventionsclient.py` & `rucio-34.2.0/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/pingclient.py` & `rucio-34.2.0/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/replicaclient.py` & `rucio-34.2.0/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/requestclient.py` & `rucio-34.2.0/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/rseclient.py` & `rucio-34.2.0/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/ruleclient.py` & `rucio-34.2.0/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/scopeclient.py` & `rucio-34.2.0/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/subscriptionclient.py` & `rucio-34.2.0/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/touchclient.py` & `rucio-34.2.0/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/client/uploadclient.py` & `rucio-34.2.0/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/__init__.py` & `rucio-34.2.0/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/cache.py` & `rucio-34.2.0/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/config.py` & `rucio-34.2.0/lib/rucio/common/config.py`

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

### Comparing `rucio-34.1.0/lib/rucio/common/constants.py` & `rucio-34.2.0/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/constraints.py` & `rucio-34.2.0/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/didtype.py` & `rucio-34.2.0/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/dumper/__init__.py` & `rucio-34.2.0/lib/rucio/common/dumper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -243,29 +243,43 @@
 def http_download_to_file(url, file_, session=None):
     '''
     Download the file in `url` storing it in the `file_` file-like
     object.
     If given `session` must be a requests.Session instance, and will be
     used to download the file, otherwise requests.get() will be used.
     '''
-    if session is None:
-        response = requests.get(url, stream=True)
-    else:
-        response = session.get(url)
+    def _do_download(url, file_, session, try_decode=False):
+        if session is None:
+            response = requests.get(url, stream=True)
+        else:
+            response = session.get(url)
 
-    if response.status_code != 200:
-        logging.error(
-            'Retrieving %s returned %d status code',
-            url,
-            response.status_code,
-        )
-        raise HTTPDownloadFailed('Error downloading ' + url, response.status_code)
+        if response.status_code != 200:
+            logging.error(
+                'Retrieving %s returned %d status code',
+                url,
+                response.status_code,
+            )
+            raise HTTPDownloadFailed('Error downloading ' + url, response.status_code)
 
-    for chunk in response.iter_content(CHUNK_SIZE):
-        file_.write(chunk)
+        if try_decode:
+            if response.encoding is None:
+                response.encoding = 'utf-8'
+            for chunk in response.iter_content(CHUNK_SIZE, decode_unicode=True):
+                file_.write(chunk)
+        else:
+            for chunk in response.iter_content(CHUNK_SIZE):
+                file_.write(chunk)
+
+    try:
+        # try without decoding first
+        _do_download(url, file_, session, False)
+    except TypeError:
+        # if that fails due to writing binary data to text file, try to force decode
+        _do_download(url, file_, session, True)
 
 
 def http_download(url, filename):
     '''
     Download the file in `url` storing it in the path given by `filename`.
     '''
     with open(filename, 'w') as f:
```

### Comparing `rucio-34.1.0/lib/rucio/common/dumper/consistency.py` & `rucio-34.2.0/lib/rucio/common/dumper/consistency.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,25 +311,23 @@
 
     sorted_name = '_'.join((prefix, 'sorted'))
     sorted_path = os.path.join(cache_dir, sorted_name)
 
     if os.path.exists(sorted_path):
         return sorted_path
 
-    # FIXME: mktemp() is an insecure function and this may be a security
-    # threat in some scenarios. Find another way to do it.
-    tfile = tempfile.mktemp(dir=cache_dir)
+    tfile = tempfile.NamedTemporaryFile(dir=cache_dir, delete=False)
 
     subprocess.check_call(
-        cmd_line.format(file_path, tfile),
+        cmd_line.format(file_path, tfile.name),
         shell=True,
     )
 
-    os.link(tfile, sorted_path)
-    os.unlink(tfile)
+    os.link(tfile.name, sorted_path)
+    os.unlink(tfile.name)
 
     return sorted_path
 
 
 def populate_args(argparser):
     # Option to download the rucio replica dumps automaticaly
     parser = argparser.add_parser(
```

### Comparing `rucio-34.1.0/lib/rucio/common/dumper/data_models.py` & `rucio-34.2.0/lib/rucio/common/dumper/data_models.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/dumper/path_parsing.py` & `rucio-34.2.0/lib/rucio/common/dumper/path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/exception.py` & `rucio-34.2.0/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/extra.py` & `rucio-34.2.0/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/logging.py` & `rucio-34.2.0/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/pcache.py` & `rucio-34.2.0/lib/rucio/common/pcache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/plugins.py` & `rucio-34.2.0/lib/rucio/common/plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/policy.py` & `rucio-34.2.0/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/__init__.py` & `rucio-34.2.0/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/atlas.py` & `rucio-34.2.0/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/belleii.py` & `rucio-34.2.0/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/cms.py` & `rucio-34.2.0/lib/rucio/common/schema/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/domatpc.py` & `rucio-34.2.0/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/escape.py` & `rucio-34.2.0/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/generic.py` & `rucio-34.2.0/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio-34.2.0/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/icecube.py` & `rucio-34.2.0/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/schema/lsst.py` & `rucio-34.2.0/lib/rucio/common/schema/lsst.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/stomp_utils.py` & `rucio-34.2.0/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/stopwatch.py` & `rucio-34.2.0/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/test_rucio_server.py` & `rucio-34.2.0/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/types.py` & `rucio-34.2.0/lib/rucio/common/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/common/utils.py` & `rucio-34.2.0/lib/rucio/common/utils.py`

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

### Comparing `rucio-34.1.0/lib/rucio/core/__init__.py` & `rucio-34.2.0/lib/rucio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/account.py` & `rucio-34.2.0/lib/rucio/core/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/account_counter.py` & `rucio-34.2.0/lib/rucio/core/account_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/account_limit.py` & `rucio-34.2.0/lib/rucio/core/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/authentication.py` & `rucio-34.2.0/lib/rucio/core/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/config.py` & `rucio-34.2.0/lib/rucio/core/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/credential.py` & `rucio-34.2.0/lib/rucio/core/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did.py` & `rucio-34.2.0/lib/rucio/core/did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/__init__.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/did_column_meta.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_column_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/filter_engine.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/json_meta.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/json_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/mongo_meta.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/mongo_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/did_meta_plugins/postgres_meta.py` & `rucio-34.2.0/lib/rucio/core/did_meta_plugins/postgres_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/dirac.py` & `rucio-34.2.0/lib/rucio/core/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/distance.py` & `rucio-34.2.0/lib/rucio/core/distance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/exporter.py` & `rucio-34.2.0/lib/rucio/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/heartbeat.py` & `rucio-34.2.0/lib/rucio/core/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/identity.py` & `rucio-34.2.0/lib/rucio/core/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/importer.py` & `rucio-34.2.0/lib/rucio/core/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from collections.abc import Iterable
+from typing import TYPE_CHECKING, Any
 
 from rucio.common.config import config_get
 from rucio.common.exception import RSEOperationNotSupported
 from rucio.common.types import InternalAccount
 from rucio.core import account as account_module
 from rucio.core import distance as distance_module
 from rucio.core import identity as identity_module
@@ -26,15 +27,15 @@
 from rucio.db.sqla.session import transactional_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @transactional_session
-def import_rses(rses, rse_sync_method='edit', attr_sync_method='edit', protocol_sync_method='edit', vo='def', *, session: "Session"):
+def import_rses(rses: dict[str, dict[str, Any]], rse_sync_method: str = 'edit', attr_sync_method: str = 'edit', protocol_sync_method: str = 'edit', vo: str = 'def', *, session: "Session") -> None:
     new_rses = []
     for rse_name in rses:
         rse = rses[rse_name]
         if isinstance(rse.get('rse_type'), str):
             rse['rse_type'] = RSEType(rse['rse_type'])
 
         if rse_module.rse_exists(rse_name, vo=vo, include_deleted=False, session=session):
@@ -134,15 +135,15 @@
                 try:
                     rse_module.del_rse(rse_id=old_rse, session=session)
                 except RSEOperationNotSupported:
                     pass
 
 
 @transactional_session
-def import_distances(distances, vo='def', *, session: "Session"):
+def import_distances(distances, vo: str = 'def', *, session: "Session") -> None:
     for src_rse_name in distances:
         src = rse_module.get_rse_id(rse=src_rse_name, vo=vo, session=session)
         for dest_rse_name in distances[src_rse_name]:
             dest = rse_module.get_rse_id(rse=dest_rse_name, vo=vo, session=session)
             distance_dict = distances[src_rse_name][dest_rse_name]
             if 'src_rse_id' in distance_dict:
                 del distance_dict['src_rse_id']
@@ -154,15 +155,15 @@
             if old_distance:
                 distance_module.update_distances(src_rse_id=src, dest_rse_id=dest, distance=new_distance, session=session)
             else:
                 distance_module.add_distance(src_rse_id=src, dest_rse_id=dest, distance=new_distance, session=session)
 
 
 @transactional_session
-def import_identities(identities, account_name, old_identities, old_identity_account, account_email, *, session: "Session"):
+def import_identities(identities: Iterable[dict[str, Any]], account_name: str, old_identities: Iterable[tuple], old_identity_account: tuple[str, str, str], account_email: str, *, session: "Session") -> None:
     for identity in identities:
         identity['type'] = IdentityType[identity['type'].upper()]
 
     missing_identities = [identity for identity in identities if (identity['identity'], identity['type']) not in old_identities]
     missing_identity_account = [identity for identity in identities if (identity['identity'], identity['type'], account_name) not in old_identity_account]
     to_be_removed_identity_account = [old_identity for old_identity in old_identity_account if (old_identity[0], old_identity[1], old_identity[2]) not in
                                       [(identity['identity'], identity['type'], account_name) for identity in identities] and old_identity[2] == account_name]
@@ -183,15 +184,15 @@
 
     # remove identities from account-identity association
     for identity in to_be_removed_identity_account:
         identity_module.del_account_identity(identity=identity[0], type_=identity[1], account=identity[2], session=session)
 
 
 @transactional_session
-def import_accounts(accounts, vo='def', *, session: "Session"):
+def import_accounts(accounts: Iterable[dict[str, Any]], vo: str = 'def', *, session: "Session") -> None:
     vo_filter = {'account': InternalAccount(account='*', vo=vo)}
     old_accounts = {account['account']: account for account in account_module.list_accounts(filter_=vo_filter, session=session)}
     missing_accounts = [account for account in accounts if account['account'] not in old_accounts]
     outdated_accounts = [account for account in accounts if account['account'] in old_accounts]
     to_be_removed_accounts = [old_account for old_account in old_accounts if old_account not in [account['account'] for account in accounts]]
     old_identities = identity_module.list_identities(session=session)
     old_identity_account = session.query(models.IdentityAccountAssociation.identity, models.IdentityAccountAssociation.identity_type, models.IdentityAccountAssociation.account).all()
@@ -220,15 +221,15 @@
 
         identities = account_dict.get('identities', [])
         if identities:
             import_identities(identities, account, old_identities, old_identity_account, email, session=session)
 
 
 @transactional_session
-def import_data(data, vo='def', *, session: "Session"):
+def import_data(data: dict[str, Any], vo: str = 'def', *, session: "Session") -> None:
     """
     Import data to add and update records in Rucio.
 
     :param data: data to be imported as dictionary.
     :param session: database session in use.
     """
     rse_sync_method = config_get('importer', 'rse_sync_method', False, 'edit')
```

### Comparing `rucio-34.1.0/lib/rucio/core/lifetime_exception.py` & `rucio-34.2.0/lib/rucio/core/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/lock.py` & `rucio-34.2.0/lib/rucio/core/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/message.py` & `rucio-34.2.0/lib/rucio/core/message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/meta_conventions.py` & `rucio-34.2.0/lib/rucio/core/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/monitor.py` & `rucio-34.2.0/lib/rucio/core/monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/naming_convention.py` & `rucio-34.2.0/lib/rucio/core/naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/nongrid_trace.py` & `rucio-34.2.0/lib/rucio/core/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/oidc.py` & `rucio-34.2.0/lib/rucio/core/oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hashlib
 import json
 import logging
-import random
 import subprocess
 import traceback
 from datetime import datetime, timedelta
 from math import floor
+from secrets import choice
 from typing import TYPE_CHECKING, Any, Final, Optional
 from urllib.parse import parse_qs, urljoin, urlparse
 
 import requests
 from dogpile.cache.api import NoValue
 from jwkest.jws import JWS
 from jwkest.jwt import JWT
@@ -320,15 +320,15 @@
             elif 'issuer' in kwargs:
                 client_secret = next((secrets[i] for i in secrets if 'issuer' in secrets[i] and  # NOQA: W504
                                       kwargs.get('issuer') in secrets[i]['issuer']), None)
             redirect_url = kwargs.get('redirect_uri', None)
             if not redirect_url:
                 redirect_to = kwargs.get("redirect_to", "auth/oidc_token")
                 redirect_urls = [u for u in client_secret["redirect_uris"] if redirect_to in u]
-                redirect_url = random.choice(redirect_urls)
+                redirect_url = choice(redirect_urls)
             if not redirect_url:
                 raise CannotAuthenticate("Could not pick any redirect URL(s) from the ones defined "
                                          + "in Rucio OIDC Client configuration file.")  # NOQA: W503
             auth_args["redirect_uri"] = redirect_url
             oidc_client = OIDC_CLIENTS[client_secret["issuer"]]
             auth_args["client_id"] = oidc_client.client_id
 
@@ -866,15 +866,15 @@
                     if all_oidc_req_claims_present(token.oidc_scope, token.audience, req_scope, req_audience):
                         return token_dictionary(token)
                 # from available tokens select preferentially the one which are being refreshed
                 if hasattr(token, 'oidc_scope') and ('offline_access' in str(token['oidc_scope'])):
                     subject_token = token
             # if not proceed with token exchange
             if not subject_token:
-                subject_token = random.choice(account_tokens)
+                subject_token = choice(account_tokens)
             exchanged_token = __exchange_token_oidc(subject_token,
                                                     scope=req_scope,
                                                     audience=req_audience,
                                                     identity=subject_token.identity,
                                                     refresh_lifetime=subject_token.refresh_lifetime,
                                                     account=account,
                                                     session=session)
```

### Comparing `rucio-34.1.0/lib/rucio/core/permission/__init__.py` & `rucio-34.2.0/lib/rucio/core/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/permission/atlas.py` & `rucio-34.2.0/lib/rucio/core/permission/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/permission/belleii.py` & `rucio-34.2.0/lib/rucio/core/permission/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/permission/cms.py` & `rucio-34.2.0/lib/rucio/core/permission/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/permission/escape.py` & `rucio-34.2.0/lib/rucio/core/permission/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/permission/generic.py` & `rucio-34.2.0/lib/rucio/core/permission/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/permission/generic_multi_vo.py` & `rucio-34.2.0/lib/rucio/core/permission/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/quarantined_replica.py` & `rucio-34.2.0/lib/rucio/core/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/replica.py` & `rucio-34.2.0/lib/rucio/core/replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,15 +646,15 @@
             selected.append(next(iterator))
             i += 1
 
         while True:
             element = next(iterator)
             i += 1
 
-            index_to_substitute = random.randint(0, i)
+            index_to_substitute = random.randint(0, i)  # noqa: S311
             if index_to_substitute < nrandom:
                 selected[index_to_substitute] = element
     except StopIteration:
         pass
 
     for r in selected:
         yield r
```

### Comparing `rucio-34.1.0/lib/rucio/core/replica_sorter.py` & `rucio-34.2.0/lib/rucio/core/replica_sorter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/request.py` & `rucio-34.2.0/lib/rucio/core/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1405,15 +1405,15 @@
         self.downsample_period = math.ceil(raw_retention.total_seconds())
 
     def __enter__(self):
         self.record_stats = config_get_bool('transfers', 'stats_enabled', default=self.record_stats)
         downsample_period = config_get_int('transfers', 'stats_downsample_period', default=self.downsample_period)
         # Introduce some voluntary jitter to reduce the likely-hood of performing this database
         # operation multiple times in parallel.
-        self.downsample_period = random.randint(downsample_period * 3 // 4, math.ceil(downsample_period * 5 / 4))
+        self.downsample_period = random.randint(downsample_period * 3 // 4, math.ceil(downsample_period * 5 / 4))  # noqa: S311
         if self.record_stats:
             self.save_timer = threading.Timer(self.raw_resolution.total_seconds(), self.periodic_save)
             self.save_timer.start()
             self.downsample_timer = threading.Timer(self.downsample_period, self.periodic_downsample_and_cleanup)
             self.downsample_timer.start()
         return self
```

### Comparing `rucio-34.1.0/lib/rucio/core/rse.py` & `rucio-34.2.0/lib/rucio/core/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/rse_counter.py` & `rucio-34.2.0/lib/rucio/core/rse_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/rse_expression_parser.py` & `rucio-34.2.0/lib/rucio/core/rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/rse_selector.py` & `rucio-34.2.0/lib/rucio/core/rse_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         Choose an RSE based on weighting.
 
         :param rses:  The rses to be considered for the choose.
         :return:      The (rse_id, staging_area) tuple of the chosen RSE.
         """
 
         shuffle(rses)
-        pick = uniform(0, sum([rse['weight'] for rse in rses]))
+        pick = uniform(0, sum([rse['weight'] for rse in rses]))  # noqa: S311
         weight = 0
         for rse in rses:
             weight += rse['weight']
             if pick <= weight:
                 return (rse['rse_id'], rse['staging_area'], rse['availability_write'])
```

### Comparing `rucio-34.1.0/lib/rucio/core/rule.py` & `rucio-34.2.0/lib/rucio/core/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/rule_grouping.py` & `rucio-34.2.0/lib/rucio/core/rule_grouping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/scope.py` & `rucio-34.2.0/lib/rucio/core/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/subscription.py` & `rucio-34.2.0/lib/rucio/core/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/topology.py` & `rucio-34.2.0/lib/rucio/core/topology.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/trace.py` & `rucio-34.2.0/lib/rucio/core/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/transfer.py` & `rucio-34.2.0/lib/rucio/core/transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/core/vo.py` & `rucio-34.2.0/lib/rucio/core/vo.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from sqlalchemy.exc import DatabaseError, IntegrityError
 from sqlalchemy.orm.exc import NoResultFound
 
 from rucio.common import exception
 from rucio.common.config import config_get, config_get_bool
 from rucio.common.types import InternalAccount
@@ -29,28 +29,28 @@
 LONG_VO_RE = re.compile(r"^[a-zA-Z0-9\.\-]+$")
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @read_session
-def vo_exists(vo, *, session: "Session"):
+def vo_exists(vo: str, *, session: "Session") -> bool:
     """
     Verify that the vo exists.
 
     :param vo: The vo to verify.
     :param session: The db session in use.
 
     :returns: True if the vo is in the vo table, False otherwise
     """
     return True if session.query(models.VO).filter_by(vo=vo).first() else False
 
 
 @transactional_session
-def add_vo(vo, description, email, *, session: "Session"):
+def add_vo(vo: str, description: str, email: str, *, session: "Session") -> None:
     """
     Add a VO and setup a new root user.
     New root user will have account name 'root' and a userpass identity with username: 'root@<vo>' and password: 'password'
 
     :param vo: 3-letter unique tag for a VO.
     :param descrition: Descriptive string for the VO (e.g. Full name).
     :param email: Contact email for the VO.
@@ -84,15 +84,15 @@
                          session=session)
 
     for ident in list_identities(account=InternalAccount('super_root', vo='def'), session=session):
         add_account_identity(identity=ident['identity'], type_=ident['type'], account=new_root, email='', session=session)
 
 
 @read_session
-def list_vos(*, session: "Session"):
+def list_vos(*, session: "Session") -> list[dict[str, Any]]:
     """
     List all the VOs in the db.
 
     :param session: The db session in use.
     :returns: List of VO dictionaries.
     """
     if not config_get_bool('common', 'multi_vo', raise_exception=False, default=False):
@@ -109,15 +109,15 @@
                    'updated_at': vo.updated_at}
         vos.append(vo_dict)
 
     return vos
 
 
 @transactional_session
-def update_vo(vo, parameters, *, session: "Session"):
+def update_vo(vo: str, parameters: dict[str, Any], *, session: "Session") -> None:
     """
     Update VO properties (email, description).
 
     :param vo: The VO to update.
     :param parameters: A dictionary with the new properties.
     :param session: The db session in use.
     """
@@ -131,15 +131,15 @@
     param = {}
     for key in parameters:
         if key in ['email', 'description']:
             param[key] = parameters[key]
     query.update(param)
 
 
-def map_vo(vo):
+def map_vo(vo: str) -> str:
     """
     Converts a long VO name into the internal short (three letter)
     tag mapping.
     Mappings are loaded from the vo-map section of the config database table.
     If a mapping is not found, the orignal is returned unchanged.
     :param vo: The long VO name string.
     :returns: The short VO name string.
```

### Comparing `rucio-34.1.0/lib/rucio/core/volatile_replica.py` & `rucio-34.2.0/lib/rucio/core/volatile_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/abacus/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/abacus/account.py` & `rucio-34.2.0/lib/rucio/daemons/abacus/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/abacus/collection_replica.py` & `rucio-34.2.0/lib/rucio/daemons/abacus/collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/abacus/rse.py` & `rucio-34.2.0/lib/rucio/daemons/abacus/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/atropos/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/atropos/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/atropos/atropos.py` & `rucio-34.2.0/lib/rucio/daemons/atropos/atropos.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         key = '{}:{}'.format(excep['scope'].internal, excep['name'])
         if key not in lifetime_exceptions:
             lifetime_exceptions[key] = excep['expires_at']
         elif lifetime_exceptions[key] < excep['expires_at']:
             lifetime_exceptions[key] = excep['expires_at']
     logger(logging.DEBUG, '%d active exceptions', len(lifetime_exceptions))
 
-    rand = random.Random(worker_number)
+    rand = random.Random(worker_number)   # noqa: S311
 
     try:
         rules = get_rules_beyond_eol(date_check, worker_number, total_workers, session=None)
         logger(logging.INFO, '%d rules to process', len(rules))
         for rule_idx, rule in enumerate(rules, start=1):
             did = '%s:%s' % (rule.scope, rule.name)
             did_key = '{}:{}'.format(rule.scope.internal, rule.name)
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/auditor/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/auditor/hdfs.py` & `rucio-34.2.0/lib/rucio/daemons/auditor/hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/auditor/srmdumps.py` & `rucio-34.2.0/lib/rucio/daemons/auditor/srmdumps.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,21 +22,25 @@
 import os
 import re
 
 import gfal2
 import requests
 
 from rucio.common.config import get_config_dirs
-from rucio.common.dumper import DUMPS_CACHE_DIR, ddmendpoint_url, gfal_download_to_file, http_download_to_file, temp_file
+from rucio.common.dumper import DUMPS_CACHE_DIR, HTTPDownloadFailed, ddmendpoint_url, gfal_download_to_file, http_download_to_file, temp_file
+from rucio.core.credential import get_signed_url
+from rucio.core.rse import get_rse_id, list_rse_attributes
 
 CHUNK_SIZE = 10485760
 
 __DUMPERCONFIGDIRS = (os.path.join(confdir, 'auditor') for confdir in get_config_dirs())
 __DUMPERCONFIGDIRS = list(filter(os.path.exists, __DUMPERCONFIGDIRS))
 
+OBJECTSTORE_NUM_TRIES = 30
+
 
 class Parser(ConfigParser.RawConfigParser):
     '''
     RawConfigParser subclass that doesn't modify the the name of the options
     and removes any quotes arround the string values.
     '''
     remove_quotes_re = re.compile(r"^'(.+)'$")
@@ -207,58 +211,92 @@
     })
 
     for conf_dir in conf_dirs:
         configuration.read(glob.glob(conf_dir + '/*.cfg'))
     return configuration
 
 
-def download_rse_dump(rse, configuration, date='latest', destdir=DUMPS_CACHE_DIR):
+def download_rse_dump(rse, configuration, date=None, destdir=DUMPS_CACHE_DIR):
     '''
     Downloads the dump for the given ddmendpoint. If this endpoint does not
     follow the standarized method to publish the dumps it should have an
     entry in the `configuration` object describing how to download the dump.
 
     `rse` is the DDMEndpoint name.
 
     `configuration` is a RawConfigParser subclass.
 
-    `date` is a datetime instance with the date of the desired dump or 'latest'
+    `date` is a datetime instance with the date of the desired dump or None
     to download the lastest available dump.
 
     `destdir` is the directory where the dump will be saved (the final component
     in the path is created if it doesn't exist).
 
     Return value: a tuple with the filename and a datetime instance with
     the date of the dump.
     '''
     logger = logging.getLogger('auditor.srmdumps')
     base_url, url_pattern = generate_url(rse, configuration)
-    if date == 'latest':
-        logger.debug('Looking for site dumps in: "%s"', base_url)
-        links = get_links(base_url)
-        url, date = get_newest(base_url, url_pattern, links)
-    else:
-        url = '{0}/{1}'.format(base_url, date.strftime(url_pattern))
 
     if not os.path.isdir(destdir):
         os.mkdir(destdir)
 
-    filename = '{0}_{1}_{2}_{3}'.format(
-        'ddmendpoint',
-        rse,
-        date.strftime('%d-%m-%Y'),
-        hashlib.sha1(url.encode()).hexdigest()
-    )
-    filename = re.sub(r'\W', '-', filename)
-    path = os.path.join(destdir, filename)
-
-    if not os.path.exists(path):
-        logger.debug('Trying to download: "%s"', url)
-        with temp_file(destdir, final_name=filename) as (f, _):
-            download(url, f)
+    # check for objectstores, which need to be handled differently
+    rse_id = get_rse_id(rse)
+    rse_attr = list_rse_attributes(rse_id)
+    if 'is_object_store' in rse_attr and rse_attr['is_object_store'] is not False:
+        tries = 1
+        if date is None:
+            # on objectstores, can't list dump files, so try the last N dates
+            date = datetime.datetime.now()
+            tries = OBJECTSTORE_NUM_TRIES
+        path = ''
+        while tries > 0:
+            url = '{0}/{1}'.format(base_url, date.strftime(url_pattern))
+
+            filename = '{0}_{1}_{2}_{3}'.format(
+                'ddmendpoint',
+                rse,
+                date.strftime('%d-%m-%Y'),
+                hashlib.sha1(url.encode()).hexdigest()
+            )
+            filename = re.sub(r'\W', '-', filename)
+            path = os.path.join(destdir, filename)
+            if not os.path.exists(path):
+                logger.debug('Trying to download: "%s"', url)
+                if 'sign_url' in rse_attr:
+                    url = get_signed_url(rse_id, rse_attr['sign_url'], 'read', url)
+                try:
+                    with temp_file(destdir, final_name=filename) as (f, _):
+                        download(url, f)
+                    tries = 0
+                except (HTTPDownloadFailed, gfal2.GError):
+                    tries -= 1
+                    date = date - datetime.timedelta(1)
+    else:
+        if date is None:
+            logger.debug('Looking for site dumps in: "%s"', base_url)
+            links = get_links(base_url)
+            url, date = get_newest(base_url, url_pattern, links)
+        else:
+            url = '{0}/{1}'.format(base_url, date.strftime(url_pattern))
+
+        filename = '{0}_{1}_{2}_{3}'.format(
+            'ddmendpoint',
+            rse,
+            date.strftime('%d-%m-%Y'),
+            hashlib.sha1(url.encode()).hexdigest()
+        )
+        filename = re.sub(r'\W', '-', filename)
+        path = os.path.join(destdir, filename)
+
+        if not os.path.exists(path):
+            logger.debug('Trying to download: "%s"', url)
+            with temp_file(destdir, final_name=filename) as (f, _):
+                download(url, f)
 
     return (path, date)
 
 
 def generate_url(rse, config):
     '''
     :param rse: Name of the endpoint.
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/automatix/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/automatix/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/automatix/automatix.py` & `rucio-34.2.0/lib/rucio/daemons/automatix/automatix.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
 import logging
 import random
+import secrets
 import tempfile
 import threading
 from configparser import NoOptionError, NoSectionError
 from datetime import datetime
 from json import load
 from os import remove, rmdir
 from typing import TYPE_CHECKING
@@ -58,15 +59,15 @@
         probabilities[key] = probability
     for key in list(probabilities):
         probabilities[key] = float(probabilities[key]) / probability
     return probabilities, data
 
 
 def choose_element(probabilities: dict, data: str) -> float:
-    rnd = random.uniform(0, 1)
+    rnd = random.uniform(0, 1)  # noqa: S311
     prob = 0
     for key in probabilities:
         prob = probabilities[key]
         if prob >= rnd:
             return data[key]
     return data[key]
 
@@ -97,19 +98,19 @@
         elif field == 'did_prefix':
             field_str = did_prefix
         elif field == "dsn":
             field_str = dsn
         elif field == "uuid":
             field_str = generate_uuid()
         elif field == "randint":
-            field_str = str(random.randint(0, 100000))
+            field_str = str(secrets.choice(range(0, 100001)))
         else:
             field_str = metadata.get(field, None)
             if not field_str:
-                field_str = str(random.randint(0, 100000))
+                field_str = str(secrets.choice(range(0, 100001)))
         file_name = "%s%s%s" % (file_name, separator, field_str)
     len_separator = len(separator)
     return file_name[len_separator:]
 
 
 def automatix(inputfile: str, sleep_time: int, once: bool = False) -> None:
     """
@@ -161,15 +162,15 @@
     )
     dataset_lifetime = config_get_int(
         "automatix", "dataset_lifetime", raise_exception=False, default=0
     )
     account = config_get("automatix", "account", raise_exception=False, default="root")
     scope = config_get("automatix", "scope", raise_exception=False, default="test")
     client = Client(account=account)
-    vo = map_vo(client.vo)
+    vo = map_vo(client.vo)  # type: ignore
     filters = {"scope": InternalScope("*", vo=vo)}
     scopes = list_scopes(filter_=filters)
     if InternalScope(scope, vo=vo) not in scopes:
         logger(logging.ERROR, "Scope %s does not exist. Exiting", scope)
         return True
 
     logger(logging.INFO, "Getting data distribution")
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/badreplicas/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/badreplicas/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/badreplicas/minos.py` & `rucio-34.2.0/lib/rucio/daemons/badreplicas/minos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py` & `rucio-34.2.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/badreplicas/necromancer.py` & `rucio-34.2.0/lib/rucio/daemons/badreplicas/necromancer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/bb8/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/bb8/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/bb8/bb8.py` & `rucio-34.2.0/lib/rucio/daemons/bb8/bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/bb8/common.py` & `rucio-34.2.0/lib/rucio/daemons/bb8/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py` & `rucio-34.2.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/bb8/t2_background_rebalance.py` & `rucio-34.2.0/lib/rucio/daemons/bb8/t2_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/simple.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/c3po.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/c3po.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/agis.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/agis.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/free_space.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/jedi_did.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/jedi_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/mock_did.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/mock_did.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Mock DID collector
 """
 
-from random import choice
+from secrets import choice
 
 
 class MockDIDCollector:
     """
     Simple collector that reads dids from a file. Used to
     test the interface.
     """
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/network_metrics.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/network_metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/collectors/workload.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/workload.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/utils/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/utils/dataset_cache.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/utils/dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/utils/expiring_list.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_list.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/utils/popularity.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/utils/popularity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/c3po/utils/timeseries.py` & `rucio-34.2.0/lib/rucio/daemons/c3po/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/cache/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/cache/consumer.py` & `rucio-34.2.0/lib/rucio/daemons/cache/consumer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/common.py` & `rucio-34.2.0/lib/rucio/daemons/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/common.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/finisher.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/finisher.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/poller.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/poller.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/preparer.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/receiver.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/receiver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/stager.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/stager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/submitter.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/conveyor/throttler.py` & `rucio-34.2.0/lib/rucio/daemons/conveyor/throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/follower/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/follower/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/follower/follower.py` & `rucio-34.2.0/lib/rucio/daemons/follower/follower.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/hermes/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/hermes/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/hermes/hermes.py` & `rucio-34.2.0/lib/rucio/daemons/hermes/hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/judge/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/judge/cleaner.py` & `rucio-34.2.0/lib/rucio/daemons/judge/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             break
         try:
             start = time.time()
             delete_rule(rule_id=rule_id, nowait=True)
             logger(logging.DEBUG, 'deletion of %s took %f' % (rule_id, time.time() - start))
         except (DatabaseException, DatabaseError, UnsupportedOperation) as e:
             if match(ORACLE_RESOURCE_BUSY_REGEX, str(e.args[0])):
-                paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(600, 2400))
+                paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(600, 2400))  # noqa: S311
                 METRICS.counter('exceptions.{exception}').labels(exception='LocksDetected').inc()
                 logger(logging.WARNING, 'Locks detected for %s' % rule_id)
             elif match('.*QueuePool.*', str(e.args[0])):
                 logger(logging.WARNING, 'DatabaseException', exc_info=True)
                 METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
             elif match(ORACLE_CONNECTION_LOST_CONTACT_REGEX, str(e.args[0])):
                 logger(logging.WARNING, 'DatabaseException', exc_info=True)
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/judge/evaluator.py` & `rucio-34.2.0/lib/rucio/daemons/judge/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             logger(logging.DEBUG, 'evaluation of %s:%s took %f', did.scope, did.name, time.time() - start_time)
             delete_updated_did(id_=did.id)
             done_dids[did_tag].append(did.rule_evaluation_action)
         except DataIdentifierNotFound:
             delete_updated_did(id_=did.id)
         except (DatabaseException, DatabaseError) as e:
             if match(ORACLE_UNIQUE_CONSTRAINT_VIOLATED_REGEX, str(e.args[0])) or match(ORACLE_RESOURCE_BUSY_REGEX, str(e.args[0])):
-                paused_dids[(did.scope.internal, did.name)] = datetime.utcnow() + timedelta(seconds=randint(60, 600))
+                paused_dids[(did.scope.internal, did.name)] = datetime.utcnow() + timedelta(seconds=randint(60, 600))  # noqa: S311
                 logger(logging.WARNING, 'Locks detected for %s:%s', did.scope, did.name)
                 METRICS.counter('exceptions.{exception}').labels(exception='LocksDetected').inc()
             elif match('.*QueuePool.*', str(e.args[0])):
                 logger(logging.WARNING, traceback.format_exc())
                 METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
             elif match(ORACLE_CONNECTION_LOST_CONTACT_REGEX, str(e.args[0])):
                 logger(logging.WARNING, traceback.format_exc())
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/judge/injector.py` & `rucio-34.2.0/lib/rucio/daemons/judge/injector.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,32 +90,32 @@
             break
         try:
             start = time.time()
             inject_rule(rule_id=rule_id, logger=logger)
             logger(logging.DEBUG, 'injection of %s took %f' % (rule_id, time.time() - start))
         except (DatabaseException, DatabaseError) as e:
             if match(ORACLE_RESOURCE_BUSY_REGEX, str(e.args[0])):
-                paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(60, 600))
+                paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(60, 600))  # noqa: S311
                 METRICS.counter('exceptions.{exception}').labels(exception='LocksDetected').inc()
                 logger(logging.WARNING, 'Locks detected for %s' % rule_id)
             elif match('.*QueuePool.*', str(e.args[0])):
                 logger(logging.WARNING, 'DatabaseException', exc_info=True)
                 METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
             elif match(ORACLE_CONNECTION_LOST_CONTACT_REGEX, str(e.args[0])):
                 logger(logging.WARNING, 'DatabaseException', exc_info=True)
                 METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
             else:
                 logger(logging.ERROR, 'DatabaseException', exc_info=True)
                 METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
         except (RSEWriteBlocked) as e:
-            paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(60, 600))
+            paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(60, 600))  # noqa: S311
             logger(logging.WARNING, 'RSEWriteBlocked for rule %s' % rule_id)
             METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
         except ReplicationRuleCreationTemporaryFailed as e:
-            paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(60, 600))
+            paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(60, 600))  # noqa: S311
             logger(logging.WARNING, 'ReplicationRuleCreationTemporaryFailed for rule %s' % rule_id)
             METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
         except RuleNotFound:
             pass
         except InsufficientAccountLimit:
             # A rule with InsufficientAccountLimit on injection hangs there potentially forever
             # It should be marked as SUSPENDED
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/judge/repairer.py` & `rucio-34.2.0/lib/rucio/daemons/judge/repairer.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             break
         try:
             start = time.time()
             repair_rule(rule_id=rule_id)
             logger(logging.DEBUG, 'repairing of %s took %f' % (rule_id, time.time() - start))
         except (DatabaseException, DatabaseError) as e:
             if match(ORACLE_RESOURCE_BUSY_REGEX, str(e.args[0])):
-                paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(600, 2400))
+                paused_rules[rule_id] = datetime.utcnow() + timedelta(seconds=randint(600, 2400))  # noqa: S311
                 logger(logging.WARNING, 'Locks detected for %s' % (rule_id))
                 METRICS.counter('exceptions.{exception}').labels(exception='LocksDetected').inc()
             elif match('.*QueuePool.*', str(e.args[0])):
                 logger(logging.WARNING, traceback.format_exc())
                 METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
             elif match(ORACLE_CONNECTION_LOST_CONTACT_REGEX, str(e.args[0])):
                 logger(logging.WARNING, traceback.format_exc())
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/oauthmanager/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/oauthmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/oauthmanager/oauthmanager.py` & `rucio-34.2.0/lib/rucio/daemons/oauthmanager/oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/reaper/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/reaper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/reaper/dark_reaper.py` & `rucio-34.2.0/lib/rucio/daemons/reaper/dark_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/reaper/reaper.py` & `rucio-34.2.0/lib/rucio/daemons/reaper/reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/replicarecoverer/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/replicarecoverer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py` & `rucio-34.2.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,22 +325,22 @@
                 replicas_nattempts_1[vo][rse_key][replica_key]["datatype"] = str(file_metadata["datatype"])
 
                 # Auditor
                 suspicious_reason = get_suspicious_reason(replicas_nattempts_1[vo][rse_key][replica_key]["rse_id"], file_scope, file_name, nattempts)
                 for reason in suspicious_reason:
                     if "auditor" in reason["reason"].lower():
                         from_auditor = True
-                        files_to_be_declared_bad_nattempts_1.append(recoverable_replicas[vo][rse_key][replica_key])
+                        files_to_be_declared_bad_nattempts_1.append(replicas_nattempts_1[vo][rse_key][replica_key])
                         break
 
                 # Bad
                 if not from_auditor:
                     if (file_name.startswith("log.")) or (file_name.startswith("user")):
                         # Don't keep log files or user files
-                        files_to_be_declared_bad_nattempts_1.append(recoverable_replicas[vo][rse_key][replica_key])
+                        files_to_be_declared_bad_nattempts_1.append(replicas_nattempts_1[vo][rse_key][replica_key])
                         action = ""
                     else:
                         # Deal with replicas based on their metadata.
                         if file_metadata["datatype"] is None:  # "None" type has no function "split()"
                             logger(logging.WARNING, "RSE: %s, replica name %s, surl %s: Replica does not have a data type associated with it. No action will be taken.",
                                    rse_key, replica_key, replicas_nattempts_1[vo][rse_key][replica_key]['surl'])
                             continue
```

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/config.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py` & `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/storage/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/storage/consistency/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/storage/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/storage/consistency/actions.py` & `rucio-34.2.0/lib/rucio/daemons/storage/consistency/actions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/tracer/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/tracer/kronos.py` & `rucio-34.2.0/lib/rucio/daemons/tracer/kronos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/transmogrifier/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/transmogrifier/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/transmogrifier/transmogrifier.py` & `rucio-34.2.0/lib/rucio/daemons/transmogrifier/transmogrifier.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/undertaker/__init__.py` & `rucio-34.2.0/lib/rucio/daemons/undertaker/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/daemons/undertaker/undertaker.py` & `rucio-34.2.0/lib/rucio/daemons/undertaker/undertaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 logger(logging.INFO, 'Delete %s dids', len(chunk))
                 METRICS.counter(name='undertaker.delete_dids').inc(len(chunk))
             except RuleNotFound as error:
                 logger(logging.ERROR, error)
             except (DatabaseException, DatabaseError, UnsupportedOperation) as e:
                 if match(ORACLE_RESOURCE_BUSY_REGEX, str(e.args[0])) or match(PSQL_LOCK_NOT_AVAILABLE_REGEX, str(e.args[0])) or match(MYSQL_LOCK_NOWAIT_REGEX, str(e.args[0])):
                     for did in chunk:
-                        paused_dids[(did['scope'], did['name'])] = datetime.utcnow() + timedelta(seconds=randint(600, 2400))
+                        paused_dids[(did['scope'], did['name'])] = datetime.utcnow() + timedelta(seconds=randint(600, 2400))  # noqa: S311
                     METRICS.counter('delete_dids.exceptions.{exception}').labels(exception='LocksDetected').inc()
                     logger(logging.WARNING, 'Locks detected for chunk')
                 else:
                     logger(logging.ERROR, 'Got database error %s.', str(e))
     except:
         logging.critical(traceback.format_exc())
```

### Comparing `rucio-34.1.0/lib/rucio/db/__init__.py` & `rucio-34.2.0/lib/rucio/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/__init__.py` & `rucio-34.2.0/lib/rucio/db/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/constants.py` & `rucio-34.2.0/lib/rucio/db/sqla/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/__init__.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/env.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/env.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py` & `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/models.py` & `rucio-34.2.0/lib/rucio/db/sqla/models.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/sautils.py` & `rucio-34.2.0/lib/rucio/db/sqla/sautils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/session.py` & `rucio-34.2.0/lib/rucio/db/sqla/session.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/types.py` & `rucio-34.2.0/lib/rucio/db/sqla/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/db/sqla/util.py` & `rucio-34.2.0/lib/rucio/db/sqla/util.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/__init__.py` & `rucio-34.2.0/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/__init__.py` & `rucio-34.2.0/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio-34.2.0/lib/rucio/rse/protocols/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/cache.py` & `rucio-34.2.0/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/dummy.py` & `rucio-34.2.0/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/gfal.py` & `rucio-34.2.0/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/globus.py` & `rucio-34.2.0/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio-34.2.0/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/http_cache.py` & `rucio-34.2.0/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/mock.py` & `rucio-34.2.0/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/ngarc.py` & `rucio-34.2.0/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/posix.py` & `rucio-34.2.0/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/protocol.py` & `rucio-34.2.0/lib/rucio/rse/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/rclone.py` & `rucio-34.2.0/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/rfio.py` & `rucio-34.2.0/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/srm.py` & `rucio-34.2.0/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/ssh.py` & `rucio-34.2.0/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/storm.py` & `rucio-34.2.0/lib/rucio/rse/protocols/storm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/webdav.py` & `rucio-34.2.0/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/protocols/xrootd.py` & `rucio-34.2.0/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/rse/rsemanager.py` & `rucio-34.2.0/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/tests/__init__.py` & `rucio-34.2.0/lib/rucio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/tests/common.py` & `rucio-34.2.0/lib/rucio/tests/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 
 import contextlib
 import itertools
 import json
 import os
 import tempfile
 from collections import namedtuple
+from functools import wraps
+from os import rename
 from random import choice, choices
 from string import ascii_letters, ascii_uppercase, digits
-from typing import Optional
+from typing import Any, Callable, Iterable, Optional
 
 import pytest
 import requests
 
 from rucio.common.config import config_get, config_get_bool, get_config_dirs
 from rucio.common.utils import execute
 from rucio.common.utils import generate_uuid as uuid
@@ -122,35 +124,35 @@
 
 
 def rse_name_generator(size: int = 10) -> str:
     """ Generate random RSE name.
 
     :returns: A random RSE name
     """
-    return 'MOCK-' + ''.join(choice(ascii_uppercase) for x in range(size))
+    return 'MOCK-' + ''.join(choice(ascii_uppercase) for x in range(size))  # noqa: S311
 
 
-def rfc2253_dn_generator():
+def rfc2253_dn_generator() -> str:
     """ Generate a random DN in RFC 2253 format.
 
     :returns: A random DN
     """
-    random_cn = ''.join(choices(ascii_letters + digits, k=8))
-    random_o = ''.join(choices(ascii_letters + digits, k=8))
-    random_c = ''.join(choices(ascii_letters, k=2))
+    random_cn = ''.join(choices(ascii_letters + digits, k=8))  # noqa: S311
+    random_o = ''.join(choices(ascii_letters + digits, k=8))  # noqa: S311
+    random_c = ''.join(choices(ascii_letters, k=2))  # noqa: S311
     random_dn = "CN={}, O={}, C={}".format(random_cn, random_o, random_c)
     return random_dn
 
 
-def file_generator(size: int = 2, namelen: int = 10):
+def file_generator(size: int = 2, namelen: int = 10) -> str:
     """ Create a bogus file and returns it's name.
     :param size: size in bytes
     :returns: The name of the generated file.
     """
-    fn = '/tmp/file_' + ''.join(choice(ascii_uppercase) for x in range(namelen))
+    fn = '/tmp/file_' + ''.join(choice(ascii_uppercase) for x in range(namelen))  # noqa: S311
     execute('dd if=/dev/urandom of={0} count={1} bs=1'.format(fn, size))
     return fn
 
 
 def make_temp_file(dir_: str, data: str) -> str:
     """
     Creates a temporal file and write `data` on it.
@@ -195,34 +197,34 @@
     if not nohdrs:
         print()
 
     text = rest_response.get_data(as_text=True)
     print(text if text else '<no content>')
 
 
-def headers(*iterables):
+def headers(*iterables: Iterable):
     return list(itertools.chain(*iterables))
 
 
-def loginhdr(account, username, password):
+def loginhdr(account: str, username: str, password: str):
     yield 'X-Rucio-Account', str(account)
     yield 'X-Rucio-Username', str(username)
     yield 'X-Rucio-Password', str(password)
 
 
 def auth(token):
     yield 'X-Rucio-Auth-Token', str(token)
 
 
-def vohdr(vo):
+def vohdr(vo: str):
     if vo:
         yield 'X-Rucio-VO', str(vo)
 
 
-def hdrdict(dictionary):
+def hdrdict(dictionary: dict):
     for key in dictionary:
         yield str(key), str(dictionary[key])
 
 
 def accept(mimetype):
     yield 'Accept', mimetype
 
@@ -231,14 +233,37 @@
     """ Enum-type class for mimetypes. """
     METALINK = 'application/metalink4+xml'
     JSON = 'application/json'
     JSON_STREAM = 'application/x-json-stream'
     BINARY = 'application/octet-stream'
 
 
-def load_test_conf_file(file_name):
+def load_test_conf_file(file_name: str) -> dict[str, Any]:
     config_dir = next(filter(lambda d: os.path.exists(os.path.join(d, file_name)), get_config_dirs()))
     with open(os.path.join(config_dir, file_name)) as f:
         return json.load(f)
 
 
+def remove_config(func: Callable) -> Callable:
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        for configfile in get_config_dirs():
+            # Rename the config to <config>.tmp
+            try:
+                rename(f"{configfile}rucio.cfg", f"{configfile}rucio.cfg.tmp")
+            except FileNotFoundError:
+                pass  # When a test uses a os.env assigned conf, there's nothing stating the default location has something
+        try:
+            # Execute the test
+            func(*args, **kwargs)
+        finally:
+            # And put the config back
+            for configfile in get_config_dirs():
+                try:
+                    rename(f"{configfile}rucio.cfg.tmp", f"{configfile}rucio.cfg")
+                except FileNotFoundError:
+                    pass
+
+    return wrapper
+
+
 RSE_namedtuple = namedtuple('RSE_namedtuple', ['name', 'id'])
```

### Comparing `rucio-34.1.0/lib/rucio/tests/common_server.py` & `rucio-34.2.0/lib/rucio/tests/common_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/__init__.py` & `rucio-34.2.0/lib/rucio/transfertool/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/bittorrent.py` & `rucio-34.2.0/lib/rucio/transfertool/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/bittorrent_driver.py` & `rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py` & `rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/fts3.py` & `rucio-34.2.0/lib/rucio/transfertool/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/fts3_plugins.py` & `rucio-34.2.0/lib/rucio/transfertool/fts3_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/globus.py` & `rucio-34.2.0/lib/rucio/transfertool/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/globus_library.py` & `rucio-34.2.0/lib/rucio/transfertool/globus_library.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/mock.py` & `rucio-34.2.0/lib/rucio/transfertool/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/transfertool/transfertool.py` & `rucio-34.2.0/lib/rucio/transfertool/transfertool.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/version.py` & `rucio-34.2.0/lib/rucio/version.py`

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

### Comparing `rucio-34.1.0/lib/rucio/web/__init__.py` & `rucio-34.2.0/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/__init__.py` & `rucio-34.2.0/lib/rucio/web/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/__init__.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/__init__.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/accounts.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accounts.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/archives.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/archives.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/auth.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/auth.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/common.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/config.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/credentials.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/credentials.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/dids.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/dirac.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/export.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/identities.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/identities.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/import.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/locks.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/main.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/metrics.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/ping.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/redirect.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/replicas.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/requests.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/rses.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/rules.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/scopes.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/scopes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/traces.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/flaskapi/v1/vos.py` & `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/vos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/main.py` & `rucio-34.2.0/lib/rucio/web/rest/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/metrics.py` & `rucio-34.2.0/lib/rucio/web/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio/web/rest/ping.py` & `rucio-34.2.0/lib/rucio/web/rest/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/lib/rucio.egg-info/SOURCES.txt` & `rucio-34.2.0/lib/rucio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/pylintrc` & `rucio-34.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/pyproject.toml` & `rucio-34.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/requirements.txt` & `rucio-34.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/setup.py` & `rucio-34.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/setuputil.py` & `rucio-34.2.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_abacus_account.py` & `rucio-34.2.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_abacus_collection_replica.py` & `rucio-34.2.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_abacus_rse.py` & `rucio-34.2.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_account.py` & `rucio-34.2.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_account_limits.py` & `rucio-34.2.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_api_external_representation.py` & `rucio-34.2.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_archive.py` & `rucio-34.2.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_auditor.py` & `rucio-34.2.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_auditor_hdfs.py` & `rucio-34.2.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_auditor_srmdumps.py` & `rucio-34.2.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_authentication.py` & `rucio-34.2.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_automatix.py` & `rucio-34.2.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_bad_replica.py` & `rucio-34.2.0/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_bb8.py` & `rucio-34.2.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_belleii.py` & `rucio-34.2.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_bin_rucio.py` & `rucio-34.2.0/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_boolean.py` & `rucio-34.2.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_common_types.py` & `rucio-34.2.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_config.py` & `rucio-34.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_conveyor.py` & `rucio-34.2.0/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_conveyor_submitter.py` & `rucio-34.2.0/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_counter.py` & `rucio-34.2.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_credential.py` & `rucio-34.2.0/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_curl.py` & `rucio-34.2.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_daemons.py` & `rucio-34.2.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_dataset_replicas.py` & `rucio-34.2.0/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_db.py` & `rucio-34.2.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_did.py` & `rucio-34.2.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_did_meta_plugins.py` & `rucio-34.2.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_didtype.py` & `rucio-34.2.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_download.py` & `rucio-34.2.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_dumper.py` & `rucio-34.2.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_dumper_consistency.py` & `rucio-34.2.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_dumper_data_model.py` & `rucio-34.2.0/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_dumper_path_parsing.py` & `rucio-34.2.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_filter_engine.py` & `rucio-34.2.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_heartbeat.py` & `rucio-34.2.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_hermes.py` & `rucio-34.2.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_identity.py` & `rucio-34.2.0/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_impl_upload_download.py` & `rucio-34.2.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_import_export.py` & `rucio-34.2.0/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_judge_cleaner.py` & `rucio-34.2.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_judge_evaluator.py` & `rucio-34.2.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_judge_injector.py` & `rucio-34.2.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_judge_repairer.py` & `rucio-34.2.0/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_lifetime.py` & `rucio-34.2.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_message.py` & `rucio-34.2.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_meta_conventions.py` & `rucio-34.2.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_meta_did.py` & `rucio-34.2.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_module_import.py` & `rucio-34.2.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_monitor.py` & `rucio-34.2.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_multi_vo.py` & `rucio-34.2.0/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_naming_convention.py` & `rucio-34.2.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_oauthmanager.py` & `rucio-34.2.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_oidc.py` & `rucio-34.2.0/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_permission.py` & `rucio-34.2.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_pfns.py` & `rucio-34.2.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_ping.py` & `rucio-34.2.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_preparer.py` & `rucio-34.2.0/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_qos.py` & `rucio-34.2.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_quarantined_replica.py` & `rucio-34.2.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_reaper.py` & `rucio-34.2.0/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_redirect.py` & `rucio-34.2.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_replica.py` & `rucio-34.2.0/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_replica_recoverer.py` & `rucio-34.2.0/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_replica_sorting.py` & `rucio-34.2.0/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_request.py` & `rucio-34.2.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_root_proxy.py` & `rucio-34.2.0/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse.py` & `rucio-34.2.0/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_expression_parser.py` & `rucio-34.2.0/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_lfn2path.py` & `rucio-34.2.0/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_gfal2.py` & `rucio-34.2.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio-34.2.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_posix.py` & `rucio-34.2.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_rclone.py` & `rucio-34.2.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_rsync.py` & `rucio-34.2.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_srm.py` & `rucio-34.2.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_ssh.py` & `rucio-34.2.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_webdav.py` & `rucio-34.2.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_protocol_xrootd.py` & `rucio-34.2.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rse_selector.py` & `rucio-34.2.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rucio_server.py` & `rucio-34.2.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_rule.py` & `rucio-34.2.0/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_schema_cms.py` & `rucio-34.2.0/tests/test_schema_cms.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_scope.py` & `rucio-34.2.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_subscription.py` & `rucio-34.2.0/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_throttler.py` & `rucio-34.2.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_tpc.py` & `rucio-34.2.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_trace.py` & `rucio-34.2.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_transfer.py` & `rucio-34.2.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_transfer_plugins.py` & `rucio-34.2.0/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_undertaker.py` & `rucio-34.2.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_upload.py` & `rucio-34.2.0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tests/test_utils.py` & `rucio-34.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tools/bootstrap.py` & `rucio-34.2.0/tools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tools/merge_rucio_configs.py` & `rucio-34.2.0/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.1.0/tools/reset_database.py` & `rucio-34.2.0/tools/reset_database.py`

 * *Files identical despite different names*

