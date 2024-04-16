# Comparing `tmp/wagtail_fedit-1.5.0a3.tar.gz` & `tmp/wagtail_fedit-1.5.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.0a3.tar", last modified: Mon Apr 15 20:34:32 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.1a0.tar", last modified: Tue Apr 16 10:17:45 2024, max compression
```

## Comparing `wagtail_fedit-1.5.0a3.tar` & `wagtail_fedit-1.5.1a0.tar`

### file list

```diff
@@ -1,126 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:32.015576 wagtail_fedit-1.5.0a3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0    12405 2024-04-15 20:34:32.015576 wagtail_fedit-1.5.0a3/PKG-INFO
--rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.5.0a3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/pyproject.toml
--rw-rw-rw-   0        0        0     1188 2024-04-15 20:34:32.030370 wagtail_fedit-1.5.0a3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.836498 wagtail_fedit-1.5.0a3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.877892 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     4259 2024-04-15 18:49:04.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     4335 2024-04-15 18:50:49.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     7692 2024-04-15 18:52:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.882857 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.805600 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.806598 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.884903 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.886419 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.887431 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.808123 wagtail_fedit-1.5.0a3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.808123 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.890480 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4333 2024-04-15 18:17:44.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.891710 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    16149 2024-04-15 19:27:25.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.810667 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.813678 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.893838 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.898892 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      446 2024-04-15 20:27:28.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.903895 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.910463 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.914019 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.916445 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.918456 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.921515 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10146 2024-04-15 20:32:57.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7357 2024-04-15 20:32:51.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.923489 wagtail_fedit-1.5.0a3/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.929718 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.966436 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.975796 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     8976 2024-04-15 20:33:16.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.983270 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:32.000934 wagtail_fedit-1.5.0a3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6318 2024-04-15 20:34:05.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:32.013580 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:34:31.870339 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12405 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4089 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 20:34:31.000000 wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.290825 wagtail_fedit-1.5.1a0/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12405 2024-04-16 10:17:45.290825 wagtail_fedit-1.5.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.5.1a0/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1188 2024-04-16 10:17:45.302935 wagtail_fedit-1.5.1a0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.078378 wagtail_fedit-1.5.1a0/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.124935 wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     4416 2024-04-16 09:57:19.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     4633 2024-04-16 09:57:51.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8483 2024-04-16 10:05:24.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.127072 wagtail_fedit-1.5.1a0/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3186 2024-04-16 10:05:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.041190 wagtail_fedit-1.5.1a0/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.041190 wagtail_fedit-1.5.1a0/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.139687 wagtail_fedit-1.5.1a0/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.140343 wagtail_fedit-1.5.1a0/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.141352 wagtail_fedit-1.5.1a0/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.042571 wagtail_fedit-1.5.1a0/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.043918 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.171290 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5159 2024-04-16 10:14:30.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.196329 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    16224 2024-04-16 10:15:53.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.043918 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.046919 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.197836 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.201847 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      446 2024-04-15 20:27:28.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.213635 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.220987 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.227204 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.246621 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.248621 wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.251588 wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9960 2024-04-15 21:09:28.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7320 2024-04-15 21:08:04.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.254958 wagtail_fedit-1.5.1a0/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.257962 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.262391 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.272473 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     9992 2024-04-15 21:13:59.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.276360 wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.281732 wagtail_fedit-1.5.1a0/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6376 2024-04-16 09:47:50.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.289819 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     1152 2024-04-16 10:06:54.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:17:45.120032 wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12405 2024-04-16 10:17:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4043 2024-04-16 10:17:45.000000 wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 10:17:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-16 10:17:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 10:17:44.000000 wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.0a3/LICENSE` & `wagtail_fedit-1.5.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/PKG-INFO` & `wagtail_fedit-1.5.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.0a3
+Version: 1.5.1a0
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.0a3 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.1a0 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.0a3/README.md` & `wagtail_fedit-1.5.1a0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/setup.cfg` & `wagtail_fedit-1.5.1a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3061 330d 0a64 6573 6372 6970 7469 6f6e  0a3..description
+00000030: 3161 300d 0a64 6573 6372 6970 7469 6f6e  1a0..description
 00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
 00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
 00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     return "-".join(map(slugify, map(str, parts)))
 
 
 import pickle
 
 
 
+class VARIABLES:
+    PY_SIZE_VAR = "editor_size"
+    FORM_SIZE_VAR = "data-editor-size"
+
 
 class PickleBlockSerializer:
     """
     Simple wrapper around pickle to be used in signing.dumps and
     signing.loads.
     """
 
