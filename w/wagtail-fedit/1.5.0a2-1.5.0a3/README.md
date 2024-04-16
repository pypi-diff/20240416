# Comparing `tmp/wagtail_fedit-1.5.0a2.tar.gz` & `tmp/wagtail_fedit-1.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.0a2.tar", last modified: Mon Apr 15 20:07:47 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.0a3.tar", last modified: Mon Apr 15 20:34:32 2024, max compression
```

## Comparing `wagtail_fedit-1.5.0a2.tar` & `wagtail_fedit-1.5.0a3.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.286973 wagtail_fedit-1.5.0a2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0    12405 2024-04-15 20:07:47.286973 wagtail_fedit-1.5.0a2/PKG-INFO
--rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.5.0a2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/pyproject.toml
--rw-rw-rw-   0        0        0     1188 2024-04-15 20:07:47.299069 wagtail_fedit-1.5.0a2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.155615 wagtail_fedit-1.5.0a2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.184056 wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     4259 2024-04-15 18:49:04.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     4335 2024-04-15 18:50:49.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     7692 2024-04-15 18:52:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.189285 wagtail_fedit-1.5.0a2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.101733 wagtail_fedit-1.5.0a2/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.102736 wagtail_fedit-1.5.0a2/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.191394 wagtail_fedit-1.5.0a2/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.192514 wagtail_fedit-1.5.0a2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.194063 wagtail_fedit-1.5.0a2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.113037 wagtail_fedit-1.5.0a2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.114461 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.198682 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4333 2024-04-15 18:17:44.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.199816 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    16149 2024-04-15 19:27:25.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.115783 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.120381 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.200684 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.205580 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      420 2024-04-15 18:48:24.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.210811 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.218678 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.222407 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.224922 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.227580 wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.231877 wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     9291 2024-04-15 18:55:47.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     6822 2024-04-15 20:06:24.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.234598 wagtail_fedit-1.5.0a2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.238331 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.243481 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.257246 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     7837 2024-04-15 19:13:02.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.262274 wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.270030 wagtail_fedit-1.5.0a2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6431 2024-04-15 20:07:37.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.285779 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:07:47.177105 wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12405 2024-04-15 20:07:47.000000 wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4043 2024-04-15 20:07:47.000000 wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 20:07:47.000000 wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-15 20:07:47.000000 wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 20:07:47.000000 wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:32.015576 wagtail_fedit-1.5.0a3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12405 2024-04-15 20:34:32.015576 wagtail_fedit-1.5.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.5.0a3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0     1188 2024-04-15 20:34:32.030370 wagtail_fedit-1.5.0a3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.836498 wagtail_fedit-1.5.0a3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.877892 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     4259 2024-04-15 18:49:04.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     4335 2024-04-15 18:50:49.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     7692 2024-04-15 18:52:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.882857 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.805600 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.806598 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.884903 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.886419 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.887431 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.808123 wagtail_fedit-1.5.0a3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.808123 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.890480 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4333 2024-04-15 18:17:44.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.891710 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    16149 2024-04-15 19:27:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.810667 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.813678 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.893838 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.898892 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      446 2024-04-15 20:27:28.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.903895 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.910463 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.914019 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.916445 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.918456 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.921515 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10146 2024-04-15 20:32:57.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7357 2024-04-15 20:32:51.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.923489 wagtail_fedit-1.5.0a3/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.929718 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.966436 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.975796 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     8976 2024-04-15 20:33:16.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.983270 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:32.000934 wagtail_fedit-1.5.0a3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6318 2024-04-15 20:34:05.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:32.013580 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.870339 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12405 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4089 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.0a2/LICENSE` & `wagtail_fedit-1.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/PKG-INFO` & `wagtail_fedit-1.5.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.0a2
+Version: 1.5.0a3
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.0a2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.0a3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.0a2/README.md` & `wagtail_fedit-1.5.0a3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/setup.cfg` & `wagtail_fedit-1.5.0a3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3061 320d 0a64 6573 6372 6970 7469 6f6e  0a2..description
+00000030: 3061 330d 0a64 6573 6372 6970 7469 6f6e  0a3..description
 00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
 00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
 00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/models.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,30 +1,33 @@
 magic:    0xa70d0d0a
-moddate:  0xb9731d66 (Mon Apr 15 18:36:41 2024 UTC)
-files sz: 6828
+moddate:  0xf38e1d66 (Mon Apr 15 20:32:51 2024 UTC)
+files sz: 7357
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 9
+   stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
       055a050100640064036c066d075a070100640064046c086d095a096d0a5a
-      0a0100640064056c086d0b5a0b0100640064066c0c6d0d5a0d0100640064
-      076c0e6d0f5a0f0100640064086c106d115a110100640064096c126d135a
-      1301006400640a6c145a14640b640c6c156d165a160100640b640d6c176d
-      185a186d195a196d1a5a1a6d1b5a1b0100640b640e6c1c6d1d5a1d010064
-      0b640f6c136d1e5a1e0100020065036a1f0000000000000000a6000000ab
-      0000000000000000005a2064105a2164115a220200470064128400641365
-      04a6030000ab0300000000000000005a236520a024000000000000000000
-      00000000000000000000006414ac15a6010000ab01000000000000000064
-      1665096417650a660464188404a6000000ab0000000000000000005a2564
-      19650d641a651a641b6526641c65276608641d84045a2864216416650964
-      1e6529652719000000000000000000641f65296527190000000000000000
-      00641c65266608642084055a2a640a5300
+      0a0100640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e0100640064066c0f6d
+      105a100100640064076c116d125a120100640064086c136d145a14010064
+      0064096c156d165a1601006400640a6c175a17640b640c6c186d195a1901
+      00640b640d6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640b640e6c
+      1f6d205a200100640b640f6c166d215a210100020065036a220000000000
+      000000a6000000ab0000000000000000005a2364105a2464115a25020047
+      006412840064136504a6030000ab0300000000000000005a266523a02700
+      000000000000000000000000000000000000006414ac15a6010000ab0100
+      000000000000006416650c6417650d660464188404a6000000ab00000000
+      00000000005a286426641a6510641b651d641c6529641d652a641e652b66
+      0a641f84055a2c6523a02d00000000000000000000000000000000000000
+      006420ac21a6010000ab010000000000000000641c6529641b651d641e65
+      2b660664228404a6000000ab0000000000000000005a2e64276416650c64
+      23652f652b190000000000000000006424652f652b190000000000000000
+      00641e65296608642584055a30640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -37,186 +40,215 @@
                 22 STORE_NAME               3 (library)
                 24 IMPORT_FROM              4 (Node)
                 26 STORE_NAME               4 (Node)
                 28 IMPORT_FROM              5 (TemplateSyntaxError)
                 30 STORE_NAME               5 (TemplateSyntaxError)
                 32 POP_TOP
    
-     3          34 LOAD_CONST               0 (0)
+     5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (('render_to_string',))
                 38 IMPORT_NAME              6 (django.template.loader)
                 40 IMPORT_FROM              7 (render_to_string)
                 42 STORE_NAME               7 (render_to_string)
                 44 POP_TOP
    
-     4          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('Parser', 'Token'))
-                50 IMPORT_NAME              8 (django.template.base)
-                52 IMPORT_FROM              9 (Parser)
-                54 STORE_NAME               9 (Parser)
-                56 IMPORT_FROM             10 (Token)
-                58 STORE_NAME              10 (Token)
+     6          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('make_context', 'Context'))
+                50 IMPORT_NAME              8 (django.template.context)
+                52 IMPORT_FROM              9 (make_context)
+                54 STORE_NAME               9 (make_context)
+                56 IMPORT_FROM             10 (Context)
+                58 STORE_NAME              10 (Context)
                 60 POP_TOP
    
