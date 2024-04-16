# Comparing `tmp/coworks-0.9.4a2.tar.gz` & `tmp/coworks-0.9.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coworks-0.9.4a2.tar", last modified: Tue Apr 16 08:27:38 2024, max compression
+gzip compressed data, was "coworks-0.9.4a3.tar", last modified: Tue Apr 16 15:15:26 2024, max compression
```

## Comparing `coworks-0.9.4a2.tar` & `coworks-0.9.4a3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1067 2024-04-16 08:27:23.929345 coworks-0.9.4a2/LICENSE.txt
--rw-r--r--   0        0        0       71 2024-04-16 08:27:23.933345 coworks-0.9.4a2/NOTICE
--rw-r--r--   0        0        0     4409 2024-04-16 08:27:23.933345 coworks-0.9.4a2/README.rst
--rw-r--r--   0        0        0      643 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/__init__.py
--rw-r--r--   0        0        0     2539 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/aws.py
--rw-r--r--   0        0        0     1255 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/__init__.py
--rw-r--r--   0        0        0     8002 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/group.py
--rw-r--r--   0        0        0    13362 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/operators.py
--rw-r--r--   0        0        0     1761 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/sensors.py
--rw-r--r--   0        0        0     8400 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/admin_blueprint.py
--rw-r--r--   0        0        0     7027 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/mail_blueprint.py
--rw-r--r--   0        0        0     3788 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/okta_blueprint.py
--rw-r--r--   0        0        0      490 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/profiler_blueprint.py
--rw-r--r--   0        0        0      852 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/test_blueprint.py
--rw-r--r--   0        0        0    21424 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/coworks.py
--rwxr-xr-x   0        0        0        0 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/__init__.py
--rw-r--r--   0        0        0     8022 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/client.py
--rw-r--r--   0        0        0      708 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/command.py
--rw-r--r--   0        0        0    24102 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/deploy.py
--rw-r--r--   0        0        0      136 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/exception.py
--rw-r--r--   0        0        0     1413 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/new.py
--rw-r--r--   0        0        0     1091 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/project_templates/README.md
--rw-r--r--   0        0        0     1304 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/project_templates/tech/app.py
--rw-r--r--   0        0        0       34 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/project_templates/template.env
--rw-r--r--   0        0        0      300 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/deploy.j2
--rw-r--r--   0        0        0      294 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/project.cws.yml
--rw-r--r--   0        0        0     2038 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform.j2
--rw-r--r--   0        0        0     2954 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/lambda.j2
--rw-r--r--   0        0        0      438 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/local.j2
--rw-r--r--   0        0        0      375 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/output.j2
--rw-r--r--   0        0        0      416 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/provider.j2
--rw-r--r--   0        0        0     3089 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/request_templates.j2
--rw-r--r--   0        0        0     1301 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/response_templates.j2
--rw-r--r--   0        0        0    10271 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/rest_api.j2
--rw-r--r--   0        0        0     2079 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/role.j2
--rwxr-xr-x   0        0        0     2856 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/utils.py
--rw-r--r--   0        0        0      723 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/__init__.py
--rw-r--r--   0        0        0     3473 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/data.py
--rw-r--r--   0        0        0    12744 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/fetching.py
--rw-r--r--   0        0        0    15584 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/jsonapi.py
--rw-r--r--   0        0        0     1347 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/query.py
--rw-r--r--   0        0        0    10878 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/odoo.py
--rw-r--r--   0        0        0     7704 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/xray.py
--rw-r--r--   0        0        0      166 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/globals.py
--rw-r--r--   0        0        0      217 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/operators.py
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/py.typed
--rw-r--r--   0        0        0      214 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/sensors.py
--rw-r--r--   0        0        0    10633 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/tech/directory.py
--rw-r--r--   0        0        0    12827 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/utils.py
--rw-r--r--   0        0        0      291 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/version.py
--rw-r--r--   0        0        0     8691 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/wrappers.py
--rw-r--r--   0        0        0     2698 2024-04-16 08:27:38.449509 coworks-0.9.4a2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/__init__.py
--rw-r--r--   0        0        0     1380 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/__init__.py
--rw-r--r--   0        0        0      725 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/blueprint.py
--rw-r--r--   0        0        0     3991 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_admin.py
--rw-r--r--   0        0        0     2346 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_blueprint.py
--rw-r--r--   0        0        0      954 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_empty.py
--rw-r--r--   0        0        0     3963 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_mail.py
--rw-r--r--   0        0        0      749 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_overload.py
--rw-r--r--   0        0        0     4461 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/event.py
--rw-r--r--   0        0        0     2214 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/ms.py
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_async.py
--rw-r--r--   0        0        0     2452 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_auth.py
--rw-r--r--   0        0        0     4318 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_content_type.py
--rw-r--r--   0        0        0     8907 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_event.py
--rw-r--r--   0        0        0    11915 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_ms.py
--rw-r--r--   0        0        0     3714 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_type.py
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/__init__.py
--rw-r--r--   0        0        0       47 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/.env.dev
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/__init__.py
--rw-r--r--   0        0        0      870 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/app.py
--rw-r--r--   0        0        0      916 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/command.py
--rw-r--r--   0        0        0      170 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/src/project.cws.yml
--rw-r--r--   0        0        0      294 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/src/project.wrong.yml
--rw-r--r--   0        0        0     2620 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_cmd.py
--rw-r--r--   0        0        0     7488 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_deploy.py
--rw-r--r--   0        0        0     4128 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_environment.py
--rw-r--r--   0        0        0     1464 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_project_file.py
--rw-r--r--   0        0        0        0 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/__init__.py
--rw-r--r--   0        0        0      846 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_client.py
--rw-r--r--   0        0        0     1313 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_complete.py
--rw-r--r--   0        0        0     2791 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_first.py
--rw-r--r--   0        0        0     1036 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_hello.py
--rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 coworks-0.9.4a2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 15:14:17.321187 coworks-0.9.4a3/LICENSE.txt
+-rw-r--r--   0        0        0       71 2024-04-16 15:14:17.321187 coworks-0.9.4a3/NOTICE
+-rw-r--r--   0        0        0     4409 2024-04-16 15:14:17.321187 coworks-0.9.4a3/README.rst
+-rw-r--r--   0        0        0      643 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/__init__.py
+-rw-r--r--   0        0        0     2539 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/aws.py
+-rw-r--r--   0        0        0     1255 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/biz/__init__.py
+-rw-r--r--   0        0        0     8002 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/biz/group.py
+-rw-r--r--   0        0        0    13362 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/biz/operators.py
+-rw-r--r--   0        0        0     1761 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/biz/sensors.py
+-rw-r--r--   0        0        0     8400 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/blueprint/admin_blueprint.py
+-rw-r--r--   0        0        0     7027 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/blueprint/mail_blueprint.py
+-rw-r--r--   0        0        0     3788 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/blueprint/okta_blueprint.py
+-rw-r--r--   0        0        0      490 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/blueprint/profiler_blueprint.py
+-rw-r--r--   0        0        0      852 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/blueprint/test_blueprint.py
+-rw-r--r--   0        0        0    21424 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/coworks.py
+-rwxr-xr-x   0        0        0        0 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/__init__.py
+-rw-r--r--   0        0        0     8230 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/client.py
+-rw-r--r--   0        0        0      708 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/command.py
+-rw-r--r--   0        0        0    24102 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/deploy.py
+-rw-r--r--   0        0        0      136 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/exception.py
+-rw-r--r--   0        0        0     1399 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/new.py
+-rw-r--r--   0        0        0     1091 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/project_templates/README.md
+-rw-r--r--   0        0        0     1304 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/project_templates/tech/app.py
+-rw-r--r--   0        0        0       34 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/project_templates/template.env
+-rw-r--r--   0        0        0      300 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/deploy.j2
+-rw-r--r--   0        0        0      294 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/project.cws.yml
+-rw-r--r--   0        0        0     2038 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform.j2
+-rw-r--r--   0        0        0     2954 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/lambda.j2
+-rw-r--r--   0        0        0      438 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/local.j2
+-rw-r--r--   0        0        0      375 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/output.j2
+-rw-r--r--   0        0        0      416 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/provider.j2
+-rw-r--r--   0        0        0     3089 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/request_templates.j2
+-rw-r--r--   0        0        0     1301 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/response_templates.j2
+-rw-r--r--   0        0        0    10271 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/rest_api.j2
+-rw-r--r--   0        0        0     2079 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/templates/terraform/role.j2
+-rwxr-xr-x   0        0        0     2856 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/cws/utils.py
+-rw-r--r--   0        0        0      723 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/jsonapi/__init__.py
+-rw-r--r--   0        0        0     3473 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/jsonapi/data.py
+-rw-r--r--   0        0        0    12744 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/jsonapi/fetching.py
+-rw-r--r--   0        0        0    15584 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/jsonapi/jsonapi.py
+-rw-r--r--   0        0        0     1347 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/jsonapi/query.py
+-rw-r--r--   0        0        0    10878 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/odoo.py
+-rw-r--r--   0        0        0     7704 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/extension/xray.py
+-rw-r--r--   0        0        0      166 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/globals.py
+-rw-r--r--   0        0        0      217 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/operators.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/py.typed
+-rw-r--r--   0        0        0      214 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/sensors.py
+-rw-r--r--   0        0        0    10633 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/tech/directory.py
+-rw-r--r--   0        0        0    12827 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/utils.py
+-rw-r--r--   0        0        0      291 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/version.py
+-rw-r--r--   0        0        0     8691 2024-04-16 15:14:17.321187 coworks-0.9.4a3/coworks/wrappers.py
+-rw-r--r--   0        0        0     3029 2024-04-16 15:15:26.514158 coworks-0.9.4a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.325187 coworks-0.9.4a3/tests/__init__.py
+-rw-r--r--   0        0        0     1380 2024-04-16 15:14:17.325187 coworks-0.9.4a3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.325187 coworks-0.9.4a3/tests/coworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.325187 coworks-0.9.4a3/tests/coworks/blueprint/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-16 15:14:17.325187 coworks-0.9.4a3/tests/coworks/blueprint/blueprint.py
+-rw-r--r--   0        0        0     3991 2024-04-16 15:14:17.325187 coworks-0.9.4a3/tests/coworks/blueprint/test_admin.py
+-rw-r--r--   0        0        0     2346 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/blueprint/test_blueprint.py
+-rw-r--r--   0        0        0      954 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/blueprint/test_empty.py
+-rw-r--r--   0        0        0     3963 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/blueprint/test_mail.py
+-rw-r--r--   0        0        0      749 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/blueprint/test_overload.py
+-rw-r--r--   0        0        0     4461 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/event.py
+-rw-r--r--   0        0        0     2214 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/ms.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/test_async.py
+-rw-r--r--   0        0        0     2452 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/test_auth.py
+-rw-r--r--   0        0        0     4318 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/test_content_type.py
+-rw-r--r--   0        0        0     8907 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/test_event.py
+-rw-r--r--   0        0        0    11915 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/test_ms.py
+-rw-r--r--   0        0        0     3714 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/coworks/tech/test_type.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/src/.env.dev
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/src/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/src/app.py
+-rw-r--r--   0        0        0      916 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/src/command.py
+-rw-r--r--   0        0        0      170 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/src/project.cws.yml
+-rw-r--r--   0        0        0      294 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/src/project.wrong.yml
+-rw-r--r--   0        0        0     2620 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/test_cmd.py
+-rw-r--r--   0        0        0     7488 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/test_deploy.py
+-rw-r--r--   0        0        0     4169 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/test_environment.py
+-rw-r--r--   0        0        0     1431 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/cws/test_project_file.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/docs/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/docs/test_client.py
+-rw-r--r--   0        0        0     1354 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/docs/test_complete.py
+-rw-r--r--   0        0        0     2791 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/docs/test_first.py
+-rw-r--r--   0        0        0     1036 2024-04-16 15:14:17.329187 coworks-0.9.4a3/tests/docs/test_hello.py
+-rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 coworks-0.9.4a3/PKG-INFO
```

### Comparing `coworks-0.9.4a2/LICENSE.txt` & `coworks-0.9.4a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/README.rst` & `coworks-0.9.4a3/README.rst`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/__init__.py` & `coworks-0.9.4a3/coworks/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/aws.py` & `coworks-0.9.4a3/coworks/aws.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/biz/__init__.py` & `coworks-0.9.4a3/coworks/biz/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/biz/group.py` & `coworks-0.9.4a3/coworks/biz/group.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/biz/operators.py` & `coworks-0.9.4a3/coworks/biz/operators.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/biz/sensors.py` & `coworks-0.9.4a3/coworks/biz/sensors.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/blueprint/admin_blueprint.py` & `coworks-0.9.4a3/coworks/blueprint/admin_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/blueprint/mail_blueprint.py` & `coworks-0.9.4a3/coworks/blueprint/mail_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/blueprint/okta_blueprint.py` & `coworks-0.9.4a3/coworks/blueprint/okta_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/blueprint/test_blueprint.py` & `coworks-0.9.4a3/coworks/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/coworks.py` & `coworks-0.9.4a3/coworks/coworks.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/client.py` & `coworks-0.9.4a3/coworks/cws/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,21 @@
                         cmd = self.commands[name]
                     else:
                         raise click.UsageError(f"The command {name} is undefined or the class option is missing.")
 
                     # Sets option's value as default command param
                     # (may then be forced in command line or defined by default)
                     for param in cmd.params:
-                        param_name = param.name.replace('-', '_')
+                        param_name = param.name
                         if param_name in options:
                             param.default = options.get(param_name)
+                        else:
+                            param_name = param_name.replace('_', '-')
+                            if param_name in options:
+                                param.default = options.get(param_name)
 
                     self.add_command(cmd, name)
 
         return ctx
 
 
 @click.group(cls=CwsGroup)
```