@@ -72,14 +76,17 @@
         if not self.request.user.is_authenticated:
             return False
         return True
     
     def get_element_id(self) -> str:
         raise NotImplementedError
     
+    def get_form_attrs(self) -> dict:
+        return {}
+    
     def get_form(self) -> "forms.Form":
         raise NotImplementedError
 
     def form_valid(self, form: "forms.Form"):
         pass
     
     def form_invalid(self, form: "forms.Form"):
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from wagtail.models import (
     RevisionMixin,
 )
 
 from .base import (
     BaseAdapter,
     AdapterError,
+    VARIABLES,
 )
 from ..forms import (
     blocks as block_forms,
 )
 from .. import utils
 
 
@@ -62,14 +63,24 @@
             "block_label": self.block.block.label,
             "model_name": self.model._meta.verbose_name,
             "model_string": model_string,
         }
     
     def get_element_id(self) -> str:
         return f"block-{self.kwargs['block_id']}-section"
+    
+    def get_form_attrs(self) -> dict:
+
+        size = getattr(self.block.block.meta, VARIABLES.PY_SIZE_VAR, None)
+        if size:
+            return super().get_form_attrs() | {
+                VARIABLES.FORM_SIZE_VAR: size,
+            }
+        
+        return {}
 
     def get_form(self):
 
         self.form_class = block_forms.get_block_form_class(self.block.block)
 
         if self.request.method == "POST":
             form = self.form_class(self.request.POST, block=self.block, parent_instance=self.object, request=self.request)
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,23 @@
 from django.utils import translation
 from django.utils.translation import gettext_lazy as _
 from django.utils.safestring import mark_safe
 from django.http import HttpRequest
 
 from wagtail.log_actions import log
 from wagtail.models import RevisionMixin
+from wagtail import hooks
 
-from .base import BaseAdapter
+from .base import (
+    BaseAdapter,
+    VARIABLES,
+)
+from ..hooks import (
+    FIELD_EDITOR_SIZE,
+)
 from ..utils import (
     use_related_form,
     model_diff,
     get_model_string,
     get_field_content,
     is_draft_capable,
     FeditIFrameMixin,
@@ -109,15 +116,38 @@
             }
 
         return super().get_help_text()
           
     def get_element_id(self) -> str:
         m = self.model
         return f"field-{self.field_name}-{m._meta.app_label}-{m._meta.model_name}-{self.object.pk}"
-  
+      
+    def get_form_attrs(self) -> dict:
+        attrs = super().get_form_attrs()
+
+        size = getattr(self.object, f"{VARIABLES.PY_SIZE_VAR}_{self.field_name}", None)
+        if not size:
+
+            for hook in hooks.get_hooks(FIELD_EDITOR_SIZE):
+                size = hook(self.object, self.meta_field)
+                if size:
+                    break
+            
+        if not size \
+          and self.meta_field.is_relation \
+          and use_related_form(self.meta_field):
+            size = "full"
+        
+        if size:
+            return attrs | {
+                VARIABLES.FORM_SIZE_VAR: size,
+            }
+        
+        return attrs
+
     def get_form(self):
         if self.request.method == "POST":
             form = self.form_class(self.request.POST, request=self.request, instance=self.object)
         else:
             form = self.form_class(request=self.request, instance=self.object)
         return form
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 def prefix(name):
     """
         Default prefix for wagtail_fedit hooks.
     """
     return f"wagtail_fedit.{name}"
 
 
+
 CONSTRUCT_ADAPTER_TOOLBAR = prefix("construct_adapter_toolbar")
 """
 ### wagtail_fedit.construct_adapter_toolbar
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
 """
 
@@ -49,14 +50,30 @@
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 """
 
 
+FIELD_EDITOR_SIZE = prefix("field_editor_size")
+"""
+### wagtail_fedit.field_editor_size
+Control the size of the editor for the given model-field type.
+
+Example of how this hook is called:
+    
+    ```python
+    for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE):
+        size = hook(model_instance, model_field)
+        if size:
+            return size
+    ```
+"""
+
+
 EXCLUDE_FROM_RELATED_FORMS = prefix("exclude_related_forms")
 """
 ### wagtail_fedit.exclude_related_forms
 Exclude the given model type from the related forms.
 This is used internally to exclude the Page, Image, and Document models from the related forms.
 This way; the user will have the actual widget for the field instead of the related form.
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.1a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.1a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/models.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 17% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     width: 100%;
     height: 100%;
     background-color: rgba(0, 0, 0, 0.05);
     outline: 2px solid #333333;
     pointer-events: none;
     z-index: 300;
 }
