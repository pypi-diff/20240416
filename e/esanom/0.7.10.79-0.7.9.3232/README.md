# Comparing `tmp/esanom-0.7.10.79.tar.gz` & `tmp/esanom-0.7.9.3232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanom-0.7.10.79.tar", max compression
+gzip compressed data, was "esanom-0.7.9.3232.tar", max compression
```

## Comparing `esanom-0.7.10.79.tar` & `esanom-0.7.9.3232.tar`

### file list

```diff
@@ -1,194 +1,183 @@
--rw-r--r--   0        0        0        0 2024-04-16 16:45:49.080587 esanom-0.7.10.79/README.md
--rw-r--r--   0        0        0      144 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/CHANGELOG.txt
--rw-r--r--   0        0        0      388 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/COPYRIGHT.txt
--rw-r--r--   0        0        0    17260 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/LICENCE.txt
--rw-r--r--   0        0        0     1413 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/__init__.py
--rw-r--r--   0        0        0     6343 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/client.py
--rw-r--r--   0        0        0     5156 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/config.py
--rw-r--r--   0        0        0    44228 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/database.py
--rw-r--r--   0        0        0     1125 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/engine.py
--rw-r--r--   0        0        0     2496 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/monitor.py
--rw-r--r--   0        0        0    10303 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/orchestrator.py
--rw-r--r--   0        0        0    13068 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/pipeline.py
--rw-r--r--   0        0        0     1613 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/account.sql
--rw-r--r--   0        0        0     1828 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/api.sql
--rw-r--r--   0        0        0     1352 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/api_group.sql
--rw-r--r--   0        0        0     1326 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/api_role.sql
--rw-r--r--   0        0        0     1226 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/resources/database/claim.sql
--rw-r--r--   0        0        0     1215 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/group.sql
--rw-r--r--   0        0        0     1828 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/io.sql
--rw-r--r--   0        0        0     1416 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/ioblock.sql
--rw-r--r--   0        0        0     1596 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/log.sql
--rw-r--r--   0        0        0     1950 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/mpin.sql
--rw-r--r--   0        0        0     1921 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/mport.sql
--rw-r--r--   0        0        0     1536 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/pin.sql
--rw-r--r--   0        0        0     1842 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/pipeline.sql
--rw-r--r--   0        0        0     1514 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/pipeline_task.sql
--rw-r--r--   0        0        0     1501 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/port.sql
--rw-r--r--   0        0        0     1388 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/port_pin.sql
--rw-r--r--   0        0        0     1126 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/role.sql
--rw-r--r--   0        0        0     1250 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/roleadmin.sql
--rw-r--r--   0        0        0     1257 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/roledashboard.sql
--rw-r--r--   0        0        0     2173 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/rolemodel.sql
--rw-r--r--   0        0        0     1655 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/roleuser.sql
--rw-r--r--   0        0        0     1319 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/resources/database/schedule.sql
--rw-r--r--   0        0        0     1156 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/resources/database/session.sql
--rw-r--r--   0        0        0     1236 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/resources/database/system.sql
--rw-r--r--   0        0        0     1914 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/task.sql
--rw-r--r--   0        0        0     5741 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/triggers.sql
--rw-r--r--   0        0        0     1432 2024-04-16 16:45:49.516584 esanom-0.7.10.79/esanom/resources/database/unit.sql
--rw-r--r--   0        0        0    11022 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/roleadmin.py
--rw-r--r--   0        0        0     4208 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/rolemodel.py
--rw-r--r--   0        0        0     3456 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/roleuser.py
--rw-r--r--   0        0        0      790 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/__init__.py
--rw-r--r--   0        0        0    40600 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/api.py
--rw-r--r--   0        0        0     8676 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/common.py
--rw-r--r--   0        0        0    80721 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   232803 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/bootstrap.min.css
--rw-r--r--   0        0        0      639 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/dashboard.css
--rw-r--r--   0        0        0    20832 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/routes/v3/static/datatables.min.css
--rw-r--r--   0        0        0   197654 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/routes/v3/static/datatables.min.js
--rw-r--r--   0        0        0      318 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/favicon.ico
--rw-r--r--   0        0        0    48036 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/htmx.min.js
--rw-r--r--   0        0        0       97 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/main.css
--rw-r--r--   0        0        0      422 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/routes/v3/static/main.js
--rw-r--r--   0        0        0     1723 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/static/nom-logo.png
--rw-r--r--   0        0        0  3620840 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/routes/v3/static/plotly.min.js
--rw-r--r--   0        0        0     1741 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/routes/v3/static/theme.css
--rw-r--r--   0        0        0      717 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/admin_db_pipeline_row.html
--rw-r--r--   0        0        0      627 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/admin_db_pipeline_rows.html
--rw-r--r--   0        0        0     1542 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/base.html
--rw-r--r--   0        0        0     1000 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/db_rolemodel_row.html
--rw-r--r--   0        0        0      633 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/db_rolemodel_rows.html
--rw-r--r--   0        0        0      140 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/dummy.html
--rw-r--r--   0        0        0      153 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/error_404.html
--rw-r--r--   0        0        0      114 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/error_500.html
--rw-r--r--   0        0        0       82 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
--rw-r--r--   0        0        0      731 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_model_io.html
--rw-r--r--   0        0        0     1331 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_model_io_port.html
--rw-r--r--   0        0        0      808 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_models.html
--rw-r--r--   0        0        0      836 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_pipelines.html
--rw-r--r--   0        0        0     2019 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_debug.html
--rw-r--r--   0        0        0      149 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_loggedin_nav.html
--rw-r--r--   0        0        0      586 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
--rw-r--r--   0        0        0      197 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_loggedin_nav_member.html
--rw-r--r--   0        0        0      152 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_footer.html
--rw-r--r--   0        0        0      628 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_head.html
--rw-r--r--   0        0        0     1332 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_header.html
--rw-r--r--   0        0        0      173 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_header_logo.html
--rw-r--r--   0        0        0      487 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_header_nav.html
--rw-r--r--   0        0        0      240 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_header_toggle.html
--rw-r--r--   0        0        0      153 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/navigation.html
--rw-r--r--   0        0        0      327 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_admin_pipelines.html
--rw-r--r--   0        0        0      921 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_dashboard_tasks.html
--rw-r--r--   0        0        0      115 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_docs.html
--rw-r--r--   0        0        0      116 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_index.html
--rw-r--r--   0        0        0      121 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_interfaces.html
--rw-r--r--   0        0        0      516 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_model.html
--rw-r--r--   0        0        0      157 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/page_models.html
--rw-r--r--   0        0        0      128 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin/main.html
--rw-r--r--   0        0        0       94 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
--rw-r--r--   0        0        0     1381 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
--rw-r--r--   0        0        0      188 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_account_create/main.html
--rw-r--r--   0        0        0        5 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
--rw-r--r--   0        0        0      110 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
--rw-r--r--   0        0        0      429 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
--rw-r--r--   0        0        0      299 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
--rw-r--r--   0        0        0      315 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/main.html
--rw-r--r--   0        0        0      272 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/read.html
--rw-r--r--   0        0        0      114 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
--rw-r--r--   0        0        0      189 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
--rw-r--r--   0        0        0      207 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/update.html
--rw-r--r--   0        0        0     1641 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
--rw-r--r--   0        0        0      113 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
--rw-r--r--   0        0        0      544 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_read/main.html
--rw-r--r--   0        0        0        6 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
--rw-r--r--   0        0        0     1221 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
--rw-r--r--   0        0        0      474 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
--rw-r--r--   0        0        0      492 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_update/main.html
--rw-r--r--   0        0        0      421 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
--rw-r--r--   0        0        0      369 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
--rw-r--r--   0        0        0      241 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_apis/main.html
--rw-r--r--   0        0        0       94 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
--rw-r--r--   0        0        0      324 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
--rw-r--r--   0        0        0      263 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_create/main.html
--rw-r--r--   0        0        0      111 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
--rw-r--r--   0        0        0      278 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_read/main.html
--rw-r--r--   0        0        0        6 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
--rw-r--r--   0        0        0      718 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
--rw-r--r--   0        0        0      352 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_update/main.html
--rw-r--r--   0        0        0       87 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
--rw-r--r--   0        0        0      425 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_groups/main.html
--rw-r--r--   0        0        0      111 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
--rw-r--r--   0        0        0      332 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_model_read/main.html
--rw-r--r--   0        0        0       24 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
--rw-r--r--   0        0        0      897 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
--rw-r--r--   0        0        0      421 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_model_update/main.html
--rw-r--r--   0        0        0      425 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_models/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
--rw-r--r--   0        0        0      245 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_models/main.html
--rw-r--r--   0        0        0       40 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_settings/hx_form_system_mailer.html
--rw-r--r--   0        0        0      445 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_mailer.html
--rw-r--r--   0        0        0      199 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_settings/main.html
--rw-r--r--   0        0        0      640 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
--rw-r--r--   0        0        0     1218 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
--rw-r--r--   0        0        0       26 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
--rw-r--r--   0        0        0      770 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
--rw-r--r--   0        0        0      128 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/main.html
--rw-r--r--   0        0        0       60 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/login/hx_login.html
--rw-r--r--   0        0        0      672 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/login/main.html
--rw-r--r--   0        0        0      117 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/logout/main.html
--rw-r--r--   0        0        0      128 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member/main.html
--rw-r--r--   0        0        0      432 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
--rw-r--r--   0        0        0      792 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
--rw-r--r--   0        0        0      182 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_api_create/main.html
--rw-r--r--   0        0        0      347 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
--rw-r--r--   0        0        0      423 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/inc_table.html
--rw-r--r--   0        0        0      367 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
--rw-r--r--   0        0        0      416 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/main.html
--rw-r--r--   0        0        0      256 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/read.html
--rw-r--r--   0        0        0      129 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/update.html
--rw-r--r--   0        0        0      637 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
--rw-r--r--   0        0        0      428 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read.html
--rw-r--r--   0        0        0      160 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_info.html
--rw-r--r--   0        0        0     1331 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_port.html
--rw-r--r--   0        0        0     1331 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
--rw-r--r--   0        0        0      733 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_ports.html
--rw-r--r--   0        0        0      238 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/rows.html
--rw-r--r--   0        0        0      424 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/rows_inc_table.html
--rw-r--r--   0        0        0      607 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
--rw-r--r--   0        0        0      189 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/pins/read.html
--rw-r--r--   0        0        0       92 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/pins/read_inc_info.html
--rw-r--r--   0        0        0      234 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/pins/rows.html
--rw-r--r--   0        0        0      420 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
--rw-r--r--   0        0        0      339 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
--rw-r--r--   0        0        0      243 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/read.html
--rw-r--r--   0        0        0       92 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/read_inc_info.html
--rw-r--r--   0        0        0      422 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/read_inc_table.html
--rw-r--r--   0        0        0      163 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
--rw-r--r--   0        0        0      125 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
--rw-r--r--   0        0        0      236 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/rows.html
--rw-r--r--   0        0        0      422 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
--rw-r--r--   0        0        0      340 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-16 16:45:49.528584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
--rw-r--r--   0        0        0      270 2024-04-16 16:45:49.524584 esanom-0.7.10.79/esanom/routes/v3/templates/pages/register/main.html
--rw-r--r--   0        0        0    44388 2024-04-16 16:45:49.520584 esanom-0.7.10.79/esanom/routes/v3/web.py
--rw-r--r--   0        0        0     1693 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/sample_gunicorn_config.py
--rw-r--r--   0        0        0      753 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/sample_nom_config.json
--rw-r--r--   0        0        0     5050 2024-04-16 16:45:49.532584 esanom-0.7.10.79/esanom/scheduler.py
--rw-r--r--   0        0        0     3661 2024-04-16 16:45:49.536584 esanom-0.7.10.79/esanom/server.py
--rw-r--r--   0        0        0    12199 2024-04-16 16:45:49.536584 esanom-0.7.10.79/esanom/util.py
--rw-r--r--   0        0        0      443 2024-04-16 16:46:06.812498 esanom-0.7.10.79/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 esanom-0.7.10.79/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 16:37:06.484637 esanom-0.7.9.3232/README.md
+-rw-r--r--   0        0        0      144 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/CHANGELOG.txt
+-rw-r--r--   0        0        0      388 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/COPYRIGHT.txt
+-rw-r--r--   0        0        0    17260 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/LICENCE.txt
+-rw-r--r--   0        0        0     1412 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/__init__.py
+-rw-r--r--   0        0        0     6229 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/client.py
+-rw-r--r--   0        0        0     5123 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/config.py
+-rw-r--r--   0        0        0    43836 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/database.py
+-rw-r--r--   0        0        0     1125 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/engine.py
+-rw-r--r--   0        0        0     2496 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/monitor.py
+-rw-r--r--   0        0        0    10303 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/orchestrator.py
+-rw-r--r--   0        0        0    13068 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/pipeline.py
+-rw-r--r--   0        0        0     1613 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/account.sql
+-rw-r--r--   0        0        0     1828 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/api.sql
+-rw-r--r--   0        0        0     1352 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/api_group.sql
+-rw-r--r--   0        0        0     1326 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/api_role.sql
+-rw-r--r--   0        0        0     1226 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/resources/database/claim.sql
+-rw-r--r--   0        0        0     1131 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/group.sql
+-rw-r--r--   0        0        0     1828 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/io.sql
+-rw-r--r--   0        0        0     1416 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/ioblock.sql
+-rw-r--r--   0        0        0     1596 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/log.sql
+-rw-r--r--   0        0        0     1950 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/mpin.sql
+-rw-r--r--   0        0        0     1921 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/mport.sql
+-rw-r--r--   0        0        0     1451 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/pin.sql
+-rw-r--r--   0        0        0     1842 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/pipeline.sql
+-rw-r--r--   0        0        0     1514 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/pipeline_task.sql
+-rw-r--r--   0        0        0     1501 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/port.sql
+-rw-r--r--   0        0        0     1388 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/port_pin.sql
+-rw-r--r--   0        0        0     1126 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/role.sql
+-rw-r--r--   0        0        0     1250 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/roleadmin.sql
+-rw-r--r--   0        0        0     1257 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/roledashboard.sql
+-rw-r--r--   0        0        0     2173 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/rolemodel.sql
+-rw-r--r--   0        0        0     1655 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/roleuser.sql
+-rw-r--r--   0        0        0     1319 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/schedule.sql
+-rw-r--r--   0        0        0     1156 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/session.sql
+-rw-r--r--   0        0        0     1236 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/system.sql
+-rw-r--r--   0        0        0     1914 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/task.sql
+-rw-r--r--   0        0        0     4725 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/triggers.sql
+-rw-r--r--   0        0        0     1432 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/unit.sql
+-rw-r--r--   0        0        0     9732 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/roleadmin.py
+-rw-r--r--   0        0        0    11371 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/roleadmin.py-bak1
+-rw-r--r--   0        0        0     4192 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/rolemodel.py
+-rw-r--r--   0        0        0     3456 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/roleuser.py
+-rw-r--r--   0        0        0      790 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/__init__.py
+-rw-r--r--   0        0        0    40473 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/api.py
+-rw-r--r--   0        0        0     8676 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/common.py
+-rw-r--r--   0        0        0    80721 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   232803 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.min.css
+-rw-r--r--   0        0        0      639 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/dashboard.css
+-rw-r--r--   0        0        0    20832 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.css
+-rw-r--r--   0        0        0   197654 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.js
+-rw-r--r--   0        0        0      318 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/favicon.ico
+-rw-r--r--   0        0        0    48036 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/htmx.min.js
+-rw-r--r--   0        0        0       97 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/main.css
+-rw-r--r--   0        0        0      422 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/main.js
+-rw-r--r--   0        0        0     1723 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/nom-logo.png
+-rw-r--r--   0        0        0  3620840 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/routes/v3/static/plotly.min.js
+-rw-r--r--   0        0        0     1741 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/theme.css
+-rw-r--r--   0        0        0      717 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_row.html
+-rw-r--r--   0        0        0      627 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_rows.html
+-rw-r--r--   0        0        0     1542 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/base.html
+-rw-r--r--   0        0        0     1000 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_row.html
+-rw-r--r--   0        0        0      633 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_rows.html
+-rw-r--r--   0        0        0      140 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/dummy.html
+-rw-r--r--   0        0        0      153 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/error_404.html
+-rw-r--r--   0        0        0      114 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/error_500.html
+-rw-r--r--   0        0        0       82 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
+-rw-r--r--   0        0        0      731 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io.html
+-rw-r--r--   0        0        0     1331 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io_port.html
+-rw-r--r--   0        0        0      808 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_models.html
+-rw-r--r--   0        0        0      836 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_pipelines.html
+-rw-r--r--   0        0        0     1827 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_debug.html
+-rw-r--r--   0        0        0      149 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav.html
+-rw-r--r--   0        0        0      586 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
+-rw-r--r--   0        0        0      197 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav_member.html
+-rw-r--r--   0        0        0      152 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_footer.html
+-rw-r--r--   0        0        0      628 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_head.html
+-rw-r--r--   0        0        0     1332 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header.html
+-rw-r--r--   0        0        0      173 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header_logo.html
+-rw-r--r--   0        0        0      487 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header_nav.html
+-rw-r--r--   0        0        0      240 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header_toggle.html
+-rw-r--r--   0        0        0      153 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/navigation.html
+-rw-r--r--   0        0        0      327 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_admin_pipelines.html
+-rw-r--r--   0        0        0      921 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_dashboard_tasks.html
+-rw-r--r--   0        0        0      115 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_docs.html
+-rw-r--r--   0        0        0      116 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_index.html
+-rw-r--r--   0        0        0      121 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_interfaces.html
+-rw-r--r--   0        0        0      516 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_model.html
+-rw-r--r--   0        0        0      157 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_models.html
+-rw-r--r--   0        0        0      128 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin/main.html
+-rw-r--r--   0        0        0       94 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
+-rw-r--r--   0        0        0     1381 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
+-rw-r--r--   0        0        0      188 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/main.html
+-rw-r--r--   0        0        0      110 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
+-rw-r--r--   0        0        0      429 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
+-rw-r--r--   0        0        0      336 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
+-rw-r--r--   0        0        0      315 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/main.html
+-rw-r--r--   0        0        0      113 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
+-rw-r--r--   0        0        0      544 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
+-rw-r--r--   0        0        0     1221 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
+-rw-r--r--   0        0        0      474 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
+-rw-r--r--   0        0        0      492 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/main.html
+-rw-r--r--   0        0        0      421 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
+-rw-r--r--   0        0        0      369 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
+-rw-r--r--   0        0        0      241 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/main.html
+-rw-r--r--   0        0        0       94 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
+-rw-r--r--   0        0        0      324 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
+-rw-r--r--   0        0        0      263 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_create/main.html
+-rw-r--r--   0        0        0      109 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
+-rw-r--r--   0        0        0      278 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
+-rw-r--r--   0        0        0      716 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
+-rw-r--r--   0        0        0      352 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/main.html
+-rw-r--r--   0        0        0       87 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
+-rw-r--r--   0        0        0      425 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
+-rw-r--r--   0        0        0      293 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
+-rw-r--r--   0        0        0      184 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/main.html
+-rw-r--r--   0        0        0      109 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
+-rw-r--r--   0        0        0      332 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_read/main.html
+-rw-r--r--   0        0        0       24 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
+-rw-r--r--   0        0        0      895 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
+-rw-r--r--   0        0        0      421 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/main.html
+-rw-r--r--   0        0        0      425 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/inc_table.html
+-rw-r--r--   0        0        0      364 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
+-rw-r--r--   0        0        0      184 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
+-rw-r--r--   0        0        0      245 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/main.html
+-rw-r--r--   0        0        0       40 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_settings/hx_form_system_mailer.html
+-rw-r--r--   0        0        0      445 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_mailer.html
+-rw-r--r--   0        0        0      199 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_settings/main.html
+-rw-r--r--   0        0        0      640 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
+-rw-r--r--   0        0        0     1218 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
+-rw-r--r--   0        0        0       26 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
+-rw-r--r--   0        0        0      770 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
+-rw-r--r--   0        0        0      128 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/main.html
+-rw-r--r--   0        0        0       60 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/login/hx_login.html
+-rw-r--r--   0        0        0      702 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/login/main.html
+-rw-r--r--   0        0        0      117 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/logout/main.html
+-rw-r--r--   0        0        0      128 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member/main.html
+-rw-r--r--   0        0        0      432 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
+-rw-r--r--   0        0        0      792 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
+-rw-r--r--   0        0        0      182 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/main.html
+-rw-r--r--   0        0        0      103 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
+-rw-r--r--   0        0        0      423 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_table.html
+-rw-r--r--   0        0        0      407 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
+-rw-r--r--   0        0        0      416 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/main.html
+-rw-r--r--   0        0        0      428 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read.html
+-rw-r--r--   0        0        0      160 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_info.html
+-rw-r--r--   0        0        0     1331 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html
+-rw-r--r--   0        0        0     1331 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
+-rw-r--r--   0        0        0      733 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_ports.html
+-rw-r--r--   0        0        0      238 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows.html
+-rw-r--r--   0        0        0      424 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table.html
+-rw-r--r--   0        0        0      607 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
+-rw-r--r--   0        0        0      189 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/read.html
+-rw-r--r--   0        0        0       92 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/read_inc_info.html
+-rw-r--r--   0        0        0      234 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows.html
+-rw-r--r--   0        0        0      420 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
+-rw-r--r--   0        0        0      337 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
+-rw-r--r--   0        0        0      243 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read.html
+-rw-r--r--   0        0        0       92 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_info.html
+-rw-r--r--   0        0        0      422 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_table.html
+-rw-r--r--   0        0        0      163 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
+-rw-r--r--   0        0        0      125 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
+-rw-r--r--   0        0        0      236 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows.html
+-rw-r--r--   0        0        0      422 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
+-rw-r--r--   0        0        0      340 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/register/main.html
+-rw-r--r--   0        0        0    39183 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/web.py
+-rw-r--r--   0        0        0     1693 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/sample_gunicorn_config.py
+-rw-r--r--   0        0        0      753 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/sample_nom_config.json
+-rw-r--r--   0        0        0     5050 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/scheduler.py
+-rw-r--r--   0        0        0     2887 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/server.py
+-rw-r--r--   0        0        0    12199 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/util.py
+-rw-r--r--   0        0        0      444 2024-04-15 16:37:23.952531 esanom-0.7.9.3232/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 esanom-0.7.9.3232/PKG-INFO
```

### Comparing `esanom-0.7.10.79/esanom/LICENCE.txt` & `esanom-0.7.9.3232/esanom/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/__init__.py` & `esanom-0.7.9.3232/esanom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # This file is subject to the terms and conditions defined in file 'LICENCE.txt', 
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 
-__version__ = "0.7.10"
+__version__ = "0.7.9"
 
 #####################################################################
 
 from importlib.metadata import version
 
 print( f"NoM v{version('esanom')} Copyright 2024 © European Space Agency. All rights reserved." )