-     5          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('FilterExpression',))
-                66 IMPORT_NAME              8 (django.template.base)
-                68 IMPORT_FROM             11 (FilterExpression)
-                70 STORE_NAME              11 (FilterExpression)
-                72 POP_TOP
-   
-     6          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               6 (('HttpRequest',))
-                78 IMPORT_NAME             12 (django.http)
-                80 IMPORT_FROM             13 (HttpRequest)
-                82 STORE_NAME              13 (HttpRequest)
-                84 POP_TOP
-   
-     7          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('reverse',))
-                90 IMPORT_NAME             14 (django.urls)
-                92 IMPORT_FROM             15 (reverse)
-                94 STORE_NAME              15 (reverse)
-                96 POP_TOP
-   
-     8          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               8 (('signing',))
-               102 IMPORT_NAME             16 (django.core)
-               104 IMPORT_FROM             17 (signing)
-               106 STORE_NAME              17 (signing)
-               108 POP_TOP
-   
-    10         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               9 (('hooks',))
-               114 IMPORT_NAME             18 (wagtail)
-               116 IMPORT_FROM             19 (hooks)
-               118 STORE_NAME              19 (hooks)
-               120 POP_TOP
-   
-    12         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST              10 (None)
-               126 IMPORT_NAME             20 (warnings)
-               128 STORE_NAME              20 (warnings)
-   
-    14         130 LOAD_CONST              11 (2)
-               132 LOAD_CONST              12 (('FeditAdapterEditButton',))
-               134 IMPORT_NAME             21 (toolbar)
-               136 IMPORT_FROM             22 (FeditAdapterEditButton)
-               138 STORE_NAME              22 (FeditAdapterEditButton)
-               140 POP_TOP
-   
-    17         142 LOAD_CONST              11 (2)
-               144 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
-               146 IMPORT_NAME             23 (adapters)
-               148 IMPORT_FROM             24 (adapter_registry)
-               150 STORE_NAME              24 (adapter_registry)
-               152 IMPORT_FROM             25 (RegistryLookUpError)
-               154 STORE_NAME              25 (RegistryLookUpError)
-               156 IMPORT_FROM             26 (BaseAdapter)
-               158 STORE_NAME              26 (BaseAdapter)
-               160 IMPORT_FROM             27 (AdapterError)
-               162 STORE_NAME              27 (AdapterError)
-               164 POP_TOP
-   
-    23         166 LOAD_CONST              11 (2)
-               168 LOAD_CONST              14 (('_can_edit',))
-               170 IMPORT_NAME             28 (utils)
-               172 IMPORT_FROM             29 (_can_edit)
-               174 STORE_NAME              29 (_can_edit)
-               176 POP_TOP
-   
-    26         178 LOAD_CONST              11 (2)
-               180 LOAD_CONST              15 (('CONSTRUCT_ADAPTER_TOOLBAR',))
-               182 IMPORT_NAME             19 (hooks)
-               184 IMPORT_FROM             30 (CONSTRUCT_ADAPTER_TOOLBAR)
-               186 STORE_NAME              30 (CONSTRUCT_ADAPTER_TOOLBAR)
-               188 POP_TOP
-   
-    31         190 PUSH_NULL
-               192 LOAD_NAME                3 (library)
-               194 LOAD_ATTR               31 (Library)
-               204 PRECALL                  0
-               208 CALL                     0
-               218 STORE_NAME              32 (register)
-   
-    34         220 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
-               222 STORE_NAME              33 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    35         224 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
-               226 STORE_NAME              34 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    39         228 PUSH_NULL
-               230 LOAD_BUILD_CLASS
-               232 LOAD_CONST              18 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 39>)
-               234 MAKE_FUNCTION            0
-               236 LOAD_CONST              19 ('AdapterNode')
-               238 LOAD_NAME                4 (Node)
-               240 PRECALL                  3
-               244 CALL                     3
-               254 STORE_NAME              35 (AdapterNode)
-   
-   116         256 LOAD_NAME               32 (register)
-               258 LOAD_METHOD             36 (tag)
-               280 LOAD_CONST              20 ('fedit')
-               282 KW_NAMES                21
-               284 PRECALL                  1
-               288 CALL                     1
-   
-   117         298 LOAD_CONST              22 ('parser')
-               300 LOAD_NAME                9 (Parser)
-               302 LOAD_CONST              23 ('token')
-               304 LOAD_NAME               10 (Token)
-               306 BUILD_TUPLE              4
-               308 LOAD_CONST              24 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 116>)
-               310 MAKE_FUNCTION            4 (annotations)
-   
-   116         312 PRECALL                  0
-               316 CALL                     0
-   
-   117         326 STORE_NAME              37 (do_render_fedit)
-   
-   155         328 LOAD_CONST              25 ('request')
-               330 LOAD_NAME               13 (HttpRequest)
-               332 LOAD_CONST              26 ('adapter')
-               334 LOAD_NAME               26 (BaseAdapter)
-               336 LOAD_CONST              27 ('context')
-               338 LOAD_NAME               38 (dict)
-               340 LOAD_CONST              28 ('return')
-               342 LOAD_NAME               39 (str)
-               344 BUILD_TUPLE              8
-               346 LOAD_CONST              29 (<code object wrap_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 155>)
-               348 MAKE_FUNCTION            4 (annotations)
-               350 STORE_NAME              40 (wrap_adapter)
-   
-   202         352 LOAD_CONST              33 ((None,))
-               354 LOAD_CONST              22 ('parser')
-               356 LOAD_NAME                9 (Parser)
-               358 LOAD_CONST              30 ('tokens')
-               360 LOAD_NAME               41 (list)
-               362 LOAD_NAME               39 (str)
-               364 BINARY_SUBSCR
-               374 LOAD_CONST              31 ('kwarg_list')
-               376 LOAD_NAME               41 (list)
-               378 LOAD_NAME               39 (str)
-               380 BINARY_SUBSCR
-               390 LOAD_CONST              28 ('return')
-               392 LOAD_NAME               38 (dict)
-               394 BUILD_TUPLE              8
-               396 LOAD_CONST              32 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 202>)
-               398 MAKE_FUNCTION            5 (defaults, annotations)
-               400 STORE_NAME              42 (get_kwargs)
-               402 LOAD_CONST              10 (None)
-               404 RETURN_VALUE
+    10          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               5 (('Parser', 'Token', 'FilterExpression'))
+                66 IMPORT_NAME             11 (django.template.base)
+                68 IMPORT_FROM             12 (Parser)
+                70 STORE_NAME              12 (Parser)
+                72 IMPORT_FROM             13 (Token)
+                74 STORE_NAME              13 (Token)
+                76 IMPORT_FROM             14 (FilterExpression)
+                78 STORE_NAME              14 (FilterExpression)
+                80 POP_TOP
+   
+    14          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('HttpRequest',))
+                86 IMPORT_NAME             15 (django.http)
+                88 IMPORT_FROM             16 (HttpRequest)
+                90 STORE_NAME              16 (HttpRequest)
+                92 POP_TOP
+   
+    15          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               7 (('reverse',))
+                98 IMPORT_NAME             17 (django.urls)
+               100 IMPORT_FROM             18 (reverse)
+               102 STORE_NAME              18 (reverse)
+               104 POP_TOP
+   
+    16         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               8 (('signing',))
+               110 IMPORT_NAME             19 (django.core)
+               112 IMPORT_FROM             20 (signing)
+               114 STORE_NAME              20 (signing)
+               116 POP_TOP
+   
+    18         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('hooks',))
+               122 IMPORT_NAME             21 (wagtail)
+               124 IMPORT_FROM             22 (hooks)
+               126 STORE_NAME              22 (hooks)
+               128 POP_TOP
+   
+    20         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              10 (None)
+               134 IMPORT_NAME             23 (warnings)
+               136 STORE_NAME              23 (warnings)
+   
+    22         138 LOAD_CONST              11 (2)
+               140 LOAD_CONST              12 (('FeditAdapterEditButton',))
+               142 IMPORT_NAME             24 (toolbar)
+               144 IMPORT_FROM             25 (FeditAdapterEditButton)
+               146 STORE_NAME              25 (FeditAdapterEditButton)
+               148 POP_TOP
+   
+    25         150 LOAD_CONST              11 (2)
+               152 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               154 IMPORT_NAME             26 (adapters)
+               156 IMPORT_FROM             27 (adapter_registry)
+               158 STORE_NAME              27 (adapter_registry)
+               160 IMPORT_FROM             28 (RegistryLookUpError)
+               162 STORE_NAME              28 (RegistryLookUpError)
+               164 IMPORT_FROM             29 (BaseAdapter)
+               166 STORE_NAME              29 (BaseAdapter)
+               168 IMPORT_FROM             30 (AdapterError)
+               170 STORE_NAME              30 (AdapterError)
+               172 POP_TOP
+   
+    31         174 LOAD_CONST              11 (2)
+               176 LOAD_CONST              14 (('_can_edit',))
+               178 IMPORT_NAME             31 (utils)
+               180 IMPORT_FROM             32 (_can_edit)
+               182 STORE_NAME              32 (_can_edit)
+               184 POP_TOP
+   
+    34         186 LOAD_CONST              11 (2)
+               188 LOAD_CONST              15 (('CONSTRUCT_ADAPTER_TOOLBAR',))
+               190 IMPORT_NAME             22 (hooks)
+               192 IMPORT_FROM             33 (CONSTRUCT_ADAPTER_TOOLBAR)
+               194 STORE_NAME              33 (CONSTRUCT_ADAPTER_TOOLBAR)
+               196 POP_TOP
+   
+    39         198 PUSH_NULL
+               200 LOAD_NAME                3 (library)
+               202 LOAD_ATTR               34 (Library)
+               212 PRECALL                  0
+               216 CALL                     0
+               226 STORE_NAME              35 (register)
+   
+    42         228 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
+               230 STORE_NAME              36 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    43         232 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
+               234 STORE_NAME              37 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    47         236 PUSH_NULL
+               238 LOAD_BUILD_CLASS
+               240 LOAD_CONST              18 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 47>)
+               242 MAKE_FUNCTION            0
+               244 LOAD_CONST              19 ('AdapterNode')
+               246 LOAD_NAME                4 (Node)
+               248 PRECALL                  3
+               252 CALL                     3
+               262 STORE_NAME              38 (AdapterNode)
+   
+   124         264 LOAD_NAME               35 (register)
+               266 LOAD_METHOD             39 (tag)
+               288 LOAD_CONST              20 ('fedit')
+               290 KW_NAMES                21
+               292 PRECALL                  1
+               296 CALL                     1
+   
+   125         306 LOAD_CONST              22 ('parser')
+               308 LOAD_NAME               12 (Parser)
+               310 LOAD_CONST              23 ('token')
+               312 LOAD_NAME               13 (Token)
+               314 BUILD_TUPLE              4
+               316 LOAD_CONST              24 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 124>)
+               318 MAKE_FUNCTION            4 (annotations)
+   
+   124         320 PRECALL                  0
+               324 CALL                     0
+   
+   125         334 STORE_NAME              40 (do_render_fedit)
+   
+   163         336 LOAD_CONST              38 ((False,))
+               338 LOAD_CONST              26 ('request')
+               340 LOAD_NAME               16 (HttpRequest)
+               342 LOAD_CONST              27 ('adapter')
+               344 LOAD_NAME               29 (BaseAdapter)
+               346 LOAD_CONST              28 ('context')
+               348 LOAD_NAME               41 (dict)
+               350 LOAD_CONST              29 ('run_context_processors')
+               352 LOAD_NAME               42 (bool)
+               354 LOAD_CONST              30 ('return')
+               356 LOAD_NAME               43 (str)
+               358 BUILD_TUPLE             10
+               360 LOAD_CONST              31 (<code object wrap_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 163>)
+               362 MAKE_FUNCTION            5 (defaults, annotations)
+               364 STORE_NAME              44 (wrap_adapter)
+   
+   204         366 LOAD_NAME               35 (register)
+               368 LOAD_METHOD             45 (simple_tag)
+               390 LOAD_CONST              32 (True)
+               392 KW_NAMES                33
+               394 PRECALL                  1
+               398 CALL                     1
+   
+   205         408 LOAD_CONST              28 ('context')
+               410 LOAD_NAME               41 (dict)
+               412 LOAD_CONST              27 ('adapter')
+               414 LOAD_NAME               29 (BaseAdapter)
+               416 LOAD_CONST              30 ('return')
+               418 LOAD_NAME               43 (str)
+               420 BUILD_TUPLE              6
+               422 LOAD_CONST              34 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 204>)
+               424 MAKE_FUNCTION            4 (annotations)
+   
+   204         426 PRECALL                  0
+               430 CALL                     0
+   
+   205         440 STORE_NAME              46 (render_adapter)
+   
+   221         442 LOAD_CONST              39 ((None,))
+               444 LOAD_CONST              22 ('parser')
+               446 LOAD_NAME               12 (Parser)
+               448 LOAD_CONST              35 ('tokens')
+               450 LOAD_NAME               47 (list)
+               452 LOAD_NAME               43 (str)
+               454 BINARY_SUBSCR
+               464 LOAD_CONST              36 ('kwarg_list')
+               466 LOAD_NAME               47 (list)
+               468 LOAD_NAME               43 (str)
+               470 BINARY_SUBSCR
+               480 LOAD_CONST              30 ('return')
+               482 LOAD_NAME               41 (dict)
+               484 BUILD_TUPLE              8
+               486 LOAD_CONST              37 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 221>)
+               488 MAKE_FUNCTION            5 (defaults, annotations)
+               490 STORE_NAME              48 (get_kwargs)
+               492 LOAD_CONST              10 (None)
+               494 RETURN_VALUE
    consts
       0
       ('Type',)
       ('library', 'Node', 'TemplateSyntaxError')
       ('render_to_string',)