-.wagtail-fedit-adapter-wrapper.wagtail-fedit-field:has(.wagtail-fedit-adapter) > .wagtail-fedit-buttons {
+.wagtail-fedit-adapter-wrapper.wagtail-fedit-field:has(.wagtail-fedit-adapter-wrapper) > .wagtail-fedit-buttons {
     right: 30px;
 }
 .wagtail-fedit-buttons {
     display: flex;
     gap: 0.5em;
     border-radius: 0.5em;
     position: absolute;
@@ -99,20 +99,14 @@
     background-color: rgba(0, 0, 0, 0.5);
     display: flex;
     justify-content: center;
     align-items: center;
     z-index: 400;
     overflow: auto;
 }
-.wagtail-fedit-modal-wrapper .wagtail-fedit-modal.fedit-full {
-    height: 100%;
-    width: 100%;
-    /* max-width: unset; */
-    /* max-height: unset; */
-}
 .wagtail-fedit-modal-wrapper .wagtail-fedit-modal {
     position: relative;
     min-width: max(60dvw, 15rem);
     min-height: max(60dvh, 15rem);
     outline: 2px solid #333333;
     outline-offset: -1px;
     box-shadow: 0 0 1em rgba(0, 0, 0, 0.5);
@@ -122,18 +116,56 @@
     flex-direction: column;
     gap: 1em;
     max-width: 80%;
     max-height: 80%;
     overflow: hidden;
     display: flex;
 }
-.wagtail-fedit-modal-wrapper .wagtail-fedit-modal:not(.fedit-full) {
-    margin-top: -5%;
+.wagtail-fedit-modal-wrapper:has(.wagtail-fedit-modal.fedit-full) {
+    z-index: 9999;
+}
+.wagtail-fedit-modal-wrapper .wagtail-fedit-modal.fedit-full {
+    height: 100%;
+    width: 100%;
+    max-width: unset;
+    max-height: unset;
+}
+.wagtail-fedit-modal-wrapper .wagtail-fedit-modal.fedit-large {
+    height: 100%;
+    width: 100%;
+}
+@media (min-width: 768px) {
+    .wagtail-fedit-modal-wrapper .wagtail-fedit-modal:not(.fedit-large, .fedit-full) {
+        margin-top: -5%;
+    }
+}
+@media (max-width: 1400px) {
+    .wagtail-fedit-modal-wrapper {
+        z-index: 9999;
+    }
+    .wagtail-fedit-modal-wrapper .wagtail-fedit-modal {
+        max-width: 80%;
+        max-height: 80%;
+        width: 100%;
+        height: 100%;
+    }
+}
+@media (max-width: 1100px) {
+    .wagtail-fedit-modal-wrapper .wagtail-fedit-modal {
+        max-width: 90%;
+        max-height: 90%;
+    }
+}
+@media (max-width: 768px) {
+    .wagtail-fedit-modal-wrapper .wagtail-fedit-modal {
+        margin: 0;
+        max-width: 100%;
+        max-height: 100%;
+    }
 }
-
 .wagtail-fedit-modal-wrapper iframe {
     width: 100%;
     height: 100%;
     border: none;
     flex: 1;
 }
 .wagtail-fedit-modal-wrapper .wagtail-fedit-close-button {
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.1a0/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -210,22 +210,24 @@
                 };
                 this.iframe.formElement.onsubmit = onSubmit;
                 this.iframe.onCancel = this.closeModal.bind(this);
 
                 // Check if we need to apply the fedit-full class to the modal
                 const formHeight = this.iframe.formElement.getBoundingClientRect().height;
                 const formWrapper = this.iframe.formWrapper;
-                if (
-                    (formWrapper && (
-                        formWrapper.classList.contains("fedit-full") ||
-                        (this.iframe.formElement.dataset.isRelation || "").toLowerCase() === "true"
-                    )) ||
-                    (formHeight > window.innerHeight)
-                ) {
-                    this.modal.classList.add("fedit-full");
+                const options = ["large", "full"]
+
+                for (const option of options) {
+                    if (formWrapper && (
+                            formWrapper.classList.contains(`fedit-${option}`) ||
+                            (this.iframe.formElement.dataset.editorSize || "").toLowerCase() === option
+                        )) {
+                        this.modal.classList.add(`fedit-${option}`);
+                        break;
+                    }
                 }
 
                 const url = window.location.href.split("#")[0];
                 window.history.pushState(null, this.iframe.document.title, url + `#${this.wrapperElement.id}`);
                 document.title = this.iframe.document.title;
             },
             onError: () => {
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf38e1d66 (Mon Apr 15 20:32:51 2024 UTC)
-files sz: 7357
+moddate:  0x34971d66 (Mon Apr 15 21:08:04 2024 UTC)
+files sz: 7320
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
@@ -16,15 +16,15 @@
       1f6d205a200100640b640f6c166d215a210100020065036a220000000000
       000000a6000000ab0000000000000000005a2364105a2464115a25020047
       006412840064136504a6030000ab0300000000000000005a266523a02700
       000000000000000000000000000000000000006414ac15a6010000ab0100
       000000000000006416650c6417650d660464188404a6000000ab00000000
       00000000005a286426641a6510641b651d641c6529641d652a641e652b66
       0a641f84055a2c6523a02d00000000000000000000000000000000000000
-      006420ac21a6010000ab010000000000000000641c6529641b651d641e65
+      006420ac21a6010000ab010000000000000000641c650a641b651d641e65
       2b660664228404a6000000ab0000000000000000005a2e64276416650c64
       23652f652b190000000000000000006424652f652b190000000000000000
       00641e65296608642584055a30640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type',))
@@ -201,15 +201,15 @@
                368 LOAD_METHOD             45 (simple_tag)
                390 LOAD_CONST              32 (True)
                392 KW_NAMES                33
                394 PRECALL                  1
                398 CALL                     1
    
    205         408 LOAD_CONST              28 ('context')
-               410 LOAD_NAME               41 (dict)
+               410 LOAD_NAME               10 (Context)
                412 LOAD_CONST              27 ('adapter')
                414 LOAD_NAME               29 (BaseAdapter)
                416 LOAD_CONST              30 ('return')
                418 LOAD_NAME               43 (str)
                420 BUILD_TUPLE              6
                422 LOAD_CONST              34 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 204>)
                424 MAKE_FUNCTION            4 (annotations)
@@ -1146,102 +1146,88 @@
             0828020c0102020c010201020102010c0102010c01020102fe10f9040c0a
             f2
       True
       ('takes_context',)
       code
          argcount  : 2
          nlocals   : 3
-         stacksize : 4
+         stacksize : 3
          flags     : 3
          code
-            0x97007c00a0000000000000000000000000000000000000000000a60000
-            00ab0000000000000000007d007c00a00100000000000000000000000000
-            0000000000000064016900a6020000ab0200000000000000007d02740500
-            0000000000000000007c02740600000000000000000000a6020000ab0200
-            0000000000000072147c02a0000000000000000000000000000000000000
-            000000a6000000ab0000000000000000007d027c00a00400000000000000
-            000000000000000000000000007c02a6010000ab01000000000000000001
-            007c016a0500000000000000007c0064023c0000007c016a060000000000
-            0000007c0064033c0000007c016a0700000000000000007c0064043c0000
-            007c01a00800000000000000000000000000000000000000007c00a60100
-            00ab0100000000000000005300
+            0x970069007d0264017c007600720b7c006401190000000000000000007d
+            027c0064013d007c00a00000000000000000000000000000000000000000
+            007c02a6010000ab01000000000000000001007c016a0100000000000000
+            007c0064023c0000007c016a0200000000000000007c0064033c0000007c
+            016a0300000000000000007c0064043c0000007c01a00400000000000000
+            000000000000000000000000007c00a6010000ab01000000000000000053
+            00
          204           0 RESUME                   0
          
-         206           2 LOAD_FAST                0 (context)
-                       4 LOAD_METHOD              0 (flatten)
-                      26 PRECALL                  0
-                      30 CALL                     0
-                      40 STORE_FAST               0 (context)
-         
-         208          42 LOAD_FAST                0 (context)
-                      44 LOAD_METHOD              1 (pop)
-                      66 LOAD_CONST               1 ('parent_context')
-                      68 BUILD_MAP                0
-                      70 PRECALL                  2
-                      74 CALL                     2
-                      84 STORE_FAST               2 (parent_context)
-         
-         209          86 LOAD_GLOBAL              5 (NULL + isinstance)
-                      98 LOAD_FAST                2 (parent_context)
-                     100 LOAD_GLOBAL              6 (Context)
-                     112 PRECALL                  2
-                     116 CALL                     2
-                     126 POP_JUMP_FORWARD_IF_FALSE    20 (to 168)
-         
-         210         128 LOAD_FAST                2 (parent_context)
-                     130 LOAD_METHOD              0 (flatten)
-                     152 PRECALL                  0
-                     156 CALL                     0
-                     166 STORE_FAST               2 (parent_context)
-         
-         212     >>  168 LOAD_FAST                0 (context)
-                     170 LOAD_METHOD              4 (update)
-                     192 LOAD_FAST                2 (parent_context)
-                     194 PRECALL                  1
-                     198 CALL                     1
-                     208 POP_TOP
+         206           2 BUILD_MAP                0
+                       4 STORE_FAST               2 (parent_context)
          
-         214         210 LOAD_FAST                1 (adapter)
-                     212 LOAD_ATTR                5 (field_name)
-                     222 LOAD_FAST                0 (context)
-                     224 LOAD_CONST               2 ('wagtail_fedit_field')
-                     226 STORE_SUBSCR
-         
-         215         230 LOAD_FAST                1 (adapter)
-                     232 LOAD_ATTR                6 (object)
-                     242 LOAD_FAST                0 (context)
-                     244 LOAD_CONST               3 ('wagtail_fedit_instance')
-                     246 STORE_SUBSCR
-         
-         216         250 LOAD_FAST                1 (adapter)
-                     252 LOAD_ATTR                7 (request)
-                     262 LOAD_FAST                0 (context)
-                     264 LOAD_CONST               4 ('request')
-                     266 STORE_SUBSCR
-         
-         218         270 LOAD_FAST                1 (adapter)
-                     272 LOAD_METHOD              8 (render_content)
-                     294 LOAD_FAST                0 (context)
-                     296 PRECALL                  1
-                     300 CALL                     1
-                     310 RETURN_VALUE
+         208           6 LOAD_CONST               1 ('parent_context')
+                       8 LOAD_FAST                0 (context)
+                      10 CONTAINS_OP              0
+                      12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
+         
+         209          14 LOAD_FAST                0 (context)
+                      16 LOAD_CONST               1 ('parent_context')
+                      18 BINARY_SUBSCR
+                      28 STORE_FAST               2 (parent_context)
+         
+         210          30 LOAD_FAST                0 (context)
+                      32 LOAD_CONST               1 ('parent_context')
+                      34 DELETE_SUBSCR
+         
+         212     >>   36 LOAD_FAST                0 (context)
+                      38 LOAD_METHOD              0 (update)
+                      60 LOAD_FAST                2 (parent_context)
+                      62 PRECALL                  1
+                      66 CALL                     1
+                      76 POP_TOP
+         
+         214          78 LOAD_FAST                1 (adapter)
+                      80 LOAD_ATTR                1 (field_name)
+                      90 LOAD_FAST                0 (context)
+                      92 LOAD_CONST               2 ('wagtail_fedit_field')
+                      94 STORE_SUBSCR
+         
+         215          98 LOAD_FAST                1 (adapter)
+                     100 LOAD_ATTR                2 (object)
+                     110 LOAD_FAST                0 (context)
+                     112 LOAD_CONST               3 ('wagtail_fedit_instance')
+                     114 STORE_SUBSCR
+         
+         216         118 LOAD_FAST                1 (adapter)
+                     120 LOAD_ATTR                3 (request)
+                     130 LOAD_FAST                0 (context)
+                     132 LOAD_CONST               4 ('request')
+                     134 STORE_SUBSCR
+         
+         218         138 LOAD_FAST                1 (adapter)
+                     140 LOAD_METHOD              4 (render_content)
+                     162 LOAD_FAST                0 (context)
+                     164 PRECALL                  1
+                     168 CALL                     1
+                     178 RETURN_VALUE
          consts
             None
             'parent_context'
             'wagtail_fedit_field'
             'wagtail_fedit_instance'
             'request'
-         names      ('flatten', 'pop', 'isinstance', 'Context', 'update', 'field_name', 'object', 'request', 'render_content')
+         names      ('update', 'field_name', 'object', 'request', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
          firstlineno 204
-         lnotab 0x020228022c012a0128022a02140114011402
+         lnotab 0x020204020801100106022a02140114011402
       'tokens'
       'kwarg_list'
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 5
          flags     : 3
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/templatetags/fedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,21 +198,21 @@
                 kwargs=reverse_kwargs,
             ),
         },
         request=request if run_context_processors else None,
     )
 
 @register.simple_tag(takes_context=True)
