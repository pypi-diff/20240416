# Comparing `tmp/ixmp4-0.8.0.tar.gz` & `tmp/ixmp4-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixmp4-0.8.0.tar", max compression
+gzip compressed data, was "ixmp4-0.8.1.tar", max compression
```

## Comparing `ixmp4-0.8.0.tar` & `ixmp4-0.8.1.tar`

### file list

```diff
@@ -1,191 +1,210 @@
--rw-r--r--   0        0        0     1067 2024-03-19 15:05:46.175346 ixmp4-0.8.0/LICENSE
--rw-r--r--   0        0        0     3561 2024-03-19 15:05:46.175346 ixmp4-0.8.0/README.md
--rw-r--r--   0        0        0      762 2024-03-19 15:06:05.731383 ixmp4-0.8.0/ixmp4/__init__.py
--rw-r--r--   0        0        0       64 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/__main__.py
--rw-r--r--   0        0        0     2724 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/cli/__init__.py
--rw-r--r--   0        0        0     9357 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/cli/platforms.py
--rw-r--r--   0        0        0     1130 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/cli/server.py
--rw-r--r--   0        0        0      393 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/cli/utils.py
--rw-r--r--   0        0        0      243 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/__init__.py
--rw-r--r--   0        0        0     4877 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/auth.py
--rw-r--r--   0        0        0      271 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/base.py
--rw-r--r--   0        0        0      827 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/credentials.py
--rw-r--r--   0        0        0      337 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/logging/debug.conf
--rw-r--r--   0        0        0      336 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/logging/development.conf
--rw-r--r--   0        0        0      413 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/logging/production.conf
--rw-r--r--   0        0        0     1301 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/logging/server.conf
--rw-r--r--   0        0        0     6326 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/manager.py
--rw-r--r--   0        0        0     4812 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/settings.py
--rw-r--r--   0        0        0     1857 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/toml.py
--rw-r--r--   0        0        0      468 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/conf/user.py
--rw-r--r--   0        0        0      385 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/__init__.py
--rw-r--r--   0        0        0      656 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/base.py
--rw-r--r--   0        0        0      425 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/decorators.py
--rw-r--r--   0        0        0     4021 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/exceptions.py
--rw-r--r--   0        0        0       64 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/iamc/__init__.py
--rw-r--r--   0        0        0     5408 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/iamc/data.py
--rw-r--r--   0        0        0     3658 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/iamc/variable.py
--rw-r--r--   0        0        0      381 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/meta.py
--rw-r--r--   0        0        0     3434 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/model.py
--rw-r--r--   0        0        0       35 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/optimization/__init__.py
--rw-r--r--   0        0        0      628 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/optimization/data.py
--rw-r--r--   0        0        0     3156 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/optimization/indexset.py
--rw-r--r--   0        0        0     4245 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/optimization/scalar.py
--rw-r--r--   0        0        0     2905 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/platform.py
--rw-r--r--   0        0        0     4565 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/region.py
--rw-r--r--   0        0        0     4566 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/run.py
--rw-r--r--   0        0        0     3568 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/scenario.py
--rw-r--r--   0        0        0     4245 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/unit.py
--rw-r--r--   0        0        0      708 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/core/utils.py
--rw-r--r--   0        0        0        0 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/__init__.py
--rw-r--r--   0        0        0      988 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/__init__.py
--rw-r--r--   0        0        0     2080 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/base.py
--rw-r--r--   0        0        0     2837 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/docs.py
--rw-r--r--   0        0        0      308 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/iamc/__init__.py
--rw-r--r--   0        0        0     4600 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/iamc/datapoint.py
--rw-r--r--   0        0        0     1137 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/iamc/measurand.py
--rw-r--r--   0        0        0     4890 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/iamc/timeseries.py
--rw-r--r--   0        0        0     2659 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/iamc/variable.py
--rw-r--r--   0        0        0     5045 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/meta.py
--rw-r--r--   0        0        0     2704 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/model.py
--rw-r--r--   0        0        0       96 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/optimization/__init__.py
--rw-r--r--   0        0        0     3717 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/optimization/indexset.py
--rw-r--r--   0        0        0     4692 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/optimization/scalar.py
--rw-r--r--   0        0        0     4106 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/region.py
--rw-r--r--   0        0        0     5775 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/run.py
--rw-r--r--   0        0        0     2693 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/scenario.py
--rw-r--r--   0        0        0     3692 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/abstract/unit.py
--rw-r--r--   0        0        0      697 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/__init__.py
--rw-r--r--   0        0        0    10459 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/base.py
--rw-r--r--   0        0        0     1160 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/docs.py
--rw-r--r--   0        0        0      255 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/iamc/__init__.py
--rw-r--r--   0        0        0     1723 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/iamc/datapoint.py
--rw-r--r--   0        0        0     1589 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/iamc/timeseries.py
--rw-r--r--   0        0        0     1498 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/iamc/variable.py
--rw-r--r--   0        0        0     1766 2024-03-19 15:05:46.179346 ixmp4-0.8.0/ixmp4/data/api/meta.py
--rw-r--r--   0        0        0     1432 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/model.py
--rw-r--r--   0        0        0       96 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/optimization/__init__.py
--rw-r--r--   0        0        0     1960 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/optimization/indexset.py
--rw-r--r--   0        0        0     2330 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/optimization/scalar.py
--rw-r--r--   0        0        0     1690 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/region.py
--rw-r--r--   0        0        0     2214 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/run.py
--rw-r--r--   0        0        0     1485 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/scenario.py
--rw-r--r--   0        0        0     1608 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/api/unit.py
--rw-r--r--   0        0        0     3679 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/auth/context.py
--rw-r--r--   0        0        0     1465 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/auth/decorators.py
--rw-r--r--   0        0        0      141 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/backend/__init__.py
--rw-r--r--   0        0        0     5376 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/backend/api.py
--rw-r--r--   0        0        0     1121 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/backend/base.py
--rw-r--r--   0        0        0     4625 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/backend/db.py
--rw-r--r--   0        0        0      802 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/__init__.py
--rw-r--r--   0        0        0    15489 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/base.py
--rw-r--r--   0        0        0     3459 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/docs.py
--rw-r--r--   0        0        0      390 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/__init__.py
--rw-r--r--   0        0        0      528 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/meta.py
--rw-r--r--   0        0        0      391 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/model.py
--rw-r--r--   0        0        0      448 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/optimizationindexset.py
--rw-r--r--   0        0        0      581 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/optimizationscalar.py
--rw-r--r--   0        0        0      385 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/region.py
--rw-r--r--   0        0        0      776 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/run.py
--rw-r--r--   0        0        0      409 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/scenario.py
--rw-r--r--   0        0        0      419 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/timeseries.py
--rw-r--r--   0        0        0      470 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/unit.py
--rw-r--r--   0        0        0      490 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/filters/variable.py
--rw-r--r--   0        0        0      331 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/__init__.py
--rw-r--r--   0        0        0      302 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/base.py
--rw-r--r--   0        0        0      129 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/__init__.py
--rw-r--r--   0        0        0     5904 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/filter.py
--rw-r--r--   0        0        0     1356 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/model.py
--rw-r--r--   0        0        0     7583 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/repository.py
--rw-r--r--   0        0        0     2917 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/measurand.py
--rw-r--r--   0        0        0       75 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/timeseries/__init__.py
--rw-r--r--   0        0        0      401 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/timeseries/filter.py
--rw-r--r--   0        0        0     1160 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/timeseries/model.py
--rw-r--r--   0        0        0     4307 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/timeseries/repository.py
--rw-r--r--   0        0        0       86 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/variable/__init__.py
--rw-r--r--   0        0        0      235 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/variable/docs.py
--rw-r--r--   0        0        0      806 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/variable/filter.py
--rw-r--r--   0        0        0      584 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/variable/model.py
--rw-r--r--   0        0        0     1444 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/iamc/variable/repository.py
--rw-r--r--   0        0        0       79 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/meta/__init__.py
--rw-r--r--   0        0        0      570 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/meta/filter.py
--rw-r--r--   0        0        0     2246 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/meta/model.py
--rw-r--r--   0        0        0     6859 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/meta/repository.py
--rw-r--r--   0        0        0      118 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/model/__init__.py
--rw-r--r--   0        0        0      426 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/model/docs.py
--rw-r--r--   0        0        0     1780 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/model/filter.py
--rw-r--r--   0        0        0      517 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/model/model.py
--rw-r--r--   0        0        0     1371 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/model/repository.py
--rw-r--r--   0        0        0       96 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/__init__.py
--rw-r--r--   0        0        0      310 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/base.py
--rw-r--r--   0        0        0       71 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/__init__.py
--rw-r--r--   0        0        0      235 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/docs.py
--rw-r--r--   0        0        0      534 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/filter.py
--rw-r--r--   0        0        0     1253 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/model.py
--rw-r--r--   0        0        0     2332 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/repository.py
--rw-r--r--   0        0        0       67 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/__init__.py
--rw-r--r--   0        0        0      225 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/docs.py
--rw-r--r--   0        0        0      595 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/filter.py
--rw-r--r--   0        0        0     1084 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/model.py
--rw-r--r--   0        0        0     2552 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/repository.py
--rw-r--r--   0        0        0      121 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/region/__init__.py
--rw-r--r--   0        0        0      496 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/region/docs.py
--rw-r--r--   0        0        0     1547 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/region/filter.py
--rw-r--r--   0        0        0      611 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/region/model.py
--rw-r--r--   0        0        0     1569 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/region/repository.py
--rw-r--r--   0        0        0       61 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/run/__init__.py
--rw-r--r--   0        0        0      916 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/run/filter.py
--rw-r--r--   0        0        0     1452 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/run/model.py
--rw-r--r--   0        0        0     5064 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/run/repository.py
--rw-r--r--   0        0        0      127 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/scenario/__init__.py
--rw-r--r--   0        0        0      222 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/scenario/docs.py
--rw-r--r--   0        0        0     1827 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/scenario/filter.py
--rw-r--r--   0        0        0      545 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/scenario/model.py
--rw-r--r--   0        0        0     1814 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/scenario/repository.py
--rw-r--r--   0        0        0     3331 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/timeseries.py
--rw-r--r--   0        0        0      126 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/unit/__init__.py
--rw-r--r--   0        0        0      495 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/unit/docs.py
--rw-r--r--   0        0        0     1714 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/unit/filter.py
--rw-r--r--   0        0        0      469 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/unit/model.py
--rw-r--r--   0        0        0     1725 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/unit/repository.py
--rw-r--r--   0        0        0      436 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/db/utils.py
--rw-r--r--   0        0        0     5531 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/generator.py
--rw-r--r--   0        0        0      284 2024-03-19 15:05:46.183346 ixmp4-0.8.0/ixmp4/data/types.py
--rw-r--r--   0        0        0     1538 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/__init__.py
--rw-r--r--   0        0        0     9522 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/filters.py
--rw-r--r--   0        0        0     2408 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/migrations/env.py
--rw-r--r--   0        0        0      509 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/migrations/script.py.mako
--rw-r--r--   0        0        0     3777 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py
--rw-r--r--   0        0        0    19021 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py
--rw-r--r--   0        0        0     5175 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py
--rw-r--r--   0        0        0     1478 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/utils/__init__.py
--rw-r--r--   0        0        0     1496 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/utils/alembic.py
--rw-r--r--   0        0        0     1064 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/db/utils/sqlite.py
--rw-r--r--   0        0        0        0 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/py.typed
--rw-r--r--   0        0        0      297 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/__init__.py
--rw-r--r--   0        0        0     2747 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/__init__.py
--rw-r--r--   0        0        0     1069 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/base.py
--rw-r--r--   0        0        0      192 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/decorators.py
--rw-r--r--   0        0        0     3606 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/deps.py
--rw-r--r--   0        0        0     6259 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/docs.py
--rw-r--r--   0        0        0       61 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/__init__.py
--rw-r--r--   0        0        0     2550 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/datapoint.py
--rw-r--r--   0        0        0      921 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/model.py
--rw-r--r--   0        0        0      930 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/region.py
--rw-r--r--   0        0        0      948 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/scenario.py
--rw-r--r--   0        0        0     1916 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/timeseries.py
--rw-r--r--   0        0        0      912 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/unit.py
--rw-r--r--   0        0        0     1263 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/iamc/variable.py
--rw-r--r--   0        0        0     1976 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/meta.py
--rw-r--r--   0        0        0      696 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/middleware.py
--rw-r--r--   0        0        0     1185 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/model.py
--rw-r--r--   0        0        0       31 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/optimization/__init__.py
--rw-r--r--   0        0        0     1775 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/optimization/indexset.py
--rw-r--r--   0        0        0     2024 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/optimization/scalar.py
--rw-r--r--   0        0        0     1372 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/region.py
--rw-r--r--   0        0        0     1621 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/run.py
--rw-r--r--   0        0        0     1227 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/scenario.py
--rw-r--r--   0        0        0     1304 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/rest/unit.py
--rw-r--r--   0        0        0      187 2024-03-19 15:05:46.187346 ixmp4-0.8.0/ixmp4/server/workers.py
--rw-r--r--   0        0        0     2904 2024-03-19 15:06:05.727383 ixmp4-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5021 1970-01-01 00:00:00.000000 ixmp4-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 11:25:24.345074 ixmp4-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3561 2024-04-16 11:25:24.345074 ixmp4-0.8.1/README.md
+-rw-r--r--   0        0        0      800 2024-04-16 11:25:48.353925 ixmp4-0.8.1/ixmp4/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-16 11:25:24.345074 ixmp4-0.8.1/ixmp4/__main__.py
+-rw-r--r--   0        0        0     2724 2024-04-16 11:25:24.345074 ixmp4-0.8.1/ixmp4/cli/__init__.py
+-rw-r--r--   0        0        0     9357 2024-04-16 11:25:24.345074 ixmp4-0.8.1/ixmp4/cli/platforms.py
+-rw-r--r--   0        0        0     1130 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/cli/server.py
+-rw-r--r--   0        0        0      393 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/cli/utils.py
+-rw-r--r--   0        0        0      243 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/auth.py
+-rw-r--r--   0        0        0      271 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/base.py
+-rw-r--r--   0        0        0      827 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/credentials.py
+-rw-r--r--   0        0        0      337 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/debug.conf
+-rw-r--r--   0        0        0      336 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/development.conf
+-rw-r--r--   0        0        0      413 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/production.conf
+-rw-r--r--   0        0        0     1301 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/server.conf
+-rw-r--r--   0        0        0     6326 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/manager.py
+-rw-r--r--   0        0        0     5051 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/settings.py
+-rw-r--r--   0        0        0     1857 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/toml.py
+-rw-r--r--   0        0        0      468 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/user.py
+-rw-r--r--   0        0        0      432 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/__init__.py
+-rw-r--r--   0        0        0      656 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/base.py
+-rw-r--r--   0        0        0      525 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/decorators.py
+-rw-r--r--   0        0        0     4419 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/exceptions.py
+-rw-r--r--   0        0        0       64 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/iamc/__init__.py
+-rw-r--r--   0        0        0     5596 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/iamc/data.py
+-rw-r--r--   0        0        0     3658 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/iamc/variable.py
+-rw-r--r--   0        0        0      381 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/meta.py
+-rw-r--r--   0        0        0     3434 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/model.py
+-rw-r--r--   0        0        0       35 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/data.py
+-rw-r--r--   0        0        0     3180 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/indexset.py
+-rw-r--r--   0        0        0     4245 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/scalar.py
+-rw-r--r--   0        0        0     3519 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/table.py
+-rw-r--r--   0        0        0     2905 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/platform.py
+-rw-r--r--   0        0        0     4565 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/region.py
+-rw-r--r--   0        0        0     4566 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/run.py
+-rw-r--r--   0        0        0     3568 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/scenario.py
+-rw-r--r--   0        0        0     4245 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/unit.py
+-rw-r--r--   0        0        0      708 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/__init__.py
+-rw-r--r--   0        0        0     2080 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/base.py
+-rw-r--r--   0        0        0     2849 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/docs.py
+-rw-r--r--   0        0        0      308 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/__init__.py
+-rw-r--r--   0        0        0     4620 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/datapoint.py
+-rw-r--r--   0        0        0     1137 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/measurand.py
+-rw-r--r--   0        0        0     4890 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/timeseries.py
+-rw-r--r--   0        0        0     2659 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/variable.py
+-rw-r--r--   0        0        0     5045 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/meta.py
+-rw-r--r--   0        0        0     2704 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/model.py
+-rw-r--r--   0        0        0      165 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/column.py
+-rw-r--r--   0        0        0     3833 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/indexset.py
+-rw-r--r--   0        0        0     4709 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/scalar.py
+-rw-r--r--   0        0        0     6019 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/table.py
+-rw-r--r--   0        0        0     4104 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/region.py
+-rw-r--r--   0        0        0     5775 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/run.py
+-rw-r--r--   0        0        0     2693 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/scenario.py
+-rw-r--r--   0        0        0     3692 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/unit.py
+-rw-r--r--   0        0        0      750 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/__init__.py
+-rw-r--r--   0        0        0    13984 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/base.py
+-rw-r--r--   0        0        0     1160 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/docs.py
+-rw-r--r--   0        0        0      255 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/datapoint.py
+-rw-r--r--   0        0        0     1589 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/timeseries.py
+-rw-r--r--   0        0        0     1483 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/variable.py
+-rw-r--r--   0        0        0     1766 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/meta.py
+-rw-r--r--   0        0        0     1417 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/model.py
+-rw-r--r--   0        0        0      138 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/__init__.py
+-rw-r--r--   0        0        0      474 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/column.py
+-rw-r--r--   0        0        0     2052 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/indexset.py
+-rw-r--r--   0        0        0     2282 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/scalar.py
+-rw-r--r--   0        0        0     2376 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/table.py
+-rw-r--r--   0        0        0     1675 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/region.py
+-rw-r--r--   0        0        0     2214 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/run.py
+-rw-r--r--   0        0        0     1470 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/scenario.py
+-rw-r--r--   0        0        0     1593 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/unit.py
+-rw-r--r--   0        0        0     3679 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/auth/context.py
+-rw-r--r--   0        0        0     1465 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/auth/decorators.py
+-rw-r--r--   0        0        0      141 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/__init__.py
+-rw-r--r--   0        0        0     6207 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/api.py
+-rw-r--r--   0        0        0     1234 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/base.py
+-rw-r--r--   0        0        0     4761 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/db.py
+-rw-r--r--   0        0        0      874 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/db/__init__.py
+-rw-r--r--   0        0        0    15233 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/db/base.py
+-rw-r--r--   0        0        0     3459 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/docs.py
+-rw-r--r--   0        0        0      502 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/meta.py
+-rw-r--r--   0        0        0      391 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/model.py
+-rw-r--r--   0        0        0      440 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationcolumn.py
+-rw-r--r--   0        0        0      448 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationindexset.py
+-rw-r--r--   0        0        0      581 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationscalar.py
+-rw-r--r--   0        0        0      436 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationtable.py
+-rw-r--r--   0        0        0      385 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/region.py
+-rw-r--r--   0        0        0      776 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/run.py
+-rw-r--r--   0        0        0      409 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/scenario.py
+-rw-r--r--   0        0        0      419 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/timeseries.py
+-rw-r--r--   0        0        0      470 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/unit.py
+-rw-r--r--   0        0        0      490 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/variable.py
+-rw-r--r--   0        0        0      331 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/base.py
+-rw-r--r--   0        0        0      129 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/__init__.py
+-rw-r--r--   0        0        0     5896 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/filter.py
+-rw-r--r--   0        0        0     1356 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/model.py
+-rw-r--r--   0        0        0     7583 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/repository.py
+-rw-r--r--   0        0        0     2917 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/measurand.py
+-rw-r--r--   0        0        0       75 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/__init__.py
+-rw-r--r--   0        0        0      401 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/filter.py
+-rw-r--r--   0        0        0     1160 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/model.py
+-rw-r--r--   0        0        0     4440 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/repository.py
+-rw-r--r--   0        0        0       86 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/docs.py
+-rw-r--r--   0        0        0      806 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/filter.py
+-rw-r--r--   0        0        0      584 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/model.py
+-rw-r--r--   0        0        0     1444 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/repository.py
+-rw-r--r--   0        0        0       79 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/__init__.py
+-rw-r--r--   0        0        0      570 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/filter.py
+-rw-r--r--   0        0        0     2246 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/model.py
+-rw-r--r--   0        0        0     6937 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/repository.py
+-rw-r--r--   0        0        0      118 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/docs.py
+-rw-r--r--   0        0        0     1780 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/filter.py
+-rw-r--r--   0        0        0      517 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/model.py
+-rw-r--r--   0        0        0     1371 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/repository.py
+-rw-r--r--   0        0        0      183 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/base.py
+-rw-r--r--   0        0        0       67 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/docs.py
+-rw-r--r--   0        0        0      692 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/filter.py
+-rw-r--r--   0        0        0     1170 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/model.py
+-rw-r--r--   0        0        0     2440 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/repository.py
+-rw-r--r--   0        0        0       71 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/docs.py
+-rw-r--r--   0        0        0      534 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/filter.py
+-rw-r--r--   0        0        0     1278 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/model.py
+-rw-r--r--   0        0        0     2348 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/repository.py
+-rw-r--r--   0        0        0       67 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/docs.py
+-rw-r--r--   0        0        0      809 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/filter.py
+-rw-r--r--   0        0        0     1084 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/model.py
+-rw-r--r--   0        0        0     2552 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/repository.py
+-rw-r--r--   0        0        0       65 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/docs.py
+-rw-r--r--   0        0        0      522 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/filter.py
+-rw-r--r--   0        0        0     3554 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/model.py
+-rw-r--r--   0        0        0     5079 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/repository.py
+-rw-r--r--   0        0        0      121 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/docs.py
+-rw-r--r--   0        0        0     1547 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/filter.py
+-rw-r--r--   0        0        0      611 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/model.py
+-rw-r--r--   0        0        0     1569 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/repository.py
+-rw-r--r--   0        0        0       61 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/filter.py
+-rw-r--r--   0        0        0     1563 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/model.py
+-rw-r--r--   0        0        0     5064 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/repository.py
+-rw-r--r--   0        0        0      127 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/__init__.py
+-rw-r--r--   0        0        0      222 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/docs.py
+-rw-r--r--   0        0        0     1827 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/filter.py
+-rw-r--r--   0        0        0      545 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/model.py
+-rw-r--r--   0        0        0     1814 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/repository.py
+-rw-r--r--   0        0        0     3331 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/timeseries.py
+-rw-r--r--   0        0        0      126 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/docs.py
+-rw-r--r--   0        0        0     1714 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/filter.py
+-rw-r--r--   0        0        0      469 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/model.py
+-rw-r--r--   0        0        0     1725 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/repository.py
+-rw-r--r--   0        0        0      436 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/utils.py
+-rw-r--r--   0        0        0     5531 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/generator.py
+-rw-r--r--   0        0        0      292 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/types.py
+-rw-r--r--   0        0        0     1585 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/__init__.py
+-rw-r--r--   0        0        0     9465 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/filters.py
+-rw-r--r--   0        0        0     2408 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/env.py
+-rw-r--r--   0        0        0      509 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/script.py.mako
+-rw-r--r--   0        0        0     5559 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py
+-rw-r--r--   0        0        0     3777 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py
+-rw-r--r--   0        0        0    19021 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py
+-rw-r--r--   0        0        0     5175 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py
+-rw-r--r--   0        0        0     1478 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/utils/__init__.py
+-rw-r--r--   0        0        0     1496 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/utils/alembic.py
+-rw-r--r--   0        0        0     1052 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/utils/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/py.typed
+-rw-r--r--   0        0        0      297 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/__init__.py
+-rw-r--r--   0        0        0     2810 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/base.py
+-rw-r--r--   0        0        0      192 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/decorators.py
+-rw-r--r--   0        0        0     3606 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/deps.py
+-rw-r--r--   0        0        0     6969 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/docs.py
+-rw-r--r--   0        0        0       61 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/__init__.py
+-rw-r--r--   0        0        0     2550 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/datapoint.py
+-rw-r--r--   0        0        0      921 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/model.py
+-rw-r--r--   0        0        0      930 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/region.py
+-rw-r--r--   0        0        0      948 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/scenario.py
+-rw-r--r--   0        0        0     1916 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/timeseries.py
+-rw-r--r--   0        0        0      912 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/unit.py
+-rw-r--r--   0        0        0     1263 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/variable.py
+-rw-r--r--   0        0        0     1976 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/meta.py
+-rw-r--r--   0        0        0      696 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/middleware.py
+-rw-r--r--   0        0        0     1185 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/model.py
+-rw-r--r--   0        0        0       38 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/__init__.py
+-rw-r--r--   0        0        0     1830 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/indexset.py
+-rw-r--r--   0        0        0     1946 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/scalar.py
+-rw-r--r--   0        0        0     1928 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/table.py
+-rw-r--r--   0        0        0     1372 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/region.py
+-rw-r--r--   0        0        0     1621 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/run.py
+-rw-r--r--   0        0        0     1227 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/scenario.py
+-rw-r--r--   0        0        0     1304 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/unit.py
+-rw-r--r--   0        0        0      187 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/workers.py
+-rw-r--r--   0        0        0     3042 2024-04-16 11:25:48.353925 ixmp4-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 ixmp4-0.8.1/PKG-INFO
```

### Comparing `ixmp4-0.8.0/LICENSE` & `ixmp4-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/README.md` & `ixmp4-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -81,22 +81,22 @@
 ## Developing
 
 See [DEVELOPING.md](DEVELOPING.md) for guidance. When contributing to this project via
 a Pull Request, add your name to the "authors" section in the `pyproject.toml` file.
 
 ## Compatibility
 
