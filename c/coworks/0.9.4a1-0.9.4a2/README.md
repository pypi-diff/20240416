# Comparing `tmp/coworks-0.9.4a1.tar.gz` & `tmp/coworks-0.9.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coworks-0.9.4a1.tar", last modified: Tue Apr 16 08:18:11 2024, max compression
+gzip compressed data, was "coworks-0.9.4a2.tar", last modified: Tue Apr 16 08:27:38 2024, max compression
```

## Comparing `coworks-0.9.4a1.tar` & `coworks-0.9.4a2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1067 2024-04-16 08:17:59.863178 coworks-0.9.4a1/LICENSE.txt
--rw-r--r--   0        0        0       71 2024-04-16 08:17:59.863178 coworks-0.9.4a1/NOTICE
--rw-r--r--   0        0        0     4409 2024-04-16 08:17:59.863178 coworks-0.9.4a1/README.rst
--rw-r--r--   0        0        0      643 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/__init__.py
--rw-r--r--   0        0        0     2539 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/aws.py
--rw-r--r--   0        0        0     1255 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/biz/__init__.py
--rw-r--r--   0        0        0     8002 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/biz/group.py
--rw-r--r--   0        0        0    13362 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/biz/operators.py
--rw-r--r--   0        0        0     1761 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/biz/sensors.py
--rw-r--r--   0        0        0     8400 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/blueprint/admin_blueprint.py
--rw-r--r--   0        0        0     7027 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/blueprint/mail_blueprint.py
--rw-r--r--   0        0        0     3788 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/blueprint/okta_blueprint.py
--rw-r--r--   0        0        0      490 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/blueprint/profiler_blueprint.py
--rw-r--r--   0        0        0      852 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/blueprint/test_blueprint.py
--rw-r--r--   0        0        0    21424 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/coworks.py
--rwxr-xr-x   0        0        0        0 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/cws/__init__.py
--rw-r--r--   0        0        0     8022 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/cws/client.py
--rw-r--r--   0        0        0      708 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/cws/command.py
--rw-r--r--   0        0        0    24102 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/cws/deploy.py
--rw-r--r--   0        0        0      136 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/cws/exception.py
--rw-r--r--   0        0        0     1413 2024-04-16 08:17:59.863178 coworks-0.9.4a1/coworks/cws/new.py
--rw-r--r--   0        0        0     1091 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/project_templates/README.md
--rw-r--r--   0        0        0     1304 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/project_templates/tech/app.py
--rw-r--r--   0        0        0       34 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/project_templates/template.env
--rw-r--r--   0        0        0      300 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/deploy.j2
--rw-r--r--   0        0        0      294 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/project.cws.yml
--rw-r--r--   0        0        0     2038 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform.j2
--rw-r--r--   0        0        0     2954 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/lambda.j2
--rw-r--r--   0        0        0      438 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/local.j2
--rw-r--r--   0        0        0      375 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/output.j2
--rw-r--r--   0        0        0      416 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/provider.j2
--rw-r--r--   0        0        0     3089 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/request_templates.j2
--rw-r--r--   0        0        0     1301 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/response_templates.j2
--rw-r--r--   0        0        0    10271 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/rest_api.j2
--rw-r--r--   0        0        0     2079 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/templates/terraform/role.j2
--rwxr-xr-x   0        0        0     2856 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/cws/utils.py
--rw-r--r--   0        0        0      723 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/jsonapi/__init__.py
--rw-r--r--   0        0        0     3473 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/jsonapi/data.py
--rw-r--r--   0        0        0    12744 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/jsonapi/fetching.py
--rw-r--r--   0        0        0    15584 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/jsonapi/jsonapi.py
--rw-r--r--   0        0        0     1347 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/jsonapi/query.py
--rw-r--r--   0        0        0    10878 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/odoo.py
--rw-r--r--   0        0        0     7704 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/extension/xray.py
--rw-r--r--   0        0        0      166 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/globals.py
--rw-r--r--   0        0        0      217 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/operators.py
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/py.typed
--rw-r--r--   0        0        0      214 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/sensors.py
--rw-r--r--   0        0        0    10633 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/tech/directory.py
--rw-r--r--   0        0        0    12767 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/utils.py
--rw-r--r--   0        0        0      291 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/version.py
--rw-r--r--   0        0        0     8691 2024-04-16 08:17:59.867178 coworks-0.9.4a1/coworks/wrappers.py
--rw-r--r--   0        0        0     2698 2024-04-16 08:18:11.903127 coworks-0.9.4a1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/__init__.py
--rw-r--r--   0        0        0     1380 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/__init__.py
--rw-r--r--   0        0        0      725 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/blueprint.py
--rw-r--r--   0        0        0     3991 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/test_admin.py
--rw-r--r--   0        0        0     2346 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/test_blueprint.py
--rw-r--r--   0        0        0      954 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/test_empty.py
--rw-r--r--   0        0        0     3963 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/test_mail.py
--rw-r--r--   0        0        0      749 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/blueprint/test_overload.py
--rw-r--r--   0        0        0     4461 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/event.py
--rw-r--r--   0        0        0     2214 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/ms.py
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/test_async.py
--rw-r--r--   0        0        0     2452 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/test_auth.py
--rw-r--r--   0        0        0     4318 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/test_content_type.py
--rw-r--r--   0        0        0     8907 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/test_event.py
--rw-r--r--   0        0        0    11915 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/test_ms.py
--rw-r--r--   0        0        0     3714 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/coworks/tech/test_type.py
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/__init__.py
--rw-r--r--   0        0        0       47 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/src/.env.dev
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/src/__init__.py
--rw-r--r--   0        0        0      870 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/src/app.py
--rw-r--r--   0        0        0      916 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/src/command.py
--rw-r--r--   0        0        0      170 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/src/project.cws.yml
--rw-r--r--   0        0        0      294 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/src/project.wrong.yml
--rw-r--r--   0        0        0     2620 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/test_cmd.py
--rw-r--r--   0        0        0     7488 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/test_deploy.py
--rw-r--r--   0        0        0     4128 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/test_environment.py
--rw-r--r--   0        0        0     1464 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/cws/test_project_file.py
--rw-r--r--   0        0        0        0 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/docs/__init__.py
--rw-r--r--   0        0        0      846 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/docs/test_client.py
--rw-r--r--   0        0        0     1313 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/docs/test_complete.py
--rw-r--r--   0        0        0     2791 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/docs/test_first.py
--rw-r--r--   0        0        0     1036 2024-04-16 08:17:59.871178 coworks-0.9.4a1/tests/docs/test_hello.py
--rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 coworks-0.9.4a1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 08:27:23.929345 coworks-0.9.4a2/LICENSE.txt
+-rw-r--r--   0        0        0       71 2024-04-16 08:27:23.933345 coworks-0.9.4a2/NOTICE
+-rw-r--r--   0        0        0     4409 2024-04-16 08:27:23.933345 coworks-0.9.4a2/README.rst
+-rw-r--r--   0        0        0      643 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/__init__.py
+-rw-r--r--   0        0        0     2539 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/aws.py
+-rw-r--r--   0        0        0     1255 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/__init__.py
+-rw-r--r--   0        0        0     8002 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/group.py
+-rw-r--r--   0        0        0    13362 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/operators.py
+-rw-r--r--   0        0        0     1761 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/biz/sensors.py
+-rw-r--r--   0        0        0     8400 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/admin_blueprint.py
+-rw-r--r--   0        0        0     7027 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/mail_blueprint.py
+-rw-r--r--   0        0        0     3788 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/okta_blueprint.py
+-rw-r--r--   0        0        0      490 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/profiler_blueprint.py
+-rw-r--r--   0        0        0      852 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/blueprint/test_blueprint.py
+-rw-r--r--   0        0        0    21424 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/coworks.py
+-rwxr-xr-x   0        0        0        0 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/__init__.py
+-rw-r--r--   0        0        0     8022 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/client.py
+-rw-r--r--   0        0        0      708 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/command.py
+-rw-r--r--   0        0        0    24102 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/deploy.py
+-rw-r--r--   0        0        0      136 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/exception.py
+-rw-r--r--   0        0        0     1413 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/new.py
+-rw-r--r--   0        0        0     1091 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/project_templates/README.md
+-rw-r--r--   0        0        0     1304 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/project_templates/tech/app.py
+-rw-r--r--   0        0        0       34 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/project_templates/template.env
+-rw-r--r--   0        0        0      300 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/deploy.j2
+-rw-r--r--   0        0        0      294 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/project.cws.yml
+-rw-r--r--   0        0        0     2038 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform.j2
+-rw-r--r--   0        0        0     2954 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/lambda.j2
+-rw-r--r--   0        0        0      438 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/local.j2
+-rw-r--r--   0        0        0      375 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/output.j2
+-rw-r--r--   0        0        0      416 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/provider.j2
+-rw-r--r--   0        0        0     3089 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/request_templates.j2
+-rw-r--r--   0        0        0     1301 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/response_templates.j2
+-rw-r--r--   0        0        0    10271 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/rest_api.j2
+-rw-r--r--   0        0        0     2079 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/templates/terraform/role.j2
+-rwxr-xr-x   0        0        0     2856 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/cws/utils.py
+-rw-r--r--   0        0        0      723 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/__init__.py
+-rw-r--r--   0        0        0     3473 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/data.py
+-rw-r--r--   0        0        0    12744 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/fetching.py
+-rw-r--r--   0        0        0    15584 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/jsonapi.py
+-rw-r--r--   0        0        0     1347 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/jsonapi/query.py
+-rw-r--r--   0        0        0    10878 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/odoo.py
+-rw-r--r--   0        0        0     7704 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/extension/xray.py
+-rw-r--r--   0        0        0      166 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/globals.py
+-rw-r--r--   0        0        0      217 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/operators.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/py.typed
+-rw-r--r--   0        0        0      214 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/sensors.py
+-rw-r--r--   0        0        0    10633 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/tech/directory.py
+-rw-r--r--   0        0        0    12827 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/utils.py
+-rw-r--r--   0        0        0      291 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/version.py
+-rw-r--r--   0        0        0     8691 2024-04-16 08:27:23.933345 coworks-0.9.4a2/coworks/wrappers.py
+-rw-r--r--   0        0        0     2698 2024-04-16 08:27:38.449509 coworks-0.9.4a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/__init__.py
+-rw-r--r--   0        0        0     1380 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/blueprint.py
+-rw-r--r--   0        0        0     3991 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_admin.py
+-rw-r--r--   0        0        0     2346 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_blueprint.py
+-rw-r--r--   0        0        0      954 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_empty.py
+-rw-r--r--   0        0        0     3963 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_mail.py
+-rw-r--r--   0        0        0      749 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/blueprint/test_overload.py
+-rw-r--r--   0        0        0     4461 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/event.py
+-rw-r--r--   0        0        0     2214 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/ms.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_async.py
+-rw-r--r--   0        0        0     2452 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_auth.py
+-rw-r--r--   0        0        0     4318 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_content_type.py
+-rw-r--r--   0        0        0     8907 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_event.py
+-rw-r--r--   0        0        0    11915 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_ms.py
+-rw-r--r--   0        0        0     3714 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/coworks/tech/test_type.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/.env.dev
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/app.py
+-rw-r--r--   0        0        0      916 2024-04-16 08:27:23.937345 coworks-0.9.4a2/tests/cws/src/command.py
+-rw-r--r--   0        0        0      170 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/src/project.cws.yml
+-rw-r--r--   0        0        0      294 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/src/project.wrong.yml
+-rw-r--r--   0        0        0     2620 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_cmd.py
+-rw-r--r--   0        0        0     7488 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_deploy.py
+-rw-r--r--   0        0        0     4128 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_environment.py
+-rw-r--r--   0        0        0     1464 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/cws/test_project_file.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_client.py
+-rw-r--r--   0        0        0     1313 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_complete.py
+-rw-r--r--   0        0        0     2791 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_first.py
+-rw-r--r--   0        0        0     1036 2024-04-16 08:27:23.941345 coworks-0.9.4a2/tests/docs/test_hello.py
+-rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 coworks-0.9.4a2/PKG-INFO
```

### Comparing `coworks-0.9.4a1/LICENSE.txt` & `coworks-0.9.4a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/README.rst` & `coworks-0.9.4a2/README.rst`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/__init__.py` & `coworks-0.9.4a2/coworks/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/aws.py` & `coworks-0.9.4a2/coworks/aws.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/biz/__init__.py` & `coworks-0.9.4a2/coworks/biz/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/biz/group.py` & `coworks-0.9.4a2/coworks/biz/group.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/biz/operators.py` & `coworks-0.9.4a2/coworks/biz/operators.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/biz/sensors.py` & `coworks-0.9.4a2/coworks/biz/sensors.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/blueprint/admin_blueprint.py` & `coworks-0.9.4a2/coworks/blueprint/admin_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/blueprint/mail_blueprint.py` & `coworks-0.9.4a2/coworks/blueprint/mail_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/blueprint/okta_blueprint.py` & `coworks-0.9.4a2/coworks/blueprint/okta_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/blueprint/test_blueprint.py` & `coworks-0.9.4a2/coworks/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/coworks.py` & `coworks-0.9.4a2/coworks/coworks.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/client.py` & `coworks-0.9.4a2/coworks/cws/client.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/command.py` & `coworks-0.9.4a2/coworks/cws/command.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/deploy.py` & `coworks-0.9.4a2/coworks/cws/deploy.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/new.py` & `coworks-0.9.4a2/coworks/cws/new.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/project_templates/README.md` & `coworks-0.9.4a2/coworks/cws/project_templates/README.md`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/project_templates/tech/app.py` & `coworks-0.9.4a2/coworks/cws/project_templates/tech/app.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/templates/terraform.j2` & `coworks-0.9.4a2/coworks/cws/templates/terraform.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/templates/terraform/lambda.j2` & `coworks-0.9.4a2/coworks/cws/templates/terraform/lambda.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/templates/terraform/request_templates.j2` & `coworks-0.9.4a2/coworks/cws/templates/terraform/request_templates.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/templates/terraform/response_templates.j2` & `coworks-0.9.4a2/coworks/cws/templates/terraform/response_templates.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/templates/terraform/rest_api.j2` & `coworks-0.9.4a2/coworks/cws/templates/terraform/rest_api.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/templates/terraform/role.j2` & `coworks-0.9.4a2/coworks/cws/templates/terraform/role.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/cws/utils.py` & `coworks-0.9.4a2/coworks/cws/utils.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/jsonapi/__init__.py` & `coworks-0.9.4a2/coworks/extension/jsonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/jsonapi/data.py` & `coworks-0.9.4a2/coworks/extension/jsonapi/data.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/jsonapi/fetching.py` & `coworks-0.9.4a2/coworks/extension/jsonapi/fetching.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/jsonapi/jsonapi.py` & `coworks-0.9.4a2/coworks/extension/jsonapi/jsonapi.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/jsonapi/query.py` & `coworks-0.9.4a2/coworks/extension/jsonapi/query.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/odoo.py` & `coworks-0.9.4a2/coworks/extension/odoo.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/extension/xray.py` & `coworks-0.9.4a2/coworks/extension/xray.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/tech/directory.py` & `coworks-0.9.4a2/coworks/tech/directory.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/coworks/utils.py` & `coworks-0.9.4a2/coworks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import types
 import typing as t
 from functools import update_wrapper
 from inspect import Parameter
 from inspect import Signature
 from inspect import signature