### Comparing `coworks-0.9.4a2/coworks/cws/command.py` & `coworks-0.9.4a3/coworks/cws/command.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/deploy.py` & `coworks-0.9.4a3/coworks/cws/deploy.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/new.py` & `coworks-0.9.4a3/coworks/cws/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import typing as t
-from distutils.dir_util import copy_tree
 from pathlib import Path
+from shutil import copytree
 
 import click
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
 
 from coworks.version import __version__
@@ -24,15 +24,15 @@
     project_conf = Path("project.cws.yml")
 
     if project_conf.exists() and not force:
         click.echo("Project already created. Set 'force' option for recreation.")
         return
 
     # Copy files
-    copy_tree(src.as_posix(), '.')
+    copytree(src.as_posix(), '.')
     Path('template.env').rename('.env')
 
     # Render project configuration file
     template_loader = PackageLoader(t.cast(str, sys.modules[__name__].__package__))
     jinja_env = Environment(loader=template_loader, autoescape=select_autoescape(['html', 'xml']))
     template = jinja_env.get_template('project.cws.yml')
     output = project_conf
```

### Comparing `coworks-0.9.4a2/coworks/cws/project_templates/README.md` & `coworks-0.9.4a3/coworks/cws/project_templates/README.md`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/project_templates/tech/app.py` & `coworks-0.9.4a3/coworks/cws/project_templates/tech/app.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/templates/terraform.j2` & `coworks-0.9.4a3/coworks/cws/templates/terraform.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/templates/terraform/lambda.j2` & `coworks-0.9.4a3/coworks/cws/templates/terraform/lambda.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/templates/terraform/request_templates.j2` & `coworks-0.9.4a3/coworks/cws/templates/terraform/request_templates.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/templates/terraform/response_templates.j2` & `coworks-0.9.4a3/coworks/cws/templates/terraform/response_templates.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/templates/terraform/rest_api.j2` & `coworks-0.9.4a3/coworks/cws/templates/terraform/rest_api.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/templates/terraform/role.j2` & `coworks-0.9.4a3/coworks/cws/templates/terraform/role.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/cws/utils.py` & `coworks-0.9.4a3/coworks/cws/utils.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/jsonapi/__init__.py` & `coworks-0.9.4a3/coworks/extension/jsonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/jsonapi/data.py` & `coworks-0.9.4a3/coworks/extension/jsonapi/data.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/jsonapi/fetching.py` & `coworks-0.9.4a3/coworks/extension/jsonapi/fetching.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/jsonapi/jsonapi.py` & `coworks-0.9.4a3/coworks/extension/jsonapi/jsonapi.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/jsonapi/query.py` & `coworks-0.9.4a3/coworks/extension/jsonapi/query.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/odoo.py` & `coworks-0.9.4a3/coworks/extension/odoo.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/extension/xray.py` & `coworks-0.9.4a3/coworks/extension/xray.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/tech/directory.py` & `coworks-0.9.4a3/coworks/tech/directory.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/utils.py` & `coworks-0.9.4a3/coworks/utils.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/coworks/wrappers.py` & `coworks-0.9.4a3/coworks/wrappers.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/pyproject.toml` & `coworks-0.9.4a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "coworks"
-version = "0.9.4a2"
+version = "0.9.4a3"
 description = "Coworks is a unified compositional microservices framework using Flask/Airflow on AWS serverless technologies."
 readme = "README.rst"
 requires-python = ">= 3.11"
 authors = [
     { name = "Guillaume Doumenc", email = "gdoumenc@fpr-coworks.com" },
 ]
 keywords = [
@@ -57,35 +57,49 @@
     "aws_xray_sdk>=2.12",
     "boto3-stubs",
     "mypy>=1.5",
     "pytest>=7.4",
     "ruff>=0.0.284",
     "sphinx>=7.1",
     "sqlalchemy>=2.0",
+    "types-Markdown>=3.6.0.20240316",
+    "types-PyYAML>=6.0.12.20240311",
+    "types-requests>=2.31.0.20240406",
 ]
 
 [tool.pdm.scripts.lint]
-cmd = "ruff coworks"
+cmd = "ruff check coworks"
 help = "Linting using Ruff"
 
 [tool.pdm.scripts.typecheck]
 cmd = "mypy coworks"
 help = "Type checking using mypy"
 
 [tool.pdm.scripts.pytest]
 cmd = "pytest"
 help = "Unit testing using pytest"
 
+[tool.pdm.scripts.github_pytest]
+cmd = "pytest -m 'not not_on_github'"
+help = "Unit testing using pytest"
+
 [tool.pdm.scripts.test]
 composite = [
     "lint",
     "typecheck",
     "pytest",
 ]
 
+[tool.pdm.scripts.on_github]
+composite = [
+    "lint",
+    "typecheck",
+    "github_pytest",
+]
+
 [tool.pdm.scripts.plugins]
 shell = "mkdir -p dist; zip -r dist/plugins.zip coworks/operators.py coworks/sensors.py coworks/biz/*"
 
 [tool.pdm.scripts.pre_fury]
 cmd = "pdm build"
 
 [tool.pdm.scripts.fury]
@@ -113,15 +127,15 @@
 overrides = [
     { module = "requests_toolbelt.*", ignore_missing_imports = true },
 ]
 
 [tool.pytest.ini_options]
 markers = [
     "wip",
-    "local",
+    "not_on_github",
 ]
 testpaths = [
     "tests",
 ]
 
 [bdist_wheel]
 universal = 1
```