-def render_adapter(context: dict, adapter: BaseAdapter) -> str:
-    context = context.flatten()
+def render_adapter(context: Context, adapter: BaseAdapter) -> str:
+    parent_context = {}
     
-    parent_context = context.pop("parent_context", {})
-    if isinstance(parent_context, Context):
-        parent_context = parent_context.flatten()
-        
+    if "parent_context" in context:
+        parent_context = context["parent_context"]
+        del context["parent_context"]
+
     context.update(parent_context)
 
     context["wagtail_fedit_field"]    = adapter.field_name
     context["wagtail_fedit_instance"] = adapter.object
     context["request"]                = adapter.request
 
     return adapter.render_content(context)
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from wagtail_fedit.templatetags.fedit import (
     wrap_adapter,
 )
 from .base import (
     BaseFEditTest,
 )
 
-import json
-
 adapters = {}
 
 class TestAdapter(BaseAdapter):
     identifier = "test"
     required_kwargs = ["test"]
 
     def __init__(self, object: Model, field_name: str, request: HttpRequest, **kwargs):
@@ -35,27 +33,26 @@
 
     def get_element_id(self) -> str:
         return f"test-{self.kwargs['id']}"
 
     def render_content(self, parent_context: dict = None) -> str:
         return f"TestAdapter: {self.field_value}"
 