-      ('Parser', 'Token')
-      ('FilterExpression',)
+      ('make_context', 'Context')
+      ('Parser', 'Token', 'FilterExpression')
       ('HttpRequest',)
       ('reverse',)
       ('signing',)
       ('hooks',)
       None
       2
       ('FeditAdapterEditButton',)
@@ -231,47 +263,47 @@
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564016506650719000000000000000000640265
             0864036509650a190000000000000000006606640484045a0b640584005a
             0c640684005a0d64075300
-          39           0 RESUME                   0
+          47           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          40          10 PUSH_NULL
+          48          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          42          40 LOAD_CONST               1 ('adapter')
+          50          40 LOAD_CONST               1 ('adapter')
                       42 LOAD_NAME                6 (Type)
                       44 LOAD_NAME                7 (BaseAdapter)
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('model')
                       58 LOAD_NAME                8 (FilterExpression)
                       60 LOAD_CONST               3 ('getters')
                       62 LOAD_NAME                9 (list)
                       64 LOAD_NAME               10 (str)
                       66 BINARY_SUBSCR
                       76 BUILD_TUPLE              6
-                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 42>)
+                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 50>)
                       80 MAKE_FUNCTION            4 (annotations)
                       82 STORE_NAME              11 (__init__)
          
-          48          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 48>)
+          56          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 56>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              12 (_resolve_expressions)
          
-          58          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 58>)
+          66          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 66>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              13 (render)
                       96 LOAD_CONST               7 (None)
                       98 RETURN_VALUE
          consts
             'AdapterNode'
             'adapter'
@@ -282,42 +314,42 @@
                nlocals   : 5
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c047c005f03000000000000000064
                   005300
-                42           0 RESUME                   0
+                50           0 RESUME                   0
                