```

### Comparing `esanom-0.7.10.79/esanom/client.py` & `esanom-0.7.9.3232/esanom/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,24 +214,19 @@
 
 def user_pipeline_await( pipeline ) :
 
     pipeline_name = pipeline.name
     t0=time.time()
 
     while not pipeline.done :
-        dt = int( time.time( ) - t0 )
+        dt=int(time.time()-t0)
         print( f"[{dt}] awaiting {pipeline_name}")
-        time.sleep( 5 )
+        time.sleep(1)
         pipeline = user_pipeline( pipeline_name )
 
-    if pipeline.done :
-        print( "PIPELINE DONE" )
-    else :
-        print( "PIPELINE NOT DONE" )
-
     return( pipeline )
 
 
 def user_pipeline_archive( pipeline_name ) :
 
     return( _roleuser.pipeline_archive( pipeline_name ) )
```

### Comparing `esanom-0.7.10.79/esanom/config.py` & `esanom-0.7.9.3232/esanom/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,15 @@
     config_fp = f"{NOM_CONFIG_PATH}"
     if not NOM_CONFIG_PATH.startswith( "/" ) :
         config_fp = f"{cwd_fp}/{NOM_CONFIG_PATH}"
 
     ####
 
     if load_from_filepath( config_fp ) == None : load_from_env( )