### Comparing `coworks-0.9.4a2/tests/conftest.py` & `coworks-0.9.4a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/blueprint/blueprint.py` & `coworks-0.9.4a3/tests/coworks/blueprint/blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/blueprint/test_admin.py` & `coworks-0.9.4a3/tests/coworks/blueprint/test_admin.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/blueprint/test_blueprint.py` & `coworks-0.9.4a3/tests/coworks/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/blueprint/test_empty.py` & `coworks-0.9.4a3/tests/coworks/blueprint/test_empty.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/blueprint/test_mail.py` & `coworks-0.9.4a3/tests/coworks/blueprint/test_mail.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/blueprint/test_overload.py` & `coworks-0.9.4a3/tests/coworks/blueprint/test_overload.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/event.py` & `coworks-0.9.4a3/tests/coworks/event.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/ms.py` & `coworks-0.9.4a3/tests/coworks/ms.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/tech/test_async.py` & `coworks-0.9.4a3/tests/coworks/tech/test_async.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/tech/test_auth.py` & `coworks-0.9.4a3/tests/coworks/tech/test_auth.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/tech/test_content_type.py` & `coworks-0.9.4a3/tests/coworks/tech/test_content_type.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/tech/test_event.py` & `coworks-0.9.4a3/tests/coworks/tech/test_event.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/tech/test_ms.py` & `coworks-0.9.4a3/tests/coworks/tech/test_ms.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/coworks/tech/test_type.py` & `coworks-0.9.4a3/tests/coworks/tech/test_type.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/cws/src/app.py` & `coworks-0.9.4a3/tests/cws/src/app.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/cws/src/command.py` & `coworks-0.9.4a3/tests/cws/src/command.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/cws/test_cmd.py` & `coworks-0.9.4a3/tests/cws/test_cmd.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/cws/test_deploy.py` & `coworks-0.9.4a3/tests/cws/test_deploy.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/cws/test_environment.py` & `coworks-0.9.4a3/tests/cws/test_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import multiprocessing
 import os
 import time
 from unittest import mock
 
