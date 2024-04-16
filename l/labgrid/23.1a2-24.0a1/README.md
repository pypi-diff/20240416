# Comparing `tmp/labgrid-23.1a2.tar.gz` & `tmp/labgrid-24.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgrid-23.1a2.tar", last modified: Fri Apr 28 13:11:52 2023, max compression
+gzip compressed data, was "labgrid-24.0a1.tar", last modified: Tue Apr  9 13:52:30 2024, max compression
```

## Comparing `labgrid-23.1a2.tar` & `labgrid-24.0a1.tar`

### file list

```diff
@@ -1,428 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.777660 labgrid-23.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 13:11:41.000000 labgrid-23.1a2/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 13:11:41.000000 labgrid-23.1a2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.737660 labgrid-23.1a2/.crossbar/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 13:11:41.000000 labgrid-23.1a2/.crossbar/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 13:11:41.000000 labgrid-23.1a2/.crossbar/config-anonymous.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 13:11:41.000000 labgrid-23.1a2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 13:11:41.000000 labgrid-23.1a2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.737660 labgrid-23.1a2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/build-and-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/push-pr-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/reusable-unit-tests-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/reusable-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/scheduled-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-28 13:11:41.000000 labgrid-23.1a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 13:11:41.000000 labgrid-23.1a2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    28027 2023-04-28 13:11:41.000000 labgrid-23.1a2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 13:11:41.000000 labgrid-23.1a2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-04-28 13:11:41.000000 labgrid-23.1a2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 13:11:41.000000 labgrid-23.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-28 13:11:52.777660 labgrid-23.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-28 13:11:41.000000 labgrid-23.1a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/completion/
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/completion/labgrid-client.bash
--rwxr-xr-x   0 runner    (1001) docker     (123)     6195 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/coordinator-statsd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/sync-places.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/labgrid-coordinator.service
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/labgrid-exporter.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/systemd/sysusers.d/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/sysusers.d/labgrid.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/systemd/tmpfiles.d/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/tmpfiles.d/labgrid.conf
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 13:11:41.000000 labgrid-23.1a2/crossbar-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-client
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-exporter
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-pytest
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-suggest
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.install
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.manpages
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.tmpfile
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.triggers
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    88586 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/design_decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/images/labgrid_logo_outline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/doc/man/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man/device-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man/exporter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/doc/res/
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/res/config_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/res/graphstrategy-via-nand.png
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/res/graphstrategy-via-nfs.png
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/exporter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/exporter/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.733660 labgrid-23.1a2/dockerfiles/staging/client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/client/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/client/.ssh/id_rsa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/client/simple-test/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/client/simple-test/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/client/simple-test/remote_shell_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/crossbar/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/crossbar/places_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/dut/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/dut/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/dut/authorized_keys
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/exporter-conf/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/exporter-conf/exporter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/examples/barebox/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/local-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_barebox.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_bootchooser.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/examples/deditec-relais8/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/deditec.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/deditec_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/export-didicontrol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/import-dedicontrol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/library/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/library/phytec.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/library/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/modbusrtu/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/modbusrtu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/modbusrtu/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/modbusrtu/test_modbusrtu_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/networkmanager/nm.env
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/networkmanager/nm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/power/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/power/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/power/power_example.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/pyvisa/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/pyvisa/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/pyvisa/pyvisa_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/qemu-networking/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/qemunetworkstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/test_qemu_networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/remote/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/remote/test_barebox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_hwclock.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_rt.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/bareboxrebootstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/quartusstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/test_barebox_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/test_uboot_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/sysfsgpio/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/export-gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/import-gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/sysfsgpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/sysfsgpio_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/mass-storage-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/mxs-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/test_usb_mxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/test_usb_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/examples/usbpower/
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/examplestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/exports.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/examples/usbsdmux/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbsdmux/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbsdmux/test_sdmux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-04-28 13:11:41.000000 labgrid-23.1a2/helpers/labgrid-bound-connect
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/labgrid/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/labgrid/autoinstall/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/autoinstall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/autoinstall/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/consoleloggingreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.757660 labgrid-23.1a2/labgrid/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/bareboxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/commandmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/consoleexpectmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/dediprogflashdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/deditecrelaisdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/dfudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/dockerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/externalconsoledriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/fastbootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/filedigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/flashromdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/flashscriptdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/gpiodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/httpvideodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/lxaiobusdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/lxausbmuxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/manualswitchdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/modbusdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/modbusrtudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/networkinterfacedriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/onewiredriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/openocddriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/driver/power/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/apc.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/digipower.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/digitalloggers_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/eaton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/eg_pms2_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude24.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude8031.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude8225.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude8316.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/netio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/netio_kshell.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/shelly_gen1.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/siglent.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/simplerest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/tplink.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/powerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/pyvisadriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/qemudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/quartushpsdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/resetdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/serialdigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/serialdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/shelldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/sigrokdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/smallubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/sshdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/ubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbaudiodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbhidrelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbsdmuxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbsdwiredriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbstoragedriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/driver/usbtmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmc/keysight_dsox2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmc/tektronix_tds2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmcdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbvideodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/xenadriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/bootstrapprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/commandprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/consoleprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/digitaloutputprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/filesystemprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/filetransferprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/infoprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/linuxbootprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/mmioprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/powerprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/resetprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/videoprotocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/pytestplugin/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/pytestplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/pytestplugin/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/pytestplugin/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.765660 labgrid-23.1a2/labgrid/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/authenticator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81571 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32314 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.765660 labgrid-23.1a2/labgrid/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/dediprogflasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/ethernetport.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/fastboot.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/flashrom.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/httpvideostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/lxaiobus.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/modbusrtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/networkservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/onewireport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/pyvisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/serialport.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/sigrok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/udev.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/xenamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/ykushpowerport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/stepreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.765660 labgrid-23.1a2/labgrid/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/bareboxstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/dockerstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/graphstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/shellstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/ubootstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.769660 labgrid-23.1a2/labgrid/util/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.769660 labgrid-23.1a2/labgrid/util/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/deditec_relais8.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/sysfsgpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/usb_hid_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agentwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/expect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/managedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/qmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/labgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.769660 labgrid-23.1a2/man/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-client.1
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-device-config.5
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-device-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-exporter.1
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-exporter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-pytest.7
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-pytest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-suggest.1
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-suggest.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 13:11:41.000000 labgrid-23.1a2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-28 13:11:41.000000 labgrid-23.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:11:52.777660 labgrid-23.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.777660 labgrid-23.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_autoinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_bareboxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_crossbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_dediprogflasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_ethernetport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_externalconsoledriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_filedigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_flashrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_flashscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_graphstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_httpvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_lxaiobus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_manualswitchdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_modbusrtudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_onewire.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_openocd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_powerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_processwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_pyvisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_qemudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sched.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_serialdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_serialport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_shelldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sigrok.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sispm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sshdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_steplogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sysfsgpioagent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_tasmota.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_ubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_usbtmc.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_usbvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.227910 labgrid-24.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:52:25.000000 labgrid-24.0a1/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 13:52:25.000000 labgrid-24.0a1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.159909 labgrid-24.0a1/.crossbar/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 13:52:25.000000 labgrid-24.0a1/.crossbar/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-09 13:52:25.000000 labgrid-24.0a1/.crossbar/config-anonymous.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 13:52:25.000000 labgrid-24.0a1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 13:52:25.000000 labgrid-24.0a1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.159909 labgrid-24.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.159909 labgrid-24.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/workflows/build-and-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/workflows/push-pr-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/workflows/reusable-unit-tests-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/workflows/reusable-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 13:52:25.000000 labgrid-24.0a1/.github/workflows/scheduled-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 13:52:25.000000 labgrid-24.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 13:52:25.000000 labgrid-24.0a1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-04-09 13:52:25.000000 labgrid-24.0a1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 13:52:25.000000 labgrid-24.0a1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    26530 2024-04-09 13:52:25.000000 labgrid-24.0a1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 13:52:25.000000 labgrid-24.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-09 13:52:30.227910 labgrid-24.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-09 13:52:25.000000 labgrid-24.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.163909 labgrid-24.0a1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.163909 labgrid-24.0a1/contrib/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/completion/labgrid-client.bash
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6375 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/coordinator-statsd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5124 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/labgrid-webapp
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/requirements-webapp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7950 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/sync-places.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.163909 labgrid-24.0a1/contrib/systemd/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/systemd/labgrid-coordinator.service
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/systemd/labgrid-exporter.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.163909 labgrid-24.0a1/contrib/systemd/sysusers.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/systemd/sysusers.d/labgrid.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.163909 labgrid-24.0a1/contrib/systemd/tmpfiles.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 13:52:25.000000 labgrid-24.0a1/contrib/systemd/tmpfiles.d/labgrid.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-09 13:52:25.000000 labgrid-24.0a1/crossbar-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.163909 labgrid-24.0a1/debian/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/control
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (127)      165 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid-client
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid-exporter
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid-pytest
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid-suggest
+-rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid.install
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid.manpages
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid.tmpfile
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid.triggers
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/labgrid.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      285 2024-04-09 13:52:25.000000 labgrid-24.0a1/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.167909 labgrid-24.0a1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99735 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/design_decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24658 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.167909 labgrid-24.0a1/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/images/labgrid_logo_outline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.167909 labgrid-24.0a1/doc/man/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/man/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/man/device-config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/man/exporter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/man.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17236 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.167909 labgrid-24.0a1/doc/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/res/config_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25639 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/res/graphstrategy-via-nand.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25480 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/res/graphstrategy-via-nfs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-04-09 13:52:25.000000 labgrid-24.0a1/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2086 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/exporter/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      145 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/exporter/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/staging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.151909 labgrid-24.0a1/dockerfiles/staging/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/staging/client/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/client/.ssh/id_rsa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/staging/client/simple-test/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/client/simple-test/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/client/simple-test/remote_shell_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/staging/crossbar/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/crossbar/places_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/staging/dut/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/dut/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/dut/authorized_keys
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/dockerfiles/staging/exporter-conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 13:52:25.000000 labgrid-24.0a1/dockerfiles/staging/exporter-conf/exporter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.171909 labgrid-24.0a1/examples/barebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/local-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/test_barebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/test_bootchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/test_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/barebox/test_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/deditec-relais8/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/deditec-relais8/deditec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/deditec-relais8/deditec_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/deditec-relais8/export-didicontrol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/deditec-relais8/import-dedicontrol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/docker/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/docker/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/docker/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/library/phytec.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/library/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/modbusrtu/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/modbusrtu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/modbusrtu/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/modbusrtu/test_modbusrtu_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/network-test/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/network-test/env.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1771 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/network-test/pkg-replay-record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/networkmanager/nm.env
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/networkmanager/nm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/power/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/power/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/power/power_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/pyvisa/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/pyvisa/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/pyvisa/pyvisa_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.175909 labgrid-24.0a1/examples/qemu-networking/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/qemu-networking/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/qemu-networking/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/qemu-networking/qemunetworkstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/qemu-networking/test_qemu_networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.179909 labgrid-24.0a1/examples/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/remote/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/remote/test_barebox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.179909 labgrid-24.0a1/examples/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/shell/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/shell/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/shell/test_hwclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/shell/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/shell/test_rt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/shell/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.179909 labgrid-24.0a1/examples/sigrok/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/sigrok/env.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/sigrok/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.179909 labgrid-24.0a1/examples/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/strategy/bareboxrebootstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/strategy/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/strategy/quartusstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/strategy/test_barebox_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/strategy/test_uboot_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.179909 labgrid-24.0a1/examples/sysfsgpio/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/sysfsgpio/export-gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/sysfsgpio/import-gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/sysfsgpio/sysfsgpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/sysfsgpio/sysfsgpio_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.179909 labgrid-24.0a1/examples/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usb/mass-storage-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usb/mxs-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usb/test_usb_mxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usb/test_usb_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.183910 labgrid-24.0a1/examples/usbpower/
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/examplestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/exports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbpower/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.183910 labgrid-24.0a1/examples/usbsdmux/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbsdmux/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:52:25.000000 labgrid-24.0a1/examples/usbsdmux/test_sdmux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.183910 labgrid-24.0a1/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2277 2024-04-09 13:52:25.000000 labgrid-24.0a1/helpers/labgrid-bound-connect
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3032 2024-04-09 13:52:25.000000 labgrid-24.0a1/helpers/labgrid-raw-interface
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.183910 labgrid-24.0a1/labgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.187909 labgrid-24.0a1/labgrid/autoinstall/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/autoinstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/autoinstall/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/consoleloggingreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.195910 labgrid-24.0a1/labgrid/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/bareboxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/commandmixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/consoleexpectmixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/dediprogflashdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/deditecrelaisdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/dfudriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/dockerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/externalconsoledriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/fastbootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/filedigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/flashromdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/flashscriptdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/gpiodriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/httpdigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/httpvideodriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/lxaiobusdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/lxausbmuxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/manualswitchdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/modbusdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/modbusrtudriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/networkinterfacedriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/onewiredriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/openocddriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.199910 labgrid-24.0a1/labgrid/driver/power/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/apc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/digipower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/digitalloggers_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/eaton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/eg_pms2_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/eth008.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/gude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/gude24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/gude8031.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/gude8225.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/gude8316.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/netio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/netio_kshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/poe_mib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/raritan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/shelly_gen1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/siglent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/simplerest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/power/tplink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/powerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/pyvisadriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13418 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/qemudriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/quartushpsdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/rawnetworkinterfacedriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/resetdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/serialdigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/serialdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/shelldriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/sigrokdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/smallubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21817 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/sshdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/ubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbaudiodriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbhidrelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbsdmuxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbsdwiredriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbstoragedriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.199910 labgrid-24.0a1/labgrid/driver/usbtmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbtmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbtmc/keysight_dsox2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbtmc/tektronix_tds2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbtmcdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/usbvideodriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/driver/xenadriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.199910 labgrid-24.0a1/labgrid/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/bootstrapprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/commandprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/consoleprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/digitaloutputprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/filesystemprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/filetransferprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/infoprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/linuxbootprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/mmioprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/powerprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/resetprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/protocol/videoprotocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.203910 labgrid-24.0a1/labgrid/pytestplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/pytestplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/pytestplugin/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/pytestplugin/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.203910 labgrid-24.0a1/labgrid/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    85195 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31382 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33317 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/remote/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.207910 labgrid-24.0a1/labgrid/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/dediprogflasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/ethernetport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/fastboot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/flashrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/httpdigitalout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/httpvideostream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/lxaiobus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/modbusrtu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/networkservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/onewireport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/pyvisa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/serialport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/sigrok.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24909 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/udev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/xenamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/resource/ykushpowerport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/stepreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.207910 labgrid-24.0a1/labgrid/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/bareboxstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/dockerstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/graphstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/shellstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/strategy/ubootstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.211910 labgrid-24.0a1/labgrid/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.211910 labgrid-24.0a1/labgrid/util/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/deditec_relais8.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/sysfsgpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/udisks2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agents/usb_hid_relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/agentwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/expect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/managedfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/qmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19343 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.223910 labgrid-24.0a1/labgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-09 13:52:30.000000 labgrid-24.0a1/labgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-04-09 13:52:30.000000 labgrid-24.0a1/labgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:52:30.000000 labgrid-24.0a1/labgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 13:52:30.000000 labgrid-24.0a1/labgrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-09 13:52:30.000000 labgrid-24.0a1/labgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 13:52:30.000000 labgrid-24.0a1/labgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-09 13:52:25.000000 labgrid-24.0a1/labgrid_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.215910 labgrid-24.0a1/man/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-client.1
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-device-config.5
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-device-config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-exporter.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-exporter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-pytest.7
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-pytest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-suggest.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-09 13:52:25.000000 labgrid-24.0a1/man/labgrid-suggest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 13:52:25.000000 labgrid-24.0a1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-09 13:52:25.000000 labgrid-24.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:52:30.227910 labgrid-24.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:52:30.223910 labgrid-24.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_autoinstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_bareboxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_crossbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_dediprogflasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_ethernetport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_externalconsoledriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_filedigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_flashrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_flashscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_graphstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_httpdigitalout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_httpvideo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_lxaiobus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_manualswitchdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_modbusrtudriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_onewire.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_openocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_powerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_processwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_pyvisa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_qemudriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_sched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_serialdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_serialport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_shelldriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_sigrok.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_sispm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_sshdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_steplogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_sysfsgpioagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14902 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_tasmota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_ubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_usbtmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_usbvideo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-09 13:52:25.000000 labgrid-24.0a1/tests/test_yaml.py
```

### Comparing `labgrid-23.1a2/.crossbar/config-anonymous.yaml` & `labgrid-24.0a1/.crossbar/config-anonymous.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,16 @@
       port: 20408
     paths:
       /:
         type: static
         directory: ../web
       ws:
         type: websocket
+        options:
+          auto_fragment_size: 65536
         auth:
           anonymous:
             type: static
             role: public
 - id: coordinator
   type: guest
   executable: /path/to/labgrid-venv/bin/python3
```

### Comparing `labgrid-23.1a2/.github/pull_request_template.md` & `labgrid-24.0a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/.github/workflows/build-and-release.yml` & `labgrid-24.0a1/.github/workflows/build-and-release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: workflow_call
 
 jobs:
   release:
     runs-on: ubuntu-22.04
     continue-on-error: false
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.11"
     - name: Install python dependencies
       run: |
         python -m pip install --upgrade pip build
     - name: Build sdist
       run: |
```

### Comparing `labgrid-23.1a2/.github/workflows/docker.yml` & `labgrid-24.0a1/.github/workflows/docker.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 name: docker build
 
 on:
   push:
     branches: [ master ]
+    tags:
+      - '*'
 
 jobs:
   docker:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install system dependencies
       run: |
         sudo apt install -yq python3-pip
-        python3 -m pip install setuptools_scm
+        pip install --upgrade setuptools
+        pip install setuptools_scm
     - name: Login to DockerHub
-      uses: docker/login-action@v2
+      uses: docker/login-action@v3
       with:
         username: ${{ secrets.DOCKERHUB_USERNAME }}
         password: ${{ secrets.DOCKERHUB_TOKEN }}
     - name: Build docker image
       run: |
         ./dockerfiles/build.sh
         docker-compose -f dockerfiles/staging/docker-compose.yml up --exit-code-from client client
         docker-compose -f dockerfiles/staging/docker-compose.yml down
         docker images
+    - name: Tag latest images
+      run: |
         docker tag labgrid-client ${{ secrets.DOCKERHUB_PREFIX }}client
         docker tag labgrid-exporter ${{ secrets.DOCKERHUB_PREFIX }}exporter
         docker tag labgrid-coordinator ${{ secrets.DOCKERHUB_PREFIX }}coordinator
-        docker push ${{ secrets.DOCKERHUB_PREFIX }}client
-        docker push ${{ secrets.DOCKERHUB_PREFIX }}exporter
-        docker push ${{ secrets.DOCKERHUB_PREFIX }}coordinator
-        docker images
+    - name: Tag release image
+      if: startsWith(github.ref, 'refs/tags')
+      run: |
+        docker tag labgrid-client ${{ secrets.DOCKERHUB_PREFIX }}client:${GITHUB_REF_NAME}
+        docker tag labgrid-exporter ${{ secrets.DOCKERHUB_PREFIX }}exporter:${GITHUB_REF_NAME}
+        docker tag labgrid-coordinator ${{ secrets.DOCKERHUB_PREFIX }}coordinator:${GITHUB_REF_NAME}
+    - name: Push to dockerhub
+      run: |
+        docker push --all-tags ${{ secrets.DOCKERHUB_PREFIX }}client
+        docker push --all-tags ${{ secrets.DOCKERHUB_PREFIX }}exporter
+        docker push --all-tags ${{ secrets.DOCKERHUB_PREFIX }}coordinator
+    - name: Show images again
+      run: docker images
```

### Comparing `labgrid-23.1a2/.github/workflows/push-pr-unit-tests.yml` & `labgrid-24.0a1/.github/workflows/push-pr-unit-tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   push-pr-unit-tests:
     name: unit tests
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
     uses: ./.github/workflows/reusable-unit-tests.yml
     with:
       python-version: ${{ matrix.python-version }}
   push-pr-unit-tests-docker:
     name: Docker Unit Tests
     uses: ./.github/workflows/reusable-unit-tests-docker.yml
   build-and-release:
```

### Comparing `labgrid-23.1a2/.github/workflows/reusable-unit-tests.yml` & `labgrid-24.0a1/.github/workflows/reusable-unit-tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,22 @@
         required: false
 
 jobs:
   build:
     runs-on: ubuntu-22.04
     continue-on-error: false
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         ref: ${{ inputs.branch }}
     - name: Set up Python ${{ inputs.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ inputs.python-version }}
-    - uses: actions/cache@v3
+    - uses: actions/cache@v4
       with:
         path: ~/.cache/pip
         key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
         restore-keys: |
           ${{ runner.os }}-pip-
     - name: Install system dependencies
       run: |
@@ -56,13 +56,16 @@
         pylint labgrid
     - name: Test with pytest
       run: |
         TERM=xterm pytest --cov-config .coveragerc --cov=labgrid --local-sshmanager --ssh-username runner --crossbar-venv crossbar-venv -k "not test_docker_with_daemon"
     - name: Build documentation
       run: |
         make -C doc clean
-        make -C doc doctest
-        make -C doc html
+        make -C doc doctest SPHINXOPTS=-W
+        make -C doc html SPHINXOPTS=-W
         make -C man clean
         make -C man all
         git --no-pager diff --exit-code
+        # check README.rst separately
+        pip install rstcheck
+        rstcheck --ignore-languages=bash --report-level=WARNING README.rst
     - uses: codecov/codecov-action@v3
```

### Comparing `labgrid-23.1a2/.github/workflows/scheduled-unit-tests.yml` & `labgrid-24.0a1/.github/workflows/scheduled-unit-tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 jobs:
   scheduled-unit-tests:
     name: scheduled unit tests
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
         branch: ['master']
     uses: ./.github/workflows/reusable-unit-tests.yml
     with:
       python-version: ${{ matrix.python-version }}
       branch: ${{ matrix.branch }}
   scheduled-unit-tests-docker:
     name: scheduled docker tests
     strategy:
       fail-fast: false
       matrix:
-        branch: ['master']
+        branch: ['master', 'stable-23.0']
     uses: ./.github/workflows/reusable-unit-tests-docker.yml
     with:
       branch: ${{ matrix.branch }}
```

### Comparing `labgrid-23.1a2/CHANGES.rst` & `labgrid-24.0a1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,57 @@
-Release 23.1 (unreleased)
-------------------------------------
+Release 24.0 (unreleased)
+-------------------------
 
-New Features in 23.1
+New Features in 24.0
 ~~~~~~~~~~~~~~~~~~~~
 - When invoking tests with pytest, the ``--log-(cli|file)-(level|format)``
   command line arguments and their corresponding pytest.ini configure options
   are now respected (making it possible to have different format and logging
   levels in the log file than then console).
 - A new log level called ``CONSOLE`` has been added between the default
   ``INFO`` and ``DEBUG`` levels. This level will show all reads and writes made
   to the serial console during testing.
+- The `QEMUDriver` now has an additional ``disk_opts`` property which can be
+  used to pass additional options for the disk directly to QEMU
+- labgrid-client now has a ``write-files`` subcommand to copy files onto mass
+  storage devices.
 
-Bug fixes in 23.1
+Bug fixes in 24.0
 ~~~~~~~~~~~~~~~~~
 - The pypi release now uses the labgrid pyserial fork in the form of the
   pyserial-labgrid package. This fixes installation with newer versions
   of pip.
 - Several tests have gained an importorskip() call to skip them if the
   module is not available.
 - The build-and-release workflow supports building wheels.
 - The markers now are restricted to patterns which won't match WARN,
   ERROR, INFO and similar log notifiers.
 - Fix named SSH lookups in conjunction with an environment file in
   labgrid-client.
-
-Breaking changes in 23.1
-~~~~~~~~~~~~~~~~~~~~~~~~~
+- Fix sftp option issue in SSH driver that caused sftp to only work once per
+  test run.
+- ManagedFile NFS detection heuristic now does symlink resolution on the
+  local host.
+- The password for the ShellDriver can now be an empty string.
+
+Breaking changes in 24.0
+~~~~~~~~~~~~~~~~~~~~~~~~
+- Support for the legacy ticket authentication was dropped: If the coordinator
+  logs ModuleNotFoundError on startup, switch the crossbar config to anonymous
+  authentication (see ``.crossbar/config-anonymous.yaml`` for an example).
 - The Debian package (``debian/``) no longer contains crossbar. Use the
   `coordinator container <https://hub.docker.com/r/labgrid/coordinator>`_ or
-  install it into a separate local venv as desribed in the
+  install it into a separate local venv as described in the
   `documentation <https://labgrid.readthedocs.io/en/latest/getting_started.html#coordinator>`_.
+  If you see ``WARNING: Ticket authentication is deprecated. Please update your
+  coordinator.`` on the client when running an updated coordinator, your
+  coordinator configuration may set ``ticket`` instead of ``anonymous`` auth.
 - The `StepReporter` API has been changed. To start step reporting, you must
-  now call ``StepReporter.start()`` instead of ``StepReporter()``
+  now call ``StepReporter.start()`` instead of ``StepReporter()``, and set up
+  logging via ``labgrid.logging.basicConfig()``.
 - Logging output when running pytest is no longer sent to stderr by default,
   since this is both chatty and also unnecessary with the improved logging
   flexibility. It it recommended to use the ``--log-cli-level=INFO`` command
   line option, or ``log_cli_level = INFO`` option in pytest.ini, but if you
   want to restore the old behavior add the following to your ``conftest.py``
   file (note that doing so may affect the ability to use some more advanced
   logging features)::
@@ -50,16 +66,25 @@
              stream=sys.stderr,
          )
 
 - The interpretation of the ``-v`` command line argument to pytest has changed
   slightly. ``-vv`` is now an alias for ``--log-cli-level=INFO`` (effectively
   unchanged), ``-vvv`` is an alias for ``--log-cli-level=CONSOLE``, and
   ``-vvvv`` is an alias for ``--log-cli-level=DEBUG``.
+- The `BareboxDriver` now remembers the log level, sets it to ``0`` on initial
+  activation/reset and recovers it on ``boot()``. During
+  ``run()``/``run_check()`` the initially detected log level is used.
+- The `NFSProviderDriver` now returns mount and path information on ``stage()``
+  instead of the path to be used on the target. The previous return value did
+  not fit the NFS mount use case.
+- The `NFSProvider` and `RemoteNFSProvider` resources no longer expect the
+  ``internal`` and ``external`` arguments as they do not fit the NFS mount use
+  case.
 
-Known issues in 23.1
+Known issues in 24.0
 ~~~~~~~~~~~~~~~~~~~~
 
 
 Release 23.0 (Released Apr 24, 2023)
 ------------------------------------
 
 New Features in 23.0
@@ -162,15 +187,15 @@
 - Fix udev matching by attributes.
 - Stop Exporter's event loop when register calls fail.
 - Fix exit codes for various subcommands.
 - Omit role and place output for ``labgrid-client reserve`` to fix shell
   evaluation.
 
 Breaking changes in 23.0
-~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~
 - ``Config``'s ``get_option()``/``get_target_option()`` convert non-string
   options no longer to strings.
 - `UBootDriver`'s ``boot_expression`` attribute is deprecated, it will no
   longer check for the string during U-Boot boot. This allows activating the
   driver on an already running U-Boot.
 - The uuu command handling was fixed for the UUUDriver.
 - `UBootDriver` boot() method was fixed.
@@ -242,15 +267,15 @@
 - Travis CI has been dropped for Github Actions.
 
 Breaking changes in 0.4.0
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 - ``EthernetInterface`` has been renamed to ``NetworkInterface``.
 
 Known issues in 0.4.0
-~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~
 - Some client commands return 0 even if the command failed.
 - Currently empty passwords are not well supported by the ShellDriver
 
 Release 0.3.0 (released Jan 22, 2021)
 -------------------------------------
 
 New Features in 0.3.0
@@ -339,15 +364,15 @@
 - The ``HawkbitTestClient`` and ``USBStick`` classes have been removed
 - The original USBStorageDriver was removed, ``NetworkUSBStorageDriver`` was
   renamed to `USBStorageDriver`.
   A deprecated `NetworkUSBStorageDriver` exists temporarily for compatibility
   reasons.
 
 Known issues in 0.3.0
-~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~
 - There are several reports of ``sshpass`` used within the SSHDriver not working
   in call cases or only on the first connection.
 - Some client commands return 0 even if the command failed.
 - Currently empty passwords are not well supported by the ShellDriver
 
 Release 0.2.0 (released Jan 4, 2019)
 ------------------------------------
```

### Comparing `labgrid-23.1a2/COPYING` & `labgrid-24.0a1/COPYING`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/LICENSE` & `labgrid-24.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/PKG-INFO` & `labgrid-24.0a1/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,35 @@
-Metadata-Version: 2.1
-Name: labgrid
-Version: 23.1a2
-Summary: embedded systems control library for development, testing and installation
-Author-email: Rouven Czerwinski <entwicklung@pengutronix.de>, Jan Luebbe <entwicklung@pengutronix.de>
-License: Copyright (C) 2016-2017 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
-        Copyright (C) 2016-2017 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
-        
-        This library is free software; you can redistribute it and/or
-        modify it under the terms of the GNU Lesser General Public
-        License as published by the Free Software Foundation; either
-        version 2.1 of the License, or (at your option) any later version.
-        
-        This library is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-        Lesser General Public License for more details.
-        
-        You should have received a copy of the GNU Lesser General Public
-        License along with this library; if not, write to the Free Software
-        Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
-        
-Project-URL: Homepage, https://github.com/labgrid-project/labgrid
-Project-URL: Bug Tracker, https://github.com/labgrid-project/labgrid/issues
-Classifier: Topic :: Software Development :: Testing
-Classifier: Framework :: Pytest
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: doc
-Provides-Extra: docker
-Provides-Extra: graph
-Provides-Extra: kasa
-Provides-Extra: modbus
-Provides-Extra: modbusrtu
-Provides-Extra: mqtt
-Provides-Extra: onewire
-Provides-Extra: pyvisa
-Provides-Extra: snmp
-Provides-Extra: vxi11
-Provides-Extra: xena
-Provides-Extra: deb
-Provides-Extra: dev
-License-File: LICENSE
-License-File: COPYING
-
-.. image:: labgrid_logo.png
+.. image:: https://raw.githubusercontent.com/labgrid-project/labgrid/master/labgrid_logo.png
    :alt: labgrid logo
    :align: center
 
 Welcome to labgrid
 ==================
-
 |license| |unit-tests| |docker-build| |coverage-status| |docs-status| |chat| |calver|
 
-Purpose
--------
 Labgrid is an embedded board control python library with a focus on testing, development
 and general automation.
 It includes a remote control layer to control boards connected to other hosts.
 
+* `Purpose and Features <#purpose-and-features>`_
+
+* `Documentation <#documentation>`_
+
+* `Contributing <#contributing>`_
+
+* `Background <#background>`_
+
+* `Installation <#installation>`_
+
+  * `Install Latest Release <#install-latest-release>`_
+
+  * `Install Development State <#install-development-state>`_
+
+Purpose and Features
+--------------------
 The idea behind labgrid is to create an abstraction of the hardware control
 layer needed for testing of embedded systems, automatic software installation
 and automation during development.
 Labgrid itself is *not* a testing framework, but is intended to be combined with
 `pytest <https://docs.pytest.org>`_ (and additional pytest plugins).
 Please see `Design Decisions
 <https://labgrid.readthedocs.io/en/latest/design_decisions.html>`_ for more
@@ -87,44 +50,57 @@
 - Docker/QEMU integration
 
 While labgrid is currently used for daily development on embedded boards and for
 automated testing, several planned features are not yet implemented and the APIs
 may be changed as more use-cases appear.
 We appreciate code contributions and feedback on using labgrid on other
 environments (see `Contributing
-<https://labgrid.readthedocs.io/en/latest/development.html#contributing>`_ for
+<https://labgrid.readthedocs.io/en/latest/development.html#contributing>`__ for
 details).
 Please consider contacting us (via a GitHub issue) before starting larger
 changes, so we can discuss design trade-offs early and avoid redundant work.
 You can also look at `Ideas
 <https://labgrid.readthedocs.io/en/latest/development.html#ideas>`_ for
 enhancements which are not yet implemented.
 
 Documentation
 -------------
-`Read the Docs <http://labgrid.readthedocs.io/en/latest/>`_
+labgrid's documentation is hosted on `Read the Docs <http://labgrid.readthedocs.io/en/latest/>`_.
 
 Contributing
 ------------
-`Development Docs <http://labgrid.readthedocs.io/en/latest/development.html>`_
+See our `Development Docs <http://labgrid.readthedocs.io/en/latest/development.html>`_.
 
-IRC channel ``#labgrid`` on libera.chat (bridged to the `Matrix channel
-#labgrid:matrix.org <https://app.element.io/#/room/#labgrid:matrix.org>`_)
+Visit us in our IRC channel ``#labgrid`` on libera.chat (bridged to the
+`Matrix channel #labgrid:matrix.org <https://app.element.io/#/room/#labgrid:matrix.org>`_)
 
 Background
 ----------
 Work on labgrid started at `Pengutronix <http://pengutronix.de/>`_ in late 2016
 and is currently in active use and development.
 
-Quickstart
-----------
+Installation
+------------
 See the `Installation section
 <http://labgrid.readthedocs.io/en/latest/getting_started.html#installation>`_
 for more details.
 
+Install Latest Release
+^^^^^^^^^^^^^^^^^^^^^^
+Install labgrid via PyPi:
+
+.. code-block:: bash
+
+   $ virtualenv -p python3 venv
+   $ source venv/bin/activate
+   venv $ pip install --upgrade pip
+   venv $ pip install labgrid
+
+Install Development State
+^^^^^^^^^^^^^^^^^^^^^^^^^
 Clone the git repository:
 
 .. code-block:: bash
 
    $ git clone https://github.com/labgrid-project/labgrid
 
 Create and activate a virtualenv for labgrid:
@@ -169,10 +145,10 @@
     :alt: documentation status
     :target: https://labgrid.readthedocs.io/en/latest/?badge=latest
 
 .. |chat| image:: https://matrix.to/img/matrix-badge.svg
     :alt: chat
     :target: https://app.element.io/#/room/#labgrid:matrix.org
 
-.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.%5BMICRO%5D-22bfda.svg
+.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR%5B.MICRO%5D-22bfda.svg
     :alt: chat
     :target: https://calver.org/
```

### Comparing `labgrid-23.1a2/contrib/completion/labgrid-client.bash` & `labgrid-24.0a1/contrib/completion/labgrid-client.bash`

 * *Files 2% similar despite different names*

```diff
@@ -765,14 +765,48 @@
         [ "$args" -ne 2 ] && return
 
         _filedir
         ;;
     esac
 }
 
+_labgrid_client_write_files()
+{
+    local cur prev words cword
+    _init_completion || return
+
+    case "$prev" in
+    -w|--wait)
+        ;&
+    -p|--partition)
+        ;&
+    -t|--target-directory)
+        ;&
+    -T)
+        ;&
+    -n|--name)
+        _labgrid_complete match-names "$cur"
+        return
+        ;;
+    esac
+
+    case "$cur" in
+    -*)
+        local options="--wait --partition --target-directory --name $_labgrid_shared_options"
+        COMPREPLY=( $(compgen -W "$options" -- "$cur") )
+        ;;
+    *)
+        local args
+        _labgrid_count_args "@(-w|--wait|-p|--partition|-t|--target-directory|-T|-n|--name)" || return
+
+        _filedir
+        ;;
+    esac
+}
+
 _labgrid_client_reserve()
 {
     _labgrid_client_generic_subcommand "--wait --shell --prio"
 }
 
 _labgrid_client_export()
 {
@@ -884,18 +918,20 @@
                                sshfs \
                                forward \
                                telnet \
                                video \
                                audio \
                                tmc \
                                write-image \
+                               write-files \
                                reserve \
                                cancel-reservation \
                                wait \
                                reservations \
+                               version \
                                export"
             COMPREPLY=( $(compgen -W "$subcommands" -- "$cur") )
             return
             ;;
         esac
     fi
```

### Comparing `labgrid-23.1a2/contrib/coordinator-statsd.py` & `labgrid-24.0a1/contrib/coordinator-statsd.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 import sys
 import argparse
 import statsd
 import os
 import labgrid.remote.client
 import time
 import asyncio
+import txaio
 
 
 def inc_gauge(gauges, key):
     gauges.setdefault(key, 0)
     gauges[key] += 1
 
 
@@ -137,14 +138,17 @@
         help="Tag values to include in statsd path for reservations. Repeat to include multiple tags",
         action="append",
         default=[],
     )
 
     args = parser.parse_args()
 
+    txaio.use_asyncio()
+    txaio.config.loop = asyncio.get_event_loop()
+
     statsd_client = None
     gauges = {}
 
     next_time = time.monotonic()
 
     while True:
         if statsd_client is None:
@@ -173,21 +177,23 @@
         try:
             extra = {}
             session = labgrid.remote.client.start_session(
                 args.crossbar,
                 os.environ.get("LG_CROSSBAR_REALM", "realm1"),
                 extra,
             )
-
-            session.loop.run_until_complete(
-                asyncio.gather(
-                    report_places(session, args.tags, gauges),
-                    report_reservations(session, args.tags, gauges),
+            try:
+                session.loop.run_until_complete(
+                    asyncio.gather(
+                        report_places(session, args.tags, gauges),
+                        report_reservations(session, args.tags, gauges),
+                    )
                 )
-            )
+            finally:
+                session.leave()
         except labgrid.remote.client.Error as e:
             print(f"Error communicating with labgrid: {e}")
             continue
 
         try:
             with statsd_client.pipeline() as pipe:
                 for k, v in gauges.items():
```

### Comparing `labgrid-23.1a2/contrib/sync-places.py` & `labgrid-24.0a1/contrib/sync-places.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,46 +58,66 @@
             if not name in seen_places:
                 print(f"Adding place {name}")
                 if not args.dry_run:
                     await session.call("org.labgrid.coordinator.add_place", name)
                 changed = True
 
         for name in config["places"]:
-            matches = config["places"][name].get("matches", [])
+            matches = []
+            for m in config["places"][name].get("matches", []):
+                if isinstance(m, dict):
+                    match = list(m.keys())[0]
+                    matches.append((match, m[match]))
+                else:
+                    matches.append((m, None))
+
             seen_matches = set()
             remove_matches = set()
             place_tags = {}
             if name in seen_places:
                 place = session.places[name]
-                for m in place.matches:
-                    m = repr(m)
+                for m in [(repr(x), x.rename) for x in place.matches]:
                     if m in matches:
                         seen_matches.add(m)
                     else:
                         remove_matches.add(m)
                 place_tags = place.tags
 
             for m in remove_matches:
-                print(f"Deleting match '{m}' for place {name}")
+                match, rename = m
+                if rename:
+                    print(f"Deleting named match '{match} -> {rename}' for place {name}")
+                else:
+                    print(f"Deleting match '{match}' for place {name}")
                 if not args.dry_run:
                     await session.call(
-                        "org.labgrid.coordinator.del_place_match", name, m
+                        "org.labgrid.coordinator.del_place_match", name, match, rename
                     )
                 changed = True
 
             for m in matches:
                 if not m in seen_matches:
-                    print(f"Adding match '{m}' for place {name}")
+                    match, rename = m
+                    if rename:
+                        print(f"Adding named match '{match} -> {rename}' for place {name}")
+                    else:
+                        print(f"Adding match '{match}' for place {name}")
+
                     if not args.dry_run:
                         await session.call(
-                            "org.labgrid.coordinator.add_place_match", name, m
+                            "org.labgrid.coordinator.add_place_match", name, match, rename
                         )
                     changed = True
 
             tags = config["places"][name].get("tags", {}).copy()
+            for k, v in tags.items():
+                if not isinstance(k, str) or not isinstance(v, str):
+                    del(tags[k])
+                    tags[str(k)] = str(v)
+
             if place_tags != tags:
                 print(
                     "Setting tags for place %s to %s"
                     % (
                         name,
                         ", ".join(
                             "%s=%s" % (key, value) for (key, value) in tags.items()
@@ -116,15 +136,18 @@
                     )
                 changed = True
 
     async def do_dump(session, args):
         config = {"places": {}}
         for name, place in session.places.items():
             config["places"][name] = {
-                "matches": [repr(m) for m in place.matches],
+                "matches": [
+                    {repr(m): m.rename} if m.rename else repr(m)
+                    for m in place.matches
+                    ],
                 "tags": {k: v for k, v in place.tags.items()},
             }
 
         with get_file(args.dest, "w", sys.stdout) as f:
             yaml.dump(config, f)
 
     parser = argparse.ArgumentParser(
@@ -135,14 +158,15 @@
             strings and tags should be assigned to those places. The files are
             structured like:
 
               places: # A dictonary of places where each key is a place name
                 my-place1: # Replace with your place
                   matches: # A list of match patterns. Replace with your match patterns
                     - "*/my-place1/*"
+                    - "exporter/my-place1/resource": name # named matches supported
                   tags: # A dictionary of key/value tags. Replace with your tags
                     board: awesomesauce
                     bar: baz
 
             When syncing places, tags, and matches will be added or removed until the
             remote configuration matches the one in the YAML file
             """
```

### Comparing `labgrid-23.1a2/debian/control` & `labgrid-24.0a1/debian/control`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/debian/copyright` & `labgrid-24.0a1/debian/copyright`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Format: https://www.debian.org/doc/packaging-manuals/copyright-format/1.0/
 Upstream-Name: labgrid
 Source: https://github.com/labgrid-project/labgrid
 
 Files: *
-Copyright: Copyright (C) 2016-2023 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
-           Copyright (C) 2016-2023 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
+Copyright: Copyright (C) 2016-2024 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
+           Copyright (C) 2016-2024 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
 License: LGPL-2.1+
 
 Files: man/*
-Copyright: Copyright (C) 2016-2023 Pengutronix
+Copyright: Copyright (C) 2016-2024 Pengutronix
 License: LGPL-2.1+
 
 License: LGPL-2.1+
  This library is free software; you can redistribute it and/or
  modify it under the terms of the GNU Lesser General Public
  License as published by the Free Software Foundation; either
  version 2.1 of the License, or (at your option) any later version.
```

### Comparing `labgrid-23.1a2/doc/Makefile` & `labgrid-24.0a1/doc/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
-SPHINXOPTS    = -W
+SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 SPHINXPROJ    = labgrid
 SOURCEDIR     = .
 BUILDDIR      = .build
 
 # Put it first so that "make" without argument is like "make help".
 help:
```

### Comparing `labgrid-23.1a2/doc/RELEASE.rst` & `labgrid-24.0a1/doc/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/conf.py` & `labgrid-24.0a1/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.doctest',
               'sphinx.ext.napoleon',
               'sphinx.ext.coverage',
               'sphinx.ext.viewcode',
-              'sphinx.ext.autosectionlabel']
+              'sphinx.ext.autosectionlabel',
+              'sphinx_rtd_theme']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['.templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -52,15 +53,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'labgrid'
-copyright = '2016-2023 Pengutronix, Jan Luebbe and Rouven Czerwinski'
+copyright = '2016-2024 Pengutronix, Jan Luebbe and Rouven Czerwinski'
 author = 'Jan Luebbe, Rouven Czerwinski'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
@@ -181,14 +182,15 @@
         'special-members': True,
 }
 autodoc_mock_imports = ['onewire',
                         'txaio',
                         'autobahn',
                         'autobahn.asyncio',
                         'autobahn.asyncio.wamp',
+                        'autobahn.asyncio.websocket',
                         'autobahn.wamp',
                         'autobahn.wamp.types',
                         'autobahn.twisted',
                         'autobahn.twisted.wamp',
                         'autobahn.wamp.exception',
                         'twisted.internet.defer',
                         'gi',
```

### Comparing `labgrid-23.1a2/doc/configuration.rst` & `labgrid-24.0a1/doc/configuration.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,349 +4,362 @@
 configuration.
 Drivers can depend on resources or other drivers, whereas resources
 have no dependencies.
 
 .. image:: res/config_graph.svg
    :width: 50%
 
-Here the resource `RawSerialPort` provides the information for the
-`SerialDriver`, which in turn is needed by the `ShellDriver`.
+Here the resource `RawSerialPort`_ provides the information for the
+`SerialDriver`_, which in turn is needed by the `ShellDriver`_.
 Driver dependency resolution is done by searching for the driver which
 implements the dependent protocol, all drivers implement one or more protocols.
 
 Resources
 ---------
 
 Serial Ports
 ~~~~~~~~~~~~
 
 RawSerialPort
 +++++++++++++
-A RawSerialPort is a serial port which is identified via the device path on the
-local computer.
+A :any:`RawSerialPort` is a serial port which is identified via the device path
+on the local computer.
 Take note that re-plugging USB serial converters can result in a different
 enumeration order.
 
 .. code-block:: yaml
 
    RawSerialPort:
-     port: /dev/ttyUSB0
+     port: '/dev/ttyUSB0'
      speed: 115200
 
-The example would access the serial port /dev/ttyUSB0 on the local computer with
-a baud rate of 115200.
+The example would access the serial port ``/dev/ttyUSB0`` on the local computer
+with a baud rate of ``115200``.
 
 Arguments:
   - port (str): path to the serial device
   - speed (int, default=115200): desired baud rate
 
 Used by:
   - `SerialDriver`_
 
 NetworkSerialPort
 +++++++++++++++++
-A NetworkSerialPort describes a serial port which is exported over the network,
-usually using RFC2217 or raw tcp.
+A :any:`NetworkSerialPort` describes a serial port which is exported over the
+network, usually using `RFC2217 <https://datatracker.ietf.org/doc/rfc2217/>`_
+or raw TCP.
 
 .. code-block:: yaml
 
    NetworkSerialPort:
-     host: remote.example.computer
+     host: 'remote.example.computer'
      port: 53867
      speed: 115200
 
-The example would access the serial port on computer remote.example.computer via
-port 53867 and use a baud rate of 115200 with the RFC2217 protocol.
+The example would access the serial port on computer
+``remote.example.computer`` via port ``53867`` and use a baud rate of
+``115200`` with the RFC2217 protocol.
 
 Arguments:
   - host (str): hostname of the remote host
   - port (str): TCP port on the remote host to connect to
   - speed (int, default=115200): baud rate of the serial port
   - protocol (str, default="rfc2217"): protocol used for connection: raw or
     rfc2217
 
 Used by:
   - `SerialDriver`_
 
 ModbusRTU
 +++++++++
-Describes the resource required to use the ModbusRTU driver.
+A :any:`ModbusRTU` resource is required to use the `ModbusRTUDriver`_.
 `Modbus RTU <https://en.wikipedia.org/wiki/Modbus>`_ is a communication
 protocol used to control many different kinds of electronic systems, such as
 thermostats, power plants, etc.
 Modbus is normally implemented on top of RS-485, though this is not strictly
 necessary, as long as the Modbus network only has one master (and up to 256
 slaves).
 
-The labgrid driver is implemented using the minimalmodbus Python library.
-The implementation only supports that labgrid will be the master on the Modbus
-network.
-For more information, see `minimalmodbus
-<https://minimalmodbus.readthedocs.io/en/stable/>`_.
-
-This resource and driver only supports local usage and will not work with an
-exporter.
+This resource only supports local usage and will not work with an exporter.
 
 .. code-block:: yaml
 
     ModbusRTU:
-      port: "/dev/ttyUSB0"
+      port: '/dev/ttyUSB0'
       address: 16
       speed: 115200
       timeout: 0.25
 
 Arguments:
-  - port (str): tty the instrument is connected to, e.g. '/dev/ttyUSB0'
+  - port (str): tty the instrument is connected to, e.g. ``/dev/ttyUSB0``
   - address (int): slave address on the modbus, e.g. 16
   - speed (int, default=115200): baud rate of the serial port
-  - timeout (float, default=0.25): optional, timeout in seconds
+  - timeout (float, default=0.25): timeout in seconds
 
 Used by:
   - `ModbusRTUDriver`_
 
 USBSerialPort
 +++++++++++++
-A USBSerialPort describes a serial port which is connected via USB and is
-identified by matching udev properties.
+A :any:`USBSerialPort` describes a serial port which is connected via USB and
+is identified by matching udev properties.
 This allows identification through hot-plugging or rebooting.
 
 .. code-block:: yaml
 
    USBSerialPort:
      match:
-       ID_SERIAL_SHORT: P-00-00682
+       ID_SERIAL_SHORT: 'P-00-00682'
+       ID_USB_INTERFACE_NUM: '00'
      speed: 115200
 
-The example would search for a USB serial converter with the key
-`ID_SERIAL_SHORT` and the value `P-00-00682` and use it with a baud rate
-of 115200.
-The `ID_SERIAL_SHORT` property is set by the usb_id builtin helper program.
+The example would search for a USB serial converter with a given serial number
+(``ID_SERIAL_SHORT`` = ``P-00-00682``) and use first interface
+(``ID_USB_INTERFACE_NUM`` = ``00``) with a baud rate of 115200.
+
+The ``ID_SERIAL_SHORT`` and ``ID_USB_INTERFACE_NUM`` properties are set by the
+``usb_id`` builtin helper program.
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
   - speed (int, default=115200): baud rate of the serial port
 
 Used by:
   - `SerialDriver`_
 
 Power Ports
 ~~~~~~~~~~~
 
 NetworkPowerPort
 ++++++++++++++++
-A NetworkPowerPort describes a remotely switchable power port.
+A :any:`NetworkPowerPort` describes a remotely switchable power port.
 
 .. code-block:: yaml
 
    NetworkPowerPort:
-     model: gude
-     host: powerswitch.example.computer
+     model: 'gude'
+     host: 'powerswitch.example.computer'
      index: 0
 
 The example describes port 0 on the remote power switch
-`powerswitch.example.computer`, which is a `gude` model.
+``powerswitch.example.computer``, which is a ``gude`` model.
 
 Arguments:
   - model (str): model of the power switch
   - host (str): hostname of the power switch
   - index (int): number of the port to switch
 
-The `model` property selects one of several `backend implementations
+The ``model`` property selects one of several `backend implementations
 <https://github.com/labgrid-project/labgrid/tree/master/labgrid/driver/power>`_.
 Currently available are:
 
 ``apc``
-  Controls an APU PDU via SNMP.
+  Controls *APU PDUs* via SNMP.
 
 ``digipower``
-  Controls a DigiPower PDU via a simple HTTP API.
+  Controls *DigiPower PDUs* via a simple HTTP API.
 
 ``digitalloggers_http``
-  Control a Digital Loggers PDU that use the legacy HTTP API. Note that
+  Controls *Digital Loggers PDUs* that use the legacy HTTP API. Note that
   host argument must include the protocol, such as
   ``http://192.168.0.3`` or ``http://admin:pass@192.168.0.4``.
 
 ``eaton``
-  Controls Eaton ePDUs via SNMP.
+  Controls *Eaton ePDUs* via SNMP.
 
 ``eg_pms2_network``
-  Controls the EG_PMS2_LAN & EG_PMS2_WLAN devices, through simple HTTP POST and
-  GET requests.  The device requires a password for logging into the control
-  interface, this module deliberately uses the standard password '1' and is
-  not compatible with a different password.
+  Controls *EG_PMS2_LAN* and *EG_PMS2_WLAN* devices, through simple HTTP POST
+  and GET requests. The device requires a password for logging into the
+  control interface, this module deliberately uses the standard password ``1``
+  and is not compatible with a different password.
+
+``eth008``
+  Controls *Robot-Electronics eth008* via a simple HTTP API.
 
 ``gude``
-  Controls a Gude PDU via a simple HTTP API.
+  Controls *Gude PDUs* via a simple HTTP API.
 
 ``gude24``
-  Controls a Gude Expert Power Control 8008 PDU via a simple HTTP API.
+  Controls *Gude Expert Power Control 8008 PDUs* via a simple HTTP API.
 
 ``gude8031``
-  Controls a Gude Expert Power Control 8031 PDU via a simple HTTP API.
+  Controls *Gude Expert Power Control 8031 PDUs* via a simple HTTP API.
 
 ``gude8225``
-  Controls a Gude Expert Power Control 8225 PDU via a simple HTTP API.
+  Controls *Gude Expert Power Control 8225 PDUs* via a simple HTTP API.
 
 ``gude8316``
-  Controls a Gude Expert Power Control 8316 PDU via a simple HTTP API.
+  Controls *Gude Expert Power Control 8316 PDUs* via a simple HTTP API.
 
 ``netio``
-  Controls a NETIO 4-Port PDU via a simple HTTP API.
+  Controls *NETIO 4-Port PDUs* via a simple HTTP API.
 
 ``netio_kshell``
-  Controls a NETIO 4C PDU via a Telnet interface.
+  Controls *NETIO 4C PDUs* via a Telnet interface.
+
+``raritan``
+  Controls *Raritan PDUs* via SNMP.
 
 ``rest``
   This is a generic backend for PDU implementations which can be controlled via
   HTTP PUT and GET requests.
   See the `docstring in the module
   <https://github.com/labgrid-project/labgrid/blob/master/labgrid/driver/power/rest.py>`__
   for details.
 
 ``sentry``
-  Controls a Sentry PDU via SNMP using Sentry3-MIB.
-  It was tested on CW-24VDD and 4805-XLS-16.
+  Controls *Sentry PDUs* via SNMP using Sentry3-MIB.
+  It was tested on *CW-24VDD* and *4805-XLS-16*.
 
 ``shelly_gen1``
-  Controls relays of Shelly devices using the Gen 1 Device API.
+  Controls relays of *Shelly* devices using the Gen 1 Device API.
   See the `docstring in the module
   <https://github.com/labgrid-project/labgrid/blob/master/labgrid/driver/power/shelly_gen1.py>`__
   for details.
 
 ``siglent``
-  Controls Siglent SPD3000X series modules via the `vxi11 Python module
+  Controls *Siglent SPD3000X* series modules via the `vxi11 Python module
   <https://pypi.org/project/python-vxi11/>`_.
 
 ``simplerest``
   This is a generic backend for PDU implementations which can be controlled via
   HTTP GET requests (both set and get).
   See the `docstring in the module
   <https://github.com/labgrid-project/labgrid/blob/master/labgrid/driver/power/simplerest.py>`__
   for details.
 
 ``tplink``
-  Controls TP-Link power strips via `python-kasa
+  Controls *TP-Link power strips* via `python-kasa
   <https://github.com/python-kasa/python-kasa>`_.
 
+``poe_mib``
+  Controls PoE switches using the PoE SNMP administration MiBs.
+
 Used by:
   - `NetworkPowerDriver`_
 
 PDUDaemonPort
 +++++++++++++
-A PDUDaemonPort describes a PDU port accessible via `PDUDaemon
+A :any:`PDUDaemonPort` describes a PDU port accessible via `PDUDaemon
 <https://github.com/pdudaemon/pdudaemon>`_.
 As one PDUDaemon instance can control many PDUs, the instance name from the
 PDUDaemon configuration file needs to be specified.
 
 .. code-block:: yaml
 
    PDUDaemonPort:
-     host: pduserver
-     pdu: apc-snmpv3-noauth
+     host: 'pduserver'
+     pdu: 'apc-snmpv3-noauth'
      index: 1
 
-The example describes port 1 on the PDU configured as `apc-snmpv3-noauth`, with
-PDUDaemon running on the host `pduserver`.
+The example describes port ``1`` on the PDU configured as
+``apc-snmpv3-noauth``, with PDUDaemon running on the host ``pduserver``.
 
 Arguments:
   - host (str): name of the host running the PDUDaemon
   - pdu (str): name of the PDU in the configuration file
   - index (int): index of the power port on the PDU
 
 Used by:
   - `PDUDaemonDriver`_
 
 YKUSHPowerPort
 ++++++++++++++
-A YKUSHPowerPort describes a YEPKIT YKUSH USB (HID) switchable USB hub.
+A :any:`YKUSHPowerPort` describes a *YEPKIT YKUSH* USB (HID) switchable USB
+hub.
 
 .. code-block:: yaml
 
    YKUSHPowerPort:
-     serial: YK12345
+     serial: 'YK12345'
      index: 1
 
 The example describes port 1 on the YKUSH USB hub with the
-serial "YK12345".
-(use "pykush -l" to get your serial...)
+serial ``YK12345``.
+Use ``ykushcmd -l`` to get your serial number.
 
 Arguments:
   - serial (str): serial number of the YKUSH hub
   - index (int): number of the port to switch
 
 Used by:
   - `YKUSHPowerDriver`_
 
+NetworkYKUSHPowerPort
++++++++++++++++++++++
+A :any:`NetworkYKUSHPowerPort` describes a `YKUSHPowerPort`_ available on a
+remote computer.
+
 USBPowerPort
 ++++++++++++
-A USBPowerPort describes a generic switchable USB hub as supported by
+A :any:`USBPowerPort` describes a generic switchable USB hub as supported by
 `uhubctl <https://github.com/mvp/uhubctl>`_.
 
 .. code-block:: yaml
 
    USBPowerPort:
      match:
-       ID_PATH: pci-0000:00:14.0-usb-0:2:1.0
+       ID_PATH: 'pci-0000:00:14.0-usb-0:2:1.0'
      index: 1
 
 The example describes port 1 on the hub with the ID_PATH
-"pci-0000:00:14.0-usb-0:2:1.0".
+``pci-0000:00:14.0-usb-0:2:1.0``.
 (use ``udevadm info /sys/bus/usb/devices/...`` to find the ID_PATH value)
 
 Arguments:
   - index (int): number of the port to switch
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `USBPowerDriver`_
 
 .. note::
-   Labgrid requires that the interface is contained in the ID_PATH.
+   labgrid requires that the interface is contained in the ID_PATH.
    This usually means that the ID_PATH should end with ``:1.0``.
    Only this first interface is registered with the ``hub`` driver labgrid is
    looking for, paths without the interface will fail to match since they use
    the ``usb`` driver.
 
 SiSPMPowerPort
 ++++++++++++++
-A SiSPMPowerPort describes a GEMBIRD SiS-PM as supported by
+A :any:`SiSPMPowerPort` describes a *GEMBIRD SiS-PM* as supported by
 `sispmctl <https://sourceforge.net/projects/sispmctl/>`_.
 
 .. code-block:: yaml
 
    SiSPMPowerPort:
      match:
-       ID_PATH: platform-1c1a400.usb-usb-0:2
+       ID_PATH: 'platform-1c1a400.usb-usb-0:2'
      index: 1
 
 The example describes port 1 on the hub with the ID_PATH
-"platform-1c1a400.usb-usb-0:2".
+``platform-1c1a400.usb-usb-0:2``.
 
 Arguments:
   - index (int): number of the port to switch
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `SiSPMPowerDriver`_
 
 TasmotaPowerPort
 ++++++++++++++++
-A :any:`TasmotaPowerPort` resource describes a switchable Tasmota power outlet
-accessed over MQTT.
+A :any:`TasmotaPowerPort` resource describes a switchable `Tasmota
+<https://tasmota.github.io/docs/>`_ power outlet accessed over *MQTT*.
 
 .. code-block:: yaml
 
    TasmotaPowerPort:
-     host: this.is.an.example.host.com
-     status_topic: stat/tasmota_575A2B/POWER
-     power_topic: cmnd/tasmota_575A2B/POWER
-     avail_topic: tele/tasmota_575A2B/LWT
+     host: 'this.is.an.example.host.com'
+     status_topic: 'stat/tasmota_575A2B/POWER'
+     power_topic: 'cmnd/tasmota_575A2B/POWER'
+     avail_topic: 'tele/tasmota_575A2B/LWT'
 
-The example uses a mosquitto server at "this.is.an.example.host.com" and has the
-topics setup for a tasmota power port that has the ID 575A2B.
+The example uses a *Mosquitto* server at ``this.is.an.example.host.com`` and
+has the topics setup for a Tasmota power port that has the ID ``575A2B``.
 
 Arguments:
   - host (str): hostname of the MQTT server
   - status_topic (str): topic that signals the current status as "ON" or "OFF"
   - power_topic (str): topic that allows switching the status between "ON" and
     "OFF"
   - avail_topic (str): topic that signals the availability of the Tasmota power
@@ -356,146 +369,221 @@
   - `TasmotaPowerDriver`_
 
 Digital Outputs
 ~~~~~~~~~~~~~~~
 
 ModbusTCPCoil
 +++++++++++++
-A ModbusTCPCoil describes a coil accessible via ModbusTCP.
+A :any:`ModbusTCPCoil` describes a coil accessible via *Modbus TCP*.
 
 .. code-block:: yaml
 
    ModbusTCPCoil:
-     host: "192.168.23.42"
+     host: '192.168.23.42'
      coil: 1
 
-The example describes the coil with the address 1 on the ModbusTCP device
-`192.168.23.42`.
+The example describes the coil with the address ``1`` on the Modbus TCP device
+``192.168.23.42``.
 
 Arguments:
-  - host (str): hostname of the Modbus TCP server e.g. "192.168.23.42:502"
-  - coil (int): index of the coil e.g. 3
+  - host (str): hostname of the Modbus TCP server e.g. ``192.168.23.42:502``
+  - coil (int): index of the coil, e.g. ``3``
   - invert (bool, default=False): whether the logic level is inverted
     (active-low)
   - write_multiple_coils (bool, default=False): whether to perform write
     using "write multiple coils" method instead of "write single coil"
 
 Used by:
   - `ModbusCoilDriver`_
 
 DeditecRelais8
 ++++++++++++++
-A DeditecRelais8 describes a Deditec USB GPO module with 8 relays.
+A :any:`DeditecRelais8` describes a *Deditec USB GPO module* with 8 relays.
 
 .. code-block:: yaml
 
    DeditecRelais8:
      index: 1
      invert: false
      match:
-       ID_PATH: pci-0000:00:14.0-usb-0:2:1.0
+       ID_PATH: 'pci-0000:00:14.0-usb-0:2:1.0'
 
 Arguments:
   - index (int): number of the relay to use
   - invert (bool, default=False): whether the logic level is inverted
     (active-low)
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `DeditecRelaisDriver`_
 
 OneWirePIO
 ++++++++++
-A OneWirePIO describes a onewire programmable I/O pin.
+A :any:`OneWirePIO` describes a *1-Wire* programmable I/O pin.
 
 .. code-block:: yaml
 
    OneWirePIO:
-     host: example.computer
-     path: /29.7D6913000000/PIO.0
+     host: 'example.computer'
+     path: '/29.7D6913000000/PIO.0'
      invert: false
 
-The example describes a `PIO.0` at device address `29.7D6913000000` via the onewire
-server on `example.computer`.
+The example describes a ``PIO.0`` at device address ``29.7D6913000000`` via the
+1-Wire server on ``example.computer``.
 
 Arguments:
-  - host (str): hostname of the remote system running the onewire server
+  - host (str): hostname of the remote system running the 1-Wire server
   - path (str): path on the server to the programmable I/O pin
   - invert (bool, default=False): whether the logic level is inverted
     (active-low)
 
 Used by:
   - `OneWirePIODriver`_
 
 LXAIOBusPIO
 +++++++++++
 An :any:`LXAIOBusPIO` resource describes a single PIO pin on an LXAIOBusNode.
 
 .. code-block:: yaml
 
    LXAIOBusPIO:
-     host: localhost:8080
-     node: IOMux-00000003
-     pin: OUT0
-     invert: False
+     host: 'localhost:8080'
+     node: 'IOMux-00000003'
+     pin: 'OUT0'
+     invert: false
 
-The example uses an lxa-iobus-server running on localhost:8080, with node
-IOMux-00000003 and pin OUT0.
+The example uses an lxa-iobus-server running on ``localhost:8080``, with node
+``IOMux-00000003`` and pin ``OUT0``.
 
 Arguments:
   - host (str): hostname with port of the lxa-io-bus server
   - node (str): name of the node to use
   - pin (str): name of the pin to use
   - invert (bool, default=False): whether to invert the pin
 
 Used by:
   - `LXAIOBusPIODriver`_
 
 NetworkLXAIOBusPIO
 ++++++++++++++++++
-A NetworkLXAIOBusPIO describes an `LXAIOBusPIO`_ exported over the network.
+A :any:`NetworkLXAIOBusPIO` describes an `LXAIOBusPIO`_ exported over the network.
 
 HIDRelay
 ++++++++
-An :any:`HIDRelay` resource describes a single output of a HID protocol based
+An :any:`HIDRelay` resource describes a single output of an HID protocol based
 USB relays.
-It currently supports the widely used "dcttech USBRelay".
+It currently supports the widely used *dcttech USBRelay*.
 
 .. code-block:: yaml
 
    HIDRelay:
      index: 2
-     invert: False
+     invert: false
      match:
-       ID_PATH: pci-0000:00:14.0-usb-0:2:1.0
+       ID_PATH: 'pci-0000:00:14.0-usb-0:2:1.0'
 
 Arguments:
   - index (int, default=1): number of the relay to use
   - invert (bool, default=False): whether to invert the relay
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `HIDRelayDriver`_
 
+HttpDigitalOutput
++++++++++++++++++
+An :any:`HttpDigitalOutput` resource describes a generic digital output that
+can be controlled via HTTP.
+
+.. code-block:: yaml
+
+   HttpDigitalOutput:
+     url: 'http://host.example/some/endpoint'
+     body_asserted: 'On'
+     body_deasserted: 'Off'
+
+The example assumes a simple scenario where the same URL is used for PUT
+requests that set the output state and GET requests to get the current state.
+It also assumes that the returned state matches either "On" or "Off" exactly.
+
+The `HttpDigitalOutputDriver`_ also supports more advanced use cases where the
+current state is fetched from another URL and is interpreted using regular
+expressions.
+
+Arguments:
+  - url (str): URL to use for setting a new state
+  - body_asserted (str): Request body to send to assert the output
+  - body_deasserted (str): Request body to send to de-assert the output
+  - method (str, default="PUT"): HTTP method to set a new state
+
+  - url_get (str): URL to use instead of ``url`` for getting the state
+  - body_get_asserted (str): Regular Expression that matches an asserted response body
+  - body_get_deasserted (str): Regular Expression that matches a de-asserted response body
+
+Used by:
+  - `HttpDigitalOutputDriver`_
+
 NetworkHIDRelay
 +++++++++++++++
-A NetworkHIDRelay describes an `HIDRelay`_ exported over the network.
+A :any:`NetworkHIDRelay` describes an `HIDRelay`_ exported over the network.
+
+SysfsGPIO
++++++++++
+
+A :any:`SysfsGPIO` resource describes a GPIO line.
+
+.. code-block:: yaml
+
+   SysfsGPIO:
+     index: 12
+
+Arguments:
+  - index (int): index of the GPIO line
+
+Used by:
+  - `GpioDigitalOutputDriver`_
+
+MatchedSysfsGPIO
+++++++++++++++++
+A :any:`MatchedSysfsGPIO` describes a GPIO line, like a `SysfsGPIO`_.
+The gpiochip is identified by matching udev properties. This allows
+identification through hot-plugging or rebooting for controllers like
+USB based gpiochips.
+
+.. code-block:: yaml
+
+   MatchedSysfsGPIO:
+     match:
+       '@SUBSYSTEM': 'usb'
+       '@ID_SERIAL_SHORT': 'D38EJ8LF'
+     pin: 0
+
+The example would search for a USB gpiochip with the key `ID_SERIAL_SHORT`
+and the value `D38EJ8LF` and use the pin 0 of this device.
+The `ID_SERIAL_SHORT` property is set by the usb_id builtin helper program.
+
+Arguments:
+  - match (dict): key and value pairs for a udev match, see `udev Matching`_
+  - pin (int): gpio pin number within the matched gpiochip.
+
+Used by:
+  - `GpioDigitalOutputDriver`_
 
 NetworkService
 ~~~~~~~~~~~~~~
-A NetworkService describes a remote SSH connection.
+A :any:`NetworkService` describes a remote SSH connection.
 
 .. code-block:: yaml
 
    NetworkService:
-     address: example.computer
-     username: root
+     address: 'example.computer'
+     username: 'root'
 
-The example describes a remote SSH connection to the computer `example.computer`
-with the username `root`.
+The example describes a remote SSH connection to the computer
+``example.computer`` with the username ``root``.
 Set the optional password password property to make SSH login with a password
 instead of the key file.
 
 When used with ``labgrid-exporter``, the address can contain a device scope
 suffix (such as ``%eth1``), which is especially useful with overlapping address
 ranges or link-local IPv6 addresses.
 In that case, the SSH connection will be proxied via the exporter, using
@@ -509,456 +597,462 @@
   - port (int, default=22): port used by SSH
 
 Used by:
   - `SSHDriver`_
 
 USBMassStorage
 ~~~~~~~~~~~~~~
-A USBMassStorage resource describes a USB memory stick or similar device.
+A :any:`USBMassStorage` resource describes a USB memory stick or similar
+device.
 
 .. code-block:: yaml
 
    USBMassStorage:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0-scsi-0:0:0:3
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0-scsi-0:0:0:3'
+
+Writing images to disk requires installation of ``dd`` or optionally
+``bmaptool`` on the same system as the block device.
+
+For mounting the file system and writing into it,
+`PyGObject <https://pygobject.readthedocs.io/>`_ must be installed.
+For Debian, the necessary packages are `python3-gi` and `gir1.2-udisks-2.0`.
+This is not required for writing images to disks.
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `USBStorageDriver`_
 
 NetworkUSBMassStorage
 ~~~~~~~~~~~~~~~~~~~~~
-A NetworkUSBMassStorage resource describes a USB memory stick or similar
+A :any:`NetworkUSBMassStorage` resource describes a USB memory stick or similar
 device available on a remote computer.
 
-Used by:
-  - `USBStorageDriver`_
-
 The NetworkUSBMassStorage can be used in test cases by calling the
-`write_image()`, and `get_size()` functions.
+``write_files()``, ``write_image()``, and ``get_size()`` functions.
 
 SigrokDevice
 ~~~~~~~~~~~~
-A SigrokDevice resource describes a sigrok device. To select a specific device
-from all connected supported devices use the `SigrokUSBDevice`_.
+A :any:`SigrokDevice` resource describes a *Sigrok* device. To select a
+specific device from all connected supported devices use the
+`SigrokUSBDevice`_.
 
 .. code-block:: yaml
 
    SigrokDevice:
-     driver: fx2lafw
-     channels: "D0=CLK,D1=DATA"
+     driver: 'fx2lafw'
+     channels: 'D0=CLK,D1=DATA'
 
 Arguments:
   - driver (str): name of the sigrok driver to use
   - channels (str): optional, channel mapping as described in the sigrok-cli
     man page
 
 Used by:
   - `SigrokDriver`_
 
 IMXUSBLoader
 ~~~~~~~~~~~~
-An IMXUSBLoader resource describes a USB device in the imx loader state.
+An :any:`IMXUSBLoader` resource describes a USB device in the imx loader state.
 
 .. code-block:: yaml
 
    IMXUSBLoader:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `IMXUSBDriver`_
   - `UUUDriver`_
+  - `BDIMXUSBDriver`_
 
 MXSUSBLoader
 ~~~~~~~~~~~~
-An MXSUSBLoader resource describes a USB device in the mxs loader state.
+An :any:`MXSUSBLoader` resource describes a USB device in the *MXS loader
+state*.
 
 .. code-block:: yaml
 
    MXSUSBLoader:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `MXSUSBDriver`_
+  - `IMXUSBDriver`_
   - `UUUDriver`_
 
 RKUSBLoader
-~~~~~~~~~~~~
-An RKUSBLoader resource describes a USB device in the rockchip loader state.
+~~~~~~~~~~~
+An :any:`RKUSBLoader` resource describes a USB device in the *Rockchip loader
+state*.
 
 .. code-block:: yaml
 
    RKUSBLoader:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `RKUSBDriver`_
 
 NetworkMXSUSBLoader
 ~~~~~~~~~~~~~~~~~~~
-A NetworkMXSUSBLoader describes an `MXSUSBLoader`_ available on a remote computer.
+A :any:`NetworkMXSUSBLoader` describes an `MXSUSBLoader`_ available on a remote
+computer.
 
 NetworkIMXUSBLoader
 ~~~~~~~~~~~~~~~~~~~
-A NetworkIMXUSBLoader describes an `IMXUSBLoader`_ available on a remote computer.
+A :any:`NetworkIMXUSBLoader` describes an `IMXUSBLoader`_ available on a remote
+computer.
 
 NetworkRKUSBLoader
-~~~~~~~~~~~~~~~~~~~
-A NetworkRKUSBLoader describes an `RKUSBLoader`_ available on a remote computer.
+~~~~~~~~~~~~~~~~~~
+A :any:`NetworkRKUSBLoader` describes an `RKUSBLoader`_ available on a remote
+computer.
 
 AndroidUSBFastboot
 ~~~~~~~~~~~~~~~~~~
-An AndroidUSBFastboot resource describes a USB device in the fastboot state.
+An :any:`AndroidUSBFastboot` resource describes a USB device in the *Fastboot
+state*.
 Previously, this resource was named AndroidFastboot and this name still
 supported for backwards compatibility.
 
 .. code-block:: yaml
 
    AndroidUSBFastboot:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - usb_vendor_id (str, default="1d6b"): USB vendor ID to be compared with the
     ``ID_VENDOR_ID`` udev property
   - usb_product_id (str, default="0104"): USB product ID, to be compared with
     the ``ID_MODEL_ID`` udev property
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `AndroidFastbootDriver`_
 
 AndroidNetFastboot
 ~~~~~~~~~~~~~~~~~~
-An AndroidNetFastboot resource describes a network device in fastboot state.
+An :any:`AndroidNetFastboot` resource describes a network device in *Fastboot
+state*.
 
 .. code-block:: yaml
 
    AndroidNetFastboot:
-     address: "192.168.23.42"
+     address: '192.168.23.42'
 
 Arguments:
   - address (str): ip address of the fastboot device
   - port (int, default=5554): udp/tcp fastboot port that is used in the
     device. (e.g. Barebox uses port 5554)
   - protocol (str, default="udp"): which protocol should be used when issuing
     fastboot commands. (Barebox supports currently only the udp protocol)
 
 Used by:
   - `AndroidFastbootDriver`_
 
 DFUDevice
 ~~~~~~~~~
-A DFUDevice resource describes a USB device in DFU (Device Firmware Upgrade)
-mode.
+A :any:`DFUDevice` resource describes a USB device in DFU (Device Firmware
+Upgrade) mode.
 
 .. code-block:: yaml
 
    DFUDevice:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `DFUDriver`_
 
 NetworkInterface
 ~~~~~~~~~~~~~~~~
-A NetworkInterface resource describes a network adapter (such as Ethernet or
-WiFi)
+A :any:`NetworkInterface` resource describes a network adapter (such as
+Ethernet or WiFi)
 
 .. code-block:: yaml
 
    NetworkInterface:
-     ifname: eth0
+     ifname: 'eth0'
 
 Arguments:
   - ifname (str): name of the interface
 
+Used by:
+  - `NetworkInterfaceDriver`_
+  - `RawNetworkInterfaceDriver`_
+
 USBNetworkInterface
-~~~~~~~~~~~~~~~~~~~~
-A USBNetworkInterface resource describes a USB network adapter (such as
+~~~~~~~~~~~~~~~~~~~
+A :any:`USBNetworkInterface` resource describes a USB network adapter (such as
 Ethernet or WiFi)
 
 .. code-block:: yaml
 
    USBNetworkInterface:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
+Used by:
+  - `NetworkInterfaceDriver`_
+  - `RawNetworkInterfaceDriver`_
+
 RemoteNetworkInterface
 ~~~~~~~~~~~~~~~~~~~~~~
-A :any:`RemoteNetworkInterface` resource describes a :any:`NetworkInterface` or
-:any:`USBNetworkInterface` resource available on a remote computer.
+A :any:`RemoteNetworkInterface` resource describes a `NetworkInterface`_ or
+`USBNetworkInterface`_ resource available on a remote computer.
 
 AlteraUSBBlaster
 ~~~~~~~~~~~~~~~~
-An AlteraUSBBlaster resource describes an Altera USB blaster.
+An :any:`AlteraUSBBlaster` resource describes an Altera USB blaster.
 
 .. code-block:: yaml
 
    AlteraUSBBlaster:
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `OpenOCDDriver`_
   - `QuartusHPSDriver`_
 
 USBDebugger
 ~~~~~~~~~~~
-An USBDebugger resource describes a JTAG USB adapter (for example an FTDI
-FT2232H).
+A :any:`USBDebugger` resource describes a JTAG USB adapter (for example an
+*FTDI FT2232H*).
 
 .. code-block:: yaml
 
    USBDebugger:
      match:
-       ID_PATH: pci-0000:00:10.0-usb-0:1.4
+       ID_PATH: 'pci-0000:00:10.0-usb-0:1.4'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `OpenOCDDriver`_
 
 SNMPEthernetPort
 ~~~~~~~~~~~~~~~~
-A SNMPEthernetPort resource describes a port on an Ethernet switch, which is
-accessible via SNMP.
+A :any:`SNMPEthernetPort` resource describes a port on an Ethernet switch,
+which is accessible via SNMP.
 
 .. code-block:: yaml
 
    SNMPEthernetPort:
-     switch: "switch-012"
-     interface: "17"
+     switch: 'switch-012'
+     interface: '17'
 
 Arguments:
   - switch (str): host name of the Ethernet switch
   - interface (str): interface name
 
+Used by:
+  - None
+
 SigrokUSBDevice
 ~~~~~~~~~~~~~~~
-A SigrokUSBDevice resource describes a sigrok USB device.
+A :any:`SigrokUSBDevice` resource describes a *Sigrok* USB device.
 
 .. code-block:: yaml
 
    SigrokUSBDevice:
-     driver: fx2lafw
-     channels: "D0=CLK,D1=DATA"
+     driver: 'fx2lafw'
+     channels: 'D0=CLK,D1=DATA'
      match:
-       ID_PATH: pci-0000:06:00.0-usb-0:1.3.2:1.0
+       ID_PATH: 'pci-0000:06:00.0-usb-0:1.3.2:1.0'
 
 Arguments:
   - driver (str): name of the sigrok driver to use
   - channels (str): optional, channel mapping as described in the sigrok-cli
     man page
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `SigrokDriver`_
 
 NetworkSigrokUSBDevice
 ~~~~~~~~~~~~~~~~~~~~~~
-A NetworkSigrokUSBDevice resource describes a sigrok USB device connected to a
-host which is exported over the network. The SigrokDriver will access it via SSH.
+A :any:`NetworkSigrokUSBDevice` resource describes a *Sigrok* USB device
+connected to a host which is exported over the network.
+The `SigrokDriver`_ will access it via SSH.
 
 SigrokUSBSerialDevice
 ~~~~~~~~~~~~~~~~~~~~~
-A SigrokUSBSerialDevice resource describes a sigrok device which communicates
-of a USB serial port instead of being a USB device itself (see
-`SigrokUSBDevice` for that case).
+A :any:`SigrokUSBSerialDevice` resource describes a *Sigrok* device which
+communicates over a USB serial port instead of being a USB device itself (see
+`SigrokUSBDevice`_ for that case).
 
 .. code-block:: yaml
 
    SigrokUSBSerialDevice:
-     driver: manson-hcs-3xxx
+     driver: 'manson-hcs-3xxx'
      match:
-       '@ID_SERIAL_SHORT': P-00-02389
+       '@ID_SERIAL_SHORT': 'P-00-02389'
 
 Arguments:
   - driver (str): name of the sigrok driver to use
-  - channels (str): optional, channel mapping as described in the sigrok-cli
-    man page
+  - channels (str): optional, channel mapping as described in the
+    ``sigrok-cli`` man page
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `SigrokPowerDriver`_
+  - `SigrokDmmDriver`_
 
 USBSDMuxDevice
 ~~~~~~~~~~~~~~
 A :any:`USBSDMuxDevice` resource describes a Pengutronix
 `USB-SD-Mux <https://www.pengutronix.de/de/2017-10-23-usb-sd-mux-automated-sd-card-juggler.html>`_
 device.
 
 .. code-block:: yaml
 
    USBSDMuxDevice:
      match:
-       '@ID_PATH': pci-0000:00:14.0-usb-0:1.2
+       '@ID_PATH': 'pci-0000:00:14.0-usb-0:1.2'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
-  - `USBSDMUXDriver`_
+  - `USBSDMuxDriver`_
+  - `USBStorageDriver`_
 
 NetworkUSBSDMuxDevice
 ~~~~~~~~~~~~~~~~~~~~~
-
 A :any:`NetworkUSBSDMuxDevice` resource describes a `USBSDMuxDevice`_ available
 on a remote computer.
 
 LXAUSBMux
 ~~~~~~~~~
-A :any:`LXAUSBMux` resource describes a Linux Automation GmbH USB-Mux device.
+An :any:`LXAUSBMux` resource describes a *Linux Automation GmbH USB-Mux* device.
 
 .. code-block:: yaml
 
    LXAUSBMux:
      match:
-       '@ID_PATH': pci-0000:00:14.0-usb-0:1.2
+       '@ID_PATH': 'pci-0000:00:14.0-usb-0:1.2'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `LXAUSBMuxDriver`_
 
 NetworkLXAUSBMux
 ~~~~~~~~~~~~~~~~
-
-A :any:`NetworkLXAUSBMux` resource describes a `LXAUSBMux`_ available on a
+A :any:`NetworkLXAUSBMux` resource describes an `LXAUSBMux`_ available on a
 remote computer.
 
 USBSDWireDevice
 ~~~~~~~~~~~~~~~
 A :any:`USBSDWireDevice` resource describes a Tizen
-`SD Wire device <https://wiki.tizen.org/SDWire>`_
-device.
+`SD Wire device <https://wiki.tizen.org/SDWire>`_.
 
 .. code-block:: yaml
 
    USBSDWireDevice:
      match:
-       '@ID_PATH': pci-0000:00:14.0-usb-0:1.2
+       '@ID_PATH': 'pci-0000:00:14.0-usb-0:1.2'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `USBSDWireDriver`_
+  - `USBStorageDriver`_
 
 NetworkUSBSDWireDevice
 ~~~~~~~~~~~~~~~~~~~~~~
-
 A :any:`NetworkUSBSDWireDevice` resource describes a `USBSDWireDevice`_ available
 on a remote computer.
 
 USBVideo
 ~~~~~~~~
-
 A :any:`USBVideo` resource describes a USB video camera which is supported by a
-Video4Linux2 kernel driver.
+Video4Linux2 (v4l2) kernel driver.
 
 .. code-block:: yaml
 
    USBVideo:
      match:
-       '@ID_PATH': pci-0000:00:14.0-usb-0:1.2
+       '@ID_PATH': 'pci-0000:00:14.0-usb-0:1.2'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `USBVideoDriver`_
 
-SysfsGPIO
-~~~~~~~~~
-
-A :any:`SysfsGPIO` resource describes a GPIO line.
-
-.. code-block:: yaml
-
-   SysfsGPIO:
-     index: 12
-
-Arguments:
-  - index (int): index of the GPIO line
-
-Used by:
-  - `GpioDigitalOutputDriver`_
-
 NetworkUSBVideo
 ~~~~~~~~~~~~~~~
-
-A :any:`NetworkUSBVideo` resource describes a :any:`USBVideo` resource available
+A :any:`NetworkUSBVideo` resource describes a `USBVideo`_ resource available
 on a remote computer.
 
 USBAudioInput
 ~~~~~~~~~~~~~
-
 A :any:`USBAudioInput` resource describes a USB audio input which is supported
 by an ALSA kernel driver.
 
 .. code-block:: yaml
 
    USBAudioInput:
      match:
-       ID_PATH: pci-0000:00:14.0-usb-0:3:1.0
+       ID_PATH: 'pci-0000:00:14.0-usb-0:3:1.0'
 
 Arguments:
   - index (int, default=0): ALSA PCM device number (as in
-    `hw:CARD=<card>,DEV=<index>`)
+    ``hw:CARD=<card>,DEV=<index>``)
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `USBAudioInputDriver`_
 
 NetworkUSBAudioInput
 ~~~~~~~~~~~~~~~~~~~~
-
-A :any:`NetworkUSBAudioInput` resource describes a :any:`USBAudioInput` resource
+A :any:`NetworkUSBAudioInput` resource describes a `USBAudioInput`_ resource
 available on a remote computer.
 
 USBTMC
 ~~~~~~
-
-A :any:`USBTMC` resource describes an oscilloscope connected via the USB TMC
-protocol.
-The low-level communication is handled by the ``usbtmc`` kernel driver.
+A :any:`USBTMC` resource describes an oscilloscope connected via the *USB TMC
+protocol*.
+The low-level communication is handled by the "usbtmc" kernel driver.
 
 
 .. code-block:: yaml
 
    USBTMC:
      match:
-       '@ID_PATH': pci-0000:00:14.0-usb-0:1.2
+       '@ID_PATH': 'pci-0000:00:14.0-usb-0:1.2'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 A udev rules file may be needed to allow access for non-root users:
 
 .. code-block:: none
@@ -966,273 +1060,344 @@
    DRIVERS=="usbtmc", MODE="0660", GROUP="plugdev"
 
 Used by:
   - `USBTMCDriver`_
 
 NetworkUSBTMC
 ~~~~~~~~~~~~~
-
-A :any:`NetworkUSBTMC` resource describes a :any:`USBTMC` resource available
+A :any:`NetworkUSBTMC` resource describes a `USBTMC`_ resource available
 on a remote computer.
 
 Flashrom
 ~~~~~~~~
-A Flashrom resource is used to configure the parameters to a local installed flashrom instance.
-It is assumed that flashrom is installed on the host and the executable is configured in:
+A :any:`Flashrom` resource is used to configure the parameters to a local
+installed flashrom instance.
+It is assumed that flashrom is installed on the host and the executable is
+configured in:
 
 .. code-block:: yaml
 
   tools:
     flashrom: '/usr/sbin/flashrom'
 
 Arguments:
-  - programmer (str): programmer device as described in `-p, --programmer` in
-    `man 8 flashrom`
+  - programmer (str): programmer device as described in ``-p, --programmer`` in
+    ``man 8 flashrom``
 
-The resource must configure which programmer to use and the parameters to the programmer.
-The programmer parameter is passed directly to the flashrom bin hence man(8) flashrom
-can be used for reference.
+The resource must configure which programmer to use and the parameters to the
+programmer.
+The programmer parameter is passed directly to the flashrom bin hence
+``man 8 flashrom`` can be used for reference.
 Below an example where the local spidev is used.
 
 .. code-block:: yaml
 
   Flashrom:
     programmer: 'linux_spi:dev=/dev/spidev0.1,spispeed=30000'
 
 Used by:
   - `FlashromDriver`_
 
-NetworkFlashRom
+NetworkFlashrom
 ~~~~~~~~~~~~~~~
-A NetworkFlashrom describes a `Flashrom`_ available on a remote computer.
+A :any:`NetworkFlashrom` describes a `Flashrom`_ available on a remote computer.
 
 USBFlashableDevice
 ~~~~~~~~~~~~~~~~~~
-Represents an "opaque" USB device used by custom flashing programs. There is
-usually not anything useful that can be done with the interface other than
-running a flashing program with `FlashScriptDriver`_.
+A :any:`USBFlashableDevice` represents an "opaque" USB device used by custom
+flashing programs.
+There is usually not anything useful that can be done with the interface other
+than running a flashing program with `FlashScriptDriver`_.
 
 .. note::
    This resource is only intended to be used as a last resort when it is
    impossible or impractical to use a different resource
 
 .. code-block:: yaml
 
    USBFlashableDevice:
      match:
-       SUBSYSTEM: usb
+       SUBSYSTEM: 'usb'
        ID_SERIAL: '1234'
 
 Arguments:
   - match (dict): key and value pairs for a udev match, see `udev Matching`_
 
 Used by:
   - `FlashScriptDriver`_
 
 NetworkUSBFlashableDevice
 ~~~~~~~~~~~~~~~~~~~~~~~~~
-A :any:`NetworkUSBFlashableDevice` resource describes a :any:`USBFlashableDevice`
+A :any:`NetworkUSBFlashableDevice` resource describes a `USBFlashableDevice`_
 resource available on a remote computer
 
-Used by:
-  - `FlashScriptDriver`_
 
 DediprogFlasher
 ~~~~~~~~~~~~~~~
-A DediprogFlasher resource is used to configure the parameters to a locally installed
-dpmcd instance. It is assumed that dpcmd is installed on the host and the
-executable can be configured via:
+A :any:`DediprogFlasher` resource is used to configure the parameters to a
+locally installed dpmcd instance.
+It is assumed that dpcmd is installed on the host and the executable can be
+configured via:
 
 .. code-block:: yaml
 
   tools:
     dpcmd: '/usr/sbin/dpcmd'
 
 Arguments:
-  - vcc (str): '3.5V', '2.5V' or '1.8V'.
+  - vcc (str): ``3.5V``, ``2.5V`` or ``1.8V``.
 
-For instance, to flash using 3.5V vcc:
+For instance, to flash using 3.5 V VCC:
 
 .. code-block:: yaml
 
   DediprogFlasher:
     vcc: '3.5V'
 
-
 Used by:
   - `DediprogFlashDriver`_
 
 NetworkDediprogFlasher
 ~~~~~~~~~~~~~~~~~~~~~~
-A NetworkDediprogFlasher describes a `DediprogFlasher`_ available on a remote computer.
+A :any:`NetworkDediprogFlasher` describes a `DediprogFlasher`_ available on a
+remote computer.
 
 XenaManager
 ~~~~~~~~~~~
-A XenaManager resource describes a Xena Manager instance which is the instance the
-`XenaDriver`_ must connect to in order to configure a Xena chassis.
+A :any:`XenaManager` resource describes a *Xena Manager* instance which is the
+instance the `XenaDriver`_ must connect to in order to configure a Xena
+chassis.
 
 .. code-block:: yaml
 
    XenaManager:
-     hostname: "example.computer"
+     hostname: 'example.computer'
 
 Arguments:
   - hostname (str): hostname or IP of the management address of the Xena tester
 
 Used by:
   - `XenaDriver`_
 
 PyVISADevice
 ~~~~~~~~~~~~
-A PyVISADevice resource describes a test stimuli device controlled by PyVISA.
+A :any:`PyVISADevice` resource describes a test stimuli device controlled by
+PyVISA.
 Such device could be a signal generator.
 
 .. code-block:: yaml
 
    PyVISADevice:
-     type: "TCPIP"
-     url: "192.168.110.11"
+     type: 'TCPIP'
+     url: '192.168.110.11'
 
 Arguments:
-  - type (str): device resource type following the pyVISA resource syntax, e.g.
+  - type (str): device resource type following the PyVISA resource syntax, e.g.
     ASRL, TCPIP...
   - url (str): device identifier on selected resource, e.g. <ip> for TCPIP
     resource
+  - backend (str): Visa library backend, e.g. '@sim' for pyvisa-sim backend
 
 Used by:
   - `PyVISADriver`_
 
 HTTPVideoStream
 ~~~~~~~~~~~~~~~
-
-A :any:`HTTPVideoStream` resource describes a IP video stream over HTTP or HTTPS.
+An :any:`HTTPVideoStream` resource describes an IP video stream over HTTP or HTTPS.
 
 .. code-block:: yaml
 
    HTTPVideoStream:
-     url: http://192.168.110.11/0.ts
+     url: 'http://192.168.110.11/0.ts'
 
 Arguments:
   - url (str): URI of the IP video stream
 
 Used by:
   - `HTTPVideoDriver`_
 
 Providers
 ~~~~~~~~~
 Providers describe directories that are accessible by the target over a
 specific protocol.
 This is useful for software installation in the bootloader (via TFTP) or
 downloading update artifacts under Linux (via HTTP).
 
-They are used with the ManagedFile helper, which ensures that the file is
-available on the server and then creates a symlink from the internal directory
-to the uploaded file.
+They are used with the :any:`ManagedFile` helper, which ensures that the file
+is available on the server. For HTTP and TFTP, a symlink from the internal
+directory to the uploaded file is created.
 The path for the target is generated by replacing the internal prefix with the
 external prefix.
+For NFS, it is assumed that ``/var/cache/labgrid`` is exported.
+The information required for mounting and accessing staged files are returned,
+see below.
 
 For now, the TFTP/NFS/HTTP server needs to be configured before using it from
 labgrid.
 
-.. _TFTPProvider:
-.. _NFSProvider:
-.. _HTTPProvider:
-
-TFTPProvider / NFSProvider / HTTPProvider
-+++++++++++++++++++++++++++++++++++++++++
+TFTPProvider
+++++++++++++
+A :any:`TFTPProvider` resource describes a TFTP server.
 
 .. code-block:: yaml
 
    TFTPProvider:
-     internal: "/srv/tftp/board-23/"
-     external: "board-23/"
+     internal: '/srv/tftp/board-23/'
+     external: 'board-23/'
+
+Arguments:
+  - internal (str): path prefix to the local directory accessible by the target
+  - external (str): corresponding path prefix for use by the target
+
+Used by:
+  - `TFTPProviderDriver`_
+
+HTTPProvider
+++++++++++++
+An :any:`HTTPProvider` resource describes an HTTP server.
+
+.. code-block:: yaml
 
    HTTPProvider:
-     internal: "/srv/www/board-23/"
-     external: "http://192.168.1.1/board-23/"
+     internal: '/srv/www/board-23/'
+     external: 'http://192.168.1.1/board-23/'
 
 Arguments:
   - internal (str): path prefix to the local directory accessible by the target
   - external (str): corresponding path prefix for use by the target
 
 Used by:
-  - `TFTPProviderDriver`_
-  - `NFSProviderDriver`_
   - `HTTPProviderDriver`_
 
-.. _RemoteTFTPProvider:
-.. _RemoteNFSProvider:
-.. _RemoteHTTPProvider:
-
-RemoteTFTPProvider / RemoteNFSProvider / RemoteHTTPProvider
-+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-These describe a `TFTPProvider`_, `NFSProvider`_ or `HTTPProvider`_ resource
-available on a remote computer
+NFSProvider
++++++++++++
+An :any:`NFSProvider` resource describes an NFS server.
+
+.. code-block:: yaml
+
+   NFSProvider: {}
+
+Arguments:
+  - None
+
+Used by:
+  - `NFSProviderDriver`_
+
+RemoteTFTPProvider
+++++++++++++++++++
+A :any:`RemoteTFTPProvider` describes a `TFTPProvider`_ resource available on
+a remote computer.
+
+.. code-block:: yaml
+
+   RemoteTFTPProvider
+     host: 'tftphost'
+     internal: '/srv/tftp/board-23/'
+     external: 'board-23/'
+
+Arguments:
+  - host (str): hostname of the remote host
+  - internal (str): path prefix to the TFTP root directory on ``host``
+  - external (str): corresponding path prefix for use by the target
 
 Used by:
   - `TFTPProviderDriver`_
-  - `NFSProviderDriver`_
+
+RemoteHTTPProvider
+++++++++++++++++++
+A :any:`RemoteHTTPProvider` describes an `HTTPProvider`_ resource available on
+a remote computer.
+
+.. code-block:: yaml
+
+   RemoteHTTPProvider:
+     host: 'httphost'
+     internal: '/srv/www/board-23/'
+     external: 'http://192.168.1.1/board-23/'
+
+Arguments:
+  - host (str): hostname of the remote host
+  - internal (str): path prefix to the HTTP root directory on ``host``
+  - external (str): corresponding path prefix for use by the target
+
+Used by:
   - `HTTPProviderDriver`_
 
+RemoteNFSProvider
++++++++++++++++++
+A :any:`RemoteNFSProvider` describes an `NFSProvider`_ resource available on a
+remote computer.
+
+.. code-block:: yaml
+
+   RemoteNFSProvider:
+     host: 'nfshost'
+
+Arguments:
+  - host (str): hostname of the remote host
+
+Used by:
+  - `NFSProviderDriver`_
+
 RemotePlace
 ~~~~~~~~~~~
-A RemotePlace describes a set of resources attached to a labgrid remote place.
+A :any:`RemotePlace` describes a set of resources attached to a labgrid remote
+place.
 
 .. code-block:: yaml
 
    RemotePlace:
-     name: example-place
+     name: 'example-place'
 
-The example describes the remote place `example-place`. It will connect to the
+The example describes the remote place ``example-place``. It will connect to the
 labgrid remote coordinator, wait until the resources become available and expose
 them to the internal environment.
 
 Arguments:
   - name (str): name or pattern of the remote place
 
 Used by:
   - potentially all drivers
 
 DockerDaemon
 ~~~~~~~~~~~~
-A DockerDaemon describes where to contact a docker daemon process.
-DockerDaemon also participates in managing `NetworkService` instances
+A :any:`DockerDaemon` describes where to contact a *docker daemon* process.
+DockerDaemon also participates in managing `NetworkService`_ instances
 created through interaction with that daemon.
 
 .. code-block:: yaml
 
    DockerDaemon:
-     docker_daemon_url: unix://var/run/docker.sock
+     docker_daemon_url: 'unix://var/run/docker.sock'
 
 The example describes a docker daemon accessible via the
-'/var/run/docker.sock' unix socket. When used by a `DockerDriver`, the
-`DockerDriver` will first create a docker container which the
+``/var/run/docker.sock`` unix socket. When used by a `DockerDriver`_, the
+`DockerDriver`_ will first create a docker container which the
 DockerDaemon resource will subsequently use to create one/more
-`NetworkService` instances - as specified by `DockerDriver` configuration.
-Each `NetworkService` instance corresponds to a network service running inside
+`NetworkService`_ instances - as specified by `DockerDriver`_ configuration.
+Each `NetworkService`_ instance corresponds to a network service running inside
 the container.
 
 Moreover, DockerDaemon will remove any hanging containers if
 DockerDaemon is used several times in a row - as is the case when
-executing test suites. Normally `DockerDriver` - when deactivated -
+executing test suites. Normally `DockerDriver`_ - when deactivated -
 cleans up the created docker container; programming errors, keyboard
 interrupts or unix kill signals may lead to hanging containers, however;
 therefore auto-cleanup is important.
 
 Arguments:
   - docker_daemon_url (str): The url of the daemon to use for this target
 
 Used by:
   - `DockerDriver`_
 
 .. _udev-matching:
 
 udev Matching
 ~~~~~~~~~~~~~
-
 labgrid allows the exporter (or the client-side environment) to match resources
 via udev rules.
 Any udev property key and value can be used, path matching USB devices is
 allowed as well.
 The udev resources become available as soon as they are plugged into the
 computer running the exporter.
 
@@ -1280,49 +1445,46 @@
   SUBSYSTEMS=="usb", IMPORT{builtin}="path_id"
 
 The following examples show how to use the udev matches for some common
 use-cases.
 
 Matching a USB Serial Converter on a Hub Port
 +++++++++++++++++++++++++++++++++++++++++++++
-
 This will match any USB serial converter connected below the hub port 1.2.5.5
 on bus 1.
-The `ID_PATH` value corresponds to the hierarchy of buses and ports as shown
+The ``ID_PATH`` value corresponds to the hierarchy of buses and ports as shown
 with ``udevadm info /dev/ttyUSB0``.
 
 .. code-block:: yaml
 
   USBSerialPort:
     match:
-      '@ID_PATH': pci-0000:05:00.0-usb-0:1.2.5.5
+      '@ID_PATH': 'pci-0000:05:00.0-usb-0:1.2.5.5'
 
 Note the ``@`` in the ``@ID_PATH`` match, which applies this match to the
 device's parents instead of directly to itself.
-This is necessary for the `USBSerialPort` because we actually want to find the
+This is necessary for the `USBSerialPort`_ because we actually want to find the
 ``ttyUSB?`` device below the USB serial converter device.
 
 Matching an Android USB Fastboot Device
 +++++++++++++++++++++++++++++++++++++++
-
 In this case, we want to match the USB device on that port directly, so we
 don't use a parent match.
 
 .. code-block:: yaml
 
   AndroidUSBFastboot:
     match:
-      ID_PATH: pci-0000:05:00.0-usb-0:1.2.3
+      ID_PATH: 'pci-0000:05:00.0-usb-0:1.2.3'
 
 Matching a Specific UART in a Dual-Port Adapter
 +++++++++++++++++++++++++++++++++++++++++++++++
-
 On this board, the serial console is connected to the second port of an
 on-board dual-port USB-UART.
-The board itself is connected to the bus 3 and port path 10.2.2.2.
+The board itself is connected to the bus 3 and port path ``10.2.2.2``.
 The correct value can be shown by running ``udevadm info /dev/ttyUSB9`` in our
 case:
 
 .. code-block:: bash
   :emphasize-lines: 21
 
   $ udevadm info /dev/ttyUSB9
@@ -1358,30 +1520,29 @@
 
 We use the ``ID_USB_INTERFACE_NUM`` to distinguish between the two ports:
 
 .. code-block:: yaml
 
   USBSerialPort:
     match:
-      '@ID_PATH': pci-0000:05:00.0-usb-2:10.2.2.2'
+      '@ID_PATH': 'pci-0000:05:00.0-usb-2:10.2.2.2'
       ID_USB_INTERFACE_NUM: '01'
 
 Matching a USB UART by Serial Number
 ++++++++++++++++++++++++++++++++++++
-
 Most of the USB serial converters in our lab have been programmed with unique
 serial numbers.
 This makes it easy to always match the same one even if the USB topology
 changes or a board has been moved between host systems.
 
 .. code-block:: yaml
 
   USBSerialPort:
     match:
-      ID_SERIAL_SHORT: P-00-03564
+      ID_SERIAL_SHORT: 'P-00-03564'
 
 To check if your device has a serial number, you can use ``udevadm info``:
 
 .. code-block:: bash
 
   $ udevadm info /dev/ttyUSB5 | grep SERIAL_SHORT
   E: ID_SERIAL_SHORT=P-00-03564
@@ -1412,73 +1573,88 @@
   Unloaded link configuration context.
 
 Drivers
 -------
 
 SerialDriver
 ~~~~~~~~~~~~
-A SerialDriver connects to a serial port. It requires one of the serial port
-resources.
+A :any:`SerialDriver` connects to a serial port. It requires one of the serial
+port resources.
 
 Binds to:
   port:
     - `NetworkSerialPort`_
     - `RawSerialPort`_
     - `USBSerialPort`_
 
 .. code-block:: yaml
 
    SerialDriver:
      txdelay: 0.05
 
 Implements:
   - :any:`ConsoleProtocol`
+  - :any:`ResetProtocol`
 
 Arguments:
   - txdelay (float, default=0.0): time in seconds to wait before sending each byte
   - timeout (float, default=3.0): time in seconds to wait for a network serial port before
     an error occurs
 
 ModbusRTUDriver
 ~~~~~~~~~~~~~~~
-A ModbusRTUDriver connects to a ModbusRTU resource. This driver only supports
-local usage and will not work with an exporter.
+A :any:`ModbusRTUDriver` connects to a ModbusRTU resource. This driver only
+supports local usage and will not work with an exporter.
+
+The driver is implemented using the
+`minimalmodbus <https://minimalmodbus.readthedocs.io/en/stable/>`_ Python
+library.
+The implementation only supports that labgrid will be the master on the Modbus
+network.
 
 .. code-block:: yaml
 
     ModbusRTUDriver: {}
 
 Binds to:
-  port:
+  resource:
     - `ModbusRTU`_
 
+Implements:
+  - None (yet)
+
+Arguments:
+  - None
+
 ShellDriver
 ~~~~~~~~~~~
-A ShellDriver binds on top of a `ConsoleProtocol` and is designed to interact
-with a login prompt and a Linux shell.
+A :any:`ShellDriver` binds on top of a :any:`ConsoleProtocol` and is designed
+to interact with a login prompt and a Linux shell.
 
 Binds to:
   console:
     - :any:`ConsoleProtocol`
 
 Implements:
   - :any:`CommandProtocol`
+  - :any:`FileTransferProtocol`
 
 .. code-block:: yaml
 
    ShellDriver:
      prompt: 'root@\w+:[^ ]+ '
      login_prompt: ' login: '
-     username: root
+     username: 'root'
 
 Arguments:
   - prompt (regex): shell prompt to match after logging in
   - login_prompt (regex): match for the login prompt
   - username (str): username to use during login
-  - password (str): optional, password to use during login
+  - password (str): optional, password to use during login.
+    Can be an empty string.
   - keyfile (str): optional, keyfile to upload after login, making the
     `SSHDriver`_ usable
   - login_timeout (int, default=60): timeout for login prompt detection in
     seconds
   - await_login_timeout (int, default=2): time in seconds of silence that needs
     to pass before sending a newline to device.
   - console_ready (regex): optional, pattern used by the kernel to inform
@@ -1498,92 +1674,98 @@
    Add ``\x1b\[\?2004h`` at the beginning of the prompt argument to allow the
    ShellDriver to still match the prompt in this case.
 
 .. _conf-sshdriver:
 
 SSHDriver
 ~~~~~~~~~
-A SSHDriver requires a `NetworkService` resource and allows the execution of
-commands and file upload via network.
-It uses SSH's `ServerAliveInterval` option to detect failed connections.
+An :any:`SSHDriver` requires a `NetworkService`_ resource and allows the
+execution of commands and file upload via network.
+It uses SSH's ``ServerAliveInterval`` option to detect failed connections.
 
 If a shared SSH connection to the target is already open, it will reuse it when
 running commands.
-In that case, `ServerAliveInterval` should be set outside of labgrid, as it
+In that case, ``ServerAliveInterval`` should be set outside of labgrid, as it
 cannot be enabled for an existing connection.
 
 Binds to:
   networkservice:
     - `NetworkService`_
 
 Implements:
   - :any:`CommandProtocol`
   - :any:`FileTransferProtocol`
 
 .. code-block:: yaml
 
    SSHDriver:
-     keyfile: example.key
+     keyfile: 'example.key'
 
 Arguments:
   - keyfile (str): optional, filename of private key to login into the remote system
-    (has precedence over `NetworkService`'s password)
-  - stderr_merge (bool, default=False): set to True to make `run()` return stderr merged with
+    (has precedence over `NetworkService`_'s password)
+  - stderr_merge (bool, default=False): set to True to make ``run()`` return stderr merged with
     stdout, and an empty list as second element.
   - connection_timeout (float, default=30.0): timeout when trying to establish connection to
     target.
-  - explicit_sftp_mode (bool, default=False): if set to True, `put()` and `get()` will
-    explicitly use the SFTP protocol for file transfers instead of scp's default protocol
+  - explicit_sftp_mode (bool, default=False): if set to True, ``put()``, ``get()``, and ``scp()``
+    will explicitly use the SFTP protocol for file transfers instead of scp's default protocol
+  - explicit_scp_mode (bool, default=False): if set to True, ``put()``, ``get()``, and ``scp()``
+    will explicitly use the SCP protocol for file transfers instead of scp's default protocol
+  - username (str, default=username from `NetworkService`_): username used by SSH
+  - password (str, default=password from `NetworkService`_): password used by SSH
 
 UBootDriver
 ~~~~~~~~~~~
-A UBootDriver interfaces with a U-Boot bootloader via a `ConsoleProtocol`.
+A :any:`UBootDriver` interfaces with a U-Boot bootloader via a
+:any:`ConsoleProtocol`.
 
 Binds to:
   console:
     - :any:`ConsoleProtocol`
 
 Implements:
   - :any:`CommandProtocol`
+  - :any:`LinuxBootProtocol`
 
 .. code-block:: yaml
 
    UBootDriver:
      prompt: 'Uboot> '
      boot_commands:
-       net: run netboot
-       spi: run spiboot
+       net: 'run netboot'
+       spi: 'run spiboot'
 
 Arguments:
   - prompt (regex, default=""): U-Boot prompt to match
   - autoboot (regex, default="stop autoboot"): autoboot message to match
   - password (str): optional, U-Boot unlock password
-  - interrupt (str, default="\\n"): string to interrupt autoboot (use "\\x03" for CTRL-C)
+  - interrupt (str, default="\\n"): string to interrupt autoboot (use ``\\x03`` for CTRL-C)
   - init_commands (tuple): optional, tuple of commands to execute after matching the
     prompt
   - password_prompt (str, default="enter Password: "): regex to match the U-Boot password prompt
   - bootstring (str): optional, regex to match on Linux Kernel boot
   - boot_command (str, default="run bootcmd"): boot command for booting target
   - boot_commands (dict, default={}): boot commands by name for LinuxBootProtocol boot command
   - login_timeout (int, default=30): timeout for login prompt detection in seconds
   - boot_timeout (int, default=30): timeout for initial Linux Kernel version detection
 
 SmallUBootDriver
 ~~~~~~~~~~~~~~~~
-A SmallUBootDriver interfaces with stripped-down U-Boot variants that are
-sometimes used in cheap consumer electronics.
+A :any:`SmallUBootDriver` interfaces with stripped-down *U-Boot* variants that
+are sometimes used in cheap consumer electronics.
 
 SmallUBootDriver is meant as a driver for U-Boot with only little functionality
 compared to a standard U-Boot.
 Especially is copes with the following limitations:
 
 - The U-Boot does not have a real password-prompt but can be activated by
   entering a "secret" after a message was displayed.
 - The command line does not have a built-in echo command.
-  Thus this driver uses 'Unknown Command' messages as marker before and after
+  Thus this driver uses "Unknown Command" messages as marker before and after
   the output of a command.
 - Since there is no echo we cannot return the exit code of the command.
   Commands will always return 0 unless the command was not found.
 
 This driver needs the following features activated in U-Boot to work:
 
 - The U-Boot must not have a real password prompt. Instead it must be keyword
@@ -1595,43 +1777,47 @@
   - U-Boot: <switching to console>
 
 - The U-Boot must be able to parse multiple commands in a single line separated
   by ";".
 - The U-Boot must support the "bootm" command to boot from a memory location.
 
 Binds to:
-  - :any:`ConsoleProtocol` (see `SerialDriver`_)
+  console:
+    - :any:`ConsoleProtocol` (see `SerialDriver`_)
 
 Implements:
   - :any:`CommandProtocol`
+  - :any:`LinuxBootProtocol`
 
 .. code-block:: yaml
 
    SmallUBootDriver:
      prompt: 'ap143-2\.0> '
      boot_expression: 'Autobooting in 1 seconds'
-     boot_secret: "tpl"
+     boot_secret: 'tpl'
 
 Arguments:
   - boot_expression (str, default="U-Boot 20\\d+"): regex to match the U-Boot start string
   - boot_secret (str, default="a"): secret used to unlock prompt
+  - boot_secret_nolf (bool, default=False): send boot_secret without new line
   - login_timeout (int, default=60): timeout for password/login prompt detection
   - for other arguments, see `UBootDriver`_
 
 BareboxDriver
 ~~~~~~~~~~~~~
-
-A BareboxDriver interfaces with a barebox bootloader via a `ConsoleProtocol`.
+A :any:`BareboxDriver` interfaces with a *barebox* bootloader via a
+:any:`ConsoleProtocol`.
 
 Binds to:
   console:
     - :any:`ConsoleProtocol`
 
 Implements:
   - :any:`CommandProtocol`
+  - :any:`LinuxBootProtocol`
 
 .. code-block:: yaml
 
    BareboxDriver:
      prompt: 'barebox@[^:]+:[^ ]+ '
 
 Arguments:
@@ -1641,16 +1827,19 @@
   - bootstring (regex, default="Linux version \\d"): regex that indicating that the Linux Kernel is
     booting
   - password (str): optional, password to use for access to the shell
   - login_timeout (int, default=60): timeout for access to the shell
 
 ExternalConsoleDriver
 ~~~~~~~~~~~~~~~~~~~~~
-An ExternalConsoleDriver implements the `ConsoleProtocol` on top of a command
-executed on the local computer.
+An :any:`ExternalConsoleDriver` implements the :any:`ConsoleProtocol` on top of
+a command executed on the local computer.
+
+Binds to:
+  - None
 
 Implements:
   - :any:`ConsoleProtocol`
 
 .. code-block:: yaml
 
    ExternalConsoleDriver:
@@ -1659,370 +1848,414 @@
 
 Arguments:
   - cmd (str): command to execute and then bind to.
   - txdelay (float, default=0.0): time in seconds to wait before sending each byte
 
 AndroidFastbootDriver
 ~~~~~~~~~~~~~~~~~~~~~
-An AndroidFastbootDriver allows the upload of images to a device in the USB or
-network fastboot state.
+An :any:`AndroidFastbootDriver` allows the upload of images to a device in the
+USB or network *Fastboot state*.
 
 Binds to:
   fastboot:
     - `AndroidUSBFastboot`_
+    - RemoteAndroidUSBFastboot
     - `AndroidNetFastboot`_
+    - RemoteAndroidNetFastboot
 
 Implements:
   - None (yet)
 
 .. code-block:: yaml
 
    AndroidFastbootDriver:
-     boot_image: mylocal.image
-     sparse_size: 100M
+     boot_image: 'mylocal.image'
+     sparse_size: '100M'
 
 Arguments:
   - boot_image (str): optional, image key referring to the image to boot
   - flash_images (dict): optional, partition to image key mapping referring to
     images to flash to the device
   - sparse_size (str): optional, sparse files greater than given size (see
     fastboot manpage -S option for allowed size suffixes). The default is the
     same as the fastboot default, which is computed after querying the target's
     ``max-download-size`` variable.
 
 DFUDriver
 ~~~~~~~~~
-A DFUDriver allows the download of images to a device in DFU (Device Firmware
-Upgrade) mode.
+A :any:`DFUDriver` allows the download of images to a device in DFU (Device
+Firmware Upgrade) mode.
 
 Binds to:
   dfu:
     - `DFUDevice`_
+    - NetworkDFUDevice
 
 Implements:
   - None (yet)
 
 .. code-block:: yaml
 
    DFUDriver: {}
 
 Arguments:
   - None
 
 OpenOCDDriver
 ~~~~~~~~~~~~~
-An OpenOCDDriver controls OpenOCD to bootstrap a target with a bootloader.
+An :any:`OpenOCDDriver` controls *OpenOCD* to bootstrap a target with a
+bootloader.
 
 Note that OpenOCD supports specifying USB paths since
 `a1b308ab <https://sourceforge.net/p/openocd/code/ci/a1b308ab/>`_ which was released with v0.11.
 The OpenOCDDriver passes the resource's USB path.
 Depending on which OpenOCD version is installed it is either used correctly or
 a warning is displayed and the first resource seen is used, which might be the
 wrong USB device.
 Consider updating your OpenOCD version when using multiple USB Blasters.
 
 Binds to:
   interface:
     - `AlteraUSBBlaster`_
+    - NetworkAlteraUSBBlaster
     - `USBDebugger`_
+    - NetworkUSBDebugger
 
 Implements:
   - :any:`BootstrapProtocol`
 
 .. code-block:: yaml
 
    OpenOCDDriver:
-     config: local-settings.cfg
-     image: bitstream
-     interface_config: ftdi/lambdaconcept_ecpix-5.cfg
-     board_config: lambdaconcept_ecpix-5.cfg
+     config: 'local-settings.cfg'
+     image: 'bitstream'
+     interface_config: 'ftdi/lambdaconcept_ecpix-5.cfg'
+     board_config: 'lambdaconcept_ecpix-5.cfg'
      load_commands:
-     - "init"
-     - "svf -quiet {filename}"
-     - "exit"
+     - 'init'
+     - 'svf -quiet {filename}'
+     - 'exit'
 
 Arguments:
   - config (str/list): optional, OpenOCD configuration file(s)
   - search (str): optional, include search path for scripts
   - image (str): optional, name of the image to bootstrap onto the device
   - interface_config (str): optional, interface config in the ``openocd/scripts/interface/`` directory
   - board_config (str): optional, board config in the ``openocd/scripts/board/`` directory
   - load_commands (list of str): optional, load commands to use instead of ``init``, ``bootstrap {filename}``, ``shutdown``
 
 QuartusHPSDriver
 ~~~~~~~~~~~~~~~~
-A QuartusHPSDriver controls the "Quartus Prime Programmer and Tools" to flash
-a target's QSPI.
+A :any:`QuartusHPSDriver` controls the "Quartus Prime Programmer and Tools" to
+flash a target's QSPI.
 
 Binds to:
-  - `AlteraUSBBlaster`_
+  interface:
+    - `AlteraUSBBlaster`_
+    - NetworkAlteraUSBBlaster
 
 Implements:
   - None
 
 Arguments:
   - image (str): optional, filename of image to write into QSPI flash
 
-The driver can be used in test cases by calling the `flash` function. An
+The driver can be used in test cases by calling its ``flash()`` method. An
 example strategy is included in labgrid.
 
 ManualPowerDriver
 ~~~~~~~~~~~~~~~~~
-A ManualPowerDriver requires the user to control the target power states. This
-is required if a strategy is used with the target, but no automatic power
+A :any:`ManualPowerDriver` requires the user to control the target power
+states.
+This is required if a strategy is used with the target, but no automatic power
 control is available.
 
 The driver's name will be displayed during interaction.
 
+Binds to:
+  - None
+
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    ManualPowerDriver:
      name: 'example-board'
 
 Arguments:
   - None
 
 ExternalPowerDriver
 ~~~~~~~~~~~~~~~~~~~
-An ExternalPowerDriver is used to control a target power state via an external command.
+An :any:`ExternalPowerDriver` is used to control a target power state via an
+external command.
+
+Binds to:
+  - None
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    ExternalPowerDriver:
-     cmd_on: example_command on
-     cmd_off: example_command off
-     cmd_cycle: example_command cycle
+     cmd_on: 'example_command on'
+     cmd_off: 'example_command off'
+     cmd_cycle: 'example_command cycle'
 
 Arguments:
   - cmd_on (str): command to turn power to the board on
   - cmd_off (str): command to turn power to the board off
   - cmd_cycle (str): optional command to switch the board off and on
   - delay (float, default=2.0): delay in seconds between off and on, if cmd_cycle is not set
 
 NetworkPowerDriver
 ~~~~~~~~~~~~~~~~~~
-A NetworkPowerDriver controls a `NetworkPowerPort`, allowing control of the
-target power state without user interaction.
+A :any:`NetworkPowerDriver` controls a `NetworkPowerPort`_, allowing control of
+the target power state without user interaction.
 
 Binds to:
   port:
     - `NetworkPowerPort`_
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    NetworkPowerDriver:
      delay: 5.0
 
 Arguments:
   - delay (float, default=2.0): delay in seconds between off and on
 
 PDUDaemonDriver
 ~~~~~~~~~~~~~~~
-A PDUDaemonDriver controls a `PDUDaemonPort`, allowing control of the target
-power state without user interaction.
+A :any:`PDUDaemonDriver` controls a `PDUDaemonPort`_, allowing control of the
+target power state without user interaction.
 
 .. note::
   PDUDaemon processes commands in the background, so the actual state change
   may happen several seconds after calls to PDUDaemonDriver return.
 
 Binds to:
   port:
     - `PDUDaemonPort`_
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    PDUDaemonDriver:
      delay: 5.0
 
 Arguments:
   - delay (float, default=5.0): delay in seconds between off and on
 
 YKUSHPowerDriver
 ~~~~~~~~~~~~~~~~
-A YKUSHPowerDriver controls a `YKUSHPowerPort`, allowing control of the
+A :any:`YKUSHPowerDriver` controls a `YKUSHPowerPort`_, allowing control of the
 target power state without user interaction.
 
 Binds to:
   port:
     - `YKUSHPowerPort`_
+    - `NetworkYKUSHPowerPort`_
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    YKUSHPowerDriver:
      delay: 5.0
 
 Arguments:
   - delay (float, default=2.0): delay in seconds between off and on
 
 DigitalOutputPowerDriver
 ~~~~~~~~~~~~~~~~~~~~~~~~
-A DigitalOutputPowerDriver can be used to control the power of a
-device using a DigitalOutputDriver.
+A :any:`DigitalOutputPowerDriver` can be used to control the power of a device
+using a DigitalOutputDriver.
 
 Using this driver you probably want an external relay to switch the
 power of your DUT.
 
 Binds to:
   output:
     - :any:`DigitalOutputProtocol`
 
+Implements:
+  - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
+
 .. code-block:: yaml
 
    DigitalOutputPowerDriver:
      delay: 2.0
 
 Arguments:
   - delay (float, default=1.0): delay in seconds between off and on
 
 USBPowerDriver
 ~~~~~~~~~~~~~~
-A USBPowerDriver controls a `USBPowerPort`, allowing control of the target
-power state without user interaction.
+A :any:`USBPowerDriver` controls a `USBPowerPort`_, allowing control of the
+target power state without user interaction.
 
 Binds to:
-  - `USBPowerPort`_
+  hub:
+    - `USBPowerPort`_
+    - NetworkUSBPowerPort
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    USBPowerDriver:
      delay: 5.0
 
 Arguments:
   - delay (float, default=2.0): delay in seconds between off and on
 
 SiSPMPowerDriver
 ~~~~~~~~~~~~~~~~
-A SiSPMPowerDriver controls a `SiSPMPowerPort`, allowing control of the target
-power state without user interaction.
+A :any:`SiSPMPowerDriver` controls a `SiSPMPowerPort`_, allowing control of the
+target power state without user interaction.
 
 Binds to:
-  - `SiSPMPowerPort`_
+  port:
+    - `SiSPMPowerPort`_
+    - NetworkSiSPMPowerPort
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    SiSPMPowerDriver:
      delay: 5.0
 
 Arguments:
   - delay (float, default=2.0): delay in seconds between off and on
 
 TasmotaPowerDriver
 ~~~~~~~~~~~~~~~~~~
-A TasmotaPowerDriver controls a `TasmotaPowerPort`, allowing the outlet to be
-switched on and off.
+A :any:`TasmotaPowerDriver` controls a `TasmotaPowerPort`_, allowing the outlet
+to be switched on and off.
 
 Binds to:
-  - `TasmotaPowerPort`_
+  power:
+    - `TasmotaPowerPort`_
 
 Implements:
   - :any:`PowerProtocol`
 
 .. code-block:: yaml
 
    TasmotaPowerDriver:
      delay: 5.0
 
 Arguments:
   - delay (float, default=2.0): delay in seconds between off and on
 
 GpioDigitalOutputDriver
 ~~~~~~~~~~~~~~~~~~~~~~~
-The GpioDigitalOutputDriver writes a digital signal to a GPIO line.
+The :any:`GpioDigitalOutputDriver` writes a digital signal to a GPIO line.
 
 This driver configures GPIO lines via `the sysfs kernel interface <https://www.kernel.org/doc/html/latest/gpio/sysfs.html>`.
 While the driver automatically exports the GPIO, it does not configure it in any other way than as an output.
 
 Binds to:
-  - `SysfsGPIO`_
+  gpio:
+    - `SysfsGPIO`_
+    - `MatchedSysfsGPIO`_
+    - NetworkSysfsGPIO
 
 Implements:
   - :any:`DigitalOutputProtocol`
 
 .. code-block:: yaml
 
    GpioDigitalOutputDriver: {}
 
 Arguments:
   - None
 
 SerialPortDigitalOutputDriver
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The SerialPortDigitalOutputDriver makes it possible to use a UART
+The :any:`SerialPortDigitalOutputDriver` makes it possible to use a UART
 as a 1-Bit general-purpose digital output.
 
 This driver acts on top of a SerialDriver and uses the its pyserial port to
 control the flow control lines.
 
+Binds to:
+  serial:
+    - `SerialDriver`_
+
 Implements:
   - :any:`DigitalOutputProtocol`
 
 .. code-block:: yaml
 
    SerialPortDigitalOutputDriver:
-     signal: "dtr"
-     bindings: { serial : "nameOfSerial" }
+     signal: 'dtr'
+     bindings:
+       serial: 'nameOfSerial'
 
 Arguments:
   - signal (str): control signal to use: "dtr" or "rts"
   - invert (bool): whether to invert the signal
   - bindings (dict): optional, a named resource of the type SerialDriver to
     bind against. This is only needed if you have multiple
     SerialDriver in your environment (what is likely to be the case
     if you are using this driver).
 
 FileDigitalOutputDriver
 ~~~~~~~~~~~~~~~~~~~~~~~
-The FileDigitalOutputDriver uses a file
+The :any:`FileDigitalOutputDriver` uses a file
 to write arbitrary string representations of booleans
 to a file and read from it.
 
 The file is checked to exist at configuration time.
 
 If the file's content does not match any of the representations
 reading defaults to False.
 
 A prime example for using this driver is Linux's sysfs.
 
+Binds to:
+  - None
+
 Implements:
   - :any:`DigitalOutputProtocol`
 
 .. code-block:: yaml
 
    FileDigitalOutputDriver:
-     filepath: "/sys/class/leds/myled/brightness"
+     filepath: '/sys/class/leds/myled/brightness'
 
 Arguments:
   - filepath (str): file that is used for reads and writes.
   - false_repr (str, default="0\\n"): representation for False
   - true_repr (str, default="1\\n"): representation for True
 
 DigitalOutputResetDriver
 ~~~~~~~~~~~~~~~~~~~~~~~~
-A DigitalOutputResetDriver uses a DigitalOutput to reset the target.
+A :any:`DigitalOutputResetDriver` uses a DigitalOutput to reset the target.
 
 Binds to:
   output:
     - :any:`DigitalOutputProtocol`
 
 Implements:
   - :any:`ResetProtocol`
@@ -2033,15 +2266,15 @@
      delay: 2.0
 
 Arguments:
   - delay (float, default=1.0): delay in seconds between setting the output 0 and 1.
 
 ModbusCoilDriver
 ~~~~~~~~~~~~~~~~
-A ModbusCoilDriver controls a `ModbusTCPCoil` resource.
+A :any:`ModbusCoilDriver` controls a `ModbusTCPCoil`_ resource.
 It can set and get the current state of the resource.
 
 Binds to:
   coil:
     - `ModbusTCPCoil`_
 
 Implements:
@@ -2052,15 +2285,15 @@
    ModbusCoilDriver: {}
 
 Arguments:
   - None
 
 HIDRelayDriver
 ~~~~~~~~~~~~~~
-A HIDRelayDriver controls a `HIDRelay` or `NetworkHIDRelay` resource.
+An :any:`HIDRelayDriver` controls an `HIDRelay`_ or `NetworkHIDRelay`_ resource.
 It can set and get the current state of the resource.
 
 Binds to:
   relay:
     - `HIDRelay`_
     - `NetworkHIDRelay`_
 
@@ -2072,52 +2305,58 @@
    HIDRelayDriver: {}
 
 Arguments:
   - None
 
 ManualSwitchDriver
 ~~~~~~~~~~~~~~~~~~
-A ManualSwitchDriver requires the user to control a switch or jumper on the
-target. This can be used if a driver binds to a :any:`DigitalOutputProtocol`,
-but no automatic control is available.
+A :any:`ManualSwitchDriver` requires the user to control a switch or jumper on
+the target.
+This can be used if a driver binds to a :any:`DigitalOutputProtocol`, but no
+automatic control is available.
+
+Binds to:
+  - None
 
 Implements:
   - :any:`DigitalOutputProtocol`
 
 .. code-block:: yaml
 
    ManualSwitchDriver:
      description: 'Jumper 5'
 
 Arguments:
   - description (str): optional, description of the switch or jumper on the target
 
 DeditecRelaisDriver
 ~~~~~~~~~~~~~~~~~~~
-A DeditecRelaisDriver controls a Deditec relay resource.
+A :any:`DeditecRelaisDriver` controls a *Deditec* relay resource.
 It can set and get the current state of the resource.
 
 Binds to:
   relais:
     - `DeditecRelais8`_
+    - NetworkDeditecRelais8
 
 Implements:
   - :any:`DigitalOutputProtocol`
 
 .. code-block:: yaml
 
    DeditecRelaisDriver: {}
 
 Arguments:
   - None
 
 MXSUSBDriver
 ~~~~~~~~~~~~
-A MXUSBDriver is used to upload an image into a device in the mxs USB loader
-state. This is useful to bootstrap a bootloader onto a device.
+An :any:`MXSUSBDriver` is used to upload an image into a device in the *MXS USB
+loader state*.
+This is useful to bootstrap a bootloader onto a device.
 
 Binds to:
   loader:
     - `MXSUSBLoader`_
     - `NetworkMXSUSBLoader`_
 
 Implements:
@@ -2125,58 +2364,62 @@
 
 .. code-block:: yaml
 
    targets:
      main:
        drivers:
          MXSUSBDriver:
-           image: mybootloaderkey
+           image: 'mybootloaderkey'
 
    images:
-     mybootloaderkey: path/to/mybootloader.img
+     mybootloaderkey: 'path/to/mybootloader.img'
 
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to bootstrap onto the target
 
 IMXUSBDriver
 ~~~~~~~~~~~~
-A IMXUSBDriver is used to upload an image into a device in the imx USB loader
-state. This is useful to bootstrap a bootloader onto a device.
-This driver uses the imx-usb-loader tool from barebox.
+An :any:`IMXUSBDriver` is used to upload an image into a device in the *i.MX
+USB loader state*.
+This is useful to bootstrap a bootloader onto a device.
+This driver uses the ``imx-usb-loader`` tool from barebox.
 
 Binds to:
   loader:
     - `IMXUSBLoader`_
     - `NetworkIMXUSBLoader`_
+    - `MXSUSBLoader`_
+    - `NetworkMXSUSBLoader`_
 
 Implements:
   - :any:`BootstrapProtocol`
 
 .. code-block:: yaml
 
    targets:
      main:
        drivers:
          IMXUSBDriver:
-           image: mybootloaderkey
+           image: 'mybootloaderkey'
 
    images:
-     mybootloaderkey: path/to/mybootloader.img
+     mybootloaderkey: 'path/to/mybootloader.img'
 
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to bootstrap onto the target
 
 BDIMXUSBDriver
 ~~~~~~~~~~~~~~
-The BDIMXUSBDriver is used to upload bootloader images into an i.MX device in
-the USB SDP mode.
-This driver uses the imx_usb tool by Boundary Devices.
-Compared to the IMXUSBLoader, it supports two-stage upload of U-Boot images.
+The :any:`BDIMXUSBDriver` is used to upload bootloader images into an *i.MX
+device* in the *USB SDP mode*.
+This driver uses the ``imx_usb`` tool by Boundary Devices.
+Compared to the ``imx-usb-loader``, it supports two-stage upload of U-Boot
+images.
 The images paths need to be specified from code instead of in the YAML
 environment, as the correct image depends on the system state.
 
 Binds to:
   loader:
     - `IMXUSBLoader`_
     - `NetworkIMXUSBLoader`_
@@ -2191,17 +2434,18 @@
        drivers:
          BDIMXUSBDriver: {}
 
 Arguments:
   - None
 
 RKUSBDriver
-~~~~~~~~~~~~
-A RKUSBDriver is used to upload an image into a device in the rockchip USB loader
-state. This is useful to bootstrap a bootloader onto a device.
+~~~~~~~~~~~
+An :any:`RKUSBDriver` is used to upload an image into a device in the *Rockchip
+USB loader state*.
+This is useful to bootstrap a bootloader onto a device.
 
 Binds to:
   loader:
     - `RKUSBLoader`_
     - `NetworkRKUSBLoader`_
 
 Implements:
@@ -2209,31 +2453,32 @@
 
 .. code-block:: yaml
 
    targets:
      main:
        drivers:
          RKUSBDriver:
-           image: mybootloaderkey
-           usb_loader: myloaderkey
+           image: 'mybootloaderkey'
+           usb_loader: 'myloaderkey'
 
    images:
-     mybootloaderkey: path/to/mybootloader.img
-     myloaderkey: path/to/myloader.bin
+     mybootloaderkey: 'path/to/mybootloader.img'
+     myloaderkey: 'path/to/myloader.bin'
 
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to bootstrap onto the target
   - usb_loader (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of a first-stage bootloader image to write
 
 UUUDriver
 ~~~~~~~~~
-A UUUDriver is used to upload an image into a device in the NXP USB loader
-state. This is useful to bootstrap a bootloader onto a device.
+A :any:`UUUDriver` is used to upload an image into a device in the *NXP USB
+loader state*.
+This is useful to bootstrap a bootloader onto a device.
 
 Binds to:
   loader:
     - `MXSUSBLoader`_
     - `NetworkMXSUSBLoader`_
     - `IMXUSBLoader`_
     - `NetworkIMXUSBLoader`_
@@ -2243,54 +2488,59 @@
 
 .. code-block:: yaml
 
    targets:
      main:
        drivers:
          UUUDriver:
-           image: mybootloaderkey
-           cmd: spl
+           image: 'mybootloaderkey'
+           cmd: 'spl'
 
    images:
-     mybootloaderkey: path/to/mybootloader.img
+     mybootloaderkey: 'path/to/mybootloader.img'
 
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to bootstrap onto the target
-  - script (str): run built-in script with "uuu -b", called with image as arg0
+  - script (str): run built-in script with ``uuu -b``, called with image as arg0
 
 USBStorageDriver
 ~~~~~~~~~~~~~~~~
-A USBStorageDriver allows access to a USB stick or similar local or
+A :any:`USBStorageDriver` allows access to a USB stick or similar local or
 remote device.
 
 Binds to:
-  - `USBMassStorage`_
-  - `NetworkUSBMassStorage`_
+  storage:
+    - `USBMassStorage`_
+    - `NetworkUSBMassStorage`_
+    - `USBSDMuxDevice`_
+    - `NetworkUSBSDMuxDevice`_
+    - `USBSDWireDevice`_
+    - `NetworkUSBSDWireDevice`_
 
 Implements:
   - None (yet)
 
 .. code-block:: yaml
 
    USBStorageDriver:
-     image: flashimage
+     image: 'flashimage'
 
 .. code-block:: yaml
 
    images:
-     flashimage: ../images/myusb.image
+     flashimage: '../images/myusb.image'
 
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to write to the target
 
 OneWirePIODriver
 ~~~~~~~~~~~~~~~~
-A OneWirePIODriver controls a `OneWirePIO` resource.
+A :any:`OneWirePIODriver` controls a `OneWirePIO`_ resource.
 It can set and get the current state of the resource.
 
 Binds to:
   port:
     - `OneWirePIO`_
 
 Implements:
@@ -2299,75 +2549,116 @@
 .. code-block:: yaml
 
    OneWirePIODriver: {}
 
 Arguments:
   - None
 
-.. _TFTPProviderDriver:
-.. _NFSProviderDriver:
-.. _HTTPProviderDriver:
-
-TFTPProviderDriver / NFSProviderDriver / HTTPProviderDriver
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-These drivers control their corresponding Provider resources, either locally or
-remotely.
+TFTPProviderDriver
+~~~~~~~~~~~~~~~~~~
+The :any:`TFTPProviderDriver` controls its corresponding TFTP resource, either
+locally or remotely.
 
 Binds to:
   provider:
     - `TFTPProvider`_
     - `RemoteTFTPProvider`_
-    - `NFSProvider`_
-    - `RemoteNFSProvider`_
+
+Implements:
+  - None (yet)
+
+.. code-block:: yaml
+
+   TFTPProviderDriver: {}
+
+Arguments:
+  - None
+
+The driver can be used in test cases by calling its ``stage()`` method, which
+returns the path to be used by the target.
+
+HTTPProviderDriver
+~~~~~~~~~~~~~~~~~~
+The :any:`HTTPProviderDriver` controls its corresponding HTTP resource, either
+locally or remotely.
+
+Binds to:
+  provider:
     - `HTTPProvider`_
     - `RemoteHTTPProvider`_
 
+Implements:
+  - None (yet)
+
 .. code-block:: yaml
 
-   TFTPProviderDriver: {}
+   HTTPProviderDriver: {}
 
 Arguments:
   - None
 
-The driver can be used in test cases by calling the `stage()` function, which
+The driver can be used in test cases by calling its ``stage()`` method, which
 returns the path to be used by the target.
 
+NFSProviderDriver
+~~~~~~~~~~~~~~~~~
+An :any:`NFSProviderDriver` controls an `NFSProvider`_ resource.
+
+Binds to:
+  provider:
+    - `NFSProvider`_
+    - `RemoteNFSProvider`_
+
+Implements:
+  - None (yet)
+
+.. code-block:: yaml
+
+   NFSProviderDriver: {}
+
+Arguments:
+  - None
+
+The driver can be used in test cases by calling its ``stage()`` method, which
+returns an NFSFile object with ``host``, ``export`` and ``relative_file_path``
+attributes.
+
 QEMUDriver
 ~~~~~~~~~~
-The QEMUDriver allows the usage of a QEMU instance as a target. It requires
-several arguments, listed below.
+The :any:`QEMUDriver` allows the usage of a QEMU instance as a target.
+It requires several arguments, listed below.
 The kernel, flash, rootfs and dtb arguments refer to images and paths declared
 in the environment configuration.
 
 Binds to:
   - None
 
 .. code-block:: yaml
 
    QEMUDriver:
-     qemu_bin: qemu_arm
-     machine: vexpress-a9
-     cpu: cortex-a9
-     memory: 512M
-     boot_args: "root=/dev/root console=ttyAMA0,115200"
-     extra_args: ""
-     kernel: kernel
-     rootfs: rootfs
-     dtb: dtb
-     nic: user
+     qemu_bin: 'qemu_arm'
+     machine: 'vexpress-a9'
+     cpu: 'cortex-a9'
+     memory: '512M'
+     boot_args: 'root=/dev/root console=ttyAMA0,115200'
+     extra_args: ''
+     kernel: 'kernel'
+     rootfs: 'rootfs'
+     dtb: 'dtb'
+     nic: 'user'
 
 .. code-block:: yaml
 
    tools:
-     qemu_arm: /bin/qemu-system-arm
+     qemu_arm: '/bin/qemu-system-arm'
    paths:
-     rootfs: ../images/root
+     rootfs: '../images/root'
    images:
-     dtb: ../images/mydtb.dtb
-     kernel: ../images/vmlinuz
+     dtb: '../images/mydtb.dtb'
+     kernel: '../images/vmlinuz'
 
 
 Implements:
   - :any:`ConsoleProtocol`
   - :any:`PowerProtocol`
 
 Arguments:
@@ -2375,121 +2666,175 @@
   - machine (str): QEMU machine type
   - cpu (str): QEMU cpu type
   - memory (str): QEMU memory size (ends with M or G)
   - extra_args (str): extra QEMU arguments, they are passed directly to the QEMU binary
   - boot_args (str): optional, additional kernel boot argument
   - kernel (str): optional, reference to the images key for the kernel
   - disk (str): optional, reference to the images key for the disk image
+  - disk_opts (str): optional, additional QEMU disk options
   - flash (str): optional, reference to the images key for the flash image
   - rootfs (str): optional, reference to the paths key for use as the virtio-9p filesystem
   - dtb (str): optional, reference to the image key for the device tree
   - bios (str): optional, reference to the image key for the bios image
-  - display (str, default="none"): optional, display output to enable; must be one of:
+  - display (str, default="none"): display output to enable; must be one of:
+
     - none: Do not create a display device
     - fb-headless: Create a headless framebuffer device
     - egl-headless: Create a headless GPU-backed graphics card. Requires host support
+
   - nic (str): optional, configuration string to pass to QEMU to create a network interface
 
 The QEMUDriver also requires the specification of:
 
 - a tool key, this contains the path to the QEMU binary
 - an image key, the path to the kernel image and optionally the dtb key to
   specify the build device tree
 - a path key, this is the path to the rootfs
 
 SigrokDriver
 ~~~~~~~~~~~~
-The SigrokDriver uses a SigrokDevice resource to record samples and provides
+The :any:`SigrokDriver` uses a `SigrokDevice`_ resource to record samples and provides
 them during test runs.
 
 Binds to:
   sigrok:
     - `SigrokUSBDevice`_
-    - `SigrokDevice`_
     - `NetworkSigrokUSBDevice`_
+    - `SigrokDevice`_
 
 Implements:
   - None yet
 
 Arguments:
   - None
 
-The driver can be used in test cases by calling the `capture`, `stop` and
-`analyze` functions.
+The driver can be used in test cases by calling its ``capture()``, ``stop()``
+and ``analyze()`` methods.
 
 SigrokPowerDriver
 ~~~~~~~~~~~~~~~~~
-The SigrokPowerDriver uses a `SigrokUSBSerialDevice`_ resource to control a
-programmable power supply.
+The :any:`SigrokPowerDriver` uses a `SigrokUSBSerialDevice`_ resource to
+control a programmable power supply.
 
 Binds to:
   sigrok:
     - `SigrokUSBSerialDevice`_
     - NetworkSigrokUSBSerialDevice
 
 Implements:
   - :any:`PowerProtocol`
+  - :any:`ResetProtocol`
 
 .. code-block:: yaml
 
    SigrokPowerDriver:
      delay: 3.0
 
 Arguments:
   - delay (float, default=3.0): delay in seconds between off and on
   - max_voltage (float): optional, maximum allowed voltage for protection against
     accidental damage (in volts)
   - max_current (float): optional, maximum allowed current for protection against
     accidental damage (in ampere)
 
+SigrokDmmDriver
+~~~~~~~~~~~~~~~
+The :any:`SigrokDmmDriver` uses a `SigrokDevice`_ resource to record samples
+from a *digital multimeter* (DMM) and provides them during test runs.
+
+It is known to work with *Unit-T UT61B* and *UT61C* devices but should also
+work with other DMMs supported by *Sigrok*.
+
+Binds to:
+  sigrok:
+    - `SigrokUSBDevice`_
+    - `NetworkSigrokUSBDevice`_
+    - `SigrokUSBSerialDevice`_
+    - NetworkSigrokUSBSerialDevice
+
+Implements:
+  - None yet
+
+Arguments:
+  - None
+
+Sampling can be started calling ``capture(samples, timeout=None)``.
+It sets up sampling and returns immediately.
+The default timeout has been chosen to work with *Unit-T UT61B*.
+Other devices may require a different timeout setting.
+
+Samples can be obtained using ``stop()``.
+``stop()`` will block until either *sigrok* terminates or *timeout* is reached.
+This method returns a ``(unit, samples)`` tuple:
+``unit`` is the physical unit reported by the DMM;
+samples is an iterable of samples.
+
+This driver relies on buffering of the subprocess call.
+Reading a few samples will very likely work - but obtaining a lot of samples may stall.
+
 USBSDMuxDriver
 ~~~~~~~~~~~~~~
-The :any:`USBSDMuxDriver` uses a USBSDMuxDevice resource to control a
+The :any:`USBSDMuxDriver` uses a `USBSDMuxDevice`_ resource to control a
 USB-SD-Mux device via `usbsdmux <https://github.com/pengutronix/usbsdmux>`_
 tool.
 
+Binds to:
+  mux:
+    - `USBSDMuxDevice`_
+    - `NetworkUSBSDMuxDevice`_
+
 Implements:
   - None yet
 
 Arguments:
   - None
 
-The driver can be used in test cases by calling the `set_mode()` function with
-argument being `dut`, `host`, `off`, or `client`.
+The driver can be used in test cases by calling its ``set_mode()`` method with
+argument being "dut", "host", "off", or "client".
 
 LXAUSBMuxDriver
 ~~~~~~~~~~~~~~~
-The :any:`LXAUSBMuxDriver` uses a LXAUSBMux resource to control a USB-Mux
+The :any:`LXAUSBMuxDriver` uses an `LXAUSBMux`_ resource to control a USB-Mux
 device via the `usbmuxctl <https://github.com/linux-automation/usbmuxctl>`_
 tool.
 
+Binds to:
+  mux:
+    - `LXAUSBMux`_
+    - `NetworkLXAUSBMux`
+
 Implements:
   - None yet
 
 Arguments:
   - None
 
-The driver can be used in test cases by calling the `set_links()` function with
+The driver can be used in test cases by calling its ``set_links()`` method with
 a list containing one or more of "dut-device", "host-dut" and "host-device".
 Not all combinations can be configured at the same time.
 
 USBSDWireDriver
 ~~~~~~~~~~~~~~~
-The :any:`USBSDWireDriver` uses a USBSDWireDevice resource to control a
+The :any:`USBSDWireDriver` uses a `USBSDWireDevice`_ resource to control a
 USB-SD-Wire device via `sd-mux-ctrl <https://wiki.tizen.org/SD_MUX#Software>`_
 tool.
 
+Binds to:
+  mux:
+    - `USBSDWireDevice`_
+    - `NetworkUSBSDWireDevice`
+
 Implements:
   - None yet
 
 Arguments:
   - None
 
-The driver can be used in test cases by calling the `set_mode()` function with
-argument being `dut`, `host`, `off`, or `client`.
+The driver can be used in test cases by calling its ``set_mode()`` method with
+argument being "dut", "host", "off", or "client".
 
 USBVideoDriver
 ~~~~~~~~~~~~~~
 The :any:`USBVideoDriver` is used to show a video stream from a remote USB
 video camera in a local window.
 It uses the GStreamer command line utility ``gst-launch`` on both sides to
 stream the video via an SSH connection to the exporter.
@@ -2501,50 +2846,50 @@
 
 Implements:
   - :any:`VideoProtocol`
 
 Arguments:
   - None
 
-Although the driver can be used from Python code by calling the `stream()`
+Although the driver can be used from Python code by calling the ``stream()``
 method, it is currently mainly useful for the ``video`` subcommand of
 ``labgrid-client``.
 It supports the `Logitech HD Pro Webcam C920` with the USB ID 046d:082d and a
 few others.
-More cameras can be added to `get_qualities()` and `get_pipeline()` in
+More cameras can be added to ``get_qualities()`` and ``get_pipeline()`` in
 ``labgrid/driver/usbvideodriver.py``.
 Appropriate configuration parameters can be determined by using the GStreamer
 ``gst-device-monitor-1.0`` command line utility.
 
 USBAudioInputDriver
 ~~~~~~~~~~~~~~~~~~~
-The :any:`USBAudioInputDriver` is used to receive a audio stream from a local
+The :any:`USBAudioInputDriver` is used to receive an audio stream from a local
 or remote USB audio input.
 It uses the GStreamer command line utility ``gst-launch`` on the sender side to
 stream the audio to the client.
 For remote resources, this is done via an SSH connection to the exporter.
 On the receiver, it either uses ``gst-launch`` for simple playback or
 `gst-python <https://gitlab.freedesktop.org/gstreamer/gst-python>`_ for more
 complex cases (such as measuring the current volume level).
 
 Binds to:
-  video:
+  res:
     - `USBAudioInput`_
     - `NetworkUSBAudioInput`_
 
 Implements:
   - None yet
 
 Arguments:
   - None
 
 USBTMCDriver
 ~~~~~~~~~~~~
-The :any:`USBTMCDriver` is used to control a oscilloscope via the USB TMC
-protocol.
+The :any:`USBTMCDriver` is used to control an oscilloscope via the *USB TMC
+protocol*.
 
 Binds to:
   tmc:
     - `USBTMC`_
     - `NetworkUSBTMC`_
 
 Implements:
@@ -2553,28 +2898,31 @@
 Arguments:
   - None
 
 Currently, it can be used by the ``labgrid-client`` ``tmc`` subcommands to show
 (and save) a screenshot, to show per channel measurements and to execute raw
 TMC commands.
 It only supports the `Keysight DSO-X 2000` series (with the USB ID 0957:1798),
-but more devices can be added by extending `on_activate()` in
+but more devices can be added by extending ``on_activate()`` in
 ``labgrid/driver/usbtmcdriver.py`` and writing a corresponding backend in
 ``labgrid/driver/usbtmc/``.
 
 FlashromDriver
 ~~~~~~~~~~~~~~
-The :any:`FlashromDriver` is used to flash a rom, using the flashrom utility.
+The :any:`FlashromDriver` is used to flash a ROM, using the flashrom utility.
 
 .. code-block:: yaml
 
    FlashromDriver:
      image: 'foo'
+
+.. code-block:: yaml
+
    images:
-     foo: ../images/image_to_load.raw
+     foo: '../images/image_to_load.raw'
 
 Binds to:
   flashrom_resource:
     - `Flashrom`_
     - `NetworkFlashrom`_
 
 Implements:
@@ -2605,18 +2953,18 @@
      script: 'foo'
      args:
        - '{device.devnode}'
 
 .. code-block:: yaml
 
    images:
-     foo: ../images/flash_device.sh
+     foo: '../images/flash_device.sh'
 
 Binds to:
-  flashabledevice_resource:
+  device:
     - `USBFlashableDevice`_
     - `NetworkUSBFlashableDevice`_
 
 Implements:
   - None (yet)
 
 Arguments:
@@ -2644,70 +2992,76 @@
 Binds to:
   video:
     - `HTTPVideoStream`_
 
 Implements:
   - :any:`VideoProtocol`
 
-Although the driver can be used from Python code by calling the `stream()`
+Arguments:
+  - None
+
+Although the driver can be used from Python code by calling the ``stream()``
 method, it is currently mainly useful for the ``video`` subcommand of
 ``labgrid-client``.
 
-
 ========== =========================================================
 Key        Description
 ========== =========================================================
 ``device`` The :any:`Resource` bound to the driver
 ``file``   The :any:`ManagedFile` used to track the flashable script
 ========== =========================================================
 
 Properties of these keys can be selected using the Python format string syntax,
-e.g. ``{device.devnode}`` to select the device node path of
-:any:`USBFlashableDevice`
+e.g. ``{device.devnode}`` to select the device node path of a
+:any:`USBFlashableDevice`.
 
 DediprogFlashDriver
 ~~~~~~~~~~~~~~~~~~~
 The :any:`DediprogFlashDriver` is used to flash an SPI device using DediprogFlasher dpcmd.
 
 .. code-block:: yaml
 
    DediprogFlashDriver:
      image: 'foo'
    images:
-     foo: ../images/image_to_load.raw
+     foo: '../images/image_to_load.raw'
 
 Binds to:
-  DediprogFlasher_resource:
+  flasher:
     - `DediprogFlasher`_
     - `NetworkDediprogFlasher`_
 
+Implements:
+  - None (yet)
+
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to flash onto the target
 
 The DediprogFlashDriver allows using DediprogFlasher dpcmd to flash or erase SPI
-devices. It is assumed that the device flashing is an exporter wired, via
-DediprogFlasher SF100 for instance, to the device being flashed.
+devices. It is assumed that the device flashing is an exporter wired, via a
+*Dediprog SF100 SPI NOR Flash Programmer* for instance, to the device being
+flashed.
 
 XenaDriver
 ~~~~~~~~~~
-The XenaDriver allows to use Xena networking test equipment.
+The :any:`XenaDriver` allows to use Xena networking test equipment.
 Using the `xenavalkyrie` library a full API to control the tester is available.
 
 Binds to:
   xena_manager:
     - `XenaManager`_
 
 The driver is supposed to work with all Xena products from the "Valkyrie Layer 2-3 Test platform"
 Currently tested on a `XenaCompact` chassis equipped with a `1 GE test module`.
 
 DockerDriver
 ~~~~~~~~~~~~
-A DockerDriver binds to a `DockerDaemon` and is used to create and control one
-docker container.
+A :any:`DockerDriver` binds to a `DockerDaemon`_ and is used to create and
+control one docker container.
 
 | The driver uses the docker python module to interact with the docker daemon.
 | For more information on the parameters see:
 | https://docker-py.readthedocs.io/en/stable/containers.html#container-objects
 
 Binds to:
   docker_daemon:
@@ -2715,18 +3069,18 @@
 
 Implements:
   - :any:`PowerProtocol`
 
 .. code-block:: yaml
 
    DockerDriver:
-     image_uri: "rastasheep/ubuntu-sshd:16.04"
-     container_name: "ubuntu-lg-example"
-     host_config: {"network_mode":"bridge"}
-     network_services: [{"port":22,"username":"root","password":"root"}]
+     image_uri: 'rastasheep/ubuntu-sshd:16.04'
+     container_name: 'ubuntu-lg-example'
+     host_config: {'network_mode': 'bridge'}
+     network_services: [{'port': 22, 'username': 'root', 'password': 'root'}]
 
 Arguments:
   - image_uri (str): identifier of the docker image to use (may have a tag suffix)
   - command (str): command to run in the container (optional, depends on image)
   - volumes (list): list to configure volumes mounted inside the container (optional)
   - container_name (str): name of the container
   - environment (list): list of environment variables (optional)
@@ -2734,16 +3088,16 @@
   - network_services (list): dictionaries that describe individual `NetworkService`_
     instances that come alive when the container is created. The "address" argument
     which `NetworkService`_ also requires will be derived automatically upon container
     creation.
 
 LXAIOBusPIODriver
 ~~~~~~~~~~~~~~~~~
-An LXAIOBusPIODriver binds to a single `LXAIOBusPIO` to toggle and read the PIO
-states.
+An :any:`LXAIOBusPIODriver` binds to a single `LXAIOBusPIO`_ to toggle and read
+the PIO states.
 
 Binds to:
   pio:
     - `LXAIOBusPIO`_
     - `NetworkLXAIOBusPIO`_
 
 .. code-block:: yaml
@@ -2752,70 +3106,134 @@
 
 Implements:
   - :any:`DigitalOutputProtocol`
 
 Arguments:
   - None
 
+HttpDigitalOutputDriver
+~~~~~~~~~~~~~~~~~~~~~~~
+A :any:`HttpDigitalOutputDriver` binds to an `HttpDigitalOutput`_ to set and
+get a digital output state via HTTP.
+
+Binds to:
+  http:
+    - `HttpDigitalOutput`_
+
+.. code-block:: yaml
+
+   HttpDigitalOutputDriver: {}
+
+Implements:
+  - :any:`DigitalOutputProtocol`
+
+Arguments:
+  - None
+
 PyVISADriver
 ~~~~~~~~~~~~
-The PyVISADriver uses a PyVISADevice resource to control test equipment manageable by PyVISA.
+The :any:`PyVISADriver` uses a `PyVISADevice`_ resource to control test
+equipment manageable by PyVISA.
 
 Binds to:
   pyvisa_resource:
     - `PyVISADevice`_
 
 Implements:
   - None yet
 
 Arguments:
   - None
 
 NetworkInterfaceDriver
 ~~~~~~~~~~~~~~~~~~~~~~
-This driver allows controlling a network interface (such as Ethernet or WiFi) on
-the exporter using NetworkManager.
+The :any:`NetworkInterfaceDriver` allows controlling a network interface (such
+as Ethernet or WiFi) on the exporter using NetworkManager.
 
 The configuration is based on dictionaries with contents similar to NM's
 connection files in INI-format.
 Currently basic wired and wireless configuration options have been tested.
 
 To use it, `PyGObject <https://pygobject.readthedocs.io/>`_ must be installed
 (on the same system as the network interface).
-For Debian, the necessary packages are `python3-gi` and `gir1.2-nm-1.0`.
+For Debian, the necessary packages are ``python3-gi`` and ``gir1.2-nm-1.0``.
 
 It supports:
+
 - static and DHCP address configuration
 - WiFi client or AP
 - connection sharing (DHCP server with NAT)
 - listing DHCP leases (if the client has sufficient permissions)
 
 Binds to:
   iface:
     - `NetworkInterface`_
+    - `RemoteNetworkInterface`_
     - `USBNetworkInterface`_
+
+Implements:
+  - None yet
+
+Arguments:
+  - None
+
+RawNetworkInterfaceDriver
+~~~~~~~~~~~~~~~~~~~~~~~~~
+The :any:`RawNetworkInterfaceDriver` allows "raw" control of a network
+interface (such as Ethernet or WiFi).
+
+The labgrid-raw-interface helper (``helpers/labgrid-raw-interface``) needs to
+be installed in the PATH and usable via sudo without password.
+A configuration file ``/etc/labgrid/helpers.yaml`` must be installed on hosts
+exporting network interfaces for the RawNetworkInterfaceDriver, e.g.:
+
+.. code-block:: yaml
+
+   raw-interface:
+     denied-interfaces:
+       - 'eth1'
+
+It supports:
+
+- recording traffic
+- replaying traffic
+- basic statistic collection
+
+For now, the RawNetworkInterfaceDriver leaves pre-configuration of the exported
+network interface to the user, including:
+
+- disabling DHCP
+- disabling IPv6 Duplicate Address Detection (DAD) by SLAAC (Stateless
+  Address Autoconfiguration) and Neighbor Discovery
+- disabling Generic Receive Offload (GRO)
+
+This might change in the future.
+
+Binds to:
+  iface:
+    - `NetworkInterface`_
     - `RemoteNetworkInterface`_
+    - `USBNetworkInterface`_
 
 Implements:
   - None yet
 
 Arguments:
   - None
 
 .. _conf-strategies:
 
 Strategies
 ----------
-
 Strategies are used to ensure that the device is in a certain state during a test.
 Such a state could be the bootloader or a booted Linux kernel with shell.
 
 BareboxStrategy
 ~~~~~~~~~~~~~~~
-A BareboxStrategy has four states:
+A :any:`BareboxStrategy` has four states:
 
 - unknown
 - off
 - barebox
 - shell
 
 Here is an example environment config:
@@ -2831,19 +3249,19 @@
        drivers:
          ManualPowerDriver: {}
          SerialDriver: {}
          BareboxDriver: {}
          ShellDriver:
            prompt: 'root@\w+:[^ ]+ '
            login_prompt: ' login: '
-           username: root
+           username: 'root'
          BareboxStrategy: {}
 
 In order to use the BareboxStrategy via labgrid as a library and transition to
-the ``shell`` state:
+the "shell" state:
 
 .. testsetup:: barebox-strategy
 
    from labgrid.strategy import BareboxStrategy
 
    BareboxStrategy.transition = Mock(return_value=None)
 
@@ -2852,19 +3270,19 @@
    >>> from labgrid import Environment
    >>> e = Environment("barebox-env.yaml")
    >>> t = e.get_target("main")
    >>> s = t.get_driver("BareboxStrategy")
    >>> s.transition("shell")
 
 This command would transition from the bootloader into a Linux shell and
-activate the ShellDriver.
+activate the `ShellDriver`_.
 
 ShellStrategy
 ~~~~~~~~~~~~~
-A ShellStrategy has three states:
+A :any:`ShellStrategy` has three states:
 
 - unknown
 - off
 - shell
 
 Here is an example environment config:
 
@@ -2878,19 +3296,19 @@
            port: '/dev/ttyUSB0'
        drivers:
          ManualPowerDriver: {}
          SerialDriver: {}
          ShellDriver:
            prompt: 'root@\w+:[^ ]+ '
            login_prompt: ' login: '
-           username: root
+           username: 'root'
          ShellStrategy: {}
 
 In order to use the ShellStrategy via labgrid as a library and transition to
-the ``shell`` state:
+the "shell" state:
 
 .. testsetup:: shell-strategy
 
    from labgrid.strategy import ShellStrategy
 
    ShellStrategy.transition = Mock(return_value=None)
 
@@ -2898,19 +3316,19 @@
 
    >>> from labgrid import Environment
    >>> e = Environment("shell-env.yaml")
    >>> t = e.get_target("main")
    >>> s = t.get_driver("ShellStrategy")
 
 This command would transition directly into a Linux shell and
-activate the ShellDriver.
+activate the `ShellDriver`_.
 
 UBootStrategy
 ~~~~~~~~~~~~~
-A UBootStrategy has four states:
+A :any:`UBootStrategy` has four states:
 
 - unknown
 - off
 - uboot
 - shell
 
 Here is an example environment config:
@@ -2926,19 +3344,19 @@
        drivers:
          ManualPowerDriver: {}
          SerialDriver: {}
          UBootDriver: {}
          ShellDriver:
            prompt: 'root@\w+:[^ ]+ '
            login_prompt: ' login: '
-           username: root
+           username: 'root'
          UBootStrategy: {}
 
 In order to use the UBootStrategy via labgrid as a library and transition to
-the ``shell`` state:
+the "shell" state:
 
 .. testsetup:: uboot-strategy
 
    from labgrid.strategy import UBootStrategy
 
    UBootStrategy.transition = Mock(return_value=None)
 
@@ -2947,44 +3365,44 @@
    >>> from labgrid import Environment
    >>> e = Environment("uboot-env.yaml")
    >>> t = e.get_target("main")
    >>> s = t.get_driver("UBootStrategy")
    >>> s.transition("shell")
 
 This command would transition from the bootloader into a Linux shell and
-activate the ShellDriver.
+activate the `ShellDriver`_.
 
 DockerStrategy
 ~~~~~~~~~~~~~~
-A DockerStrategy has three states:
+A :any:`DockerStrategy` has three states:
 
 - unknown
 - gone
 - accessible
 
 Here is an example environment config:
 
 .. code-block:: yaml
    :name: docker-env.yaml
 
    targets:
      main:
        resources:
          DockerDaemon:
-           docker_daemon_url: unix://var/run/docker.sock
+           docker_daemon_url: 'unix://var/run/docker.sock'
        drivers:
          DockerDriver:
-           image_uri: "rastasheep/ubuntu-sshd:16.04"
-           container_name: "ubuntu-lg-example"
-           host_config: {"network_mode":"bridge"}
-           network_services: [{"port":22,"username":"root","password":"root"}]
+           image_uri: 'rastasheep/ubuntu-sshd:16.04'
+           container_name: 'ubuntu-lg-example'
+           host_config: {'network_mode': 'bridge'}
+           network_services: [{'port': 22, 'username': 'root', 'password': 'root'}]
          DockerStrategy: {}
 
 In order to use the DockerStrategy via labgrid as a library and transition to
-the ``accessible`` state:
+the "accessible" state:
 
 .. testsetup:: docker-strategy
 
    from labgrid.strategy import DockerStrategy
 
    patch("docker.DockerClient").start()
    DockerStrategy.transition = Mock(return_value=None)
@@ -3002,15 +3420,15 @@
 available which can be used for e.g. SSH access.
 
 Reporters
 ---------
 
 StepReporter
 ~~~~~~~~~~~~
-The StepReporter outputs individual labgrid steps to `STDOUT`.
+The :any:`StepReporter` outputs individual labgrid steps to `STDOUT`.
 
 .. doctest::
 
     >>> from labgrid import StepReporter
     >>> StepReporter.start()
 
 The Reporter can be stopped with a call to the stop function:
@@ -3019,38 +3437,34 @@
 
     >>> from labgrid import StepReporter
     >>> StepReporter.stop()
 
 Stopping the StepReporter if it has not been started will raise an
 AssertionError, as will starting an already started StepReporter.
 
-
 ConsoleLoggingReporter
 ~~~~~~~~~~~~~~~~~~~~~~
-The ConsoleLoggingReporter outputs read calls from the console transports into
+The :any:`ConsoleLoggingReporter` outputs read calls from the console transports into
 files. It takes the path as a parameter.
 
 .. doctest::
 
     >>> from labgrid import ConsoleLoggingReporter
     >>> ConsoleLoggingReporter.start(".")
 
 The Reporter can be stopped with a call to the stop function:
 
 .. doctest::
 
     >>> from labgrid import ConsoleLoggingReporter
     >>> ConsoleLoggingReporter.stop()
 
-
 Stopping the ConsoleLoggingReporter if it has not been started will raise an
 AssertionError, as will starting an already started StepReporter.
 
-
-
 Environment Configuration
 -------------------------
 The environment configuration for a test environment consists of a YAML file
 which contains targets, drivers and resources.
 
 .. note::
 
@@ -3130,16 +3544,16 @@
       port: '/dev/ttyS1'
   - RawSerialPort:
       port: '/dev/ttyS2'
   drivers:
   - SerialDriver: {}
   - SerialDriver: {}
 
-This configuration doesn't specify which :any:`RawSerialPort` to use for each
-:any:`SerialDriver`, so it will cause an exception when instantiating the
+This configuration doesn't specify which `RawSerialPort`_ to use for each
+`SerialDriver`_, so it will cause an exception when instantiating the
 :any:`Target`.
 To bind the correct driver to the correct resource, explicit ``name`` and
 ``bindings`` properties are used:
 
 .. code-block:: yaml
 
   resources:
@@ -3155,38 +3569,39 @@
       bindings:
         port: 'foo'
   - SerialDriver:
       name: 'bar_driver'
       bindings:
         port: 'bar'
 
-The property name for the binding (e.g. `port` in the example above) is
+The property name for the binding (e.g. ``port`` in the example above) is
 documented for each individual driver in this chapter.
 
 The YAML configuration file also supports templating for some substitutions,
 these are:
 
-- LG_* variables, are replaced with their respective LG_* environment variable
-- BASE is substituted with the base directory of the YAML file.
+- ``LG_*`` variables, are replaced with their respective ``LG_*`` environment
+  variable
+- ``BASE`` is substituted with the base directory of the YAML file.
 
 As an example:
 
 .. code-block:: yaml
 
   targets:
     main:
       resources:
         RemotePlace:
-          name: !template $LG_PLACE
+          name: !template '$LG_PLACE'
   tools:
-    qemu_bin: !template "$BASE/bin/qemu-bin"
+    qemu_bin: !template '$BASE/bin/qemu-bin'
 
-would resolve the qemu_bin path relative to the BASE dir of the YAML file and
-try to use the RemotePlace with the name set in the LG_PLACE environment
-variable.
+would resolve the ``qemu_bin`` path relative to the ``BASE`` dir of the YAML
+file and try to use the `RemotePlace`_ with the name set in the ``LG_PLACE``
+environment variable.
 
 See the :ref:`labgrid-device-config` man page for documentation on the
 top-level ``options``, ``images``, ``tools``, and ``examples`` keys in the
 environment configuration.
 
 Exporter Configuration
 ----------------------
@@ -3217,80 +3632,87 @@
      <resource-name-1>:
        <params>
 
 By default, the class name is inferred from the resource name,
 and `<params>` will be passed to its constructor.
 For USB resources, you will most likely want to use :ref:`udev-matching` here.
 
-As a simple example, here is one group called *usb-hub-in-rack12* containing
-a single :any:`USBSerialPort` resource (using udev matching), which will be
-exported as `exportername/usb-hub-in-rack12/NetworkSerialPort/USBSerialPort`:
+As a simple example, here is one group called ``usb-hub-in-rack12`` containing
+a single `USBSerialPort`_ resource (using udev matching), which will be
+exported as ``exportername/usb-hub-in-rack12/NetworkSerialPort/USBSerialPort``:
 
 .. code-block:: yaml
 
    usb-hub-in-rack12:
      USBSerialPort:
        match:
-         '@ID_PATH': pci-0000:05:00.0-usb-3-1.3
+         '@ID_PATH': 'pci-0000:05:00.0-usb-3-1.3'
 
 To export multiple resources of the same class in the same group,
 you can choose a unique resource name, and then use the ``cls`` parameter to
 specify the class name instead (which will not be passed as a parameter to the
 class constructor).
-In this next example we will export one :any:`USBSerialPort` as
-`exportername/usb-hub-in-rack12/NetworkSerialPort/console-main`,
-and another :any:`USBSerialPort` as
-`exportername/usb-hub-in-rack12/NetworkSerialPort/console-secondary`:
+In this next example we will export one `USBSerialPort`_ as
+``exportername/usb-hub-in-rack12/NetworkSerialPort/console-main``,
+and another `USBSerialPort`_ as
+``exportername/usb-hub-in-rack12/NetworkSerialPort/console-secondary``:
 
 .. code-block:: yaml
 
    usb-hub-in-rack12:
      console-main:
-       cls: USBSerialPort
+       cls: 'USBSerialPort'
        match:
-         '@ID_PATH': pci-0000:05:00.0-usb-3-1.3
+         '@ID_PATH': 'pci-0000:05:00.0-usb-3-1.3'
      console-secondary:
-       cls: USBSerialPort
+       cls: 'USBSerialPort'
        match:
-         '@ID_PATH': pci-0000:05:00.0-usb-3-1.4
+         '@ID_PATH': 'pci-0000:05:00.0-usb-3-1.4'
 
 Note that you could also split the resources up into distinct groups instead
 to achieve the same effect:
 
 .. code-block:: yaml
 
    usb-hub-in-rack12-port3:
      USBSerialPort:
        match:
-         '@ID_PATH': pci-0000:05:00.0-usb-3-1.3
+         '@ID_PATH': 'pci-0000:05:00.0-usb-3-1.3'
    usb-hub-in-rack12-port4:
      USBSerialPort:
        match:
-         '@ID_PATH': pci-0000:05:00.0-usb-3-1.4
+         '@ID_PATH': 'pci-0000:05:00.0-usb-3-1.4'
 
 Templating
 ~~~~~~~~~~
 To reduce the amount of repeated declarations when many similar resources
 need to be exported, the `Jinja2 template engine <http://jinja.pocoo.org/>`_
 is used as a preprocessor for the configuration file:
 
 .. code-block:: yaml
 
    ## Iterate from group 1001 to 1016
    # for idx in range(1, 17)
    {{ 1000 + idx }}:
      NetworkSerialPort:
-       {host: rl1, port: {{ 4000 + idx }}}
+       host: 'rl1'
+       port: {{ 4000 + idx }}
      NetworkPowerPort:
        # if 1 <= idx <= 8
-       {model: apc, host: apc1, index: {{ idx }}}
+       model: 'apc'
+       host: 'apc1'
+       index: {{ idx }}
        # elif 9 <= idx <= 12
-       {model: netio, host: netio4, index: {{ idx - 8 }}}
+       model: 'netio'
+       host: 'netio4'
+       index: {{ idx - 8 }}
        # elif 13 <= idx <= 16
-       {model: netio, host: netio5, index: {{ idx - 12 }}}
+       model: 'netio'
+       host: 'netio5'
+       index: {{ idx - 12 }}
        # endif
    # endfor
 
 Use ``#`` for line statements (like the for loops in the example) and ``##``
 for line comments.
 Statements like ``{{ 4000 + idx }}`` are expanded based on variables in the
 Jinja2 template.
```

### Comparing `labgrid-23.1a2/doc/design_decisions.rst` & `labgrid-24.0a1/doc/design_decisions.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/development.rst` & `labgrid-24.0a1/doc/development.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/getting_started.rst` & `labgrid-24.0a1/doc/getting_started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,33 +21,45 @@
 
 .. code-block:: bash
 
     $ virtualenv -p python3 labgrid-venv
     $ source labgrid-venv/bin/activate
     labgrid-venv $ pip install --upgrade pip
 
+Install Latest Release
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: bash
+
+    labgrid-venv $ pip install labgrid
+
+Install Development State
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
 Start by cloning the repository and installing labgrid:
 
 .. code-block:: bash
 
     labgrid-venv $ git clone https://github.com/labgrid-project/labgrid
     labgrid-venv $ cd labgrid && pip install .
 
 .. note::
    If you are **not** installing via pip and intend to use Serial over IP
    (RFC2217), it is highly recommended to uninstall pyserial after installation
    and replace it with the pyserial version from the labgrid project:
 
-   https://github.com/labgrid-project/pyserial/releases/tag/v3.4.0.1
+   https://github.com/labgrid-project/pyserial/tags
 
    This pyserial version has two fixes for an Issue we found with Serial over IP
    multiplexers. Additionally it reduces the Serial over IP traffic considerably
    since the port is not reconfigured when labgrid changes the timeout (which is
    done inside the library a lot).
 
+Test Installation
+~~~~~~~~~~~~~~~~~
 
 Test your installation by running:
 
 .. code-block:: bash
 
     labgrid-venv $ labgrid-client --help
     usage: labgrid-client [-h] [-x URL] [-c CONFIG] [-p PLACE] [-d] COMMAND ...
@@ -368,15 +380,16 @@
    :file:`.crossbar/config-anonymous.yaml` as a starting point. You most likely
    want to make sure that the ``workdir`` option matches the path given via the
    ``--cbdir`` option in the service file; see
    :ref:`remote-getting-started-coordinator` for further information.
 #. Adjust the ``SupplementaryGroups`` option in the
    :file:`labgrid-exporter.service` file to your distribution so that the
    exporter gains read and write access on TTY devices (for ``ser2net``); most
-   often, this group is called ``dialout`` or ``tty``.
+   often, these groups are called ``dialout``, ``plugdev`` or ``tty``.
+   Depending on your udev configuration, you may need multiple groups.
 #. Set the coordinator URL the exporter should connect to by overriding the
    exporter service file; i.e. execute ``systemctl edit
    labgrid-exporter.service`` and add the following snippet:
 
    .. code-block::
 
       [Service]
```

### Comparing `labgrid-23.1a2/doc/images/favicon.png` & `labgrid-24.0a1/doc/images/favicon.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/images/labgrid_logo_outline.svg` & `labgrid-24.0a1/doc/images/labgrid_logo_outline.svg`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/index.rst` & `labgrid-24.0a1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/overview.rst` & `labgrid-24.0a1/doc/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,20 @@
 serial port case).
 
 Resources which do not need explicit support in the exporter, are just
 published as declared in the configuration file.
 This is useful to register externally configured resources such as network
 power switches or serial port servers with a labgrid coordinator.
 
+.. note::
+  Users will require SSH access to the exporter to access services and command
+  line utilities. You also have to ensure that users can access usb devices for
+  i.e. imx-usb-loader. To test a SSH jump to a device over the exporter outside
+  of labgrid, `ssh -J EXPORTER USER@DEVICE` can be used.
+
 .. _overview-client:
 
 Client
 ~~~~~~
 The client requests the current lists of resources and places from the
 coordinator when it connects to it and then registers for change events.
 Most of its functionality is exposed via the `labgrid-client` CLI tool.
```

### Comparing `labgrid-23.1a2/doc/res/config_graph.svg` & `labgrid-24.0a1/doc/res/config_graph.svg`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/res/graphstrategy-via-nand.png` & `labgrid-24.0a1/doc/res/graphstrategy-via-nand.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/res/graphstrategy-via-nfs.png` & `labgrid-24.0a1/doc/res/graphstrategy-via-nfs.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/doc/usage.rst` & `labgrid-24.0a1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/dockerfiles/Dockerfile` & `labgrid-24.0a1/dockerfiles/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-FROM debian:bullseye-slim AS labgrid-base
+FROM debian:bookworm-slim AS labgrid-base
 
 LABEL maintainer="eha@deif.com"
 
 ENV DEBIAN_FRONTEND=noninteractive
 
 COPY ./ /opt/labgrid/
 
 RUN set -e ;\
     apt update -q=2 ;\
     apt install -q=2 --yes --no-install-recommends python3 python3-dev python3-pip python3-setuptools git build-essential libsnappy-dev ;\
-    pip3 install -U pip;\
+    pip3 install --break-system-packages -U pip;\
     apt clean ;\
     rm -rf /var/lib/apt/lists/* ;\
     git clone https://github.com/vishnubob/wait-for-it.git opt/wait-for-it && cd opt/wait-for-it  && git reset --hard 54d1f0bfeb6557adf8a3204455389d0901652242
 
 #
 # Client
 #
 FROM labgrid-base AS labgrid-client
 ARG VERSION
 
 RUN set -e ;\
     cd /opt/labgrid ;\
-    pip3 install yq ;\
-    SETUPTOOLS_SCM_PRETEND_VERSION="$VERSION" pip3 install --no-cache-dir . ;\
+    pip3 install --break-system-packages yq ;\
+    SETUPTOOLS_SCM_PRETEND_VERSION="$VERSION" pip3 install --break-system-packages --no-cache-dir . ;\
     apt update -q=2 ;\
     apt install -q=2 --yes --no-install-recommends microcom openssh-client rsync jq qemu-system qemu-utils ;\
     apt clean ;\
     rm -rf /var/lib/apt/lists/*
 
 CMD ["/bin/bash"]
 
@@ -37,18 +37,18 @@
 FROM labgrid-base AS labgrid-coordinator
 ARG VERSION
 
 ENV CROSSBAR_DIR=/opt/crossbar
 
 RUN set -e ;\
     cd /opt/labgrid ;\
-    pip3 install virtualenv ;\
-    SETUPTOOLS_SCM_PRETEND_VERSION="$VERSION" pip3 install --no-cache-dir . ;\
+    pip3 install --break-system-packages virtualenv ;\
+    SETUPTOOLS_SCM_PRETEND_VERSION="$VERSION" pip3 install --break-system-packages --no-cache-dir . ;\
     virtualenv -p python3 crossbar-venv ;\
-    crossbar-venv/bin/pip3 install -r crossbar-requirements.txt ;\
+    crossbar-venv/bin/pip3 install --break-system-packages -r crossbar-requirements.txt ;\
     sed -i "s#^  executable: .*\$#  executable: python3#" .crossbar/config-anonymous.yaml
 
 VOLUME /opt/crossbar
 
 EXPOSE 20408
 
 CMD ["/opt/labgrid/crossbar-venv/bin/crossbar", "start", "--config", "/opt/labgrid/.crossbar/config-anonymous.yaml"]
@@ -59,15 +59,15 @@
 FROM labgrid-base AS labgrid-exporter
 ARG VERSION
 
 COPY dockerfiles/exporter/entrypoint.sh /entrypoint.sh
 
 RUN set -e ;\
     cd /opt/labgrid ;\
-    SETUPTOOLS_SCM_PRETEND_VERSION="$VERSION" pip3 install --no-cache-dir . ;\
+    SETUPTOOLS_SCM_PRETEND_VERSION="$VERSION" pip3 install --break-system-packages --no-cache-dir . ;\
     apt update -q=2 ;\
     apt install -q=2 --yes --no-install-recommends ser2net ;\
     apt clean ;\
     rm -rf /var/lib/apt/lists/*
 
 VOLUME /opt/conf
```

### Comparing `labgrid-23.1a2/dockerfiles/README.rst` & `labgrid-24.0a1/dockerfiles/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,40 @@
 
    $ docker build --target labgrid-client -t labgrid-client -f dockerfiles/Dockerfile .
 
 Using `BuildKit <https://docs.docker.com/develop/develop-images/build_enhancements/>`_
 is recommended to reduce build times.
 
 You can also choose to build all 3 images,
-with the included script
-(which also must be run from the root of this repository):
+with the included script.
 
 .. code-block:: bash
 
    $ pip install --upgrade setuptools_scm
    $ ./dockerfiles/build.sh
 
-The script supports ``podman`` as well
+The script supports ``podman`` as well.
 
 .. code-block:: bash
   
    $ export DOCKER=podman
    $ ./dockerfiles/build.sh
 
+It builds for the native platform by default. However, building
+for foreign platforms is also supported using `docker buildx
+<https://docs.docker.com/build/building/multi-platform/>` or `podman
+buildx <https://docs.podman.io/en/latest/markdown/podman-build.1.html>`
+by passing the platform of choice, e.g. `linux/arm64`.
+
+.. code-block:: bash
+
+   $ pip install --upgrade setuptools_scm
+   $ ./dockerfiles/build.sh linux/arm64
+
+
 Usage
 -----
 
 All 3 images are to be considered base images
 with the required software installed.
 No policy or configuration is done.
```

### Comparing `labgrid-23.1a2/dockerfiles/staging/client/.ssh/id_rsa` & `labgrid-24.0a1/dockerfiles/staging/client/.ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/dockerfiles/staging/docker-compose.yml` & `labgrid-24.0a1/dockerfiles/staging/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/dockerfiles/staging/dut/Dockerfile` & `labgrid-24.0a1/dockerfiles/staging/dut/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM debian:bullseye-slim
+FROM debian:bookworm-slim
 
 MAINTAINER "Kasper Revsbech" <mail@krevsbech.dk>
 
 ENV DEBIAN_FRONTEND=noninteractive
 
 RUN set -e ;\
     apt update -q=2 ;\
@@ -11,15 +11,15 @@
     rm -rf /var/lib/apt/lists/* ;\
     mkdir /var/run/sshd ;\
     echo 'root:PASSWORD' | chpasswd ;\
     echo 'PermitRootLogin yes' >> /etc/ssh/sshd_config ;\
     sed 's@session\s*required\s*pam_loginuid.so@session optional pam_loginuid.so@g' -i /etc/pam.d/sshd
     # SSH login fix. Otherwise user is kicked off after login
 
-COPY [--chown=root:root] ./authorized_keys /root/.ssh/authorized_keys
+COPY --chown=root:root ./authorized_keys /root/.ssh/authorized_keys
 
 # As sshd scrubs ENV variables if they are set by the ENV varibale ensure to put the into /etc/profile as shown below
 ENV NOTVISIBLE "in users profile"
 RUN echo "export VISIBLE=now" >> /etc/profile
 
 EXPOSE 2222
 CMD ["/usr/sbin/sshd", "-D", "-p", "2222"]
```

### Comparing `labgrid-23.1a2/examples/barebox/test_sleep.py` & `labgrid-24.0a1/examples/barebox/test_sleep.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/deditec-relais8/deditec.py` & `labgrid-24.0a1/examples/deditec-relais8/deditec.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/deditec-relais8/deditec_remote.py` & `labgrid-24.0a1/examples/deditec-relais8/deditec_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/docker/README.md` & `labgrid-24.0a1/examples/docker/README.md`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/library/test.py` & `labgrid-24.0a1/examples/library/test.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/networkmanager/nm.py` & `labgrid-24.0a1/examples/networkmanager/nm.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/qemu-networking/conftest.py` & `labgrid-24.0a1/examples/qemu-networking/conftest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/qemu-networking/local.yaml` & `labgrid-24.0a1/examples/qemu-networking/local.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/qemu-networking/qemunetworkstrategy.py` & `labgrid-24.0a1/examples/qemu-networking/qemunetworkstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/qemu-networking/test_qemu_networking.py` & `labgrid-24.0a1/examples/qemu-networking/test_qemu_networking.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/shell/test_hwclock.py` & `labgrid-24.0a1/examples/shell/test_hwclock.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/shell/test_memory.py` & `labgrid-24.0a1/examples/shell/test_memory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/shell/test_rt.py` & `labgrid-24.0a1/examples/shell/test_rt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/strategy/bareboxrebootstrategy.py` & `labgrid-24.0a1/examples/strategy/bareboxrebootstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/strategy/quartusstrategy.py` & `labgrid-24.0a1/examples/strategy/quartusstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/strategy/test_barebox_strategy.py` & `labgrid-24.0a1/examples/strategy/test_barebox_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/strategy/test_uboot_strategy.py` & `labgrid-24.0a1/examples/strategy/test_uboot_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/sysfsgpio/sysfsgpio.py` & `labgrid-24.0a1/examples/sysfsgpio/sysfsgpio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/sysfsgpio/sysfsgpio_remote.py` & `labgrid-24.0a1/examples/sysfsgpio/sysfsgpio_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usb/mxs-usb.yaml` & `labgrid-24.0a1/examples/usb/mxs-usb.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usbpower/README.rst` & `labgrid-24.0a1/examples/usbpower/README.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usbpower/cycle.py` & `labgrid-24.0a1/examples/usbpower/cycle.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usbpower/examplestrategy.py` & `labgrid-24.0a1/examples/usbpower/examplestrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usbpower/exports.yaml` & `labgrid-24.0a1/examples/usbpower/exports.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usbpower/local.yaml` & `labgrid-24.0a1/examples/usbpower/local.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/examples/usbpower/test_example.py` & `labgrid-24.0a1/examples/usbpower/test_example.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/helpers/labgrid-bound-connect` & `labgrid-24.0a1/helpers/labgrid-bound-connect`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/autoinstall/main.py` & `labgrid-24.0a1/labgrid/autoinstall/main.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/binding.py` & `labgrid-24.0a1/labgrid/binding.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,20 @@
     def resolve_conflicts(self, client):
         """
         Called by the Target to allow this object to deactivate conflicting
         clients.
         """
         pass
 
+    def get_bound_resources(self):
+        """
+        Called by the Target to find the correct driver corresponding to a resource
+        """
+        raise NotImplementedError("get_bound_resources not implemented!")
+
     @classmethod
     def check_active(cls, func):
         @wraps(func)
         def wrapper(self, *_args, **_kwargs):
             if self.state is not BindingState.active:
                 raise StateError(
                     f'{self} has not been activated, {func.__qualname__} cannot be called in state "{self.state.name}"'  # pylint: disable=line-too-long
```

### Comparing `labgrid-23.1a2/labgrid/config.py` & `labgrid-24.0a1/labgrid/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,22 @@
             tool (str): the tool to retrieve the path for
 
         Returns:
             str: path to the requested tools
         """
         try:
             path = str(self.data['tools'][tool])
-            return self.resolve_path(path)
         except KeyError:
-            return None
+            return tool
+
+        resolved = self.resolve_path(path)
+        if os.path.exists(resolved):
+            return resolved
+
+        return path
 
     def get_image_path(self, kind):
         """Retrieve an entry from the images subkey
 
         Args:
             kind (str): the kind of the image to retrieve the path for
```

### Comparing `labgrid-23.1a2/labgrid/consoleloggingreporter.py` & `labgrid-24.0a1/labgrid/consoleloggingreporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/__init__.py` & `labgrid-24.0a1/labgrid/driver/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .usbloader import MXSUSBDriver, IMXUSBDriver, BDIMXUSBDriver, RKUSBDriver, UUUDriver
 from .usbsdmuxdriver import USBSDMuxDriver
 from .usbsdwiredriver import USBSDWireDriver
 from .common import Driver
 from .qemudriver import QEMUDriver
 from .modbusdriver import ModbusCoilDriver
 from .modbusrtudriver import ModbusRTUDriver
-from .sigrokdriver import SigrokDriver, SigrokPowerDriver
+from .sigrokdriver import SigrokDriver, SigrokPowerDriver, SigrokDmmDriver
 from .usbstoragedriver import USBStorageDriver, NetworkUSBStorageDriver, Mode
 from .resetdriver import DigitalOutputResetDriver
 from .gpiodriver import GpioDigitalOutputDriver
 from .filedigitaloutput import FileDigitalOutputDriver
 from .serialdigitaloutput import SerialPortDigitalOutputDriver
 from .xenadriver import XenaDriver
 from .dockerdriver import DockerDriver
@@ -36,13 +36,15 @@
 from .pyvisadriver import PyVISADriver
 from .usbhidrelay import HIDRelayDriver
 from .flashscriptdriver import FlashScriptDriver
 from .usbaudiodriver import USBAudioInputDriver
 from .usbvideodriver import USBVideoDriver
 from .httpvideodriver import HTTPVideoDriver
 from .networkinterfacedriver import NetworkInterfaceDriver
-from .provider import HTTPProviderDriver, NFSPProviderDriver, TFTPProviderDriver
+from .provider import HTTPProviderDriver, NFSProviderDriver, TFTPProviderDriver
+from .rawnetworkinterfacedriver import RawNetworkInterfaceDriver
 from .mqtt import TasmotaPowerDriver
 from .manualswitchdriver import ManualSwitchDriver
 from .usbtmcdriver import USBTMCDriver
 from .deditecrelaisdriver import DeditecRelaisDriver
 from .dediprogflashdriver import DediprogFlashDriver
+from .httpdigitaloutput import HttpDigitalOutputDriver
```

### Comparing `labgrid-23.1a2/labgrid/driver/bareboxdriver.py` & `labgrid-24.0a1/labgrid/driver/bareboxdriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import shlex
 
 import attr
 from pexpect import TIMEOUT
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, ConsoleProtocol, LinuxBootProtocol
@@ -36,16 +35,17 @@
     interrupt = attr.ib(default="\n", validator=attr.validators.instance_of(str))
     bootstring = attr.ib(default=r"Linux version \d", validator=attr.validators.instance_of(str))
     password = attr.ib(default="", validator=attr.validators.instance_of(str))
     login_timeout = attr.ib(default=60, validator=attr.validators.instance_of(int))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}:{self.target}")
         self._status = 0
+        # barebox' default log level, used as fallback if no log level can be saved
+        self.saved_log_level = 7
 
     def on_activate(self):
         """Activate the BareboxDriver
 
         This function tries to login if not already active
         """
         if self._status == 0:
@@ -59,30 +59,37 @@
         self._status = 0
 
     @Driver.check_active
     @step(args=['cmd'])
     def run(self, cmd: str, *, timeout: int = 30):
         return self._run(cmd, timeout=timeout)
 
-    def _run(self, cmd: str, *, timeout: int = 30, codec: str = "utf-8", decodeerrors: str = "strict"):  # pylint: disable=unused-argument,line-too-long
+    def _run(self, cmd: str, *, timeout: int = 30, adjust_log_level: bool = True, codec: str = "utf-8", decodeerrors: str = "strict"):  # pylint: disable=unused-argument,line-too-long
         """
         Runs the specified command on the shell and returns the output.
 
         Args:
             cmd (str): command to run on the shell
             timeout (int): optional, timeout in seconds
 
         Returns:
             Tuple[List[str],List[str], int]: if successful, None otherwise
         """
         # FIXME: use codec, decodeerrors
         marker = gen_marker()
         # hide marker from expect
         hidden_marker = f'"{marker[:4]}""{marker[4:]}"'
-        cmp_command = f'''echo -o /cmd {shlex.quote(cmd)}; echo {hidden_marker}; sh /cmd; echo {hidden_marker} $?;'''  # pylint: disable=line-too-long
+        # generate command with marker and log level adjustment
+        cmp_command = f'echo -o /cmd {shlex.quote(cmd)}; echo {hidden_marker};'
+        if self.saved_log_level and adjust_log_level:
+            cmp_command += f' global.loglevel={self.saved_log_level};'
+        cmp_command += f' sh /cmd; echo {hidden_marker} $?;'
+        if self.saved_log_level and adjust_log_level:
+            cmp_command += ' global.loglevel=0;'
+
         if self._status == 1:
             self.console.sendline(cmp_command)
             _, _, match, _ = self.console.expect(
                 rf'{marker}(.*){marker}\s+(\d+)\s+.*{self.prompt}',
                 timeout=timeout)
             # Remove VT100 Codes and split by newline
             data = re_vt100.sub('', match.group(1).decode('utf-8')).split('\r\n')[1:-1]
@@ -182,24 +189,39 @@
                         f"Timeout of {self.login_timeout} seconds exceeded during waiting for login"
                     )
 
             last_before = before
 
         self._check_prompt()
 
+        # remember barebox' log level - we don't expect to be interrupted here
+        # by pollers because no hardware interaction is triggered by echo, so
+        # it should be safe to use the usual shell wrapper via _run()
+        stdout, _, exitcode = self._run("echo $global.loglevel", adjust_log_level=False)
+        [saved_log_level] = stdout
+        if exitcode == 0 and saved_log_level.isnumeric():
+            self.saved_log_level = saved_log_level
+
+        # silence barebox, the driver can get confused by asynchronous messages
+        # logged to the console otherwise
+        self._run("global.loglevel=0", adjust_log_level=False)
+
     @Driver.check_active
     def await_boot(self):
         """Wait for the initial Linux version string to verify we successfully
         jumped into the kernel.
         """
         self.console.expect(self.bootstring)
 
     @Driver.check_active
     def boot(self, name: str):
         """Boot the default or a specific boot entry
 
         Args:
             name (str): name of the entry to boot"""
+        # recover saved log level
+        self._run(f"global.loglevel={self.saved_log_level}", adjust_log_level=False)
+
         if name:
             self.console.sendline(f"boot -v {name}")
         else:
             self.console.sendline("boot -v")
```

### Comparing `labgrid-23.1a2/labgrid/driver/commandmixin.py` & `labgrid-24.0a1/labgrid/driver/commandmixin.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/common.py` & `labgrid-24.0a1/labgrid/driver/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import subprocess
 import attr
 
 from ..binding import BindingError, BindingMixin
 from .exception import ExecutionError
 
 
@@ -21,14 +22,19 @@
     """
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if self.target is None:
             raise BindingError("Drivers can only be created on a valid target")
 
+        logger_name = f"{self.__class__.__name__}({self.target.name})"
+        if self.name:
+            logger_name += f":{self.name}"
+        self.logger = logging.getLogger(logger_name)
+
     def get_priority(self, protocol):
         """Retrieve the priority for a given protocol
 
         Arguments:
         protocol - protocol to search for in the MRO
 
         Returns:
@@ -63,10 +69,20 @@
         """Drivers are deactivated on export by default.
 
         If the driver can handle external accesses even while active, it can
         return True here.
         """
         return False
 
+    def get_bound_resources(self):
+        """Return the bound resources for a driver
+
+        This recursively calls all suppliers and combines the sets of returned resources.
+        """
+        res = set()
+        for supplier in self.suppliers:
+            res |= supplier.get_bound_resources()
+        return res
+
 def check_file(filename, *, command_prefix=[]):
     if subprocess.call(command_prefix + ['test', '-r', filename]) != 0:
         raise ExecutionError(f"File {filename} is not readable")
```

### Comparing `labgrid-23.1a2/labgrid/driver/consoleexpectmixin.py` & `labgrid-24.0a1/labgrid/driver/consoleexpectmixin.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/dediprogflashdriver.py` & `labgrid-24.0a1/labgrid/driver/dediprogflashdriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os.path
-import logging
 import attr
 
 from ..resource import NetworkDediprogFlasher
 from ..factory import target_factory
 from ..step import step
 from .common import Driver, check_file
 from ..util.managedfile import ManagedFile
@@ -20,15 +19,14 @@
     }
 
     image = attr.ib(validator=attr.validators.optional(attr.validators.instance_of(str)),
                     default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f'{self}')
         if self.target.env:
             self.tool = self.target.env.config.get_tool('dpcmd')
         else:
             self.tool = 'dpcmd'
 
     def _get_dediprog_prefix(self):
         return self.flasher.command_prefix + [self.tool]
```

### Comparing `labgrid-23.1a2/labgrid/driver/deditecrelaisdriver.py` & `labgrid-24.0a1/labgrid/driver/deditecrelaisdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/dfudriver.py` & `labgrid-24.0a1/labgrid/driver/dfudriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "dfu": {"DFUDevice", "NetworkDFUDevice"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('dfu-util') or 'dfu-util'
+            self.tool = self.target.env.config.get_tool('dfu-util')
         else:
             self.tool = 'dfu-util'
 
     def _get_dfu_prefix(self):
         return self.dfu.command_prefix + [
             self.tool,
             "-p", self.dfu.path,
```

### Comparing `labgrid-23.1a2/labgrid/driver/dockerdriver.py` & `labgrid-24.0a1/labgrid/driver/dockerdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """
 Class for connecting to a docker daemon running on the host machine.
 """
-
-import logging
-
 import attr
 
 from labgrid.factory import target_factory
 from labgrid.driver.common import Driver
 from labgrid.resource.docker import DockerConstants
 from labgrid.protocol.powerprotocol import PowerProtocol
 
@@ -58,15 +55,14 @@
         default=None, validator=attr.validators.optional(
             attr.validators.instance_of(dict)))
     network_services = attr.ib(
         default=None, validator=attr.validators.optional(
             attr.validators.instance_of(list)))
 
     def __attrs_post_init__(self):
-        self.logger = logging.getLogger(f"{self}({self.target})")
         super().__attrs_post_init__()
         self._client = None
         self._container = None
 
     def on_activate(self):
         """ On activation:
         1. Import docker module (_client and _container remain available)
```

### Comparing `labgrid-23.1a2/labgrid/driver/externalconsoledriver.py` & `labgrid-24.0a1/labgrid/driver/externalconsoledriver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import fcntl
-import logging
 import os
 import select
 import shlex
 import subprocess
 
 import attr
 
@@ -21,20 +20,19 @@
     Driver implementing the ConsoleProtocol interface using a subprocess
     """
     cmd = attr.ib(validator=attr.validators.instance_of(str))
     txdelay = attr.ib(default=0.0, validator=attr.validators.instance_of(float))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}({self.target})")
         self.status = 0
         self._child = None
 
     def open(self):
-        """Starts the subprocess, does nothing if it is already closed"""
+        """Starts the subprocess, does nothing if it is already open"""
         if self.status:
             return
         cmd = shlex.split(self.cmd)
         self._child = subprocess.Popen(
             cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=None
         )
```

### Comparing `labgrid-23.1a2/labgrid/driver/fake.py` & `labgrid-24.0a1/labgrid/driver/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # pylint: disable=arguments-differ
-import logging
 import re
 
 import attr
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, ConsoleProtocol, FileTransferProtocol, PowerProtocol
 from .common import Driver
@@ -14,15 +13,14 @@
 @target_factory.reg_driver
 @attr.s(eq=False)
 class FakeConsoleDriver(ConsoleExpectMixin, Driver, ConsoleProtocol):
     txdelay = attr.ib(default=0.0, validator=attr.validators.instance_of(float))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}({self.target})")
         self.rxq = []
         self.txq = []
 
     def _read(self, *_, **__):
         if self.rxq:
             return self.rxq.pop()
         return b''
```

### Comparing `labgrid-23.1a2/labgrid/driver/fastbootdriver.py` & `labgrid-24.0a1/labgrid/driver/fastbootdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         validator=attr.validators.optional(attr.validators.instance_of(str))
     )
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('fastboot') or 'fastboot'
+            self.tool = self.target.env.config.get_tool('fastboot')
         else:
             self.tool = 'fastboot'
 
     def _get_fastboot_prefix(self):
         if isinstance(self.fastboot, (AndroidUSBFastboot, RemoteAndroidUSBFastboot)):
             option = f"usb:{self.fastboot.path}"
         else:
```

### Comparing `labgrid-23.1a2/labgrid/driver/filedigitaloutput.py` & `labgrid-24.0a1/labgrid/driver/filedigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/flashromdriver.py` & `labgrid-24.0a1/labgrid/driver/flashromdriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os.path
-import logging
 import attr
 
 from ..resource import NetworkFlashrom
 from ..factory import target_factory
 from ..step import step
 from ..protocol import BootstrapProtocol
 from .common import Driver, check_file
@@ -20,15 +19,14 @@
         'flashrom_resource': {"Flashrom", NetworkFlashrom},
     }
 
     image = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f'{self}')
         if self.target.env:
             self.tool = self.target.env.config.get_tool('flashrom')
         else:
             self.tool = 'flashrom'
         self.logger.debug('Tool %s', self.tool)
 
     def _get_flashrom_prefix(self):
```

### Comparing `labgrid-23.1a2/labgrid/driver/flashscriptdriver.py` & `labgrid-24.0a1/labgrid/driver/flashscriptdriver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import attr
 
 from ..factory import target_factory
 from ..step import step
 from ..util.managedfile import ManagedFile
 from .common import Driver
 
@@ -23,18 +22,14 @@
         validator=attr.validators.optional(attr.validators.instance_of(str)),
     )
     args = attr.ib(
         default=attr.Factory(list),
         validator=attr.validators.optional(attr.validators.instance_of(list)),
     )
 
-    def __attrs_post_init__(self):
-        super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}:{self.target}")
-
     def on_activate(self):
         pass
 
     def on_deactivate(self):
         pass
 
     @Driver.check_active
```

### Comparing `labgrid-23.1a2/labgrid/driver/gpiodriver.py` & `labgrid-24.0a1/labgrid/driver/gpiodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/httpvideodriver.py` & `labgrid-24.0a1/labgrid/driver/httpvideodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/lxaiobusdriver.py` & `labgrid-24.0a1/labgrid/driver/lxaiobusdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/lxausbmuxdriver.py` & `labgrid-24.0a1/labgrid/driver/lxausbmuxdriver.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     bindings = {
         "mux": {"LXAUSBMux", "NetworkLXAUSBMux"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('usbmuxctl') or 'usbmuxctl'
+            self.tool = self.target.env.config.get_tool('usbmuxctl')
         else:
             self.tool = 'usbmuxctl'
 
     @Driver.check_active
     @step(title='usbmux_set', args=['links'])
     def set_links(self, links):
         args = []
```

### Comparing `labgrid-23.1a2/labgrid/driver/manualswitchdriver.py` & `labgrid-24.0a1/labgrid/driver/manualswitchdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/modbusdriver.py` & `labgrid-24.0a1/labgrid/driver/modbusdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         self.client = self._module.ModbusClient(
             host=host, port=int(port), auto_open=True, auto_close=True)
 
     def on_deactivate(self):
         self.client = None
 
     def _handle_error(self, action):
-        error_code = self.client.last_error()
+        error_code = self.client.last_error
         if error_code == self._consts.MB_EXCEPT_ERR:
-            exc = self.client.last_except()
+            exc = self.client.last_except
             if exc not in [self._consts.EXP_ACKNOWLEDGE, self._consts.EXP_NONE]:
                 raise ExecutionError(
                     f'Could not {action} coil (code={error_code}/exception={exc})')
         raise ExecutionError(f'Could not {action} coil (code={error_code})')
 
     @Driver.check_active
     def set(self, status):
```

### Comparing `labgrid-23.1a2/labgrid/driver/modbusrtudriver.py` & `labgrid-24.0a1/labgrid/driver/modbusrtudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/mqtt.py` & `labgrid-24.0a1/labgrid/driver/mqtt.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     delay = attr.ib(default=2.0, validator=attr.validators.instance_of(float))
     _client = attr.ib(default=None)
     _status = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         import paho.mqtt.client as mqtt
-        self._client = mqtt.Client()
+        self._client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
 
     def on_activate(self):
         self._client.on_message = self._on_message
         self._client.on_connect = self._on_connect
         self._client.connect(self.power.host)
         self._client.loop_start()
 
@@ -41,15 +41,15 @@
     def _on_message(self, client, userdata, msg):
         if msg.payload == b'ON':
             status = True
         elif msg.payload == b'OFF':
             status = False
         self._status = status
 
-    def _on_connect(self, client, userdata, flags, rc):
+    def _on_connect(self, client, userdata, flags, reason_code, properties):
         client.subscribe(self.power.status_topic)
 
     def _publish(self, topic, payload):
         msg = self._client.publish(topic, payload=payload)
         timeout = Timeout(3.0)
         while not msg.is_published:
             time.sleep(0.1)
```

### Comparing `labgrid-23.1a2/labgrid/driver/networkinterfacedriver.py` & `labgrid-24.0a1/labgrid/driver/networkinterfacedriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/onewiredriver.py` & `labgrid-24.0a1/labgrid/driver/onewiredriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/openocddriver.py` & `labgrid-24.0a1/labgrid/driver/openocddriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from itertools import chain
 import attr
 
 from ..factory import target_factory
 from ..protocol import BootstrapProtocol
 from ..step import step
 from ..util.managedfile import ManagedFile
@@ -43,19 +42,18 @@
     load_commands = attr.ib(
         default=None,
         validator=attr.validators.optional(attr.validators.instance_of(list))
     )
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}:{self.target}")
 
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('openocd') or 'openocd'
+            self.tool = self.target.env.config.get_tool('openocd')
             self.config = self.target.env.config.resolve_path_str_or_list(self.config)
             self.search = self.target.env.config.resolve_path_str_or_list(self.search)
         else:
             self.tool = 'openocd'
             if isinstance(self.config, str):
                 self.config = [self.config]
             if isinstance(self.search, str):
```

### Comparing `labgrid-23.1a2/labgrid/driver/power/apc.py` & `labgrid-24.0a1/labgrid/driver/power/apc.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/digipower.py` & `labgrid-24.0a1/labgrid/driver/power/digipower.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/digitalloggers_http.py` & `labgrid-24.0a1/labgrid/driver/power/digitalloggers_http.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/eg_pms2_network.py` & `labgrid-24.0a1/labgrid/driver/power/eg_pms2_network.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/gude.py` & `labgrid-24.0a1/labgrid/driver/power/gude.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/gude24.py` & `labgrid-24.0a1/labgrid/driver/power/gude24.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/gude8031.py` & `labgrid-24.0a1/labgrid/driver/power/gude8031.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/gude8225.py` & `labgrid-24.0a1/labgrid/driver/power/gude8225.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/gude8316.py` & `labgrid-24.0a1/labgrid/driver/power/gude8316.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/netio.py` & `labgrid-24.0a1/labgrid/driver/power/netio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/netio_kshell.py` & `labgrid-24.0a1/labgrid/driver/power/netio_kshell.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/rest.py` & `labgrid-24.0a1/labgrid/driver/power/rest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/sentry.py` & `labgrid-24.0a1/labgrid/driver/power/sentry.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/shelly_gen1.py` & `labgrid-24.0a1/labgrid/driver/power/shelly_gen1.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/siglent.py` & `labgrid-24.0a1/labgrid/driver/power/siglent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/simplerest.py` & `labgrid-24.0a1/labgrid/driver/power/simplerest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/power/tplink.py` & `labgrid-24.0a1/labgrid/driver/power/tplink.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/powerdriver.py` & `labgrid-24.0a1/labgrid/driver/powerdriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     bindings = {"port": {"SiSPMPowerPort", "NetworkSiSPMPowerPort"}, }
     delay = attr.ib(default=2.0, validator=attr.validators.instance_of(float))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('sispmctl') or 'sispmctl'
+            self.tool = self.target.env.config.get_tool('sispmctl')
         else:
             self.tool = 'sispmctl'
 
     def _get_sispmctl_prefix(self):
         return self.port.command_prefix + [
             self.tool,
             "-U", f"{self.port.busnum:03d}:{self.port.devnum:03d}",
@@ -267,60 +267,88 @@
     def get(self):
         return self.output.get()
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class YKUSHPowerDriver(Driver, PowerResetMixin, PowerProtocol):
     """YKUSHPowerDriver - Driver using a YEPKIT YKUSH switchable USB hub
-        to control a target's power - https://www.yepkit.com/products/ykush"""
-    bindings = {"port": "YKUSHPowerPort", }
+        to control a target's power - https://www.yepkit.com/products/ykush.
+        Uses ykushcmd tool to control the hub."""
+    bindings = {"port": {"YKUSHPowerPort", "NetworkYKUSHPowerPort"} }
     delay = attr.ib(default=2.0, validator=attr.validators.instance_of(float))
 
-
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        # uses the YKUSH pykush interface from here:
-        # https://github.com/Yepkit/pykush
-        self.pykush_mod = import_module('pykush.pykush')
-        self.pykush = self.pykush_mod.YKUSH(serial=self.port.serial)
+        if self.target.env:
+            self.tool = self.target.env.config.get_tool('ykushcmd') or 'ykushcmd'
+        else:
+            self.tool = 'ykushcmd'
 
     @Driver.check_active
     @step()
     def on(self):
-        self.pykush.set_port_state(self.port.index, self.pykush_mod.YKUSH_PORT_STATE_UP)
+        cmd = [
+            self.tool,
+            "-s", f"{self.port.serial}",
+            "-u", f"{self.port.index}"
+        ]
+        processwrapper.check_output(self.port.command_prefix + cmd)
 
     @Driver.check_active
     @step()
     def off(self):
-        self.pykush.set_port_state(self.port.index, self.pykush_mod.YKUSH_PORT_STATE_DOWN)
+        cmd = [
+            self.tool,
+            "-s", f"{self.port.serial}",
+            "-d", f"{self.port.index}"
+        ]
+        processwrapper.check_output(self.port.command_prefix + cmd)
 
     @Driver.check_active
     @step()
     def cycle(self):
         self.off()
         time.sleep(self.delay)
         self.on()
 
     @Driver.check_active
     def get(self):
-        return self.pykush.get_port_state(self.port.index)
+        cmd = [
+            self.tool,
+            "-s", f"{self.port.serial}",
+            "-g", f"{self.port.index}"
+        ]
+        res = processwrapper.check_output(self.port.command_prefix + cmd)
+        res = res.decode("utf-8")
+
+        # the example of ykushcmd -g like below:
+        # cmd: ykushcmd -g 1
+        # output: Downstream port 1 is ON/OFF
+        check_str = "Downstream port {port} is {status}"
+        if check_str.format(port=self.port.index, status="ON") in res:
+            return True
+        if check_str.format(port=self.port.index, status="OFF") in res:
+            return False
+
+        raise ExecutionError(f"Could not find port string in ykushcmd output: {res}")
+
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class USBPowerDriver(Driver, PowerResetMixin, PowerProtocol):
     """USBPowerDriver - Driver using a power switchable USB hub and the uhubctl
     tool (https://github.com/mvp/uhubctl) to control a target's power"""
 
     bindings = {"hub": {"USBPowerPort", "NetworkUSBPowerPort"}, }
     delay = attr.ib(default=2.0, validator=attr.validators.instance_of(float))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('uhubctl') or 'uhubctl'
+            self.tool = self.target.env.config.get_tool('uhubctl')
         else:
             self.tool = 'uhubctl'
 
     def _switch(self, cmd):
         cmd = self.hub.command_prefix + [
             self.tool,
             "-l", self.hub.path,
@@ -392,26 +420,23 @@
         self._host, self._port = proxymanager.get_host_and_port(self.port, default_port=16421)
 
     @Driver.check_active
     @step()
     def on(self):
         r = self._requests.get(self._build_url('on'))
         r.raise_for_status()
-        time.sleep(1)  # give pdudaemon some time to execute the request
 
     @Driver.check_active
     @step()
     def off(self):
         r = self._requests.get(self._build_url('off'))
         r.raise_for_status()
-        time.sleep(1)  # give pdudaemon some time to execute the request
 
     @Driver.check_active
     @step()
     def cycle(self):
         r = self._requests.get(self._build_url('reboot'))
         r.raise_for_status()
-        time.sleep(self.delay + 1)  # give pdudaemon some time to execute the request
 
     @Driver.check_active
     def get(self):
-        return None
+        raise NotImplementedError("pdudaemon does not support retrieving the port's state")
```

### Comparing `labgrid-23.1a2/labgrid/driver/pyvisadriver.py` & `labgrid-24.0a1/labgrid/driver/pyvisadriver.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             bindings (dict): driver to use with PyVISA
         """
     bindings = {"pyvisa_resource": "PyVISADevice"}
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         _py_pyvisa_module = import_module('pyvisa')
-        self._pyvisa_resource_manager = _py_pyvisa_module.ResourceManager()
+        self._pyvisa_resource_manager = _py_pyvisa_module.ResourceManager(self.pyvisa_resource.backend)
         self.pyvisa_device = None
 
     def on_activate(self):
         device_identifier = f'{self.pyvisa_resource.type}::{self.pyvisa_resource.url}::INSTR'
         self.pyvisa_device = self._pyvisa_resource_manager.open_resource(device_identifier)
 
     def on_deactivate(self):
```

### Comparing `labgrid-23.1a2/labgrid/driver/quartushpsdriver.py` & `labgrid-24.0a1/labgrid/driver/quartushpsdriver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import subprocess
 import re
 import time
-import logging
 
 import attr
 
 from ..factory import target_factory
 from ..step import step
 from .common import Driver
 from .exception import ExecutionError
@@ -24,20 +23,19 @@
     image = attr.ib(
         default=None,
         validator=attr.validators.optional(attr.validators.instance_of(str))
     )
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}({self.target})")
 
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('quartus_hps') or 'quartus_hps'
-            self.jtag_tool = self.target.env.config.get_tool('jtagconfig') or 'jtagconfig'
+            self.tool = self.target.env.config.get_tool('quartus_hps')
+            self.jtag_tool = self.target.env.config.get_tool('jtagconfig')
         else:
             self.tool = 'quartus_hps'
             self.jtag_tool = 'jtagconfig'
 
     def _get_cable_number(self):
         """
         Returns the JTAG cable number with an intact JTAG chain for the USB path of the device.
```

### Comparing `labgrid-23.1a2/labgrid/driver/resetdriver.py` & `labgrid-24.0a1/labgrid/driver/resetdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/serialdigitaloutput.py` & `labgrid-24.0a1/labgrid/driver/serialdigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/serialdriver.py` & `labgrid-24.0a1/labgrid/driver/serialdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import logging
-
 import attr
 from pexpect import TIMEOUT
 import serial
 import serial.rfc2217
 
 from ..factory import target_factory
 from ..protocol import ConsoleProtocol
@@ -22,15 +20,14 @@
     bindings = {"port": {"SerialPort", "NetworkSerialPort"}, }
 
     txdelay = attr.ib(default=0.0, validator=attr.validators.instance_of(float))
     timeout = attr.ib(default=3.0, validator=attr.validators.instance_of(float))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}({self.target})")
         if isinstance(self.port, SerialPort):
             self.serial = serial.Serial()
         else:
             if self.port.protocol == "rfc2217":
                 self.serial = serial.rfc2217.Serial()
             elif self.port.protocol == "raw":
                 self.serial = serial.serial_for_url("socket://", do_not_open=True)
@@ -95,15 +92,15 @@
 
         Arguments:
         data -- data to write, must be bytes
         """
         return self.serial.write(data)
 
     def open(self):
-        """Opens the serialport, does nothing if it is already closed"""
+        """Opens the serialport, does nothing if it is already open"""
         if not self.status:
             try:
                 self.serial.open()
             except serial.SerialException as e:
                 raise serial.SerialException(
                     f"Could not open serial port {self.serial.port}: {str(e)}") from e
```

### Comparing `labgrid-23.1a2/labgrid/driver/shelldriver.py` & `labgrid-24.0a1/labgrid/driver/shelldriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # pylint: disable=unused-argument
 """The ShellDriver provides the CommandProtocol, ConsoleProtocol and
  InfoProtocol on top of a SerialPort."""
 import io
-import logging
 import re
 import shlex
 import ipaddress
 
 import attr
 from pexpect import TIMEOUT
 import xmodem
@@ -44,25 +43,24 @@
             before check for a prompt. Useful when the console is interleaved with boot
             output which may interrupt prompt detection.
     """
     bindings = {"console": ConsoleProtocol, }
     prompt = attr.ib(validator=attr.validators.instance_of(str))
     login_prompt = attr.ib(validator=attr.validators.instance_of(str))
     username = attr.ib(validator=attr.validators.instance_of(str))
-    password = attr.ib(default="", validator=attr.validators.instance_of(str))
+    password = attr.ib(default=None, validator=attr.validators.optional(attr.validators.instance_of(str)))
     keyfile = attr.ib(default="", validator=attr.validators.instance_of(str))
     login_timeout = attr.ib(default=60, validator=attr.validators.instance_of(int))
     console_ready = attr.ib(default="", validator=attr.validators.instance_of(str))
     await_login_timeout = attr.ib(default=2, validator=attr.validators.instance_of(int))
     post_login_settle_time = attr.ib(default=0, validator=attr.validators.instance_of(int))
 
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}:{self.target}")
         self._status = 0
 
         self._xmodem_cached_rx_cmd = ""
         self._xmodem_cached_sx_cmd = ""
 
     def on_activate(self):
         if self._status == 0:
@@ -139,24 +137,24 @@
                 if did_login and not did_silence_kernel:
                     # Silence the kernel and wait for another prompt
                     self.console.sendline("dmesg -n 1")
                     did_silence_kernel = True
                 else:
                     # we got a prompt. no need for any further action to
                     # activate this driver.
-                    self.status = 1
+                    self._status = 1
                     break
 
             elif index == 1:
                 # we need to login
                 self.console.sendline(self.username)
                 did_login = True
 
             elif index == 2:
-                if self.password:
+                if self.password is not None:
                     self.console.sendline(self.password)
                 else:
                     raise Exception("Password entry needed but no password set")
 
             elif index == 3:
                 # expect hit a timeout while waiting for a match
                 if before == last_before:
@@ -307,15 +305,15 @@
         Start transfer command and synchronize until start of XMODEM stream.
 
         We don't use _run() here because it expects a prompt, but we want to
         read from the console directly into our XMODEM instance instead.
         """
 
         marker = gen_marker()
-        marked_cmd = f"echo '{marker[:4]}''{marker[4:]}'; {cmd}"
+        marked_cmd = f"echo -n '{marker[:4]}''{marker[4:]}'; {cmd}"
         self.console.sendline(marked_cmd)
         self.console.expect(marker, timeout=30)
 
     def _get_xmodem_rx_cmd(self, filename):
         """ Detect which XMODEM receive command can be used on the target, and cache the result. """
         if not self._xmodem_cached_rx_cmd:
             if self._run('which lrz')[2] == 0:
```

### Comparing `labgrid-23.1a2/labgrid/driver/smallubootdriver.py` & `labgrid-24.0a1/labgrid/driver/smallubootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/sshdriver.py` & `labgrid-24.0a1/labgrid/driver/sshdriver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """The SSHDriver uses SSH as a transport to implement CommandProtocol and FileTransferProtocol"""
 import contextlib
-import logging
 import os
 import re
 import stat
 import shlex
 import shutil
 import subprocess
 import tempfile
 import time
+from functools import cached_property
 
 import attr
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, FileTransferProtocol
 from .commandmixin import CommandMixin
 from .common import Driver
@@ -30,28 +30,38 @@
     """SSHDriver - Driver to execute commands via SSH"""
     bindings = {"networkservice": "NetworkService", }
     priorities = {CommandProtocol: 10, FileTransferProtocol: 10}
     keyfile = attr.ib(default="", validator=attr.validators.instance_of(str))
     stderr_merge = attr.ib(default=False, validator=attr.validators.instance_of(bool))
     connection_timeout = attr.ib(default=float(get_ssh_connect_timeout()), validator=attr.validators.instance_of(float))
     explicit_sftp_mode = attr.ib(default=False, validator=attr.validators.instance_of(bool))
+    explicit_scp_mode = attr.ib(default=False, validator=attr.validators.instance_of(bool))
+    username = attr.ib(default="", validator=attr.validators.instance_of(str))
+    password = attr.ib(default="", validator=attr.validators.instance_of(str))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}({self.target})")
         self._keepalive = None
 
+    def _get_username(self):
+        """Get the username from this class or from NetworkService"""
+        return self.username or self.networkservice.username
+
+    def _get_password(self):
+        """Get the password from this class or from NetworkService"""
+        return self.password or self.networkservice.password
+
     def on_activate(self):
         self.ssh_prefix = ["-o", "LogLevel=ERROR"]
         if self.keyfile:
             keyfile_path = self.keyfile
             if self.target.env:
                 keyfile_path = self.target.env.config.resolve_path(self.keyfile)
             self.ssh_prefix += ["-i", keyfile_path ]
-        if not self.networkservice.password:
+        if not self._get_password():
             self.ssh_prefix += ["-o", "PasswordAuthentication=no"]
 
         self.control = self._start_own_master()
         self.ssh_prefix += ["-F", "none"]
         if self.control:
             self.ssh_prefix += ["-o", f"ControlPath={self.control.replace('%', '%%')}"]
 
@@ -95,15 +105,15 @@
             self.tmpdir, f'control-{self.networkservice.address}'
         )
 
         args = ["ssh", "-f", *self.ssh_prefix, "-x", "-o", f"ConnectTimeout={timeout}",
                  "-o", "ControlPersist=300", "-o",
                  "UserKnownHostsFile=/dev/null", "-o", "StrictHostKeyChecking=no",
                  "-o", "ServerAliveInterval=15", "-MN", "-S", control.replace('%', '%%'), "-p",
-                 str(self.networkservice.port), "-l", self.networkservice.username,
+                 str(self.networkservice.port), "-l", self._get_username(),
                  self.networkservice.address]
 
         # proxy via the exporter if we have an ifname suffix
         address = self.networkservice.address
         if address.count('%') > 1:
             raise ValueError(f"Multiple '%' found in '{address}'.")
         if '%' in address:
@@ -115,22 +125,22 @@
         if proxy_cmd:  # only proxy if needed
             args += [
                 "-o", f"ProxyCommand={' '.join(proxy_cmd)} 2>{self.tmpdir}/proxy-stderr"
             ]
 
         env = os.environ.copy()
         pass_file = ''
-        if self.networkservice.password:
+        if self._get_password():
             fd, pass_file = tempfile.mkstemp()
             os.fchmod(fd, stat.S_IRWXU)
             #with openssh>=8.4 SSH_ASKPASS_REQUIRE can be used to force SSH_ASK_PASS
             #openssh<8.4 requires the DISPLAY var and a detached process with start_new_session=True
             env = {'SSH_ASKPASS': pass_file, 'DISPLAY':'', 'SSH_ASKPASS_REQUIRE':'force'}
             with open(fd, 'w') as f:
-                f.write("#!/bin/sh\necho " + shlex.quote(self.networkservice.password))
+                f.write("#!/bin/sh\necho " + shlex.quote(self._get_password()))
 
         self.process = subprocess.Popen(args, env=env,
                                         stdout=subprocess.PIPE,
                                         stderr=subprocess.STDOUT,
                                         stdin=subprocess.DEVNULL,
                                         start_new_session=True)
 
@@ -159,15 +169,15 @@
                     stdout=stdout,
                 )
         except subprocess.TimeoutExpired:
             raise ExecutionError(
                 f"Subprocess timed out [{subprocess_timeout}s] while executing {args}",
             )
         finally:
-            if self.networkservice.password and os.path.exists(pass_file):
+            if self._get_password() and os.path.exists(pass_file):
                 os.remove(pass_file)
 
         if not os.path.exists(control):
             raise ExecutionError(
                 f"no control socket to {self.networkservice.address}"
             )
 
@@ -190,25 +200,25 @@
         returns:
         (stdout, stderr, returncode)
         """
         if not self._check_keepalive():
             raise ExecutionError("Keepalive no longer running")
 
         complete_cmd = ["ssh", "-x", *self.ssh_prefix,
-                        "-p", str(self.networkservice.port), "-l", self.networkservice.username,
+                        "-p", str(self.networkservice.port), "-l", self._get_username(),
                         self.networkservice.address
                         ] + cmd.split(" ")
         self.logger.debug("Sending command: %s", complete_cmd)
         if self.stderr_merge:
             stderr_pipe = subprocess.STDOUT
         else:
             stderr_pipe = subprocess.PIPE
         try:
             sub = subprocess.Popen(
-                complete_cmd, stdout=subprocess.PIPE, stderr=stderr_pipe
+                complete_cmd, stdin=subprocess.DEVNULL, stdout=subprocess.PIPE, stderr=stderr_pipe
             )
         except:
             raise ExecutionError(
                 f"error executing command: {complete_cmd}"
             )
 
         stdout, stderr = sub.communicate(timeout=timeout)
@@ -307,14 +317,42 @@
             raise ExecutionError("Keepalive no longer running")
 
         forward = f"-R{remoteport:d}:localhost:{localport:d}"
         with self._forward(forward):
             yield
 
     @Driver.check_active
+    @contextlib.contextmanager
+    def forward_unix_socket(self, unixsocket, localport=None):
+        """Forward a unix socket on the target to a local port
+
+        A context manager that keeps a unix socket forwarded to a local port as
+        long as the context remains valid. A connection can be made to the
+        remote socket on the target device will be forwarded to the returned
+        local port on localhost
+
+        usage:
+            with ssh.forward_unix_socket("/run/docker.sock") as localport:
+                # Use localhost:localport here to connect to the socket on the
+                # target
+
+        returns:
+        localport
+        """
+        if not self._check_keepalive():
+            raise ExecutionError("Keepalive no longer running")
+
+        if localport is None:
+            localport = get_free_port()
+
+        forward = f"-L{localport:d}:{unixsocket:s}"
+        with self._forward(forward):
+            yield localport
+
+    @Driver.check_active
     @step(args=['src', 'dst'])
     def scp(self, *, src, dst):
         if not self._check_keepalive():
             raise ExecutionError("Keepalive no longer running")
 
         if src.startswith(':') == dst.startswith(':'):
             raise ValueError("Either source or destination must be remote (start with :)")
@@ -324,14 +362,20 @@
             dst = '_' + dst
 
         complete_cmd = ["scp",
                 "-F", "none",
                 "-o", f"ControlPath={self.control.replace('%', '%%')}",
                 src, dst,
         ]
+        
+        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
+            complete_cmd.insert(1, "-s")
+        if self.explicit_scp_mode and self._scp_supports_explicit_scp_mode():
+            complete_cmd.insert(1, "-O")
+
         self.logger.info("Running command: %s", complete_cmd)
         sub = subprocess.Popen(
             complete_cmd,
         )
         return sub.wait()
 
     @Driver.check_active
@@ -395,42 +439,56 @@
 
         sub.wait()
 
     def get_status(self):
         """The SSHDriver is always connected, return 1"""
         return 1
 
-    def _scp_supports_explicit_sftp_mode(self):
+    @cached_property
+    def _ssh_version(self):
         version = subprocess.run(["ssh", "-V"], capture_output=True, text=True)
         version = re.match(r"^OpenSSH_(\d+)\.(\d+)", version.stderr)
-        major, minor = map(int, version.groups())
+        return tuple(int(x) for x in version.groups())
+
+    def _scp_supports_explicit_sftp_mode(self):
+        major, minor = self._ssh_version
 
         # OpenSSH >= 8.6 supports explicitly using the SFTP protocol via -s
         if major == 8 and minor >= 6:
             return True
         # OpenSSH >= 9.0 default to the SFTP protocol
         if major >= 9:
             return False
         raise Exception(f"OpenSSH version {major}.{minor} does not support explicit SFTP mode")
 
+    def _scp_supports_explicit_scp_mode(self):
+        major, minor = self._ssh_version
+
+        # OpenSSH >= 9.0 default to the SFTP protocol
+        if major >= 9:
+            return True
+        raise Exception(f"OpenSSH version {major}.{minor} does not support explicit SCP mode")
+
     @Driver.check_active
     @step(args=['filename', 'remotepath'])
     def put(self, filename, remotepath=''):
-        ssh_prefix = self.ssh_prefix
-        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
-            ssh_prefix.append("-s")
         transfer_cmd = [
             "scp",
-            *ssh_prefix,
+            *self.ssh_prefix,
             "-P", str(self.networkservice.port),
             "-r",
             filename,
-            f"{self.networkservice.username}@{self.networkservice.address}:{remotepath}"
+            f"{self._get_username()}@{self.networkservice.address}:{remotepath}"
             ]
 
+        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
+            transfer_cmd.insert(1, "-s")
+        if self.explicit_scp_mode and self._scp_supports_explicit_scp_mode():
+            transfer_cmd.insert(1, "-O")
+
         try:
             sub = subprocess.call(
                 transfer_cmd
             )  #, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         except:
             raise ExecutionError(
                 f"error executing command: {transfer_cmd}"
@@ -439,26 +497,28 @@
             raise ExecutionError(
                 f"error executing command: {transfer_cmd}"
             )
 
     @Driver.check_active
     @step(args=['filename', 'destination'])
     def get(self, filename, destination="."):
-        ssh_prefix = self.ssh_prefix
-        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
-            ssh_prefix.append("-s")
         transfer_cmd = [
             "scp",
-            *ssh_prefix,
+            *self.ssh_prefix,
             "-P", str(self.networkservice.port),
             "-r",
-            f"{self.networkservice.username}@{self.networkservice.address}:{filename}",
+            f"{self._get_username()}@{self.networkservice.address}:{filename}",
             destination
             ]
 
+        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
+            transfer_cmd.insert(1, "-s")
+        if self.explicit_scp_mode and self._scp_supports_explicit_scp_mode():
+            transfer_cmd.insert(1, "-O")
+
         try:
             sub = subprocess.call(
                 transfer_cmd
             )  #, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         except:
             raise ExecutionError(
                 f"error executing command: {transfer_cmd}"
@@ -466,52 +526,61 @@
         if sub != 0:
             raise ExecutionError(
                 f"error executing command: {transfer_cmd}"
             )
 
     def _cleanup_own_master(self):
         """Exit the controlmaster and delete the tmpdir"""
-        complete_cmd = f"ssh -x -o ControlPath={self.control.replace('%', '%%')} -O exit -p {self.networkservice.port} -l {self.networkservice.username} {self.networkservice.address}".split(' ')  # pylint: disable=line-too-long
+        complete_cmd = f"ssh -x -o ControlPath={self.control.replace('%', '%%')} -O exit -p {self.networkservice.port} -l {self._get_username()} {self.networkservice.address}".split(' ')  # pylint: disable=line-too-long
         res = subprocess.call(
             complete_cmd,
             stdin=subprocess.DEVNULL,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL
         )
 
         if res != 0:
             self.logger.info("Socket already closed")
-        shutil.rmtree(self.tmpdir)
 
         self.process.communicate()
 
+        shutil.rmtree(self.tmpdir, ignore_errors=True)
+
     def _start_keepalive(self):
         """Starts a keepalive connection via the own or external master."""
         args = ["ssh", *self.ssh_prefix, self.networkservice.address, "cat"]
 
         assert self._keepalive is None
         self._keepalive = subprocess.Popen(
             args,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            encoding="utf-8",
         )
 
         self.logger.debug('Started keepalive for %s', self.networkservice.address)
 
     def _check_keepalive(self):
         return self._keepalive.poll() is None
 
     def _stop_keepalive(self):
         assert self._keepalive is not None
 
         self.logger.debug('Stopping keepalive for %s', self.networkservice.address)
 
+        stdout = None
         try:
-            self._keepalive.communicate(timeout=60)
+            stdout, _ = self._keepalive.communicate(timeout=60)
         except subprocess.TimeoutExpired:
             self._keepalive.kill()
-
-        try:
-            self._keepalive.wait(timeout=60)
+            try:
+                # Try again to get output
+                stdout, _ = self._keepalive.communicate(timeout=60)
+            except subprocess.TimeoutExpired:
+                self.logger.warning("ssh keepalive for %s timed out during termination", self.networkservice.address)
         finally:
             self._keepalive = None
+
+        if stdout:
+            for line in stdout.splitlines():
+                self.logger.warning("Keepalive %s: %s", self.networkservice.address, line)
```

### Comparing `labgrid-23.1a2/labgrid/driver/ubootdriver.py` & `labgrid-24.0a1/labgrid/driver/ubootdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """The U-Boot Module contains the UBootDriver"""
-import logging
-
 import attr
 from pexpect import TIMEOUT
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, ConsoleProtocol, LinuxBootProtocol
 from ..util import gen_marker, Timeout, re_vt100
 from ..step import step
@@ -44,15 +42,14 @@
     boot_command = attr.ib(default="run bootcmd", validator=attr.validators.instance_of(str))
     boot_commands = attr.ib(default=attr.Factory(dict), validator=attr.validators.instance_of(dict))
     login_timeout = attr.ib(default=30, validator=attr.validators.instance_of(int))
     boot_timeout = attr.ib(default=30, validator=attr.validators.instance_of(int))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}:{self.target}")
         self._status = 0
 
         if self.boot_expression:
             import warnings
             warnings.warn("boot_expression is deprecated and will be ignored", DeprecationWarning)
 
     def on_activate(self):
```

### Comparing `labgrid-23.1a2/labgrid/driver/usbaudiodriver.py` & `labgrid-24.0a1/labgrid/driver/usbaudiodriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import subprocess
 import attr
 
 from .common import Driver
 from ..factory import target_factory
 from ..step import step
 
@@ -24,15 +23,14 @@
     """
     bindings = {
         "res": {"USBAudioInput", "NetworkUSBAudioInput"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}")
         self._prepared = False
 
     def _get_pipeline(self):
         return [
             "alsasrc", f"device={self.res.alsa_name}", "!",
             "matroskamux", "streamable=true", "!",
             "fdsink"
```

### Comparing `labgrid-23.1a2/labgrid/driver/usbhidrelay.py` & `labgrid-24.0a1/labgrid/driver/usbhidrelay.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/usbloader.py` & `labgrid-24.0a1/labgrid/driver/usbloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     image = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('mxs-usb-loader') or 'mxs-usb-loader'
+            self.tool = self.target.env.config.get_tool('mxs-usb-loader')
         else:
             self.tool = 'mxs-usb-loader'
 
     def on_activate(self):
         pass
 
     def on_deactivate(self):
@@ -38,15 +38,16 @@
     def load(self, filename=None):
         if filename is None and self.image is not None:
             filename = self.target.env.config.get_image_path(self.image)
         mf = ManagedFile(filename, self.loader)
         mf.sync_to_resource()
 
         processwrapper.check_output(
-            self.loader.command_prefix + [self.tool, "0", mf.get_remote_path()]
+            self.loader.command_prefix + [self.tool, "0", mf.get_remote_path()],
+            print_on_silent_log=True
         )
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class IMXUSBDriver(Driver, BootstrapProtocol):
     bindings = {
@@ -55,15 +56,15 @@
 
     image = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('imx-usb-loader') or 'imx-usb-loader'
+            self.tool = self.target.env.config.get_tool('imx-usb-loader')
         else:
             self.tool = 'imx-usb-loader'
 
     def on_activate(self):
         pass
 
     def on_deactivate(self):
@@ -75,15 +76,16 @@
         if filename is None and self.image is not None:
             filename = self.target.env.config.get_image_path(self.image)
         mf = ManagedFile(filename, self.loader)
         mf.sync_to_resource()
 
         processwrapper.check_output(
             self.loader.command_prefix +
-            [self.tool, "-p", str(self.loader.path), "-c", mf.get_remote_path()]
+            [self.tool, "-p", str(self.loader.path), "-c", mf.get_remote_path()],
+            print_on_silent_log=True
         )
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class RKUSBDriver(Driver, BootstrapProtocol):
     bindings = {
@@ -93,15 +95,15 @@
     image = attr.ib(default=None)
     usb_loader = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('rk-usb-loader') or 'rk-usb-loader'
+            self.tool = self.target.env.config.get_tool('rk-usb-loader')
         else:
             self.tool = 'rk-usb-loader'
 
     def on_activate(self):
         pass
 
     def on_deactivate(self):
@@ -116,15 +118,16 @@
             mf.sync_to_resource()
 
         timeout = Timeout(3.0)
         while True:
             try:
                 processwrapper.check_output(
                     self.loader.command_prefix +
-                    [self.tool, 'db', mf.get_remote_path()]
+                    [self.tool, 'db', mf.get_remote_path()],
+                    print_on_silent_log=True
                 )
                 break
             except subprocess.CalledProcessError:
                 if timeout.expired:
                     raise
 
         if filename is None and self.image is not None:
@@ -133,15 +136,16 @@
         mf.sync_to_resource()
 
         timeout = Timeout(3.0)
         while True:
             try:
                 processwrapper.check_output(
                     self.loader.command_prefix +
-                    [self.tool, 'wl', '0x40', mf.get_remote_path()]
+                    [self.tool, 'wl', '0x40', mf.get_remote_path()],
+                    print_on_silent_log=True
                 )
                 break
             except subprocess.CalledProcessError:
                 if timeout.expired:
                     raise
 
 
@@ -155,15 +159,15 @@
     image = attr.ib(default=None)
     script = attr.ib(default='', validator=attr.validators.instance_of(str))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('uuu-loader') or 'uuu-loader'
+            self.tool = self.target.env.config.get_tool('uuu-loader')
         else:
             self.tool = 'uuu-loader'
 
     def on_activate(self):
         pass
 
     def on_deactivate(self):
@@ -176,15 +180,16 @@
             filename = self.target.env.config.get_image_path(self.image)
         mf = ManagedFile(filename, self.loader)
         mf.sync_to_resource()
 
         cmd = ['-b', self.script] if self.script else []
 
         processwrapper.check_output(
-            self.loader.command_prefix + [self.tool] + cmd + [mf.get_remote_path()]
+            self.loader.command_prefix + [self.tool] + cmd + [mf.get_remote_path()],
+            print_on_silent_log=True
         )
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class BDIMXUSBDriver(Driver, BootstrapProtocol):
     """
@@ -199,15 +204,15 @@
         "loader": {"IMXUSBLoader", "NetworkIMXUSBLoader"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('imx_usb') or 'imx_usb'
+            self.tool = self.target.env.config.get_tool('imx_usb')
         else:
             self.tool = 'imx_usb'
 
     def on_activate(self):
         pass
 
     def on_deactivate(self):
@@ -221,9 +226,10 @@
 
         processwrapper.check_output(
             self.loader.command_prefix + [
                 self.tool,
                 f"--bus={self.loader.busnum}",
                 f"--device={self.loader.devnum}",
                 mf.get_remote_path(),
-            ]
+            ],
+            print_on_silent_log=True
         )
```

### Comparing `labgrid-23.1a2/labgrid/driver/usbsdmuxdriver.py` & `labgrid-24.0a1/labgrid/driver/usbsdmuxdriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     bindings = {
         "mux": {"USBSDMuxDevice", "NetworkUSBSDMuxDevice"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('usbsdmux') or 'usbsdmux'
+            self.tool = self.target.env.config.get_tool('usbsdmux')
         else:
             self.tool = 'usbsdmux'
 
     @Driver.check_active
     @step(title='sdmux_set', args=['mode'])
     def set_mode(self, mode):
         if not mode.lower() in ['dut', 'host', 'off', 'client']:
```

### Comparing `labgrid-23.1a2/labgrid/driver/usbsdwiredriver.py` & `labgrid-24.0a1/labgrid/driver/usbsdwiredriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     bindings = {
         "mux": {"USBSDWireDevice", "NetworkUSBSDWireDevice"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('sd-mux-ctrl') or 'sd-mux-ctrl'
+            self.tool = self.target.env.config.get_tool('sd-mux-ctrl')
         else:
             self.tool = 'sd-mux-ctrl'
 
     @Driver.check_active
     @step(title='sdmux_set', args=['mode'])
     def set_mode(self, mode):
         if not mode.lower() in ['dut', 'host']:
```

### Comparing `labgrid-23.1a2/labgrid/driver/usbtmc/keysight_dsox2000.py` & `labgrid-24.0a1/labgrid/driver/usbtmc/keysight_dsox2000.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/usbtmc/tektronix_tds2000.py` & `labgrid-24.0a1/labgrid/driver/usbtmc/tektronix_tds2000.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/usbtmcdriver.py` & `labgrid-24.0a1/labgrid/driver/usbtmcdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/driver/usbvideodriver.py` & `labgrid-24.0a1/labgrid/driver/usbvideodriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import subprocess
 
 import attr
 
 from ..exceptions import InvalidConfigError
 from ..factory import target_factory
 from ..protocol import VideoProtocol
@@ -14,15 +13,14 @@
 class USBVideoDriver(Driver, VideoProtocol):
     bindings = {
         "video": {"USBVideo", "NetworkUSBVideo"},
     }
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}")
         self._prepared = False
 
     def get_qualities(self):
         match = (self.video.vendor_id, self.video.model_id)
         if match == (0x046d, 0x082d):
             return ("mid", [
                 ("low", "video/x-h264,width=640,height=360,framerate=5/1"),
@@ -129,15 +127,15 @@
     def stream(self, caps_hint=None, controls=None):
         caps = self.select_caps(caps_hint)
         pipeline = self.get_pipeline(self.video.path, caps, controls)
 
         tx_cmd = self.video.command_prefix + ["gst-launch-1.0", "-q"]
         tx_cmd += pipeline.split()
         rx_cmd = ["gst-launch-1.0"]
-        rx_cmd += "playbin uri=fd://0".split()
+        rx_cmd += "playbin3 uri=fd://0".split()
 
         tx = subprocess.Popen(
             tx_cmd,
             stdin=subprocess.DEVNULL,
             stdout=subprocess.PIPE,
         )
         rx = subprocess.Popen(
```

### Comparing `labgrid-23.1a2/labgrid/driver/xenadriver.py` & `labgrid-24.0a1/labgrid/driver/xenadriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from importlib import import_module
 import attr
 
 from ..factory import target_factory
 from .common import Driver
 
 @target_factory.reg_driver
@@ -13,19 +12,18 @@
     """
     bindings = {"xena_manager": "XenaManager"}
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self._xena_app = import_module('xenavalkyrie.xena_app')
         self._tgn_utils = import_module('trafficgenerator.tgn_utils')
-        self._logger = logging.getLogger(f"{self}")
         self._xm = None
 
     def on_activate(self):
-        self._xm = self._xena_app.init_xena(self._tgn_utils.ApiType.socket, self._logger, 'labgrid')
+        self._xm = self._xena_app.init_xena(self._tgn_utils.ApiType.socket, self.logger, 'labgrid')
         self._xm.session.add_chassis(self.xena_manager.hostname)
 
     def on_deactivate(self):
         if self._xm:
             self._xm.session.disconnect()
             self._xm = None
```

### Comparing `labgrid-23.1a2/labgrid/environment.py` & `labgrid-24.0a1/labgrid/environment.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/exceptions.py` & `labgrid-24.0a1/labgrid/exceptions.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/factory.py` & `labgrid-24.0a1/labgrid/factory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/logging.py` & `labgrid-24.0a1/labgrid/logging.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/protocol/__init__.py` & `labgrid-24.0a1/labgrid/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/protocol/commandprotocol.py` & `labgrid-24.0a1/labgrid/protocol/commandprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/protocol/consoleprotocol.py` & `labgrid-24.0a1/labgrid/protocol/consoleprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/protocol/infoprotocol.py` & `labgrid-24.0a1/labgrid/protocol/infoprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/pytestplugin/fixtures.py` & `labgrid-24.0a1/labgrid/pytestplugin/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pytest
 
 from ..exceptions import NoResourceFoundError, NoDriverFoundError
 from ..remote.client import UserError
 from ..resource.remote import RemotePlace
 from ..util.ssh import sshmanager
 from ..logging import DEFAULT_FORMAT
+from .hooks import LABGRID_ENV_KEY
 
 # pylint: disable=redefined-outer-name
 
 
 def pytest_addoption(parser):
     group = parser.getgroup('labgrid')
     group.addoption(
@@ -56,15 +57,15 @@
 
 
 @pytest.fixture(scope="session")
 def env(request, record_testsuite_property):
     """Return the environment configured in the supplied configuration file.
     It contains the targets contained in the configuration file.
     """
-    env = request.config._labgrid_env
+    env = request.config.stash[LABGRID_ENV_KEY]
 
     if not env:
         pytest.skip("missing environment config (use --lg-env)")
 
     record_testsuite_property('ENV_CONFIG', env.config_file)
     targets = list(env.config.get_targets().keys())
     record_testsuite_property('TARGETS', targets)
```

### Comparing `labgrid-23.1a2/labgrid/pytestplugin/hooks.py` & `labgrid-24.0a1/labgrid/pytestplugin/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 import pytest
 
 from .. import Environment
 from ..consoleloggingreporter import ConsoleLoggingReporter
 from ..util.helper import processwrapper
 from ..logging import StepFormatter, StepLogger
 
+LABGRID_ENV_KEY = pytest.StashKey[Environment]()
+
+
 @pytest.hookimpl(tryfirst=True)
 def pytest_cmdline_main(config):
     def set_cli_log_level(level):
         nonlocal config
 
-        current_level = config.getoption("log_cli_level") or config.getini("log_cli_level")
+        try:
+            current_level = config.getoption("log_cli_level") or config.getini("log_cli_level")
+        except ValueError:
+            return
         print(f"current_level: {current_level}")
 
         if isinstance(current_level, str):
             try:
                 current_level = int(logging.getLevelName(current_level))
             except ValueError:
                 current_level = None
@@ -32,36 +38,40 @@
         set_cli_log_level(logging.DEBUG)
     elif verbosity > 2: # enable with -vvv
         set_cli_log_level(logging.CONSOLE)
     elif verbosity > 1: # enable with -vv
         set_cli_log_level(logging.INFO)
 
 
-@pytest.hookimpl(trylast=True)
-def pytest_configure(config):
-    StepLogger.start()
-    config.add_cleanup(StepLogger.stop)
-
-    logging_plugin = config.pluginmanager.getplugin('logging-plugin')
-    logging_plugin.log_cli_handler.formatter.add_color_level(logging.CONSOLE, "blue")
-    logging_plugin.log_cli_handler.setFormatter(StepFormatter(
+def configure_pytest_logging(config, plugin):
+    plugin.log_cli_handler.formatter.add_color_level(logging.CONSOLE, "blue")
+    plugin.log_cli_handler.setFormatter(StepFormatter(
         color=config.option.lg_colored_steps,
-        parent=logging_plugin.log_cli_handler.formatter,
+        parent=plugin.log_cli_handler.formatter,
     ))
-    logging_plugin.log_file_handler.setFormatter(StepFormatter(
-        parent=logging_plugin.log_file_handler.formatter,
+    plugin.log_file_handler.setFormatter(StepFormatter(
+        parent=plugin.log_file_handler.formatter,
     ))
 
     # Might be the same formatter instance, so get a reference for both before
     # changing either
-    report_formatter = logging_plugin.report_handler.formatter
-    caplog_formatter = logging_plugin.caplog_handler.formatter
+    report_formatter = plugin.report_handler.formatter
+    caplog_formatter = plugin.caplog_handler.formatter
 
-    logging_plugin.report_handler.setFormatter(StepFormatter(parent=report_formatter))
-    logging_plugin.report_handler.setFormatter(StepFormatter(parent=caplog_formatter))
+    plugin.report_handler.setFormatter(StepFormatter(parent=report_formatter))
+    plugin.report_handler.setFormatter(StepFormatter(parent=caplog_formatter))
+
+@pytest.hookimpl(trylast=True)
+def pytest_configure(config):
+    StepLogger.start()
+    config.add_cleanup(StepLogger.stop)
+
+    logging_plugin = config.pluginmanager.getplugin('logging-plugin')
+    if logging_plugin:
+        configure_pytest_logging(config, logging_plugin)
 
     config.addinivalue_line("markers",
                             "lg_feature: marker for labgrid feature flags")
     lg_log = config.option.lg_log
     if lg_log:
         ConsoleLoggingReporter(lg_log)
     env_config = config.option.env_config
@@ -78,23 +88,23 @@
     env = None
     if lg_env is None:
         lg_env = os.environ.get('LG_ENV')
     if lg_env is not None:
         env = Environment(config_file=lg_env)
         if lg_coordinator is not None:
             env.config.set_option('crossbar_url', lg_coordinator)
-    config._labgrid_env = env
+    config.stash[LABGRID_ENV_KEY] = env
 
     processwrapper.enable_logging()
 
 @pytest.hookimpl()
 def pytest_collection_modifyitems(config, items):
     """This function matches function feature flags with those found in the
     environment and disables the item if no match is found"""
-    env = config._labgrid_env
+    env = config.stash[LABGRID_ENV_KEY]
 
     if not env:
         return
 
     have_feature = env.get_features() | env.get_target_features()
 
     for item in items:
```

### Comparing `labgrid-23.1a2/labgrid/remote/client.py` & `labgrid-24.0a1/labgrid/remote/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """The remote.client module contains the functionality to connect to a
 coordinator, acquire a place and interact with the connected resources"""
 import argparse
 import asyncio
 import contextlib
 import enum
 import os
+import pathlib
 import subprocess
 import traceback
 import logging
 import signal
 import sys
 import shlex
 import json
@@ -19,25 +20,26 @@
 from datetime import datetime
 from pprint import pformat
 import txaio
 txaio.use_asyncio()
 from autobahn.asyncio.wamp import ApplicationSession
 
 from .common import (ResourceEntry, ResourceMatch, Place, Reservation, ReservationState, TAG_KEY,
-                     TAG_VAL, enable_tcp_nodelay)
+                     TAG_VAL, enable_tcp_nodelay, monkey_patch_max_msg_payload_size_ws_option)
 from .. import Environment, Target, target_factory
 from ..exceptions import NoDriverFoundError, NoResourceFoundError, InvalidConfigError
 from ..resource.remote import RemotePlaceManager, RemotePlace
-from ..util import diff_dict, flat_dict, filter_dict, dump, atomic_replace, Timeout
+from ..util import diff_dict, flat_dict, filter_dict, dump, atomic_replace, labgrid_version, Timeout
 from ..util.proxy import proxymanager
 from ..util.helper import processwrapper
 from ..driver import Mode, ExecutionError
 from ..logging import basicConfig, StepLogger
 
 txaio.config.loop = asyncio.get_event_loop()  # pylint: disable=no-member
+monkey_patch_max_msg_payload_size_ws_option()
 
 
 class Error(Exception):
     pass
 
 
 class UserError(Error):
@@ -113,21 +115,21 @@
             old = None
             group[resource_name] = ResourceEntry(resource)
         else:
             old = group[resource_name].data
             group[resource_name].data = resource
         if self.monitor:
             if resource and not old:
-                print(f"Resource {exporter}/{group_name}/{resource_name} created: {resource}")
+                print(f"Resource {exporter}/{group_name}/{resource['cls']}/{resource_name} created: {resource}")
             elif resource and old:
-                print(f"Resource {exporter}/{group_name}/{resource_name} changed:")
+                print(f"Resource {exporter}/{group_name}/{resource['cls']}/{resource_name} changed:")
                 for k, v_old, v_new in diff_dict(flat_dict(old), flat_dict(resource)):
                     print(f"  {k}: {v_old} -> {v_new}")
             else:
-                print(f"Resource {exporter}/{group_name}/{resource_name} deleted")
+                print(f"Resource {exporter}/{group_name}/???/{resource_name} deleted")
 
     async def on_place_changed(self, name, config):
         if not config:
             del self.places[name]
             if self.monitor:
                 print(f"Place {name} deleted")
             return
@@ -626,25 +628,25 @@
         print(f"allowed {self.args.user} for place {place.name}")
 
     def get_target_resources(self, place):
         self._check_allowed(place)
         resources = {}
         for resource_path in place.acquired_resources:
             match = place.getmatch(resource_path)
-            (exporter, group_name, _, resource_name) = resource_path
+            (exporter, group_name, cls, resource_name) = resource_path
             name = resource_name
             if match.rename:
                 name = match.rename
-            resources[name] = self.resources[exporter][group_name][resource_name]
+            resources[(name, cls)] = self.resources[exporter][group_name][resource_name]
         return resources
 
     def get_target_config(self, place):
         config = {}
         resources = config['resources'] = []
-        for name, resource in self.get_target_resources(place).items():
+        for (name, _), resource in self.get_target_resources(place).items():
             args = OrderedDict()
             if name != resource.cls:
                 args['name'] = name
             args.update(resource.args)
             resources.append({resource.cls: args})
         return config
 
@@ -721,31 +723,35 @@
         place = self.get_acquired_place()
         action = self.args.action
         delay = self.args.delay
         name = self.args.name
         target = self._get_target(place)
         from ..resource.power import NetworkPowerPort, PDUDaemonPort
         from ..resource.remote import NetworkUSBPowerPort, NetworkSiSPMPowerPort
-        from ..resource import TasmotaPowerPort
+        from ..resource import TasmotaPowerPort, NetworkYKUSHPowerPort
 
         drv = None
         try:
             drv = target.get_driver("PowerProtocol", name=name)
         except NoDriverFoundError:
             for resource in target.resources:
+                if name and resource.name != name:
+                    continue
                 if isinstance(resource, NetworkPowerPort):
                     drv = self._get_driver_or_new(target, "NetworkPowerDriver", name=name)
                 elif isinstance(resource, NetworkUSBPowerPort):
                     drv = self._get_driver_or_new(target, "USBPowerDriver", name=name)
                 elif isinstance(resource, NetworkSiSPMPowerPort):
                     drv = self._get_driver_or_new(target, "SiSPMPowerDriver", name=name)
                 elif isinstance(resource, PDUDaemonPort):
                     drv = self._get_driver_or_new(target, "PDUDaemonDriver", name=name)
                 elif isinstance(resource, TasmotaPowerPort):
                     drv = self._get_driver_or_new(target, "TasmotaPowerDriver", name=name)
+                elif isinstance(resource, NetworkYKUSHPowerPort):
+                    drv = self._get_driver_or_new(target, "YKUSHPowerDriver", name=name)
                 if drv:
                     break
 
         if not drv:
             raise UserError("target has no compatible resource available")
         if delay is not None:
             drv.delay = delay
@@ -754,27 +760,29 @@
             print(f"power{' ' + name if name else ''} for place {place.name} is {'on' if res else 'off'}")
 
     def digital_io(self):
         place = self.get_acquired_place()
         action = self.args.action
         name = self.args.name
         target = self._get_target(place)
-        from ..resource import ModbusTCPCoil, OneWirePIO
+        from ..resource import ModbusTCPCoil, OneWirePIO, HttpDigitalOutput
         from ..resource.remote import (NetworkDeditecRelais8, NetworkSysfsGPIO, NetworkLXAIOBusPIO,
                                        NetworkHIDRelay)
 
         drv = None
         try:
             drv = target.get_driver("DigitalOutputProtocol", name=name)
         except NoDriverFoundError:
             for resource in target.resources:
                 if isinstance(resource, ModbusTCPCoil):
                     drv = self._get_driver_or_new(target, "ModbusCoilDriver", name=name)
                 elif isinstance(resource, OneWirePIO):
                     drv = self._get_driver_or_new(target, "OneWirePIODriver", name=name)
+                elif isinstance(resource, HttpDigitalOutput):
+                    drv = self._get_driver_or_new(target, "HttpDigitalOutputDriver", name=name)
                 elif isinstance(resource, NetworkDeditecRelais8):
                     drv = self._get_driver_or_new(target, "DeditecRelaisDriver", name=name)
                 elif isinstance(resource, NetworkSysfsGPIO):
                     drv = self._get_driver_or_new(target, "GpioDigitalOutputDriver", name=name)
                 elif isinstance(resource, NetworkLXAIOBusPIO):
                     drv = self._get_driver_or_new(target, "LXAIOBusPIODriver", name=name)
                 elif isinstance(resource, NetworkHIDRelay):
@@ -803,14 +811,18 @@
             if resource.avail or (not loop and timeout.expired):
                 break
             await asyncio.sleep(0.1)
 
         # use zero timeout to prevent blocking sleeps
         target.await_resources([resource], timeout=0.0)
 
+        if not place.acquired:
+            print("place released")
+            return 255
+
         host, port = proxymanager.get_host_and_port(resource)
 
         # check for valid resources
         assert port is not None, "Port is not set"
 
         call = ['microcom', '-s', str(resource.speed), '-t', f"{host}:{port}"]
 
@@ -846,19 +858,22 @@
             print("connection lost", file=sys.stderr)
         return p.returncode
 
     async def console(self, place, target):
         while True:
             res = await self._console(place, target, 10.0, logfile=self.args.logfile,
                                       loop=self.args.loop, listen_only=self.args.listenonly)
-            if res:
-                exc = InteractiveCommandError("microcom error")
-                exc.exitcode = res
-                raise exc
+            # place released
+            if res == 255:
+                break
             if not self.args.loop:
+                if res:
+                    exc = InteractiveCommandError("microcom error")
+                    exc.exitcode = res
+                    raise exc
                 break
             await asyncio.sleep(1.0)
     console.needs_target = True
 
     def dfu(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
@@ -1196,14 +1211,40 @@
         if action == 'info':
             data = drv.get_channel_info(channel)
         elif action == 'values':
             data = drv.get_channel_values(channel)
         for k, v in sorted(data.items()):
             print(f"{k:<16s} {str(v):<10s}")
 
+    def write_files(self):
+        place = self.get_acquired_place()
+        target = self._get_target(place)
+        name = self.args.name
+        drv = self._get_driver_or_new(target, "USBStorageDriver", activate=False, name=name)
+        drv.storage.timeout = self.args.wait
+        target.activate(drv)
+
+        try:
+            if self.args.partition == 0:
+                self.args.partition = None
+
+            if self.args.rename:
+                if len(self.args.SOURCE) != 2:
+                    self.args.parser.error("the following arguments are required: SOURCE DEST")
+
+                drv.write_files([self.args.SOURCE[0]], self.args.SOURCE[1],
+                                self.args.partition, target_is_directory=False)
+            else:
+                drv.write_files(self.args.SOURCE, self.args.target_directory,
+                                self.args.partition, target_is_directory=True)
+        except subprocess.CalledProcessError as e:
+            raise UserError(f"could not copy files to network usb storage: {e}")
+        except FileNotFoundError as e:
+            raise UserError(e)
+
     def write_image(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
         name = self.args.name
         drv = self._get_driver_or_new(target, "USBStorageDriver", activate=False, name=name)
         drv.storage.timeout = self.args.wait
         target.activate(drv)
@@ -1291,14 +1332,17 @@
             print("Waiting for CTRL+C or SIGTERM...", file=sys.stderr)
             while True:
                 await asyncio.sleep(1.0)
         except GeneratorExit:
             print("Exiting...\n", file=sys.stderr)
     export.needs_target = True
 
+    def print_version(self):
+        print(labgrid_version())
+
 
 def start_session(url, realm, extra):
     from autobahn.asyncio.wamp import ApplicationRunner
 
     loop = asyncio.get_event_loop()
     ready = asyncio.Event()
 
@@ -1740,14 +1784,35 @@
     tmc_subparser.set_defaults(func=ClientSession.tmc_screen)
 
     tmc_subparser = tmc_subparsers.add_parser('channel', help="use a channel")
     tmc_subparser.add_argument('channel', type=int)
     tmc_subparser.add_argument('action', choices=['info', 'values'])
     tmc_subparser.set_defaults(func=ClientSession.tmc_channel)
 
+    subparser = subparsers.add_parser('write-files', help="copy files onto mass storage device",
+                                      usage="%(prog)s [OPTION]... -T SOURCE DEST\n" +
+                                     "       %(prog)s [OPTION]... [-t DIRECTORY] SOURCE...")
+    subparser.add_argument('-w', '--wait', type=float, default=10.0,
+                           help='storage poll timeout in seconds')
+    subparser.add_argument('-p', '--partition', type=int, choices=range(0, 256),
+                           metavar='0-255', default=1,
+                           help='partition number to mount or 0 to mount whole disk (default: %(default)s)')
+    group = subparser.add_mutually_exclusive_group()
+    group.add_argument('-t', '--target-directory', type=pathlib.PurePath, metavar='DIRECTORY',
+                           default=pathlib.PurePath("/"),
+                           help='copy all SOURCE files into DIRECTORY (default: partition root)')
+    group.add_argument('-T', action='store_true', dest='rename',
+                           help='copy SOURCE file and rename to DEST')
+    subparser.add_argument('--name', '-n', help="optional resource name")
+    subparser.add_argument('SOURCE', type=pathlib.PurePath, nargs='+',
+                           help='source file(s) to copy')
+    subparser.add_argument('DEST', type=pathlib.PurePath, nargs='?',
+                           help='destination file name for SOURCE')
+    subparser.set_defaults(func=ClientSession.write_files, parser=subparser)
+
     subparser = subparsers.add_parser('write-image', help="write an image onto mass storage")
     subparser.add_argument('-w', '--wait', type=float, default=10.0)
     subparser.add_argument('-p', '--partition', type=int, help="partition number to write to")
     subparser.add_argument('--skip', type=int, default=0,
                            help="skip n 512-sized blocks at start of input")
     subparser.add_argument('--seek', type=int, default=0,
                            help="skip n 512-sized blocks at start of output")
@@ -1783,14 +1848,17 @@
     subparser = subparsers.add_parser('export', help="export driver information to a file (needs environment with drivers)")
     subparser.add_argument('--format', dest='format',
                            type=ExportFormat, choices=ExportFormat, default=ExportFormat.SHELL_EXPORT,
                            help="output format (default: %(default)s)")
     subparser.add_argument('filename', help='output filename')
     subparser.set_defaults(func=ClientSession.export)
 
+    subparser = subparsers.add_parser('version', help="show version")
+    subparser.set_defaults(func=ClientSession.print_version)
+
     # make any leftover arguments available for some commands
     args, leftover = parser.parse_known_args()
     if args.command not in ['ssh', 'rsync', 'forward']:
         args = parser.parse_args()
     else:
         args.leftover = leftover
```

### Comparing `labgrid-23.1a2/labgrid/remote/common.py` & `labgrid-24.0a1/labgrid/remote/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     'TAG_VAL',
     'ResourceEntry',
     'ResourceMatch',
     'Place',
     'ReservationState',
     'Reservation',
     'enable_tcp_nodelay',
+    'monkey_patch_max_msg_payload_size_ws_option',
 ]
 
 TAG_KEY = re.compile(r"[a-z][a-z0-9_]+")
 TAG_VAL = re.compile(r"[a-z0-9_]?")
 
 
 @attr.s(eq=False)
@@ -308,7 +309,40 @@
 def enable_tcp_nodelay(session):
     """
     asyncio/autobahn does not set TCP_NODELAY by default, so we need to do it
     like this for now.
     """
     s = session._transport.transport.get_extra_info('socket')
     s.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, True)
+
+
+def monkey_patch_max_msg_payload_size_ws_option():
+    """
+    The default maxMessagePayloadSize in autobahn is 1M. For larger setups with a big number of
+    exported resources, this becomes the limiting factor.
+    Increase maxMessagePayloadSize in WampWebSocketClientFactory.setProtocolOptions() by monkey
+    patching it, so autobahn.asyncio.wamp.ApplicationRunner effectively sets the increased value.
+
+    This function must be called before ApplicationRunner is instanciated.
+    """
+    from autobahn.asyncio.websocket import WampWebSocketClientFactory
+
+    original_method = WampWebSocketClientFactory.setProtocolOptions
+
+    def set_protocol_options(*args, **kwargs):
+        new_max_message_payload_size = 10485760
+
+        # maxMessagePayloadSize given as positional arg
+        args = list(args)
+        try:
+            args[9] = max((args[9], new_max_message_payload_size))
+        except IndexError:
+            pass
+
+        # maxMessagePayloadSize given as kwarg
+        kwarg_name = "maxMessagePayloadSize"
+        if kwarg_name in kwargs and kwargs[kwarg_name] is not None:
+            kwargs[kwarg_name] = max((kwargs[kwarg_name], new_max_message_payload_size))
+
+        return original_method(*args, **kwargs)
+
+    WampWebSocketClientFactory.setProtocolOptions = set_protocol_options
```

### Comparing `labgrid-23.1a2/labgrid/remote/config.py` & `labgrid-24.0a1/labgrid/remote/config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/remote/coordinator.py` & `labgrid-24.0a1/labgrid/remote/coordinator.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from autobahn.wamp.types import RegisterOptions
 
 from .common import *  # pylint: disable=wildcard-import
 from .scheduler import TagSet, schedule
 from ..util import atomic_replace, yaml
 
 
+monkey_patch_max_msg_payload_size_ws_option()
+
+
 class Action(Enum):
     ADD = 0
     DEL = 1
     UPD = 2
 
 
 @attr.s(init=False, eq=False)
@@ -129,22 +132,19 @@
 
         self.load()
         self.save_later()
 
         enable_tcp_nodelay(self)
         self.join(
             self.config.realm,
-            authmethods=["anonymous", "ticket"],
+            authmethods=["anonymous"],
             authid="coordinator",
             authextra={"authid": "coordinator"},
         )
 
-    def onChallenge(self, challenge):
-        return "dummy-ticket"
-
     @locked
     async def onJoin(self, details):
         await self.subscribe(self.on_session_join, 'wamp.session.on_join')
         await self.subscribe(
             self.on_session_leave, 'wamp.session.on_leave'
         )
         await self.register(
@@ -310,15 +310,15 @@
 
         loop = asyncio.get_event_loop()
         await loop.run_in_executor(None, atomic_replace, 'resources.yaml', resources)
         await loop.run_in_executor(None, atomic_replace, 'places.yaml', places)
 
     def load(self):
         try:
-            self.place = {}
+            self.places = {}
             with open('places.yaml', 'r') as f:
                 self.places = yaml.load(f.read())
             for placename, config in self.places.items():
                 config['name'] = placename
                 # FIXME maybe recover previously acquired places here?
                 if 'acquired' in config:
                     del config['acquired']
```

### Comparing `labgrid-23.1a2/labgrid/remote/exporter.py` & `labgrid-24.0a1/labgrid/remote/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 from pathlib import Path
 from typing import Dict, Type
 from socket import gethostname, getfqdn
 import attr
 from autobahn.asyncio.wamp import ApplicationRunner, ApplicationSession
 
 from .config import ResourceConfig
-from .common import ResourceEntry, enable_tcp_nodelay
-from ..util import get_free_port
+from .common import ResourceEntry, enable_tcp_nodelay, monkey_patch_max_msg_payload_size_ws_option
+from ..util import get_free_port, labgrid_version
 
-try:
-    import pkg_resources
-    __version__ = pkg_resources.get_distribution('labgrid').version
-except pkg_resources.DistributionNotFound:
-    __version__ = "unknown"
 
+monkey_patch_max_msg_payload_size_ws_option()
 
+__version__ = labgrid_version()
 exports: Dict[str, Type[ResourceEntry]] = {}
 reexec = False
 
 class ExporterError(Exception):
     pass
 
 
@@ -578,19 +575,21 @@
 class GPIOSysFSExport(ResourceExport):
     _gpio_sysfs_path_prefix = '/sys/class/gpio'
 
     """ResourceExport for GPIO lines accessed directly from userspace"""
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        local_cls_name = self.cls
-        self.data['cls'] = f"Network{self.cls}"
-        from ..resource import base
-        local_cls = getattr(base, local_cls_name)
-        self.local = local_cls(target=None, name=None, **self.local_params)
+        if self.cls == "SysfsGPIO":
+            from ..resource.base import SysfsGPIO
+            self.local = SysfsGPIO(target=None, name=None, **self.local_params)
+        elif self.cls == "MatchedSysfsGPIO":
+            from ..resource.udev import MatchedSysfsGPIO
+            self.local = MatchedSysfsGPIO(target=None, name=None, **self.local_params)
+        self.data['cls'] = "NetworkSysfsGPIO"
         self.export_path = Path(GPIOSysFSExport._gpio_sysfs_path_prefix,
                                 f'gpio{self.local.index}')
         self.system_exported = False
 
     def _get_params(self):
         """Helper function to return parameters"""
         return {
@@ -623,14 +622,15 @@
             return
 
         export_sysfs_path = os.path.join(GPIOSysFSExport._gpio_sysfs_path_prefix, 'unexport')
         with open(export_sysfs_path, mode='wb') as unexport:
             unexport.write(str(index).encode('utf-8'))
 
 exports["SysfsGPIO"] = GPIOSysFSExport
+exports["MatchedSysfsGPIO"] = GPIOSysFSExport
 
 
 @attr.s
 class NetworkServiceExport(ResourceExport):
     """ResourceExport for a NetworkService
 
     This checks if the address has a interface suffix and then provides the
@@ -696,14 +696,34 @@
 
     def _get_params(self):
         """Helper function to return parameters"""
         return {'host' : self.host, **self.local_params}
 
 exports["AndroidNetFastboot"] = AndroidNetFastbootExport
 
+@attr.s(eq=False)
+class YKUSHPowerPortExport(ResourceExport):
+    """ResourceExport for YKUSHPowerPort devices"""
+
+    def __attrs_post_init__(self):
+        super().__attrs_post_init__()
+        local_cls_name = self.cls
+        self.data['cls'] = f"Network{local_cls_name}"
+        from ..resource import ykushpowerport
+        local_cls = getattr(ykushpowerport, local_cls_name)
+        self.local = local_cls(target=None, name=None, **self.local_params)
+
+    def _get_params(self):
+        return {
+            "host": self.host,
+            **self.local_params
+        }
+
+exports["YKUSHPowerPort"] = YKUSHPowerPortExport
+
 class ExporterSession(ApplicationSession):
     def onConnect(self):
         """Set up internal datastructures on successful connection:
         - Setup loop, name, authid and address
         - Join the coordinator as an exporter"""
         self.loop = self.config.extra['loop']
         self.name = self.config.extra['name']
@@ -898,14 +918,20 @@
         '--hostname',
         dest='hostname',
         type=str,
         default=None,
         help='hostname (or IP) published for accessing resources (defaults to the system hostname)'
     )
     parser.add_argument(
+        '--fqdn',
+        action='store_true',
+        default=False,
+        help='Use fully qualified domain name as default for hostname'
+    )
+    parser.add_argument(
         '-d',
         '--debug',
         action='store_true',
         default=False,
         help="enable debug mode"
     )
     parser.add_argument(
@@ -924,15 +950,15 @@
 
     args = parser.parse_args()
 
     level = 'debug' if args.debug else 'info'
 
     extra = {
         'name': args.name or gethostname(),
-        'hostname': args.hostname or gethostname(),
+        'hostname': args.hostname or (getfqdn() if args.fqdn else gethostname()),
         'resources': args.resources,
         'isolated': args.isolated
     }
 
     crossbar_url = args.crossbar
     crossbar_realm = os.environ.get("LG_CROSSBAR_REALM", "realm1")
```

### Comparing `labgrid-23.1a2/labgrid/remote/scheduler.py` & `labgrid-24.0a1/labgrid/remote/scheduler.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/base.py` & `labgrid-24.0a1/labgrid/resource/base.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/common.py` & `labgrid-24.0a1/labgrid/resource/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import shlex
 from typing import Dict, Type, List
 import attr
 
 from ..binding import BindingMixin
 from ..util.ssh import sshmanager
 
@@ -22,14 +23,21 @@
     """
     avail = attr.ib(default=True, init=False, validator=attr.validators.instance_of(bool))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self._parent = None
 
+        logger_name = self.__class__.__name__
+        if self.target:
+            logger_name += f"({self.target.name})"
+        if self.name:
+            logger_name += f":{self.name}"
+        self.logger = logging.getLogger(logger_name)
+
     @property
     def command_prefix(self):
         return []
 
     def wrap_command(self, command):
         """
         Returns the command as-is, no need for command wrapping for local resources.
@@ -57,14 +65,20 @@
         return self._parent.get_managed_parent() if self._parent else None
 
     def poll(self):
         managed_parent = self.get_managed_parent()
         if managed_parent:
             managed_parent.poll()
 
+    def get_bound_resources(self):
+        """
+        Resources only return themselves in a set, drivers will combine those sets.
+        """
+        return {self}
+
 
 @attr.s(eq=False)
 class NetworkResource(Resource):
     """
     Represents a remote Resource available on another computer.
 
     This stores a command_prefix to describe how to connect to the remote
@@ -108,14 +122,15 @@
         if instance is None:
             instance = cls()
             ResourceManager.instances[cls] = instance
         return instance
 
     def __attrs_post_init__(self):
         self.resources: List[ManagedResource] = []
+        self.logger = logging.getLogger(str(self))
 
     def _add_resource(self, resource: 'ManagedResource'):
         self.resources.append(resource)
         self.on_resource_added(resource)
 
     def on_resource_added(self, resource: 'ManagedResource'):
         pass
```

### Comparing `labgrid-23.1a2/labgrid/resource/docker.py` & `labgrid-24.0a1/labgrid/resource/docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Auxiliary classes that assist DockerDriver. Specifically, DockerDaemon
 and DockerManager will create the NetworkResource instance that is declared
 in the specification (e.g. yaml) of DockerDriver.
 """
 
-import logging
 import socket
 
 import attr
 
 from labgrid.util.dict import find_dict
 from ..factory import target_factory
 from .common import ManagedResource, ResourceManager
@@ -30,15 +29,14 @@
     containers and managing the managed NetworkService
     resources. Different docker daemons for different targets are
     allowed, but there has to be only one for each target.
     """
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.log = logging.getLogger('DockerManager')
         self._client = dict()
         self._docker_daemons_cleaned = list()
 
     def on_resource_added(self, resource):
         """If the resource added is a DockerDaemon, make sure this is the
         only one added for this target.  If it is, create a docker
         client to be used to communicate with the docker daemon.
@@ -67,15 +65,15 @@
         """
         if docker_client.api.base_url not in self._docker_daemons_cleaned:
             container_list = docker_client.api.containers(
                 all=True, filters={"label": DockerConstants.DOCKER_LG_CLEANUP_LABEL})
             for container in container_list:
                 if (container['Labels'][DockerConstants.DOCKER_LG_CLEANUP_LABEL] ==
                         DockerConstants.DOCKER_LG_CLEANUP_TYPE_AUTO):
-                    self.log.info("Deleting container %s", container['Names'][0])
+                    self.logger.info("Deleting container %s", container['Names'][0])
                     docker_client.api.remove_container(container['Id'], force=True)
             self._docker_daemons_cleaned.append(docker_client.api.base_url)
 
 
 @target_factory.reg_resource
 @attr.s(eq=False)
 class DockerDaemon(ManagedResource):
@@ -86,15 +84,14 @@
     container name to a network service.
     """
     manager_cls = DockerManager
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self._nw_services = dict()
-        self.log = logging.getLogger('DockerContainer')
         self.timeout = 5.0
         self.avail = True
 
     def on_client_bound(self, client):
         """Each time a docker driver binds to the DockerDaemon resource
         the docker driver network services list is iterated and for each
         network service defined a NetworkService resource instance is
@@ -128,15 +125,15 @@
         :param docker_client: The docker client to use for lookup
         """
         for container_name, nw_service_list in self._nw_services.items():
             for nw_service in nw_service_list:
                 if nw_service.address == "":
                     container = docker_client.api.containers(
                         filters={"name": "/" + container_name})
-                    self.log.debug("Containers found %s", container)
+                    self.logger.debug("Containers found %s", container)
                     if container:
                         nw_service.address = find_dict(
                             d=container[0]['NetworkSettings'],
                             key='IPAddress')
                 if (nw_service.address != "" and
                         self._socket_connect(nw_service.address,
                                              nw_service.port)):
```

### Comparing `labgrid-23.1a2/labgrid/resource/ethernetport.py` & `labgrid-24.0a1/labgrid/resource/ethernetport.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,14 @@
 
 
 @attr.s
 class EthernetPortManager(ResourceManager):
     """The EthernetPortManager periodically polls the switch for new updates."""
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}")
         self.loop = None
         self.poll_tasks = []
         self.switches = {}
         self.neighbors = {}
 
     def on_resource_added(self, resource):
         """Handler to execute when the resource is added
```

### Comparing `labgrid-23.1a2/labgrid/resource/lxaiobus.py` & `labgrid-24.0a1/labgrid/resource/lxaiobus.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from time import monotonic
 from importlib import import_module
 
 import attr
 
 from ..factory import target_factory
 from .common import ManagedResource, ResourceManager
@@ -10,26 +9,24 @@
 
 @attr.s(eq=False)
 class LXAIOBusNodeManager(ResourceManager):
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self._requests = import_module('requests')
 
-        self.log = logging.getLogger('LXAIOBusNodeManager')
-
         self._last = 0.0
 
     def _get_nodes(self, host):
         try:
             r = self._requests.get(f'http://{host}/nodes/')
             r.raise_for_status()
             j = r.json()
             return j["result"]
         except self._requests.exceptions.ConnectionError:
-            self.log.exception("failed to connect to host %s", host)
+            self.logger.exception("failed to connect to host %s", host)
             return []
 
     def poll(self):
         if monotonic()-self._last < 2:
             return  # ratelimit requests
         self._last = monotonic()
         hosts = {r.host for r in self.resources}
```

### Comparing `labgrid-23.1a2/labgrid/resource/modbus.py` & `labgrid-24.0a1/labgrid/resource/modbus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/modbusrtu.py` & `labgrid-24.0a1/labgrid/resource/modbusrtu.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/mqtt.py` & `labgrid-24.0a1/labgrid/resource/mqtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import threading
 from time import monotonic
 
 import attr
 
 from .common import ManagedResource, ResourceManager
 from ..factory import target_factory
@@ -12,21 +11,17 @@
     _available = attr.ib(default=attr.Factory(set), validator=attr.validators.instance_of(set))
     _avail_lock = attr.ib(default=threading.Lock())
     _clients = attr.ib(default=attr.Factory(dict), validator=attr.validators.instance_of(dict))
     _topics = attr.ib(default=attr.Factory(list), validator=attr.validators.instance_of(list))
     _topic_lock = attr.ib(default=threading.Lock())
     _last = attr.ib(default=0.0, validator=attr.validators.instance_of(float))
 
-    def __attrs_post_init__(self):
-        super().__attrs_post_init__()
-        self.log = logging.getLogger('MQTTManager')
-
     def _create_mqtt_connection(self, host):
         import paho.mqtt.client as mqtt
-        client = mqtt.Client()
+        client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
         client.connect(host)
         client.on_message = self._on_message
         client.loop_start()
         return client
 
     def on_resource_added(self, resource):
         host = resource.host
```

### Comparing `labgrid-23.1a2/labgrid/resource/onewireport.py` & `labgrid-24.0a1/labgrid/resource/onewireport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/power.py` & `labgrid-24.0a1/labgrid/resource/power.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/remote.py` & `labgrid-24.0a1/labgrid/resource/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import logging
+import copy
 import os
 import attr
 
 from ..factory import target_factory
 from .common import NetworkResource, ManagedResource, ResourceManager
 
 
 @attr.s(eq=False)
 class RemotePlaceManager(ResourceManager):
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.logger = logging.getLogger(f"{self}")
         self.url = None
         self.realm = None
         self.loop = None
         self.session = None
         self.ready = None
         self.unmanaged_resources = []
 
@@ -46,26 +45,27 @@
                 config = self.env.config
                 self.url = config.get_option('crossbar_url', self.url)
                 self.realm = config.get_option('crossbar_realm', self.realm)
             self._start()
         place = self.session.get_place(remote_place.name)  # pylint: disable=no-member
         resource_entries = self.session.get_target_resources(place)  # pylint: disable=no-member
         expanded = []
-        for resource_name, resource_entry in resource_entries.items():
+        for (resource_name, _), resource_entry in resource_entries.items():
             new = target_factory.make_resource(
                 remote_place.target, resource_entry.cls, resource_name, resource_entry.args)
             new.parent = remote_place
             new.avail = resource_entry.avail
             new.extra = resource_entry.extra
             new._remote_entry = resource_entry
             if not isinstance(new, ManagedResource):
                 self.unmanaged_resources.append(new)
             expanded.append(new)
         self.logger.debug("expanded remote resources for place %s: %s", remote_place.name, expanded)
         remote_place.avail = True
+        remote_place.tags = copy.deepcopy(place.tags)
 
     def poll(self):
         import asyncio
         if not self.loop.is_running():
             self.loop.run_until_complete(asyncio.sleep(0.1))
         for resource in self.resources + self.unmanaged_resources:
             if isinstance(resource, RemotePlace):
@@ -93,14 +93,15 @@
 @target_factory.reg_resource
 @attr.s(eq=False)
 class RemotePlace(ManagedResource):
     manager_cls = RemotePlaceManager
 
     def __attrs_post_init__(self):
         self.timeout = 10.0
+        self.tags = {}
         super().__attrs_post_init__()
 
 @attr.s(eq=False)
 class RemoteUSBResource(NetworkResource, ManagedResource):
     manager_cls = RemotePlaceManager
 
     busnum = attr.ib(validator=attr.validators.optional(attr.validators.instance_of(int)))
@@ -396,15 +397,15 @@
 @attr.s(eq=False)
 class RemoteTFTPProvider(RemoteBaseProvider):
     pass
 
 
 @target_factory.reg_resource
 @attr.s(eq=False)
-class RemoteNFSProvider(RemoteBaseProvider):
+class RemoteNFSProvider(NetworkResource):
     pass
 
 
 @target_factory.reg_resource
 @attr.s(eq=False)
 class RemoteHTTPProvider(RemoteBaseProvider):
     pass
```

### Comparing `labgrid-23.1a2/labgrid/resource/serialport.py` & `labgrid-24.0a1/labgrid/resource/serialport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/sigrok.py` & `labgrid-24.0a1/labgrid/resource/sigrok.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/resource/suggest.py` & `labgrid-24.0a1/labgrid/resource/suggest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     USBNetworkInterface,
     SiSPMPowerPort,
     USBAudioInput,
     LXAUSBMux,
     HIDRelay,
     USBDebugger,
     USBPowerPort,
+    MatchedSysfsGPIO
 )
 from ..util import dump
 
 
 class Suggester:
     def __init__(self, args):
         self.resources = []
@@ -52,14 +53,15 @@
         self.resources.append(USBNetworkInterface(**args))
         self.resources.append(SiSPMPowerPort(**args))
         self.resources.append(USBAudioInput(**args))
         self.resources.append(LXAUSBMux(**args))
         self.resources.append(HIDRelay(**args))
         self.resources.append(USBDebugger(**args))
         self.resources.append(USBPowerPort(**args, index=0))
+        self.resources.append(MatchedSysfsGPIO(**args, pin=0))
 
     def suggest_callback(self, resource, meta, suggestions):
         cls = type(resource).__name__
         if resource.device.action == 'add':
             print("=== added device ===")
         else:
             print("=== existing device ===")
@@ -80,14 +82,16 @@
                 print("  ---")
             print(textwrap.indent(
                 dump({cls: {"match": suggestion}}).strip(),
                 '  ',
             ))
             if cls == 'USBPowerPort':
                 print('    index: ?')
+            if cls == 'MatchedSysfsGPIO':
+                print('    pin: ?')
         print("  ---")
         print()
 
     def run(self):
         while True:
             managers = {r.get_managed_parent().manager for r in self.resources}
             for manager in managers:
```

### Comparing `labgrid-23.1a2/labgrid/resource/udev.py` & `labgrid-24.0a1/labgrid/resource/udev.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import queue
 import warnings
 from collections import OrderedDict
 from importlib import import_module
 
 import attr
@@ -15,55 +14,53 @@
 
 @attr.s(eq=False)
 class UdevManager(ResourceManager):
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self.queue = queue.Queue()
 
-        self.log = logging.getLogger('UdevManager')
         self._pyudev = import_module('pyudev')
         self._context = self._pyudev.Context()
         self._monitor = self._pyudev.Monitor.from_netlink(self._context)
         self._observer = self._pyudev.MonitorObserver(self._monitor,
                                                 callback=self._insert_into_queue)
         self._observer.start()
 
     def on_resource_added(self, resource):
         devices = self._context.list_devices()
         devices.match_subsystem(resource.match['SUBSYSTEM'])
         for device in devices:
             if resource.try_match(device):
-                self.log.debug(" matched successfully against %s", resource.device)
+                self.logger.debug(" matched successfully against %s", resource.device)
 
     def _insert_into_queue(self, device):
         self.queue.put(device)
 
     def poll(self):
         timeout = Timeout(0.1)
         while not timeout.expired:
             try:
                 device = self.queue.get(False)
             except queue.Empty:
                 break
-            self.log.debug("%s: %s", device.action, device)
+            self.logger.debug("%s: %s", device.action, device)
             for resource in self.resources:
                 if resource.try_match(device):
-                    self.log.debug(" matched successfully")
+                    self.logger.debug(" matched successfully")
 
 @attr.s(eq=False)
 class USBResource(ManagedResource):
     manager_cls = UdevManager
 
     match = attr.ib(factory=dict, validator=attr.validators.instance_of(dict), hash=False)
     device = attr.ib(default=None, hash=False)
     suggest = attr.ib(default=False, hash=False, repr=False)
 
     def __attrs_post_init__(self):
         self.timeout = 5.0
-        self.log = logging.getLogger('USBResource')
         self.match.setdefault('SUBSYSTEM', 'usb')
         super().__attrs_post_init__()
 
     def filter_match(self, device):  # pylint: disable=unused-argument,no-self-use
         return True
 
     def suggest_match(self, device):
@@ -90,20 +87,30 @@
             suggestions.append({'ID_PATH': path})
         elif self.match.get('@SUBSYSTEM', None) == 'usb':
             path = self._get_usb_device().properties.get('ID_PATH')
             if path:
                 suggestions.append({'@ID_PATH': path})
 
         serial = self.device.properties.get('ID_SERIAL_SHORT')
+        interface_num = self.device.properties.get('ID_USB_INTERFACE_NUM')
         if serial:
-            suggestions.append({'ID_SERIAL_SHORT': serial})
+            if interface_num is not None:
+                suggestions.append({'ID_SERIAL_SHORT': serial,
+                                    'ID_USB_INTERFACE_NUM': interface_num})
+            else:
+                suggestions.append({'ID_SERIAL_SHORT': serial})
         elif self.match.get('@SUBSYSTEM', None) == 'usb':
             serial = self._get_usb_device().properties.get('ID_SERIAL_SHORT')
+            interface_num = self._get_usb_device().properties.get('ID_USB_INTERFACE_NUM')
             if serial:
-                suggestions.append({'@ID_SERIAL_SHORT': serial})
+                if interface_num is not None:
+                    suggestions.append({'@ID_SERIAL_SHORT': serial,
+                                        '@ID_USB_INTERFACE_NUM': interface_num})
+                else:
+                    suggestions.append({'@ID_SERIAL_SHORT': serial})
 
         return meta, suggestions
 
     def try_match(self, device):
         if self.device is None:  # new device
             def match_single(dev, key, value):
                 if dev.properties.get(key) == value:
@@ -130,15 +137,15 @@
 
             if not self.filter_match(device):
                 return False
         else:  # update
             if self.device.sys_path != device.sys_path:
                 return False
 
-        self.log.debug(" found match: %s", self)
+        self.logger.debug(" found match: %s", self)
 
         if self.suggest and device.action in [None, 'add']:
             self.device = device
             self.suggest(self, *self.suggest_match(device))
             self.device = None
             return False
 
@@ -276,14 +283,15 @@
         if match not in [("15a2", "0054"), ("15a2", "0061"),
                          ("15a2", "0063"), ("15a2", "0071"),
                          ("15a2", "007d"), ("15a2", "0076"),
                          ("15a2", "0080"), ("15a2", "003a"),
                          ("1fc9", "0128"), ("1fc9", "0126"),
                          ("1fc9", "012b"), ("1fc9", "0134"),
                          ("1fc9", "013e"), ("1fc9", "0146"),
+                         ("1fc9", "014e"),
                          ("1b67", "4fff"), ("0525", "b4a4"), # SPL
                          ("3016", "1001"),
                          ]:
             return False
 
         return super().filter_match(device)
 
@@ -342,14 +350,19 @@
 
 @target_factory.reg_resource
 @attr.s(eq=False)
 class USBNetworkInterface(USBResource, NetworkInterface):
     def __attrs_post_init__(self):
         self.match['SUBSYSTEM'] = 'net'
         self.match['@SUBSYSTEM'] = 'usb'
+        if self.ifname:
+            warnings.warn(
+                "USBNetworkInterface: The ifname attribute will be overwritten by udev.\n"
+                "Please use udev matching as described in http://labgrid.readthedocs.io/en/latest/configuration.html#udev-matching"  # pylint: disable=line-too-long
+            )
         super().__attrs_post_init__()
 
     def update(self):
         super().update()
         if self.device is not None:
             self.ifname = self.device.properties.get('INTERFACE')
         else:
@@ -463,23 +476,25 @@
     def avail(self, prop):
         pass
 
     # Overwrite the poll function. Only mark the SDWire as available if both
     # paths are available.
     def poll(self):
         super().poll()
+        if self.device is not None and not self.avail:
+            for child in self.device.parent.children:
+                if child.subsystem == 'block' and child.device_type == 'disk':
+                    self.disk_path = child.device_node
+            self.control_serial = self.device.properties.get('ID_SERIAL_SHORT')
+
+    def update(self):
+        super().update()
         if self.device is None:
             self.disk_path = None
             self.control_serial = None
-        else:
-            if not self.avail:
-                for child in self.device.parent.children:
-                    if child.subsystem == 'block' and child.device_type == 'disk':
-                        self.disk_path = child.device_node
-                self.control_serial = self.device.properties.get('ID_SERIAL_SHORT')
 
     @property
     def path(self):
         return self.disk_path
 
 @target_factory.reg_resource
 @attr.s(eq=False)
@@ -506,24 +521,26 @@
     def avail(self, prop):
         pass
 
     # Overwrite the poll function. Only mark the SDMux as available if both
     # paths are available.
     def poll(self):
         super().poll()
+        if self.device is not None and not self.avail:
+            for child in self.device.children:
+                if child.subsystem == 'block' and child.device_type == 'disk':
+                    self.disk_path = child.device_node
+                elif child.subsystem == 'scsi_generic':
+                    self.control_path = child.device_node
+
+    def update(self):
+        super().update()
         if self.device is None:
             self.control_path = None
             self.disk_path = None
-        else:
-            if not self.avail:
-                for child in self.device.children:
-                    if child.subsystem == 'block' and child.device_type == 'disk':
-                        self.disk_path = child.device_node
-                    elif child.subsystem == 'scsi_generic':
-                        self.control_path = child.device_node
 
     @property
     def path(self):
         return self.disk_path
 
 @target_factory.reg_resource
 @attr.s(eq=False)
@@ -683,16 +700,50 @@
 @target_factory.reg_resource
 @attr.s(eq=False)
 class USBDebugger(USBResource):
     def filter_match(self, device):
         match = (device.properties.get('ID_VENDOR_ID'), device.properties.get('ID_MODEL_ID'))
 
         if match not in [("0403", "6010"),  # FT2232C/D/H Dual UART/FIFO IC
+                         ("0483", "374b"),  # STLINK-V3
                          ("0483", "374f"),  # STLINK-V3
                          ("15ba", "0003"),  # Olimex ARM-USB-OCD
                          ("15ba", "002b"),  # Olimex ARM-USB-OCD-H
                          ("15ba", "0004"),  # Olimex ARM-USB-TINY
                          ("15ba", "002a"),  # Olimex ARM-USB-TINY-H
+                         ("1366", "0101"),  # SEGGER J-Link PLUS
+                         ("1366", "0105"),  # SEGGER J-Link
+                         ("1366", "1015"),  # SEGGER J-Link
+                         ("1366", "1051"),  # SEGGER J-Link
                          ]:
             return False
 
         return super().filter_match(device)
+
+@target_factory.reg_resource
+@attr.s(eq=False)
+class MatchedSysfsGPIO(USBResource):
+    """The MatchedSysfsGPIO described a SysfsGPIO matched by Udev
+
+    Args:
+        pin (int): gpio pin number within the matched gpiochip."""
+    pin = attr.ib(default=None, validator=attr.validators.instance_of(int))
+    index = None
+
+    def __attrs_post_init__(self):
+        self.match['SUBSYSTEM'] = 'gpio'
+        super().__attrs_post_init__()
+
+    def filter_match(self, device):
+        # Filter out the char device
+        if device.properties.get('DEVNAME') is not None:
+            return False
+        return super().filter_match(device)
+
+    def update(self):
+        super().update()
+        if self.device is not None:
+            if self.pin >= int(self.read_attr('ngpio')):
+                raise ValueError("MatchedSysfsGPIO pin out of bound")
+            self.index = int(self.read_attr('base')) + self.pin
+        else:
+            self.index = None
```

### Comparing `labgrid-23.1a2/labgrid/step.py` & `labgrid-24.0a1/labgrid/step.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/stepreporter.py` & `labgrid-24.0a1/labgrid/stepreporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     @classmethod
     def start(cls):
         """starts the StepReporter"""
         from warnings import warn
         warn(
             """
-            StepLogger is deprecated, use the StepLogger and basicConfig from labgrid.logging
+            StepReporter is deprecated, use the StepLogger and basicConfig from labgrid.logging
             instead which integrates with the python logging infrastructure.
             """,
             DeprecationWarning,
             stacklevel=2,
         )
         assert not cls._started
         steps.subscribe(cls.notify)
```

### Comparing `labgrid-23.1a2/labgrid/strategy/bareboxstrategy.py` & `labgrid-24.0a1/labgrid/strategy/bareboxstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/strategy/common.py` & `labgrid-24.0a1/labgrid/strategy/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/strategy/dockerstrategy.py` & `labgrid-24.0a1/labgrid/strategy/dockerstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/strategy/graphstrategy.py` & `labgrid-24.0a1/labgrid/strategy/graphstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/strategy/shellstrategy.py` & `labgrid-24.0a1/labgrid/strategy/shellstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/strategy/ubootstrategy.py` & `labgrid-24.0a1/labgrid/strategy/ubootstrategy.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,7 +53,20 @@
             self.uboot.boot("")
             self.uboot.await_boot()
             self.target.activate(self.shell)
             self.shell.run("systemctl is-system-running --wait")
         else:
             raise StrategyError(f"no transition found from {self.status} to {status}")
         self.status = status
+
+    def force(self, status):
+        if not isinstance(status, Status):
+            status = Status[status]
+        if status == Status.off:
+            self.target.activate(self.power)
+        elif status == Status.uboot:
+            self.target.activate(self.uboot)
+        elif status == Status.shell:
+            self.target.activate(self.shell)
+        else:
+            raise StrategyError("can not force state {}".format(status))
+        self.status = status
```

### Comparing `labgrid-23.1a2/labgrid/target.py` & `labgrid-24.0a1/labgrid/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,56 +136,58 @@
         if not name and default and len(found) != 1:
             found = [default]
 
         if not found:
             name_msg = f" named '{name}'" if name else ""
             if other_names:
                 raise NoResourceFoundError(
-                    f"no {cls} resource{name_msg} found in {self}, matching resources with other names: {other_names}"  # pylint: disable=line-too-long
+                    f"no {cls.__name__} resource{name_msg} found in {self}, matching resources with other names: {other_names}"  # pylint: disable=line-too-long
                 )
 
             raise NoResourceFoundError(
-                f"no {cls} resource{name_msg} found in {self}"
+                f"no {cls.__name__} resource{name_msg} found in {self}"
             )
         elif len(found) > 1:
             raise NoResourceFoundError(
-                f"multiple resources matching {cls} found in {self}", found=found
+                f"multiple resources matching {cls.__name__} found in {self}", found=found
             )
         if wait_avail:
             self.await_resources(found)
         return found[0]
 
-    def _get_driver(self, cls, *, name=None, activate=True, active=False):
+    def _get_driver(self, cls, *, name=None, resource=None, activate=True, active=False):
         assert not (activate is True and active is True)
 
         found = []
         other_names = []
         if isinstance(cls, str):
             cls = target_factory.class_from_string(cls)
 
         for drv in self.drivers:
             if not isinstance(drv, cls):
                 continue
+            if resource and resource not in drv.get_bound_resources():
+                continue
             if name and drv.name != name:
                 other_names.append(drv.name)
                 continue
             if active and drv.state != BindingState.active:
                 continue
             found.append(drv)
         if not found:
             name_msg = f" named '{name}'" if name else ""
             if other_names:
                 raise NoDriverFoundError(
                     "no {active}{cls} driver{name} found in {target}, matching resources with other names: {other_names}".format(  # pylint: disable=line-too-long
-                        active="active " if active else "", cls=cls, name=name_msg, target=self,
-                        other_names=other_names)
+                        active="active " if active else "", cls=cls.__name__, name=name_msg,
+                        target=self, other_names=other_names)
                 )
 
             raise NoDriverFoundError(
-                f"no {'active ' if active else ''}{cls} driver{name_msg} found in {self}"
+                f"no {'active ' if active else ''}{cls.__name__} driver{name_msg} found in {self}"
             )
         elif len(found) > 1:
             prio_last = -255
             prio_found = []
             for drv in found:
                 prio = drv.get_priority(cls)
                 if prio > prio_last:
@@ -196,42 +198,44 @@
                     prio_found.append(drv)
 
             if len(prio_found) == 1:
                 found = prio_found
             else:
                 raise NoDriverFoundError(
                     "multiple {active}drivers matching {cls} found in {target} with the same priorities".format(  # pylint: disable=line-too-long
-                        active="active " if active else "", cls=cls, target=self)
+                        active="active " if active else "", cls=cls.__name__, target=self)
                 )
         if activate:
             self.activate(found[0])
         return found[0]
 
-    def get_active_driver(self, cls, *, name=None):
+    def get_active_driver(self, cls, *, name=None, resource=None):
         """
         Helper function to get the active driver of the target.
         Returns the active driver found, otherwise None.
 
         Arguments:
         cls -- driver-class to return as a resource
         name -- optional name to use as a filter
+        resource -- optional resource to use as a filter
         """
-        return self._get_driver(cls, name=name, activate=False, active=True)
+        return self._get_driver(cls, name=name, resource=resource, activate=False, active=True)
 
-    def get_driver(self, cls, *, name=None, activate=True):
+    def get_driver(self, cls, *, name=None, resource=None, activate=True):
         """
         Helper function to get a driver of the target.
         Returns the first valid driver found, otherwise None.
 
         Arguments:
         cls -- driver-class to return as a resource
         name -- optional name to use as a filter
+        resource -- optional resource to use as a filter
         activate -- activate the driver (default True)
         """
-        return self._get_driver(cls, name=name, activate=activate)
+        return self._get_driver(cls, name=name, resource=resource, activate=activate)
 
     def get_strategy(self):
         """
         Helper function to get the strategy of the target.
 
         Returns the Strategy, if exactly one exists and raises a
         NoStrategyFoundError otherwise.
@@ -268,15 +272,15 @@
             cls = key
         elif len(key) == 2:
             cls, name = key
         if isinstance(cls, str):
             cls = target_factory.class_from_string(cls)
         if not issubclass(cls, (Driver, abc.ABC)): # all Protocols derive from ABC
             raise NoDriverFoundError(
-                f"invalid driver class {cls}"
+                f"invalid driver class {cls.__name__}"
             )
 
         return self.get_active_driver(cls, name=name)
 
     def set_binding_map(self, mapping):
         """
         Configure the binding name mapping for the next driver only.
@@ -362,21 +366,24 @@
                             self.get_driver(requirement, name=supplier_name, activate=False),
                         )
                     else:
                         raise NoSupplierFoundError(f"invalid binding type {requirement}")
                 except NoSupplierFoundError as e:
                     errors.append(e)
             if not suppliers:
+                client_name = client.name or client.__class__.__name__
                 if optional:
                     supplier = None
                 elif len(errors) == 1:
-                    raise errors[0]
+                    err = errors[0]
+                    err_cls = type(err)
+                    raise err_cls(f"binding {client_name} failed: {err}") from err
                 else:
                     raise NoSupplierFoundError(
-                        f"no supplier matching {requirements} found in {self} (errors: {errors})"
+                        f"binding {client_name} failed: no supplier matching {requirements} found in {self} (errors: {errors})"
                     )
             elif len(suppliers) > 1:
                 raise NoSupplierFoundError(f"conflicting suppliers matching {requirements} found in target {self}")  # pylint: disable=line-too-long
             else:
                 supplier = suppliers[0]
             if supplier is not None and (requirement, supplier) in bound_req_pairs:
                 raise BindingError(
```

### Comparing `labgrid-23.1a2/labgrid/util/agent.py` & `labgrid-24.0a1/labgrid/util/agent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/agents/deditec_relais8.py` & `labgrid-24.0a1/labgrid/util/agents/deditec_relais8.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/agents/network_interface.py` & `labgrid-24.0a1/labgrid/util/agents/network_interface.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/agents/sysfsgpio.py` & `labgrid-24.0a1/labgrid/util/agents/sysfsgpio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/agents/usb_hid_relay.py` & `labgrid-24.0a1/labgrid/util/agents/usb_hid_relay.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/agentwrapper.py` & `labgrid-24.0a1/labgrid/util/agentwrapper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/dict.py` & `labgrid-24.0a1/labgrid/util/dict.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/expect.py` & `labgrid-24.0a1/labgrid/util/expect.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/helper.py` & `labgrid-24.0a1/labgrid/util/helper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/managedfile.py` & `labgrid-24.0a1/labgrid/util/managedfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import logging
 import os
 import subprocess
+from importlib import import_module
 
 import attr
 
 from .helper import get_user
 from .ssh import sshmanager
 from ..resource.common import Resource, NetworkResource
 from ..driver.exception import ExecutionError
@@ -26,15 +27,15 @@
 
         ManagedFile("/tmp/examplefile", <your-resource>)
 
     Synchronisation is done with the sync_to_resource method.
     """
     local_path = attr.ib(
         validator=attr.validators.instance_of(str),
-        converter=lambda x: os.path.abspath(str(x))
+        converter=lambda x: os.path.realpath(str(x))
     )
     resource = attr.ib(
         validator=attr.validators.instance_of(Resource),
     )
     detect_nfs = attr.ib(default=True, validator=attr.validators.instance_of(bool))
 
     def __attrs_post_init__(self):
@@ -55,15 +56,15 @@
             host = self.resource.host
             conn = sshmanager.open(host)
 
             if self._on_nfs(conn):
                 self.logger.info("File %s is accessible on %s, skipping copy", self.local_path, host)
                 self.rpath = os.path.dirname(self.local_path) + "/"
             else:
-                self.rpath = f"/var/cache/labgrid/{get_user()}/{self.get_hash()}/"
+                self.rpath = f"{self.get_user_cache_path()}/{self.get_hash()}/"
                 self.logger.info("Synchronizing %s to %s", self.local_path, host)
                 conn.run_check(f"mkdir -p {self.rpath}")
                 conn.put_file(
                     self.local_path,
                     f"{self.rpath}{os.path.basename(self.local_path)}"
                 )
 
@@ -84,16 +85,24 @@
 
         if not self.detect_nfs:
             return False
 
         self._on_nfs_cached = False
 
         fmt = "inode=%i,size=%s,modified=%Y"
-        local = subprocess.run(["stat", "--format", fmt, self.local_path],
-                               stdout=subprocess.PIPE)
+        # The stat command is very different on MacOs
+        platform = import_module('platform')
+        if platform.system() == 'Darwin':
+            darwin_fmt = "inode=%i,size=%z,modified=%m"
+            local = subprocess.run(["stat", "-f", darwin_fmt, self.local_path],
+                                   stdout=subprocess.PIPE)
+        else:
+            local = subprocess.run(["stat", "--format", fmt, self.local_path],
+                                   stdout=subprocess.PIPE)
+
         if local.returncode != 0:
             self.logger.debug("local: stat: unsuccessful error code %d", local.returncode)
             return False
 
         remote = conn.run(f"stat --format '{fmt}' {self.local_path}",
                           decodeerrors="backslashreplace")
         if remote[2] != 0:
@@ -137,7 +146,10 @@
         hasher = hashlib.sha256()
         with open(self.local_path, 'rb') as f:
             for block in iter(lambda: f.read(1048576), b''):
                 hasher.update(block)
         self.hash = hasher.hexdigest()
 
         return self.hash
+
+    def get_user_cache_path(self):
+        return f"/var/cache/labgrid/{get_user()}"
```

### Comparing `labgrid-23.1a2/labgrid/util/proxy.py` & `labgrid-24.0a1/labgrid/util/proxy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/qmp.py` & `labgrid-24.0a1/labgrid/util/qmp.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @attr.s(eq=False)
 class QMPMonitor:
     monitor_out = attr.ib()
     monitor_in = attr.ib()
 
     def __attrs_post_init__(self):
-        self.logger = logging.getLogger(f"{self}:")
+        self.logger = logging.getLogger(f"{self}")
         self._negotiate_capabilities()
 
     def _negotiate_capabilities(self):
         greeting = self._read_parse_json()
         if not greeting.get('QMP'):
             raise QMPError("QMP greeting message invalid")
```

### Comparing `labgrid-23.1a2/labgrid/util/ssh.py` & `labgrid-24.0a1/labgrid/util/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,16 +449,16 @@
             args,
             stdin=subprocess.DEVNULL,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
 
         try:
-            if self._master.wait(timeout=connect_timeout) != 0:
-                stdout, stderr = self._master.communicate()
+            stdout, stderr = self._master.communicate(timeout=connect_timeout)
+            if self._master.returncode != 0:
                 raise ExecutionError(
                     f"failed to connect to {self.host} with args {args}, returncode={self._master.returncode} {stdout},{stderr}"  # pylint: disable=line-too-long
                 )
         except subprocess.TimeoutExpired:
             self._master.kill()
             stdout, stderr = self._master.communicate()
             raise ExecutionError(
```

### Comparing `labgrid-23.1a2/labgrid/util/timeout.py` & `labgrid-24.0a1/labgrid/util/timeout.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid/util/yaml.py` & `labgrid-24.0a1/labgrid/util/yaml.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/labgrid.egg-info/SOURCES.txt` & `labgrid-24.0a1/labgrid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 .github/pull_request_template.md
 .github/workflows/build-and-release.yml
 .github/workflows/docker.yml
 .github/workflows/push-pr-unit-tests.yml
 .github/workflows/reusable-unit-tests-docker.yml
 .github/workflows/reusable-unit-tests.yml
 .github/workflows/scheduled-unit-tests.yml
+contrib/README.rst
 contrib/coordinator-statsd.py
+contrib/labgrid-webapp
+contrib/requirements-webapp.txt
 contrib/sync-places.py
 contrib/completion/labgrid-client.bash
 contrib/systemd/labgrid-coordinator.service
 contrib/systemd/labgrid-exporter.service
 contrib/systemd/sysusers.d/labgrid.conf
 contrib/systemd/tmpfiles.d/labgrid.conf
 debian/changelog
@@ -93,14 +96,16 @@
 examples/docker/env.yaml
 examples/docker/test_shell.py
 examples/library/phytec.yaml
 examples/library/test.py
 examples/modbusrtu/conftest.py
 examples/modbusrtu/env.yaml
 examples/modbusrtu/test_modbusrtu_example.py
+examples/network-test/env.yaml
+examples/network-test/pkg-replay-record.py
 examples/networkmanager/nm.env
 examples/networkmanager/nm.py
 examples/power/env.yaml
 examples/power/power_example.py
 examples/pyvisa/env.yaml
 examples/pyvisa/pyvisa_example.py
 examples/qemu-networking/conftest.py
@@ -111,14 +116,16 @@
 examples/remote/test_barebox.py
 examples/shell/conftest.py
 examples/shell/local.yaml
 examples/shell/test_hwclock.py
 examples/shell/test_memory.py
 examples/shell/test_rt.py
 examples/shell/test_shell.py
+examples/sigrok/env.yaml
+examples/sigrok/main.py
 examples/strategy/bareboxrebootstrategy.py
 examples/strategy/local.yaml
 examples/strategy/quartusstrategy.py
 examples/strategy/test_barebox_strategy.py
 examples/strategy/test_uboot_strategy.py
 examples/sysfsgpio/export-gpio.yaml
 examples/sysfsgpio/import-gpio.yaml
@@ -134,14 +141,15 @@
 examples/usbpower/exports.yaml
 examples/usbpower/local.yaml
 examples/usbpower/remote.yaml
 examples/usbpower/test_example.py
 examples/usbsdmux/local.yaml
 examples/usbsdmux/test_sdmux.py
 helpers/labgrid-bound-connect
+helpers/labgrid-raw-interface
 labgrid/__init__.py
 labgrid/binding.py
 labgrid/config.py
 labgrid/consoleloggingreporter.py
 labgrid/environment.py
 labgrid/exceptions.py
 labgrid/factory.py
@@ -170,14 +178,15 @@
 labgrid/driver/externalconsoledriver.py
 labgrid/driver/fake.py
 labgrid/driver/fastbootdriver.py
 labgrid/driver/filedigitaloutput.py
 labgrid/driver/flashromdriver.py
 labgrid/driver/flashscriptdriver.py
 labgrid/driver/gpiodriver.py
+labgrid/driver/httpdigitaloutput.py
 labgrid/driver/httpvideodriver.py
 labgrid/driver/lxaiobusdriver.py
 labgrid/driver/lxausbmuxdriver.py
 labgrid/driver/manualswitchdriver.py
 labgrid/driver/modbusdriver.py
 labgrid/driver/modbusrtudriver.py
 labgrid/driver/mqtt.py
@@ -185,14 +194,15 @@
 labgrid/driver/onewiredriver.py
 labgrid/driver/openocddriver.py
 labgrid/driver/powerdriver.py
 labgrid/driver/provider.py
 labgrid/driver/pyvisadriver.py
 labgrid/driver/qemudriver.py
 labgrid/driver/quartushpsdriver.py
+labgrid/driver/rawnetworkinterfacedriver.py
 labgrid/driver/resetdriver.py
 labgrid/driver/serialdigitaloutput.py
 labgrid/driver/serialdriver.py
 labgrid/driver/shelldriver.py
 labgrid/driver/sigrokdriver.py
 labgrid/driver/smallubootdriver.py
 labgrid/driver/sshdriver.py
@@ -208,21 +218,24 @@
 labgrid/driver/xenadriver.py
 labgrid/driver/power/__init__.py
 labgrid/driver/power/apc.py
 labgrid/driver/power/digipower.py
 labgrid/driver/power/digitalloggers_http.py
 labgrid/driver/power/eaton.py
 labgrid/driver/power/eg_pms2_network.py
+labgrid/driver/power/eth008.py
 labgrid/driver/power/gude.py
 labgrid/driver/power/gude24.py
 labgrid/driver/power/gude8031.py
 labgrid/driver/power/gude8225.py
 labgrid/driver/power/gude8316.py
 labgrid/driver/power/netio.py
 labgrid/driver/power/netio_kshell.py
+labgrid/driver/power/poe_mib.py
+labgrid/driver/power/raritan.py
 labgrid/driver/power/rest.py
 labgrid/driver/power/sentry.py
 labgrid/driver/power/shelly_gen1.py
 labgrid/driver/power/siglent.py
 labgrid/driver/power/simplerest.py
 labgrid/driver/power/tplink.py
 labgrid/driver/usbtmc/__init__.py
@@ -241,29 +254,29 @@
 labgrid/protocol/powerprotocol.py
 labgrid/protocol/resetprotocol.py
 labgrid/protocol/videoprotocol.py
 labgrid/pytestplugin/__init__.py
 labgrid/pytestplugin/fixtures.py
 labgrid/pytestplugin/hooks.py
 labgrid/remote/__init__.py
-labgrid/remote/authenticator.py
 labgrid/remote/client.py
 labgrid/remote/common.py
 labgrid/remote/config.py
 labgrid/remote/coordinator.py
 labgrid/remote/exporter.py
 labgrid/remote/scheduler.py
 labgrid/resource/__init__.py
 labgrid/resource/base.py
 labgrid/resource/common.py
 labgrid/resource/dediprogflasher.py
 labgrid/resource/docker.py
 labgrid/resource/ethernetport.py
 labgrid/resource/fastboot.py
 labgrid/resource/flashrom.py
+labgrid/resource/httpdigitalout.py
 labgrid/resource/httpvideostream.py
 labgrid/resource/lxaiobus.py
 labgrid/resource/modbus.py
 labgrid/resource/modbusrtu.py
 labgrid/resource/mqtt.py
 labgrid/resource/networkservice.py
 labgrid/resource/onewireport.py
@@ -292,22 +305,25 @@
 labgrid/util/exceptions.py
 labgrid/util/expect.py
 labgrid/util/helper.py
 labgrid/util/managedfile.py
 labgrid/util/marker.py
 labgrid/util/proxy.py
 labgrid/util/qmp.py
+labgrid/util/snmp.py
 labgrid/util/ssh.py
 labgrid/util/timeout.py
+labgrid/util/version.py
 labgrid/util/yaml.py
 labgrid/util/agents/__init__.py
 labgrid/util/agents/deditec_relais8.py
 labgrid/util/agents/dummy.py
 labgrid/util/agents/network_interface.py
 labgrid/util/agents/sysfsgpio.py
+labgrid/util/agents/udisks2.py
 labgrid/util/agents/usb_hid_relay.py
 man/Makefile
 man/labgrid-client.1
 man/labgrid-client.rst
 man/labgrid-device-config.5
 man/labgrid-device-config.rst
 man/labgrid-exporter.1
@@ -331,14 +347,15 @@
 tests/test_factory.py
 tests/test_filedigitaloutput.py
 tests/test_fixtures.py
 tests/test_flags.py
 tests/test_flashrom.py
 tests/test_flashscript.py
 tests/test_graphstrategy.py
+tests/test_httpdigitalout.py
 tests/test_httpvideo.py
 tests/test_lxaiobus.py
 tests/test_manualswitchdriver.py
 tests/test_modbusrtudriver.py
 tests/test_onewire.py
 tests/test_openocd.py
 tests/test_powerdriver.py
```

### Comparing `labgrid-23.1a2/labgrid.egg-info/requires.txt` & `labgrid-24.0a1/labgrid.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,75 +3,74 @@
 autobahn>=21.3.1
 jinja2>=3.0.2
 pexpect>=4.8.0
 pyserial-labgrid>=3.4.0.1
 pytest>=7.0.0
 pyudev>=0.22.0
 pyusb>=1.2.1
-PyYAML>=5.4.1
+PyYAML>=6.0.1
 requests>=2.26.0
 xmodem>=0.4.6
 
 [deb]
 pyModbusTCP>=0.1.10
 onewire>=0.2
-pysnmp>=4.4.12
-pysnmp-mibs>=0.1.6
+pysnmp-lextudio<6,>=4.4.12
 
 [dev]
 sphinx_rtd_theme>=1.0.0
+Sphinx>=2.0.0
 docker>=5.0.2
 graphviz>=0.17.0
 python-kasa>=0.4.0
 pyModbusTCP>=0.1.10
 minimalmodbus>=1.0.2
-paho-mqtt>=1.5.1
+paho-mqtt>=2.0.0
 onewire>=0.2
 pyvisa>=1.11.3
 PyVISA-py>=0.5.2
-pysnmp>=4.4.12
-pysnmp-mibs>=0.1.6
+pysnmp-lextudio<6,>=4.4.12
 python-vxi11>=0.9
 psutil>=5.8.0
 pytest-cov>=3.0.0
 pytest-dependency>=0.5.1
 pytest-isort>=2.0.0
 pytest-mock>=3.6.1
-pytest-pylint>=0.18.0
+pylint>=3.0.0
 
 [doc]
 sphinx_rtd_theme>=1.0.0
+Sphinx>=2.0.0
 
 [docker]
 docker>=5.0.2
 
 [graph]
 graphviz>=0.17.0
 
 [kasa]
 python-kasa>=0.4.0
 
 [modbus]
-pyModbusTCP>=0.1.10
+pyModbusTCP>=0.2.0
 
 [modbusrtu]
 minimalmodbus>=1.0.2
 
 [mqtt]
-paho-mqtt>=1.5.1
+paho-mqtt>=2.0.0
 
 [onewire]
 onewire>=0.2
 
 [pyvisa]
 pyvisa>=1.11.3
 PyVISA-py>=0.5.2
 
 [snmp]
-pysnmp>=4.4.12
-pysnmp-mibs>=0.1.6
+pysnmp-lextudio<6,>=4.4.12
 
 [vxi11]
 python-vxi11>=0.9
 
 [xena]
 xenavalkyrie>=3.0.1
```

### Comparing `labgrid-23.1a2/labgrid_logo.png` & `labgrid-24.0a1/labgrid_logo.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/man/labgrid-client.1` & `labgrid-24.0a1/man/labgrid-client.1`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 meaning it may be acquired by another user or
 not at all.
 .UNINDENT
 .UNINDENT
 .sp
 \fBenv\fP                         Generate a labgrid environment file for a place
 .sp
-\fBpower (pw)\fP action           Change (or get) a place\(aqs power status, where action is one of get, on, off, status
+\fBpower (pw)\fP action           Change (or get) a place\(aqs power status, where action is one of get, on, off, cycle
 .sp
 \fBio\fP action                   Interact with GPIO (OneWire, relays, ...) devices, where action is one of high, low, get
 .sp
 \fBconsole (con)\fP               Connect to the console
 .sp
 \fBdfu\fP arg                     Run dfu commands
 .sp
@@ -215,25 +215,29 @@
 .sp
 \fBvideo\fP                       Start a video stream
 .sp
 \fBaudio\fP                       Start an audio stream
 .sp
 \fBtmc\fP command                 Control a USB TMC device
 .sp
+\fBwrite\-files\fP filename(s)     Copy files onto mass storage device
+.sp
 \fBwrite\-image\fP                 Write images onto block devices (USBSDMux, USB Sticks, …)
 .sp
 \fBreserve\fP filter              Create a reservation
 .sp
 \fBcancel\-reservation\fP token    Cancel a pending reservation
 .sp
 \fBwait\fP token                  Wait for a reservation to be allocated
 .sp
 \fBreservations\fP                List current reservations
 .sp
 \fBexport\fP filename             Export driver information to file (needs environment with drivers)
+.sp
+\fBversion\fP                     Print the labgrid version
 .SH ADDING NAMED RESOURCES
 .sp
 If a target contains multiple Resources of the same type, named matches need to
 be used to address the individual resources. In addition to the \fImatch\fP taken by
 \fIadd\-match\fP, \fIadd\-named\-match\fP also takes a name for the resource. The other
 client commands support the name as an optional parameter and will inform the
 user that a name is required if multiple resources are found, but no name is
```

### Comparing `labgrid-23.1a2/man/labgrid-client.rst` & `labgrid-24.0a1/man/labgrid-client.rst`

 * *Files 3% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                                 Note that this command returns success as long
                                 as the specified user no longer owns the place,
                                 meaning it may be acquired by another user or
                                 not at all.
 
 ``env``                         Generate a labgrid environment file for a place
 
-``power (pw)`` action           Change (or get) a place's power status, where action is one of get, on, off, status
+``power (pw)`` action           Change (or get) a place's power status, where action is one of get, on, off, cycle
 
 ``io`` action                   Interact with GPIO (OneWire, relays, ...) devices, where action is one of high, low, get
 
 ``console (con)``               Connect to the console
 
 ``dfu`` arg                     Run dfu commands
 
@@ -207,26 +207,30 @@
 
 ``video``                       Start a video stream
 
 ``audio``                       Start an audio stream
 
 ``tmc`` command                 Control a USB TMC device
 
+``write-files`` filename(s)     Copy files onto mass storage device
+
 ``write-image``                 Write images onto block devices (USBSDMux, USB Sticks, …)
 
 ``reserve`` filter              Create a reservation
 
 ``cancel-reservation`` token    Cancel a pending reservation
 
 ``wait`` token                  Wait for a reservation to be allocated
 
 ``reservations``                List current reservations
 
 ``export`` filename             Export driver information to file (needs environment with drivers)
 
+``version``                     Print the labgrid version
+
 ADDING NAMED RESOURCES
 ----------------------
 If a target contains multiple Resources of the same type, named matches need to
 be used to address the individual resources. In addition to the `match` taken by
 `add-match`, `add-named-match` also takes a name for the resource. The other
 client commands support the name as an optional parameter and will inform the
 user that a name is required if multiple resources are found, but no name is
```

### Comparing `labgrid-23.1a2/man/labgrid-device-config.5` & `labgrid-24.0a1/man/labgrid-device-config.5`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,18 @@
 .B \fBusbsdmux\fP
 Path to the usbsdmux tool, used by the USBSDMuxDriver.
 See: \fI\%https://github.com/linux\-automation/usbsdmux\fP
 .TP
 .B \fBuuu\-loader\fP
 Path to the uuu\-loader binary, used by the UUUDriver.
 See: \fI\%https://github.com/nxp\-imx/mfgtools\fP
+.TP
+.B \fBykushcmd\fP
+Path to the ykushcmd binary, used by the YKUSHPowerDriver.
+See: \fI\%https://github.com/Yepkit/ykush\fP
 .UNINDENT
 .sp
 The QEMUDriver expects a custom key set via its \fBqemu_bin\fP argument.
 See \fI\%https://www.qemu.org/\fP
 .SS TOOLS EXAMPLE
 .sp
 Configure the tool path for \fBimx\-usb\-loader\fP:
@@ -258,14 +262,14 @@
 .sp
 \fBlabgrid\-client\fP(1), \fBlabgrid\-exporter\fP(1)
 .SH AUTHOR
 Rouven Czerwinski <r.czerwinski@pengutronix.de>
 
 Organization: Labgrid-Project
 .SH COPYRIGHT
-Copyright (C) 2016-2023 Pengutronix. This library is free software;
+Copyright (C) 2016-2024 Pengutronix. This library is free software;
 you can redistribute it and/or modify it under the terms of the GNU
 Lesser General Public License as published by the Free Software
 Foundation; either version 2.1 of the License, or (at your option)
 any later version.
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `labgrid-23.1a2/man/labgrid-device-config.rst` & `labgrid-24.0a1/man/labgrid-device-config.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 labgrid test configuration files
 ================================
 
 
 :Author: Rouven Czerwinski <r.czerwinski@pengutronix.de>
 :organization: Labgrid-Project
 :Date:   2017-04-15
-:Copyright: Copyright (C) 2016-2023 Pengutronix. This library is free software;
+:Copyright: Copyright (C) 2016-2024 Pengutronix. This library is free software;
             you can redistribute it and/or modify it under the terms of the GNU
             Lesser General Public License as published by the Free Software
             Foundation; either version 2.1 of the License, or (at your option)
             any later version.
 :Version: 0.0.1
 :Manual section: 5
 :Manual group: embedded testing
@@ -155,14 +155,18 @@
     Path to the usbsdmux tool, used by the USBSDMuxDriver.
     See: https://github.com/linux-automation/usbsdmux
 
 ``uuu-loader``
     Path to the uuu-loader binary, used by the UUUDriver.
     See: https://github.com/nxp-imx/mfgtools
 
+``ykushcmd``
+    Path to the ykushcmd binary, used by the YKUSHPowerDriver.
+    See: https://github.com/Yepkit/ykush
+
 The QEMUDriver expects a custom key set via its ``qemu_bin`` argument.
 See https://www.qemu.org/
 
 TOOLS EXAMPLE
 ~~~~~~~~~~~~~~
 Configure the tool path for ``imx-usb-loader``:
```

### Comparing `labgrid-23.1a2/man/labgrid-exporter.1` & `labgrid-24.0a1/man/labgrid-exporter.1`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 .TP
 .B  \-n\fP,\fB  \-\-name
 the public name of the exporter
 .TP
 .B  \-\-hostname
 hostname (or IP) published for accessing resources
 .TP
+.B  \-\-fqdn
+use fully qualified domain name as default for hostname
+.TP
 .B  \-d\fP,\fB  \-\-debug
 enable debug mode
 .UNINDENT
 .SS \-i / \-\-isolated
 .sp
 This option enables isolated mode, which causes all exported resources being
 marked as requiring SSH connection forwarding.
@@ -79,14 +82,19 @@
 .SS \-\-hostname
 .sp
 For resources like USBSerialPort, USBGenericExport or USBSigrokExport, the
 exporter needs to provide a host name to set the exported value of the \(dqhost\(dq
 key.
 If the system hostname is not resolvable via DNS, this option can be used to
 override this default with another name (or an IP address).
+.SS \-\-fqdn
+.sp
+In some networks the fully qualified domain name may be needed to reach resources
+on an exporter. This option changes the default to fqdn when no \-\-hostname is
+explicitly set.
 .SH CONFIGURATION
 .sp
 The exporter uses a YAML configuration file which defines groups of related
 resources.
 See <\fI\%https://labgrid.readthedocs.io/en/latest/configuration.html#exporter\-configuration\fP>
 for more information.
 .SH ENVIRONMENT VARIABLES
@@ -129,14 +137,14 @@
 .sp
 \fBlabgrid\-client\fP(1), \fBlabgrid\-device\-config\fP(5)
 .SH AUTHOR
 Rouven Czerwinski <r.czerwinski@pengutronix.de>
 
 Organization: Labgrid-Project
 .SH COPYRIGHT
-Copyright (C) 2016-2023 Pengutronix. This library is free software;
+Copyright (C) 2016-2024 Pengutronix. This library is free software;
 you can redistribute it and/or modify it under the terms of the GNU
 Lesser General Public License as published by the Free Software
 Foundation; either version 2.1 of the License, or (at your option)
 any later version.
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `labgrid-23.1a2/man/labgrid-exporter.rst` & `labgrid-24.0a1/man/labgrid-exporter.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 labgrid-exporter interface to control boards
 ============================================
 
 
 :Author: Rouven Czerwinski <r.czerwinski@pengutronix.de>
 :organization: Labgrid-Project
 :Date:   2017-04-15
-:Copyright: Copyright (C) 2016-2023 Pengutronix. This library is free software;
+:Copyright: Copyright (C) 2016-2024 Pengutronix. This library is free software;
             you can redistribute it and/or modify it under the terms of the GNU
             Lesser General Public License as published by the Free Software
             Foundation; either version 2.1 of the License, or (at your option)
             any later version.
 :Version: 0.0.1
 :Manual section: 1
 :Manual group: embedded testing
@@ -42,14 +42,16 @@
     the crossbar url of the coordinator
 -i, --isolated
     enable isolated mode (always request SSH forwards)
 -n, --name
     the public name of the exporter
 --hostname
     hostname (or IP) published for accessing resources
+--fqdn
+    use fully qualified domain name as default for hostname
 -d, --debug
     enable debug mode
 
 -i / --isolated
 ~~~~~~~~~~~~~~~
 This option enables isolated mode, which causes all exported resources being
 marked as requiring SSH connection forwarding.
@@ -69,14 +71,20 @@
 ~~~~~~~~~~
 For resources like USBSerialPort, USBGenericExport or USBSigrokExport, the
 exporter needs to provide a host name to set the exported value of the "host"
 key.
 If the system hostname is not resolvable via DNS, this option can be used to
 override this default with another name (or an IP address).
 
+--fqdn
+~~~~~~
+In some networks the fully qualified domain name may be needed to reach resources
+on an exporter. This option changes the default to fqdn when no --hostname is
+explicitly set.
+
 CONFIGURATION
 -------------
 The exporter uses a YAML configuration file which defines groups of related
 resources.
 See <https://labgrid.readthedocs.io/en/latest/configuration.html#exporter-configuration>
 for more information.
```

### Comparing `labgrid-23.1a2/man/labgrid-pytest.7` & `labgrid-24.0a1/man/labgrid-pytest.7`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,14 @@
 .sp
 \fBlabgrid\-device\-config\fP(5)
 .SH AUTHOR
 Rouven Czerwinski <r.czerwinski@pengutronix.de>
 
 Organization: Labgrid-Project
 .SH COPYRIGHT
-Copyright (C) 2016-2023 Pengutronix. This library is free software;
+Copyright (C) 2016-2024 Pengutronix. This library is free software;
 you can redistribute it and/or modify it under the terms of the GNU
 Lesser General Public License as published by the Free Software
 Foundation; either version 2.1 of the License, or (at your option)
 any later version.
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `labgrid-23.1a2/man/labgrid-pytest.rst` & `labgrid-24.0a1/man/labgrid-pytest.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 labgrid-pytest labgrid integration for pytest
 =============================================
 
 :Author: Rouven Czerwinski <r.czerwinski@pengutronix.de>
 :organization: Labgrid-Project
 :Date:   2017-04-15
-:Copyright: Copyright (C) 2016-2023 Pengutronix. This library is free software;
+:Copyright: Copyright (C) 2016-2024 Pengutronix. This library is free software;
             you can redistribute it and/or modify it under the terms of the GNU
             Lesser General Public License as published by the Free Software
             Foundation; either version 2.1 of the License, or (at your option)
             any later version.
 :Version: 0.0.1
 :Manual section: 7
 :Manual group: embedded testing
```

### Comparing `labgrid-23.1a2/man/labgrid-suggest.1` & `labgrid-24.0a1/man/labgrid-suggest.1`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,14 @@
 .UNINDENT
 .SH SEE ALSO
 .sp
 \fBlabgrid\-device\-config\fP(5)
 
 Organization: Labgrid-Project
 .SH COPYRIGHT
-Copyright (C) 2016-2023 Pengutronix. This library is free software;
+Copyright (C) 2016-2024 Pengutronix. This library is free software;
 you can redistribute it and/or modify it under the terms of the GNU
 Lesser General Public License as published by the Free Software
 Foundation; either version 2.1 of the License, or (at your option)
 any later version.
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `labgrid-23.1a2/man/labgrid-suggest.rst` & `labgrid-24.0a1/man/labgrid-suggest.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 labgrid-suggest generator for YAML config files
 ===============================================
 
 
 :organization: Labgrid-Project
 :Date:   2021-05-20
-:Copyright: Copyright (C) 2016-2023 Pengutronix. This library is free software;
+:Copyright: Copyright (C) 2016-2024 Pengutronix. This library is free software;
             you can redistribute it and/or modify it under the terms of the GNU
             Lesser General Public License as published by the Free Software
             Foundation; either version 2.1 of the License, or (at your option)
             any later version.
 :Version: 0.0.1
 :Manual section: 1
 :Manual group: embedded testing
```

### Comparing `labgrid-23.1a2/pyproject.toml` & `labgrid-24.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,76 +14,80 @@
   { name="Jan Luebbe", email="entwicklung@pengutronix.de" },
 ]
 description = "embedded systems control library for development, testing and installation"
 readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
+    "Intended Audience :: Developers",
+    "Development Status :: 5 - Production/Stable",
+    "Operating System :: POSIX :: Linux",
     "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
 ]
 dependencies = [
     "ansicolors>=1.1.8",
     "attrs>=21.4.0",
     "autobahn>=21.3.1",
     "jinja2>=3.0.2",
     "pexpect>=4.8.0",
     "pyserial-labgrid>=3.4.0.1",
     "pytest>=7.0.0",
     "pyudev>=0.22.0",
     "pyusb>=1.2.1",
-    "PyYAML>=5.4.1",
+    "PyYAML>=6.0.1",
     "requests>=2.26.0",
     "xmodem>=0.4.6",
 ]
 dynamic = ["version"]  # via setuptools_scm
 
 [project.urls]
 "Homepage" = "https://github.com/labgrid-project/labgrid"
 "Bug Tracker" = "https://github.com/labgrid-project/labgrid/issues"
 
 [project.optional-dependencies]
-doc = ["sphinx_rtd_theme>=1.0.0"]
+doc = [
+    "sphinx_rtd_theme>=1.0.0",
+    "Sphinx>=2.0.0",
+]
 docker = ["docker>=5.0.2"]
 graph = ["graphviz>=0.17.0"]
 kasa = ["python-kasa>=0.4.0"]
-modbus = ["pyModbusTCP>=0.1.10"]
+modbus = ["pyModbusTCP>=0.2.0"]
 modbusrtu = ["minimalmodbus>=1.0.2"]
-mqtt = ["paho-mqtt>=1.5.1"]
+mqtt = ["paho-mqtt>=2.0.0"]
 onewire = ["onewire>=0.2"]
 pyvisa = [
     "pyvisa>=1.11.3",
     "PyVISA-py>=0.5.2",
 ]
-snmp = [
-    "pysnmp>=4.4.12",
-    "pysnmp-mibs>=0.1.6",
-]
+snmp = ["pysnmp-lextudio>=4.4.12, <6"]
 vxi11 = ["python-vxi11>=0.9"]
 xena = ["xenavalkyrie>=3.0.1"]
 deb = [
     # labgrid[modbus]
     "pyModbusTCP>=0.1.10",
 
     # labgrid[onewire]
     "onewire>=0.2",
 
     # labgrid[snmp]
-    "pysnmp>=4.4.12",
-    "pysnmp-mibs>=0.1.6",
+    "pysnmp-lextudio>=4.4.12, <6",
 ]
 dev = [
     # references to other optional dependency groups
     # labgrid[doc]
     "sphinx_rtd_theme>=1.0.0",
+    "Sphinx>=2.0.0",
 
     # labgrid[docker]
     "docker>=5.0.2",
 
     # labgrid[graph]
     "graphviz>=0.17.0",
 
@@ -93,37 +97,36 @@
     # labgrid[modbus]
     "pyModbusTCP>=0.1.10",
 
     # labgrid[modbusrtu]
     "minimalmodbus>=1.0.2",
 
     # labgrid[mqtt]
-    "paho-mqtt>=1.5.1",
+    "paho-mqtt>=2.0.0",
 
     # labgrid[onewire]
     "onewire>=0.2",
 
     # labgrid[pyvisa]
     "pyvisa>=1.11.3",
     "PyVISA-py>=0.5.2",
 
     # labgrid[snmp]
-    "pysnmp>=4.4.12",
-    "pysnmp-mibs>=0.1.6",
+    "pysnmp-lextudio>=4.4.12, <6",
 
     # labgrid[vxi11]
     "python-vxi11>=0.9",
 
     # additional dev dependencies
     "psutil>=5.8.0",
     "pytest-cov>=3.0.0",
     "pytest-dependency>=0.5.1",
     "pytest-isort>=2.0.0",
     "pytest-mock>=3.6.1",
-    "pytest-pylint>=0.18.0",
+    "pylint>=3.0.0",
 ]
 
 [project.scripts]
 labgrid-autoinstall = "labgrid.autoinstall.main:main"
 labgrid-client = "labgrid.remote.client:main"
 labgrid-exporter = "labgrid.remote.exporter:main"
 labgrid-suggest = "labgrid.resource.suggest:main"
@@ -154,17 +157,14 @@
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
     "labgrid",
 ]
 addopts = "-p no:labgrid"
 
-[tool.pylint.MASTER]
-ignore-paths = ["labgrid/remote/authenticator.py"]
-
 [tool.pylint.imports]
 ignored-modules = ["gi"]
 
 [tool.pylint."messages control"]
 # disable all, then enable explicitly
 disable = ["all"]
 enable = [
@@ -212,15 +212,15 @@
     "labgrid.strategy.*",
 ]
 signature-mutators = ["labgrid.step.step"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37, py38, py39, py310, py311
+envlist = py38, py39, py310, py311
 isolated_build = true
 
 [testenv]
 extras = dev
 passenv = TERM
 commands =
   pytest tests {posargs} \
```

### Comparing `labgrid-23.1a2/tests/conftest.py` & `labgrid-24.0a1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,21 @@
     Testport:
         NetworkSerialPort:
           host: 'localhost'
           port: 4000
     Broken:
         RawSerialPort:
           port: 'none'
+    Many:
+        NetworkSerialPort:
+          host: 'localhost'
+          port: 4000
+        NetworkService:
+          address: "192.168.0.1"
+          username: "root"
     """
     )
     spawn = pexpect.spawn(
             f'{sys.executable} -m labgrid.remote.exporter --name testhost exports.yaml',
             logfile=Prefixer(sys.stdout.buffer, 'exporter'),
             cwd=str(tmpdir))
     try:
```

### Comparing `labgrid-23.1a2/tests/test_agent.py` & `labgrid-24.0a1/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_autoinstall.py` & `labgrid-24.0a1/tests/test_autoinstall.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_bareboxdriver.py` & `labgrid-24.0a1/tests/test_bareboxdriver.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,23 +15,29 @@
         assert (isinstance(d, BareboxDriver))
         assert (isinstance(d, CommandProtocol))
         assert (isinstance(d, LinuxBootProtocol))
 
     def test_barebox_run(self, target_with_fakeconsole, mocker):
         t = target_with_fakeconsole
         d = BareboxDriver(t, "barebox")
-        d = t.get_driver(BareboxDriver)
+        d = t.get_driver(BareboxDriver, activate=False)
+        # mock for d._run('echo $global.loglevel')
+        d._run = mocker.MagicMock(return_value=(['7'], [], 0))
+        t.activate(d)
         d._run = mocker.MagicMock(return_value=(['success'], [], 0))
         res = d.run_check("test")
         assert res == ['success']
         res = d.run("test")
         assert res == (['success'], [], 0)
 
     def test_barebox_run_error(self, target_with_fakeconsole, mocker):
         t = target_with_fakeconsole
         d = BareboxDriver(t, "barebox")
-        d = t.get_driver(BareboxDriver)
+        d = t.get_driver(BareboxDriver, activate=False)
+        # mock for d._run('echo $global.loglevel')
+        d._run = mocker.MagicMock(return_value=(['7'], [], 0))
+        t.activate(d)
         d._run = mocker.MagicMock(return_value=(['error'], [], 1))
         with pytest.raises(ExecutionError):
             res = d.run_check("test")
         res = d.run("test")
         assert res == (['error'], [], 1)
```

### Comparing `labgrid-23.1a2/tests/test_config.py` & `labgrid-24.0a1/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,7 +96,34 @@
         """
         string: !template ${INVALID}
         """
     )
     with pytest.raises(InvalidConfigError) as excinfo:
         Config(str(p))
     assert "unknown variable" in excinfo.value.msg
+
+def test_tool(tmpdir):
+    t = tmpdir.join("testtool")
+    t.write("content")
+    p = tmpdir.join("config.yaml")
+    p.write(
+        """
+        tools:
+          testtool: {}
+        """.format(t)
+    )
+    c = Config(str(p))
+
+    assert c.get_tool("testtool") == t
+
+def test_tool_no_explicit_tool(tmpdir):
+    t = tmpdir.join("testtool")
+    t.write("content")
+    p = tmpdir.join("config.yaml")
+    p.write(
+        """
+        dict: {}
+        """
+    )
+    c = Config(str(p))
+
+    assert c.get_tool("testtool") == "testtool"
```

### Comparing `labgrid-23.1a2/tests/test_crossbar.py` & `labgrid-24.0a1/tests/test_crossbar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import sys
 import time
 
 import pytest
 import pexpect
 
 psutil = pytest.importorskip("psutil")
 
@@ -17,14 +18,15 @@
 
 def resume_tree(pid):
     main = psutil.Process(pid)
     main.resume()
     for child in main.children(recursive=True):
         child.resume()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_startup(crossbar):
     pass
 
 @pytest.fixture(scope='function')
 def place(crossbar):
     with pexpect.spawn('python -m labgrid.remote.client -p test create') as spawn:
         spawn.expect(pexpect.EOF)
@@ -65,57 +67,62 @@
 def test_connect_error():
     with pexpect.spawn('python -m labgrid.remote.client -x ws://127.0.0.1:20409/ws places') as spawn:
         spawn.expect("Could not connect to coordinator")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 1, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_connect_timeout(crossbar):
     suspend_tree(crossbar.pid)
     try:
         with pexpect.spawn('python -m labgrid.remote.client places') as spawn:
             spawn.expect("connection closed during setup")
             spawn.expect(pexpect.EOF)
             spawn.close()
             assert spawn.exitstatus == 1, spawn.before.strip()
     finally:
         resume_tree(crossbar.pid)
         pass
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_show(place):
     with pexpect.spawn('python -m labgrid.remote.client -p test show') as spawn:
         spawn.expect("Place 'test':")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_alias(place):
     with pexpect.spawn('python -m labgrid.remote.client -p test add-alias foo') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p foo del-alias foo') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_comment(place):
     with pexpect.spawn('python -m labgrid.remote.client -p test set-comment my comment') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test show') as spawn:
         spawn.expect("Place 'test':")
         spawn.expect(" comment: my comment")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_match(place):
     with pexpect.spawn('python -m labgrid.remote.client -p test add-match "e1/g1/r1" "e2/g2/*"') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test del-match "e1/g1/r1"') as spawn:
@@ -126,14 +133,15 @@
     with pexpect.spawn('python -m labgrid.remote.client -p test show') as spawn:
         spawn.expect(" matches:")
         spawn.expect(" e2/g2/*")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_match_duplicates(place):
     # first given match should succeed, second should be skipped
     matches = (
         ("e1/g1/r1", "e1/g1/r1"),
         ("e1/g1/r1/n1", "e1/g1/r1/n1"),
         ("e1/g1/r1/n1", "e1/g1/r1"),
         ("e1/g1/r1", "e1/g1/r1/n1"),
@@ -146,14 +154,15 @@
             assert spawn.exitstatus == 0, spawn.before.strip()
 
         with pexpect.spawn(f'python -m labgrid.remote.client -p test del-match "{match[0]}"') as spawn:
             spawn.expect(pexpect.EOF)
             spawn.close()
             assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_acquire(place):
     with pexpect.spawn('python -m labgrid.remote.client -p test acquire') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client who') as spawn:
@@ -163,14 +172,15 @@
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test release') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_acquire_enforce(place):
     with pexpect.spawn('python -m labgrid.remote.client -p test add-match does/not/exist') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test acquire') as spawn:
@@ -186,14 +196,15 @@
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test release') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_acquire_broken(place, exporter):
     with pexpect.spawn('python -m labgrid.remote.client -p test add-match "*/Broken/*"') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test acquire') as spawn:
@@ -205,14 +216,15 @@
     with pexpect.spawn('python -m labgrid.remote.client -p test show') as spawn:
         spawn.expect("'broken': 'start failed'")
         spawn.expect(pexpect.EOF)
         spawn.close()
         print(spawn.before.decode())
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_release_from(monkeypatch, place, exporter):
     user = "test-user"
     host = "test-host"
     monkeypatch.setenv("LG_USERNAME", user)
     monkeypatch.setenv("LG_HOSTNAME", host)
 
     # Acquire place
@@ -251,28 +263,31 @@
     with pexpect.spawn('python -m labgrid.remote.client who') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
         before = spawn.before.decode("utf-8").strip()
         assert user not in before and not host in before, before
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_add_no_name(crossbar):
     with pexpect.spawn('python -m labgrid.remote.client create') as spawn:
         spawn.expect("missing place name")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus != 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_place_del_no_name(crossbar):
     with pexpect.spawn('python -m labgrid.remote.client delete') as spawn:
         spawn.expect("deletes require an exact place name")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus != 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_remoteplace_target(place_acquire, tmpdir):
     from labgrid.environment import Environment
     p = tmpdir.join("config.yaml")
     p.write(
         """
     targets:
       test1:
@@ -282,21 +297,27 @@
             name: test
     """
     )
     e = Environment(str(p))
     t = e.get_target("test1")
     t.await_resources(t.resources)
 
+    remote_place = t.get_resource("RemotePlace")
+    assert remote_place.tags == {"board": "bar"}
+
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_remoteplace_target_without_env(request, place_acquire):
     from labgrid import Target
     from labgrid.resource import RemotePlace
 
     t = Target(request.node.name)
-    RemotePlace(t, name="test")
+    remote_place = RemotePlace(t, name="test")
+    assert remote_place.tags == {"board": "bar"}
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_resource_conflict(place_acquire, tmpdir):
     with pexpect.spawn('python -m labgrid.remote.client -p test2 create') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test2 add-match "*/Testport/*"') as spawn:
@@ -310,14 +331,15 @@
         assert spawn.exitstatus != 0, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test2 delete') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_reservation(place_acquire, tmpdir):
     with pexpect.spawn('python -m labgrid.remote.client reserve --shell board=bar name=test') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
         m = re.search(rb"^export LG_TOKEN=(\S+)$", spawn.before.replace(b'\r\n', b'\n'), re.MULTILINE)
         assert m is not None, spawn.before.strip()
@@ -387,14 +409,15 @@
         assert token not in spawn.before, spawn.before.strip()
 
     with pexpect.spawn('python -m labgrid.remote.client -p test acquire') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_exporter_timeout(place, exporter):
     with pexpect.spawn('python -m labgrid.remote.client resources') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
         assert b'/Testport/NetworkSerialPort' in spawn.before
 
@@ -424,14 +447,15 @@
     assert exporter.exitstatus == 100
 
     with pexpect.spawn('python -m labgrid.remote.client -p test release') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
 
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
 def test_reservation_custom_config(place, exporter, tmpdir):
     p = tmpdir.join("config.yaml")
     p.write(
     """
     targets:
       test1:
         role: foo
@@ -460,7 +484,36 @@
         assert spawn.exitstatus == 0, spawn.before.strip()
 
     with pexpect.spawn(f'python -m labgrid.remote.client -c {p} -p + release', env=env) as spawn:
         spawn.expect("released place test")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
+
+@pytest.mark.xfail(sys.version_info >= (3, 12), reason="latest crossbar release incompatible with python3.12+")
+def test_same_name_resources(place, exporter, tmpdir):
+    with pexpect.spawn('python -m labgrid.remote.client -p test add-named-match "testhost/Many/NetworkService" "samename"') as spawn:
+        spawn.expect(pexpect.EOF)
+        spawn.close()
+        assert spawn.exitstatus == 0, spawn.before.strip()
+
+    with pexpect.spawn('python -m labgrid.remote.client -p test add-named-match "testhost/Many/NetworkSerialPort" "samename"') as spawn:
+        spawn.expect(pexpect.EOF)
+        spawn.close()
+        assert spawn.exitstatus == 0, spawn.before.strip()
+
+    with pexpect.spawn('python -m labgrid.remote.client -p test acquire') as spawn:
+        spawn.expect(pexpect.EOF)
+        spawn.close()
+        assert spawn.exitstatus == 0, spawn.before.strip()
+
+    with pexpect.spawn('python -m labgrid.remote.client -p test env') as spawn:
+        spawn.expect(pexpect.EOF)
+        spawn.close()
+        assert spawn.exitstatus == 0, spawn.before.strip()
+        assert "NetworkService".encode("utf-8") in spawn.before.replace(b'\r\n', b'\n'), spawn.before.strip()
+        assert "NetworkSerialPort".encode("utf-8") in spawn.before.replace(b'\r\n', b'\n'), spawn.before.strip()
+
+    with pexpect.spawn('python -m labgrid.remote.client -p test release') as spawn:
+        spawn.expect(pexpect.EOF)
+        spawn.close()
+        assert spawn.exitstatus == 0, spawn.before.strip()
```

### Comparing `labgrid-23.1a2/tests/test_dediprogflasher.py` & `labgrid-24.0a1/tests/test_dediprogflasher.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_docker.py` & `labgrid-24.0a1/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_environment.py` & `labgrid-24.0a1/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_export.py` & `labgrid-24.0a1/tests/test_export.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from labgrid.resource import Resource, NetworkSerialPort
+from labgrid.resource import Resource, NetworkSerialPort, TFTPProvider
 from labgrid.resource.remote import RemoteNetworkInterface, RemoteTFTPProvider
 from labgrid.driver import Driver, SerialDriver, NetworkInterfaceDriver, TFTPProviderDriver
 from labgrid.strategy import Strategy
 from labgrid.binding import StateError
 
 
 class ResourceA(Resource):
@@ -84,14 +84,26 @@
     exported = target.export()
     assert exported == {
         'LG__NETIF_HOST': 'testhost',
         'LG__NETIF_IFNAME': 'wlan0'
     }
 
 
+def test_export_tftp_provider(target):
+    TFTPProvider(target, None, internal='/srv/tftp/testboard/', external='testboard/')
+    TFTPProviderDriver(target, "tftp")
+
+    exported = target.export()
+    assert exported == {
+        'LG__TFTP_HOST': 'localhost',
+        'LG__TFTP_INTERNAL': '/srv/tftp/testboard/',
+        'LG__TFTP_EXTERNAL': 'testboard/',
+    }
+
+
 def test_export_remote_tftp_provider(target):
     RemoteTFTPProvider(target, None, host='testhost', internal='/srv/tftp/testboard/', external='testboard/')
     TFTPProviderDriver(target, "tftp")
 
     exported = target.export()
     assert exported == {
         'LG__TFTP_HOST': 'testhost',
```

### Comparing `labgrid-23.1a2/tests/test_externalconsoledriver.py` & `labgrid-24.0a1/tests/test_externalconsoledriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_factory.py` & `labgrid-24.0a1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_filedigitaloutput.py` & `labgrid-24.0a1/tests/test_filedigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_fixtures.py` & `labgrid-24.0a1/tests/test_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
 def test_env_fixture(short_env, short_test):
     with pexpect.spawn(f'pytest --lg-env {short_env} {short_test}') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0
 
+def test_env_fixture_no_logging(short_env, short_test):
+    with pexpect.spawn(f'pytest -p no:logging --lg-env {short_env} {short_test}') as spawn:
+        spawn.expect(pexpect.EOF)
+        spawn.close()
+        assert spawn.exitstatus == 0, spawn.before
 
 def test_env_old_fixture(short_env, short_test):
     with pexpect.spawn(f'pytest --env-config {short_env} {short_test}') as spawn:
         spawn.expect("deprecated option --env-config")
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0
```

### Comparing `labgrid-23.1a2/tests/test_flags.py` & `labgrid-24.0a1/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_flashrom.py` & `labgrid-24.0a1/tests/test_flashrom.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_flashscript.py` & `labgrid-24.0a1/tests/test_flashscript.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 import subprocess
 import tempfile
 import attr
+import os
 from pathlib import Path
 from labgrid.driver.flashscriptdriver import FlashScriptDriver
 from labgrid.resource.common import ManagedResource
 from labgrid import target_factory
 
 
 @target_factory.reg_resource
@@ -65,8 +66,8 @@
 def test_argument_device_expansion(target, resource, driver):
     value = capture_argument_expansion(driver, "device.prop")
     assert value == resource.prop
 
 
 def test_argument_file_expansion(target, driver):
     value = capture_argument_expansion(driver, "file.local_path")
-    assert value == "/bin/sh"
+    assert os.path.samefile(value, "/bin/sh")
```

### Comparing `labgrid-23.1a2/tests/test_graphstrategy.py` & `labgrid-24.0a1/tests/test_graphstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_lxaiobus.py` & `labgrid-24.0a1/tests/test_lxaiobus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_manualswitchdriver.py` & `labgrid-24.0a1/tests/test_manualswitchdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_modbusrtudriver.py` & `labgrid-24.0a1/tests/test_modbusrtudriver.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,17 +20,16 @@
     assert dut.address == 10
     assert dut.speed == 9600
     assert dut.timeout == 0.5
 
 
 def test_driver(target, mocker):
     pytest.importorskip("minimalmodbus")
+    mocker.patch('serial.Serial')
+
     ModbusRTU(target, name=None, port="/dev/tty0", address=10)
     driver = ModbusRTUDriver(target, name=None)
 
-    # Ensure pyserial will not try to open the port
-    driver.resource.port = None
-
     target.activate(driver)
 
     assert driver.instrument.serial.baudrate == 115200
     assert driver.instrument.serial.timeout == 0.25
```

### Comparing `labgrid-23.1a2/tests/test_onewire.py` & `labgrid-24.0a1/tests/test_onewire.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_openocd.py` & `labgrid-24.0a1/tests/test_openocd.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_powerdriver.py` & `labgrid-24.0a1/tests/test_powerdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,15 @@
         get.assert_called_with(expected_host)
 
     def test_import_backends(self):
         import labgrid.driver.power
         import labgrid.driver.power.apc
         import labgrid.driver.power.digipower
         import labgrid.driver.power.digitalloggers_http
+        import labgrid.driver.power.eth008
         import labgrid.driver.power.gude
         import labgrid.driver.power.gude24
         import labgrid.driver.power.netio
         import labgrid.driver.power.netio_kshell
         import labgrid.driver.power.rest
         import labgrid.driver.power.sentry
         import labgrid.driver.power.eg_pms2_network
@@ -260,7 +261,11 @@
     def test_import_backend_tplink(self):
         pytest.importorskip("kasa")
         import labgrid.driver.power.tplink
 
     def test_import_backend_siglent(self):
         pytest.importorskip("vxi11")
         import labgrid.driver.power.siglent
+
+    def test_import_backend_poe_mib(self):
+        pytest.importorskip("pysnmp")
+        import labgrid.driver.power.poe_mib
```

### Comparing `labgrid-23.1a2/tests/test_processwrapper.py` & `labgrid-24.0a1/tests/test_processwrapper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_qemudriver.py` & `labgrid-24.0a1/tests/test_qemudriver.py`

 * *Files 19% similar despite different names*

```diff
@@ -56,30 +56,36 @@
 
     select_mock = mocker.patch('select.select')
     select_mock.return_value = True, None, None
 
     socket_mock = mocker.patch('socket.socket')
     socket_mock.return_value.accept.return_value = mocker.MagicMock(), ''
 
+@pytest.fixture
+def qemu_version_mock(mocker):
+    run_mock = mocker.patch('subprocess.run')
+    run_mock.return_value.returncode = 0
+    run_mock.return_value.stdout = "QEMU emulator version 4.2.1"
+
 def test_qemu_instance(qemu_target, qemu_driver):
     assert (isinstance(qemu_driver, QEMUDriver))
 
-def test_qemu_activate_deactivate(qemu_target, qemu_driver):
+def test_qemu_activate_deactivate(qemu_target, qemu_driver, qemu_version_mock):
     qemu_target.activate(qemu_driver)
     qemu_target.deactivate(qemu_driver)
 
-def test_qemu_on_off(qemu_target, qemu_driver, qemu_mock):
+def test_qemu_on_off(qemu_target, qemu_driver, qemu_mock, qemu_version_mock):
     qemu_target.activate(qemu_driver)
 
     qemu_driver.on()
     qemu_driver.off()
 
     qemu_target.deactivate(qemu_driver)
 
-def test_qemu_read_write(qemu_target, qemu_driver, qemu_mock):
+def test_qemu_read_write(qemu_target, qemu_driver, qemu_mock, qemu_version_mock):
     qemu_target.activate(qemu_driver)
 
     qemu_driver.on()
     qemu_driver.read()
     qemu_driver.read(max_size=10)
     qemu_driver.write(b'abc')
```

### Comparing `labgrid-23.1a2/tests/test_remote.py` & `labgrid-24.0a1/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_reporter.py` & `labgrid-24.0a1/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_resource.py` & `labgrid-24.0a1/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_sched.py` & `labgrid-24.0a1/tests/test_sched.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_serialdriver.py` & `labgrid-24.0a1/tests/test_serialdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_shelldriver.py` & `labgrid-24.0a1/tests/test_shelldriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_sigrok.py` & `labgrid-24.0a1/tests/test_sigrok.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_sshdriver.py` & `labgrid-24.0a1/tests/test_sshdriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     call.return_value = 0
     popen = mocker.patch('subprocess.Popen', autospec=True)
     path = mocker.patch('os.path.exists')
     path.return_value = True
     instance_mock = mocker.MagicMock()
     popen.return_value = instance_mock
     instance_mock.wait = mocker.MagicMock(return_value=0)
+    instance_mock.communicate = mocker.MagicMock(return_value=(b"", b""))
     SSHDriver(target, "ssh")
     s = target.get_driver("SSHDriver")
     return s
 
 def test_create_fail_missing_resource(target):
     with pytest.raises(NoResourceFoundError):
         SSHDriver(target, "ssh")
@@ -31,32 +32,35 @@
     call.return_value = 0
     popen = mocker.patch('subprocess.Popen', autospec=True)
     path = mocker.patch('os.path.exists')
     path.return_value = True
     instance_mock = mocker.MagicMock()
     popen.return_value = instance_mock
     instance_mock.wait = mocker.MagicMock(return_value=0)
+    instance_mock.communicate = mocker.MagicMock(return_value=(b"", b""))
     s = SSHDriver(target, "ssh")
     assert isinstance(s, SSHDriver)
 
-def test_run_check(ssh_driver_mocked_and_activated, mocker):
+def test_run_check(target, ssh_driver_mocked_and_activated, mocker):
     s = ssh_driver_mocked_and_activated
     s._run = mocker.MagicMock(return_value=(['success'], [], 0))
     res = s.run_check("test")
     assert res == ['success']
     res = s.run("test")
     assert res == (['success'], [], 0)
+    target.deactivate(s)
 
-def test_run_check_raise(ssh_driver_mocked_and_activated, mocker):
+def test_run_check_raise(target, ssh_driver_mocked_and_activated, mocker):
     s = ssh_driver_mocked_and_activated
     s._run = mocker.MagicMock(return_value=(['error'], [], 1))
     with pytest.raises(ExecutionError):
         res = s.run_check("test")
     res = s.run("test")
     assert res == (['error'], [], 1)
+    target.deactivate(s)
 
 @pytest.fixture(scope='function')
 def ssh_localhost(target, pytestconfig):
     name = pytestconfig.getoption("--ssh-username")
     NetworkService(target, "service", "localhost", name)
     SSHDriver(target, "ssh")
     s = target.get_driver("SSHDriver")
@@ -168,7 +172,27 @@
                 send_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 send_socket.connect(("127.0.0.1", remoteport))
 
                 client_socket, address = server_socket.accept()
                 send_socket.send(test_string.encode('utf-8'))
 
                 assert client_socket.recv(16).decode("utf-8") == test_string
+
+
+@pytest.mark.sshusername
+def test_unix_socket_forward(ssh_localhost, tmpdir):
+    p = tmpdir.join("console.sock")
+    test_string = "Hello World"
+
+    with ssh_localhost.forward_unix_socket(str(p)) as localport:
+        with socket.socket(socket.AF_UNIX, socket.SOCK_STREAM) as server_socket:
+            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as send_socket:
+                server_socket.bind(str(p))
+                server_socket.listen(1)
+
+                send_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                send_socket.connect(("127.0.0.1", localport))
+
+                client_socket, address = server_socket.accept()
+                send_socket.send(test_string.encode("utf-8"))
+
+                assert client_socket.recv(16).decode("utf-8") == test_string
```

### Comparing `labgrid-23.1a2/tests/test_step.py` & `labgrid-24.0a1/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_steplogger.py` & `labgrid-24.0a1/tests/test_steplogger.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_strategy.py` & `labgrid-24.0a1/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_sysfsgpioagent.py` & `labgrid-24.0a1/tests/test_sysfsgpioagent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_target.py` & `labgrid-24.0a1/tests/test_target.py`

 * *Files 25% similar despite different names*

```diff
@@ -37,14 +37,31 @@
         pass
 
     a = A(target, "aresource")
     b = A(target, "default")
     with pytest.raises(NoResourceFoundError) as excinfo:
         target.get_resource(A, name="nosuchresource")
 
+def test_get_resource_multiple_with_default(target):
+    class A(Resource):
+        pass
+
+    class B(Resource):
+        pass
+
+    a = A(target, "aresource")
+    adef = A(target, "default")
+    b = B(target, "bresource")
+    bdef = B(target, "default")
+
+    assert target.get_resource(A) is adef
+    assert target.get_resource(B) is bdef
+    assert target.get_resource(A, name="aresource") is a
+    assert target.get_resource(B, name="bresource") is b
+
 def test_get_driver(target):
     class A(Driver):
         pass
 
     a = A(target, "adriver")
     assert isinstance(target.get_driver(A), A)
     assert target.get_driver(A) is a
@@ -523,7 +540,71 @@
     target.set_binding_map({"c": "driver1", "d": "driver2"})
     s = Opt4DiffStrategy(target, None)
 
     assert s.a is None
     assert s.b is None
     assert s.c == d1
     assert s.d == d2
+
+def test_get_bound_resources(target):
+    class AResource(Resource):
+        pass
+
+    class ADriver(Driver):
+        bindings = {
+            "a": AResource,
+        }
+
+    class BDriver(Driver):
+        bindings = {
+            "a": ADriver,
+        }
+
+    aresource = AResource(target, "aresource")
+    adriver = ADriver(target, "adriver")
+    bdriver = BDriver(target, "bdriver")
+
+    assert bdriver.get_bound_resources() == {aresource}
+    assert adriver.get_bound_resources() == {aresource}
+
+    assert target.get_driver(ADriver, resource=aresource) 
+
+def test_get_bound_multiple_resources(target):
+    class AResource(Resource):
+        pass
+
+    class BResource(Resource):
+        pass
+
+    class ADriver(Driver):
+        bindings = {
+            "a": AResource,
+        }
+
+    class BDriver(Driver):
+        bindings = {
+            "b": BResource,
+        }
+
+    class CDriver(Driver):
+        bindings = {
+            "a": ADriver,
+            "b": BDriver,
+        }
+
+    aresource = AResource(target, "aresource")
+    bresource = BResource(target, "bresource")
+    adriver = ADriver(target, "adriver")
+    bdriver = BDriver(target, "bdriver")
+    cdriver = CDriver(target, "bdriver")
+
+    assert adriver.get_bound_resources() == {aresource}
+    assert bdriver.get_bound_resources() == {bresource}
+    assert cdriver.get_bound_resources() == {aresource, bresource}
+
+    assert target.get_driver(ADriver, resource=aresource) 
+    assert target.get_driver(BDriver, resource=bresource) 
+    assert target.get_driver(CDriver, resource=aresource) 
+
+    assert target.get_active_driver(ADriver, resource=aresource) 
+    assert target.get_active_driver(BDriver, resource=bresource) 
+    assert target.get_active_driver(CDriver, resource=aresource)
```

### Comparing `labgrid-23.1a2/tests/test_tasmota.py` & `labgrid-24.0a1/tests/test_tasmota.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_timeout.py` & `labgrid-24.0a1/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_ubootdriver.py` & `labgrid-24.0a1/tests/test_ubootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_usbtmc.py` & `labgrid-24.0a1/tests/test_usbtmc.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_util.py` & `labgrid-24.0a1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a2/tests/test_yaml.py` & `labgrid-24.0a1/tests/test_yaml.py`

 * *Files identical despite different names*

