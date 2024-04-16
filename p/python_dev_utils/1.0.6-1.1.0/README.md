# Comparing `tmp/python_dev_utils-1.0.6.tar.gz` & `tmp/python_dev_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.0.6.tar", last modified: Sun Apr 14 10:12:32 2024, max compression
+gzip compressed data, was "python_dev_utils-1.1.0.tar", last modified: Mon Apr 15 09:43:59 2024, max compression
```

## Comparing `python_dev_utils-1.0.6.tar` & `python_dev_utils-1.1.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.0.6/LICENCE
--rw-r--r--   0        0        0     1992 2024-04-12 13:50:09.038622 python_dev_utils-1.0.6/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.0.6/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.0.6/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.0.6/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.0.6/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.0.6/dev_utils/core/results.py
--rw-r--r--   0        0        0      776 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/core/utils.py
--rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.0.6/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.0.6/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/handlers.py
--rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/utils.py
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.0.6/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16331 2024-04-12 09:11:29.070964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2241 2024-04-12 13:02:27.561733 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0      652 2024-04-11 07:40:31.379144 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/encryption.py
--rw-r--r--   0        0        0     1955 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/pydantic.py
--rw-r--r--   0        0        0    12623 2024-04-12 09:11:29.069965 python_dev_utils-1.0.6/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     3005 2024-04-14 10:12:32.389819 python_dev_utils-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.0.6/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/core/test_abstract.py
--rw-r--r--   0        0        0      508 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/core/test_guards.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/core/test_results.py
--rw-r--r--   0        0        0      933 2024-04-12 09:01:52.920056 python_dev_utils-1.0.6/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.0.6/tests/fastapi/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.0.6/tests/fastapi/conftest.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions_handlers.py
--rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.0.6/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.0.6/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.0.6/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0     1423 2024-04-12 13:01:52.229885 python_dev_utils-1.0.6/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     7407 2024-04-12 12:47:25.071609 python_dev_utils-1.0.6/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.0.6/tests/types.py
--rw-r--r--   0        0        0     7467 2024-04-12 13:03:36.658336 python_dev_utils-1.0.6/tests/utils.py
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 python_dev_utils-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.1.0/LICENCE
+-rw-r--r--   0        0        0     4373 2024-04-15 09:42:56.043729 python_dev_utils-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.1.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.1.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.1.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.1.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.1.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      776 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/core/utils.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.1.0/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.1.0/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.1.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16331 2024-04-12 09:11:29.070964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2241 2024-04-12 13:02:27.561733 python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0      652 2024-04-11 07:40:31.379144 python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/encryption.py
+-rw-r--r--   0        0        0     1955 2024-04-12 09:11:29.068964 python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0    12623 2024-04-12 09:11:29.069965 python_dev_utils-1.1.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3054 2024-04-15 09:43:59.556198 python_dev_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.1.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      508 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/core/test_results.py
+-rw-r--r--   0        0        0      933 2024-04-12 09:01:52.920056 python_dev_utils-1.1.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.1.0/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.1.0/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.1.0/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.1.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.1.0/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.1.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.1.0/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.1.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.1.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.1.0/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.1.0/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.1.0/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0     1423 2024-04-12 13:01:52.229885 python_dev_utils-1.1.0/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     7407 2024-04-12 12:47:25.071609 python_dev_utils-1.1.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.1.0/tests/types.py
+-rw-r--r--   0        0        0     7467 2024-04-12 13:03:36.658336 python_dev_utils-1.1.0/tests/utils.py
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 python_dev_utils-1.1.0/PKG-INFO
```

### Comparing `python_dev_utils-1.0.6/LICENCE` & `python_dev_utils-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/core/abstract.py` & `python_dev_utils-1.1.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/core/exc.py` & `python_dev_utils-1.1.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/core/guards.py` & `python_dev_utils-1.1.0/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/core/logging.py` & `python_dev_utils-1.1.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/core/results.py` & `python_dev_utils-1.1.0/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/core/utils.py` & `python_dev_utils-1.1.0/dev_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/fastapi/__init__.py` & `python_dev_utils-1.1.0/dev_utils/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.1.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/exc.py` & `python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/handlers.py` & `python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/utils.py` & `python_dev_utils-1.1.0/dev_utils/fastapi/verbose_http_exceptions/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/audit.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/encryption.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/encryption.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/pydantic.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/types/pydantic.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.1.0/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/pyproject.toml` & `python_dev_utils-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -165,27 +165,30 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.0.6"
+version = "1.1.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
+fastapi_exceptions = [
+    "fastapi>=0.110.0",
+]
 profiling = [
     "fastapi>=0.110.0",
     "sqlalchemy>=2.0.28",
 ]
 sqlalchemy_filters = [
     "sqlalchemy>=2.0.28",
 ]
```

### Comparing `python_dev_utils-1.0.6/tests/conftest.py` & `python_dev_utils-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/core/test_abstract.py` & `python_dev_utils-1.1.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/core/test_results.py` & `python_dev_utils-1.1.0/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/core/test_utils.py` & `python_dev_utils-1.1.0/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/fastapi/conftest.py` & `python_dev_utils-1.1.0/tests/fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions.py` & `python_dev_utils-1.1.0/tests/fastapi/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions_handlers.py` & `python_dev_utils-1.1.0/tests/fastapi/test_verbose_http_exceptions_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions_utils.py` & `python_dev_utils-1.1.0/tests/fastapi/test_verbose_http_exceptions_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/mixins/test_general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/test_types.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.1.0/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/types.py` & `python_dev_utils-1.1.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.0.6/tests/utils.py` & `python_dev_utils-1.1.0/tests/utils.py`

 * *Files identical despite different names*