-from pathlib import PosixPath
+from pathlib import PurePosixPath
 from urllib.parse import parse_qs
 from urllib.parse import urlencode
 from urllib.parse import urlsplit as urllib_urlsplit
 from urllib.parse import urlunsplit as urllib_urlunsplit
 
 import dotenv
 from flask import current_app
@@ -110,15 +110,16 @@
             elif request.method in ['POST', 'PUT', 'PATCH', 'DELETE']:
                 try:
                     if request.is_json:
                         if request.data:
                             post_data = request.json
                             if not isinstance(post_data, dict):
                                 if len(func_kwargs) != 1:
-                                    msg = f"If request payload is not a dict, there must be only one kwarg {type(post_data)}"
+                                    msg = ("If request payload is not a dict, "
+                                           f"there must be only one kwarg {type(post_data)}")
                                     raise UnprocessableEntity(msg)
                                 post_data = {next(iter(func_kwargs)): post_data}
                             view_args = {**view_args, **as_fun_params(post_data, False)}
                     elif request.is_multipart:
                         post_data = request.form.to_dict(False)
                         files = request.files.to_dict(False)
                         view_args = {**view_args, **as_fun_params(post_data), **as_fun_params(files)}
@@ -168,21 +169,21 @@
 
 def path_join(*args: str) -> str:
     """ Joins given arguments into an entry route.
     Slashes are stripped for each argument.
     """
 
     reduced = (x.lstrip('/').rstrip('/') for x in args if x)