-                43           2 LOAD_FAST                1 (adapter)
+                51           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                44          16 LOAD_FAST                2 (model)
+                52          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                45          30 LOAD_FAST                3 (getters)
+                53          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                46          44 LOAD_FAST                4 (kwargs)
+                54          44 LOAD_FAST                4 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                             58 LOAD_CONST               0 (None)
                             60 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs')
                varnames   ('self', 'adapter', 'model', 'getters', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 42
+               firstlineno 50
                lnotab 0x02010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -325,70 +357,70 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                48           0 RESUME                   0
+                56           0 RESUME                   0
                
-                49           2 LOAD_FAST                3 (kwargs)
+                57           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                50          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                58          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                51          94 LOAD_FAST                5 (v)
+                59          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                53     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                61     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                54         186 LOAD_FAST                2 (model)
+                62         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                56     >>  228 LOAD_FAST                2 (model)
+                64     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 48
+               firstlineno 56
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 8
                flags     : 3
                code
@@ -418,254 +450,254 @@
                   00ab0100000000000000007d0a02007c006a07000000000000000064097c
                   067c057c0a64089c037c04a4018e017d0b7c0ba015000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007210742d00
                   0000000000000000007c0a7c06a6020000ab02000000000000000073157c
                   0ba01700000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000053007431000000000000000000007c0a7c0b7c01a6
                   030000ab0300000000000000005300
-                58           0 RESUME                   0
+                66           0 RESUME                   0
                
-                59           2 LOAD_FAST                0 (self)
+                67           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                60          16 LOAD_FAST                0 (self)
+                68          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                62          30 PUSH_NULL
+                70          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                63          44 LOAD_FAST                1 (context)
+                71          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                62          48 BUILD_TUPLE              2
+                70          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                63          52 LOAD_FAST                0 (self)
+                71          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                62          64 DICT_MERGE               1
+                70          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                66          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                74          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
                             82 POP_JUMP_FORWARD_IF_FALSE    24 (to 132)
                
-                67          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                75          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    20 (to 132)
                
-                68          92 LOAD_FAST                2 (model)
+                76          92 LOAD_FAST                2 (model)
                
-                67          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
+                75          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
                
-                70          96 LOAD_FAST                1 (context)
+                78          96 LOAD_FAST                1 (context)
                             98 LOAD_CONST               1 ('wagtail_fedit_field')
                            100 BINARY_SUBSCR
                            110 STORE_FAST               5 (field_name)
                
-                71         112 LOAD_FAST                1 (context)
+                79         112 LOAD_FAST                1 (context)
                            114 LOAD_CONST               2 ('wagtail_fedit_instance')
                            116 BINARY_SUBSCR
                            126 STORE_FAST               6 (obj)
                            128 EXTENDED_ARG             1
                            130 JUMP_FORWARD           264 (to 660)
                
-                75     >>  132 LOAD_FAST                2 (model)
+                83     >>  132 LOAD_FAST                2 (model)
                            134 POP_JUMP_FORWARD_IF_TRUE   132 (to 400)
                
-                76         136 LOAD_GLOBAL              9 (NULL + warnings)
+                84         136 LOAD_GLOBAL              9 (NULL + warnings)
                            148 LOAD_ATTR                5 (warn)
                
-                77         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+                85         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-                78         170 LOAD_CONST               3 ('object')
+                86         170 LOAD_CONST               3 ('object')
                            172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                7 (adapter)
                            184 LOAD_ATTR                8 (__name__)
                
-                77         194 BUILD_MAP                1
+                85         194 BUILD_MAP                1
                            196 BINARY_OP                6 (%)
                
-                80         200 LOAD_GLOBAL             18 (RuntimeWarning)
+                88         200 LOAD_GLOBAL             18 (RuntimeWarning)
                
-                76         212 PRECALL                  2
+                84         212 PRECALL                  2
                            216 CALL                     2
                            226 POP_TOP
                
-                83         228 LOAD_FAST                1 (context)
+                91         228 LOAD_FAST                1 (context)
                            230 LOAD_METHOD             10 (flatten)
                            252 PRECALL                  0
                            256 CALL                     0
                            266 STORE_FAST               1 (context)
                
-                85         268 NOP
+                93         268 NOP
                
-                86         270 PUSH_NULL
+                94         270 PUSH_NULL
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                7 (adapter)
                            284 LOAD_ATTR               11 (render_from_kwargs)
                
-                87         294 LOAD_FAST                1 (context)
+                95         294 LOAD_FAST                1 (context)
                
-                86         296 BUILD_TUPLE              1
+                94         296 BUILD_TUPLE              1
                            298 BUILD_MAP                0
                
-                87         300 LOAD_FAST                4 (kwargs)
+                95         300 LOAD_FAST                4 (kwargs)
                
-                86         302 DICT_MERGE               1
+                94         302 DICT_MERGE               1
                            304 CALL_FUNCTION_EX         1
                            306 RETURN_VALUE
                        >>  308 PUSH_EXC_INFO
                
-                89         310 LOAD_GLOBAL             24 (AdapterError)
+                97         310 LOAD_GLOBAL             24 (AdapterError)
                            322 CHECK_EXC_MATCH
                            324 POP_JUMP_FORWARD_IF_FALSE    33 (to 392)
                            326 STORE_FAST               7 (e)
                
-                90         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
+                98         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
                            340 LOAD_GLOBAL             29 (NULL + str)
                            352 LOAD_FAST                7 (e)
                            354 PRECALL                  1
                            358 CALL                     1
                            368 PRECALL                  1
                            372 CALL                     1
                            382 RAISE_VARARGS            1
                        >>  384 LOAD_CONST               0 (None)
                            386 STORE_FAST               7 (e)
                            388 DELETE_FAST              7 (e)
                            390 RERAISE                  1
                
-                89     >>  392 RERAISE                  0
+                97     >>  392 RERAISE                  0
                        >>  394 COPY                     3
                            396 POP_EXCEPT
                            398 RERAISE                  1
                
-                92     >>  400 LOAD_FAST                3 (getters)
+               100     >>  400 LOAD_FAST                3 (getters)
                            402 LOAD_GLOBAL             31 (NULL + len)
                            414 LOAD_FAST                3 (getters)
                            416 PRECALL                  1
                            420 CALL                     1
                            430 LOAD_CONST               4 (1)
                            432 BINARY_OP               10 (-)
                            436 BINARY_SUBSCR
                            446 STORE_FAST               5 (field_name)
                
-                93         448 LOAD_FAST                2 (model)
+               101         448 LOAD_FAST                2 (model)
                            450 STORE_FAST               6 (obj)
                
-                94         452 LOAD_GLOBAL             33 (NULL + range)
+               102         452 LOAD_GLOBAL             33 (NULL + range)
                            464 LOAD_GLOBAL             31 (NULL + len)
                            476 LOAD_FAST                3 (getters)
                            478 PRECALL                  1
                            482 CALL                     1
                            492 LOAD_CONST               4 (1)
                            494 BINARY_OP               10 (-)
                            498 PRECALL                  1
                            502 CALL                     1
                            512 GET_ITER
                        >>  514 FOR_ITER                72 (to 660)
                            516 STORE_FAST               8 (i)
                
-                95         518 LOAD_FAST                3 (getters)
+               103         518 LOAD_FAST                3 (getters)
                            520 LOAD_FAST                8 (i)
                            522 BINARY_SUBSCR
                            532 STORE_FAST               9 (getter)
                
-                96         534 NOP
+               104         534 NOP
                
-                97         536 LOAD_GLOBAL             35 (NULL + getattr)
+               105         536 LOAD_GLOBAL             35 (NULL + getattr)
                            548 LOAD_FAST                6 (obj)
                            550 LOAD_FAST                9 (getter)
                            552 PRECALL                  2
                            556 CALL                     2
                            566 STORE_FAST               6 (obj)
                            568 JUMP_BACKWARD           28 (to 514)
                        >>  570 PUSH_EXC_INFO
                
-                98         572 LOAD_GLOBAL             36 (AttributeError)
+               106         572 LOAD_GLOBAL             36 (AttributeError)
                            584 CHECK_EXC_MATCH
                            586 POP_JUMP_FORWARD_IF_FALSE    32 (to 652)
                            588 POP_TOP
                
-                99         590 LOAD_GLOBAL             37 (NULL + AttributeError)
+               107         590 LOAD_GLOBAL             37 (NULL + AttributeError)
                            602 LOAD_CONST               5 ('Object ')
                            604 LOAD_FAST                2 (model)
                            606 LOAD_ATTR               19 (__class__)
                            616 LOAD_ATTR                8 (__name__)
                            626 FORMAT_VALUE             0
                            628 LOAD_CONST               6 (' does not have attribute ')
                            630 LOAD_FAST                9 (getter)
                            632 FORMAT_VALUE             0
                            634 BUILD_STRING             4
                            636 PRECALL                  1
                            640 CALL                     1
                            650 RAISE_VARARGS            1
                
-                98     >>  652 RERAISE                  0
+               106     >>  652 RERAISE                  0
                        >>  654 COPY                     3
                            656 POP_EXCEPT
                            658 RERAISE                  1
                
-               101     >>  660 LOAD_FAST                1 (context)
+               109     >>  660 LOAD_FAST                1 (context)
                            662 LOAD_METHOD             20 (get)
                            684 LOAD_CONST               7 ('request')
                            686 PRECALL                  1
                            690 CALL                     1
                            700 STORE_FAST              10 (request)
                
-               102         702 PUSH_NULL
+               110         702 PUSH_NULL
                            704 LOAD_FAST                0 (self)
                            706 LOAD_ATTR                7 (adapter)
                            716 LOAD_CONST               9 (())
                
-               103         718 LOAD_FAST                6 (obj)
+               111         718 LOAD_FAST                6 (obj)
                
-               104         720 LOAD_FAST                5 (field_name)
+               112         720 LOAD_FAST                5 (field_name)
                
-               105         722 LOAD_FAST               10 (request)
+               113         722 LOAD_FAST               10 (request)
                
-               102         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
+               110         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
                            726 BUILD_CONST_KEY_MAP      3
                
-               106         728 LOAD_FAST                4 (kwargs)
+               114         728 LOAD_FAST                4 (kwargs)
                
-               102         730 DICT_MERGE               1
+               110         730 DICT_MERGE               1
                            732 CALL_FUNCTION_EX         1
                            734 STORE_FAST              11 (adapter)
                
-               109         736 LOAD_FAST               11 (adapter)
+               117         736 LOAD_FAST               11 (adapter)
                            738 LOAD_METHOD             21 (check_permissions)
                            760 PRECALL                  0
                            764 CALL                     0
                            774 POP_JUMP_FORWARD_IF_FALSE    16 (to 808)
                
-               110         776 LOAD_GLOBAL             45 (NULL + _can_edit)
+               118         776 LOAD_GLOBAL             45 (NULL + _can_edit)
                            788 LOAD_FAST               10 (request)
                            790 LOAD_FAST                6 (obj)
                            792 PRECALL                  2
                            796 CALL                     2
                
-               109         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
+               117         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
                
-               111     >>  808 LOAD_FAST               11 (adapter)
+               119     >>  808 LOAD_FAST               11 (adapter)
                            810 LOAD_METHOD             23 (render_content)
                            832 LOAD_FAST                1 (context)
                            834 PRECALL                  1
                            838 CALL                     1
                            848 RETURN_VALUE
                
-               113     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
+               121     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
                            862 LOAD_FAST               10 (request)
                            864 LOAD_FAST               11 (adapter)
                            866 LOAD_FAST                1 (context)
                            868 PRECALL                  3
                            872 CALL                     3
                            882 RETURN_VALUE
                ExceptionTable:
@@ -688,28 +720,28 @@
                   ()
                names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 58
+               firstlineno 66
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff02031001140404
                   0116010c0118ff06030cfc100728020201180102ff040102ff0803120140
                   ff080330010401420110010201240112013eff08032a0110010201020102
                   fd040402fc060728011eff02022a02
             None
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 39
+         firstlineno 47
          lnotab 0x0a011e022c06060a
       'AdapterNode'
       'fedit'
       ('name',)
       'parser'
       'token'
       code
@@ -735,153 +767,153 @@
             00000000007c07a6010000ab01000000000000000064096b040000000072
             287c00a00700000000000000000000000000000000000000007c07a00100
             000000000000000000000000000000000000006401a6010000ab01000000
             0000000000a6010000ab0100000000000000007d06741100000000000000
             0000007c007c027c056a090000000000000000a6030000ab030000000000
             0000007d09741500000000000000000000640b7c057c067c07640a9c037c
             09a4018e015300
-         116           0 RESUME                   0
+         124           0 RESUME                   0
          
-         119           2 LOAD_FAST                1 (token)
+         127           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         121          42 LOAD_FAST                2 (tokens)
+         129          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         122          84 LOAD_FAST                2 (tokens)
+         130          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         124         126 NOP
+         132         126 NOP
          
-         125         128 LOAD_GLOBAL              4 (adapter_registry)
+         133         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         126         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         134         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         127         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         135         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         126     >>  214 RERAISE                  0
+         134     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         129     >>  222 LOAD_CONST               4 ((None, None))
+         137     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         130         232 LOAD_FAST                2 (tokens)
+         138         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   147 (to 530)
          
-         131         236 LOAD_FAST                2 (tokens)
+         139         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         132         278 LOAD_FAST                8 (model__field)
+         140         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         134         320 LOAD_GLOBAL             13 (NULL + len)
+         142         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    27 (to 412)
          
-         135         358 LOAD_FAST                7 (model_tokens)
+         143         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    15 (to 412)
          
-         136         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         144         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         137         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         145         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         136         396 PRECALL                  1
+         144         396 PRECALL                  1
                      400 CALL                     1
                      410 RAISE_VARARGS            1
          
-         140     >>  412 LOAD_GLOBAL             13 (NULL + len)
+         148     >>  412 LOAD_GLOBAL             13 (NULL + len)
                      424 LOAD_FAST                7 (model_tokens)
                      426 PRECALL                  1
                      430 CALL                     1
                      440 LOAD_CONST               9 (1)
                      442 COMPARE_OP               4 (>)
                      448 POP_JUMP_FORWARD_IF_FALSE    40 (to 530)
          
-         143         450 LOAD_FAST                0 (parser)
+         151         450 LOAD_FAST                0 (parser)
                      452 LOAD_METHOD              7 (compile_filter)
                      474 LOAD_FAST                7 (model_tokens)
                      476 LOAD_METHOD              1 (pop)
                      498 LOAD_CONST               1 (0)
                      500 PRECALL                  1
                      504 CALL                     1
                      514 PRECALL                  1
                      518 CALL                     1
                      528 STORE_FAST               6 (model)
          
-         145     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
+         153     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
                      542 LOAD_FAST                0 (parser)
                      544 LOAD_FAST                2 (tokens)
                      546 LOAD_FAST                5 (adapter)
                      548 LOAD_ATTR                9 (required_kwargs)
                      558 PRECALL                  3
                      562 CALL                     3
                      572 STORE_FAST               9 (kwargs)
          
-         147         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
+         155         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
                      586 LOAD_CONST              11 (())
          
-         148         588 LOAD_FAST                5 (adapter)
+         156         588 LOAD_FAST                5 (adapter)
          
-         149         590 LOAD_FAST                6 (model)
+         157         590 LOAD_FAST                6 (model)
          
-         150         592 LOAD_FAST                7 (model_tokens)
+         158         592 LOAD_FAST                7 (model_tokens)
          
-         147         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
+         155         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
                      596 BUILD_CONST_KEY_MAP      3
          
-         151         598 LOAD_FAST                9 (kwargs)
+         159         598 LOAD_FAST                9 (kwargs)
          
-         147         600 DICT_MERGE               1
+         155         600 DICT_MERGE               1
                      602 CALL_FUNCTION_EX         1
                      604 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
@@ -898,211 +930,187 @@
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 116
+         firstlineno 124
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a02260118
             010c0102ff1004260350022c020e010201020102fd040402fc
+      False
       'request'
       'adapter'
       'context'
+      'run_context_processors'
       'return'
       code
-         argcount  : 3
+         argcount  : 4
          nlocals   : 8
          stacksize : 13
          flags     : 3
          code
-            0x870097007c02730269007d027c016a0000000000000000007c0264013c
-            0000007c016a0100000000000000007c0264023c00000089007c0264033c
-            0000007c01a00200000000000000000000000000000000000000007c02a6
-            010000ab0100000000000000007d037c01a0030000000000000000000000
-            000000000000000000a6000000ab0000000000000000007d047409000000
-            00000000000000a6000000ab00000000000000000067017d05740b000000
-            000000000000006a060000000000000000740e00000000000000000000a6
-            010000ab01000000000000000044005d0f7d0602007c067c057c01ac04a6
-            020000ab02000000000000000001008c1088006601640584087c054400a6
-            000000ab0000000000000000007d05741100000000000000000000741300
-            00000000000000000064007c05a6020000ab020000000000000000a60100
-            00ab0100000000000000007d057c016a0a00000000000000007c016a0000
-            000000000000007c016a0100000000000000006a0b00000000000000006a
-            0c00000000000000007c016a0100000000000000006a0b00000000000000
-            006a0d00000000000000007c016a0100000000000000006a0e0000000000
-            00000064069c057d07741f0000000000000000000064077c016a0a000000
-            00000000007c037c017c057c047c016a1000000000000000007423000000
-            0000000000000064087c07ac09a6020000ab020000000000000000640a9c
-            078900ac0ba6030000ab0300000000000000005300
+            0x870097007c02730269007d02740100000000000000000000a6000000ab
+            00000000000000000067017d047403000000000000000000006a02000000
+            0000000000740600000000000000000000a6010000ab0100000000000000
+            0044005d0f7d0502007c057c047c01ac01a6020000ab0200000000000000
+            0001008c1088006601640284087c044400a6000000ab0000000000000000
+            007d04740900000000000000000000740b0000000000000000000064007c
+            04a6020000ab020000000000000000a6010000ab0100000000000000007d
+            047c016a0600000000000000007c016a0700000000000000007c016a0800
+            000000000000006a0900000000000000006a0a00000000000000007c016a
+            0800000000000000006a0900000000000000006a0b00000000000000007c
+            016a0800000000000000006a0c000000000000000064039c057d067c01a0
+            0d0000000000000000000000000000000000000000a6000000ab00000000
+            00000000007d07741d0000000000000000000064047c016a060000000000
+            0000007c017c047c077c016a0f00000000000000007c0274210000000000
+            000000000064057c06ac06a6020000ab02000000000000000064079c077c
+            03720289006e016400ac08a6030000ab0300000000000000005300
                        0 MAKE_CELL                0 (request)
          
-         155           2 RESUME                   0
+         163           2 RESUME                   0
          
-         156           4 LOAD_FAST                2 (context)
+         164           4 LOAD_FAST                2 (context)
                        6 POP_JUMP_FORWARD_IF_TRUE     2 (to 12)
          
-         157           8 BUILD_MAP                0
+         165           8 BUILD_MAP                0
                       10 STORE_FAST               2 (context)
          
-         159     >>   12 LOAD_FAST                1 (adapter)
-                      14 LOAD_ATTR                0 (field_name)
-                      24 LOAD_FAST                2 (context)
-                      26 LOAD_CONST               1 ('wagtail_fedit_field')
-                      28 STORE_SUBSCR
-         
-         160          32 LOAD_FAST                1 (adapter)
-                      34 LOAD_ATTR                1 (object)
-                      44 LOAD_FAST                2 (context)
-                      46 LOAD_CONST               2 ('wagtail_fedit_instance')
-                      48 STORE_SUBSCR
-         
-         161          52 LOAD_DEREF               0 (request)
-                      54 LOAD_FAST                2 (context)
-                      56 LOAD_CONST               3 ('request')
-                      58 STORE_SUBSCR
-         
-         163          62 LOAD_FAST                1 (adapter)
-                      64 LOAD_METHOD              2 (render_content)
-                      86 LOAD_FAST                2 (context)
-                      88 PRECALL                  1
-                      92 CALL                     1
-                     102 STORE_FAST               3 (content)
-         
-         164         104 LOAD_FAST                1 (adapter)
-                     106 LOAD_METHOD              3 (encode_shared_context)
-                     128 PRECALL                  0
-                     132 CALL                     0
-                     142 STORE_FAST               4 (shared)
-         
-         167         144 LOAD_GLOBAL              9 (NULL + FeditAdapterEditButton)
-                     156 PRECALL                  0
-                     160 CALL                     0
-         
-         166         170 BUILD_LIST               1
-                     172 STORE_FAST               5 (items)
-         
-         170         174 LOAD_GLOBAL             11 (NULL + hooks)
-                     186 LOAD_ATTR                6 (get_hooks)
-                     196 LOAD_GLOBAL             14 (CONSTRUCT_ADAPTER_TOOLBAR)
-                     208 PRECALL                  1
-                     212 CALL                     1
-                     222 GET_ITER
-                 >>  224 FOR_ITER                15 (to 256)
-                     226 STORE_FAST               6 (hook)
-         
-         171         228 PUSH_NULL
-                     230 LOAD_FAST                6 (hook)
-                     232 LOAD_FAST                5 (items)
-                     234 LOAD_FAST                1 (adapter)
-                     236 KW_NAMES                 4
-                     238 PRECALL                  2
-                     242 CALL                     2
-                     252 POP_TOP
-                     254 JUMP_BACKWARD           16 (to 224)
-         
-         173     >>  256 LOAD_CLOSURE             0 (request)
-                     258 BUILD_TUPLE              1
-                     260 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 173>)
-                     262 MAKE_FUNCTION            8 (closure)
-                     264 LOAD_FAST                5 (items)
-                     266 GET_ITER
-                     268 PRECALL                  0
-                     272 CALL                     0
-                     282 STORE_FAST               5 (items)
-         
-         174         284 LOAD_GLOBAL             17 (NULL + list)
-                     296 LOAD_GLOBAL             19 (NULL + filter)
-                     308 LOAD_CONST               0 (None)
-                     310 LOAD_FAST                5 (items)
-                     312 PRECALL                  2
-                     316 CALL                     2
-                     326 PRECALL                  1
-                     330 CALL                     1
-                     340 STORE_FAST               5 (items)
+         168     >>   12 LOAD_GLOBAL              1 (NULL + FeditAdapterEditButton)
+                      24 PRECALL                  0
+                      28 CALL                     0
+         
+         167          38 BUILD_LIST               1
+                      40 STORE_FAST               4 (items)
+         
+         171          42 LOAD_GLOBAL              3 (NULL + hooks)
+                      54 LOAD_ATTR                2 (get_hooks)
+                      64 LOAD_GLOBAL              6 (CONSTRUCT_ADAPTER_TOOLBAR)
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 GET_ITER
+                 >>   92 FOR_ITER                15 (to 124)
+                      94 STORE_FAST               5 (hook)
+         
+         172          96 PUSH_NULL
+                      98 LOAD_FAST                5 (hook)
+                     100 LOAD_FAST                4 (items)
+                     102 LOAD_FAST                1 (adapter)
+                     104 KW_NAMES                 1
+                     106 PRECALL                  2
+                     110 CALL                     2
+                     120 POP_TOP
+                     122 JUMP_BACKWARD           16 (to 92)
+         
+         174     >>  124 LOAD_CLOSURE             0 (request)
+                     126 BUILD_TUPLE              1
+                     128 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 174>)
+                     130 MAKE_FUNCTION            8 (closure)
+                     132 LOAD_FAST                4 (items)
+                     134 GET_ITER
+                     136 PRECALL                  0
+                     140 CALL                     0
+                     150 STORE_FAST               4 (items)
+         
+         175         152 LOAD_GLOBAL              9 (NULL + list)
+                     164 LOAD_GLOBAL             11 (NULL + filter)
+                     176 LOAD_CONST               0 (None)
+                     178 LOAD_FAST                4 (items)
+                     180 PRECALL                  2
+                     184 CALL                     2
+                     194 PRECALL                  1
+                     198 CALL                     1
+                     208 STORE_FAST               4 (items)
          