-This project mainly targets postgres version 15 but we test version 16 continously also. Tests with pyarrow installed alongside are also run due to its effect on pandas etc.
+This project mainly targets postgres version 16 but we test version 15 continously also. Tests with pyarrow installed alongside are also run due to its effect on pandas etc.
 | python | postgres | with pyarrow |
 |--------|----------|--------------|
-| 3.10 | 15 | false |
-| 3.11 | 15 | false |
-| 3.12 | 15 | false |
-| 3.12 | 15 | true |
+| 3.10 | 16 | false |
+| 3.11 | 16 | false |
 | 3.12 | 16 | false |
+| 3.12 | 16 | true |
+| 3.12 | 15 | false |
 
 ## Funding ackownledgement
 
 <img src="./doc/source/_static/ECEMF-logo.png" width="264" height="100"
 alt="ECEMF logo" />
 <img src="./doc/source/_static/openENTRANCE-logo.png" width="187" height="120"
 alt="openENTRANCE logo" />
```

### Comparing `ixmp4-0.8.0/ixmp4/__init__.py` & `ixmp4-0.8.1/ixmp4/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from ixmp4.core import Region as Region
 from ixmp4.core import Run as Run
 from ixmp4.core import Scenario as Scenario
 from ixmp4.core import Unit as Unit
 from ixmp4.core import Variable as Variable
 from ixmp4.core import IndexSet as IndexSet
 from ixmp4.core import Scalar as Scalar