-    return str(PosixPath('/').joinpath(*reduced))[1:]
+    return str(PurePosixPath('/').joinpath(*reduced))[1:]
 
 
 def make_absolute(route: str, url_prefix: str) -> str:
     """Creates an absolute route.
     """
-    path = PosixPath('/')
+    path = PurePosixPath('/')
     if url_prefix:
         path = path / url_prefix
     if route:
         path = path / route
     return str(path)
```

### Comparing `coworks-0.9.4a1/coworks/wrappers.py` & `coworks-0.9.4a2/coworks/wrappers.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/pyproject.toml` & `coworks-0.9.4a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "coworks"
-version = "0.9.4a1"
+version = "0.9.4a2"
 description = "Coworks is a unified compositional microservices framework using Flask/Airflow on AWS serverless technologies."
 readme = "README.rst"
 requires-python = ">= 3.11"
 authors = [
     { name = "Guillaume Doumenc", email = "gdoumenc@fpr-coworks.com" },
 ]
 keywords = [
```

### Comparing `coworks-0.9.4a1/tests/conftest.py` & `coworks-0.9.4a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/blueprint/blueprint.py` & `coworks-0.9.4a2/tests/coworks/blueprint/blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/blueprint/test_admin.py` & `coworks-0.9.4a2/tests/coworks/blueprint/test_admin.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/blueprint/test_blueprint.py` & `coworks-0.9.4a2/tests/coworks/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/blueprint/test_empty.py` & `coworks-0.9.4a2/tests/coworks/blueprint/test_empty.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/blueprint/test_mail.py` & `coworks-0.9.4a2/tests/coworks/blueprint/test_mail.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/blueprint/test_overload.py` & `coworks-0.9.4a2/tests/coworks/blueprint/test_overload.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/event.py` & `coworks-0.9.4a2/tests/coworks/event.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/ms.py` & `coworks-0.9.4a2/tests/coworks/ms.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/tech/test_async.py` & `coworks-0.9.4a2/tests/coworks/tech/test_async.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/tech/test_auth.py` & `coworks-0.9.4a2/tests/coworks/tech/test_auth.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/tech/test_content_type.py` & `coworks-0.9.4a2/tests/coworks/tech/test_content_type.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/tech/test_event.py` & `coworks-0.9.4a2/tests/coworks/tech/test_event.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/tech/test_ms.py` & `coworks-0.9.4a2/tests/coworks/tech/test_ms.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/coworks/tech/test_type.py` & `coworks-0.9.4a2/tests/coworks/tech/test_type.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/cws/src/app.py` & `coworks-0.9.4a2/tests/cws/src/app.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/cws/src/command.py` & `coworks-0.9.4a2/tests/cws/src/command.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/cws/test_cmd.py` & `coworks-0.9.4a2/tests/cws/test_cmd.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/cws/test_deploy.py` & `coworks-0.9.4a2/tests/cws/test_deploy.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/cws/test_environment.py` & `coworks-0.9.4a2/tests/cws/test_environment.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/cws/test_project_file.py` & `coworks-0.9.4a2/tests/cws/test_project_file.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/docs/test_client.py` & `coworks-0.9.4a2/tests/docs/test_client.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/docs/test_complete.py` & `coworks-0.9.4a2/tests/docs/test_complete.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/docs/test_first.py` & `coworks-0.9.4a2/tests/docs/test_first.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/tests/docs/test_hello.py` & `coworks-0.9.4a2/tests/docs/test_hello.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.4a1/PKG-INFO` & `coworks-0.9.4a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coworks
-Version: 0.9.4a1
+Version: 0.9.4a2
 Summary: Coworks is a unified compositional microservices framework using Flask/Airflow on AWS serverless technologies.
 Keywords: python3,serverless,microservice,flask,airflow,aws-lambda,aws
 Author-Email: Guillaume Doumenc <gdoumenc@fpr-coworks.com>
 License: MIT License
         
         Copyright (c) 2019 FPR-Coworks
```