-    if "_load_from_env" not in DATA :
-        DATA[ "_load_from_env" ] = False 
-        DATA[ "_config_fp" ] = NOM_CONFIG_PATH
+    if "_load_from_env" not in DATA : DATA[ "_load_from_env" ] = False 
 
     ####
 
     DATA[ "_package_fp" ] = os.path.abspath( os.path.dirname( __file__ ) )
     DATA[ "_cwd_fp" ] = cwd_fp
     DATA[ "_time_created" ] = time.time( )
 
@@ -74,15 +72,15 @@
 
     config_init_default_boolean( "server_debug" )
     config_init_default_boolean( "server_security_lax" )
     config_init_default_boolean( "database_disable_init" )
 
     ####
 
-    #_util.print_debug( DATA )
+    _util.print_debug( DATA )
 
     return
 
 #####################################################################
 
 def config_init_default_boolean( k , v = False ) :
     global DATA
@@ -95,27 +93,26 @@
         DATA[ k ] = True
     else :
         DATA[ k ] = False
 
 #####################################################################
 
 def load_from_filepath( config_fp ) :
-
     global DATA
 
     if not os.path.isfile( config_fp ) :
-        print( f"CONFIG FILE NOT FOUND {config_fp=}" )
+        print( f"WARNING CONFIG FILE NOT FOUND {config_fp=}" )
         return( None )
 
     ####
 
     with open( config_fp ) as f :
         try :
             DATA = json.loads( f.read( ) )
-            print( f"CONFIG FILE FOUND {config_fp=}" )
+            print( f"Config loaded from file config_fp = {config_fp}" )
             return( True )
         except json.decoder.JSONDecodeError as e :
             print( f"ERROR JSONDecodeError {e.msg}" )
             sys.exit( 4 )
 
 
 def env_get( k ) :
@@ -148,18 +145,19 @@
         "fs_storage_path" : env_get( "NOM_CONFIG_FS_STORAGE_PATH" ),
         "database_disable_init" : env_get( "NOM_CONFIG_DATABASE_DISABLE_INIT" ),
         "server_debug" : env_get( "NOM_CONFIG_SERVER_DEBUG" ),
         "server_security_lax" : env_get( "NOM_CONFIG_SERVER_SECURITY_LAX" ) 
 
     }
 
