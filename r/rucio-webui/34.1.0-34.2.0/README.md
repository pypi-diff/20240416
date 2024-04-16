# Comparing `tmp/rucio-webui-34.1.0.tar.gz` & `tmp/rucio_webui-34.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-webui-34.1.0.tar", last modified: Tue Apr  2 13:57:13 2024, max compression
+gzip compressed data, was "rucio_webui-34.2.0.tar", last modified: Tue Apr 16 10:35:12 2024, max compression
```

## Comparing `rucio-webui-34.1.0.tar` & `rucio_webui-34.2.0.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio-webui-34.1.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2024-04-02 13:57:10.000000 rucio-webui-34.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      866 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-04-02 11:45:19.000000 rucio-webui-34.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.710326 rucio-webui-34.1.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.713326 rucio-webui-34.1.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/alembicrevision.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-02 11:50:17.000000 rucio-webui-34.1.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1549 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.713326 rucio-webui-34.1.0/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.713326 rucio-webui-34.1.0/lib/rucio/web/ui/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.714326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.714326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/
--rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.715326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.715326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/certs/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/certs/README
--rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/settings.json
--rw-r--r--   0 root         (0) root         (0)    27943 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/utils.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.722326 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account.html
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage.html
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage_history.html
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounting.html
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounts.html
--rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/add_rse.html
--rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/approve_rules.html
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/atlas_index.html
--rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/backlog_mon.html
--rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas.html
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
--rw-r--r--   0 root         (0) root         (0)     8979 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/cond.html
--rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dbrelease.html
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/did.html
--rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dumps.html
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/heartbeats.html
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/infrastructure.html
--rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html
--rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
--rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_rules.html
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/login.html
--rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/no_certificate.html
--rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/problem.html
--rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/request_rule.html
--rw-r--r--   0 root         (0) root         (0)     4124 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse.html
--rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html
--rw-r--r--   0 root         (0) root         (0)     7277 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_locks.html
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rses.html
--rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rule.html
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rules.html
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/select_login_method.html
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscription.html
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html
--rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions.html
--rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
--rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
--rw-r--r--   0 root         (0) root         (0)      717 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/lib/rucio/web/ui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.724326 rucio-webui-34.1.0/lib/rucio/web/ui/media/
--rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/RucioUI.png
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/details_close.png
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/details_open.png
--rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/error.jpg
--rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.725326 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/
--rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.eot
--rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.svg
--rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.ttf
--rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.woff
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/get_info.png
--rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/logo.png
--rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/rucio_logo.png
--rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/media/spinner.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.738326 rucio-webui-34.1.0/lib/rucio/web/ui/static/
--rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account.js
--rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account_rse_usage.js
--rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage_history.js
--rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/accounting.js
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/accounts.js
--rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/add_rse.js
--rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/approve_rules.js
--rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/atlas_index.js
--rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/backlog_mon.js
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas.js
--rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas_summary.js
--rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/base.js
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.css
--rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.js
--rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.js
--rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.min.js
--rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/cond.js
--rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/dbrelease.js
--rw-r--r--   0 root         (0) root         (0)    43648 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/did.js
--rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/filesize.min.js
--rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.css
--rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.eot
--rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.svg
--rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/heartbeats.js
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring.css
--rw-r--r--   0 root         (0) root         (0)    12386 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_account_details.js
--rw-r--r--   0 root         (0) root         (0)     3525 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_accounts.js
--rw-r--r--   0 root         (0) root         (0)     5294 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
--rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
--rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_index.js
--rw-r--r--   0 root         (0) root         (0)     3043 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_resources.js
--rw-r--r--   0 root         (0) root         (0)     8872 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
--rw-r--r--   0 root         (0) root         (0)     3055 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js
--rw-r--r--   0 root         (0) root         (0)    10028 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_utils.js
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/index.js
--rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select.js
--rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select2.js
--rw-r--r--   0 root         (0) root         (0)     4151 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.quicksearch.js
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.storageapi.min.js
--rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/lifetime_exception.js
--rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js
--rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/list_rules.js
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/login.js
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.css
--rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.png
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select2.css
--rw-r--r--   0 root         (0) root         (0)    54419 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/request_rule.js
--rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse.js
--rw-r--r--   0 root         (0) root         (0)    23373 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_add_protocol.js
--rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_locks.js
--rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_usage.js
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rses.js
--rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.css
--rw-r--r--   0 root         (0) root         (0)    63519 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.js
--rw-r--r--   0 root         (0) root         (0)    23335 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rule.js
--rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/rules.js
--rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/search.js
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/select_login_method.css
--rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscription.js
--rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptionrules.js
--rw-r--r--   0 root         (0) root         (0)     4946 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions.js
--rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions_editor.js
--rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/suspicious_replicas.js
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/switch.png
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/version.js
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-02 11:50:17.000000 rucio-webui-34.1.0/lib/rucio/web/ui/static/webui_version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/lib/rucio_webui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8846 2024-04-02 13:57:13.000000 rucio-webui-34.1.0/lib/rucio_webui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-webui-34.1.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-03-19 15:04:29.000000 rucio-webui-34.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-02 13:57:13.758327 rucio-webui-34.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2128 2024-04-02 13:57:10.000000 rucio-webui-34.1.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 13:57:13.756327 rucio-webui-34.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     6929 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio-webui-34.1.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio-webui-34.1.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio-webui-34.1.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.380100 rucio_webui-34.2.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio_webui-34.2.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-16 10:35:08.000000 rucio_webui-34.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      866 2024-04-16 10:35:12.380100 rucio_webui-34.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-16 07:53:27.000000 rucio_webui-34.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.335100 rucio_webui-34.2.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.337100 rucio_webui-34.2.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/alembicrevision.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-16 07:53:37.000000 rucio_webui-34.2.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-08 15:22:52.000000 rucio_webui-34.2.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.337100 rucio_webui-34.2.0/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.338100 rucio_webui-34.2.0/lib/rucio/web/ui/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.338100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.338100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.339100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.339100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/certs/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/certs/README
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/settings.json
+-rw-r--r--   0 root         (0) root         (0)    27943 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/utils.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.346100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account.html
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage_history.html
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounting.html
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounts.html
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/add_rse.html
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/approve_rules.html
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/atlas_index.html
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/backlog_mon.html
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas.html
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
+-rw-r--r--   0 root         (0) root         (0)     8979 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/cond.html
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dbrelease.html
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/did.html
+-rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dumps.html
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/heartbeats.html
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/infrastructure.html
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
+-rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_rules.html
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/login.html
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/no_certificate.html
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/problem.html
+-rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/request_rule.html
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse.html
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     7277 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_locks.html
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rses.html
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rule.html
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rules.html
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/select_login_method.html
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscription.html
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions.html
+-rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
+-rw-r--r--   0 root         (0) root         (0)      717 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.348100 rucio_webui-34.2.0/lib/rucio/web/ui/media/
+-rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/RucioUI.png
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/details_close.png
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/details_open.png
+-rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/error.jpg
+-rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.349100 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/
+-rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.eot
+-rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.svg
+-rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.ttf
+-rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.woff
+-rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/get_info.png
+-rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/logo.png
+-rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/rucio_logo.png
+-rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/spinner.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.362100 rucio_webui-34.2.0/lib/rucio/web/ui/static/
+-rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account.js
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account_rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage_history.js
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/accounting.js
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/accounts.js
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/add_rse.js
+-rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/approve_rules.js
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/atlas_index.js
+-rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/backlog_mon.js
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas.js
+-rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas_summary.js
+-rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/base.js
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.css
+-rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.js
+-rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.js
+-rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.min.js
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/cond.js
+-rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/dbrelease.js
+-rw-r--r--   0 root         (0) root         (0)    43648 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/did.js
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/filesize.min.js
+-rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.css
+-rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/heartbeats.js
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring.css
+-rw-r--r--   0 root         (0) root         (0)    12386 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_account_details.js
+-rw-r--r--   0 root         (0) root         (0)     3525 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_accounts.js
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_index.js
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_resources.js
+-rw-r--r--   0 root         (0) root         (0)     8872 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js
+-rw-r--r--   0 root         (0) root         (0)    10028 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_utils.js
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/index.js
+-rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select.js
+-rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select2.js
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.quicksearch.js
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.storageapi.min.js
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/lifetime_exception.js
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/list_rules.js
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/login.js
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.css
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.png
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select2.css
+-rw-r--r--   0 root         (0) root         (0)    54419 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/request_rule.js
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse.js
+-rw-r--r--   0 root         (0) root         (0)    23373 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_add_protocol.js
+-rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_locks.js
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rses.js
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.css
+-rw-r--r--   0 root         (0) root         (0)    63519 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.js
+-rw-r--r--   0 root         (0) root         (0)    23335 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rule.js
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rules.js
+-rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/search.js
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/select_login_method.css
+-rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscription.js
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptionrules.js
+-rw-r--r--   0 root         (0) root         (0)     4946 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions.js
+-rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions_editor.js
+-rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/suspicious_replicas.js
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/switch.png
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/version.js
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 07:53:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/webui_version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.379100 rucio_webui-34.2.0/lib/rucio_webui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8846 2024-04-16 10:35:12.000000 rucio_webui-34.2.0/lib/rucio_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-04-16 07:53:27.000000 rucio_webui-34.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-16 10:35:12.381100 rucio_webui-34.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2128 2024-04-16 10:35:08.000000 rucio_webui-34.2.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.379100 rucio_webui-34.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-04-08 15:14:19.000000 rucio_webui-34.2.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_utils.py
```

### Comparing `rucio-webui-34.1.0/AUTHORS.rst` & `rucio_webui-34.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/LICENSE` & `rucio_webui-34.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/PKG-INFO` & `rucio_webui-34.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-webui
-Version: 34.1.0
+Version: 34.2.0
 Summary: Rucio WebUI Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-webui-34.1.0/README.rst` & `rucio_webui-34.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/__init__.py` & `rucio_webui-34.2.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/alembicrevision.py` & `rucio_webui-34.2.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/version.py` & `rucio_webui-34.2.0/lib/rucio/version.py`

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

### Comparing `rucio-webui-34.1.0/lib/rucio/web/__init__.py` & `rucio_webui-34.2.0/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/__init__.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/__init__.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/bp.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/bp.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/__init__.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/saml/settings.json` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/settings.json`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/common/utils.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/main.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/main.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/account_usage_history.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage_history.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounting.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounting.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/accounts.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounts.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/add_rse.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/add_rse.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/approve_rules.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/approve_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/atlas_index.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/atlas_index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/backlog_mon.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/backlog_mon.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/base.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/base.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/cond.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/cond.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dbrelease.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dbrelease.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/did.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/did.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/dumps.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dumps.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/heartbeats.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/heartbeats.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/index.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/infrastructure.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/infrastructure.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/list_rules.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/login.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/no_certificate.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/no_certificate.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/problem.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/problem.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/request_rule.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/request_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_locks.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_locks.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rse_usage.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rses.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rses.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rule.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/rules.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/search.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/search.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/select_login_method.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/select_login_method.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscription.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html` & `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/main.py` & `rucio_webui-34.2.0/lib/rucio/web/ui/main.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/RucioUI.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/RucioUI.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/details_close.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/details_close.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/details_open.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/details_open.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/error.jpg` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/error.jpg`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/favicon.ico` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.eot` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.svg` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.ttf` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/fonts/login_icons.woff` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/get_info.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/get_info.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/logo.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/rucio_logo.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/media/spinner.gif` & `rucio_webui-34.2.0/lib/rucio/web/ui/media/spinner.gif`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/account.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/account.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/account_rse_usage.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/account_rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/account_usage_history.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage_history.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/accounting.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/accounting.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/accounts.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/add_rse.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/add_rse.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/approve_rules.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/approve_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/atlas_index.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/atlas_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/backlog_mon.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/backlog_mon.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/bad_replicas_summary.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas_summary.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/base.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/base.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen-sprite@2x.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.jquery.min.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.min.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.min.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/chosen.proto.min.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/cond.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/cond.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/dbrelease.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/dbrelease.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/did.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/did.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/filesize.min.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/filesize.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.eot` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.svg` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.ttf` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/foundation-icons.woff` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/heartbeats.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/heartbeats.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_account_details.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_account_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_accounts.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_index.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_resources.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_resources.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/http_monitoring_utils.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_utils.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.multiple.select2.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select2.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.quicksearch.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.quicksearch.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/jquery.storageapi.min.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.storageapi.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/lifetime_exception.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/lifetime_exception.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/list_rules.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/list_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/multiple-select2.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select2.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/request_rule.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/request_rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_account_usage.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_add_protocol.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_add_protocol.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_locks.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_locks.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rse_usage.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rses.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rucio.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rule.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/rules.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/search.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/search.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/select_login_method.css` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/select_login_method.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscription.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscription.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptionrules.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptionrules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/subscriptions_editor.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions_editor.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/suspicious_replicas.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/suspicious_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/switch.png` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/switch.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio/web/ui/static/version.js` & `rucio_webui-34.2.0/lib/rucio/web/ui/static/version.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/lib/rucio_webui.egg-info/SOURCES.txt` & `rucio_webui-34.2.0/lib/rucio_webui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/pylintrc` & `rucio_webui-34.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/pyproject.toml` & `rucio_webui-34.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/requirements.txt` & `rucio_webui-34.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/setup.py` & `rucio_webui-34.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/setuputil.py` & `rucio_webui-34.2.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_abacus_account.py` & `rucio_webui-34.2.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_abacus_collection_replica.py` & `rucio_webui-34.2.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_abacus_rse.py` & `rucio_webui-34.2.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_account.py` & `rucio_webui-34.2.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_account_limits.py` & `rucio_webui-34.2.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_api_external_representation.py` & `rucio_webui-34.2.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_archive.py` & `rucio_webui-34.2.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_auditor.py` & `rucio_webui-34.2.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_auditor_hdfs.py` & `rucio_webui-34.2.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_auditor_srmdumps.py` & `rucio_webui-34.2.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_authentication.py` & `rucio_webui-34.2.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_automatix.py` & `rucio_webui-34.2.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_bad_replica.py` & `rucio_webui-34.2.0/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_bb8.py` & `rucio_webui-34.2.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_belleii.py` & `rucio_webui-34.2.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_bin_rucio.py` & `rucio_webui-34.2.0/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_boolean.py` & `rucio_webui-34.2.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_common_types.py` & `rucio_webui-34.2.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_config.py` & `rucio_webui-34.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_conveyor.py` & `rucio_webui-34.2.0/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_conveyor_submitter.py` & `rucio_webui-34.2.0/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_counter.py` & `rucio_webui-34.2.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_credential.py` & `rucio_webui-34.2.0/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_curl.py` & `rucio_webui-34.2.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_daemons.py` & `rucio_webui-34.2.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_dataset_replicas.py` & `rucio_webui-34.2.0/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_db.py` & `rucio_webui-34.2.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_did.py` & `rucio_webui-34.2.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_did_meta_plugins.py` & `rucio_webui-34.2.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_didtype.py` & `rucio_webui-34.2.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_download.py` & `rucio_webui-34.2.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_dumper.py` & `rucio_webui-34.2.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_dumper_consistency.py` & `rucio_webui-34.2.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_dumper_data_model.py` & `rucio_webui-34.2.0/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_dumper_path_parsing.py` & `rucio_webui-34.2.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_filter_engine.py` & `rucio_webui-34.2.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_heartbeat.py` & `rucio_webui-34.2.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_hermes.py` & `rucio_webui-34.2.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_identity.py` & `rucio_webui-34.2.0/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_impl_upload_download.py` & `rucio_webui-34.2.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_import_export.py` & `rucio_webui-34.2.0/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_judge_cleaner.py` & `rucio_webui-34.2.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_judge_evaluator.py` & `rucio_webui-34.2.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_judge_injector.py` & `rucio_webui-34.2.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_judge_repairer.py` & `rucio_webui-34.2.0/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_lifetime.py` & `rucio_webui-34.2.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_message.py` & `rucio_webui-34.2.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_meta_conventions.py` & `rucio_webui-34.2.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_meta_did.py` & `rucio_webui-34.2.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_module_import.py` & `rucio_webui-34.2.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_monitor.py` & `rucio_webui-34.2.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_multi_vo.py` & `rucio_webui-34.2.0/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_naming_convention.py` & `rucio_webui-34.2.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_oauthmanager.py` & `rucio_webui-34.2.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_oidc.py` & `rucio_webui-34.2.0/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_permission.py` & `rucio_webui-34.2.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_pfns.py` & `rucio_webui-34.2.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_ping.py` & `rucio_webui-34.2.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_preparer.py` & `rucio_webui-34.2.0/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_qos.py` & `rucio_webui-34.2.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_quarantined_replica.py` & `rucio_webui-34.2.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_reaper.py` & `rucio_webui-34.2.0/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_redirect.py` & `rucio_webui-34.2.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_replica.py` & `rucio_webui-34.2.0/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_replica_recoverer.py` & `rucio_webui-34.2.0/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_replica_sorting.py` & `rucio_webui-34.2.0/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_request.py` & `rucio_webui-34.2.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_root_proxy.py` & `rucio_webui-34.2.0/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse.py` & `rucio_webui-34.2.0/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_expression_parser.py` & `rucio_webui-34.2.0/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_lfn2path.py` & `rucio_webui-34.2.0/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_gfal2.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_posix.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_rclone.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_rsync.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_srm.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_ssh.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_webdav.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_protocol_xrootd.py` & `rucio_webui-34.2.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rse_selector.py` & `rucio_webui-34.2.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rucio_server.py` & `rucio_webui-34.2.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_rule.py` & `rucio_webui-34.2.0/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_schema_cms.py` & `rucio_webui-34.2.0/tests/test_schema_cms.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_scope.py` & `rucio_webui-34.2.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_subscription.py` & `rucio_webui-34.2.0/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_throttler.py` & `rucio_webui-34.2.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_tpc.py` & `rucio_webui-34.2.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_trace.py` & `rucio_webui-34.2.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_transfer.py` & `rucio_webui-34.2.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_transfer_plugins.py` & `rucio_webui-34.2.0/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_undertaker.py` & `rucio_webui-34.2.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_upload.py` & `rucio_webui-34.2.0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-34.1.0/tests/test_utils.py` & `rucio_webui-34.2.0/tests/test_utils.py`

 * *Files identical despite different names*