+class TestContextAdapter(TestAdapter):
+    identifier = "test_context"
+
+    def render_content(self, parent_context: dict = None) -> str:
+        return parent_context["testing"]
 
 class TestBlockAdapter(BlockAdapter, TestAdapter):
     identifier = "test_block"
 
 class TestFieldAdapter(FieldAdapter, TestAdapter):
     identifier = "test_field"
 
-class TestContextAdapter(TestAdapter):
-    identifier = "test_context"
-
-    def render_content(self, parent_context: dict = None) -> str:
-        return parent_context["testing"]
-
 adapter_registry.register(TestAdapter)
 adapter_registry.register(TestBlockAdapter)
 adapter_registry.register(TestFieldAdapter)
 adapter_registry.register(TestContextAdapter)
 
 
 class TestBaseAdapter(BaseFEditTest):
@@ -189,14 +186,15 @@
 
         setattr(
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
 
+        # In this test we are testing the adapter - not the template.
         tpl = tpl.render(
             Context({
                 "request": request,
                 "object": self.basic_model,
                 "testing": "testing context processor",
             }),
         )
@@ -304,7 +302,40 @@
 
         tpl = template.render(Context(context))
 
         self.assertHTMLEqual(
             tpl,
             block_value.render(context),
         )
+
+
+class TestFieldAdapter(BaseFEditTest):
+    
+        def test_render(self):
+            request = self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            )
+            request.user = self.admin_user
+            setattr(
+                request,
+                FEDIT_PREVIEW_VAR,
+                True,
+            )
+            template = Template(
+                "{% load fedit %}"
+                "{% fedit test_field object.title test=True id=7 %}"
+            )
+    
+            context = {
+                "object": self.basic_model,
+                "request": request,
+            }
+    
+            tpl = template.render(Context(context))
+    
+            self.assertHTMLEqual(
+                tpl,
+                wrap_adapter(request, adapters[7], {})
+            )
+
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/views/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
                 self.request.GET["shared_context"]
 
         return super().get_context_data(**kwargs) | {
             "meta_field": self.adapter.meta_field,
             "field_name": self.adapter.field_name,
             "locked_for_user": self.locked_for_user,
             "shared_context": shared_context,
+            "form_attrs": self.adapter.get_form_attrs(),
             "locked": self.lock is not None,
         }
 
 class EditAdapterView(BaseAdapterView):
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.adapter.get_form()
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.1a0/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.0a3
+Version: 1.5.1a0
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
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.0a3 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.1a0 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.0a3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.1a0/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,13 @@
 wagtail_fedit/test/testapp/wsgi.py
 wagtail_fedit/views/__init__.py
 wagtail_fedit/views/adapters.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/mixins.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/action_menu.py
+wagtail_fedit/wagtail_hooks/adapter_hooks.py
 wagtail_fedit/wagtail_hooks/adapter_registry.py
-wagtail_fedit/wagtail_hooks/excluded_relations.py
 wagtail_fedit/wagtail_hooks/icons.py
 wagtail_fedit/wagtail_hooks/log_actions.py
-wagtail_fedit/wagtail_hooks/renderers.py
 wagtail_fedit/wagtail_hooks/urls.py
 wagtail_fedit/wagtail_hooks/userbar.py
```