-    print( "CONFIG loaded from ENV" )
+    print("CONFIG loaded from ENV")
 
     #_util.print_debug( DATA , "Config loaded from ENV" )
 
+
     #if db_host == None or db_port == None : return( None )
     #if db_user == None or db_passwd == None : return( None )
     #if db_database == None : return( None )
 
     #if admin_api_email == None : return( None )
 
     return
```

### Comparing `esanom-0.7.10.79/esanom/database.py` & `esanom-0.7.9.3232/esanom/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,18 @@
     if _config.DATA[ "database_disable_init" ] : return
 
     # FIXME TODO find a better way to detect that we don't want database init
     if _config.DATA[ "database" ][ "port" ].startswith( "_" ) : return
     if _config.DATA[ "database" ][ "host" ] == "" : return
 
     print( "ATTEMPT DB INIT" )
+    time.sleep(10)
 
     try :
         db = mysql.connect( **_config.DATA[ "database" ] )
-        db.autocommit = True
         cursor = db.cursor( )
     except Exception as e :
         print( f"database create_tables connect exception {e}" )
         sys.exit( 4 )
 
     ####
 
@@ -89,25 +89,24 @@
         ####
 
         with open( sql_fp , "r" ) as f : sql = f.read( )
 
         try :
 
             cursor.execute( sql )
-            #print(f"{sql_fp=}")
 
         except Error as err :
 
             cursor.close( )
             db.close( )
 
             # FIXME TODO check if this is "client" run and bypass database stuff
             # FIXME TODO keep account as first table to create otherwise it fails
             if err.errno == errorcode.ER_TABLE_EXISTS_ERROR and sql_file == "account" :
-                print( "DATABASE SETUP SKIPPING" )
+                #print( "DATABASE SETUP SKIPPING" )
                 return
 
             print( f"create_tables {sql_file} {err.msg}" )
             sys.exit( 4 )
 
         ####
 
@@ -118,15 +117,14 @@
 
     insert_fromdict( "system" , { "key" : "database/version" , "val_str" : version( "esanom" ) } )
 
     insert_fromdict( "system" , { "key" : "orchestrator/time" , "val_int" : 0 } )
     insert_fromdict( "system" , { "key" : "scheduler/time" , "val_int" : 0 } )
 
     insert_fromdict( "system" , { "key" : "system/mailer/token" } )
-    insert_fromdict( "system" , { "key" : "system/id" , "val_str" : "SPARC" } )
 
     print( "DB INIT OK" )
 
 #####################################################################
 
 def init_tables( ) :
 
@@ -1250,15 +1248,15 @@
             ####
 
             for unit_data in pin_data[ "units" ] :
                 default = 0
                 if not flag_unit_default_found :
                     default = 1
                     flag_unit_default_found = True
-                if "default" in pin_data : default = pin_data[ "default" ]
+                if "default" in pin_data : default = pin_data["default"]
                 unit_name = f"{unit_data['name']}"
                 insert_fromdict( "unit" , { "name" : unit_name , "pin_id" : pin_id , "default" : default , "visible" : 0 } )
 
 ####
 
 def handle_overrides( task_uid ) :
     #print( f"handle_overrides {task_uid=}" )
@@ -1266,15 +1264,15 @@
 
     rolemodel_id = task_row[ "rolemodel_id" ]
     mport_rows = db_query_select_rows( "SELECT * from mport where rolemodel_id=%s" , [ rolemodel_id ] )
 
     for mport_row in mport_rows :
         mpin_rows = db_query_select_rows( "SELECT * from mpin where mport_id=%s and override IS NOT NULL" , [ mport_row[ "id" ] ] )
         for mpin_row in mpin_rows :
-            io_row = db_query_select_row( "SELECT * from io where task_id=%s AND mpin_id=%s LIMIT 1" , [ task_row[ "id" ] , mpin_row[ "id" ] ] )
+            io_row = db_query_select_row( "SELECT * from io where task_id=%s AND mpin_id=%s LIMIT 1" , [ task_row["id"],mpin_row["id"] ] )
             if io_row is None : handle_override( task_row[ "id" ] , mpin_row[ "id" ] , mpin_row[ "override" ] )
 
 
 def handle_override( task_id , mpin_id , mpin_override ) :
 
     override_sections = mpin_override.split( "," )
 
@@ -1302,15 +1300,15 @@
         file_data = dumps( cmd_val )
         file_hash = sha256( file_data ).hexdigest( ) 
         file_path = _util.get_io_hash_filepath( file_hash )
         with open( file_path , "wb" ) as f : f.write( file_data )
         file_size = os.path.getsize( file_path )
         #dtype = type( cmd_val ).__name__ 
 