+from ixmp4.core import Table as Table
 from ixmp4.core.exceptions import InconsistentIamcType as InconsistentIamcType
 from ixmp4.core.exceptions import IxmpError as IxmpError
 from ixmp4.core.exceptions import NotFound as NotFound
 from ixmp4.core.exceptions import NotUnique as NotUnique
 from ixmp4.data.abstract import DataPoint as DataPoint
 
-__version__ = "0.8.0"
-__version_tuple__ = (0, 8, 0)
+__version__ = "0.8.1"
+__version_tuple__ = (0, 8, 1)
```

### Comparing `ixmp4-0.8.0/ixmp4/cli/__init__.py` & `ixmp4-0.8.1/ixmp4/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/cli/platforms.py` & `ixmp4-0.8.1/ixmp4/cli/platforms.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/cli/server.py` & `ixmp4-0.8.1/ixmp4/cli/server.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/conf/auth.py` & `ixmp4-0.8.1/ixmp4/conf/auth.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/conf/credentials.py` & `ixmp4-0.8.1/ixmp4/conf/credentials.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/conf/logging/server.conf` & `ixmp4-0.8.1/ixmp4/conf/logging/server.conf`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/conf/manager.py` & `ixmp4-0.8.1/ixmp4/conf/manager.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/conf/settings.py` & `ixmp4-0.8.1/ixmp4/conf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     )
     secret_hs256: str = "default_secret_hs256"
     migration_db_uri: str = "sqlite:///./run/db.sqlite"
     manager_url: HttpUrl = Field("https://api.manager.ece.iiasa.ac.at/v1")
     managed: bool = True
     max_page_size: int = 10_000
     default_page_size: int = 5_000
-    default_upload_chunk_size: int = 10_000
+    client_default_upload_chunk_size: int = 10_000
+    client_max_concurrent_requests: int = Field(2, lt=4)
+    client_max_request_retries: int = Field(3)
+    client_backoff_factor: int = Field(5)
+    client_timeout: int = Field(30)
     model_config = SettingsConfigDict(env_prefix="ixmp4_", extra="allow")
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.storage_directory.mkdir(parents=True, exist_ok=True)
 
@@ -51,14 +55,16 @@
         self.configure_logging(self.mode)
 
         self._credentials = None
         self._toml = None
         self._default_auth = None
         self._manager = None
 
+        logger.debug(f"Settings loaded: {self}")
+
     @property
     def credentials(self):
         if self._credentials is None:
             self.load_credentials()
         return self._credentials
 
     @property
```

### Comparing `ixmp4-0.8.0/ixmp4/conf/toml.py` & `ixmp4-0.8.1/ixmp4/conf/toml.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/base.py` & `ixmp4-0.8.1/ixmp4/core/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/exceptions.py` & `ixmp4-0.8.1/ixmp4/core/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,14 +86,18 @@
     http_error_name = "manager_api_error"
 
 
 class UnknownApiError(IxmpError):
     http_error_name = "unknown_api_error"
 
 
+class ApiEncumbered(IxmpError):
+    http_error_name = "api_encumbered"
+
+
 class PlatformNotFound(IxmpError):
     http_status_code = 404
     http_error_name = "platform_not_found"
 
 
 class PlatformNotUnique(IxmpError):
     http_status_code = 409
@@ -150,14 +154,16 @@
 
 class InvalidRunMeta(IxmpError):
     http_status_code = 400
     http_error_name = "run_invalid_meta"
 
 
 # == Filters ==
+
+
 class BadFilterArguments(IxmpError):
     _message = "The provided filter arguments are malformed."
     http_status_code = 400
     http_error_name = "bad_filter_arguments"
 
     def __str__(self) -> str:
         return f"{self.kwargs.get('model')} {self.kwargs.get('errors')}"
@@ -166,7 +172,18 @@
 # == Api Exceptions ==
 
 
 class InvalidCredentials(IxmpError):
     _message = "The provided credentials are invalid."
     http_status_code = 401
     http_error_name = "invalid_credentials"
+
+
+# == Optimization.Table ==
+
+
+class OptimizationTableDataKeysNotUnique(NotUnique):
+    _message = (
+        "The keys of the Table's data are not unique. Please consider using "
+        "`constrained_to_indexsets` to specify the IndexSet identifiers."
+    )
+    http_error_name = "optimization_table_data_keys_not_unique"
```

### Comparing `ixmp4-0.8.0/ixmp4/core/iamc/data.py` & `ixmp4-0.8.1/ixmp4/core/iamc/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,53 +88,57 @@
 
     run: Run
 
     def __init__(self, *args, run: Run, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.run = run
 
-    def _contract_parameters(self, df: pd.DataFrame) -> pd.DataFrame:
-        ts_df = df[["region", "variable", "unit", "run__id"]].drop_duplicates()
+    def _get_or_create_ts(self, df: pd.DataFrame) -> pd.DataFrame:
+        id_cols = ["region", "variable", "unit", "run__id"]
+        # create set of unqiue timeseries (if missing)
+        ts_df = df[id_cols].drop_duplicates()
         self.backend.iamc.timeseries.bulk_upsert(ts_df, create_related=True)
 
+        # retrieve them again to get database ids
         ts_df = self.backend.iamc.timeseries.tabulate(
             join_parameters=True,
             run={"id": self.run.id, "default_only": False},
         )
         ts_df = ts_df.rename(columns={"id": "time_series__id"})
 
+        # merge on the identity columns
         return pd.merge(
             df,
             ts_df,
             how="left",
-            on=["run__id", "region", "unit", "variable"],
+            on=id_cols,
             suffixes=(None, "_y"),
-        )
+        )  # tada, df with 'time_series__id' added from the database.
 
     def add(
         self,
         df: pd.DataFrame,
         type: Optional[DataPointModel.Type] = None,
     ):
         df = AddDataPointFrameSchema.validate(df)  # type:ignore
         df = to_dimensionless(df.copy())
         df["run__id"] = self.run.id
-        df = self._contract_parameters(df)
+        df = self._get_or_create_ts(df)
         substitute_type(df, type)
         self.backend.iamc.datapoints.bulk_upsert(df)
 
     def remove(
         self,
         df: pd.DataFrame,
         type: Optional[DataPointModel.Type] = None,
     ):
         df = RemoveDataPointFrameSchema.validate(df)  # type:ignore
         df = to_dimensionless(df.copy())
         df["run__id"] = self.run.id