-         177         342 LOAD_FAST                1 (adapter)
-                     344 LOAD_ATTR               10 (identifier)
+         178         210 LOAD_FAST                1 (adapter)
+                     212 LOAD_ATTR                6 (identifier)
          
-         178         354 LOAD_FAST                1 (adapter)
-                     356 LOAD_ATTR                0 (field_name)
+         179         222 LOAD_FAST                1 (adapter)
+                     224 LOAD_ATTR                7 (field_name)
          
-         179         366 LOAD_FAST                1 (adapter)
-                     368 LOAD_ATTR                1 (object)
-                     378 LOAD_ATTR               11 (_meta)
-                     388 LOAD_ATTR               12 (app_label)
+         180         234 LOAD_FAST                1 (adapter)
+                     236 LOAD_ATTR                8 (object)
+                     246 LOAD_ATTR                9 (_meta)
+                     256 LOAD_ATTR               10 (app_label)
          
-         180         398 LOAD_FAST                1 (adapter)
-                     400 LOAD_ATTR                1 (object)
-                     410 LOAD_ATTR               11 (_meta)
-                     420 LOAD_ATTR               13 (model_name)
+         181         266 LOAD_FAST                1 (adapter)
+                     268 LOAD_ATTR                8 (object)
+                     278 LOAD_ATTR                9 (_meta)
+                     288 LOAD_ATTR               11 (model_name)
          