-        #print( f"{file_path=}" )
+        print(f"{file_path=}")
 
         ####
         # FIXME TODO handle if data is > than block limit (8MB)
 
         io_data = {
             "task_id" : task_id ,
             "mpin_id" : mpin_id ,
@@ -1381,19 +1379,16 @@
     ####
 
     if override_key == "pipeline_status" :
 
         pipeline_task_row = db_query_select_row( "SELECT * from pipeline_task WHERE task_id=%s OR next_task_id=%s LIMIT 1" , [ task_id , task_id ] )
         pipeline_row = db_query_select_row( "SELECT * from pipeline WHERE id=%s LIMIT 1" , [ pipeline_task_row[ "pipeline_id" ] ] )
 
-        task_row = db_query_select_row( "SELECT * from `task` WHERE `id`=%s LIMIT 1" , [ task_id ] )
-
-        system_row = db_query_select_row( "SELECT * from `system` WHERE `key`=%s LIMIT 1" , [ "system/id" ] )
-
-        dt=round(time.time()-task_row['created_at'].timestamp(),1)
-        msg = f"{system_row['val_str']} -> {pipeline_row['name']} -> {dt}s"
-        return( msg )
+        v = pipeline_row['name']
+        #print(f"{v=}")
+        return( v )
+        #return( pipeline_row[ "name" ] )
 
     return( None )
 
 ####
```

### Comparing `esanom-0.7.10.79/esanom/engine.py` & `esanom-0.7.9.3232/esanom/engine.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/monitor.py` & `esanom-0.7.9.3232/esanom/monitor.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/orchestrator.py` & `esanom-0.7.9.3232/esanom/orchestrator.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/pipeline.py` & `esanom-0.7.9.3232/esanom/pipeline.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/account.sql` & `esanom-0.7.9.3232/esanom/resources/database/account.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/api.sql` & `esanom-0.7.9.3232/esanom/resources/database/api.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/api_group.sql` & `esanom-0.7.9.3232/esanom/resources/database/api_group.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/api_role.sql` & `esanom-0.7.9.3232/esanom/resources/database/api_role.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/claim.sql` & `esanom-0.7.9.3232/esanom/resources/database/claim.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/group.sql` & `esanom-0.7.9.3232/esanom/resources/database/group.sql`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 CREATE TABLE `group` (
 
     `id` INT UNSIGNED NOT NULL AUTO_INCREMENT,
 
     `name` VARCHAR(255) NOT NULL CHECK (`name` <> ""),
     `description` VARCHAR(255) DEFAULT "",
     `enable` BOOLEAN DEFAULT 0,
-    `uid` varchar(255) NOT NULL CHECK (`uid` <> ""),
     
     PRIMARY KEY (`id`),
     
     UNIQUE KEY `name` (`name`),
-    UNIQUE KEY `uid` (`uid`) ,
     KEY `enable` (`enable`) 
 
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.10.79/esanom/resources/database/io.sql` & `esanom-0.7.9.3232/esanom/resources/database/io.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/ioblock.sql` & `esanom-0.7.9.3232/esanom/resources/database/ioblock.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/log.sql` & `esanom-0.7.9.3232/esanom/resources/database/log.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/mpin.sql` & `esanom-0.7.9.3232/esanom/resources/database/mpin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/mport.sql` & `esanom-0.7.9.3232/esanom/resources/database/mport.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/pin.sql` & `esanom-0.7.9.3232/esanom/resources/database/port.sql`

 * *Files 9% similar despite different names*

```diff
@@ -16,37 +16,35 @@
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 */
 
-CREATE TABLE `pin` (
+CREATE TABLE `port` (
 
     `id` int UNSIGNED NOT NULL AUTO_INCREMENT,
 
     `name` varchar(255) NOT NULL CHECK (`name` <> ""),
     `description` TEXT ,
     
     `visible` BOOLEAN DEFAULT 1,
     `rolemodel_id` INT UNSIGNED DEFAULT NULL,
-    
-    `type` varchar(255) DEFAULT "",
     `uid` varchar(255) NOT NULL CHECK (`uid` <> "") ,
 
     `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,
     `updated_at` DATETIME DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
 
     PRIMARY KEY (`id`) ,
 
     UNIQUE KEY `name` (`name`) ,
     UNIQUE KEY `uid` (`uid`) ,
 
     KEY `rolemodel_id` (`rolemodel_id`),
-    CONSTRAINT `pin_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
-
+    CONSTRAINT `port_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
+    
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.10.79/esanom/resources/database/pipeline.sql` & `esanom-0.7.9.3232/esanom/resources/database/pipeline.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/pipeline_task.sql` & `esanom-0.7.9.3232/esanom/resources/database/pipeline_task.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/port.sql` & `esanom-0.7.9.3232/esanom/resources/database/pin.sql`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 */
 
-CREATE TABLE `port` (
+CREATE TABLE `pin` (
 
     `id` int UNSIGNED NOT NULL AUTO_INCREMENT,
 
     `name` varchar(255) NOT NULL CHECK (`name` <> ""),
     `description` TEXT ,
     
     `visible` BOOLEAN DEFAULT 1,
     `rolemodel_id` INT UNSIGNED DEFAULT NULL,
-    `uid` varchar(255) NOT NULL CHECK (`uid` <> "") ,
+    
+    `type` varchar(255) DEFAULT "",
 
     `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,
     `updated_at` DATETIME DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
 
     PRIMARY KEY (`id`) ,
 
     UNIQUE KEY `name` (`name`) ,
-    UNIQUE KEY `uid` (`uid`) ,
 
     KEY `rolemodel_id` (`rolemodel_id`),
-    CONSTRAINT `port_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
-    
+    CONSTRAINT `pin_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
+
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.10.79/esanom/resources/database/port_pin.sql` & `esanom-0.7.9.3232/esanom/resources/database/port_pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/role.sql` & `esanom-0.7.9.3232/esanom/resources/database/role.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/roleadmin.sql` & `esanom-0.7.9.3232/esanom/resources/database/roleadmin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/roledashboard.sql` & `esanom-0.7.9.3232/esanom/resources/database/roledashboard.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/rolemodel.sql` & `esanom-0.7.9.3232/esanom/resources/database/rolemodel.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/roleuser.sql` & `esanom-0.7.9.3232/esanom/resources/database/roleuser.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/schedule.sql` & `esanom-0.7.9.3232/esanom/resources/database/schedule.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/session.sql` & `esanom-0.7.9.3232/esanom/resources/database/session.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/system.sql` & `esanom-0.7.9.3232/esanom/resources/database/system.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/task.sql` & `esanom-0.7.9.3232/esanom/resources/database/task.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/resources/database/triggers.sql` & `esanom-0.7.9.3232/esanom/resources/database/triggers.sql`

 * *Files 12% similar despite different names*

```diff
@@ -16,61 +16,36 @@
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 */
 
-
-CREATE TRIGGER group_insert BEFORE INSERT ON `group` FOR EACH ROW BEGIN
-
-    SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
-
-END ;
-
-/******************************************************************/
-
 CREATE TRIGGER account_insert BEFORE INSERT ON account FOR EACH ROW BEGIN
 
     IF ( NEW.email_confirmed = 1 ) THEN
         SET NEW.email_confirmsent_at = NOW( ) ;
         SET NEW.email_confirmed_at = NOW( ) ;
     END IF ;
 
     SET NEW.password = SHA2( NEW.password , 256 ) ;
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
-CREATE TRIGGER account_update BEFORE UPDATE ON account FOR EACH ROW BEGIN
-
-    IF NEW.password <> OLD.password THEN
-        SET NEW.password = SHA2( NEW.password , 256 ) ;
-    END IF ;
-
-END ;
-
 /******************************************************************/
 
 CREATE TRIGGER api_insert BEFORE INSERT ON api FOR EACH ROW BEGIN
 
     SET NEW.token = CONCAT( "NOM" , SUBSTRING( SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) , 4 , 64 ) ) ;
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
-CREATE TRIGGER api_update BEFORE UPDATE ON api FOR EACH ROW BEGIN
-
-    IF NEW.token <> OLD.token THEN
-        SET NEW.token = CONCAT( "NOM" , SUBSTRING( SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) , 4 , 64 ) ) ;
-    END IF ;
-
-END ;
-
 /******************************************************************/
 
 CREATE TRIGGER pipeline_insert BEFORE INSERT ON pipeline FOR EACH ROW BEGIN
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
@@ -179,19 +154,7 @@
 
 CREATE TRIGGER port_insert BEFORE INSERT ON port FOR EACH ROW BEGIN
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
-/******************************************************************/
-
-CREATE TRIGGER pin_insert BEFORE INSERT ON pin FOR EACH ROW BEGIN
-
-    SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
-
-END ;
-
-/**WARNING-DO-NOT-DB-INIT-GROUP-TRIGGERS-AT-THE-BOTTOM-WTF*********/
-
-
-
```

### Comparing `esanom-0.7.10.79/esanom/resources/database/unit.sql` & `esanom-0.7.9.3232/esanom/resources/database/unit.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/roleadmin.py` & `esanom-0.7.9.3232/esanom/roleadmin.py-bak1`

 * *Files 8% similar despite different names*

```diff
@@ -298,101 +298,125 @@
     delete_testdata( "group" )
 
     delete_testdata( "port" )
     delete_testdata( "pin" )
     delete_testdata( "unit" )
 
     ####
-
+    
     config = { }
 
-    # GROUPS
-    for i in range( 10 ) :
+    config[ "group_total" ] = 10
+
+    for i in range( config[ "group_total" ] ) :
         config[ f"group{i}_name" ] = _util.get_test_uid( postfix = f"{i}_GROUP" )
         row_data = { "name" : config[ f"group{i}_name" ] , "enable" : 1 }
         create( "group" , row_data )
 
     ####
 
-    # USERS
-    for i in range( 10 ) :
-        account_id = create( "account" , { "name" : _util.get_test_uid( postfix = f"{i}_USER" ) , "enable" : 1 , "email" :  f"nom_user_test{i}@sparc.space" , "password" : f"{i}_USER" , "email_confirmed" : 1 } )
+    test_models = [
+        "TESTNOTIFICATIONEMAIL_MODEL" ,
+        "TESTMATHINCREMENT_MODEL" ,
+        "TESTNOP_MODEL" , "TESTSLEEP_MODEL" , "TESTFAILURE_MODEL" ,
+        "TESTNAND_MODEL" , "TESTREBOUND_MODEL" ,"TESTXLSX_MODEL" ,"TESTPLOT_MODEL" ,
+        "TESTPILLOW_MODEL" , "TESTDATETIME_MODEL" ,
+        "TRAJECTORY_MODEL"
+    ]
+
+    for test_model in test_models :
+        options = {
+            "api" : { "name" : _util.get_test_uid( postfix = f"{test_model}" ) , "enable" : 1 } ,
+            "group" : [ config[ f"group0_name" ] ] 
+        } 
+        create_model( options )
+
+    ####
+
+    config[ "user_total" ] = 10
+    for i in range( config[ "user_total" ] ) :
+
+        api_email = f"nomserver_user_{i}@sparc.space"
         
         options = {
-            "api" : { "account_id" : account_id , "name" : _util.get_test_uid( postfix = f"{i}_USER" ) , "enable" : 1 } ,
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_USER" ) , "enable" : 1 , "email" : api_email } ,
             "group" : [ config[ f"group0_name" ] ] 
         } 
         create_user( options )
 
     ####
-    # MODELS
-    for i in range( 10 ) :
-        account_id = create( "account" , { "name" : _util.get_test_uid( postfix = f"{i}_MODEL" ) , "enable" : 1 , "email" :  f"nom_model_test{i}@sparc.space" , "password" : f"{i}_MODEL" , "email_confirmed" : 1 } )
-        
+
+    config[ "model_total" ] = 10
+    for i in range( config[ "model_total" ] ) :
         options = {
-            "api" : { "account_id" : account_id , "name" : _util.get_test_uid( postfix = f"{i}_MODEL" ) , "enable" : 1 } ,
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_MODEL" ) , "enable" : 1 } ,
             "group" : [ config[ f"group0_name" ] ] 
         } 
         create_model( options )
 
+    ####
 
-    # DASHBOARD (Single)
-    account_id = create( "account" , { "name" : _util.get_test_uid( postfix = f"0_DASHBOARD" ) , "enable" : 1 , "email" :  f"nom_dashboard_test0@sparc.space" , "password" : f"0_DASHBOARD" , "email_confirmed" : 1 } )
-    
-    options = {
-        "api" : { "account_id" : account_id , "name" : _util.get_test_uid( postfix = f"0_DASHBOARD" ) , "enable" : 1 } ,
-        "group" : [ ] ,
-        "role" : "dashboard"
-    } 
-    create_api_with_rolegroup( options )
+    config[ "admin_total" ] = 10
+    for i in range( config[ "admin_total" ] ) :
+        options = {
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_ADMIN" ) , "enable" : 1 } ,
+            "group" : [ ] ,
+            "role" : "admin"
+        } 
+        create_api_with_rolegroup( options )
 
+    ####
 
+    config[ "dashboard_total" ] = 10
+    for i in range( config[ "dashboard_total" ] ) :
+        options = {
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_DASHBOARD" ) , "enable" : 1 } ,
+            "group" : [ ] ,
+            "role" : "dashboard"
+        } 
+        create_api_with_rolegroup( options )
+
+    ####
 
     port_prefixes = [ ]
     for chi in range( 26 ) : port_prefixes.append( f"test_port_{chr(97+chi)}_")
 