-        df = self._contract_parameters(df)
+        df = self._get_or_create_ts(df)
         substitute_type(df, type)
         df = df.drop(columns=["unit", "variable", "region"])
         self.backend.iamc.datapoints.bulk_delete(df)
 
     def tabulate(
         self,
         *,
```

### Comparing `ixmp4-0.8.0/ixmp4/core/iamc/variable.py` & `ixmp4-0.8.1/ixmp4/core/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/model.py` & `ixmp4-0.8.1/ixmp4/core/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/optimization/data.py` & `ixmp4-0.8.1/ixmp4/core/optimization/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from ixmp4.data.abstract import Run
 
 from ..base import BaseFacade
 from .indexset import IndexSetRepository
 from .scalar import ScalarRepository
+from .table import TableRepository
 
 
 class OptimizationData(BaseFacade):
     """An optimization data instance, which provides access to optimization data such as
     IndexSet, Table, Variable, etc."""
 
     indexsets: IndexSetRepository
     scalars: ScalarRepository
+    tables: TableRepository
 
     def __init__(self, *args, run: Run, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.indexsets = IndexSetRepository(_backend=self.backend, _run=run)
         self.scalars = ScalarRepository(_backend=self.backend, _run=run)
+        self.tables = TableRepository(_backend=self.backend, _run=run)
```

### Comparing `ixmp4-0.8.0/ixmp4/core/optimization/indexset.py` & `ixmp4-0.8.1/ixmp4/core/optimization/indexset.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         return self._model.id
 
     @property
     def name(self) -> str:
         return self._model.name
 
     @property
-    def elements(self) -> list[int | str]:
+    def elements(self) -> list[float | int | str]:
         return self._model.elements
 
-    def add(self, elements: int | list[int | str] | str) -> None:
+    def add(self, elements: float | int | list[float | int | str] | str) -> None:
         """Adds elements to an existing IndexSet."""
         self.backend.optimization.indexsets.add_elements(
             indexset_id=self._model.id, elements=elements
         )
         self._model.elements = self.backend.optimization.indexsets.get(
             run_id=self._model.run__id, name=self._model.name
         ).elements
```

### Comparing `ixmp4-0.8.0/ixmp4/core/optimization/scalar.py` & `ixmp4-0.8.1/ixmp4/core/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/platform.py` & `ixmp4-0.8.1/ixmp4/core/platform.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/region.py` & `ixmp4-0.8.1/ixmp4/core/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/run.py` & `ixmp4-0.8.1/ixmp4/core/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/scenario.py` & `ixmp4-0.8.1/ixmp4/core/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/unit.py` & `ixmp4-0.8.1/ixmp4/core/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/core/utils.py` & `ixmp4-0.8.1/ixmp4/core/utils.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/__init__.py` & `ixmp4-0.8.1/ixmp4/data/abstract/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,12 +25,19 @@
     TimeSeries,
     TimeSeriesRepository,
     Variable,
     VariableRepository,
 )
 from .meta import MetaValue, RunMetaEntry, RunMetaEntryRepository, StrictMetaValue
 from .model import Model, ModelRepository
-from .optimization import IndexSet, IndexSetRepository, Scalar, ScalarRepository
+from .optimization import (
+    IndexSet,
+    IndexSetRepository,
+    Scalar,
+    ScalarRepository,
+    Table,
+    TableRepository,
+)
 from .region import Region, RegionRepository
 from .run import Run, RunRepository
 from .scenario import Scenario, ScenarioRepository
 from .unit import Unit, UnitRepository
```

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/base.py` & `ixmp4-0.8.1/ixmp4/data/abstract/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/docs.py` & `ixmp4-0.8.1/ixmp4/data/abstract/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     description: types.String
     "Description of the dimension object."
     dimension__id: types.Integer
     "Foreign unique integer id of the object in the dimension's table."
     dimension: types.Mapped
     "The documented object."
 
-    # This doesn't work since each dimension has a different self.dimension object atm
+    # This doesn't work since each dimension has a different self.dimension object as
+    # of now
     # def __str__(self) -> str:
     #    return (
     #        f"<Documentation for {self.dimension} {self.dimension.name}>"
     #    )
 
 
 # TODO: adjust all type hints once things work
```

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/iamc/datapoint.py` & `ixmp4-0.8.1/ixmp4/data/abstract/iamc/datapoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                     if it contains data points of type `CATEGORICAL`
                 - step_datetime
                     if it contains data points of type `DATETIME`
                 - ... misc parameter columns if `join_parameters` is set to `True`
         """
         ...
 
-    def bulk_upsert(self, df: pd.DataFrame) -> None:
+    def bulk_upsert(self, df: pd.DataFrame, **kwargs) -> None:
         """Looks which data points in the supplied data frame already exists,
         updates those that have changed and inserts new ones.
 
         Parameters
         ----------
         df : :class:`pandas.DataFrame`
             A data frame with the columns:
@@ -119,15 +119,15 @@
                 - step_category
                     if it contains data points of type `CATEGORICAL`
                 - step_datetime
                     if it contains data points of type `DATETIME`
         """
         ...
 
-    def bulk_delete(self, df: pd.DataFrame) -> None:
+    def bulk_delete(self, df: pd.DataFrame, **kwargs) -> None:
         """Deletes data points which match criteria in the supplied data frame.
 
         Parameters
         ----------
         df : :class:`pandas.DataFrame`
             A data frame with the columns:
                 - time_series__id
```

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/iamc/measurand.py` & `ixmp4-0.8.1/ixmp4/data/abstract/iamc/measurand.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/iamc/timeseries.py` & `ixmp4-0.8.1/ixmp4/data/abstract/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/iamc/variable.py` & `ixmp4-0.8.1/ixmp4/data/abstract/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/meta.py` & `ixmp4-0.8.1/ixmp4/data/abstract/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/model.py` & `ixmp4-0.8.1/ixmp4/data/abstract/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/optimization/indexset.py` & `ixmp4-0.8.1/ixmp4/data/abstract/optimization/indexset.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,27 +117,30 @@
         Returns
         -------
         :class:`pandas.DataFrame`:
             A data frame with the columns:
                 - id
                 - name
                 - elements
+                - run__id
+                - created_at
+                - created_by
         """
         ...
 
     def add_elements(
-        self, indexset_id: int, elements: int | List[int | str] | str
+        self, indexset_id: int, elements: float | int | List[float | int | str] | str
     ) -> None:
         """Adds elements to an existing IndexSet.
 
         Parameters
         ----------
         indexset_id : int
             The id of the target IndexSet.
-        elements : int | List[int | str] | str
+        elements : float | int | List[float | int | str] | str
             The elements to be added to the IndexSet.
 
         Returns
         -------
         None:
             Due to compatibility with ixmp.
         """
```

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/optimization/scalar.py` & `ixmp4-0.8.1/ixmp4/data/abstract/optimization/scalar.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         -------
         :class:`ixmp4.data.abstract.optimization.Scalar`:
             The retrieved Scalar.
         """
         ...
 
     def get_by_id(self, id: int) -> Scalar:
-        """Retrieves a Scalar by it's id.
+        """Retrieves a Scalar by its id.
 
         Parameters
         ----------
         id : int
             Unique integer id.
 
         Raises
@@ -166,11 +166,13 @@
         Returns
         -------
         :class:`pandas.DataFrame`:
             A data frame with the columns:
                 - id
                 - name
                 - value
-                - `ixmp4.data.abstract.Unit`
-                - `ixmp4.data.abstract.Unit`.id
+                - unit__id
+                - run__id
+                - created_at
+                - created_by
         """
         ...
```

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/region.py` & `ixmp4-0.8.1/ixmp4/data/abstract/region.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,16 @@
         hierarchy: str | None = None,
     ) -> Region:
         try:
             region = self.get(name)
         except Region.NotFound:
             if hierarchy is None:
                 raise TypeError(
-                    """Argument `hierarchy` is required if `Region` with `name` does not
-                     exist."""
+                    "Argument `hierarchy` is required if `Region` with `name` does not "
+                    "exist."
                 )
             return self.create(name, hierarchy)
 
         if hierarchy is not None and region.hierarchy != hierarchy:
             raise Region.NotUnique(name)
         else:
             return region
```

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/run.py` & `ixmp4-0.8.1/ixmp4/data/abstract/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/scenario.py` & `ixmp4-0.8.1/ixmp4/data/abstract/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/abstract/unit.py` & `ixmp4-0.8.1/ixmp4/data/abstract/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/api/__init__.py` & `ixmp4-0.8.1/ixmp4/data/api/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,12 +8,19 @@
     TimeSeries,
     TimeSeriesRepository,
     Variable,
     VariableRepository,
 )
 from .meta import RunMetaEntry, RunMetaEntryRepository
 from .model import Model, ModelRepository
-from .optimization import IndexSet, IndexSetRepository, Scalar, ScalarRepository
+from .optimization import (
+    IndexSet,
+    IndexSetRepository,
+    Scalar,
+    ScalarRepository,
+    Table,
+    TableRepository,
+)
 from .region import Region, RegionParent, RegionRepository
 from .run import Run, RunRepository
 from .scenario import Scenario, ScenarioRepository
 from .unit import Unit, UnitRepository
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/base.py` & `ixmp4-0.8.1/ixmp4/data/api/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,39 @@
+import asyncio
 import logging
 from json.decoder import JSONDecodeError
-from typing import Any, ClassVar, Generic, Type, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    ClassVar,
+    Coroutine,
+    Generic,
+    Type,
+    TypeVar,
+)
 
 import httpx
 import pandas as pd
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import ConfigDict, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 
 from ixmp4.conf import settings
 from ixmp4.core.exceptions import (
+    ApiEncumbered,
     ImproperlyConfigured,
     IxmpError,
     UnknownApiError,
     registry,
 )
 
+if TYPE_CHECKING:
+    from ixmp4.data.backend.api import RestBackend
+
 logger = logging.getLogger(__name__)
 
 
 class BaseModel(PydanticBaseModel):
     NotFound: ClassVar[type[IxmpError]]
     NotUnique: ClassVar[type[IxmpError]]
 
@@ -80,18 +94,18 @@
 
 
 class BaseRepository(Generic[ModelType]):
     model_class: Type[ModelType]
     prefix: ClassVar[str]
     enumeration_method: str = "PATCH"
 
-    client: httpx.Client
+    backend: "RestBackend"
 
-    def __init__(self, client: httpx.Client, *args, **kwargs) -> None:
-        self.client = client
+    def __init__(self, backend: "RestBackend", *args, **kwargs) -> None:
+        self.backend = backend
 
     def sanitize_params(self, params: dict):
         return {k: params[k] for k in params if params[k] is not None}
 
     def get_remote_exception(self, res: httpx.Response, status_code: int):
         try:
             json = res.json()
@@ -108,36 +122,95 @@
         except KeyError:
             raise ImproperlyConfigured(
                 "Could not find remote exception in registry. "
                 "Are you sure client and server ixmp versions are compatible?"
             )
         return exc.from_dict(json)
 
-    def _request(
+    def _request(self, *args, **kwargs) -> dict | list | None:
+        res = asyncio.run(self._async_request(*args, **kwargs))
+        return res
+
+    async def _async_request(
         self,
         method: str,
         path: str,
         params: dict | None = None,
         json: dict | None = None,
+        max_retries: int = settings.client_max_request_retries,
         **kwargs,
     ) -> dict | list | None:
-        """Sends a request and reraises remote exception if thrown."""
+        """Sends an asyncronous request and handles potential error responses.
+        Uses the backend's semaphore to limit how many
+        requests are sent concurrently per backend.
+        Re-raises a remote `IxmpError` if thrown and transferred from the backend.
+        Handles read timeouts and rate limiting responses
+        via retries with exponential backoffs.
+        Returns `None` if the response body is empty
+        but has a status code less than 300.
+        """
+
+        async def retry(max_retries=max_retries) -> dict | list | None:
+            if max_retries == 0:
+                self.backend.semaphore
+                logger.error(f"API Encumbered: '{self.backend.info.dsn}'")
+                raise ApiEncumbered(
+                    f"The service connected to the backend '{self.backend.info.name}' "
+                    "is currently overencumbered with requests. "
+                    "Try again at a later time or re-configure your client "
+                    "to behave more leniently."
+                )
+            # increase backoff by `settings.client_backoff_factor`
+            # for each retry
+            backoff_s = settings.client_backoff_factor * (
+                settings.client_max_request_retries - max_retries
+            )
+            logger.debug(f"Retrying request in {backoff_s} seconds.")
+            await asyncio.sleep(backoff_s)
+            return await self._async_request(
+                method,
+                path,
+                params=params,
+                json=json,
+                max_retries=max_retries - 1,
+                **kwargs,
+            )
+
         if params is None:
             params = {}
         else:
             params = self.sanitize_params(params)
 
-        res = self.client.request(method, path, params=params, json=json, **kwargs)
+        try:
+            async with self.backend.semaphore:
+                res = await self.backend.async_client.request(
+                    method, path, params=params, json=json, **kwargs
+                )
+        except httpx.ReadTimeout:
+            logger.warn("Read timeout, retrying request...")
+            return await retry()
 
-        if res.status_code >= 400:
+        return await self._async_handle_response(res, retry)
+
+    async def _async_handle_response(
+        self,
+        res: httpx.Response,
+        retry: Callable[..., Coroutine[Any, Any, dict | list | None]],
+    ) -> dict | list | None:
+        if res.status_code in [
+            429,  # Too Many Requests
+            420,  # Enhance Your Calm
+        ]:
+            return await retry()
+        elif res.status_code >= 400:
             if res.status_code == 413:
                 raise ImproperlyConfigured(
                     "Received status code 413 (Payload Too Large). "
-                    "Consider decreasing `IXMP4_DEFAULT_UPLOAD_CHUNK_SIZE` "
-                    f"(current: {settings.default_upload_chunk_size})."
+                    "Consider decreasing `IXMP4_CLIENT_DEFAULT_UPLOAD_CHUNK_SIZE` "
+                    f"(current: {settings.client_default_upload_chunk_size})."
                 )
             raise self.get_remote_exception(res, res.status_code)
         else:
             try:
                 return res.json()
             except JSONDecodeError:
                 if res.status_code < 300 and res.text == "":
@@ -163,41 +236,73 @@
         return self._request(
             self.enumeration_method,
             self.prefix,
             params={**params, "table": table},
             json=json,
         )
 
+    def _build_pagination_requests(
+        self,
+        total: int,
+        start: int,
+        limit: int,
+        params: dict | None,
+        json: dict | None,
+    ) -> list[Coroutine]:
+        requests: list[Coroutine] = []
+        for req_offset in range(start, total, limit):
+            if params is not None:
+                req_params = params.copy()
+            else:
+                req_params = {}
+
+            req_params.update({"limit": limit, "offset": req_offset})
+            request = self._async_request(
+                self.enumeration_method,
+                self.prefix,
+                params=req_params,
+                json=json,
+            )
+            requests.append(request)
+        return requests
+
+    def _collect_pagination_results(self, requests: list[Coroutine]) -> list:
+        async def gather():
+            return await asyncio.gather(*requests)
+
+        responses = asyncio.run(gather())
+        return [r.pop("results") for r in responses]
+
     def _handle_pagination(
         self,
         data: dict,
         table: bool = False,
         params: dict | None = None,
         json: dict | None = None,
     ) -> list[list] | list[dict]:
         """Handles paginated response and sends subsequent requests if necessary.
         Returns aggregated pages as a list."""
 
+        if params is None:
+            params = {"table": table}
+        else:
+            params["table"] = table
+
         total = data.pop("total")
         pagination = data.pop("pagination")
         offset = pagination.pop("offset")
         limit = pagination.pop("limit")
         if total <= offset + limit:
             return [data.pop("results")]
         else:
-            new_params = {"limit": limit, "offset": offset + limit}
-            if params is not None:
-                params.update(new_params)
-            else:
-                params = new_params
-            next_data = self._request_enumeration(table=table, params=params, json=json)
-            pages = self._handle_pagination(
-                next_data, table=table, params=params, json=json
+            requests = self._build_pagination_requests(
+                total, offset + limit, limit, params, json
             )
-            return [data.pop("results")] + pages
+            results = self._collect_pagination_results(requests)
+            return [data.pop("results")] + results
 
     def _list(
         self, params: dict | None = None, json: dict | None = None, **kwargs
     ) -> list[ModelType]:
         data = self._request_enumeration(params=params, table=False, json=json)
         if isinstance(data, dict):
             # we can assume this type on list endpoints
@@ -291,15 +396,15 @@
             yield chunk
 
 
 class BulkUpserter(BulkOperator[ModelType]):
     def bulk_upsert(
         self,
         df: pd.DataFrame,
-        chunk_size: int = settings.default_upload_chunk_size,
+        chunk_size: int = settings.client_default_upload_chunk_size,
         **kwargs,
     ):
         for chunk in self.yield_chunks(df, chunk_size):
             self.bulk_upsert_chunk(chunk, **kwargs)
 
     def bulk_upsert_chunk(self, df: pd.DataFrame, **kwargs) -> None:
         dict_ = df_to_dict(df)
@@ -312,15 +417,15 @@
         )
 
 
 class BulkDeleter(BulkOperator[ModelType]):
     def bulk_delete(
         self,
         df: pd.DataFrame,
-        chunk_size: int = settings.default_upload_chunk_size,
+        chunk_size: int = settings.client_default_upload_chunk_size,
         **kwargs,
     ):
         for chunk in self.yield_chunks(df, chunk_size):
             self.bulk_delete_chunk(chunk, **kwargs)
 
     def bulk_delete_chunk(self, df: pd.DataFrame, **kwargs) -> None:
         dict_ = df_to_dict(df)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/docs.py` & `ixmp4-0.8.1/ixmp4/data/api/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/api/iamc/datapoint.py` & `ixmp4-0.8.1/ixmp4/data/api/iamc/datapoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,12 +59,12 @@
             json=kwargs,
             params={
                 "join_parameters": join_parameters,
                 "join_runs": join_runs,
             },
         )
 