-         181         430 LOAD_FAST                1 (adapter)
-                     432 LOAD_ATTR                1 (object)
-                     442 LOAD_ATTR               14 (pk)
+         182         298 LOAD_FAST                1 (adapter)
+                     300 LOAD_ATTR                8 (object)
+                     310 LOAD_ATTR               12 (pk)
          
-         176         452 LOAD_CONST               6 (('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id'))
-                     454 BUILD_CONST_KEY_MAP      5
-                     456 STORE_FAST               7 (reverse_kwargs)
+         177         320 LOAD_CONST               3 (('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id'))
+                     322 BUILD_CONST_KEY_MAP      5
+                     324 STORE_FAST               6 (reverse_kwargs)
          
-         184         458 LOAD_GLOBAL             31 (NULL + render_to_string)
+         185         326 LOAD_FAST                1 (adapter)
+                     328 LOAD_METHOD             13 (encode_shared_context)
+                     350 PRECALL                  0
+                     354 CALL                     0
+                     364 STORE_FAST               7 (shared)
          
-         185         470 LOAD_CONST               7 ('wagtail_fedit/content/editable_adapter.html')
+         187         366 LOAD_GLOBAL             29 (NULL + render_to_string)
          
-         187         472 LOAD_FAST                1 (adapter)
-                     474 LOAD_ATTR               10 (identifier)
+         188         378 LOAD_CONST               4 ('wagtail_fedit/content/editable_adapter.html')
          
-         188         484 LOAD_FAST                3 (content)
+         190         380 LOAD_FAST                1 (adapter)
+                     382 LOAD_ATTR                6 (identifier)
          
-         189         486 LOAD_FAST                1 (adapter)
+         191         392 LOAD_FAST                1 (adapter)
          
-         190         488 LOAD_FAST                5 (items)
+         192         394 LOAD_FAST                4 (items)
          
-         191         490 LOAD_FAST                4 (shared)
+         193         396 LOAD_FAST                7 (shared)
          
-         192         492 LOAD_FAST                1 (adapter)
-                     494 LOAD_ATTR               16 (kwargs)
+         194         398 LOAD_FAST                1 (adapter)
+                     400 LOAD_ATTR               15 (kwargs)
          
-         193         504 LOAD_GLOBAL             35 (NULL + reverse)
+         195         410 LOAD_FAST                2 (context)
          
-         194         516 LOAD_CONST               8 ('wagtail_fedit:edit')
+         196         412 LOAD_GLOBAL             33 (NULL + reverse)
          
-         195         518 LOAD_FAST                7 (reverse_kwargs)
+         197         424 LOAD_CONST               5 ('wagtail_fedit:edit')
          
-         193         520 KW_NAMES                 9
-                     522 PRECALL                  2
-                     526 CALL                     2
+         198         426 LOAD_FAST                6 (reverse_kwargs)
          
-         186         536 LOAD_CONST              10 (('identifier', 'content', 'adapter', 'buttons', 'shared', 'shared_context', 'edit_url'))
-                     538 BUILD_CONST_KEY_MAP      7
+         196         428 KW_NAMES                 6
+                     430 PRECALL                  2
+                     434 CALL                     2
          
-         198         540 LOAD_DEREF               0 (request)
+         189         444 LOAD_CONST               7 (('identifier', 'adapter', 'buttons', 'shared', 'shared_context', 'parent_context', 'edit_url'))
+                     446 BUILD_CONST_KEY_MAP      7
          
-         184         542 KW_NAMES                11
-                     544 PRECALL                  3
-                     548 CALL                     3
-                     558 RETURN_VALUE
+         201         448 LOAD_FAST                3 (run_context_processors)
+                     450 POP_JUMP_FORWARD_IF_FALSE     2 (to 456)
+                     452 LOAD_DEREF               0 (request)
+                     454 JUMP_FORWARD             1 (to 458)
+                 >>  456 LOAD_CONST               0 (None)
+         
+         187     >>  458 KW_NAMES                 8
+                     460 PRECALL                  3
+                     464 CALL                     3
+                     474 RETURN_VALUE
          consts
             None
-            'wagtail_fedit_field'
-            'wagtail_fedit_instance'
-            'request'
             ('items', 'adapter')
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               173           2 RESUME                   0
+               174           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -1114,33 +1122,126 @@
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 173
+               firstlineno 174
                lnotab 0x
             ('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id')
             'wagtail_fedit/content/editable_adapter.html'
             'wagtail_fedit:edit'
             ('kwargs',)
