# Comparing `tmp/coworks-0.9.2.tar.gz` & `tmp/coworks-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coworks-0.9.2.tar", last modified: Tue Dec 19 10:25:00 2023, max compression
+gzip compressed data, was "coworks-0.9.3.tar", last modified: Tue Apr 16 07:11:34 2024, max compression
```

## Comparing `coworks-0.9.2.tar` & `coworks-0.9.3.tar`

### file list

```diff
@@ -1,85 +1,88 @@
--rw-r--r--   0        0        0     1067 2023-12-19 10:24:48.663092 coworks-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0       71 2023-12-19 10:24:48.663092 coworks-0.9.2/NOTICE
--rw-r--r--   0        0        0     4409 2023-12-19 10:24:48.663092 coworks-0.9.2/README.rst
--rw-r--r--   0        0        0      643 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/__init__.py
--rw-r--r--   0        0        0     2539 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/aws.py
--rw-r--r--   0        0        0     1255 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/biz/__init__.py
--rw-r--r--   0        0        0     8002 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/biz/group.py
--rw-r--r--   0        0        0    12849 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/biz/operators.py
--rw-r--r--   0        0        0     1761 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/biz/sensors.py
--rw-r--r--   0        0        0     8948 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/blueprint/admin_blueprint.py
--rw-r--r--   0        0        0     5033 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/blueprint/gsheets_blueprint.py
--rw-r--r--   0        0        0     7027 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/blueprint/mail_blueprint.py
--rw-r--r--   0        0        0     3761 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/blueprint/okta_blueprint.py
--rw-r--r--   0        0        0      490 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/blueprint/profiler_blueprint.py
--rw-r--r--   0        0        0      852 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/blueprint/test_blueprint.py
--rw-r--r--   0        0        0    21113 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/coworks.py
--rwxr-xr-x   0        0        0        0 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/__init__.py
--rw-r--r--   0        0        0     8013 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/client.py
--rw-r--r--   0        0        0      706 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/command.py
--rw-r--r--   0        0        0    23835 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/deploy.py
--rw-r--r--   0        0        0      136 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/exception.py
--rw-r--r--   0        0        0     1413 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/new.py
--rw-r--r--   0        0        0     1091 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/project_templates/README.md
--rw-r--r--   0        0        0     1333 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/project_templates/tech/app.py
--rw-r--r--   0        0        0       34 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/project_templates/template.env
--rw-r--r--   0        0        0      300 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/deploy.j2
--rw-r--r--   0        0        0      294 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/project.cws.yml
--rw-r--r--   0        0        0     2037 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform.j2
--rw-r--r--   0        0        0     2990 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/lambda.j2
--rw-r--r--   0        0        0      438 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/local.j2
--rw-r--r--   0        0        0      371 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/output.j2
--rw-r--r--   0        0        0      416 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/provider.j2
--rw-r--r--   0        0        0     3089 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/request_templates.j2
--rw-r--r--   0        0        0     1301 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/response_templates.j2
--rw-r--r--   0        0        0    10279 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/rest_api.j2
--rw-r--r--   0        0        0     2071 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/templates/terraform/role.j2
--rwxr-xr-x   0        0        0     2803 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/cws/utils.py
--rw-r--r--   0        0        0    19503 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/extension/jsonapi.py
--rw-r--r--   0        0        0     8882 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/extension/odoo.py
--rw-r--r--   0        0        0     7571 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/extension/xray.py
--rw-r--r--   0        0        0      166 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/globals.py
--rw-r--r--   0        0        0      217 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/operators.py
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/py.typed
--rw-r--r--   0        0        0      214 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/sensors.py
--rw-r--r--   0        0        0    10633 2023-12-19 10:24:48.663092 coworks-0.9.2/coworks/tech/directory.py
--rw-r--r--   0        0        0    12602 2023-12-19 10:24:48.667092 coworks-0.9.2/coworks/utils.py
--rw-r--r--   0        0        0      127 2023-12-19 10:24:48.667092 coworks-0.9.2/coworks/version.py
--rw-r--r--   0        0        0     8698 2023-12-19 10:24:48.667092 coworks-0.9.2/coworks/wrappers.py
--rw-r--r--   0        0        0     2527 2023-12-19 10:25:00.235114 coworks-0.9.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     1380 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/__init__.py
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/__init__.py
--rw-r--r--   0        0        0      725 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/blueprint.py
--rw-r--r--   0        0        0     3991 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/test_admin.py
--rw-r--r--   0        0        0     2346 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/test_blueprint.py
--rw-r--r--   0        0        0      954 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/test_empty.py
--rw-r--r--   0        0        0     3963 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/test_mail.py
--rw-r--r--   0        0        0      749 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/blueprint/test_overload.py
--rw-r--r--   0        0        0     4461 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/event.py
--rw-r--r--   0        0        0     2214 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/ms.py
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/__init__.py
--rw-r--r--   0        0        0     1168 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/test_async.py
--rw-r--r--   0        0        0     2452 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/test_auth.py
--rw-r--r--   0        0        0     4318 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/test_content_type.py
--rw-r--r--   0        0        0     8907 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/test_event.py
--rw-r--r--   0        0        0    11915 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/test_ms.py
--rw-r--r--   0        0        0     3716 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/coworks/tech/test_type.py
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/__init__.py
--rw-r--r--   0        0        0       47 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/src/.env.dev
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/src/__init__.py
--rw-r--r--   0        0        0     1016 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/src/app.py
--rw-r--r--   0        0        0      916 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/src/command.py
--rw-r--r--   0        0        0      170 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/src/project.cws.yml
--rw-r--r--   0        0        0      294 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/src/project.wrong.yml
--rw-r--r--   0        0        0     2627 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/test_cmd.py
--rw-r--r--   0        0        0     7430 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/test_deploy.py
--rw-r--r--   0        0        0     4349 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/test_environment.py
--rw-r--r--   0        0        0     1464 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/cws/test_project_file.py
--rw-r--r--   0        0        0        0 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/docs/__init__.py
--rw-r--r--   0        0        0      846 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/docs/test_client.py
--rw-r--r--   0        0        0     1313 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/docs/test_complete.py
--rw-r--r--   0        0        0     2791 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/docs/test_first.py
--rw-r--r--   0        0        0     1036 2023-12-19 10:24:48.671092 coworks-0.9.2/tests/docs/test_hello.py
--rw-r--r--   0        0        0     6733 1970-01-01 00:00:00.000000 coworks-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 07:11:22.630195 coworks-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0       71 2024-04-16 07:11:22.630195 coworks-0.9.3/NOTICE
+-rw-r--r--   0        0        0     4409 2024-04-16 07:11:22.630195 coworks-0.9.3/README.rst
+-rw-r--r--   0        0        0      643 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/__init__.py
+-rw-r--r--   0        0        0     2539 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/aws.py
+-rw-r--r--   0        0        0     1255 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/biz/__init__.py
+-rw-r--r--   0        0        0     8002 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/biz/group.py
+-rw-r--r--   0        0        0    13362 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/biz/operators.py
+-rw-r--r--   0        0        0     1761 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/biz/sensors.py
+-rw-r--r--   0        0        0     8400 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/blueprint/admin_blueprint.py
+-rw-r--r--   0        0        0     7027 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/blueprint/mail_blueprint.py
+-rw-r--r--   0        0        0     3788 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/blueprint/okta_blueprint.py
+-rw-r--r--   0        0        0      490 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/blueprint/profiler_blueprint.py
+-rw-r--r--   0        0        0      852 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/blueprint/test_blueprint.py
+-rw-r--r--   0        0        0    21424 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/coworks.py
+-rwxr-xr-x   0        0        0        0 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/__init__.py
+-rw-r--r--   0        0        0     8022 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/client.py
+-rw-r--r--   0        0        0      708 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/command.py
+-rw-r--r--   0        0        0    24102 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/deploy.py
+-rw-r--r--   0        0        0      136 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/exception.py
+-rw-r--r--   0        0        0     1413 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/new.py
+-rw-r--r--   0        0        0     1091 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/project_templates/README.md
+-rw-r--r--   0        0        0     1304 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/project_templates/tech/app.py
+-rw-r--r--   0        0        0       34 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/project_templates/template.env
+-rw-r--r--   0        0        0      300 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/deploy.j2
+-rw-r--r--   0        0        0      294 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/project.cws.yml
+-rw-r--r--   0        0        0     2038 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform.j2
+-rw-r--r--   0        0        0     2954 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/lambda.j2
+-rw-r--r--   0        0        0      438 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/local.j2
+-rw-r--r--   0        0        0      375 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/output.j2
+-rw-r--r--   0        0        0      416 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/provider.j2
+-rw-r--r--   0        0        0     3089 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/request_templates.j2
+-rw-r--r--   0        0        0     1301 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/response_templates.j2
+-rw-r--r--   0        0        0    10271 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/rest_api.j2
+-rw-r--r--   0        0        0     2079 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/templates/terraform/role.j2
+-rwxr-xr-x   0        0        0     2856 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/cws/utils.py
+-rw-r--r--   0        0        0      723 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/jsonapi/__init__.py
+-rw-r--r--   0        0        0     3473 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/jsonapi/data.py
+-rw-r--r--   0        0        0    12744 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/jsonapi/fetching.py
+-rw-r--r--   0        0        0    15584 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/jsonapi/jsonapi.py
+-rw-r--r--   0        0        0     1347 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/jsonapi/query.py
+-rw-r--r--   0        0        0    10878 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/odoo.py
+-rw-r--r--   0        0        0     7704 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/extension/xray.py
+-rw-r--r--   0        0        0      166 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/globals.py
+-rw-r--r--   0        0        0      217 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/operators.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/py.typed
+-rw-r--r--   0        0        0      214 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/sensors.py
+-rw-r--r--   0        0        0    10633 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/tech/directory.py
+-rw-r--r--   0        0        0    12752 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/utils.py
+-rw-r--r--   0        0        0      291 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/version.py
+-rw-r--r--   0        0        0     8691 2024-04-16 07:11:22.630195 coworks-0.9.3/coworks/wrappers.py
+-rw-r--r--   0        0        0     2696 2024-04-16 07:11:34.758216 coworks-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.634195 coworks-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     1380 2024-04-16 07:11:22.634195 coworks-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.634195 coworks-0.9.3/tests/coworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.634195 coworks-0.9.3/tests/coworks/blueprint/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-16 07:11:22.634195 coworks-0.9.3/tests/coworks/blueprint/blueprint.py
+-rw-r--r--   0        0        0     3991 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/blueprint/test_admin.py
+-rw-r--r--   0        0        0     2346 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/blueprint/test_blueprint.py
+-rw-r--r--   0        0        0      954 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/blueprint/test_empty.py
+-rw-r--r--   0        0        0     3963 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/blueprint/test_mail.py
+-rw-r--r--   0        0        0      749 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/blueprint/test_overload.py
+-rw-r--r--   0        0        0     4461 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/event.py
+-rw-r--r--   0        0        0     2214 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/ms.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/test_async.py
+-rw-r--r--   0        0        0     2452 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/test_auth.py
+-rw-r--r--   0        0        0     4318 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/test_content_type.py
+-rw-r--r--   0        0        0     8907 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/test_event.py
+-rw-r--r--   0        0        0    11915 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/test_ms.py
+-rw-r--r--   0        0        0     3714 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/coworks/tech/test_type.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/src/.env.dev
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/src/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/src/app.py
+-rw-r--r--   0        0        0      916 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/src/command.py
+-rw-r--r--   0        0        0      170 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/src/project.cws.yml
+-rw-r--r--   0        0        0      294 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/src/project.wrong.yml
+-rw-r--r--   0        0        0     2620 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/test_cmd.py
+-rw-r--r--   0        0        0     7488 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/test_deploy.py
+-rw-r--r--   0        0        0     4128 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/test_environment.py
+-rw-r--r--   0        0        0     1464 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/cws/test_project_file.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/docs/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/docs/test_client.py
+-rw-r--r--   0        0        0     1313 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/docs/test_complete.py
+-rw-r--r--   0        0        0     2791 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/docs/test_first.py
+-rw-r--r--   0        0        0     1036 2024-04-16 07:11:22.638195 coworks-0.9.3/tests/docs/test_hello.py
+-rw-r--r--   0        0        0     6733 1970-01-01 00:00:00.000000 coworks-0.9.3/PKG-INFO
```

### Comparing `coworks-0.9.2/LICENSE.txt` & `coworks-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/README.rst` & `coworks-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/__init__.py` & `coworks-0.9.3/coworks/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/aws.py` & `coworks-0.9.3/coworks/aws.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/biz/__init__.py` & `coworks-0.9.3/coworks/biz/__init__.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/biz/group.py` & `coworks-0.9.3/coworks/biz/group.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/biz/operators.py` & `coworks-0.9.3/coworks/biz/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import base64
 import typing as t
 from json import JSONDecodeError
 from json import loads
 
 import requests
 from airflow.exceptions import AirflowFailException
+from airflow.models import Variable
 from airflow.models.baseoperator import BaseOperator
 from airflow.operators.branch import BaseBranchOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.http.hooks.http import HttpHook
 
 XCOM_DEFAULT_KEY = 'return_value'
 XCOM_CWS_BUCKET = 'bucket'  # the AWS S3 bucket where the coworks techmicroservice result is stored
 XCOM_CWS_KEY = 'key'  # the AWS S3 key where the coworks techmicroservice result is stored
 XCOM_CWS_NAME = 'cws_name'
 XCOM_STATUS_CODE = 'status_code'
 
 
 class TechMicroServiceOperator(BaseOperator):