-    def bulk_upsert(self, df: pd.DataFrame) -> None:
+    def bulk_upsert(self, df: pd.DataFrame, **kwargs) -> None:
         super().bulk_upsert(df)
 
-    def bulk_delete(self, df: pd.DataFrame) -> None:
+    def bulk_delete(self, df: pd.DataFrame, **kwargs) -> None:
         super().bulk_delete(df)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/iamc/timeseries.py` & `ixmp4-0.8.1/ixmp4/data/api/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/api/iamc/variable.py` & `ixmp4-0.8.1/ixmp4/data/api/iamc/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     base.Retriever[Variable],
     base.Enumerator[Variable],
     abstract.VariableRepository,
 ):
     model_class = Variable
     prefix = "iamc/variables/"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = VariableDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = VariableDocsRepository(self.backend)
 
     def create(
         self,
         name: str,
     ) -> Variable:
         return super().create(name=name)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/meta.py` & `ixmp4-0.8.1/ixmp4/data/api/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/api/model.py` & `ixmp4-0.8.1/ixmp4/data/api/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     base.Retriever[Model],
     base.Enumerator[Model],
     abstract.ModelRepository,
 ):
     model_class = Model
     prefix = "models/"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = ModelDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = ModelDocsRepository(self.backend)
 
     def create(
         self,
         name: str,
     ) -> Model:
         return super().create(name=name)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/optimization/indexset.py` & `ixmp4-0.8.1/ixmp4/data/api/optimization/indexset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from datetime import datetime
 from typing import ClassVar, List
 
 import pandas as pd
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictFloat, StrictInt, StrictStr
 
 from ixmp4.data import abstract
 
 from .. import base
 from ..docs import Docs, DocsRepository
 
 
 class IndexSet(base.BaseModel):
     NotFound: ClassVar = abstract.IndexSet.NotFound
     NotUnique: ClassVar = abstract.IndexSet.NotUnique
     DeletionPrevented: ClassVar = abstract.IndexSet.DeletionPrevented
 
     id: int
     name: str
-    elements: StrictInt | list[StrictInt | StrictStr] | StrictStr | None
+    elements: StrictFloat | StrictInt | list[
+        StrictFloat | StrictInt | StrictStr
+    ] | StrictStr | None
     run__id: int
 
     created_at: datetime | None
     created_by: str | None
 
 
 class IndexSetDocsRepository(DocsRepository):
@@ -34,17 +36,17 @@
     base.Retriever[IndexSet],
     base.Enumerator[IndexSet],
     abstract.IndexSetRepository,
 ):
     model_class = IndexSet
     prefix = "optimization/indexsets/"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = IndexSetDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = IndexSetDocsRepository(self.backend)
 
     def create(
         self,
         run_id: int,
         name: str,
     ) -> IndexSet:
         return super().create(run_id=run_id, name=name)
@@ -60,11 +62,14 @@
 
     def tabulate(self, **kwargs) -> pd.DataFrame:
         return super()._tabulate(json=kwargs)
 
     def add_elements(
         self,
         indexset_id: int,
-        elements: StrictInt | List[StrictInt | StrictStr] | StrictStr,
+        elements: StrictFloat
+        | StrictInt
+        | List[StrictFloat | StrictInt | StrictStr]
+        | StrictStr,
     ) -> None:
         kwargs = {"indexset_id": indexset_id, "elements": elements}
         self._request("PATCH", self.prefix + str(indexset_id) + "/", json=kwargs)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/optimization/scalar.py` & `ixmp4-0.8.1/ixmp4/data/api/optimization/scalar.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,18 @@
     base.Creator[Scalar],
     base.Retriever[Scalar],
     base.Enumerator[Scalar],
     abstract.ScalarRepository,
 ):
     model_class = Scalar
     prefix = "optimization/scalars/"
-    enumeration_method = "PATCH"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = ScalarDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = ScalarDocsRepository(self.backend)
 
     def create(
         self,
         name: str,
         value: float,
         unit_name: str,
         run_id: int,
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/region.py` & `ixmp4-0.8.1/ixmp4/data/api/region.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     base.Retriever[Region],
     base.Enumerator[Region],
     abstract.RegionRepository,
 ):
     model_class = Region
     prefix = "regions/"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = RegionDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = RegionDocsRepository(self.backend)
 
     def create(
         self,
         name: str,
         hierarchy: str,
     ) -> Region:
         return super().create(name=name, hierarchy=hierarchy)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/run.py` & `ixmp4-0.8.1/ixmp4/data/api/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/api/scenario.py` & `ixmp4-0.8.1/ixmp4/data/api/scenario.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     base.Retriever[Scenario],
     base.Enumerator[Scenario],
     abstract.ScenarioRepository,
 ):
     model_class = Scenario
     prefix = "scenarios/"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = ScenarioDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = ScenarioDocsRepository(self.backend)
 
     def create(
         self,
         name: str,
     ) -> Scenario:
         return super().create(name=name)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/api/unit.py` & `ixmp4-0.8.1/ixmp4/data/api/unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     base.Retriever[Unit],
     base.Enumerator[Unit],
     abstract.UnitRepository,
 ):
     model_class = Unit
     prefix = "units/"
 
-    def __init__(self, client, *args, **kwargs) -> None:
-        super().__init__(client, *args, **kwargs)
-        self.docs = UnitDocsRepository(self.client)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.docs = UnitDocsRepository(self.backend)
 
     def create(
         self,
         name: str,
     ) -> Unit:
         return super().create(name=name)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/auth/context.py` & `ixmp4-0.8.1/ixmp4/data/auth/context.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/auth/decorators.py` & `ixmp4-0.8.1/ixmp4/data/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/backend/api.py` & `ixmp4-0.8.1/ixmp4/data/backend/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 
 import httpx
 import pandas as pd
 from fastapi.testclient import TestClient
 
 from ixmp4.conf import settings
@@ -12,14 +13,15 @@
     DataPointRepository,
     IndexSetRepository,
     ModelRepository,
     RunMetaEntryRepository,
     RunRepository,
     ScalarRepository,
     ScenarioRepository,
+    TableRepository,
     TimeSeriesRepository,
     VariableRepository,
 )
 from ixmp4.data.api.region import RegionRepository
 from ixmp4.data.api.unit import UnitRepository
 from ixmp4.server import app, v1
 from ixmp4.server.rest import APIInfo, deps
@@ -27,33 +29,52 @@
 from .base import Backend
 
 logger = logging.getLogger(__name__)
 
 
 class RestBackend(Backend):
     client: httpx.Client
-
-    def __init__(self, info: PlatformInfo, auth: BaseAuth | None = None) -> None:
+    async_client: httpx.AsyncClient
+    semaphore: asyncio.Semaphore
+    timeout: httpx.Timeout
+
+    def __init__(
+        self,
+        info: PlatformInfo,
+        auth: BaseAuth | None = None,
+        max_concurrent_requests: int = settings.client_max_concurrent_requests,
+    ) -> None:
         super().__init__(info)
-        logger.info(f"Connecting to IXMP4 REST API at {info.dsn}")
+        logger.info(f"Connecting to IXMP4 REST API at {info.dsn}.")
+        self.semaphore = asyncio.Semaphore(max_concurrent_requests)
+        self.timeout = httpx.Timeout(settings.client_timeout, connect=60.0)
         if isinstance(info, ManagerPlatformInfo):
             if info.notice is not None:
                 logger.info("Platform notice: " + info.notice)
         self.make_client(info.dsn, auth=auth)
         self.create_repositories()
 
     def make_client(self, rest_url: str, auth: BaseAuth | None):
         auth = self.get_auth(rest_url, auth)
 
         self.client = httpx.Client(
             base_url=rest_url,
-            timeout=30.0,
+            timeout=self.timeout,
+            http2=True,
+            auth=auth,
+        )
+        self.async_client = httpx.AsyncClient(
+            base_url=rest_url,
+            timeout=self.timeout,
             http2=True,
             auth=auth,
-            follow_redirects=True,
+            # when requesting concurrently,
+            # we send need to send this header
+            # to
+            headers=[("Connection", "close")],
         )
 
     def get_auth(self, rest_url: str, override_auth: BaseAuth | None) -> BaseAuth:
         root = httpx.get(rest_url, follow_redirects=True)
         if root.status_code != 200:
             logger.error("Root API response not OK: " + root.text)
             raise UnknownApiError(f"Server response not OK. ({root.status_code})")
@@ -86,25 +107,26 @@
                     "falling back to self-signed auth."
                 )
                 return SelfSignedAuth(settings.secret_hs256)
         else:
             return override_auth
 
     def create_repositories(self):