-            ('identifier', 'content', 'adapter', 'buttons', 'shared', 'shared_context', 'edit_url')
+            ('identifier', 'adapter', 'buttons', 'shared', 'shared_context', 'parent_context', 'edit_url')
             ('request',)
-         names      ('field_name', 'object', 'render_content', 'encode_shared_context', 'FeditAdapterEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_ADAPTER_TOOLBAR', 'list', 'filter', 'identifier', '_meta', 'app_label', 'model_name', 'pk', 'render_to_string', 'kwargs', 'reverse')
-         varnames   ('request', 'adapter', 'context', 'content', 'shared', 'items', 'hook', 'reverse_kwargs')
+         names      ('FeditAdapterEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_ADAPTER_TOOLBAR', 'list', 'filter', 'identifier', 'field_name', 'object', '_meta', 'app_label', 'model_name', 'pk', 'encode_shared_context', 'render_to_string', 'kwargs', 'reverse')
+         varnames   ('request', 'adapter', 'context', 'run_context_processors', 'items', 'hook', 'reverse_kwargs', 'shared')
          freevars   ()
          cellvars   ('request',)
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'wrap_adapter'
-         firstlineno 155
+         firstlineno 163
          lnotab
-            0x040104010402140114010a022a0128031aff040436011c021c013a030c
-            010c012001200116fb06080c0102020c0102010201020102010c010c0102
-            0102fe10f9040c02f2
+            0x0401040104031aff040436011c021c013a030c010c012001200116fb06
+            0828020c0102020c010201020102010c0102010c01020102fe10f9040c0a
+            f2
+      True
+      ('takes_context',)
+      code
+         argcount  : 2
+         nlocals   : 3
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007c00a0000000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d007c00a00100000000000000000000000000
+            0000000000000064016900a6020000ab0200000000000000007d02740500
+            0000000000000000007c02740600000000000000000000a6020000ab0200
+            0000000000000072147c02a0000000000000000000000000000000000000
+            000000a6000000ab0000000000000000007d027c00a00400000000000000
+            000000000000000000000000007c02a6010000ab01000000000000000001
+            007c016a0500000000000000007c0064023c0000007c016a060000000000
+            0000007c0064033c0000007c016a0700000000000000007c0064043c0000
+            007c01a00800000000000000000000000000000000000000007c00a60100
+            00ab0100000000000000005300
+         204           0 RESUME                   0
+         
+         206           2 LOAD_FAST                0 (context)
+                       4 LOAD_METHOD              0 (flatten)
+                      26 PRECALL                  0
+                      30 CALL                     0
+                      40 STORE_FAST               0 (context)
+         
+         208          42 LOAD_FAST                0 (context)
+                      44 LOAD_METHOD              1 (pop)
+                      66 LOAD_CONST               1 ('parent_context')
+                      68 BUILD_MAP                0
+                      70 PRECALL                  2
+                      74 CALL                     2
+                      84 STORE_FAST               2 (parent_context)
+         
+         209          86 LOAD_GLOBAL              5 (NULL + isinstance)
+                      98 LOAD_FAST                2 (parent_context)
+                     100 LOAD_GLOBAL              6 (Context)
+                     112 PRECALL                  2
+                     116 CALL                     2
+                     126 POP_JUMP_FORWARD_IF_FALSE    20 (to 168)
+         
+         210         128 LOAD_FAST                2 (parent_context)
+                     130 LOAD_METHOD              0 (flatten)
+                     152 PRECALL                  0
+                     156 CALL                     0
+                     166 STORE_FAST               2 (parent_context)
+         
+         212     >>  168 LOAD_FAST                0 (context)
+                     170 LOAD_METHOD              4 (update)
+                     192 LOAD_FAST                2 (parent_context)
+                     194 PRECALL                  1
+                     198 CALL                     1
+                     208 POP_TOP
+         
+         214         210 LOAD_FAST                1 (adapter)
+                     212 LOAD_ATTR                5 (field_name)
+                     222 LOAD_FAST                0 (context)
+                     224 LOAD_CONST               2 ('wagtail_fedit_field')
+                     226 STORE_SUBSCR
+         
+         215         230 LOAD_FAST                1 (adapter)
+                     232 LOAD_ATTR                6 (object)
+                     242 LOAD_FAST                0 (context)
+                     244 LOAD_CONST               3 ('wagtail_fedit_instance')
+                     246 STORE_SUBSCR
+         
+         216         250 LOAD_FAST                1 (adapter)
+                     252 LOAD_ATTR                7 (request)
+                     262 LOAD_FAST                0 (context)
+                     264 LOAD_CONST               4 ('request')
+                     266 STORE_SUBSCR
+         
+         218         270 LOAD_FAST                1 (adapter)
+                     272 LOAD_METHOD              8 (render_content)
+                     294 LOAD_FAST                0 (context)
+                     296 PRECALL                  1
+                     300 CALL                     1
+                     310 RETURN_VALUE
+         consts
+            None
+            'parent_context'
+            'wagtail_fedit_field'
+            'wagtail_fedit_instance'
+            'request'
+         names      ('flatten', 'pop', 'isinstance', 'Context', 'update', 'field_name', 'object', 'request', 'render_content')
+         varnames   ('context', 'adapter', 'parent_context')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         name       'render_adapter'
+         firstlineno 204
+         lnotab 0x020228022c012a0128022a02140114011402
       'tokens'
       'kwarg_list'
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 5
          flags     : 3
@@ -1155,123 +1256,123 @@
             017c00a00400000000000000000000000000000000000000007c06a60100
             00ab0100000000000000007c047c027c05190000000000000000003c0000
             008c707c076405190000000000000000007d087c00a00400000000000000
             000000000000000000000000007c07640319000000000000000000a60100
             00ab0100000000000000007c047c083c00000064067d038c997c0244005d
             187d097c097c0476017212740b0000000000000000000064077c099b009d
             02a6010000ab01000000000000000082018c197c045300
-         202           0 RESUME                   0
+         221           0 RESUME                   0
          
-         203           2 LOAD_CONST               1 (False)
+         222           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         204           6 BUILD_MAP                0
+         223           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         206          10 LOAD_FAST                2 (kwarg_list)
+         225          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
          
-         207          14 BUILD_LIST               0
+         226          14 BUILD_LIST               0
                       16 STORE_FAST               2 (kwarg_list)
          
-         209     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
+         228     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
                       30 LOAD_FAST                1 (tokens)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 GET_ITER
                  >>   48 FOR_ITER               152 (to 354)
                       50 UNPACK_SEQUENCE          2
                       54 STORE_FAST               5 (i)
                       56 STORE_FAST               6 (token)
          
-         210          58 LOAD_FAST                6 (token)
+         229          58 LOAD_FAST                6 (token)
                       60 LOAD_METHOD              1 (split)
                       82 LOAD_CONST               2 ('=')
                       84 PRECALL                  1
                       88 CALL                     1
                       98 STORE_FAST               7 (split)
          
-         211         100 LOAD_GLOBAL              5 (NULL + len)
+         230         100 LOAD_GLOBAL              5 (NULL + len)
                      112 LOAD_FAST                7 (split)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 LOAD_CONST               3 (1)
                      130 COMPARE_OP               2 (==)
                      136 POP_JUMP_FORWARD_IF_FALSE    67 (to 272)
                      138 LOAD_GLOBAL              5 (NULL + len)
                      150 LOAD_FAST                2 (kwarg_list)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 LOAD_FAST                5 (i)
                      168 COMPARE_OP               4 (>)
                      174 POP_JUMP_FORWARD_IF_FALSE    48 (to 272)
          
-         212         176 LOAD_FAST                3 (had_kwargs)
+         231         176 LOAD_FAST                3 (had_kwargs)
                      178 POP_JUMP_FORWARD_IF_FALSE    15 (to 210)
          
-         213         180 LOAD_GLOBAL              7 (NULL + ValueError)
+         232         180 LOAD_GLOBAL              7 (NULL + ValueError)
                      192 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RAISE_VARARGS            1
          
-         215     >>  210 LOAD_FAST                0 (parser)
+         234     >>  210 LOAD_FAST                0 (parser)
                      212 LOAD_METHOD              4 (compile_filter)
                      234 LOAD_FAST                6 (token)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 LOAD_FAST                4 (kwargs)
                      252 LOAD_FAST                2 (kwarg_list)
                      254 LOAD_FAST                5 (i)
                      256 BINARY_SUBSCR
                      266 STORE_SUBSCR
                      270 JUMP_BACKWARD          112 (to 48)
          
-         217     >>  272 LOAD_FAST                7 (split)
+         236     >>  272 LOAD_FAST                7 (split)
                      274 LOAD_CONST               5 (0)
                      276 BINARY_SUBSCR
                      286 STORE_FAST               8 (key)
          