-    template_fields = ["cws_name", "entry", "query_params", "json", "data"]
+    template_fields = ["cws_name", "headers", "entry", "query_params", "json", "data"]
 
     def __init__(self, *, cws_name: str = None, entry: str = '/', method: str = 'get', no_auth: bool = False,
                  query_params: t.Union[dict, str] = None, json: t.Union[dict, str] = None,
                  data: t.Union[dict, str] = None,
                  stage: str = None, api_id: str = None, token: str = None,
                  raise_errors: bool = True, raise_400_errors: bool = True,
                  accept: str = 'application/json', headers: dict = None, log_response: bool = False,
@@ -46,15 +47,15 @@
         :param directory_conn_id: connection defined for the directory service (default 'coworks_directory').
         :param asynchronous: asynchronous call (default False).
         :param xcom_push: pushes result in XCom (default True).
         :param json_result: returns a JSON value in 'return_value' (default True).
         :param raise_errors: raise error on client errors (default True).
         :param raise_400_errors: raise error on client 400 errors (default True).
         :param accept: accept header value (default 'application/json').
-        :param headers: specific header values forced (default {}).
+        :param headers: specific header values added to default ones and may override them (default {}).
         :param log_response: trace result content (default False).
         :param multiple_outputs_transformer: if defined, return a multi-output XCOM after tranformation.
 
          .. versionchanged:: 0.8.4
             Added the ``multiple_outputs_transformer`` parameter.
         """
         super().__init__(**kwargs)
@@ -72,21 +73,17 @@
         self.directory_conn_id = directory_conn_id
         self.asynchronous = asynchronous
         self.xcom_push_flag = xcom_push
         self.json_result = json_result
         self.raise_errors = raise_errors
         self.raise_400_errors = raise_400_errors
         self.multiple_outputs_transformer = multiple_outputs_transformer
-        self._accept = accept
-        self._url = self._bucket = self._key = self._headers = None
-
-        # Creates header
-        self._headers = self.headers
-        if headers:
-            self._headers.update(headers)
+        self.accept = accept
+        self.headers = headers
+        self._url = self._bucket = self._key = self.__headers = None
 
     def pre_execute(self, context):
         """Gets url and token from name or parameters.
 
         Done only before execution not on DAG loading.
         """
         dag_run = context['dag_run']
@@ -138,21 +135,29 @@
 
     @property
     def url(self):
         """Default url construction."""
         return f'https://{self.api_id}.execute-api.eu-west-1.amazonaws.com/{self.stage}/{self.entry}'
 
     @property
-    def headers(self):
+    def default_headers(self):
         """Default headers values."""
         return {
             'Content-Type': "application/json",
-            'Accept': self._accept,
+            'Accept': self.accept,
         }
 
+    @property
+    def _headers(self):
+        if self.__headers is None:
+            self.__headers = self.default_headers
+            if self.headers:
+                self.__headers.update(self.headers)
+        return self.__headers
+
     def _call_cws(self, context):
         """Method used by operator and sensor."""
         self.log.info(f"Calling {self.method.upper()} method to {self._url}")
         resp = requests.request(
             self.method.upper(), self._url, headers=self._headers,
             params=self.query_params, json=self.json, data=self.data
         )
@@ -271,24 +276,31 @@
             text = int(context['ti'].xcom_pull(task_ids=self.cws_task_id))
             if self.response_check(text):
                 return self.on_check
         return self.on_success
 
 
 class NeoRezoServiceOperator(TechMicroServiceOperator):
+    """This operator is defined as an example of how to use TechMicroServiceOperator.
+
+     This model used JSONAPI extension."""
 
     def __init__(self, *, module: str = None, service: str = None, accept: str = 'application/vnd.api+json', **kwargs):
         super().__init__(accept=accept, **kwargs)
-        self._module = module
-        self._service = service
+        self.module = module
+        self.service = service
 
     @property
     def url(self):
-        return f'https://jsonapi.neorezo.io/{self._module}/{self._service}/{self.entry}'
+        path = f"{self.module}/{self.service}/{self.entry}"
+        if self.stage == 'dev':
+            return f'https://dev.jsonapi.neorezo.io/{path}'
+        return f'https://jsonapi.neorezo.io/{path}'
 
     @property
-    def headers(self):
+    def default_headers(self):
+        nr_jwt = Variable.get("BIZ_NR_JWT")
         return {
             'Content-Type': "application/json",
-            'Accept': self._accept,
-            'X-JSONAPI-TOKEN': "notdefined"
+            'Accept': self.accept,
+            'X-NR-JWT': nr_jwt
         }
```

### Comparing `coworks-0.9.2/coworks/biz/sensors.py` & `coworks-0.9.3/coworks/biz/sensors.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/blueprint/admin_blueprint.py` & `coworks-0.9.3/coworks/blueprint/admin_blueprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import markdown
 from flask import abort
 from flask import current_app
 from flask import render_template_string
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
-from jsonapi_pydantic.v1_0 import TopLevel, Resource
+from jsonapi_pydantic.v1_0 import Resource
+from jsonapi_pydantic.v1_0 import TopLevel
 from pydantic import BaseModel
 from werkzeug.exceptions import NotFound
 
 from coworks import Blueprint
 from coworks import entry
 from coworks.utils import get_cws_annotations
 
 
 class Admin(Blueprint):
     """Administration blueprint to get details on the microservice containing it.
     """
 
-    def __init__(self, name: str = 'admin', models: t.Optional[t.List[t.Type[BaseModel]]] = None, **kwargs):
+    def __init__(self, name: str = 'admin', models: t.Optional[list[type[BaseModel]]] = None, **kwargs):
         super().__init__(name=name, **kwargs)
         self.models = {model.__name__: model for model in models} if models else {}
 
     @entry(no_auth=True, no_cors=True)
     def get(self):
         """Returns the markdown documentation associated to this microservice.
         """
@@ -47,29 +48,14 @@
         headers = {
             "Content-Type": 'text/html; charset=utf-8'
         }
         content = self.header_template + '<hr/>' + content + '<hr/>' + bottom + '\n'
         return content, 200, headers
 
     @entry(no_auth=True, no_cors=True)
-    def get_schema(self, included: bool = False):
-        """Returns the list of schemas defined in the microservices.
-        """
-        id = current_app.name
-        schemas = [model for model in self.models]
-        attributes = {"schemas": schemas}
-        if included:
-            included = [Resource(id=name, type="JsonApiSchema", attributes={"schema": model.schema()})
-                        for name, model in self.models.items()]
-        else:
-            included = []
-        return TopLevel(data=Resource(id=id, type="JsonApiSchemas", attributes=attributes),
-                        included=included).model_dump_json()
-
-    @entry(no_auth=True, no_cors=True)
     # @jsonapi(type)
     def get__schema(self, model):
         """Returns the JSON schemas of the model.
 
         :param model: Model's name.
        """
         if model in self.models:
@@ -84,15 +70,15 @@
 
         :param prefix: Prefix path to limit the number of returned routes.
         :param blueprint: Show named blueprint routes if defined ('__all__' or blueprint name).
         """
         if blueprint and (blueprint != '__all__' and blueprint not in current_app.blueprints):
             raise NotFound(f"Undefined blueprint {blueprint}")
 
-        routes = defaultdict(dict)
+        routes: dict[str, dict[str, str]] = defaultdict(dict)
 
         for rule in current_app.url_map.iter_rules():
 
             # Must return only prefixed routes
             if prefix:
                 if rule.rule.startswith(prefix):
                     self.add_route_from_rule(routes, rule)
@@ -154,70 +140,70 @@
                     if len(docstring) > 1:
                         # noinspection PyTypeChecker
                         route[http_method]['params'] = docstring[1:]
 
         routes[rule.rule].update(route)
 
     @property
-    def header_template(self):
+    def header_template(self) -> str:
         deployed = os.getenv("CWS_DATETIME", None)
         description = current_app.name
         if deployed:
             lambda_name = os.getenv("CWS_LAMBDA", description)
             description = f"{lambda_name} deployed {deployed}"
         return dedent(f"""<div style=\"display:flex;justify-content:space-between;\">
             <span style=\"font-size:xx-large;font-weight:bold\">{current_app.__class__.__name__}</span>
             <img style=\"margin-bottom:auto;width:100px;\"
             src=\"https://github.com/gdoumenc/coworks/raw/dev/docs/img/coworks.png\"/>
             </div><div style=\"display:flex;flex-direction:row-reverse;font-size:small;margin-top:5px;\">
             {description}</div>""")
 
     @property
-    def routes_template(self):
+    def routes_template(self) -> str:
         return dedent(
             """<style type="text/css">ul.nobull {list-style-type: none;}</style>
             <ul class="nobull">{% for entry,route in routes.items() %}
                 <li>{{ entry }} : <ul>{% for method,info in route.items() %}
                     <li><i>{{ method }}{{ info.signature }}[endpoint: {{info.endpoint}}]</i> : {{ info.doc }}
                     <ul class="nobull">{% for param in info.params %}<li><i>{{ param }}</i>{% endfor %}</ul>
                 {% endfor %}</li></ul></li>
             {% endfor %}</ul>"""
         )
 
 
-def get_signature(func):
+def get_signature(func: t.Callable) -> str:
     sig = ""
     params = inspect.signature(func).parameters
     for i, (k, p) in enumerate(params.items()):
         if i == 0:
             continue
         sp = k
         if p.annotation != Parameter.empty:
             sp = f"{sp}:{str(p.annotation)}"
         if p.default != Parameter.empty:
             sp = f"{sp}={p.default}"
         sig = f"{sp}" if i == 1 else f"{sig}, {sp}"
     return f"({sig})"
 
 
-def positional_params(func):
+def positional_params(func: t.Callable) -> str:
     res = ''
     params = inspect.signature(func).parameters
     for i, (k, p) in enumerate(params.items()):
         if i == 0 or p.kind not in [Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD,
                                     Parameter.VAR_POSITIONAL]:
             continue
         if p.kind == Parameter.POSITIONAL_OR_KEYWORD and p.default != Parameter.empty:
             continue
         sp = f"'{k}' : {k}"
         res = f"{sp}" if i == 1 else f"{res}, {sp}"
     return res
 
 
-def keyword_params(func):
+def keyword_params(func: t.Callable) -> str:
     res = ''
     params = inspect.signature(func).parameters
     for i, (k, p) in enumerate(params.items()):
         if i == 0 or p.kind not in [Parameter.KEYWORD_ONLY, Parameter.POSITIONAL_OR_KEYWORD, Parameter.VAR_KEYWORD]:
             continue
         if p.kind == Parameter.POSITIONAL_OR_KEYWORD and p.default == Parameter.empty:
             continue
```

### Comparing `coworks-0.9.2/coworks/blueprint/mail_blueprint.py` & `coworks-0.9.3/coworks/blueprint/mail_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/blueprint/okta_blueprint.py` & `coworks-0.9.3/coworks/blueprint/okta_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 from aws_xray_sdk.core import xray_recorder
-from coworks.extension.xray import XRay
 from flask import request
 from okta.client import Client
 from okta.okta_object import OktaObject
 from werkzeug.exceptions import InternalServerError
 
 from coworks import Blueprint
 from coworks import entry
+from coworks.extension.xray import XRay
 
 
 class OktaClient(Client):
     """Okta client extended to allow next call event on new client defined."""
 
     @XRay.capture(xray_recorder)
     async def next(self, next):
@@ -61,15 +61,15 @@
 
         # noinspection PyProtectedMember
         self.next_url = self.api_resp._next if self.api_resp else None
 
     @property
     def body(self):
         """Get OKTA body response."""
-        return self.api_resp.get_body()
+        return self.api_resp.get_body() if self.api_resp else None
 
     @property
     def response(self):
         """Cast the Okta response as microservice response."""
         if self.error:
             return self.error.message, self.error.status
         return {'value': self.body, 'next': self.next_url}
```

### Comparing `coworks-0.9.2/coworks/blueprint/test_blueprint.py` & `coworks-0.9.3/coworks/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/coworks.py` & `coworks-0.9.3/coworks/coworks.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,36 @@
 from .utils import BIZ_KEY_HEADER_KEY
 from .utils import HTTP_METHODS
 from .utils import create_cws_proxy
 from .utils import get_app_stage
 from .utils import get_cws_annotations
 from .utils import is_arg_parameter
 from .utils import is_kwarg_parameter
-from .utils import load_dotenv
 from .utils import make_absolute
 from .utils import path_join
 from .utils import trim_underscores
 from .wrappers import CoworksMapAdapter
 from .wrappers import CoworksRequest
 from .wrappers import CoworksResponse
 from .wrappers import TokenResponse
 
+if t.TYPE_CHECKING:  # pragma: no cover
+    from _typeshed.wsgi import StartResponse
+    from _typeshed.wsgi import WSGIEnvironment
+else:
+    WSGIEnvironment = t.Any
+    StartResponse = t.Any
+
 
 #
 # Decorators
 #
 
 
-def entry(fun: t.Callable | None = None, binary_headers: t.Dict[str, str] | None = None,
+def entry(fun: t.Callable | None = None, binary_headers: dict[str, str] | None = None,
           stage: str | t.Iterable[str] | None = None,
           no_auth: bool = False, no_cors: bool = True) -> t.Callable:
     """Decorator to create a microservice entry point from function name.
 
     :param fun: the entry function.
     :param binary_headers: force default content-type.
     :param stage: entry defined only for this stage(s).
@@ -168,15 +174,16 @@
         """.. deprecated:: 0.8.0"""
         ...
 
     @property
     def logger(self) -> logging.Logger:
         return current_app.logger
 
-    def make_setup_state(self, app: "TechMicroService", options: t.Dict, *args) -> BlueprintSetupState:
+    def make_setup_state(self, app: "TechMicroService",  # type: ignore[override]
+                         options: dict, *args) -> BlueprintSetupState:
         """Stores creation state for deferred initialization."""
         state = super().make_setup_state(app, options, *args)
 
         # Defer blueprint route initialization.
         if not options.get('hide_routes', False):
             func = partial(TechMicroService.add_coworks_routes, state.app, state)
             app.deferred_init_routes_functions = itertools.chain(app.deferred_init_routes_functions, (func,))
@@ -198,32 +205,28 @@
 
     def __init__(self, name: str | None = None, stage_prefixed: bool = True, **kwargs) -> None:
         """ Initialize a technical microservice.
         :param name: Name used to identify the microservice.
         :param stage_prefixed: if accessed with stage or not.
         :param kwargs: Other Flask parameters.
         """
-        stage = get_app_stage()
-        load_dotenv(stage)
-
         self.default_config = ImmutableDict({
             **self.default_config,
-            "FLASK_SKIP_DOTENV": True,
         })
 
         name = name or self.__class__.__name__.lower()
         super().__init__(import_name=name, static_folder=None, **kwargs)
 
-        self.request_class: t.Type[CoworksRequest] = CoworksRequest
-        self.response_class: t.Type[CoworksResponse] = CoworksResponse
+        self.request_class: type[CoworksRequest] = CoworksRequest
+        self.response_class: type[CoworksResponse] = CoworksResponse
 
         self.deferred_init_routes_functions: t.Iterable[t.Callable] = []
         self._cws_app_initialized = False
         self._cws_conf_updated = False
-        self.__aws_url_map = None
+        self.__aws_url_map: dict | None = None
         self.__stage_prefixed = stage_prefixed
 
         @self.before_request
         def before():
             self._check_token()
 
     def init_app(self):
@@ -242,64 +245,67 @@
 
     def app_context(self):
         """Override to initialize coworks microservice.
         """
         self._init_app(False)
         return super().app_context()
 
-    def create_url_adapter(self, _request: t.Optional[CoworksRequest]):
+    def create_url_adapter(self, _request: CoworksRequest | None):  # type: ignore[override]
         if _request and _request.aws_event:
             self.subdomain_matching = True
             return CoworksMapAdapter(_request.environ, self.url_map, self.aws_url_map, self.__stage_prefixed)
         return super().create_url_adapter(_request)
 
     def cws_client(self, aws_event, aws_context):
         """CoWorks client used by the lambda call.
         """
         return CoworksClient(self, CoworksResponse, use_cookies=True, aws_event=aws_event, aws_context=aws_context)
 
     @property
-    def autorizer_identity_source(self):
+    def header_autorizer_token(self):
         """The identity source for which authorization is requested usefull only on local.
         Usually defined in API GAateway Authorizer resource."""
         return request.headers.get('Authorization')
 
     @property
     def in_lambda_context(self):
         """Defined as a property to be read only."""
         return self._in_lambda_context
 
     @property
-    def aws_url_map(self) -> t.Dict[str, t.List[Rule]]:
+    def aws_url_map(self) -> dict[str, list[Rule]]:
         if self.__aws_url_map is None:
             self.__aws_url_map = {}
             for rule in self.url_map.iter_rules():
                 entry_path = rule.rule.replace('<', '{').replace('>', '}')
                 if entry_path in self.__aws_url_map:
                     self.__aws_url_map[entry_path].append(rule)
                 else:
                     self.__aws_url_map[entry_path] = [rule]
         return self.__aws_url_map
 
     @property
-    def routes(self) -> t.List[str]:
+    def routes(self) -> list[str]:
         """Returns the list of routes defined in the microservice.
         """
         return [k for k in self.aws_url_map]
 
-    def token_authorizer(self, token: str) -> t.Union[bool, str]:
+    def token_authorizer(self, token: str) -> bool | str:
         """Defined the authorization process.
 
         If the returned value is False, all routes for all stages are denied.
         If the returned value is True, all routes for all stages are accepted.
         If the returned value is a string, then it must be a stage name and all routes are accepted for this stage.
 
         By default, just using the token authentification process (defined from terraform template).
         """
 
+        if token is None:
+            raise Unauthorized(www_authenticate=WWWAuthenticate(auth_type="basic"))
+
         return token == os.getenv('TOKEN')
 
     def auto_find_instance_path(self):
         """Instance path may be redefined by an environment variable.
         """
         instance_relative_path = os.getenv('INSTANCE_RELATIVE_PATH', '')
         path = Path(self.root_path) / instance_relative_path
@@ -352,36 +358,36 @@
         if in_flask:
             res = self._flask_handler(arg1, arg2)
         else:
             res = self._lambda_handler(arg1, arg2)
 
         return res
 
-    def _lambda_handler(self, event: t.Dict[str, t.Any], context: t.Dict[str, t.Any]):
+    def _lambda_handler(self, event: dict[str, t.Any], context: dict[str, t.Any]):
         """Lambda handler.
         """
         if event.get('type') == 'TOKEN':
             return self._token_handler(event, context)
         return self._api_handler(event, context)
 
-    def _token_handler(self, aws_event: t.Dict[str, t.Any], aws_context: t.Dict[str, t.Any]) -> dict:
+    def _token_handler(self, aws_event: dict[str, t.Any], aws_context: dict[str, t.Any]) -> dict:
         """Authorization token handler.
         """
         self.logger.warning(f"Calling {self.name} for authorization : {aws_event}")
 
         try:
             res = self.token_authorizer(aws_event['authorizationToken'])
             self.logger.warning(f"Token authorizer return is : {res}")
             return TokenResponse(res, aws_event['methodArn']).json
         except Exception as e:
             self.full_logger_error(e)
             return TokenResponse(False, aws_event['methodArn']).json
 
     def _api_handler(
-            self, aws_event: t.Dict[str, t.Any], aws_context: t.Dict[str, t.Any]
+            self, aws_event: dict[str, t.Any], aws_context: dict[str, t.Any]
     ) -> t.Optional[t.Union[dict, str]]:
         """API handler.
         """
         self.logger.warning(f"Calling {self.name} by api : {aws_event}")
 
         # Transforms as simple client call and manage exception if needed
         try:
@@ -393,31 +399,37 @@
                 # Strores response in S3 if asynchronous call
                 invocation_type = aws_event['headers'].get('invocationtype')
                 if invocation_type == 'Event':
                     self.store_response(resp, aws_event['headers'])
 
                 # Encodes binary content
                 if not isinstance(resp, dict):
-                    resp = base64.b64encode(resp).decode('ascii')
-                    content_length = len(resp) if self.logger.getEffectiveLevel() == logging.DEBUG else "N/A"
+                    str_resp = base64.b64encode(resp).decode('ascii')
+                    content_length = len(str_resp) if self.logger.getEffectiveLevel() == logging.DEBUG else "N/A"
                     self.logger.warning(f"API returns binary content [length: {content_length}]")
-                    return resp
+                    return str_resp
 
                 # Adds trace
                 self.logger.warning(f"API returns code {resp.get('statusCode')} and headers {resp.get('headers')}")
                 self.logger.warning(f"API body: {str(resp.get('body'))[:self.size_max_for_debug]}")
 
                 return resp
 
         except Exception as e:
-            self.full_logger_error(e)
+            # no more in app context so must print for trace
+            print(f"Exception in {self.name} : {e}")
+            parts = ["Traceback (most recent call last):\n"]
+            parts.extend(traceback.format_stack(limit=15)[:-2])
+            parts.extend(traceback.format_exception(*sys.exc_info())[1:])
+            trace = reduce(lambda x, y: x + y, parts, "")
+            print(f"Traceback: {trace}")
             headers = {'content_type': "application/json"}
             return self._aws_payload(str(e), InternalServerError.code, headers)
 
-    def _flask_handler(self, environ: t.Dict[str, t.Any], start_response: t.Callable[[t.Any], None]):
+    def _flask_handler(self, environ: WSGIEnvironment, start_response: StartResponse):
         """Flask handler.
         """
         return self.wsgi_app(environ, start_response)
 
     def _update_config(self, *, in_lambda: bool):
         if not self._cws_conf_updated:
             # Set predefined environment variables
@@ -435,18 +447,16 @@
             if request.url_rule:
                 view_function = self.view_functions.get(request.url_rule.endpoint, None)
                 if view_function:
                     no_auth = get_cws_annotations(view_function, '__CWS_NO_AUTH', False)
 
             # Checks token if authorization needed
             if not no_auth:
-                token = self.autorizer_identity_source
-                if token is None:
-                    raise Unauthorized(www_authenticate=WWWAuthenticate(auth_type="basic"))
                 try:
+                    token = self.header_autorizer_token
                     valid = self.token_authorizer(token)
                     if not valid:
                         raise Forbidden()
                 except Exception as e:
                     current_app.logger.exception(e)
                     raise Forbidden()
 
@@ -479,28 +489,24 @@
             "statusCode": status_code,
             "headers": {k: v for k, v in headers.items()},
             "body": body,
             "isBase64Encoded": False,
         }
 
     def full_logger_error(self, error):
-        if self.debug:
-            if not request.in_lambda_context:
-                raise
-            self.logger.error(f"Exception in {self.name} : {error}")
-            parts = ["Traceback (most recent call last):\n"]
-            parts.extend(traceback.format_stack(limit=15)[:-2])
-            parts.extend(traceback.format_exception(*sys.exc_info())[1:])
-            trace = reduce(lambda x, y: x + y, parts, "")
-            self.logger.error(f"Traceback: {trace}")
+        self.logger.error(f"Exception in {self.name} : {error}")
+        parts = ["Traceback (most recent call last):\n"]
+        parts.extend(traceback.format_stack(limit=15)[:-2])
+        parts.extend(traceback.format_exception(*sys.exc_info())[1:])
+        trace = reduce(lambda x, y: x + y, parts, "")
+        self.logger.error(f"Traceback: {trace}")
 
     def add_coworks_routes(self, bp_state: BlueprintSetupState | None = None) -> None:
         """ Creates all routes for a microservice.
 
-        :param app: The app microservice.
         :param bp_state: The blueprint state.
         """
 
         # Adds entrypoints
         stage = get_app_stage()
         scaffold = bp_state.blueprint if bp_state else self
         method_members = inspect.getmembers(scaffold.__class__, lambda x: inspect.isfunction(x))
```

### Comparing `coworks-0.9.2/coworks/cws/client.py` & `coworks-0.9.3/coworks/cws/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,46 +13,38 @@
 import yaml
 from click import UsageError
 from flask.cli import ScriptInfo
 
 from coworks import __version__
 from coworks.utils import DEFAULT_PROJECT_DIR
 from coworks.utils import PROJECT_CONFIG_VERSION
-from coworks.utils import get_app_stage
-from coworks.utils import load_dotenv
 from .deploy import deploy_command
 from .deploy import deployed_command
 from .deploy import destroy_command
 from .new import new_command
 from .utils import get_system_info
 from .utils import show_stage_banner
 
 
 class CwsScriptInfo(ScriptInfo):
 
     def __init__(self, project_dir=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.project_dir = project_dir
-        self.__dotenv_loaded = False
 
     @property
     def project_dir(self):
         return self.__project_dir
 
     @project_dir.setter
     def project_dir(self, project_dir):
-        self.__project_dir = Path(project_dir).absolute().as_posix() if project_dir else None
+        self.__project_dir = Path(project_dir).absolute() if project_dir else None
 
     @contextmanager
     def project_context(self, ctx=None):
-        if not self.__dotenv_loaded:
-            workspace = get_app_stage()
-            load_dotenv(workspace)
-            self.__dotenv_loaded = True
-
         old_dir = os.getcwd()
         try:
             os.chdir(self.project_dir)
         except OSError:
             if not ctx:
                 raise UsageError(f"Project dir {self.project_dir} not found.")
         finally:
@@ -71,15 +63,15 @@
 
 
 class CwsGroup(flask.cli.FlaskGroup):
 
     def __init__(self, add_default_commands=True, **extra):
         params = list(extra.pop("params", None) or ())
         extra["add_version_option"] = False
-        extra["load_dotenv"] = False
+        extra["load_dotenv"] = True
         super().__init__(params=params, **extra)
 
         if add_default_commands:
             self.add_command(t.cast(click.Command, new_command))
             self.add_command(t.cast(click.Command, deploy_command))
             self.add_command(t.cast(click.Command, destroy_command))
             self.add_command(t.cast(click.Command, deployed_command))
@@ -97,48 +89,50 @@
         if project_dir:
             script_info.project_dir = project_dir
             sys.path.insert(0, project_dir)
 
         # Adds environment variables and defined commands from project file
         project_config = ProjectConfig(project_dir, config_file, config_file_suffix)
         with script_info.project_context(ctx):
-            commands = project_config.get_commands(get_app_stage())
+            commands = project_config.get_commands(ctx.params.get('stage'))
             if commands:
                 for name, options in commands.items():
                     cmd_class_name = options.pop('class', None)
                     if cmd_class_name:
                         cmd_module, cmd_class = cmd_class_name.rsplit('.', 1)
                         try:
                             cmd = import_attr(cmd_module, cmd_class)
-                        except ModuleNotFoundError as e:
+                        except ModuleNotFoundError:
                             raise click.UsageError(f"Cannot load command {cmd_class!r} in module {cmd_module!r}.")
                     elif name in self.commands:
                         cmd = self.commands[name]
                     else:
                         raise click.UsageError(f"The command {name} is undefined or the class option is missing.")
 
                     # Sets option's value as default command param
                     # (may then be forced in command line or defined by default)
                     for param in cmd.params:
-                        if param.name in options:
-                            param.default = options.get(param.name)
+                        param_name = param.name.replace('-', '_')
+                        if param_name in options:
+                            param.default = options.get(param_name)
 
                     self.add_command(cmd, name)
 
         return ctx
 
 
 @click.group(cls=CwsGroup)
 @click.version_option(version=__version__, message=f'%(prog)s %(version)s, {get_system_info()}')
 @click.option('-p', '--project-dir', default=DEFAULT_PROJECT_DIR,
               help=f"The project directory path (absolute or relative) [default to '{DEFAULT_PROJECT_DIR}'].")
 @click.option('-c', '--config-file', default='project', help="Configuration file path [relative from project dir].")
 @click.option('--config-file-suffix', default='.cws.yml', help="Configuration file suffix.")
+@click.option('-s', '--stage', default='dev', help="Stage environment.")
 def client(*args, **kwargs):
-    ...
+    os.environ['CWS_STAGE'] = kwargs['stage']
 
 
 class ProjectConfig:
     """Class for the project configuration file."""
 
     def __init__(self, project_dir, file_name, file_suffix):
         getLogger('anyconfig').setLevel(WARNING)
@@ -176,14 +170,17 @@
             except FileNotFoundError:
                 return {}
 
         params = load(project_dir)
         if not params:
             params = load('.')
 
+        if not params:
+            click.secho("Warning: no project configuration file found", fg="yellow")
+
         return params
 
 
 def overriden_run_banner():
     """Copy the original function and add stage banner."""
     show_server_banner_copy = types.FunctionType(flask.cli.show_server_banner.__code__,
                                                  flask.cli.show_server_banner.__globals__,
```

### Comparing `coworks-0.9.2/coworks/cws/command.py` & `coworks-0.9.3/coworks/cws/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from click import Command
 from click import UsageError
 
+
 def no_project_context(f):
     """Decorator to allow command without need to have a project dir defined."""
     setattr(f, '__need_project_context', False)
     return f
 
+
 class CwsCommand(Command):
 
     def invoke(self, ctx):
         if getattr(self.callback, '__need_project_context', True) and not self._context_project_dir(ctx):
             raise UsageError(f"Project dir {self._context_project_dir(ctx)} not defined.")
         return super().invoke(ctx)
```

### Comparing `coworks-0.9.2/coworks/cws/deploy.py` & `coworks-0.9.3/coworks/cws/deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 import inspect
 import os
 import subprocess
 import sys
 import sysconfig
 import tempfile
 import typing as t
-from dataclasses import dataclass
 from datetime import datetime
 from functools import cached_property
 from functools import partial
 from pathlib import Path
 from shutil import ExecError
 from shutil import copyfile
 from shutil import copytree
 from shutil import ignore_patterns
 from shutil import make_archive
 from subprocess import CompletedProcess
 
 import boto3
 import click
-import dotenv
 from flask.cli import pass_script_info
 from flask.cli import with_appcontext
 from jinja2 import BaseLoader
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
+from pydantic import BaseModel
+from pydantic import ConfigDict
 from werkzeug.routing import Rule
 
 from coworks import aws
-from coworks.utils import get_app_stage
-from coworks.utils import get_env_filenames
 from coworks.utils import get_cws_annotations
+from coworks.utils import load_dotenv
 from .command import CwsCommand
 from .utils import progressbar
 from .utils import show_stage_banner
 from .utils import show_terraform_banner
 
 UID_SEP = '_'
 
@@ -53,63 +52,69 @@
         if info.app_import_path and '/' in info.app_import_path:
             msg = f"Cannot deploy or destroy a project with handler not on project folder : {info.app_import_path}.\n"
             msg += f"Add option -p {'/'.join(info.app_import_path.split('/')[:-1])} to resolve this."""
             raise ModuleNotFoundError()
         self.app_import_path = info.app_import_path.replace(':', '.') if info.app_import_path else "app.app"
 
 
-@dataclass
-class TerraformResource:
-    parent_uid: str
-    path: str
-    rules: t.List[Rule] = None
+class TerraformResource(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
+    parent_uid: str | None
+    path: str | None
+    rules: list[Rule] | None = None
 
     @cached_property
     def uid(self) -> str:
 
         if self.is_root:
             return ''
 
+        assert self.path is not None, "TerraformResource Path cannot be None"
         uid = self.path.replace('{', '').replace('}', '')
 
         if self.parent_is_root:
             return uid
 
-        parent_uid = self.parent_uid if len(self.parent_uid) < 80 else id(self.parent_uid)
+        # avoid too long id for ressources
+        parent_uid: str = self.parent_uid if len(self.parent_uid) < 80 else str(id(self.parent_uid))  # type: ignore
         return f"{parent_uid}{UID_SEP}{uid}" if self.path else parent_uid
 
     @cached_property
     def is_root(self) -> bool:
         return self.path is None
 
     @cached_property
     def parent_is_root(self) -> bool:
         return self.parent_uid == ''
 
-    # noinspection PyUnresolvedReferences
     @cached_property
-    def no_cors_methods(self) -> t.Iterator[t.Optional[str]]:
-        return (rule.methods for rule in self.rules if rule.cws_no_cors)
+    def no_cors_methods(self) -> t.Iterator[set[str] | None]:
+        if not self.rules:
+            return iter(())
+        return (rule.methods for rule in self.rules if getattr(rule, 'cws_no_cors', None))
 
     def __repr__(self):
         return f"{self.uid}:{self.rules}"
 
 
 class Terraform:
     """Terraform class to manage local terraform commands."""
     TIMEOUT = 600
 
-    def __init__(self, backend: 'TerraformBackend', terraform_dir, stage):
+    def __init__(self, backend: 'TerraformBackend', terraform_dir, workspace):
+        root_context = backend.terraform_context.ctx.find_root()
         self.terraform_context = backend.terraform_context
         self.app_context = backend.terraform_context
         self.bar = backend.bar
         self.terraform_dir = terraform_dir
         self.refresh = backend.terraform_refresh
-        self.stage = stage
-        self.working_dir = Path(backend.terraform_context.ctx.find_root().params.get('project_dir'))
+        self.stage = root_context.params['stage']
+        self.workspace = workspace
+        self.working_dir = Path(root_context.params.get('project_dir'))
 
     def init(self):
         self._execute(['init', '-input=false'])
 
     def apply(self) -> None:
         """Executes terraform apply command."""
         try:
@@ -127,50 +132,50 @@
     def output(self):
         values = self._execute(['output']).stdout
         return values.decode("utf-8").strip()
 
     @property
     def api_resources(self):
         """Returns the list of flatten path (prev_uid, last, rule)."""
-        resources: t.Dict[str, TerraformResource] = {}
+        resources: dict[str, TerraformResource] = {}
 
-        def add_rule(previous: t.Optional[str], path: t.Optional[str], rule_: t.Optional[Rule]):
+        def add_rule(previous: str, path: str, rule_: Rule | None):
             """Add a method rule in a resource."""
             # todo : may use now aws_url_map
             path = None if path is None else path.replace('<', '{').replace('>', '}')
-            resource = TerraformResource(previous, path)
+            resource = TerraformResource(parent_uid=previous, path=path)
             if rule_:
                 view_function = self.app_context.app.view_functions.get(rule_.endpoint)
-                rule_.cws_binary_headers = get_cws_annotations(view_function, '__CWS_BINARY_HEADERS')
-                rule_.cws_no_auth = get_cws_annotations(view_function, '__CWS_NO_AUTH')
-                rule_.cws_no_cors = get_cws_annotations(view_function, '__CWS_NO_CORS')
+                setattr(rule_, 'cws_binary_headers', get_cws_annotations(view_function, '__CWS_BINARY_HEADERS'))
+                setattr(rule_, 'cws_no_auth', get_cws_annotations(view_function, '__CWS_NO_AUTH'))
+                setattr(rule_, 'cws_no_cors', get_cws_annotations(view_function, '__CWS_NO_CORS'))
 
             # Creates terraform ressources if it doesn't exist.
             uid = resource.uid
             if uid not in resources:
                 resources[uid] = resource
 
             resource = resources[uid]
             if rule_:
                 if resources[uid].rules is None:
                     resources[uid].rules = [rule_]
                 else:
-                    resources[uid].rules.append(rule_)
+                    resources[uid].rules.append(rule_)  # type: ignore[union-attr]
             return uid
 
         for rule in self.app_context.app.url_map.iter_rules():
             route = rule.rule
             previous_uid = ''
             if route.startswith('/'):
                 route = route[1:]
             splited_route = route.split('/')
 
             # special root case
             if splited_route == ['']:
-                add_rule(None, None, rule)
+                add_rule('', '', rule)
                 continue
 
             # creates intermediate resources
             for prev in splited_route[:-1]:
                 previous_uid = add_rule(previous_uid, prev, None)
 
             # set entry keys for last entry
@@ -180,54 +185,54 @@
 
     @property
     def logger(self):
         return self.app_context.app.logger
 
     @property
     def template_loader(self) -> BaseLoader:
-        return PackageLoader(sys.modules[__name__].__package__)
+        package_name = sys.modules[__name__].__package__
+        assert package_name is not None
+        return PackageLoader(package_name)
 
     @property
     def jinja_env(self) -> Environment:
         return Environment(loader=self.template_loader, autoescape=select_autoescape(['html', 'xml']),
                            trim_blocks=True, lstrip_blocks=True)
 
     def get_context_data(self, **options) -> dict:
-        workspace = get_app_stage()
-
         # Microservice context data
         app = self.app_context.app
+        tf_key = options.pop('tf_key', None) or app.name.replace('_', '/')
         data = {
             'api_resources': self.api_resources,
             'app': app,
             'app_import_path': self.app_context.app_import_path,
             'debug': app.debug,
             'description': inspect.getdoc(app) or "",
-            'environment_variables': load_dotvalues(self.working_dir, workspace),
+            'environment_variables': load_dotenv(self.stage),
             'ms_name': app.name,
             'now': datetime.now().isoformat(),
-            'workspace': workspace,
+            'tf_key': tf_key,
+            'stage': self.stage,
+            'workspace': self.workspace,
             **options
         }
 
-        if self.stage:
-            data['stage'] = self.stage
-
         # AWS context data
         profile_name = options.get('profile_name')
         if profile_name:
             aws_session = boto3.Session(profile_name=profile_name)
             aws_region = aws_session.region_name
             data['aws_region'] = aws_region
             aws_account = aws_session.client("sts").get_caller_identity()["Account"]
             data['aws_account'] = aws_account
 
         return data
 
-    def _execute(self, cmd_args: t.List[str]) -> CompletedProcess:
+    def _execute(self, cmd_args: list[str]) -> CompletedProcess:
         self.logger.debug(f"Terraform arguments : ['-chdir={self.terraform_dir} {' '.join(cmd_args)}]")
         p = subprocess.run(["terraform", *cmd_args], capture_output=True, cwd=self.terraform_dir,
                            timeout=self.TIMEOUT)
         if p.returncode != 0:
             msg = p.stderr.decode('utf-8')
             if not msg:
                 msg = p.stdout.decode('utf-8')
@@ -251,42 +256,42 @@
         """
         self.terraform_context = terraform_context
         self.app = terraform_context.app
         self.bar = bar
 
         # Creates terraform dir if needed
         self.terraform_dir = Path(options['terraform_dir'])
-        self.stage = get_app_stage()
+        self.stage = terraform_context.ctx.find_root().params['stage']
 
         self.terraform_class = Terraform
         self.terraform_refresh = options['terraform_refresh']
         self._api_terraform = self._stage_terraform = None
 
     @property
     def api_terraform(self):
         if self._api_terraform is None:
             self.app.logger.debug(f"Create common terraform instance using {self.terraform_class}")
             self.terraform_dir.mkdir(exist_ok=True)
-            self._api_terraform = self.terraform_class(self, terraform_dir=self.terraform_dir, stage="common")
+            self._api_terraform = self.terraform_class(self, terraform_dir=self.terraform_dir, workspace="common")
         return self._api_terraform
 
     @property
     def stage_terraform(self):
         if self._stage_terraform is None:
             self.app.logger.debug(f"Create {self.stage} terraform instance using {self.terraform_class}")
             terraform_dir = Path(f"{self.terraform_dir}_{self.stage}")
             terraform_dir.mkdir(exist_ok=True)
-            self._stage_terraform = self.terraform_class(self, terraform_dir=terraform_dir, stage=self.stage)
+            self._stage_terraform = self.terraform_class(self, terraform_dir=terraform_dir, workspace=self.stage)
         return self._stage_terraform
 
     def process_terraform(self, command_template, terraform_init=True, **options):
         root_command_params = self.terraform_context.ctx.find_root().params
 
         # Set default options calculated value
-        options['key'] = options.get('key') or f"{self.app.__module__}-{self.app.name}/archive.zip"
+        options['key'] = options.get('key') or f"{self.app.name}/archive.zip"
 
         # Transfert zip file to S3
         self.bar.update(msg="Copy source files on S3")
         b64sha256 = self.copy_sources_to_s3(**options)
         options['source_code_hash'] = b64sha256
 
         self.bar.update(msg="Generates terraform files")
@@ -308,14 +313,15 @@
         if options['dry']:
             self.bar.update(msg="Nothing deployed and destroyed (dry mode)")
             return
 
         if terraform_init:
             self.app.logger.debug("Init terraform")
             self.api_terraform.init()
+            assert self._stage_terraform is not None
             self._stage_terraform.init()
 
         # Apply to api terraform
         self.bar.update(msg="Create or update API")
         self.api_terraform.apply()
         if options.get('api'):
             return
@@ -326,15 +332,15 @@
 
         self.delete_sources_on_s3(**options)
 
         # Traces output
         self.bar.terminate()
         click.echo()
         echo_output(self.api_terraform)
-        click.secho("Microservice deployed", fg="green")
+        click.secho("🎉 CoWorks Microservice deployed", fg="green")
 
     def copy_sources_to_s3(self, dry, **options):
         module_name = options.get('module_name') or []
         bucket = options.get('bucket')
         key = options.get('key')
         with tempfile.TemporaryDirectory() as tmp_dir:
             tmp_path = Path(tmp_dir)
@@ -367,14 +373,15 @@
 
             for name in module_name:
                 if name.endswith(".py"):
                     file_path = Path(sysconfig.get_path('purelib')) / name
                     copyfile(file_path, tmp_sources_path / name)
                 else:
                     mod = importlib.import_module(name)
+                    assert mod.__file__ is not None
                     module_path = Path(mod.__file__).resolve().parent
                     copytree(module_path, tmp_sources_path / name, ignore=full_ignore_patterns())
             module_archive = make_archive(str(tmp_path / 'sources'), 'zip', tmp_sources_path)
 
             # Uploads archive on S3
             with open(module_archive, 'rb') as archive:
                 size = int(os.path.getsize(module_archive) / 1000)
@@ -421,57 +428,61 @@
               help="Content types defined as binary contents (no encoding).")
 @click.option('--json-types', multiple=True,
               help="Add mime types for JSON response.")
 @click.option('--layers', '-l', multiple=True, required=True,
               help="Add layer (full arn: aws:lambda:...). Must contains CoWorks at least.")
 @click.option('--memory-size', default=128,
               help="Lambda memory size (default 128).")
-@click.option('--python', '-p', type=click.Choice(['3.7', '3.8', '3.9', '3.10', '3.11']), default='3.11',
+@click.option('--python', '-p', type=click.Choice(['3.8', '3.9', '3.10', '3.11']), default='3.11',
               help="Python version for the lambda.")
+@click.option('--tf-bucket',
+              help="Bucket's name if not using cloud terraform.")
+@click.option('--tf-key',
+              help="Bucket's key if not using cloud terraform (default microservice's name).")
 @click.option('--security-groups', multiple=True, default=[],
               help="Security groups to be added [ids].")
-@click.option('-s', '--stage', default='dev',
-              help="Deploiement stage.")
 @click.option('--subnets', multiple=True, default=[],
               help="Subnets to be added [ids].")
 @click.option('--terraform-cloud', '-tc', is_flag=True, default=False,
               help="Use cloud workspaces (default false).")
 @click.option('--terraform-dir', '-td', default="terraform",
               help="Terraform files folder (default terraform).")
 @click.option('--terraform-organization', '-to',
-              help="Terraform organization needed if using cloud terraform.")
-@click.option('--terraform-refresh', '-tr', is_flag=True, default=False,
-              help="Forces terraform to refresh the state (default false).")
+              help="Terraform organization (needed if using cloud terraform).")
+@click.option('--terraform-refresh', '-tr', is_flag=True, default=True,
+              help="Forces terraform to refresh the state (default true).")
 @click.option('--text-types', multiple=True,
               help="Add mime types for JSON response [at least text/plain, text/html].")
 @click.option('--timeout', default=60,
               help="Lambda timeout (default 60s).Only for asynchronous call (API call 30s).")
 @click.option('--token-key',
               help="Header token key.")
 @click.pass_context
 @pass_script_info
 @with_appcontext
-def deploy_command(info, ctx, stage, **options) -> None:
+def deploy_command(info, ctx, **options) -> None:
     """ Deploiement in 2 steps:
         Step 1. Create API and routes integrations
         Step 2. Deploy API and Lambda
     """
     if options.get('terraform_cloud') and not options.get('terraform_organization'):
         raise click.BadParameter('An organization must be defined if using cloud terraform')
+    if not options.get('terraform_cloud') and not options.get('tf_bucket'):
+        raise click.BadParameter('A bucket must be defined if using terraform on S3 [--tf-bucket option]')
 
     terraform_context = TerraformContext(info, ctx)
     app = terraform_context.app
-    os.environ['CWS_STAGE'] = stage  # TODO Should be removed
+    stage = ctx.parent.params['stage']
 
     app.logger.debug(f"Start deploy command: {options}")
     show_stage_banner(stage)
-    cloud = options.get('terraform_cloud')
-    refresh = options.get('terraform_refresh')
+    cloud = options['terraform_cloud']
+    refresh = options['terraform_refresh']
     show_terraform_banner(cloud, refresh)
-    with progressbar(label="Deploy microservice", threaded=not app.debug) as bar:
+    with progressbar(label="Deploy microservice", threaded=not app.debug) as bar:  # type: ignore
         terraform_backend_class = options.pop('terraform_class', TerraformBackend)
         app.logger.debug(f"Deploying {app} using {terraform_backend_class}")
         backend = terraform_backend_class(terraform_context, bar, **options)
         backend.process_terraform('deploy.j2', **options)
 
 
 @click.command("destroy", CwsCommand, short_help="Destroy the CoWorks microservice on AWS Lambda.")
@@ -480,73 +491,67 @@
               help="Bucket to upload sources zip file to")
 @click.option('--dry', is_flag=True,
               help="Doesn't perform deploy [Global option only].")
 @click.option('--key', '-k',
               help="Sources zip file bucket's name.")
 @click.option('--profile-name', '-pn', required=True,
               help="AWS credential profile.")
-@click.option('-s', '--stage', default='dev',
-              help="Deploiement stage.")
-@click.option('--terraform-dir', default="terraform",
-              help="Terraform folder (default terraform).")
-@click.option('--terraform-cloud', is_flag=True,
+@click.option('--terraform-cloud', is_flag=True, default=False,
               help="Use cloud workspaces (default false).")
 @click.option('--terraform-dir', '-td', default="terraform",
               help="Terraform files folder (default terraform).")
 @click.option('--terraform-organization', '-to',
               help="Terraform organization needed if using cloud terraform.")
-@click.option('--terraform-refresh', '-tr', is_flag=True, default=False,
-              help="Forces terraform to refresh the state (default false).")
+@click.option('--terraform-refresh', '-tr', is_flag=True, default=True,
+              help="Forces terraform to refresh the state (default true).")
 @click.pass_context
 @pass_script_info
 @with_appcontext
-def destroy_command(info, ctx, stage, **options) -> None:
+def destroy_command(info, ctx, **options) -> None:
     """ Destroy by setting counters to 0.
     """
     terraform_context = TerraformContext(info, ctx)
-    os.environ['CWS_STAGE'] = stage  # TODO Should be removed
+    stage = ctx.parent.params['stage']
 
     app = terraform_context.app
     app.logger.debug(f"Start destroy command: {options}")
     show_stage_banner(stage)
-    cloud = options.get('terraform_cloud')
-    refresh = options.get('terraform_refresh')
+    cloud = options['terraform_cloud']
+    refresh = options['terraform_refresh']
     show_terraform_banner(cloud, refresh)
-    with progressbar(label='Destroy microservice', threaded=not app.debug) as bar:
+    with progressbar(label='Destroy microservice', threaded=not app.debug) as bar:  # type: ignore
         terraform_backend_class = options.pop('terraform_class', TerraformBackend)
         app.logger.debug(f'Destroying {app} using {terraform_backend_class}')
         backend = terraform_backend_class(terraform_context, bar, **options)
         backend.process_terraform('destroy.j2', terraform_init=False, **options)
     if not options['dry']:
-        click.echo(f"You can now delete the terraform_{get_app_stage()} folder.")
+        click.echo(f"You can now delete the terraform_{options.get('stage')} folder.")
 
 
 @click.command("deployed", CwsCommand, short_help="Retrieve the microservices deployed for this project.")
-@click.option('-s', '--stage', default='dev',
-              help="Deploiement stage.")
 @click.option('--terraform-dir', default="terraform",
               help="Terraform folder (default terraform).")
-@click.option('--terraform-cloud', is_flag=True,
+@click.option('--terraform-cloud', is_flag=True, default=False,
               help="Use cloud workspaces (default false).")
-@click.option('--terraform-refresh', '-tr', is_flag=True, default=False,
-              help="Forces terraform to refresh the state (default false).")
+@click.option('--terraform-refresh', '-tr', is_flag=True, default=True,
+              help="Forces terraform to refresh the state (default true).")
 @click.pass_context
 @pass_script_info
 @with_appcontext
-def deployed_command(info, ctx, stage, **options) -> None:
+def deployed_command(info, ctx, **options) -> None:
     terraform_context = TerraformContext(info, ctx)
     app = terraform_context.app
-    os.environ['CWS_STAGE'] = stage  # TODO Should be removed
+    stage = ctx.parent.params['stage']
 
     app.logger.debug(f"Start destroy command: {options}")
     show_stage_banner(stage)
-    cloud = options.get('terraform_cloud')
-    refresh = options.get('terraform_refresh')
+    cloud = options['terraform_cloud']
+    refresh = options['terraform_refresh']
     show_terraform_banner(cloud, refresh)
-    with progressbar(label='Retrieving information', threaded=not app.debug) as bar:
+    with progressbar(label='Retrieving information', threaded=not app.debug) as bar:  # type: ignore
         terraform_backend_class = options.pop('terraform_class', TerraformBackend)
         app.logger.debug(f'Destroying {app} using {terraform_backend_class}')
         backend = terraform_backend_class(terraform_context, bar, **options)
     echo_output(backend.api_terraform)
 
 
 def echo_output(terraform):
@@ -556,16 +561,7 @@
     for row in rows.split('\n'):
         values = row.split('=')
         if len(values) > 1:
             cws_name = values[0].strip()[:-3]  # remove last _id
             api_id = values[1].strip()[1:-1]  # remove quotes
             api_url = f"https://{api_id}.execute-api.eu-west-1.amazonaws.com/"
             click.secho(f"The microservice {cws_name} is deployed at {api_url}", fg='yellow')
-
-
-def load_dotvalues(working_dir, stage):
-    environment_variables = {}
-    for env_filename in get_env_filenames(stage):
-        path = dotenv.find_dotenv(working_dir / env_filename, usecwd=True)
-        if path:
-            environment_variables.update(dotenv.dotenv_values(path))
-    return environment_variables
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `coworks-0.9.2/coworks/cws/new.py` & `coworks-0.9.3/coworks/cws/new.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/cws/project_templates/README.md` & `coworks-0.9.3/coworks/cws/project_templates/README.md`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/cws/project_templates/tech/app.py` & `coworks-0.9.3/coworks/cws/project_templates/tech/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
 from coworks import TechMicroService
 from coworks import entry
 from coworks.blueprint.admin_blueprint import Admin
 from coworks.blueprint.profiler_blueprint import Profiler
-from coworks.utils import get_app_stage
 
 
 # from aws_xray_sdk.core import xray_recorder
 # from coworks.extension.xray import XRay
 
 
 class MyMicroService(TechMicroService):
@@ -16,15 +15,15 @@
 ## Microservice for ...
 """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.register_blueprint(Admin(), url_prefix='/admin')
-        if get_app_stage() == "dev":
+        if os.getenv('CWS_STAGE') == "dev":
             self.register_blueprint(Profiler(self), url_prefix='/profiler')
 
         @self.before_request
         def before():
             ...
 
         @self.errorhandler(500)
@@ -36,15 +35,15 @@
         from flask_migrate import Migrate
         Migrate(self, db)
         """
 
     def token_authorizer(self, token):
         # Simple authorization process.
         # If you want to access AWS event or context for a more complex case, override the function _token_handler.
-        return token in os.getenv('USER_KEYS').split(',')
+        return token in os.getenv('USER_KEYS', '').split(',')
 
     @entry
     def get(self):
         return 'project ready!\n'
 
 
 app = MyMicroService()
```

### Comparing `coworks-0.9.2/coworks/cws/templates/terraform.j2` & `coworks-0.9.3/coworks/cws/templates/terraform.j2`

 * *Files 12% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 # TERRAFORM ON S3
 # ---------------------------------------------------------------------------------------------------------------------
 
 variable "AWS_REGION" {default="eu-west-1"}
 
 terraform {
   backend "s3" {
-    bucket  = "neorezo-terraform"
-    key     = "{{ project }}/{{ stage }}/tfstate.json"
+    bucket  = "{{ tf_bucket }}"
+    key     = "{{ tf_key }}/tfstate_{{ workspace }}.json"
     region  = {{ '"{}"'.format(aws_region) if aws_region else 'var.CUSTOMER_AWS_REGION'}}
     profile = "{{ profile_name }}"
   }
   required_version = ">= 1.2.0"
   required_providers {
     local = {
       source  = "hashicorp/local"
```

### Comparing `coworks-0.9.2/coworks/cws/templates/terraform/lambda.j2` & `coworks-0.9.3/coworks/cws/templates/terraform/lambda.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-{% if stage != "common" %}
+{% if workspace != "common" %}
 # ---------------------------------------------------------------------------------------------------------------------
 # LAMBDA
 # ---------------------------------------------------------------------------------------------------------------------
 
 locals {
-  {{ ms_name }}_lambda_name = "{{ ms_name }}-{{ workspace }}"
+  {{ ms_name }}_lambda_name = "{{ ms_name }}-{{ stage }}"
   {% if environment_variable_files %}
   {{ ms_name }}_environment_variables = [
     for envars_string in data.local_file.{{ ms_name }}_environment_variables_files: jsondecode(envars_string.content)
   ]
   {% endif %}
 }
 
@@ -42,19 +42,16 @@
   {% endif %}
   runtime = "python{{ python }}"
   timeout = {{ timeout }}
   memory_size = {{ memory_size }}
   environment {
     variables = merge(
       {{ environment_variables | tojson }},
-      {"FLASK_DEBUG":"{{ '1' if workspace == "dev" else '0' }}", "CWS_STAGE":"{{ workspace }}"},
-      {"CWS_DATETIME": "{{ now }}"},
-      {"CWS_LAMBDA": "{{ ms_name }}"},
-      {"CWS_BUCKET": "{{ bucket }}"},
-      {"CWS_KEY": "{{ key }}"}
+      {"FLASK_DEBUG":"{{ '1' if stage == "dev" else '0' }}","CWS_STAGE":"{{ stage }}"},
+      {"CWS_DATETIME": "{{ now }}","CWS_LAMBDA": "{{ ms_name }}","CWS_BUCKET": "{{ bucket }}","CWS_KEY": "{{ key }}"}
     )
   }
   tracing_config {
     mode = "Active"
   }
   {% block vpc_config %}
   vpc_config {
```

### Comparing `coworks-0.9.2/coworks/cws/templates/terraform/request_templates.j2` & `coworks-0.9.3/coworks/cws/templates/terraform/request_templates.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/cws/templates/terraform/response_templates.j2` & `coworks-0.9.3/coworks/cws/templates/terraform/response_templates.j2`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/cws/templates/terraform/rest_api.j2` & `coworks-0.9.3/coworks/cws/templates/terraform/rest_api.j2`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # ---------------------------------------------------------------------------------------------------------------------
 # API GATEWAY
 # ---------------------------------------------------------------------------------------------------------------------
 
 locals {
   {{ ms_name }}_authorizer_uri = "arn:aws:apigateway:${local.region}:lambda:path/2015-03-31/functions/arn:aws:lambda:${local.region}:${local.account_id}:function:{{ ms_name }}-$${stageVariables.stage}/invocations"
-{% if stage != "common" %}
+{% if workspace != "common" %}
   {{ ms_name }}_api_arn = data.aws_api_gateway_rest_api.{{ ms_name }}.arn
   {{ ms_name }}_api_id = data.aws_api_gateway_rest_api.{{ ms_name }}.id
   {{ ms_name }}_api_root_id = data.aws_api_gateway_rest_api.{{ ms_name }}.root_resource_id
 {% else %}
   {{ ms_name }}_api_arn = aws_api_gateway_rest_api.{{ ms_name }}.arn
   {{ ms_name }}_api_id = aws_api_gateway_rest_api.{{ ms_name }}.id
   {{ ms_name }}_api_root_id = aws_api_gateway_rest_api.{{ ms_name }}.root_resource_id
 {% endif %}
   {{ ms_name }}_api_binary_media_types = ["multipart/form-data", "application/octet-stream", "application/pdf", "image/*"
     {%- if binary_types -%}{%- for type in binary_types -%},"{{ type }}"{%- endfor -%}{%- endif -%}]
 }
 
-{% if stage == "common" %}
+{% if workspace == "common" %}
 resource "aws_api_gateway_rest_api" "{{ ms_name }}" {
   provider = aws.{{ ms_name }}
   {% block aws_api_gateway_rest_api %}
   name = "{{ ms_name }}"
   description = "{{ description | replace("\n", "\\n") }}"
   binary_media_types = local.{{ ms_name }}_api_binary_media_types
   endpoint_configuration {
@@ -56,18 +56,18 @@
   {% endif %}
   {% if resource.rules %}
     {% for rule in resource.rules %}
     {% for method in rule.methods if method not in ['HEAD', 'OPTIONS'] %}
 resource "aws_api_gateway_method" "{{ ms_name }}_{{ uid }}_{{ method }}" {
   provider = aws.{{ ms_name }}
   rest_api_id = local.{{ ms_name }}_api_id
-  {% if resource.is_root %}
-  resource_id = local.{{ ms_name }}_api_root_id
-  {% else %}
+  {% if resource.path %}
   resource_id = aws_api_gateway_resource.{{ ms_name }}_{{ uid }}.id
+  {% else %}
+  resource_id = local.{{ ms_name }}_api_root_id
   {% endif %}
   http_method = "{{ method }}"
   {% if rule.cws_no_auth %}
   authorization = "NONE"
   {% else %}
   authorization = "CUSTOM"
   authorizer_id = aws_api_gateway_authorizer.{{ ms_name }}.id
@@ -78,18 +78,18 @@
     "method.request.header.Referer" = false
     "method.request.header.X-Forwarded-Host" = false
   }
 }
 resource "aws_api_gateway_integration" "{{ ms_name }}_{{ uid }}_{{ method }}" {
   provider = aws.{{ ms_name }}
   rest_api_id = local.{{ ms_name }}_api_id
-  {% if resource.is_root %}
-  resource_id = local.{{ ms_name }}_api_root_id
-  {% else %}
+  {% if resource.path %}
   resource_id = aws_api_gateway_resource.{{ ms_name }}_{{ uid }}.id
+  {% else %}
+  resource_id = local.{{ ms_name }}_api_root_id
   {% endif %}
   http_method = "{{ method }}"
   integration_http_method = "POST"
   type = "AWS"
   uri = local.{{ ms_name }}_authorizer_uri
   passthrough_behavior = "NEVER"
   content_handling = "CONVERT_TO_TEXT"
@@ -103,18 +103,18 @@
     {% include "terraform/request_templates.j2" %}
   }
   depends_on = [aws_api_gateway_method.{{ ms_name }}_{{ uid }}_{{ method }}]
 }
 resource "aws_api_gateway_integration_response" "{{ ms_name }}_{{ uid }}_{{ method }}_200" {
   provider = aws.{{ ms_name }}
   rest_api_id = local.{{ ms_name }}_api_id
-  {% if resource.is_root %}
-  resource_id = local.{{ ms_name }}_api_root_id
-  {% else %}
+  {% if resource.path %}
   resource_id = aws_api_gateway_resource.{{ ms_name }}_{{ uid }}.id
+  {% else %}
+  resource_id = local.{{ ms_name }}_api_root_id
   {% endif %}
   http_method = join("", aws_api_gateway_method.{{ ms_name }}_{{ uid }}_{{ method }}.*.http_method)
   status_code = "200"
   {% if rule.cws_binary_headers %}
   response_parameters = {
   {% for k, v in rule.cws_binary_headers.items() %}
     "method.response.header.{{ k }}" = "'{{ v }}'",
@@ -127,18 +127,18 @@
   }
   {% endif %}
   depends_on = [aws_api_gateway_method_response.{{ ms_name }}_{{ uid }}_{{ method }}_200]
 }
 resource "aws_api_gateway_method_response" "{{ ms_name }}_{{ uid }}_{{ method }}_200" {
   provider = aws.{{ ms_name }}
   rest_api_id = local.{{ ms_name }}_api_id
-  {% if resource.is_root %}
-  resource_id = local.{{ ms_name }}_api_root_id
-  {% else %}
+  {% if resource.path %}
   resource_id = aws_api_gateway_resource.{{ ms_name }}_{{ uid }}.id
+  {% else %}
+  resource_id = local.{{ ms_name }}_api_root_id
   {% endif %}
   http_method = "{{ method }}"
   status_code = "200"
   {% if rule.cws_binary_headers %}
   response_parameters = {
     {% for k in rule.cws_binary_headers.keys() %}
     "method.response.header.{{ k }}" = true,
@@ -261,15 +261,15 @@
   }
   {% endblock %}
 }
 
 resource "aws_cloudwatch_log_group" "api_{{ ms_name }}" {
   provider = aws.{{ ms_name }}
   {% block aws_cloudwatch_log_group %}
-  name = "API-Gateway-Execution-Logs_${local.{{ ms_name }}_api_id}/{{ workspace }}"
+  name = "API-Gateway-Execution-Logs_${local.{{ ms_name }}_api_id}/{{ stage }}"
   retention_in_days = 7
   {% endblock %}
 }
 
 resource "aws_api_gateway_method_settings" "api_{{ ms_name }}" {
   provider = aws.{{ ms_name }}
   {% block aws_api_gateway_method_settings %}
```

### Comparing `coworks-0.9.2/coworks/cws/templates/terraform/role.j2` & `coworks-0.9.3/coworks/cws/templates/terraform/role.j2`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 locals {
-{% if stage != "common" %}
+{% if workspace != "common" %}
   {{ ms_name }}_role_arn = data.aws_iam_role.{{ ms_name }}_cws.arn
 {% else %}
   {{ ms_name }}_role_arn = aws_iam_role.{{ ms_name }}_cws.arn
 {% endif %}
 }
 
 # ---------------------------------------------------------------------------------------------------------------------
 # ROLE
 # ---------------------------------------------------------------------------------------------------------------------
 
-{% if stage != "common" %}
+{% if workspace != "common" %}
 data "aws_iam_role" "{{ ms_name }}_cws" {
   provider = aws.{{ ms_name }}
   name = "{{ ms_name }}_cws_role"
 }
 {% else %}
 resource "aws_iam_role" "{{ ms_name }}_cws" {
   provider = aws.{{ ms_name }}
```

### Comparing `coworks-0.9.2/coworks/cws/utils.py` & `coworks-0.9.3/coworks/cws/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,33 +4,31 @@
 from contextlib import contextmanager
 from importlib.metadata import version
 from threading import Thread
 from time import sleep
 
 import click
 
-from coworks.utils import get_app_stage
-
 
 def get_system_info():
     flask_version = version("flask")
 
     flask_info = f"flask {flask_version}"
     python_info = f"python {sys.version_info[0]}.{sys.version_info[1]}.{sys.version_info[2]}"
     platform_system = platform.system().lower()
     platform_release = platform.release()
     platform_info = f"{platform_system} {platform_release}"
     return f"{flask_info}, {python_info}, {platform_info}"
 
 
-def show_stage_banner(stage='dev'):
-    click.secho(f" * Stage: {get_app_stage()}", fg="green")
+def show_stage_banner(stage: str = 'dev'):
+    click.secho(f" * Stage: {stage}", fg="green")
 
 
-def show_terraform_banner(cloud, refresh):
+def show_terraform_banner(cloud: bool, refresh: bool):
     click.secho(f" * Using terraform backend {'cloud' if cloud else 's3'} (refresh={refresh})", fg="green")
 
 
 class ProgressBar:
 
     def __init__(self, bar):
         self.bar = bar
@@ -56,14 +54,17 @@
         self.bar.finish()
         self.bar.render_progress()
         if msg:
             self.echo(msg)
 
 
 class DebugProgressBar:
+    def update(self, msg: str):
+        if msg:
+            click.echo("==> " + msg)
 
     def echo(self, msg: str):
         if msg:
             click.echo("==> " + msg)
 
 
 @contextmanager  # type: ignore[arg-type]
```

### Comparing `coworks-0.9.2/coworks/extension/odoo.py` & `coworks-0.9.3/coworks/extension/odoo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-import base64
 import os
 import typing as t
 import xmlrpc.client
 
 import requests
 from aws_xray_sdk.core import xray_recorder
-from flask import json
 from pydantic import BaseModel
+from pydantic import ConfigDict
 from pydantic import Field
+from pydantic import field_validator
 from werkzeug.exceptions import BadRequest
-from werkzeug.exceptions import Forbidden
 from werkzeug.exceptions import NotFound
 
+from coworks import TechMicroService
 from coworks.extension.xray import XRay
+from .jsonapi import JsonApiDataMixin
+from .jsonapi import JsonApiDict
+from .jsonapi.data import CursorPagination
 
 
 class OdooConfig(BaseModel):
-    ref: t.Optional[str] = "default"
+    model_config = ConfigDict(from_attributes=True)
+
     url: str
     dbname: str
     user: str
     passwd: str
-    const: t.Optional[t.Dict[str, t.Any]] = Field(default_factory=dict)
+    const: dict[str, t.Any] = Field(default_factory=dict)
 
     @classmethod
     def from_env_var_prefix(cls, env_var_prefix):
         env_url_var_name = f"{env_var_prefix}_URL"
         env_dbname_var_name = f"{env_var_prefix}_DBNAME"
         env_user_var_name = f"{env_var_prefix}_USER"
         env_passwd_var_name = f"{env_var_prefix}_PASSWD"
@@ -46,169 +50,221 @@
         passwd = os.getenv(env_passwd_var_name)
         if not passwd:
             raise RuntimeError(f'{env_passwd_var_name} not defined in environment.')
 
         return OdooConfig(url=url, dbname=dbname, user=user, passwd=passwd)
 
 
+class OdooPagination(CursorPagination):
+    """Odoo pagination using limit value and odoo request."""
+    max_per_page: int | None = None
+    query: t.Any | None = None
+
+    @field_validator("max_per_page")
+    def set_max_per_page(cls, max_per_page):
+        return max_per_page or 100
+
+    def __iter__(self):
+        if self.query:
+            return iter(self.query.odoo_execute_kw(self.params))
+        raise StopIteration()
+
+    @property
+    def params(self):
+        assert self.page is not None  # by the validator
+        assert self.per_page is not None  # by the validator
+        if self.page < 1:
+            self.page = 1
+        return {
+            'limit': self.per_page,
+            'offset': (self.page - 1) * self.per_page,
+        }
+
+
+class OdooQuery(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
+    odoo: "Odoo"
+    model: str
+    method: str
+    order: str | None = None
+    fields: list[str] | None = None
+    domain: list[tuple[str, str, t.Any]] | None
+    bind_key: str | None = None  # key to access the configuration defined in binds
+
+    def paginate(self, *, page=None, per_page=None, max_per_page=None) -> OdooPagination:
+        pagination = OdooPagination(query=self, page=page, per_page=per_page, max_per_page=max_per_page, total=0)
+        res = self.odoo.odoo_execute_kw(self.model, "search_count", [self.domain], bind_key=self.bind_key)
+        pagination.total = res
+        return pagination
+
+    def all(self, limit=2) -> list[JsonApiDataMixin]:
+        """Mainly used only to get one resource so set limit to 2."""
+        params = {
+            'limit': limit,
+            'offset': 0,
+        }
+        return self.odoo_execute_kw(params)
+
+    def odoo_execute_kw(self, params):
+        res = self.odoo.odoo_execute_kw(self.model, self.method, [self.domain], params, bind_key=self.bind_key)
+        return [JsonApiDict(**rec) for rec in res]
+
+
 class Odoo:
     """Flask's extension for Odoo.
     This extension uses the external API of ODOO.
 
+    At creation: a default configuration must be done or a binding dict oj configurations.
+    At execution: if no binding key is provided, the default configuration is used.
+
     .. versionchanged:: 0.7.3
         ``env_var_prefix`` parameter may be a dict of bind values.
         GraphQL removed.
     """
 
-    def __init__(self, app=None, config: OdooConfig = None, binds: t.Dict[t.Optional[str], OdooConfig] = None):
+    def __init__(self, app: TechMicroService | None = None,
+                 config: OdooConfig | None = None, binds: dict[str | None, OdooConfig] | None = None):
+
         """
         :param app: Flask application.
-        :param config: default configuration.
-        :param binds: configuration binds.
+        :param config: default configuration if no bind given in execution.
+        :param binds: list of configuration binds.
         """
+
         self.app = None
 
         self.binds = binds if binds else {}
         if config:
             self.binds[None] = config
 
         if app:
             self.init_app(app)
 
     def init_app(self, app):
         self.app = app
 
     @XRay.capture(xray_recorder)
-    def kw(self, model: str, method: str = "search_read", id: int = None, fields: t.List[str] = None,
-           order: str = None, domain: t.List[t.Tuple[str, str, t.Any]] = None, limit: t.Optional[int] = None,
-           page: t.Optional[int] = None, ensure_one: bool = False, bind: str = None):
+    def query(self, model: str, method: str = "search_read", *, fields: list[str] | None = None,
+              order: str | None = None, domain: list[tuple[str, str, t.Any]] | None = None,
+              bind_key: str | None = None):
+        return OdooQuery(odoo=self, model=model, method=method, fields=fields, order=order, domain=domain,
+                         bind_key=bind_key)
+
+    @XRay.capture(xray_recorder)
+    def kw(self, model: str, method: str = "search_read", *, id: int | None = None, fields: list[str] | None = None,
+           order: str | None = None, domain: list[tuple[str, str, t.Any]] | None = None, limit: int = 100,
+           page_size: int | None = None, page: int = 0, ensure_one: bool = False, bind_key: str | None = None):
         """Searches with API for records based on the args.
         
         See also: https://www.odoo.com/documentation/14.0/developer/reference/addons/orm.html#odoo.models.Model.search
         @param model: python as a dot separated class name.
         @param method : API method name maybe search_read, search_count
         @param id : id for one element
         @param fields: record fields for result.
         @param order: oder of result.
         @param domain: domain for records.
         @param limit: maximum number of records to return from odoo (default: all).
+        @param page_size: pagination done by the microservice.
         @param page: current page searched.
         @param ensure_one: raise error if result is not one (404) and only one (400) object.
-        @param bind: bind configuration to be used.
+        @param bind_key: bind configuration to be used.
 
         .. versionchanged:: 0.7.3
             Added the ``bind`` parameter.
        """
         if id and domain:
             raise BadRequest("Domain and Id parameters cannot be defined tin same time")
-        if page is not None and limit is None:
-            raise BadRequest("Pagination needs limit as page size.")
-
         if id:
-            domain = [[('id', '=', id)]]
+            filters = [[('id', '=', id)]]
         else:
-            domain = [domain] if domain else [[]]
+            filters = [domain] if domain else [[]]
 
-        params = {}
+        params: dict[str, t.Any] = {}
         if order:
             params.update({'order': order})
         if fields:
             params.update({'fields': fields})
         if limit:
             params.update({'limit': limit})
         if page:
-            params.update({'offset': page * limit})
+            page_size = page_size or limit
+            params.update({'offset': (page - 1) * page_size})
 
-        res = self.odoo_execute_kw(bind, model, method, domain, params)
+        res = self.odoo_execute_kw(model, method, filters, params, bind_key=bind_key)
 
         if method == 'search_count':
             return res
 
         if len(res) == 0:
             raise NotFound("No element found.")
         if ensure_one:
             if len(res) != 1:
                 raise NotFound("More than one element found and ensure_one parameters was set")
             return res[0]
 
         return {"ids": [rec['id'] for rec in res], "values": res}
 
     @XRay.capture(xray_recorder)
-    def create(self, model: str, data: t.Iterator[dict] = None, bind: str = None) -> int:
+    def create(self, model: str, data: list[dict] | None = None, bind_key: str | None = None) -> int:
         """Creates new records for the model.
 
         See also: https://www.odoo.com/documentation/14.0/developer/reference/addons/orm.html#odoo.models.Model.create
         @param model: python as a dot separated class name.
         @param data: fields, as a list of dictionaries, to initialize and the value to set on them.
-        @param bind: bind configuration to be used.
+        @param bind_key: bind configuration to be used.
         See also:
         https://www.odoo.com/documentation/14.0/developer/reference/addons/orm.html#odoo.models.Model.with_context
         """
-        return self.odoo_execute_kw(bind, model, "create", data)
+        return self.odoo_execute_kw(model, "create", data, bind_key=bind_key)
 
     @XRay.capture(xray_recorder)
-    def write(self, model: str, id: int, data: dict = None, bind: str = None) -> list:
+    def write(self, model: str, id: int, data: dict | None = None, bind_key: str | None = None) -> list:
         """Updates one record with the provided values.
         See also: https://www.odoo.com/documentation/14.0/developer/reference/addons/orm.html#odoo.models.Model.write
         @param model: python as a dot separated class name.
         @param id: id of the record.
         @param data: fields to update and the value to set on them.
-        @param bind: bind configuration to be used.
+        @param bind_key: bind configuration to be used.
         """
-        return self.odoo_execute_kw(bind, model, "write", [[id], data])
+        return self.odoo_execute_kw(model, "write", [[id], data], bind_key=bind_key)
 
     @XRay.capture(xray_recorder)
-    def delete_(self, model: str, id: int, bind: str = None) -> list:
+    def delete_(self, model: str, id: int, bind_key: str | None = None) -> list:
         """delete the record.
         See also: https://www.odoo.com/documentation/14.0/developer/reference/addons/orm.html#odoo.models.Model.unlink
         @param model: python as a dot separated class name.
         @param id: id of the record.
-        @param bind: bind configuration to be used.
+        @param bind_key: bind configuration to be used.
+        """
+        return self.odoo_execute_kw(model, "unlink", [[id]], bind_key=bind_key)
+
+    def get_pdf(self, invoice_id: int, access_token: str, bind_key: str | None = None) -> bytes:
+        """Returns the invoice as a PDF invoice.
+
+        @param invoice_id: invoice id.
+        @param access_token: access token of this invoice.
+        @param bind_key: bind configuration to be used.
         """
-        return self.odoo_execute_kw(bind, model, "unlink", [[id]])
+        config = self.binds[bind_key]
 
-    def get_pdf(self, report_id: int, rec_ids: t.Iterator[str], bind: str = None) -> bytes:
-        """Returns the PDF document attached to a report.
-        Specif entry to allow PDF base64 encoding with JSON_RPC.
-
-        @param report_id: id of the report record (ir.actions.report).
-        @param rec_ids: records needed to generate the report.
-        @param bind: bind configuration to be used.
-        """
-
-        config = self.binds[bind]
-        try:
-            headers = {'Content-type': 'application/json'}
-            data = {'jsonrpc': "2.0", 'params': {'db': config.dbname, 'login': config.user, 'password': config.passwd}}
-            res = requests.post(f'{config.url}/web/session/authenticate/', data=json.dumps(data), headers=headers)
-            result = res.json()
-            if result['result']['session_id']:
-                session_id = res.cookies["session_id"]
-                data = {'jsonrpc': "2.0", 'session_id': session_id}
-                params = {'params': {'res_ids': json.dumps(rec_ids)}}
-                try:
-                    res = requests.post(f"{config.url}/report/{report_id}", params=data, json=params)
-                    result = res.json()
-                    if 'error' in result:
-                        raise NotFound(f"{result['error']['message']}:{result['error']['data']}")
-                    return base64.b64decode(result['result'])
-                except NotFound:
-                    raise
-                except Exception:
-                    raise BadRequest(res.text)
-        except NotFound:
-            raise
-        except Exception:
-            raise Forbidden()
+        url = f"{config.url}/my/invoices/{invoice_id}/?report_type=pdf&download=true&access_token={access_token}"
+        resp = requests.get(url)
+        if resp.ok:
+            return resp.content
+        raise NotFound
 
-    def odoo_execute_kw(self, bind, model, method, *args, **kwargs):
+    def odoo_execute_kw(self, model, method, *args, bind_key: str | None = None, **kwargs):
         """Standard externalm API entries.
         See also: https://www.odoo.com/documentation/15.0/developer/misc/api/odoo.html
         """
-        config = self.binds[bind]
+        config = self.binds[bind_key]
 
         if '__uid' not in config.const:
             common = xmlrpc.client.ServerProxy(f'{config.url}/xmlrpc/2/common')
-            config.const['__uid'] = common.authenticate(config.dbname, config.user, config.passwd, {})
+            connected_uid = common.authenticate(config.dbname, config.user, config.passwd, {})
+            if not connected_uid:
+                raise ConnectionError()
+            config.const['__uid'] = connected_uid
 
         models = xmlrpc.client.ServerProxy(f'{config.url}/xmlrpc/2/object')
         return models.execute_kw(config.dbname, config.const['__uid'], config.passwd, model, method, *args, **kwargs)
```

### Comparing `coworks-0.9.2/coworks/extension/xray.py` & `coworks-0.9.3/coworks/extension/xray.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import traceback
 import typing as t
 from functools import partial
 from functools import update_wrapper
 
 from aws_xray_sdk import global_sdk_config
-from aws_xray_sdk.core import patch_all
+# from aws_xray_sdk.core import patch_all
 from aws_xray_sdk.core.exceptions.exceptions import SegmentNotFoundException
 from aws_xray_sdk.core.recorder import TRACING_NAME_KEY
 from aws_xray_sdk.ext.flask.middleware import XRayMiddleware
 
 from coworks.globals import request
 from coworks.wrappers import CoworksResponse
 
@@ -52,15 +52,15 @@
             # Checks XRay is available
             try:
                 self._recorder.current_segment()
             except SegmentNotFoundException:
                 pass
             else:
                 # Captures routes
-                patch_all()
+                # patch_all() # Bug in aws_xray if engine is defined by flask_sqlalchemy
                 app.errorhandler(500)(self.capture_exception)
                 self.capture_routes()
                 return
 
         self._app.logger.debug("Skipped capture routes because the SDK is currently disabled.")
 
     @staticmethod
@@ -149,30 +149,30 @@
                         subsegment.put_metadata('response', metadata, COWORKS_NAMESPACE)
                     except (Exception,):
                         pass
 
                 return response
 
             wrapped_fun = update_wrapper(partial(route_captured, view_function), view_function)
-            self._app.view_functions[rule.endpoint] = self._recorder.capture(name=wrapped_fun.__name__)(wrapped_fun)
+            fun_name = getattr(wrapped_fun, '__name__', 'wrapped_fun')
+            self._app.view_functions[rule.endpoint] = self._recorder.capture(name=fun_name)(wrapped_fun)
 
     def capture_exception(self, e):
+        self._app.logger.error(f"Event: {request.aws_event}")
+        self._app.logger.error(f"Context: {request.aws_context}")
         try:
             subsegment = self._recorder.current_subsegment()
             if subsegment:
                 subsegment.add_error_flag()
                 subsegment.put_annotation('service', self._app.name)
                 subsegment.add_exception(e, traceback.extract_stack())
-        except (SegmentNotFoundException,):
-            pass
-
-        self._app.logger.error(f"Event: {request.aws_event}")
-        self._app.logger.error(f"Context: {request.aws_context}")
-        self._app.logger.debug("Skipped capture exception because the SDK is currently disabled.")
-        raise e
+        except SegmentNotFoundException:
+            self._app.logger.debug("Skipped capture exception because the SDK is currently disabled.")
+        except Exception:
+            raise
 
 
 def lambda_context_to_json(context):
     return {
         'function_name': context.function_name,
         'function_version': context.function_version,
         'memory_limit_in_mb': context.memory_limit_in_mb,
```

### Comparing `coworks-0.9.2/coworks/tech/directory.py` & `coworks-0.9.3/coworks/tech/directory.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/coworks/utils.py` & `coworks-0.9.3/coworks/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 BIZ_BUCKET_HEADER_KEY: str = 'X-CWS-S3Bucket'
 BIZ_KEY_HEADER_KEY: str = 'X-CWS-S3Key'
 
 OPEN_SQUARE_BRACKETED_KWARG_PATTERN = re.compile(r'([a-zA-Z0-9]+)__')
 SQUARE_BRACKETED_KWARG_PATTERN = re.compile(r'([a-zA-Z0-9]+)__([a-zA-Z0-9._]+)__')
 
 
-def create_cws_proxy(scaffold: "Scaffold", func, func_args: list[str], func_kwargs: dict, func_generic_kwargs: str):
+def create_cws_proxy(scaffold: "Scaffold", func, func_args: list[str], func_kwargs: dict,
+                     func_generic_kwargs: str | None):
     """Creates the AWS Lambda proxy function.
 
     :param scaffold: The Flask or Blueprint object.
     :param func: The initial function proxied.
     :param func_args: The declared function args.
     :param func_kwargs: The declared function kwargs.
     :param func_generic_kwargs: The function generic kwargs if defined (usually **kwargs).
@@ -102,15 +103,15 @@
 
             # Adds parameters from query parameters
             if request.method == 'GET':
                 get_data = request.values.to_dict(False)
                 view_args = dict(**view_args, **as_fun_params(get_data))
 
             # Adds parameters from body
-            elif request.method in ['POST', 'PUT', 'DELETE']:
+            elif request.method in ['POST', 'PUT', 'PATCH', 'DELETE']:
                 try:
                     if request.is_json:
                         if request.data:
                             post_data = request.json
                             if not isinstance(post_data, dict):
                                 if len(func_kwargs) != 1:
                                     msg = f"If request payload is not a dict, there must be only one kwarg {type(post_data)}"
@@ -209,52 +210,53 @@
 def remove_brackets(name):
     """Removes brackets.
     Parameter like page[number] is passed to the function as page__number__."""
     return name.replace('[', '__').replace(']', '__')
 
 
 def as_typed_kwargs(func: t.Callable, kwargs: dict):
-    def get_typed_value(name: str, prameter_type, val):
-        if isinstance(prameter_type, types.UnionType):
-            for arg in t.get_args(prameter_type):
+    def get_typed_value(name: str, parameter_type, val):
+        if isinstance(parameter_type, types.UnionType):
+            for arg in t.get_args(parameter_type):
                 try:
                     return get_typed_value(name, arg, val)
                 except (UnprocessableEntity, ValidationError):
                     raise
                 except (TypeError, ValueError):
                     pass
             raise TypeError()
-        origin = t.get_origin(prameter_type)
+        origin = t.get_origin(parameter_type)
         if origin is t.Union:
-            for arg in t.get_args(prameter_type):
+            for arg in t.get_args(parameter_type):
                 return get_typed_value(name, arg, val)
             raise TypeError()
         if origin is list:
-            arg = t.get_args(prameter_type)[0]
+            arg = t.get_args(parameter_type)[0]
             if isinstance(val, list):
                 return [arg(v) for v in val]
             return [arg(val)]
         if origin is set:
-            arg = t.get_args(prameter_type)[0]
+            arg = t.get_args(parameter_type)[0]
             if isinstance(val, list):
                 return {arg(v) for v in val}
             return {arg(val)}
         if origin is None:
-            if prameter_type is Signature.empty:
+            if not parameter_type or parameter_type is Signature.empty:
                 return val
             if isinstance(val, list):
                 msg = f"Multiple values for '{name}' query parameters are not allowed"
                 raise UnprocessableEntity(msg)
-            if issubclass(prameter_type, bool):
+            if issubclass(parameter_type, bool):
                 return str_to_bool(val)
-            if issubclass(prameter_type, dict):
-                return json.loads(val)
-            if issubclass(prameter_type, BaseModel):
-                return prameter_type(**json.loads(val))
-            return val if isinstance(val, prameter_type) else prameter_type(val)
+            if issubclass(parameter_type, dict):
+                if isinstance(val, str):
+                    return json.loads(val)
+            if issubclass(parameter_type, BaseModel):
+                return parameter_type(**json.loads(val))
+            return val if isinstance(val, parameter_type) else parameter_type(val)
 
     typed_kwargs = {**kwargs}
     try:
         parameters = signature(func).parameters
         for name, value in kwargs.items():
             typed_kwargs[name] = get_typed_value(name, t.cast(Parameter, parameters.get(name)).annotation, value)
     except (UnprocessableEntity, ValidationError):
@@ -278,24 +280,25 @@
 
 
 def str_to_bool(val: str) -> bool:
     return val.lower() in ['true', '1', 'yes']
 
 
 def get_app_stage():
+    """Defined only on deployed microservice or should be set manually."""
     return os.getenv('CWS_STAGE', DEFAULT_DEV_STAGE)
 
 
-def load_dotenv(stage: str, as_dict: bool = False):
-    loaded = True
+def load_dotenv(stage: str):
+    values = {}
     for env_filename in get_env_filenames(stage):
         path = dotenv.find_dotenv(env_filename, usecwd=True)
         if path:
-            loaded = loaded and dotenv.load_dotenv(path, override=True)
-    return loaded
+            values.update(dotenv.dotenv_values(path))
+    return values
 
 
 def get_env_filenames(stage):
     return [".env", ".flaskenv", f".env.{stage}", f".flaskenv.{stage}"]
 
 
 def nr_url(path: str = '', query: dict | None = None, merge_query: bool = False):
```

### Comparing `coworks-0.9.2/coworks/wrappers.py` & `coworks-0.9.3/coworks/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 from werkzeug.exceptions import NotFound
 from werkzeug.routing import MapAdapter
 
 
 class TokenResponse:
     """AWS authorization response."""
 
-    def __init__(self, allow: bool, arn: str):
+    def __init__(self, allow: str | bool, arn: str):
         """Value may be string when allowed only if match workspace label."""
         self.allow = allow
         self.arn = arn
 
     @property
-    def json(self) -> t.Optional[t.Any]:
+    def json(self) -> dict:
         return {
             "principalId": "user",
             "policyDocument": {
                 "Version": "2012-10-17",
                 "Statement": [
                     {
                         "Action": "execute-api:Invoke",
```

### Comparing `coworks-0.9.2/pyproject.toml` & `coworks-0.9.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "coworks"
-version = "0.9.2"
+version = "0.9.3"
 description = "Coworks is a unified compositional microservices framework using Flask/Airflow on AWS serverless technologies."
 readme = "README.rst"
 requires-python = ">= 3.11"
 authors = [
     { name = "Guillaume Doumenc", email = "gdoumenc@fpr-coworks.com" },
 ]
 keywords = [
@@ -50,20 +50,21 @@
 Source = "https://github.com/gdoumenc/coworks"
 
 [project.scripts]
 cws = "coworks.cws.client:client"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "aws_xray_sdk>=2.12.1",
+    "aws_xray_sdk>=2.12",
     "boto3-stubs",
-    "mypy>=1.5.0",
-    "pytest>=7.4.0",
+    "mypy>=1.5",
+    "pytest>=7.4",
     "ruff>=0.0.284",
-    "sphinx>=7.1.2",
+    "sphinx>=7.1",
+    "sqlalchemy>=2.0",
 ]
 
 [tool.pdm.scripts.lint]
 cmd = "ruff coworks"
 help = "Linting using Ruff"
 
 [tool.pdm.scripts.typecheck]
@@ -96,17 +97,21 @@
 
 [tool.ruff.lint]
 ignore = [
     "F403",
 ]
 
 [tool.mypy]
-python_version = "3.11"
+python_version = ">=3.11"
+ignore_missing_imports = true
 exclude = [
     "biz",
+    "coworks/tech/directory.py",
+    "coworks/blueprint/mail_blueprint.py",
+    "coworks/blueprint/gsheets_blueprint.py",
 ]
 check_untyped_defs = true
 overrides = [
     { module = "requests_toolbelt.*", ignore_missing_imports = true },
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `coworks-0.9.2/tests/conftest.py` & `coworks-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/blueprint/blueprint.py` & `coworks-0.9.3/tests/coworks/blueprint/blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/blueprint/test_admin.py` & `coworks-0.9.3/tests/coworks/blueprint/test_admin.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/blueprint/test_blueprint.py` & `coworks-0.9.3/tests/coworks/blueprint/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/blueprint/test_empty.py` & `coworks-0.9.3/tests/coworks/blueprint/test_empty.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/blueprint/test_mail.py` & `coworks-0.9.3/tests/coworks/blueprint/test_mail.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/blueprint/test_overload.py` & `coworks-0.9.3/tests/coworks/blueprint/test_overload.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/event.py` & `coworks-0.9.3/tests/coworks/event.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/ms.py` & `coworks-0.9.3/tests/coworks/ms.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/tech/test_async.py` & `coworks-0.9.3/tests/coworks/tech/test_async.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/tech/test_auth.py` & `coworks-0.9.3/tests/coworks/tech/test_auth.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/tech/test_content_type.py` & `coworks-0.9.3/tests/coworks/tech/test_content_type.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/tech/test_event.py` & `coworks-0.9.3/tests/coworks/tech/test_event.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/tech/test_ms.py` & `coworks-0.9.3/tests/coworks/tech/test_ms.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/coworks/tech/test_type.py` & `coworks-0.9.3/tests/coworks/tech/test_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return "not ok", 400
 
     @entry
     def get_union(self, i: t.Union[int, int] = 0):
         return ("ok", 200) if type(i) is int else ("not ok", 400)
 
     @entry
-    def get_list(self, i: t.List[int] = 0):
+    def get_list(self, i: list[int] = 0):
         return ("ok", 200) if type(i) is list else ("not ok", 400)
 
     @entry
     def post(self, i: t.Union[int, int] = 0):
         return ("ok", 200) if type(i) is int else ("not ok", 400)
```

### Comparing `coworks-0.9.2/tests/cws/src/command.py` & `coworks-0.9.3/tests/cws/src/command.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/cws/test_cmd.py` & `coworks-0.9.3/tests/cws/test_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
         try:
             client.main(['--project-dir', '.', 'test', '--b', 'right'], 'cws', standalone_mode=False)
         finally:
             os.unsetenv("FLASK_RUN_FROM_CLI")
         captured = capsys.readouterr()
         assert captured.out == "test command with a=default/test command with b=right"
 
-    @mock.patch.dict(os.environ, {"CWS_STAGE": "v1", "FLASK_APP": "command:app"})
+    @mock.patch.dict(os.environ, {"FLASK_APP": "command:app"})
     def test_v1_cmd(self, example_dir, capsys):
-        client.main(['--project-dir', '.', 'test', '-a', 'right'], 'cws',
+        client.main(['--project-dir', '.', '-s', 'v1', 'test', '-a', 'right'], 'cws',
                     standalone_mode=False)
         captured = capsys.readouterr()
         assert captured.out == "test command v1 with a=right/test command v1 with b=value1"
```

### Comparing `coworks-0.9.2/tests/cws/test_deploy.py` & `coworks-0.9.3/tests/cws/test_deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import tempfile
-from pathlib import Path
+from pathlib import PosixPath
 from unittest import mock
 
 import boto3
 from flask.cli import ScriptInfo
 
 from coworks import Blueprint
 from coworks import TechMicroService
 from coworks import entry
-from coworks.cws.deploy import Terraform
-from coworks.cws.deploy import TerraformContext
 from coworks.cws.client import CwsScriptInfo
+from coworks.cws.deploy import Terraform
 from coworks.cws.deploy import TerraformBackend
+from coworks.cws.deploy import TerraformContext
 
 
 class CliCtxMokup:
+
+    def __init__(self, stage='dev'):
+        super().__init__()
+        self.params = {'project_dir': ".", 'stage': stage}
+
     def find_root(self):
         return self
 
-    @property
-    def params(self):
-        return {'project_dir': "."}
-
 
 class BP(Blueprint):
 
     @entry
     def get_test(self, index):
         return f"blueprint {self} {index}"
 
@@ -52,19 +53,19 @@
         return b"image content"
 
 
 class TestClass:
 
     def test_api_resources(self, example_dir, progressbar):
         app = TechMS()
-        with app.test_request_context() as ctx:
+        with app.test_request_context() as app_ctx:
             info = ScriptInfo(create_app=lambda: app)
-            terraform_context = TerraformContext(info, CliCtxMokup())
+            terraform_context = TerraformContext(info, CliCtxMokup(stage='dev'))
             backend = TerraformBackend(terraform_context, None, terraform_dir=".", terraform_refresh=False)
-            terraform = Terraform(backend, terraform_dir="terraform", stage="common")
+            terraform = Terraform(backend, terraform_dir="terraform", workspace="common")
             api_ressources = terraform.api_resources
         assert len(api_ressources) == 7
         assert api_ressources[''].rules is not None
         assert len(api_ressources[''].rules) == 1
         assert not api_ressources[''].rules[0].cws_binary_headers
         assert not api_ressources[''].rules[0].cws_no_auth
         assert len(api_ressources['img'].rules) == 1
@@ -76,19 +77,19 @@
         assert api_ressources['extended'].rules is None
 
     @mock.patch.dict(os.environ, {"test": "local", "FLASK_RUN_FROM_CLI": "true"})
     def test_deploy_ressources(self, example_dir, progressbar, capsys):
         info = CwsScriptInfo(project_dir='.')
         info.app_import_path = "command:app"
         app = info.load_app()
-        with app.test_request_context() as ctx:
+        with app.test_request_context() as app_ctx:
             info = ScriptInfo(create_app=lambda: app)
-            terraform_context = TerraformContext(info, CliCtxMokup())
+            terraform_context = TerraformContext(info, CliCtxMokup(stage='dev'))
             backend = TerraformBackend(terraform_context, None, terraform_dir=".", terraform_refresh=False)
-            terraform = Terraform(backend, terraform_dir="terraform", stage="common")
+            terraform = Terraform(backend, terraform_dir="terraform", workspace="common")
             api_ressources = terraform.api_resources
         assert len(api_ressources) == 5
         assert '' in api_ressources
         assert 'init' in api_ressources
         assert 'env' in api_ressources
         assert 'value' in api_ressources
         assert 'value_index' in api_ressources
@@ -98,54 +99,54 @@
         assert len(ter_resource.rules) == 2
 
     @mock.patch.dict(os.environ, {"test": "local", "FLASK_RUN_FROM_CLI": "true"})
     def test_deploy_local_cmd(self, monkeypatch, example_dir, progressbar, capsys):
         info = CwsScriptInfo(project_dir='.')
         info.app_import_path = "command:app"
         app = info.load_app()
-        with app.test_request_context() as ctx:
+        with app.test_request_context() as app_ctx:
             options = {
                 'project_dir': example_dir,
-                'workspace': 'workspace',
-                'debug': False,
+                'stage': 'dev',
                 'timeout': 30,
                 'memory_size': 100,
-                'deploy': True,
+                'terraform_dir': ".",
+                'terraform_refresh': False,
             }
             info = ScriptInfo(create_app=lambda: app)
             terraform_context = TerraformContext(info, CliCtxMokup())
-            backend = TerraformBackend(terraform_context, None, terraform_dir=".", terraform_refresh=False)
-            terraform = Terraform(backend, terraform_dir=Path("terraform"), stage="common")
+            backend = TerraformBackend(terraform_context, None, **options)
+            terraform = Terraform(backend, terraform_dir=PosixPath("terraform"), workspace="common")
             with tempfile.NamedTemporaryFile() as fp:
                 terraform.generate_file("deploy.j2", fp.name, **options)
                 fp.seek(0)
                 lines = fp.readlines()
                 assert len(lines) == 2049
                 assert lines[1].strip() == 'alias = "envtechms"'.encode('utf-8')
 
     @mock.patch.dict(os.environ, {"test": "local", "FLASK_RUN_FROM_CLI": "true"})
     def test_deploy_remote_cmd(self, monkeypatch, example_dir, progressbar, capsys):
         info = CwsScriptInfo(project_dir='.')
         info.app_import_path = "command:app"
         app = info.load_app()
-        with app.test_request_context() as ctx:
+        with app.test_request_context() as app_ctx:
             options = {
                 'project_dir': example_dir,
-                'workspace': 'workspace',
-                'debug': False,
+                'stage': 'dev',
                 'timeout': 30,
                 'memory_size': 100,
-                'deploy': True,
                 'terraform_cloud': True,
                 'terraform_organization': "CoWorks",
+                'terraform_dir': ".",
+                'terraform_refresh': False,
             }
             info = ScriptInfo(create_app=lambda: app)
             terraform_context = TerraformContext(info, CliCtxMokup())
-            backend = TerraformBackend(terraform_context, None, terraform_dir=".", terraform_refresh=False)
-            terraform = Terraform(backend, terraform_dir=Path("terraform"), stage="common")
+            backend = TerraformBackend(terraform_context, None, **options)
+            terraform = Terraform(backend, terraform_dir=PosixPath("terraform"), workspace="common")
             with tempfile.NamedTemporaryFile() as fp:
                 terraform.generate_file("terraform.j2", fp.name, **options)
                 fp.seek(0)
                 lines = fp.readlines()
                 assert len(lines) == 43
                 print(lines)
                 assert "TERRAFORM ON CLOUD" in lines[1].decode('utf-8')
@@ -153,26 +154,26 @@
 
     @mock.patch.dict(os.environ, {"test": "local", "FLASK_RUN_FROM_CLI": "true"})
     def test_destroy_cmd(self, monkeypatch, example_dir, progressbar, capsys):
         monkeypatch.setattr(boto3, "Session", mock.Mock(return_value=mock.Mock(return_value='region')))
         info = CwsScriptInfo(project_dir='.')
         info.app_import_path = "command:app"
         app = info.load_app()
-        with app.test_request_context() as ctx:
+        with app.test_request_context() as app_ctx:
             options = {
                 'project_dir': example_dir,
-                'workspace': 'workspace',
-                'debug': False,
+                'stage': 'dev',
                 'timeout': 30,
                 'memory_size': 100,
-                'deploy': False,
+                'terraform_dir': ".",
+                'terraform_refresh': False,
             }
             info = ScriptInfo(create_app=lambda: app)
             terraform_context = TerraformContext(info, CliCtxMokup())
-            backend = TerraformBackend(terraform_context, None, terraform_dir=".", terraform_refresh=False)
-            terraform = Terraform(backend, terraform_dir=Path("terraform"), stage="common")
+            backend = TerraformBackend(terraform_context, None, **options)
+            terraform = Terraform(backend, terraform_dir=PosixPath("terraform"), workspace="common")
             with tempfile.NamedTemporaryFile() as fp:
                 terraform.generate_file("deploy.j2", fp.name, **options)
                 fp.seek(0)
                 lines = fp.readlines()
                 assert len(lines) == 2049
                 assert lines[1].strip() == 'alias = "envtechms"'.encode('utf-8')
```

### Comparing `coworks-0.9.2/tests/cws/test_environment.py` & `coworks-0.9.3/tests/cws/test_environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,96 @@
 import multiprocessing
 import os
 import time
 from unittest import mock
 
-import pytest
 import requests
 from flask.cli import ScriptInfo
 
 from coworks.cws.client import client
+from coworks.utils import load_dotenv
 from tests.coworks.event import get_event
 from tests.cws.src.app import EnvTechMS
 
 
 class TestClass:
 
-    @mock.patch.dict(os.environ, {"CWS_STAGE": "no", "FLASK_RUN_FROM_CLI": "true"})
+    @mock.patch.dict(os.environ, {"FLASK_ENV_FILE": ".env.no", "FLASK_RUN_FROM_CLI": "true"})
     def test_no_env(self, example_dir, empty_aws_context):
-        os.environ.pop("STAGE")
-        with pytest.raises(AssertionError) as pytest_wrapped_e:
-            app = EnvTechMS()
-            event = get_event('/', 'get')
-            with app.cws_client(event, empty_aws_context) as c:
-                response = c.get('/', headers={'Authorization': 'token'})
-        assert pytest_wrapped_e.type == AssertionError
-        assert pytest_wrapped_e.value.args[0] == "no environment variable 'STAGE'"
+        app = EnvTechMS()
+        event = get_event('/', 'get')
+        with app.cws_client(event, empty_aws_context) as c:
+            response = c.get('/', headers={'Authorization': 'token'})
 
-    @mock.patch.dict(os.environ, {"CWS_STAGE": 'dev', "FLASK_RUN_FROM_CLI": "true"})
+    @mock.patch.dict(os.environ, {"FLASK_ENV_FILE": '.env.dev', "FLASK_RUN_FROM_CLI": "true"})
     def test_run_dev_env(self, example_dir, unused_tcp_port):
-        os.environ.pop('TEST', None)
         server = multiprocessing.Process(target=run_server, args=(example_dir, unused_tcp_port), daemon=True)
         server.start()
         counter = 1
         time.sleep(counter)
         while not server.is_alive() and counter < 3:
             time.sleep(counter)
             counter += 1
         response = requests.get(f'http://localhost:{unused_tcp_port}/env', headers={'Authorization': "token"})
         assert response.text == "Value of environment variable test is : test dev environment variable."
         server.terminate()
 
-    @mock.patch.dict(os.environ, {"CWS_STAGE": 'v1', "FLASK_RUN_FROM_CLI": "true"})
+    @mock.patch.dict(os.environ, {"FLASK_ENV_FILE": '.env.v1', "FLASK_RUN_FROM_CLI": "true"})
     def test_run_prod_env(self, example_dir, unused_tcp_port):
-        os.environ.pop('TEST', None)
         server = multiprocessing.Process(target=run_server, args=(example_dir, unused_tcp_port), daemon=True)
         server.start()
         counter = 1
         time.sleep(counter)
         while not server.is_alive() and counter < 3:
             time.sleep(counter)
             counter += 1
         response = requests.get(f'http://localhost:{unused_tcp_port}/env', headers={'Authorization': "token"})
         assert response.text == "Value of environment variable test is : test prod environment variable."
         server.terminate()
 
     def test_run_dev_stage(self, example_dir, unused_tcp_port):
-        os.environ.pop('TEST', None)
-        server = multiprocessing.Process(target=run_server_with_workspace,
+        server = multiprocessing.Process(target=run_server_with_stage,
                                          args=(example_dir, unused_tcp_port, "dev"),
                                          daemon=True)
         server.start()
         counter = 1
         time.sleep(counter)
         while not server.is_alive() and counter < 3:
             time.sleep(counter)
             counter += 1
         response = requests.get(f'http://localhost:{unused_tcp_port}/env', headers={'Authorization': "token"})
         assert response.text == "Value of environment variable test is : test dev environment variable."
         server.terminate()
 
     def test_run_prod_stage(self, example_dir, unused_tcp_port):
-        os.environ.pop('TEST', None)
-        server = multiprocessing.Process(target=run_server_with_workspace,
+        server = multiprocessing.Process(target=run_server_with_stage,
                                          args=(example_dir, unused_tcp_port, "v1"),
                                          daemon=True)
         server.start()
         counter = 1
         time.sleep(counter)
         while not server.is_alive() and counter < 3:
             time.sleep(counter)
             counter += 1
         response = requests.get(f'http://localhost:{unused_tcp_port}/env', headers={'Authorization': "token"})
         assert response.text == "Value of environment variable test is : test prod environment variable."
         server.terminate()
 
+    import pytest
+    @pytest.mark.wip
+    def test_load_env(self):
+        variables = load_dotenv("dev")
+        assert True
+
 
 def run_server(project_dir, port):
     obj = ScriptInfo(create_app=lambda: EnvTechMS(), set_debug_flag=False)
     client.main(['--project-dir', '.', 'run', '--port', port], 'cws', obj=obj, standalone_mode=False)
 
 
-def run_server_with_workspace(project_dir, port, workspace):
-    @mock.patch.dict(os.environ, {"CWS_STAGE": workspace, "FLASK_RUN_FROM_CLI": "true"})
+def run_server_with_stage(project_dir, port, stage):
+    @mock.patch.dict(os.environ, {"FLASK_ENV_FILE": f".env.{stage}", "FLASK_RUN_FROM_CLI": "true"})
     def run():
         obj = ScriptInfo(create_app=lambda: EnvTechMS(), set_debug_flag=False)
         client.main(['-p', '.', 'run', '--port', port], 'cws', obj=obj, standalone_mode=False)
 
     run()
```

### Comparing `coworks-0.9.2/tests/cws/test_project_file.py` & `coworks-0.9.3/tests/cws/test_project_file.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/docs/test_client.py` & `coworks-0.9.3/tests/docs/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 
     @mock.patch.dict(os.environ, {"FLASK_APP": "complete:app"})
     def test_routes_command(self, monkeypatch, samples_docs_dir):
         mclick = Mock()
         monkeypatch.setattr(click, "echo", mclick)
         client.main(['routes'], 'cws', standalone_mode=False)
         mclick.assert_called()
-        assert len(mclick.mock_calls) == 9
+        assert len(mclick.mock_calls) == 8
         out = [call.args[0].split(' ')[0] for call in mclick.mock_calls]
         assert 'Endpoint' in out
         assert 'admin.get_route' in out
         assert 'get' in out
         assert 'post' in out
```

### Comparing `coworks-0.9.2/tests/docs/test_complete.py` & `coworks-0.9.3/tests/docs/test_complete.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/tests/docs/test_first.py` & `coworks-0.9.3/tests/docs/test_first.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         server.start()
         counter = 1
         time.sleep(counter)
         while not server.is_alive() and counter < 10:
             time.sleep(counter)
             counter += 1
         response = requests.get(f'http://localhost:{unused_tcp_port}/')
-        assert response.status_code == 401
+        assert response.status_code == 403
         server.terminate()
 
     @mock.patch.dict(os.environ, {"FLASK_RUN_FROM_CLI": "false"})
     def test_run_first_wrong_token(self, samples_docs_dir, unused_tcp_port):
         info = CwsScriptInfo(project_dir='tech')
         info.app_import_path = "first:app"
         app = info.load_app()
```

### Comparing `coworks-0.9.2/tests/docs/test_hello.py` & `coworks-0.9.3/tests/docs/test_hello.py`

 * *Files identical despite different names*

### Comparing `coworks-0.9.2/PKG-INFO` & `coworks-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: coworks
-Version: 0.9.2
+Version: 0.9.3
 Summary: Coworks is a unified compositional microservices framework using Flask/Airflow on AWS serverless technologies.
-Keywords: python3 serverless microservice flask airflow aws-lambda aws
+Keywords: python3,serverless,microservice,flask,airflow,aws-lambda,aws
 Author-Email: Guillaume Doumenc <gdoumenc@fpr-coworks.com>
 License: MIT License
         
         Copyright (c) 2019 FPR-Coworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