-        self.iamc.datapoints = DataPointRepository(self.client)
-        self.iamc.timeseries = TimeSeriesRepository(self.client)
-        self.iamc.variables = VariableRepository(self.client)
-        self.meta = RunMetaEntryRepository(self.client)
-        self.models = ModelRepository(self.client)
-        self.optimization.indexsets = IndexSetRepository(self.client)
-        self.optimization.scalars = ScalarRepository(self.client)
-        self.regions = RegionRepository(self.client)
-        self.runs = RunRepository(self.client)
-        self.scenarios = ScenarioRepository(self.client)
-        self.units = UnitRepository(self.client)
+        self.iamc.datapoints = DataPointRepository(self)
+        self.iamc.timeseries = TimeSeriesRepository(self)
+        self.iamc.variables = VariableRepository(self)
+        self.meta = RunMetaEntryRepository(self)
+        self.models = ModelRepository(self)
+        self.optimization.indexsets = IndexSetRepository(self)
+        self.optimization.scalars = ScalarRepository(self)
+        self.optimization.tables = TableRepository(self)
+        self.regions = RegionRepository(self)
+        self.runs = RunRepository(self)
+        self.scenarios = ScenarioRepository(self)
+        self.units = UnitRepository(self)
 
 
 test_platform = ManagerPlatformInfo(
     id=1,
     management_group=1,
     access_group=1,
     accessibility=ManagerPlatformInfo.Accessibilty.PRIVATE,
@@ -128,15 +150,21 @@
         self.db_backend = db_backend
         self.auth_params = (test_user, mock_manager, test_platform)
         super().__init__(
             test_platform, SelfSignedAuth(settings.secret_hs256), *args, **kwargs
         )
 
     def make_client(self, rest_url: str, auth: BaseAuth):
-        self.client = TestClient(app=app, base_url=rest_url)
+        self.client = TestClient(
+            app=app,
+            base_url=rest_url,
+        )
+        self.async_client = httpx.AsyncClient(
+            app=app, base_url=rest_url, headers=[("Connection", "close")]
+        )
 
         app.dependency_overrides[deps.validate_token] = deps.do_not_validate_token
         v1.dependency_overrides[deps.validate_token] = deps.do_not_validate_token
 
         app.dependency_overrides[deps.get_backend] = deps.get_test_backend_dependency(
             self.db_backend, self.auth_params
         )
```

### Comparing `ixmp4-0.8.0/ixmp4/data/backend/base.py` & `ixmp4-0.8.1/ixmp4/data/backend/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     IndexSetRepository,
     ModelRepository,
     RegionRepository,
     RunMetaEntryRepository,
     RunRepository,
     ScalarRepository,
     ScenarioRepository,
+    TableRepository,
     TimeSeriesRepository,
     UnitRepository,
     VariableRepository,
 )
 
 
 class IamcSubobject(object):
@@ -19,14 +20,15 @@
     timeseries: TimeSeriesRepository
     variables: VariableRepository
 
 
 class OptimizationSubobject(object):
     indexsets: IndexSetRepository
     scalars: ScalarRepository
+    tables: TableRepository
 
 
 class Backend(object):
     iamc: IamcSubobject
     info: PlatformInfo
     meta: RunMetaEntryRepository
     models: ModelRepository
@@ -40,7 +42,10 @@
         self.info = info
         self.iamc = IamcSubobject()
         self.optimization = OptimizationSubobject()
 
     def close(self) -> None:
         """Closes the connection to the database."""
         ...
+
+    def __str__(self):
+        return f"<Backend {self.info}>"
```

### Comparing `ixmp4-0.8.0/ixmp4/data/backend/db.py` & `ixmp4-0.8.1/ixmp4/data/backend/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     IndexSetRepository,
     ModelRepository,
     RegionRepository,
     RunMetaEntryRepository,
     RunRepository,
     ScalarRepository,
     ScenarioRepository,
+    TableRepository,
     TimeSeriesRepository,
     UnitRepository,
     VariableRepository,
 )
 
 from ..auth.context import AuthorizationContext
 from .base import (
@@ -50,14 +51,16 @@
     datapoints: DataPointRepository
     timeseries: TimeSeriesRepository
     variables: VariableRepository
 
 
 class OptimizationSubobject(BaseOptimizationSubobject):
     indexsets: IndexSetRepository
+    scalars: ScalarRepository
+    tables: TableRepository
 
 
 class SqlAlchemyBackend(Backend):
     iamc: IamcSubobject
     info: PlatformInfo
     meta: RunMetaEntryRepository
     models: ModelRepository
@@ -87,14 +90,15 @@
         self.iamc.datapoints = DataPointRepository(self)
         self.iamc.timeseries = TimeSeriesRepository(self)
         self.iamc.variables = VariableRepository(self)
         self.meta = RunMetaEntryRepository(self)
         self.models = ModelRepository(self)
         self.optimization.indexsets = IndexSetRepository(self)
         self.optimization.scalars = ScalarRepository(self)
+        self.optimization.tables = TableRepository(self)
         self.regions = RegionRepository(self)
         self.runs = RunRepository(self)
         self.scenarios = ScenarioRepository(self)
         self.units = UnitRepository(self)
 
     def close(self):
         self.session.close()
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/__init__.py` & `ixmp4-0.8.1/ixmp4/data/db/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 This module contains sqlalchemy database models and repositories.
 """
-# flake8: noqa
 
 from .base import BaseModel, BaseRepository
 from .docs import BaseDocsRepository, docs_model
 from .iamc import (  # AnnualDataPoint,; SubAnnualDataPoint,; CategoricalDataPoint,
     DataPoint,
     DataPointRepository,
     Measurand,
@@ -14,12 +13,21 @@
     TimeSeriesRepository,
     UniversalDataPoint,
     Variable,
     VariableRepository,
 )
 from .meta import RunMetaEntry, RunMetaEntryRepository
 from .model import Model, ModelRepository
-from .optimization import IndexSet, IndexSetRepository, Scalar, ScalarRepository
+from .optimization import (
+    Column,
+    ColumnRepository,
+    IndexSet,
+    IndexSetRepository,
+    Scalar,
+    ScalarRepository,
+    Table,
+    TableRepository,
+)
 from .region import Region, RegionRepository
 from .run import Run, RunRepository
 from .scenario import Scenario, ScenarioRepository
 from .unit import Unit, UnitRepository
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/base.py` & `ixmp4-0.8.1/ixmp4/data/db/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Generic,
     Iterable,
     Iterator,
     Tuple,
     TypeVar,
 )
 
-import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 from sqlalchemy import event, text
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.exc import IntegrityError, NoResultFound
 from sqlalchemy.ext.compiler import compiles
@@ -283,35 +282,28 @@
         return 50_000
 
     def merge_existing(
         self, df: pd.DataFrame, existing_df: pd.DataFrame
     ) -> pd.DataFrame:
         columns = db.utils.get_columns(self.model_class)
         primary_key_columns = db.utils.get_pk_columns(self.model_class)
-        foreign_columns = db.utils.get_foreign_columns(self.model_class)
         on = (
             (
                 set(existing_df.columns) & set(df.columns) & set(columns.keys())
             )  # all cols which exist in both dfs and the db model
             - set(self.model_class.updateable_columns)  # no updateable columns
             - set(primary_key_columns)  # no pk columns
         )  # = all columns that are constant and provided during creation
 
-        ddf = (
-            # https://github.com/dask/dask/issues/9710
-            dd.from_pandas(df, chunksize=512_000)  # type: ignore
-            .set_index(foreign_columns.keys()[0])
-            .merge(
-                existing_df,
-                how="left",
-                on=list(on),
-                suffixes=(None, self.merge_suffix),
-            )
+        return df.merge(
+            existing_df,
+            how="left",
+            on=list(on),
+            suffixes=(None, self.merge_suffix),
         )
-        return ddf.compute()
 
     def drop_merge_artifacts(
         self, df: pd.DataFrame, extra_columns: list[str] | None = None
     ) -> pd.DataFrame:
         if extra_columns is None:
             extra_columns = []
 
@@ -377,15 +369,15 @@
                 self.bulk_upsert_chunk(pd.DataFrame(chunk_df))
 
     def bulk_upsert_chunk(self, df: pd.DataFrame) -> None:
         columns = db.utils.get_columns(self.model_class)
         df = df[list(set(columns.keys()) & set(df.columns))]
         existing_df = self.tabulate_existing(df)
         if existing_df.empty:
-            self.bulk_insert(df)
+            self.bulk_insert(df, skip_validation=True)
         else:
             df = self.merge_existing(df, existing_df)
             df["exists"] = np.where(pd.notnull(df["id"]), True, False)
             cond = []
             for col in self.model_class.updateable_columns:
                 updated_col = col + self.merge_suffix
                 if updated_col in df.columns:
@@ -405,30 +397,30 @@
             )
             update_df = self.drop_merge_artifacts(
                 df.where(df["exists"] & df["differs"]),
                 extra_columns=["differs", "exists"],
             )
 
             if not insert_df.empty:
-                self.bulk_insert(insert_df)
+                self.bulk_insert(insert_df, skip_validation=True)
             if not update_df.empty:
-                self.bulk_update(update_df)
+                self.bulk_update(update_df, skip_validation=True)
 
         self.session.commit()
 
-    def bulk_insert(self, df: pd.DataFrame) -> None:
+    def bulk_insert(self, df: pd.DataFrame, **kwargs) -> None:
         # to_dict returns a more general list[Mapping[Hashable, Unknown]]
         m: list[dict[str, Any]] = df.to_dict("records")  # type: ignore
 
         try:
             self.session.execute(db.insert(self.model_class), m)
         except IntegrityError as e:
             raise self.model_class.NotUnique(*e.args)
 
-    def bulk_update(self, df: pd.DataFrame) -> None:
+    def bulk_update(self, df: pd.DataFrame, **kwargs) -> None:
         # to_dict returns a more general list[Mapping[Hashable, Unknown]]
         m: list[dict[str, Any]] = df.to_dict("records")  # type: ignore
         self.session.bulk_update_mappings(self.model_class, m)  # type: ignore
 
 
 class BulkDeleter(BulkOperator[ModelType]):
     def bulk_delete(self, df: pd.DataFrame) -> None:
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/docs.py` & `ixmp4-0.8.1/ixmp4/data/db/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/filters/meta.py` & `ixmp4-0.8.1/ixmp4/data/db/filters/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/filters/optimizationscalar.py` & `ixmp4-0.8.1/ixmp4/data/db/filters/optimizationscalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/filters/run.py` & `ixmp4-0.8.1/ixmp4/data/db/filters/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,23 +140,23 @@
         Filter for the run, options are id or default_only
 
     Examples
     --------
 
     Return all data points for a given year.
 
-    >>> DataPointFilter(year = 2020)
+    >>> DataPointFilter(year=2020)
 
     Return all data points a number of years
 
-    >>> DataPointFilter(year__in = [2020, 2025])
+    >>> DataPointFilter(year__in=[2020, 2025])
 
     Return all data point that map to a given variable
 
-    >>> DataPointFilter(variable = VariableFilter(name = "variable 1"))
+    >>> DataPointFilter(variable=VariableFilter(name="variable 1"))
 
     Note that for actual use providing the filter parameters as key word arguments is
     sufficient. Calling an endpoint could look like this:
 
     >>> filter = {"variable": {"name": "variable 1"}, "year": 2020}
     >>> iamc.tabulate(**filter)
     """
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/model.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/datapoint/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/measurand.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/measurand.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/timeseries/model.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/timeseries/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,17 +119,21 @@
 
         def map_measurand(df):
             variable_name, unit__id = df.name
             measurand = self.measurands.get_or_create(
                 variable_name=variable_name, unit__id=int(unit__id)
             )
             df["measurand__id"] = measurand.id
+            df["variable"] = variable_name
+            df["unit__id"] = unit__id
             return df
 
         return pd.DataFrame(
-            df.groupby(["variable", "unit__id"], group_keys=False).apply(map_measurand)
+            df.groupby(["variable", "unit__id"], group_keys=False).apply(
+                map_measurand, include_groups=False
+            )
         )
 
     def map_relationships(self, df: pd.DataFrame) -> pd.DataFrame:
         df = self.map_regions(df)
         df = self.map_measurands(df)
         return df
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/variable/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/variable/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/variable/model.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/variable/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/iamc/variable/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/iamc/variable/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/meta/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/meta/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/meta/model.py` & `ixmp4-0.8.1/ixmp4/data/db/meta/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/meta/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/meta/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,20 @@
             )
 
         def map_value_column(df: pd.DataFrame):
             type_str = df.name
             type_ = RunMetaEntry.Type(type_str)
             col = RunMetaEntry._column_map[type_]
             df["value"] = df[col]