-         221         288 LOAD_FAST                0 (parser)
+         240         288 LOAD_FAST                0 (parser)
                      290 LOAD_METHOD              4 (compile_filter)
                      312 LOAD_FAST                7 (split)
                      314 LOAD_CONST               3 (1)
                      316 BINARY_SUBSCR
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                4 (kwargs)
                      342 LOAD_FAST                8 (key)
                      344 STORE_SUBSCR
          
-         222         348 LOAD_CONST               6 (True)
+         241         348 LOAD_CONST               6 (True)
                      350 STORE_FAST               3 (had_kwargs)
                      352 JUMP_BACKWARD          153 (to 48)
          
-         224     >>  354 LOAD_FAST                2 (kwarg_list)
+         243     >>  354 LOAD_FAST                2 (kwarg_list)
                      356 GET_ITER
                  >>  358 FOR_ITER                24 (to 408)
                      360 STORE_FAST               9 (kwarg)
          
-         225         362 LOAD_FAST                9 (kwarg)
+         244         362 LOAD_FAST                9 (kwarg)
                      364 LOAD_FAST                4 (kwargs)
                      366 CONTAINS_OP              1
                      368 POP_JUMP_FORWARD_IF_FALSE    18 (to 406)
          
-         226         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
+         245         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
                      382 LOAD_CONST               7 ('Missing required keyword argument ')
                      384 LOAD_FAST                9 (kwarg)
                      386 FORMAT_VALUE             0
                      388 BUILD_STRING             2
                      390 PRECALL                  1
                      394 CALL                     1
                      404 RAISE_VARARGS            1
          
-         225     >>  406 JUMP_BACKWARD           25 (to 358)
+         244     >>  406 JUMP_BACKWARD           25 (to 358)
          
-         228     >>  408 LOAD_FAST                4 (kwargs)
+         247     >>  408 LOAD_FAST                4 (kwargs)
                      410 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -1280,22 +1381,23 @@
             'Missing required keyword argument '
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'kwarg')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 202
+         firstlineno 221
          lnotab
             0x0201040104020401040228012a014c0104011e023e0210043c01060208
             01080124ff0203
+      (False,)
       (None,)
-   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'toolbar', 'FeditAdapterEditButton', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', '_can_edit', 'CONSTRUCT_ADAPTER_TOOLBAR', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'dict', 'str', 'wrap_adapter', 'list', 'get_kwargs')
+   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.loader', 'render_to_string', 'django.template.context', 'make_context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'toolbar', 'FeditAdapterEditButton', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', '_can_edit', 'CONSTRUCT_ADAPTER_TOOLBAR', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'dict', 'bool', 'str', 'wrap_adapter', 'simple_tag', 'render_adapter', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0114010c0110010c010c010c010c020c0208020c0318060c
-      030c051e03040104041c4d2a010eff0e010226182f
+      0x00ff02010c0114030c01100414040c010c010c020c0208020c0318060c
+      030c051e03040104041c4d2a010eff0e0102261e292a0112ff0e010210
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/fedit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import Type
 from django.template import (
     library, Node, TemplateSyntaxError,
 )
 from django.template.loader import render_to_string
+from django.template.context import (
+    make_context,
+    Context,
+)
 from django.template.base import (
     Parser, Token,
     FilterExpression,
 )
 from django.http import HttpRequest
 from django.urls import reverse
 from django.core import signing
@@ -152,25 +156,18 @@
         adapter=adapter,
         model=model,
         getters=model_tokens,
         **kwargs,
     )
 
 
-def wrap_adapter(request: HttpRequest, adapter: BaseAdapter, context: dict) -> str:
+def wrap_adapter(request: HttpRequest, adapter: BaseAdapter, context: dict, run_context_processors: bool = False) -> str:
     if not context:
         context = {}
 
-    context["wagtail_fedit_field"] = adapter.field_name
-    context["wagtail_fedit_instance"] = adapter.object
-    context["request"] = request
-
-    content = adapter.render_content(context)
-    shared = adapter.encode_shared_context()
-
     items = [
         FeditAdapterEditButton(),
     ]
 
     for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
         hook(items=items, adapter=adapter)
 
@@ -181,31 +178,49 @@
         "adapter_id": adapter.identifier,
         "field_name": adapter.field_name,
         "app_label": adapter.object._meta.app_label,
         "model_name": adapter.object._meta.model_name,
         "model_id": adapter.object.pk,
     }
 
+    shared = adapter.encode_shared_context()
+    
     return render_to_string(
         "wagtail_fedit/content/editable_adapter.html",
         {
             "identifier": adapter.identifier,
-            "content": content,
             "adapter": adapter,
             "buttons": items,
             "shared": shared,
             "shared_context": adapter.kwargs,
+            "parent_context": context,
             "edit_url": reverse(
                 "wagtail_fedit:edit",
                 kwargs=reverse_kwargs,
             ),
         },
-        request=request,
+        request=request if run_context_processors else None,
     )
 
+@register.simple_tag(takes_context=True)
+def render_adapter(context: dict, adapter: BaseAdapter) -> str:
+    context = context.flatten()
+    
+    parent_context = context.pop("parent_context", {})
+    if isinstance(parent_context, Context):
+        parent_context = parent_context.flatten()
+        
+    context.update(parent_context)
+
+    context["wagtail_fedit_field"]    = adapter.field_name
+    context["wagtail_fedit_instance"] = adapter.object
+    context["request"]                = adapter.request
+
+    return adapter.render_content(context)
+    
 
 def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None) -> dict:
     had_kwargs = False
     kwargs = {}
 
     if not kwarg_list:
         kwarg_list = []
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,17 +42,24 @@
 
 class TestBlockAdapter(BlockAdapter, TestAdapter):
     identifier = "test_block"
 
 class TestFieldAdapter(FieldAdapter, TestAdapter):
     identifier = "test_field"
 
+class TestContextAdapter(TestAdapter):
+    identifier = "test_context"
+
+    def render_content(self, parent_context: dict = None) -> str:
+        return parent_context["testing"]
+
 adapter_registry.register(TestAdapter)
 adapter_registry.register(TestBlockAdapter)
 adapter_registry.register(TestFieldAdapter)
+adapter_registry.register(TestContextAdapter)
 
 
 class TestBaseAdapter(BaseFEditTest):
 
     def test_required_kwargs_ok(self):
         self.assertEqual(TestAdapter.required_kwargs, ["test"])
 
@@ -163,14 +170,46 @@
         )
 
         self.assertHTMLEqual(
             tpl,
             wrap_adapter(request, adapters[4], {})
         )
 
+    def test_context_processors_run(self):
+        tpl = Template(
+            "{% load fedit %}"
+            "{% fedit test_context object.title test='test' id=5 %}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        setattr(
+            request,
+            FEDIT_PREVIEW_VAR,
+            True,
+        )
+
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+                "testing": "testing context processor",
+            }),
+        )
+
+        self.assertHTMLEqual(
+            tpl,
+            wrap_adapter(request, adapters[5], {}, run_context_processors=True)
+        )
+
 
 class TestBlockAdapter(BaseFEditTest):
 
     def test_render(self):
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         'APP_DIRS': True,
         'OPTIONS': {
             'context_processors': [
                 'django.template.context_processors.debug',
                 'django.template.context_processors.request',
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
+                'wagtail_fedit.test.core.context_processors.test_context_processor'
             ],
         },
     },
 ]
 
 WSGI_APPLICATION = 'testapp.wsgi.application'
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/views/adapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any
 from django.shortcuts import render
 from django.utils.translation import gettext as _
 from django.utils.decorators import method_decorator
 from django.template.loader import render_to_string
 from django.views.decorators.clickjacking import xframe_options_sameorigin
-from django.template.context import make_context
 from django.views.generic import View
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     JsonResponse,
     HttpResponse,
@@ -179,24 +178,20 @@
 
         context = self.get_context_data()
         if isinstance(self.instance, Page):
             # Add the page template variable to the context.
             # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
             context[PAGE_TEMPLATE_VAR] = self.instance
 
-        context = make_context(
-            context,
-            self.request,
-        ).flatten()
-
         # Render the frame HTML
         html = wrap_adapter(
             request=self.request,
             adapter=self.adapter,
             context=context,
+            run_context_processors=True,
         )
 
         return JsonResponse({
             "success": True,
             "html": html,
         })
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.0a2
+Version: 1.5.0a3
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.0a2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.0a3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.0a2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 wagtail_fedit/templatetags/fedit.py
 wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
 wagtail_fedit/test/__init__.py
 wagtail_fedit/test/manage.py
 wagtail_fedit/test/core/__init__.py
 wagtail_fedit/test/core/apps.py
+wagtail_fedit/test/core/context_processors.py
 wagtail_fedit/test/core/models.py
 wagtail_fedit/test/core/migrations/0001_initial.py
 wagtail_fedit/test/core/migrations/0002_basicmodel.py
 wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
 wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
 wagtail_fedit/test/core/migrations/__init__.py
 wagtail_fedit/test/core/tests/__init__.py
```