-    ####
-
     data_rows_unit = [ ] 
     data_rows_port_pin = [ ] 
 
-    ####
-
     for port_prefix in port_prefixes :
 
         for i in range( 3 ) :
 
             port_name = f"{port_prefix}{i}"
             port_id = create( "port" , { "name" : port_name } )
             
             ####
 
             for j in range( 3 ) :
 
                 pin_name = f"{port_name}_pin_{j}"
-                pin_id = create( "pin" , { "name" : pin_name , "type" : "str" } )
+                pin_id = create( "pin" , { "name" : pin_name } )
 
                 ####
 
                 for k in range( 3 ) :
 
                     unit_default = 0
-                    #if k == 0 and j == 1 : unit_default = 1
                     if k == 0 : unit_default = 1
 
                     row_data = { "name" : f"{pin_name}_unit_{k}" , "pin_id" : pin_id , "default" : unit_default }
 
                     data_rows_unit.append( row_data )
 
                 ####
 
                 cardinal = j
-                #if i == 0 : cardinal = j
 
-                row_data = { "port_id" : port_id , "pin_id" : pin_id ,"cardinal" : cardinal }
+                row_data = { "port_id" : port_id , "pin_id" : pin_id , "cardinal" : cardinal }
                 data_rows_port_pin.append( row_data )
 
     ####
 
     create_bulk( "unit" , data_rows_unit )
     create_bulk( "port_pin" , data_rows_port_pin )
```

### Comparing `esanom-0.7.10.79/esanom/rolemodel.py` & `esanom-0.7.9.3232/esanom/rolemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     return( _util.request_get( "/model_state" ) )
 
 
 def specs( specs_in ) :
 
     res = _util.request_post( "/model_specs" , data = specs_in )
-    print(res)
     return( isinstance( res , dict ) )
 
 def model_pipeline( ) :
 
     model_schedule_messages = _util.request_get( "/model_schedule" )
     #print(model_schedule_messages)
 
@@ -62,15 +61,15 @@
     if model_claim_set_messages[ "claim_status" ] == "NO" : raise Exception( "claim_status NO" )
     ####
 
     claim_uid = model_claim_set_messages[ "claim_uid" ]
     for i in range( 6 ) :
         time.sleep( 5 )
         model_claim_get_messages = _util.request_post( "/model_claim_get" , params = { "claim_uid" : claim_uid } )
-        #_util.print_debug( model_claim_get_messages )
+        _util.print_debug( model_claim_get_messages )
         if model_claim_get_messages[ "claim_status" ] == "NO" : raise Exception( "claim_status NO" )
         if model_claim_get_messages[ "claim_status" ] == "YES" : break
         print(f"model_pipeline model_claim_get WAIT {i}/15")
 
     if model_claim_get_messages[ "claim_status" ] != "YES" :
         _util.request_post( "/model_claim_release" , params = { "claim_uid" : claim_uid } )
         raise Exception( "claim_status NO... Claim released." )
```

### Comparing `esanom-0.7.10.79/esanom/roleuser.py` & `esanom-0.7.9.3232/esanom/roleuser.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/__init__.py` & `esanom-0.7.9.3232/esanom/routes/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/api.py` & `esanom-0.7.9.3232/esanom/routes/v3/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,18 +288,15 @@
             "type" : request.json.get( "type" ) ,
             "user_api_ip_prefix" : request.json.get( "user_api_ip_prefix" , "127.,192.168.,172.,10." ) ,
             "user_api_email_postfix" : request.json.get( "user_api_email_postfix" , "sparc.gr,esa.int,aeronomie.be" ) ,
             "input_size_max" : request.json.get( "input_size_max" , 10485760 ) ,
             "ignore_pred_fail" : request.json.get( "ignore_pred_fail" ) ,
             "enable" : rolemodel_enable
         }