+            df["type"] = type_str
             return df.drop(columns=RunMetaEntry._column_map.values())
 
-        return df.groupby("type", group_keys=False).apply(map_value_column)
+        return df.groupby("type", group_keys=False).apply(
+            map_value_column, include_groups=False
+        )
 
     @check_types
     @guard("edit")
     def bulk_upsert(self, df: DataFrame[AddRunMetaEntryFrameSchema]) -> None:
         self.check_df_access(df)
         df["type"] = df["value"].map(type).map(RunMetaEntry.Type.from_pytype)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/model/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/model/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/model/model.py` & `ixmp4-0.8.1/ixmp4/data/db/model/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/model/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/model.py` & `ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     run__id: types.Integer = db.Column(
         db.Integer, db.ForeignKey("run.id"), nullable=False, index=True
     )
 
     __table_args__ = (UniqueConstraint(name, run__id),)
 
     @validates("elements")
-    def validate_elements(self, key, value):
+    def validate_elements(self, key, value: list[float | int | str]):
         unique = set()
         for element in value:
             if element in unique:
                 raise ValueError(f"{element} already defined for IndexSet {self.name}!")
             else:
                 unique.add(element)
         return value
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/optimization/indexset/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def tabulate(self, *args, **kwargs) -> pd.DataFrame:
         return super().tabulate(*args, **kwargs)
 
     @guard("edit")
     def add_elements(
         self,
         indexset_id: int,
-        elements: int | List[int | str] | str,
+        elements: float | int | List[float | int | str] | str,
     ) -> None:
         indexset = self.get_by_id(id=indexset_id)
         if not isinstance(elements, list):
             elements = [elements]
         if indexset.elements is None:
             indexset.elements = elements
         else:
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/model.py` & `ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/optimization/scalar/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/region/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/region/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/region/model.py` & `ixmp4-0.8.1/ixmp4/data/db/region/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/region/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/region/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/run/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/optimization/column/filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from ixmp4.data.db import filters as base
-from ixmp4.data.db.iamc.datapoint import get_datapoint_model
-from ixmp4.data.db.iamc.timeseries import TimeSeries
-from ixmp4.data.db.run.model import Run
+from ixmp4.data.db.optimization.table import Table
 from ixmp4.db import filters, utils
 
+from .model import Column
 
-class IamcRunFilter(filters.BaseFilter, metaclass=filters.FilterMeta):
-    region: base.RegionFilter
-    variable: base.VariableFilter
-    unit: base.UnitFilter
 
+# NB: This is currently not in use, but would be the basis to filter Columns by
+# corresponding Tables
+class OptimizationTableFilter(
+    base.OptimizationTableFilter, metaclass=filters.FilterMeta
+):
     def join(self, exc, session=None):
-        if not utils.is_joined(exc, TimeSeries):
-            exc = exc.join(TimeSeries, onclause=TimeSeries.run__id == Run.id)
-
-        model = get_datapoint_model(session)
-        if not utils.is_joined(exc, model):
-            exc = exc.join(model, onclause=model.time_series__id == TimeSeries.id)
+        if not utils.is_joined(exc, Table):
+            exc = exc.join(Table, onclause=Column.table__id == Table.id)
         return exc
 
 
-class RunFilter(base.RunFilter, metaclass=filters.FilterMeta):
-    iamc: IamcRunFilter | filters.Boolean
-
-    def join(self, exc, **kwargs):
+class OptimizationColumnFilter(
+    base.OptimizationColumnFilter, metaclass=filters.FilterMeta
+):
+    def join(self, exc, session=None):
         return exc
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/run/model.py` & `ixmp4-0.8.1/ixmp4/data/db/run/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import ClassVar
 
 from ixmp4 import db
 from ixmp4.data import abstract, types
 from ixmp4.data.db.model.model import Model
 from ixmp4.data.db.optimization.indexset import IndexSet
 from ixmp4.data.db.optimization.scalar import Scalar
+from ixmp4.data.db.optimization.table import Table
 from ixmp4.data.db.scenario.model import Scenario
 
 from .. import base
 
 
 class Run(base.BaseModel):
     NotFound: ClassVar = abstract.Run.NotFound
@@ -37,10 +38,11 @@
         "Scenario",
         backref="run",
         foreign_keys=[scenario__id],
     )
 
     indexsets: types.Mapped[list["IndexSet"]] = db.relationship()
     scalars: types.Mapped[list["Scalar"]] = db.relationship()
+    tables: types.Mapped[list["Table"]] = db.relationship()
 
     version: types.Integer = db.Column(db.Integer, nullable=False)
     is_default: types.Boolean = db.Column(db.Boolean, default=False, nullable=False)
```

### Comparing `ixmp4-0.8.0/ixmp4/data/db/run/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/run/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/scenario/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/scenario/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/scenario/model.py` & `ixmp4-0.8.1/ixmp4/data/db/scenario/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/scenario/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/scenario/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/timeseries.py` & `ixmp4-0.8.1/ixmp4/data/db/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/unit/filter.py` & `ixmp4-0.8.1/ixmp4/data/db/unit/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/db/unit/repository.py` & `ixmp4-0.8.1/ixmp4/data/db/unit/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/data/generator.py` & `ixmp4-0.8.1/ixmp4/data/generator.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/__init__.py` & `ixmp4-0.8.1/ixmp4/db/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
    # run one migration backward
    alembic downgrade -1
 
    # autogenerate new migration (please choose a descriptive change message)
    alembic revision -m "<message>" --autogenerate
 
 You will have to run all migrations before being able to create new ones