+import pytest
 import requests
 from flask.cli import ScriptInfo
 
 from coworks.cws.client import client
 from coworks.utils import load_dotenv
 from tests.coworks.event import get_event
 from tests.cws.src.app import EnvTechMS
 
 
+@pytest.mark.not_on_github
 class TestClass:
 
     @mock.patch.dict(os.environ, {"FLASK_ENV_FILE": ".env.no", "FLASK_RUN_FROM_CLI": "true"})
     def test_no_env(self, example_dir, empty_aws_context):
         app = EnvTechMS()
         event = get_event('/', 'get')
         with app.cws_client(event, empty_aws_context) as c:
```

### Comparing `coworks-0.9.4a2/tests/cws/test_project_file.py` & `coworks-0.9.4a3/tests/cws/test_project_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == 0
 
     @mock.patch.dict(os.environ, {"FLASK_APP": "command:app"})
     def test_wrong_project_dir(self, example_dir):
         with pytest.raises(UsageError) as pytest_wrapped_e:
             client.main(['--project-dir', 'doesntexist', 'test'], 'cws', standalone_mode=False)
-        msg = "Project dir /home/gdo/workspace/coworks/tests/cws/src/doesntexist not found."
-        assert pytest_wrapped_e.value.args[0] == msg
+        msg = "tests/cws/src/doesntexist not found."
+        assert pytest_wrapped_e.value.args[0].endswith(msg)
         with pytest.raises(SystemExit) as pytest_wrapped_e:
             client(prog_name='cws', args=['-p', 'doesntexist', 'test'])
 
     def test_wrong_project_config_version(self, example_dir):
         with pytest.raises(RuntimeError) as pytest_wrapped_e:
             client.main(['--project-dir', '.', '--config-file-suffix', '.wrong.yml', 'cmd'], 'cws',
                         standalone_mode=False)