-        try :
-            rolemodel_id = _database.insert_fromdict( "rolemodel" , rolemodel_data )
-        except Exception as e :
-            return( _common.response_error( e_msg = f"verify specs {e}"  ) )
+        rolemodel_id = _database.insert_fromdict( "rolemodel" , rolemodel_data )
     else :
         if rolemodel_row[ "updateable" ] == 0 :
             if not _config.DATA[ "server_security_lax" ]  :
                 return( _common.response_error( e_msg = "not updateable"  ) )
         if json.loads( rolemodel_row[ "specs" ] ) == request.json : return( _common.response_default( ) )
         rolemodel_id = rolemodel_row[ "id" ]
         rolemodel_data = {
```

### Comparing `esanom-0.7.10.79/esanom/routes/v3/common.py` & `esanom-0.7.9.3232/esanom/routes/v3/common.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/bootstrap.bundle.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/bootstrap.min.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/dashboard.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/datatables.min.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/datatables.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/htmx.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/nom-logo.png` & `esanom-0.7.9.3232/esanom/routes/v3/static/nom-logo.png`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/plotly.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/plotly.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/static/theme.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/theme.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/admin_db_pipeline_row.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_row.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/admin_db_pipeline_rows.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/base.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/base.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/db_rolemodel_row.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_row.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/db_rolemodel_rows.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_model_io.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_model_io_port.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io_port.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_models.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_models.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_content_pipelines.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_debug.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_debug.html`

 * *Files 11% similar despite different names*

```diff
@@ -47,33 +47,19 @@
 <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
   <div class="offcanvas-header">
     <h5 class="offcanvas-title" id="offcanvasExampleLabel">DEBUG</h5>
     <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
   </div>
   <div class="offcanvas-body">
     <div>
-
-<div>
+<pre>
 benchmark={{_tdata["benchmark"]}}
-</div>
-
-
-
-{% if _tdata["is_fs_tmp"] %}
-{% set alert_name="danger" %}
-{% else %}
-{% set alert_name="success" %}
-{% endif %}
-<div class="alert alert-{{alert_name}}" role="alert">
 fs_storage_path={{_tdata["config_data"]["fs_storage_path"]}}
-</div>
-
-<div>
 _load_from_env={{_tdata["config_data"]["_load_from_env"]}}
-</div>
+</pre>
 
     </div>
 
 
   </div>
 </div>
```

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_loggedin_nav_admin.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav_admin.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_head.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_head.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/inc_page_header.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/page_dashboard_tasks.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/page_dashboard_tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/page_model.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/page_model.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 
-
+{% if tdata['row']['ip_update']==1 %}
+{% set ip_update_checked='checked' %}
+{% else %}
+{% set ip_update_checked='' %}
+{% endif %}
 
 {% if tdata['row']['enable']==1 %}
 {% set enable_checked='checked' %}
 {% else %}
 {% set enable_checked='' %}
 {% endif %}
 
-{% if tdata['row']['email_confirmed']==1 %}
-{% set email_confirmed_checked='checked' %}
-{% else %}
-{% set email_confirmed_checked='' %}
-{% endif %}
-
-<form id="admin_accounts_update" hx-post="{{url_for('.hx_admin_accounts_update',uid=tdata['row']['uid'])}}" hx-target="#hx-results">
+<form hx-post="{{url_for('.hx_admin_api_update',api_uid=tdata['row']['uid'])}}" hx-target="#hx-results">
 
 
     <div class="mb-3">
-        <label for="form_email" class="form-label">Email</label>
-        <input type="email" class="form-control" id="form_email" name="email" value="{{tdata['row']['email']}}">
-    </div>
-
-    <div class="mb-3">
-        <label for="form_password" class="form-label">Password</label>
-        <input type="password" class="form-control" id="form_password" name="[password]">
-    </div>
-
-    <div class="mb-3">
-        <label for="form_name" class="form-label">Name</label>
-        <input class="form-control" id="form_name" name="name" value="{{tdata['row']['name']}}">
+        <label for="form_ip" class="form-label">ip</label>
+        <input class="form-control" id="form_ip" name="ip" value="{{tdata['row']['ip']}}">
     </div>
 
     <div class="form-check">
-        <input class="form-check-input" type="checkbox" value="1" id="account_enable" name="[enable]" {{enable_checked}}>
-        <label class="form-check-label" for="account_enable">Enable</label>
+        <input class="form-check-input" type="checkbox" value="1" id="ip_update" name="ip_update" {{ip_update_checked}}>
+        <label class="form-check-label" for="ip_update">ip_update</label>
     </div>
 
     <div class="form-check">
-        <input class="form-check-input" type="checkbox" value="1" id="account_email_confirmed" name="[email_confirmed]" {{email_confirmed_checked}}>
-        <label class="form-check-label" for="account_email_confirmed">Email confirmed</label>
+        <input class="form-check-input" type="checkbox" value="1" id="input_enable" name="enable" {{enable_checked}}>
+        <label class="form-check-label" for="input_enable">enable</label>
     </div>
 
+    {% if tdata["group_rows"]|length>0 %}
+    {% include( "pages/admin_api_update/inc_form_groups.html" ) %}
+    {% endif %}
+    
     <button type="submit" class="btn btn-primary">UPDATE</button>
 
 </form>
 
-<div id="hx-results"></div>
-
```

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_api_read/main.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_read/main.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 {% if tdata['row']['enable']==1 %}
 {% set enable_checked='checked' %}
 {% else %}
 {% set enable_checked='' %}
 {% endif %}
 
-<form hx-post="{{url_for('.hx_admin_group_update',uid=tdata['row']['uid'])}}" hx-target="#hx-results">
+<form hx-post="{{url_for('.hx_admin_group_update',id=tdata['row']['id'])}}" hx-target="#hx-results">
 
 
     <div class="mb-3">
         <label for="input_1" class="form-label">name</label>
         <input class="form-control" id="input_1" name="name" value="{{tdata['row']['name']}}">
     </div>
```

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 {% if tdata['row']['updateable']==1 %}
 {% set updateable_checked='checked' %}
 {% else %}
 {% set updateable_checked='' %}
 {% endif %}
 
-<form hx-post="{{url_for('.hx_admin_model_update',uid=tdata['row']['uid'])}}" hx-target="#hx-results">
+<form hx-post="{{url_for('.hx_admin_model_update',id=tdata['row']['id'])}}" hx-target="#hx-results">
 
 
     <div class="form-check">
         <input class="form-check-input" type="checkbox" value="1" id="input_2" name="enable" {{enable_checked}}>
         <label class="form-check-label" for="input_2">enable</label>
     </div>
```

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/member_api_create/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_port.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/read_inc_ports.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_ports.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/routes/v3/web.py` & `esanom-0.7.9.3232/esanom/routes/v3/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,31 +113,27 @@
 
     is_admin = False
     is_loggedin = False
     if session_data.get( "account_row" ) :
         is_loggedin = True
         is_admin = ( session_data["account_row"]["name"]=="_admin" )
 
-    is_fs_tmp = False
-    if _config.DATA["fs_storage_path"].startswith("/tmp/"): is_fs_tmp = True
-
     data = {
         "config_data" : _config.DATA ,
         "admin_account_email" : "".join(f"&#{ord(c)};" for c in _config.DATA[ "admin_account_email" ] ) ,
         "nom_version" : version( "esanom" ) ,
         "database_version" : system_databaseversion_row[ "val_str" ] ,
         "orchestrator_time_dt" : orchestrator_time_dt ,
         "scheduler_time_dt" : scheduler_time_dt ,
         "year" : datetime.now( ).strftime( "%Y" ) ,
         "flag_sampledata" : flag_sampledata ,
         "benchmark" : round( time.time( ) - _g._benchmark_before_request , 3 ) ,
         "session_data" : session_data ,
         "is_loggedin" : is_loggedin ,
-        "is_admin" : is_admin ,
-        "is_fs_tmp" : is_fs_tmp 
+        "is_admin" : is_admin 
     }
 
     #print(data)
 
     return( dict( _tdata = data ) )
 
 @ROUTES.app_template_global( "test" )
@@ -302,218 +298,26 @@
     return( render_template( "pages/pins/rows.html" , tdata = tdata ) )
 
 
 
 @ROUTES.route( "/pins_read" , methods = [ "GET" ] )
 def page_pins_read( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_str( "id" )
 
-    row = _database.db_query_select_row( "SELECT * from `pin` WHERE uid=%s LIMIT 1" , [ uid ] )
+    row = _database.db_query_select_row( "SELECT * from `pin` WHERE id=%s LIMIT 1" , [ id ] )
     if row == None : return( render_template( "error_500.html" ) )
 
     ####
 
     tdata = {
         "row" : row 
     }
 
     return( render_template( "pages/pins/read.html" , tdata = tdata ) )
-
-
-@ROUTES.route( "/member_apis_read" , methods = [ "GET" ] )
-def page_member_apis_read( ) :
-
-    uid = _common.request_arg_str( "uid" )
-
-    row = _database.db_query_select_row( "SELECT * from `api` WHERE uid=%s LIMIT 1" , [ uid ] )
-    if row == None : return( render_template( "error_500.html" ) )
-
-    ####
-
-    tdata = {
-        "row" : row 
-    }
-
-    return( render_template( "pages/member_apis/read.html" , tdata = tdata ) )
-
-
-@ROUTES.route( "/member_apis_update" , methods = [ "GET" ] )
-@_common.decorator_web_login_required( )
-def page_member_apis_update( ) :
-
-    uid = _common.request_arg_str( "uid" )
-
-    row = _database.db_query_select_row( "SELECT * from `api` WHERE uid=%s LIMIT 1" , [ uid ] )
-    if row is None : raise Exception( f"row None" )
-
-    tdata = {
-        "k1" : time.time( ) ,
-        "row" : row 
-    }
-
-    #print(tdata)
-
-    return( render_template( "pages/member_apis/update.html" , tdata = tdata ) )
-
-
-@ROUTES.route( "/hx_member_apis_update" , methods = [ "POST" ] )
-@_common.decorator_web_login_required( )
-def hx_member_apis_update( ) :
-
-    uid = _common.request_arg_str( "uid" )
-
-    # FIXME TODO check if id is available and allowed
-    #row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
-    #if row is None : raise Exception( f"row None" )
-
-    ####
-
-    form = request.form.to_dict( flat = False )
-    print(form)
-
-    ####
-    row_data = { }
-
-    for i , ( k , v ) in enumerate( form.items( ) ) :
-        if k.startswith("[") : continue
-        row_data[k]=v[0]
-
-
-    is_new_token=False
-    if "[new_token]" in form : 
-        row_data["token"]=""
-        is_new_token=True
-        print("NEW TOKEN")
-
-    #print(row_data)
-
-    _database.update_fromdict( "api" , uid , row_data , cid = "uid" )
-    ####
-
-    row = _database.db_query_select_row( "SELECT * from `api` WHERE uid=%s LIMIT 1" , [ uid ] )
-    if row is None : raise Exception( f"row None" )
-
-    tdata = {
-        "k1" : time.time( ) ,
-        "row" : row,
-        "is_new_token" : is_new_token
-    }
-
-    #print(tdata)
-
-    response = make_response( render_template( "pages/member_apis/hx_form.html" , tdata = tdata ) )
-
-    if not is_new_token :
-        response.headers[ "HX-Redirect" ] = url_for( ".page_member_apis_read" , uid = uid )
-
-    ####
-
-    return( response )
-
-####
-
-@ROUTES.route( "/admin_accounts_read" , methods = [ "GET" ] )
-def page_admin_accounts_read( ) :
-
-    uid = _common.request_arg_str( "uid" )
-
-    row = _database.db_query_select_row( "SELECT * from `account` WHERE uid=%s LIMIT 1" , [ uid ] )
-    if row == None : return( render_template( "error_500.html" ) )
-
-    ####
-
-    tdata = {
-        "row" : row 
-    }
-
-    return( render_template( "pages/admin_accounts/read.html" , tdata = tdata ) )
-
-
-@ROUTES.route( "/admin_accounts_update" , methods = [ "GET" ] )
-@_common.decorator_web_login_required( )
-def page_admin_accounts_update( ) :
-
-    uid = _common.request_arg_str( "uid" )
-
-    row = _database.db_query_select_row( "SELECT * from `account` WHERE uid=%s LIMIT 1" , [ uid ] )
-    if row is None : raise Exception( f"row None" )
-
-    tdata = {
-        "k1" : time.time( ) ,
-        "row" : row 
-    }
-
-    #print(tdata)
-
-    return( render_template( "pages/admin_accounts/update.html" , tdata = tdata ) )
-
-
-@ROUTES.route( "/hx_admin_accounts_update" , methods = [ "POST" ] )
-@_common.decorator_web_login_required( )
-def hx_admin_accounts_update( ) :
-
-    uid = _common.request_arg_str( "uid" )
-
-    # FIXME TODO check if id is available and allowed
-    #row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
-    #if row is None : raise Exception( f"row None" )
-
-    ####
-
-    form = request.form.to_dict( flat = False )
-    print(form)
-
-    ####
-    row_data = { }
-
-    for i , ( k , v ) in enumerate( form.items( ) ) :
-        if k.startswith("[") : continue
-        row_data[k]=v[0]
-
-
-    if "[enable]" in form : 
-        row_data[ "enable" ] = 1
-    else :
-        row_data[ "enable" ] = 0
-
-
-    if "[email_confirmed]" in form : 
-        row_data[ "email_confirmed" ] = 1
-    else :
-        row_data[ "email_confirmed" ] = 0
-
-
-    if form["[password]"][0]!="" : 
-        row_data[ "password" ] = form["[password]"][0]
-
-    #print(row_data)
-
-    _database.update_fromdict( "account" , uid , row_data , cid = "uid" )
-    ####
-
-    row = _database.db_query_select_row( "SELECT * from `account` WHERE uid=%s LIMIT 1" , [ uid ] )
-    if row is None : raise Exception( f"row None" )
-
-    tdata = {
-        "k1" : time.time( ) ,
-        "row" : row
-    }
-
-    #print(tdata)
-
-    response = make_response( render_template( "pages/admin_accounts/hx_form.html" , tdata = tdata ) )
-
-    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_accounts_read" , uid = uid )
-
-    ####
-
-    return( response )
-
-
 ####
 
 @ROUTES.route( "/docs" , methods = [ "GET" ] )
 def page_docs( ) :
     return( render_template( "page_docs.html" ) )
 
 
@@ -761,15 +565,15 @@
         "time" : time.time( ) ,
         "error_msgs" : error_msgs ,
         "id" : id
     }
 
     response = make_response( render_template( "pages/admin_group_create/hx_form.html" , tdata = tdata ) )
 
-    if len( error_msgs ) == 0 : response.headers[ "HX-Redirect" ] = url_for( ".page_admin_groups" )
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_groups" )
 
     return( response )
 
 
 @ROUTES.route( "/hx_admin_account_create" , methods = [ "POST" ] )
 @_common.decorator_web_login_required( "_admin" )
 def hx_admin_account_create( ) :
@@ -808,21 +612,15 @@
 
     tdata = {
         "time" : time.time( ) ,
         "error_msgs" : error_msgs ,
         "account_id" : account_id
     }
 
-    response = make_response( render_template( "pages/admin_account_create/hx_form.html" , tdata = tdata ) )
-
-    if len( error_msgs ) == 0 : response.headers[ "HX-Redirect" ] = url_for( ".page_admin_accounts"  )
-
-    return( response )
-
-
+    return( render_template( "pages/admin_account_create/hx_form.html" , tdata = tdata ) )
 
 
 @ROUTES.route( "/hx_dashboard_tasks_taskcount" , methods = [ "GET" ] )
 def hx_dashboard_tasks_taskcount( ) :
 
     task_rows = _database.db_query_select_rows( "SELECT * from task where done=%s" , [ 0 ] )
 
@@ -992,15 +790,15 @@
 
 @ROUTES.route( "/admin_models" , methods = [ "GET" ] )
 @_common.decorator_web_login_required( "_admin" )
 def page_admin_models( ) :
 
     rows = _database.db_query_select_rows( "SELECT * from `rolemodel`" )
 
-    columns = [ "uid" , "name" , "category" , "enable" , "updateable" ]
+    columns = [ "id" , "name" , "category" , "enable" , "updateable" ]
 
     tdata = {
         "k1" : time.time( ) ,
         "rows" : rows ,
         "columns" : columns
     }
 
@@ -1008,17 +806,17 @@
 
     return( render_template( "pages/admin_models/main.html" , tdata = tdata ) )
 
 @ROUTES.route( "/admin_model_read" , methods = [ "GET" ] )
 @_common.decorator_web_login_required( "_admin" )
 def page_admin_model_read( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_str( "id" )
 
-    row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE uid=%s LIMIT 1" , [ uid ] )
+    row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE id=%s LIMIT 1" , [id])
     if row is None : raise Exception( f"row None" )
 
     tdata = {
         "row" : row 
     }
 
     #print(tdata)
@@ -1026,17 +824,17 @@
     return( render_template( "pages/admin_model_read/main.html" , tdata = tdata ) )
 
 
 @ROUTES.route( "/admin_model_update" , methods = [ "GET" ] )
 @_common.decorator_web_login_required( "_admin" )
 def page_admin_model_update( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_str( "id" )
 
-    row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE uid=%s LIMIT 1" , [ uid ] )
+    row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE id=%s LIMIT 1" , [id])
     if row is None : raise Exception( f"row None" )
 
     tdata = {
         "k1" : time.time( ) ,
         "row" : row 
     }
 
@@ -1045,15 +843,15 @@
     return( render_template( "pages/admin_model_update/main.html" , tdata = tdata ) )
 
 
 @ROUTES.route( "/hx_admin_model_update" , methods = [ "POST" ] )
 @_common.decorator_web_login_required( "_admin" )
 def hx_admin_model_update( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_int( "id" )
 
     # FIXME TODO check if id is available and allowed
     #row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
     #if row is None : raise Exception( f"row None" )
 
     ####
 
@@ -1067,28 +865,28 @@
         if k.startswith("[") : continue
         row_data[k]=v[0]
 
 
     if "enable" not in row_data : row_data["enable"]=0
     if "updateable" not in row_data : row_data["updateable"]=0
 
-    #print(row_data)
+    print(row_data)
 
-    _database.update_fromdict( "rolemodel" , uid , row_data , cid = "uid" )
+    _database.update_fromdict( "rolemodel" , id , row_data )
     ####
 
     tdata = {
         "k1" : time.time( ) 
     }
 
     #print(tdata)
 
     response = make_response( render_template( "pages/admin_model_update/hx_form.html" , tdata = tdata ) )
 
-    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_model_read" , uid = uid )
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_model_read" , id=id)
 
     ####
 
     return( response )
 
 
 @ROUTES.route( "/admin_apis" , methods = [ "GET" ] )
@@ -1119,15 +917,15 @@
 
 
 @ROUTES.route( "/admin_groups" , methods = [ "GET" ] )
 @_common.decorator_web_login_required( "_admin" )
 def page_admin_groups( ) :
 
     rows = _database.db_query_select_rows( "SELECT * from `group`" )
-    columns = [ "uid" , "name" , "enable" ]
+    columns = [ "id" , "name" , "enable" ]
 
     tdata = {
         "k1" : time.time( ) ,
         "rows" : rows ,
         "columns" : columns
     }
 
@@ -1135,17 +933,17 @@
 
     return( render_template( "pages/admin_groups/main.html" , tdata = tdata ) )
 
 @ROUTES.route( "/admin_group_read" , methods = [ "GET" ] )
 @_common.decorator_web_login_required( "_admin" )
 def page_admin_group_read( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_str( "id" )
 
-    row = _database.db_query_select_row( "SELECT * from `group` WHERE uid=%s LIMIT 1" , [ uid ] )
+    row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
     if row is None : raise Exception( f"api_row None" )
 
     tdata = {
         "k1" : time.time( ) ,
         "row" : row 
     }
 
@@ -1216,17 +1014,17 @@
 
     return( render_template( "pages/admin_api_update/main.html" , tdata = tdata ) )
 
 @ROUTES.route( "/admin_group_update" , methods = [ "GET" ] )
 @_common.decorator_web_login_required( "_admin" )
 def page_admin_group_update( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_str( "id" )
 
-    row = _database.db_query_select_row( "SELECT * from `group` WHERE uid=%s LIMIT 1" , [ uid ] )
+    row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
     if row is None : raise Exception( f"api_row None" )
 
     tdata = {
         "k1" : time.time( ) ,
         "row" : row 
     }
 
@@ -1235,15 +1033,15 @@
     return( render_template( "pages/admin_group_update/main.html" , tdata = tdata ) )
 
 
 @ROUTES.route( "/hx_admin_group_update" , methods = [ "POST" ] )
 @_common.decorator_web_login_required( "_admin" )
 def hx_admin_group_update( ) :
 
-    uid = _common.request_arg_str( "uid" )
+    id = _common.request_arg_int( "id" )
 
     # FIXME TODO check if id is available and allowed
     #row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
     #if row is None : raise Exception( f"row None" )
 
 
     ####
@@ -1256,28 +1054,28 @@
 
     for i , ( k , v ) in enumerate( form.items( ) ) :
         if k.startswith("[") : continue
         row_data[k]=v[0]
 
     if "enable" not in row_data : row_data["enable"]=0
 
-    #print(row_data)
+    print(row_data)
 
-    _database.update_fromdict( "group" , uid , row_data , cid = "uid" )
+    _database.update_fromdict( "group" , id , row_data )
     ####
 
     tdata = {
         "k1" : time.time( ) 
     }
 
     #print(tdata)
 
     response = make_response( render_template( "pages/admin_group_update/hx_form.html" , tdata = tdata ) )
 
-    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_group_read" , uid = uid )
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_group_read" , id=id)
 
     ####
 
     return( response )
 
 @ROUTES.route( "/hx_admin_api_update" , methods = [ "POST" ] )
 @_common.decorator_web_login_required( "_admin" )
```

### Comparing `esanom-0.7.10.79/esanom/sample_gunicorn_config.py` & `esanom-0.7.9.3232/esanom/sample_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/sample_nom_config.json` & `esanom-0.7.9.3232/esanom/sample_nom_config.json`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/scheduler.py` & `esanom-0.7.9.3232/esanom/scheduler.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/esanom/util.py` & `esanom-0.7.9.3232/esanom/util.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.10.79/PKG-INFO` & `esanom-0.7.9.3232/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanom
-Version: 0.7.10.79
+Version: 0.7.9.3232
 Summary: ESANOM
 Author: Zafar Iqbal
 Author-email: zaf@sparc.space
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