-in the development database. Be sure to run ``black`` on newly created
+in the development database. Be sure to run ``ruff`` on newly created
 migrations before committing them!
 
 """
 # flake8: noqa
 
 from sqlalchemy import (
     ForeignKey,
@@ -45,14 +45,15 @@
     insert,
     or_,
     select,
     sql,
     update,
 )
 from sqlalchemy.dialects.postgresql import JSONB
+from sqlalchemy.exc import MultipleResultsFound
 from sqlalchemy.orm import (
     Relationship,
     Session,
     aliased,
     backref,
     mapped_column,
     relationship,
```

### Comparing `ixmp4-0.8.0/ixmp4/db/filters.py` & `ixmp4-0.8.1/ixmp4/db/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 )
         else:
             override_lookups = None
         if isinstance(override_lookups, list):
             lookups = {k: v for k, v in lookups.items() if k in override_lookups}
         elif override_lookups is None:
             pass
-        else:  # TODO (How) do we ensure the type of override_lookups?
+        else:
             lookups = {}
         base_field_alias = str(field.alias) if field.alias else field_name
 
         cls.expand_lookups(
             field_name,
             lookups,
             namespace,
```

### Comparing `ixmp4-0.8.0/ixmp4/db/migrations/env.py` & `ixmp4-0.8.1/ixmp4/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py` & `ixmp4-0.8.1/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py` & `ixmp4-0.8.1/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py` & `ixmp4-0.8.1/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/utils/__init__.py` & `ixmp4-0.8.1/ixmp4/db/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/utils/alembic.py` & `ixmp4-0.8.1/ixmp4/db/utils/alembic.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/db/utils/sqlite.py` & `ixmp4-0.8.1/ixmp4/db/utils/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 def get_dsn(database_path: Path) -> str:
     """Returns sqlalchemy-friendly sqlite database URI for a given database name."""
 
     return database_path.absolute().as_uri().replace("file://", "sqlite:///")
 
 
 def search_databases(name: str) -> str | None:
-    """Returns a database URI if the desired database exists, otherwise returns
-    `None`."""
+    """Returns a database URI if the desired database exists, otherwise `None`."""
 
     database_path = get_database_path(name)
     if database_path.exists():
         return get_dsn(database_path)
     else:
         return None
```

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/__init__.py` & `ixmp4-0.8.1/ixmp4/server/rest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .iamc import datapoint, timeseries
 from .iamc import model as iamc_model
 from .iamc import region as iamc_region
 from .iamc import scenario as iamc_scenario
 from .iamc import unit as iamc_unit
 from .iamc import variable as iamc_variable
 from .middleware import RequestSizeLoggerMiddleware, RequestTimeLoggerMiddleware
-from .optimization import indexset, scalar
+from .optimization import indexset, scalar, table
 
 v1 = FastAPI(
     servers=[{"url": "/v1", "description": "v1"}],
     redirect_slashes=False,
     docs_url="/docs/",
     redoc_url="/redoc/",
 )
@@ -48,14 +48,15 @@
 v1.include_router(indexset.router, prefix="/optimization")
 v1.include_router(meta.router)
 v1.include_router(model.router)
 v1.include_router(region.router)
 v1.include_router(run.router)
 v1.include_router(scalar.router, prefix="/optimization")
 v1.include_router(scenario.router)
+v1.include_router(table.router, prefix="/optimization")
 v1.include_router(timeseries.router, prefix="/iamc")
 v1.include_router(unit.router)
 
 
 class APIInfo(BaseModel):
     name: str
     version: str
```

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/base.py` & `ixmp4-0.8.1/ixmp4/server/rest/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/deps.py` & `ixmp4-0.8.1/ixmp4/server/rest/deps.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/docs.py` & `ixmp4-0.8.1/ixmp4/server/rest/docs.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,7 +209,31 @@
 
 @router.delete("/optimization/scalars/{dimension_id}/")
 def delete_scalars(
     dimension_id: int = Path(),
     backend: Backend = Depends(deps.get_backend),
 ):
     return backend.optimization.scalars.docs.delete(dimension_id)
+
+
+@router.get("/optimization/tables/", response_model=list[api.Docs])
+def list_tables(
+    dimension_id: int | None = Query(None),
+    backend: Backend = Depends(deps.get_backend),
+):
+    return backend.optimization.tables.docs.list(dimension_id=dimension_id)
+
+
+@router.post("/optimization/tables/", response_model=api.Docs)
+def set_tables(
+    docs: DocsInput,
+    backend: Backend = Depends(deps.get_backend),
+):
+    return backend.optimization.tables.docs.set(**docs.model_dump())
+
+
+@router.delete("/optimization/tables/{dimension_id}/")
+def delete_tables(
+    dimension_id: int = Path(),
+    backend: Backend = Depends(deps.get_backend),
+):
+    return backend.optimization.tables.docs.delete(dimension_id)
```

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/datapoint.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/model.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/region.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/scenario.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/timeseries.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/unit.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/iamc/variable.py` & `ixmp4-0.8.1/ixmp4/server/rest/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/meta.py` & `ixmp4-0.8.1/ixmp4/server/rest/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/middleware.py` & `ixmp4-0.8.1/ixmp4/server/rest/middleware.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/model.py` & `ixmp4-0.8.1/ixmp4/server/rest/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/optimization/indexset.py` & `ixmp4-0.8.1/ixmp4/server/rest/optimization/indexset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fastapi import APIRouter, Body, Depends, Query
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictFloat, StrictInt, StrictStr
 
 from ixmp4.data import api
 from ixmp4.data.backend.db import SqlAlchemyBackend as Backend
 from ixmp4.data.db.optimization.indexset.filter import OptimizationIndexSetFilter
 
 from .. import deps
 from ..base import BaseModel, EnumerationOutput, Pagination
@@ -17,15 +17,17 @@
 
 class IndexSetInput(BaseModel):
     run_id: int
     name: str
 
 
 class ElementsInput(BaseModel):
-    elements: StrictInt | list[StrictInt | StrictStr] | StrictStr
+    elements: StrictFloat | StrictInt | list[
+        StrictFloat | StrictInt | StrictStr
+    ] | StrictStr
 
 
 @autodoc
 @router.patch("/", response_model=EnumerationOutput[api.IndexSet])
 def query(
     filter: OptimizationIndexSetFilter = Body(OptimizationIndexSetFilter()),
     table: bool = Query(False),
```

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/optimization/scalar.py` & `ixmp4-0.8.1/ixmp4/server/rest/optimization/scalar.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from fastapi import APIRouter, Body, Depends, Query
-from pydantic import RootModel
 
 from ixmp4.data import api
-from ixmp4.data.backend.base import Backend
-from ixmp4.data.db.filters.optimizationscalar import OptimizationScalarFilter
+from ixmp4.data.backend.db import SqlAlchemyBackend as Backend
+from ixmp4.data.db.optimization.scalar.filter import OptimizationScalarFilter
 
 from .. import deps
-from ..base import BaseModel
+from ..base import BaseModel, EnumerationOutput, Pagination
 from ..decorators import autodoc
 
 router: APIRouter = APIRouter(
     prefix="/scalars",
     tags=["optimization", "scalars"],
 )
 
@@ -23,47 +22,43 @@
 
 
 class ScalarUpdateInput(BaseModel):
     value: float | None
     unit_id: int | None
 
 
-class EnumerationOutput(BaseModel, RootModel):
-    root: list[api.Scalar] | api.DataFrame
-
-
-@autodoc
-@router.get("/", response_model=EnumerationOutput)
-def enumerate(
-    filter: OptimizationScalarFilter = Depends(),
-    table: bool | None = Query(False),
-    backend: Backend = Depends(deps.get_backend),
-):
-    return backend.optimization.scalars.enumerate(_filter=filter, table=bool(table))
-
-
 @autodoc
 @router.get("/{id}/", response_model=api.Scalar)
 def get_by_id(
     id: int,
     backend: Backend = Depends(deps.get_backend),
 ):
     return backend.optimization.scalars.get_by_id(id)
 
 
 @autodoc
-@router.patch("/", response_model=EnumerationOutput)
+@router.patch("/", response_model=EnumerationOutput[api.Scalar])
 def query(
     filter: OptimizationScalarFilter = Body(
         OptimizationScalarFilter(id=None, name=None, unit__id=None)
     ),
     table: bool = Query(False),
+    pagination: Pagination = Depends(),
     backend: Backend = Depends(deps.get_backend),
 ):
-    return backend.optimization.scalars.enumerate(_filter=filter, table=bool(table))
+    return EnumerationOutput(
+        results=backend.optimization.scalars.paginate(
+            _filter=filter,
+            limit=pagination.limit,
+            offset=pagination.offset,
+            table=bool(table),
+        ),
+        total=backend.optimization.scalars.count(_filter=filter),
+        pagination=pagination,
+    )
 
 
 @autodoc
 @router.patch("/{id}/", response_model=api.Scalar)
 def update(
     id: int,
     scalar: ScalarUpdateInput,
```

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/region.py` & `ixmp4-0.8.1/ixmp4/server/rest/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/run.py` & `ixmp4-0.8.1/ixmp4/server/rest/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/scenario.py` & `ixmp4-0.8.1/ixmp4/server/rest/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/ixmp4/server/rest/unit.py` & `ixmp4-0.8.1/ixmp4/server/rest/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.0/pyproject.toml` & `ixmp4-0.8.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,82 +2,83 @@
 authors = [
     "Max Wolschlager <wolschlager@iiasa.ac.at>",
     "Fridolin Glatter <glatter@iiasa.ac.at>",
     "Daniel Huppmann <huppmann@iiasa.ac.at>",
     "Philip Hackstock <hackstock@iiasa.ac.at>",
 ]
 name = "ixmp4"
-version = "0.8.0"
+version = "0.8.1"
 description = "a data warehouse for scenario analysis"
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ixmp4" }, { include = "ixmp4/py.typed" }]
 homepage = "https://software.ece.iiasa.ac.at"
 repository = "https://github.com/iiasa/ixmp4"
 documentation = "https://docs.ece.iiasa.ac.at/projects/ixmp4"
 
 [tool.poetry.dependencies]
-PyJWT = "^2.4.0"
-SQLAlchemy = { extras = ["mypy"], version = "^2.0.25" }
-SQLAlchemy-Utils = "^0.41.1"
-alembic = "^1.13.1"
-dask = { extras = ["dataframe"], version = "^2024.1.1" }
-fastapi = "^0.109.0"
-httpx = { extras = ["http2"], version = "^0.26.0" }
-openpyxl = "^3.0.9"
-pandas = "~2.1.2"
-pandera = "^0.18.0"
-pydantic = "^2.5.3"
+PyJWT = ">=2.4.0"
+SQLAlchemy = { extras = ["mypy"], version = ">=2.0.22" }
+SQLAlchemy-Utils = ">=0.41.0"
+alembic = ">=1.12.0"
+fastapi = ">=0.100.0"
+httpx = { extras = ["http2"], version = ">=0.25.0" }
+openpyxl = ">=3.0.9"
+pandas = [
+    {version = ">=2.1.1", python = ">=3.12"},
+    {version = ">=2.0.0", python = ">=3.10"}
+]
+pandera = ">=0.17.0"
+pydantic = ">=2.3.0"
 python = ">=3.10, <3.13"
-python-dotenv = "^1.0.1"
-requests = "^2.27.1"
-typer = "^0.9.0"
-toml = "^0.10.2"
-psycopg = { extras = ["binary"], version = "^3.1.17" }
-pydantic-settings = "^2.1.0"
-rich = "^13.7.0"
+python-dotenv = ">=1.0.1"
+typer = ">=0.9.0"
+toml = ">=0.10.2"
+psycopg = { extras = ["binary"], version = "^3.1.12" }
+pydantic-settings = ">=2.1.0"
+rich = ">=13.5.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^7.2.6"
-sphinx-multiversion = "^0.2.4"
-sphinx-rtd-theme = "^2.0.0"
-sphinxcontrib-bibtex = "^2.6.2"
-sphinxcontrib-openapi = "^0.8.3"
+sphinx = ">=7.2.4"
+sphinx-multiversion = ">=0.2.4"
+sphinx-rtd-theme = ">=2.0.0"
+sphinxcontrib-bibtex = ">=2.6.1"
+sphinxcontrib-openapi = ">=0.8.1"
 
 [tool.poetry.group.server]
 optional = true
 
 [tool.poetry.group.server.dependencies]
-gunicorn = "^21.2.0"
-uvicorn = { extras = ["standard"], version = "^0.27.0.post1" }
+gunicorn = ">=21.2.0"
+uvicorn = { extras = ["standard"], version = ">=0.24.0" }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-ptvsd = "^4.3.2"
-pytest = "^8.0.0"
-pytest-benchmark = "^4.0.0"
-pytest-cov = "^4.1.0"
-snakeviz = "^2.1.1"
-types-toml = "^0.10.8.7"
-build = "^1.0.3"
-ruff = "^0.2.1"
-pre-commit = "^3.6.0"
-mypy = "^1.8.0"
-pandas-stubs = "^2.1.4.231227"
+build = ">=1.0.3"
+mypy = ">=1.0.0"
+pandas-stubs = ">=2.0.0.230412"
+pre-commit = ">=3.3.3"
+ptvsd = ">=4.3.2"
+pytest = ">=8.0.0"
+pytest-benchmark = ">=4.0.0"
+pytest-cov = ">=4.1.0"
+ruff = ">=0.2.0"
+snakeviz = ">=2.1.1"
+types-toml = ">=0.10.8.7"
 
 [tool.poetry.group.tutorial]
 optional = true
 
 [tool.poetry.group.tutorial.dependencies]
-ipykernel = "^6.29.0"
+ipykernel = ">=6.27.1"
 
 [tool.poetry.scripts]
 ixmp4 = "ixmp4.__main__:app"
 
 [build-system]
 build-backend = "poetry_dynamic_versioning.backend"
 requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
@@ -107,14 +108,18 @@
     ".mypy_cache",
     ".venv",
     "example.py",
     "import.py",
 ]
 line-length = 88
 
+[tool.ruff.format]
+# Enable reformatting of code snippets in docstrings.
+docstring-code-format = true
+
 [tool.ruff.lint]
 select = ["C9", "E", "F", "I", "W"]
 ignore = ["B008"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `ixmp4-0.8.0/PKG-INFO` & `ixmp4-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: ixmp4
-Version: 0.8.0
+Version: 0.8.1
 Summary: a data warehouse for scenario analysis
 Home-page: https://software.ece.iiasa.ac.at
 License: MIT
 Author: Max Wolschlager
 Author-email: wolschlager@iiasa.ac.at
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
-Requires-Dist: SQLAlchemy-Utils (>=0.41.1,<0.42.0)
-Requires-Dist: SQLAlchemy[mypy] (>=2.0.25,<3.0.0)
-Requires-Dist: alembic (>=1.13.1,<2.0.0)
-Requires-Dist: dask[dataframe] (>=2024.1.1,<2025.0.0)
-Requires-Dist: fastapi (>=0.109.0,<0.110.0)
-Requires-Dist: httpx[http2] (>=0.26.0,<0.27.0)
-Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
-Requires-Dist: pandas (>=2.1.2,<2.2.0)
-Requires-Dist: pandera (>=0.18.0,<0.19.0)
-Requires-Dist: psycopg[binary] (>=3.1.17,<4.0.0)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: PyJWT (>=2.4.0)
+Requires-Dist: SQLAlchemy-Utils (>=0.41.0)
+Requires-Dist: SQLAlchemy[mypy] (>=2.0.22)
+Requires-Dist: alembic (>=1.12.0)
+Requires-Dist: fastapi (>=0.100.0)
+Requires-Dist: httpx[http2] (>=0.25.0)
+Requires-Dist: openpyxl (>=3.0.9)
+Requires-Dist: pandas (>=2.0.0) ; python_version >= "3.10"
+Requires-Dist: pandas (>=2.1.1) ; python_version >= "3.12"
+Requires-Dist: pandera (>=0.17.0)
+Requires-Dist: psycopg[binary] (>=3.1.12,<4.0.0)
+Requires-Dist: pydantic (>=2.3.0)
+Requires-Dist: pydantic-settings (>=2.1.0)
+Requires-Dist: python-dotenv (>=1.0.1)
+Requires-Dist: rich (>=13.5.2)
+Requires-Dist: toml (>=0.10.2)
+Requires-Dist: typer (>=0.9.0)
 Project-URL: Documentation, https://docs.ece.iiasa.ac.at/projects/ixmp4
 Project-URL: Repository, https://github.com/iiasa/ixmp4
 Description-Content-Type: text/markdown
 
 # The ixmp4 package for scenario data management
 
 Copyright (c) 2023-2024 IIASA - Energy, Climate, and Environment Program (ECE)
@@ -117,22 +116,22 @@
 ## Developing
 
 See [DEVELOPING.md](DEVELOPING.md) for guidance. When contributing to this project via
 a Pull Request, add your name to the "authors" section in the `pyproject.toml` file.
 
 ## Compatibility
 
-This project mainly targets postgres version 15 but we test version 16 continously also. Tests with pyarrow installed alongside are also run due to its effect on pandas etc.
+This project mainly targets postgres version 16 but we test version 15 continously also. Tests with pyarrow installed alongside are also run due to its effect on pandas etc.
 | python | postgres | with pyarrow |
 |--------|----------|--------------|
-| 3.10 | 15 | false |
-| 3.11 | 15 | false |
-| 3.12 | 15 | false |
-| 3.12 | 15 | true |
+| 3.10 | 16 | false |
+| 3.11 | 16 | false |
 | 3.12 | 16 | false |
+| 3.12 | 16 | true |
+| 3.12 | 15 | false |
 
 ## Funding ackownledgement
 
 <img src="./doc/source/_static/ECEMF-logo.png" width="264" height="100"
 alt="ECEMF logo" />
 <img src="./doc/source/_static/openENTRANCE-logo.png" width="187" height="120"
 alt="openENTRANCE logo" />
```