```

### Comparing `coworks-0.9.4a2/tests/docs/test_client.py` & `coworks-0.9.4a3/tests/docs/test_client.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/docs/test_complete.py` & `coworks-0.9.4a3/tests/docs/test_complete.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from unittest import mock
-
 import multiprocessing
 import os
-import requests
 import time
+from unittest import mock
+
+import pytest
+import requests
 
 from coworks.cws.client import CwsScriptInfo
 from coworks.cws.client import import_attr
 
 
+@pytest.mark.not_on_github
 class TestClass:
     @mock.patch.dict(os.environ, {"FLASK_RUN_FROM_CLI": "false"})
     def test_run_complete(self, samples_docs_dir, unused_tcp_port):
         info = CwsScriptInfo(project_dir='tech')
         info.app_import_path = "complete:app"
         app = info.load_app()
         app = import_attr('complete', 'app')
```

### Comparing `coworks-0.9.4a2/tests/docs/test_first.py` & `coworks-0.9.4a3/tests/docs/test_first.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/tests/docs/test_hello.py` & `coworks-0.9.4a3/tests/docs/test_hello.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a2/PKG-INFO` & `coworks-0.9.4a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coworks
-Version: 0.9.4a2
+Version: 0.9.4a3
 Summary: Coworks is a unified compositional microservices framework using Flask/Airflow on AWS serverless technologies.
 Keywords: python3,serverless,microservice,flask,airflow,aws-lambda,aws
 Author-Email: Guillaume Doumenc <gdoumenc@fpr-coworks.com>
 License: MIT License
         
         Copyright (c) 2019 FPR-Coworks
```

