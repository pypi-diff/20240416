# Comparing `tmp/reflex-0.4.8.tar.gz` & `tmp/reflex-0.4.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.4.8.tar", max compression
+gzip compressed data, was "reflex-0.4.8a1.tar", max compression
```

## Comparing `reflex-0.4.8.tar` & `reflex-0.4.8a1.tar`

### file list

```diff
@@ -1,510 +1,510 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.8/LICENSE
--rw-r--r--   0        0        0     9568 2024-04-05 17:14:14.456384 reflex-0.4.8/README.md
--rw-r--r--   0        0        0     2920 2024-04-15 22:12:45.851859 reflex-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.8/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.8/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      861 2024-04-05 17:14:14.457193 reflex-0.4.8/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.8/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.8/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.8/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.8/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.8/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.8/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.8/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.8/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.8/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.8/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.8/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.8/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.8/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.8/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.8/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.8/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.8/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.8/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.8/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.8/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.8/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.8/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.8/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.8/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.4.8/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.4.8/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.8/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.8/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.8/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.8/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.8/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.8/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.4.8/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.4.8/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.8/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.8/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.8/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.8/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.8/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.8/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.8/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.8/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.8/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.8/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.8/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.8/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.8/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.8/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.8/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.8/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0    21909 2024-04-12 01:14:12.255596 reflex-0.4.8/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5723 2024-04-05 17:14:14.458168 reflex-0.4.8/reflex/__init__.py
--rw-r--r--   0        0        0     7649 2024-04-06 01:20:11.620853 reflex-0.4.8/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.8/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.8/reflex/admin.py
--rw-r--r--   0        0        0    45016 2024-04-12 01:14:12.255992 reflex-0.4.8/reflex/app.py
--rw-r--r--   0        0        0     5010 2024-04-04 14:57:26.376271 reflex-0.4.8/reflex/app.pyi
--rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.8/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4250 2024-04-04 14:57:26.376408 reflex-0.4.8/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.8/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17037 2024-04-05 17:14:14.458702 reflex-0.4.8/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.8/reflex/compiler/templates.py
--rw-r--r--   0        0        0    14024 2024-04-12 01:14:12.256301 reflex-0.4.8/reflex/compiler/utils.py
--rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.8/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.8/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.8/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-04-04 14:57:26.376832 reflex-0.4.8/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.4.8/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.8/reflex/components/base/body.py
--rw-r--r--   0        0        0     3206 2024-04-12 01:14:12.256423 reflex-0.4.8/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.8/reflex/components/base/document.py
--rw-r--r--   0        0        0    14232 2024-04-12 01:14:12.256750 reflex-0.4.8/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.8/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3218 2024-04-12 01:14:12.256848 reflex-0.4.8/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.8/reflex/components/base/head.py
--rw-r--r--   0        0        0     6002 2024-04-12 01:14:12.257050 reflex-0.4.8/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.8/reflex/components/base/link.py
--rw-r--r--   0        0        0     6990 2024-04-12 01:14:12.257244 reflex-0.4.8/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.8/reflex/components/base/meta.py
--rw-r--r--   0        0        0    12804 2024-04-12 01:14:12.257347 reflex-0.4.8/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.8/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-04-04 14:57:26.377962 reflex-0.4.8/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.8/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.8/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    10917 2024-04-12 01:14:12.257771 reflex-0.4.8/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.8/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.8/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3654 2024-04-12 01:14:12.257918 reflex-0.4.8/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.8/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3229 2024-04-12 01:14:12.258034 reflex-0.4.8/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.8/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     3934 2024-04-12 01:14:12.258149 reflex-0.4.8/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.8/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3251 2024-04-12 01:14:12.258264 reflex-0.4.8/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.8/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    12994 2024-04-12 01:14:12.258377 reflex-0.4.8/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.8/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.258509 reflex-0.4.8/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.8/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27252 2024-04-12 01:14:12.258649 reflex-0.4.8/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.8/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    15734 2024-04-12 01:14:12.258803 reflex-0.4.8/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.8/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.8/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    15803 2024-04-12 01:14:12.258961 reflex-0.4.8/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.8/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18525 2024-04-12 01:14:12.259114 reflex-0.4.8/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.8/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20003 2024-04-12 01:14:12.259285 reflex-0.4.8/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.8/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3258 2024-04-12 01:14:12.259424 reflex-0.4.8/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.8/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.8/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12381 2024-04-12 01:14:12.259528 reflex-0.4.8/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.8/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7637 2024-04-12 01:14:12.259726 reflex-0.4.8/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.8/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4278 2024-04-12 01:14:12.259930 reflex-0.4.8/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.8/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10690 2024-04-12 01:14:12.260187 reflex-0.4.8/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.8/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4107 2024-04-12 01:14:12.260440 reflex-0.4.8/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.8/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.8/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10545 2024-04-12 01:14:12.260613 reflex-0.4.8/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.8/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10301 2024-04-12 01:14:12.260767 reflex-0.4.8/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.8/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18459 2024-04-12 01:14:12.260906 reflex-0.4.8/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.8/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.380782 reflex-0.4.8/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.8/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-04-04 14:57:26.380893 reflex-0.4.8/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.8/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13339 2024-04-12 01:14:12.261047 reflex-0.4.8/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.8/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-04-04 14:57:26.381120 reflex-0.4.8/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.8/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20619 2024-04-12 01:14:12.261180 reflex-0.4.8/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.8/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4668 2024-04-12 01:14:12.261417 reflex-0.4.8/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.8/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21514 2024-04-12 01:14:12.261540 reflex-0.4.8/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.8/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.8/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18093 2024-04-12 01:14:12.261730 reflex-0.4.8/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.8/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-04-04 14:57:26.381709 reflex-0.4.8/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.4.8/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9357 2024-04-12 01:14:12.262316 reflex-0.4.8/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.4.8/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8410 2024-04-12 01:14:12.263294 reflex-0.4.8/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.4.8/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    13939 2024-04-12 01:14:12.263866 reflex-0.4.8/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.8/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-04-04 14:57:26.382156 reflex-0.4.8/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.8/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.263981 reflex-0.4.8/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.8/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6531 2024-04-12 01:14:12.264203 reflex-0.4.8/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.8/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-04-04 14:57:26.382551 reflex-0.4.8/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.8/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.382659 reflex-0.4.8/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.8/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.8/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3379 2024-04-12 01:14:12.264318 reflex-0.4.8/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.8/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3662 2024-04-12 01:14:12.264413 reflex-0.4.8/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.8/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    13850 2024-04-12 01:14:12.264513 reflex-0.4.8/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.8/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8692 2024-04-12 01:14:12.264634 reflex-0.4.8/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.8/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3431 2024-04-12 01:14:12.264741 reflex-0.4.8/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.8/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4138 2024-04-12 01:14:12.264933 reflex-0.4.8/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.8/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    13853 2024-04-12 01:14:12.265035 reflex-0.4.8/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.8/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3230 2024-04-12 01:14:12.265136 reflex-0.4.8/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.8/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12219 2024-04-12 01:14:12.265267 reflex-0.4.8/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.8/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     6943 2024-04-12 01:14:12.265632 reflex-0.4.8/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.8/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.8/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10445 2024-04-12 01:14:12.265841 reflex-0.4.8/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.8/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6271 2024-04-12 01:14:12.266058 reflex-0.4.8/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.8/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-04-04 14:57:26.384173 reflex-0.4.8/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.8/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.8/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13575 2024-04-12 01:14:12.266197 reflex-0.4.8/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.8/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-04-04 14:57:26.384405 reflex-0.4.8/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.8/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6233 2024-04-12 01:14:12.266398 reflex-0.4.8/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.8/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    27922 2024-04-12 01:14:12.266521 reflex-0.4.8/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.8/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.8/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    23985 2024-04-12 01:14:12.266681 reflex-0.4.8/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.8/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25406 2024-04-12 01:14:12.266827 reflex-0.4.8/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.8/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    28682 2024-04-12 01:14:12.266967 reflex-0.4.8/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.8/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23549 2024-04-12 01:14:12.267114 reflex-0.4.8/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.8/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    29893 2024-04-12 01:14:12.267256 reflex-0.4.8/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.8/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6060 2024-04-12 01:14:12.267494 reflex-0.4.8/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.8/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.8/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3706 2024-04-12 01:14:12.267618 reflex-0.4.8/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.8/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3645 2024-04-12 01:14:12.267722 reflex-0.4.8/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.8/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3372 2024-04-12 01:14:12.267821 reflex-0.4.8/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.8/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3596 2024-04-12 01:14:12.267927 reflex-0.4.8/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    66011 2024-04-12 01:14:12.268153 reflex-0.4.8/reflex/components/component.py
--rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.8/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.4.8/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-04-04 14:57:26.386284 reflex-0.4.8/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.8/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6264 2024-04-12 01:14:12.268957 reflex-0.4.8/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.8/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6291 2024-04-04 14:19:59.331531 reflex-0.4.8/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4642 2024-03-20 23:54:55.842359 reflex-0.4.8/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4149 2024-04-04 14:57:26.386549 reflex-0.4.8/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.8/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.8/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-04-04 14:57:26.386705 reflex-0.4.8/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.8/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.8/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.4.8/reflex/components/core/responsive.py
--rw-r--r--   0        0        0     9035 2024-04-12 01:14:12.269123 reflex-0.4.8/reflex/components/core/upload.py
--rw-r--r--   0        0        0     8596 2024-04-12 01:14:12.269265 reflex-0.4.8/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.4.8/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-04 14:19:59.332304 reflex-0.4.8/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31107 2024-04-04 14:57:26.387164 reflex-0.4.8/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.8/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-04-04 14:57:26.387318 reflex-0.4.8/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.4.8/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.8/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.8/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.8/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.8/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.8/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.8/reflex/components/el/element.py
--rw-r--r--   0        0        0     3213 2024-04-12 01:14:12.269384 reflex-0.4.8/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.8/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.8/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6340 2024-04-12 01:14:12.269589 reflex-0.4.8/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20102 2024-04-05 17:14:14.460921 reflex-0.4.8/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0    99553 2024-04-12 01:14:12.269801 reflex-0.4.8/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.8/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   164607 2024-04-12 01:14:12.270476 reflex-0.4.8/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.8/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    93567 2024-04-12 01:14:12.270712 reflex-0.4.8/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.8/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28031 2024-04-12 01:14:12.270995 reflex-0.4.8/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.8/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42033 2024-04-12 01:14:12.271158 reflex-0.4.8/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.8/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19615 2024-04-12 01:14:12.271357 reflex-0.4.8/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.8/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    87242 2024-04-12 01:14:12.271561 reflex-0.4.8/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.8/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    61849 2024-04-12 01:14:12.271965 reflex-0.4.8/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.8/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    89115 2024-04-12 01:14:12.272183 reflex-0.4.8/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.8/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.8/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7053 2024-04-12 01:14:12.272607 reflex-0.4.8/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.8/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.8/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34237 2024-04-04 14:57:26.389624 reflex-0.4.8/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    37949 2024-04-12 01:14:12.272820 reflex-0.4.8/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.8/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    11448 2024-04-05 17:14:14.461428 reflex-0.4.8/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5278 2024-04-05 17:14:14.461583 reflex-0.4.8/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.8/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.8/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.8/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.8/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-04-04 14:57:26.390245 reflex-0.4.8/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.8/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.8/reflex/components/next/base.py
--rw-r--r--   0        0        0     3233 2024-04-12 01:14:12.273046 reflex-0.4.8/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.8/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-04-04 14:57:26.390489 reflex-0.4.8/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.8/reflex/components/next/link.py
--rw-r--r--   0        0        0     3461 2024-04-12 01:14:12.273179 reflex-0.4.8/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.8/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-04-04 14:57:26.390675 reflex-0.4.8/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.8/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.8/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     6865 2024-04-12 01:14:12.273411 reflex-0.4.8/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.8/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.8/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.8/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    26885 2024-04-12 01:14:12.273564 reflex-0.4.8/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.8/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6478 2024-04-12 01:14:12.273957 reflex-0.4.8/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.8/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34484 2024-04-12 01:14:12.274125 reflex-0.4.8/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.8/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    47939 2024-04-12 01:14:12.274318 reflex-0.4.8/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.8/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22784 2024-04-12 01:14:12.274470 reflex-0.4.8/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.8/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    16697 2024-04-12 01:14:12.275306 reflex-0.4.8/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.8/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.8/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    24074 2024-04-12 01:14:12.275479 reflex-0.4.8/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.8/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    21283 2024-04-04 14:57:26.391843 reflex-0.4.8/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.8/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.8/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-04-04 14:57:26.391969 reflex-0.4.8/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0    40237 2024-02-17 20:02:02.428774 reflex-0.4.8/reflex/components/radix/themes/components/alertdialog.pyi
--rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.8/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-04-04 14:57:26.392096 reflex-0.4.8/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0     5724 2024-02-17 20:02:02.429087 reflex-0.4.8/reflex/components/radix/themes/components/aspectratio.pyi
--rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.8/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-04-04 14:57:26.392242 reflex-0.4.8/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.8/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9315 2024-04-04 14:57:26.392362 reflex-0.4.8/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.8/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11758 2024-04-04 14:57:26.392476 reflex-0.4.8/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.8/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-04-04 14:57:26.392589 reflex-0.4.8/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.8/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-04-04 14:57:26.392715 reflex-0.4.8/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.8/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-04-04 14:57:26.392804 reflex-0.4.8/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.8/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-04-04 14:57:26.392918 reflex-0.4.8/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0    44130 2024-02-17 20:02:02.432309 reflex-0.4.8/reflex/components/radix/themes/components/contextmenu.pyi
--rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.8/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-04-04 14:57:26.393065 reflex-0.4.8/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.8/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-04-04 14:57:26.393223 reflex-0.4.8/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0    52185 2024-02-17 20:02:02.435613 reflex-0.4.8/reflex/components/radix/themes/components/dropdownmenu.pyi
--rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.8/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-04-04 14:57:26.393356 reflex-0.4.8/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0    26453 2024-02-17 20:02:02.436260 reflex-0.4.8/reflex/components/radix/themes/components/hovercard.pyi
--rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.8/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    11916 2024-04-04 14:57:26.393481 reflex-0.4.8/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0    12021 2024-02-17 20:02:02.436631 reflex-0.4.8/reflex/components/radix/themes/components/iconbutton.pyi
--rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.8/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-04-04 14:57:26.393614 reflex-0.4.8/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.8/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-04-04 14:57:26.393725 reflex-0.4.8/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.8/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-04-04 14:57:26.393848 reflex-0.4.8/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0    26222 2024-03-20 23:54:55.854920 reflex-0.4.8/reflex/components/radix/themes/components/radiogroup.pyi
--rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.8/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-04-04 14:57:26.393997 reflex-0.4.8/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     6513 2024-02-17 20:02:02.439025 reflex-0.4.8/reflex/components/radix/themes/components/scrollarea.pyi
--rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.4.8/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-04-04 14:57:26.394155 reflex-0.4.8/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.8/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-04-04 14:57:26.394306 reflex-0.4.8/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.8/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-04-04 14:57:26.394440 reflex-0.4.8/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.8/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-04-04 14:57:26.394593 reflex-0.4.8/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.8/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-04-04 14:57:26.394744 reflex-0.4.8/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.8/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    17321 2024-04-04 14:57:26.394873 reflex-0.4.8/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.8/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-04-04 14:57:26.395020 reflex-0.4.8/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.8/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    43043 2024-04-04 14:57:26.395140 reflex-0.4.8/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0    43365 2024-02-17 20:02:02.442188 reflex-0.4.8/reflex/components/radix/themes/components/textfield.pyi
--rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.8/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-04-04 14:57:26.395307 reflex-0.4.8/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.4.8/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.8/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7643 2024-04-04 14:57:26.395455 reflex-0.4.8/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.8/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-04-04 14:57:26.395640 reflex-0.4.8/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.8/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.395883 reflex-0.4.8/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.8/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     6779 2024-04-04 14:57:26.396069 reflex-0.4.8/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.8/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-04-04 14:57:26.396231 reflex-0.4.8/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.8/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-04-04 14:57:26.396387 reflex-0.4.8/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4889 2024-04-04 14:19:59.341578 reflex-0.4.8/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    29367 2024-04-04 14:57:26.396553 reflex-0.4.8/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.8/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-04-04 14:57:26.396712 reflex-0.4.8/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.8/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.396834 reflex-0.4.8/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.8/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-04-04 14:57:26.396967 reflex-0.4.8/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.8/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.8/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.8/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-04-04 14:57:26.397104 reflex-0.4.8/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.8/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-04-04 14:57:26.397215 reflex-0.4.8/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     8547 2024-02-17 20:02:02.446585 reflex-0.4.8/reflex/components/radix/themes/typography/em.pyi
--rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.8/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-04-04 14:57:26.397327 reflex-0.4.8/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     8872 2024-02-17 20:02:02.446866 reflex-0.4.8/reflex/components/radix/themes/typography/kbd.pyi
--rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.8/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12063 2024-04-04 14:57:26.397447 reflex-0.4.8/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     8701 2024-02-17 20:02:02.447165 reflex-0.4.8/reflex/components/radix/themes/typography/quote.pyi
--rw-r--r--   0        0        0     8563 2024-02-17 20:02:02.447296 reflex-0.4.8/reflex/components/radix/themes/typography/strong.pyi
--rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.8/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-04-04 14:57:26.397579 reflex-0.4.8/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.8/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.8/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.275710 reflex-0.4.8/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.8/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4354 2024-04-12 01:14:12.275922 reflex-0.4.8/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.8/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.276135 reflex-0.4.8/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.8/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.8/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    84151 2024-04-12 01:14:12.276362 reflex-0.4.8/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.8/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-04-04 14:57:26.398259 reflex-0.4.8/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.8/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    22787 2024-04-12 01:14:12.276538 reflex-0.4.8/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.8/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24326 2024-04-12 01:14:12.276828 reflex-0.4.8/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.8/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8535 2024-04-12 01:14:12.277140 reflex-0.4.8/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.8/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.8/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-04-04 14:57:26.398718 reflex-0.4.8/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.8/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.8/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.8/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.8/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.8/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.8/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    11082 2024-04-05 17:14:06.328847 reflex-0.4.8/reflex/config.py
--rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.4.8/reflex/config.pyi
--rw-r--r--   0        0        0     2128 2024-04-12 01:14:12.277275 reflex-0.4.8/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5833 2024-04-12 01:14:12.277500 reflex-0.4.8/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-04-05 17:14:14.462329 reflex-0.4.8/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.8/reflex/constants/colors.py
--rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.4.8/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.8/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.8/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.8/reflex/constants/event.py
--rw-r--r--   0        0        0     3223 2024-04-12 01:14:12.277858 reflex-0.4.8/reflex/constants/installer.py
--rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.8/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.8/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.8/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    31705 2024-04-11 18:27:43.382941 reflex-0.4.8/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    26537 2024-04-12 01:14:12.278011 reflex-0.4.8/reflex/event.py
--rw-r--r--   0        0        0      369 2024-04-12 01:14:12.278154 reflex-0.4.8/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     1647 2024-04-05 17:14:14.462793 reflex-0.4.8/reflex/experimental/hooks.py
--rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.4.8/reflex/experimental/misc.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.8/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.8/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.8/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13116 2024-04-12 01:14:12.278614 reflex-0.4.8/reflex/model.py
--rw-r--r--   0        0        0     1921 2024-04-05 17:14:14.463098 reflex-0.4.8/reflex/page.py
--rw-r--r--   0        0        0    17828 2024-04-12 01:14:12.279090 reflex-0.4.8/reflex/reflex.py
--rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.8/reflex/route.py
--rw-r--r--   0        0        0   105642 2024-04-04 14:57:26.399697 reflex-0.4.8/reflex/state.py
--rw-r--r--   0        0        0     8834 2024-04-04 14:57:26.399846 reflex-0.4.8/reflex/style.py
--rw-r--r--   0        0        0    29808 2024-04-05 17:14:14.463602 reflex-0.4.8/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.8/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.8/reflex/utils/build.py
--rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.4.8/reflex/utils/compat.py
--rw-r--r--   0        0        0     5168 2024-04-12 01:14:12.279640 reflex-0.4.8/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.8/reflex/utils/exceptions.py
--rw-r--r--   0        0        0     9969 2024-04-05 17:14:14.463946 reflex-0.4.8/reflex/utils/exec.py
--rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.4.8/reflex/utils/export.py
--rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.8/reflex/utils/format.py
--rw-r--r--   0        0        0     2277 2024-04-12 01:14:12.280013 reflex-0.4.8/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.8/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    47173 2024-04-15 22:12:45.054777 reflex-0.4.8/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0    10032 2024-04-15 22:12:45.055263 reflex-0.4.8/reflex/utils/processes.py
--rw-r--r--   0        0        0    27674 2024-04-04 14:57:26.400476 reflex-0.4.8/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     8771 2024-04-11 18:27:43.383699 reflex-0.4.8/reflex/utils/serializers.py
--rw-r--r--   0        0        0     4013 2024-04-04 14:57:26.400591 reflex-0.4.8/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    13679 2024-04-12 01:14:12.280735 reflex-0.4.8/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.8/reflex/utils/watch.py
--rw-r--r--   0        0        0    67152 2024-04-04 14:57:26.400899 reflex-0.4.8/reflex/vars.py
--rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.4.8/reflex/vars.pyi
--rw-r--r--   0        0        0    11813 1970-01-01 00:00:00.000000 reflex-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.8a1/LICENSE
+-rw-r--r--   0        0        0     9568 2024-04-05 17:14:14.456384 reflex-0.4.8a1/README.md
+-rw-r--r--   0        0        0     2922 2024-04-12 01:14:24.524384 reflex-0.4.8a1/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.8a1/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.8a1/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-05 17:14:14.457193 reflex-0.4.8a1/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.8a1/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.8a1/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.8a1/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.8a1/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.8a1/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.8a1/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.8a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.8a1/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.8a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.8a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.8a1/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.8a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.8a1/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.8a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.8a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.8a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.8a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.8a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.8a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.8a1/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.8a1/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.8a1/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0    21909 2024-04-12 01:14:12.255596 reflex-0.4.8a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5723 2024-04-05 17:14:14.458168 reflex-0.4.8a1/reflex/__init__.py
+-rw-r--r--   0        0        0     7649 2024-04-06 01:20:11.620853 reflex-0.4.8a1/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.8a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.8a1/reflex/admin.py
+-rw-r--r--   0        0        0    45016 2024-04-12 01:14:12.255992 reflex-0.4.8a1/reflex/app.py
+-rw-r--r--   0        0        0     5010 2024-04-04 14:57:26.376271 reflex-0.4.8a1/reflex/app.pyi
+-rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.8a1/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4250 2024-04-04 14:57:26.376408 reflex-0.4.8a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.8a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17037 2024-04-05 17:14:14.458702 reflex-0.4.8a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.8a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    14024 2024-04-12 01:14:12.256301 reflex-0.4.8a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.8a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.8a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.8a1/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-04-04 14:57:26.376832 reflex-0.4.8a1/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.4.8a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.8a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-04-12 01:14:12.256423 reflex-0.4.8a1/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.8a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-04-12 01:14:12.256750 reflex-0.4.8a1/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.8a1/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3218 2024-04-12 01:14:12.256848 reflex-0.4.8a1/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.8a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6002 2024-04-12 01:14:12.257050 reflex-0.4.8a1/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.8a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-04-12 01:14:12.257244 reflex-0.4.8a1/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.8a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-04-12 01:14:12.257347 reflex-0.4.8a1/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.8a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-04-04 14:57:26.377962 reflex-0.4.8a1/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.8a1/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.8a1/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-04-12 01:14:12.257771 reflex-0.4.8a1/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.8a1/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-04-12 01:14:12.257918 reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-04-12 01:14:12.258034 reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-04-12 01:14:12.258149 reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-04-12 01:14:12.258264 reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12994 2024-04-12 01:14:12.258377 reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.258509 reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-04-12 01:14:12.258649 reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-04-12 01:14:12.258803 reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.8a1/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-04-12 01:14:12.258961 reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-04-12 01:14:12.259114 reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-04-12 01:14:12.259285 reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-04-12 01:14:12.259424 reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.8a1/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.8a1/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-04-12 01:14:12.259528 reflex-0.4.8a1/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-04-12 01:14:12.259726 reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.8a1/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-04-12 01:14:12.259930 reflex-0.4.8a1/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-04-12 01:14:12.260187 reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-04-12 01:14:12.260440 reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.8a1/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.8a1/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-04-12 01:14:12.260613 reflex-0.4.8a1/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-04-12 01:14:12.260767 reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-04-12 01:14:12.260906 reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.380782 reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-04-04 14:57:26.380893 reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.8a1/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-04-12 01:14:12.261047 reflex-0.4.8a1/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.8a1/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-04-04 14:57:26.381120 reflex-0.4.8a1/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.8a1/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-04-12 01:14:12.261180 reflex-0.4.8a1/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-04-12 01:14:12.261417 reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.8a1/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-04-12 01:14:12.261540 reflex-0.4.8a1/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.8a1/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-04-12 01:14:12.261730 reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.8a1/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-04-04 14:57:26.381709 reflex-0.4.8a1/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.4.8a1/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9357 2024-04-12 01:14:12.262316 reflex-0.4.8a1/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.4.8a1/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-04-12 01:14:12.263294 reflex-0.4.8a1/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-04-12 01:14:12.263866 reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.8a1/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-04-04 14:57:26.382156 reflex-0.4.8a1/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.8a1/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.263981 reflex-0.4.8a1/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.8a1/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-04-12 01:14:12.264203 reflex-0.4.8a1/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.8a1/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-04-04 14:57:26.382551 reflex-0.4.8a1/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.382659 reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.8a1/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-04-12 01:14:12.264318 reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.8a1/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-04-12 01:14:12.264413 reflex-0.4.8a1/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.8a1/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-04-12 01:14:12.264513 reflex-0.4.8a1/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.8a1/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-04-12 01:14:12.264634 reflex-0.4.8a1/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.8a1/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-04-12 01:14:12.264741 reflex-0.4.8a1/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.8a1/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-04-12 01:14:12.264933 reflex-0.4.8a1/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.8a1/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-04-12 01:14:12.265035 reflex-0.4.8a1/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.8a1/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-04-12 01:14:12.265136 reflex-0.4.8a1/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.8a1/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-04-12 01:14:12.265267 reflex-0.4.8a1/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.8a1/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-04-12 01:14:12.265632 reflex-0.4.8a1/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.8a1/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.8a1/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-04-12 01:14:12.265841 reflex-0.4.8a1/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.8a1/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-04-12 01:14:12.266058 reflex-0.4.8a1/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.8a1/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-04-04 14:57:26.384173 reflex-0.4.8a1/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.8a1/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-04-12 01:14:12.266197 reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.8a1/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-04-04 14:57:26.384405 reflex-0.4.8a1/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-04-12 01:14:12.266398 reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-04-12 01:14:12.266521 reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.8a1/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-04-12 01:14:12.266681 reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-04-12 01:14:12.266827 reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.8a1/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-04-12 01:14:12.266967 reflex-0.4.8a1/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.8a1/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-04-12 01:14:12.267114 reflex-0.4.8a1/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.8a1/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-04-12 01:14:12.267256 reflex-0.4.8a1/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-04-12 01:14:12.267494 reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.8a1/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.8a1/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-04-12 01:14:12.267618 reflex-0.4.8a1/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.8a1/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-04-12 01:14:12.267722 reflex-0.4.8a1/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.8a1/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-04-12 01:14:12.267821 reflex-0.4.8a1/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.8a1/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-04-12 01:14:12.267927 reflex-0.4.8a1/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    66011 2024-04-12 01:14:12.268153 reflex-0.4.8a1/reflex/components/component.py
+-rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.8a1/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.4.8a1/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    17164 2024-04-04 14:57:26.386284 reflex-0.4.8a1/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.8a1/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-04-12 01:14:12.268957 reflex-0.4.8a1/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.8a1/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6291 2024-04-04 14:19:59.331531 reflex-0.4.8a1/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4642 2024-03-20 23:54:55.842359 reflex-0.4.8a1/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4149 2024-04-04 14:57:26.386549 reflex-0.4.8a1/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.8a1/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.8a1/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-04-04 14:57:26.386705 reflex-0.4.8a1/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.8a1/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.8a1/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.4.8a1/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0     9035 2024-04-12 01:14:12.269123 reflex-0.4.8a1/reflex/components/core/upload.py
+-rw-r--r--   0        0        0     8596 2024-04-12 01:14:12.269265 reflex-0.4.8a1/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.4.8a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-04 14:19:59.332304 reflex-0.4.8a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31107 2024-04-04 14:57:26.387164 reflex-0.4.8a1/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-04-04 14:57:26.387318 reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.4.8a1/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.8a1/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.8a1/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.8a1/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.8a1/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.8a1/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.8a1/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-04-12 01:14:12.269384 reflex-0.4.8a1/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.8a1/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.8a1/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-04-12 01:14:12.269589 reflex-0.4.8a1/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20102 2024-04-05 17:14:14.460921 reflex-0.4.8a1/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99553 2024-04-12 01:14:12.269801 reflex-0.4.8a1/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.8a1/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   164607 2024-04-12 01:14:12.270476 reflex-0.4.8a1/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.8a1/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93567 2024-04-12 01:14:12.270712 reflex-0.4.8a1/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.8a1/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28031 2024-04-12 01:14:12.270995 reflex-0.4.8a1/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.8a1/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42033 2024-04-12 01:14:12.271158 reflex-0.4.8a1/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.8a1/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19615 2024-04-12 01:14:12.271357 reflex-0.4.8a1/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.8a1/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87242 2024-04-12 01:14:12.271561 reflex-0.4.8a1/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.8a1/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    61849 2024-04-12 01:14:12.271965 reflex-0.4.8a1/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.8a1/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89115 2024-04-12 01:14:12.272183 reflex-0.4.8a1/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.8a1/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.8a1/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-04-12 01:14:12.272607 reflex-0.4.8a1/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.8a1/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.8a1/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34237 2024-04-04 14:57:26.389624 reflex-0.4.8a1/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37949 2024-04-12 01:14:12.272820 reflex-0.4.8a1/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.8a1/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    11448 2024-04-05 17:14:14.461428 reflex-0.4.8a1/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5278 2024-04-05 17:14:14.461583 reflex-0.4.8a1/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.8a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.8a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.8a1/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.8a1/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-04-04 14:57:26.390245 reflex-0.4.8a1/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.8a1/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.8a1/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-04-12 01:14:12.273046 reflex-0.4.8a1/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.8a1/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-04-04 14:57:26.390489 reflex-0.4.8a1/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.8a1/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-04-12 01:14:12.273179 reflex-0.4.8a1/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.8a1/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-04-04 14:57:26.390675 reflex-0.4.8a1/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.8a1/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.8a1/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     6865 2024-04-12 01:14:12.273411 reflex-0.4.8a1/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.8a1/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.8a1/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.8a1/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    26885 2024-04-12 01:14:12.273564 reflex-0.4.8a1/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.8a1/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-04-12 01:14:12.273957 reflex-0.4.8a1/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.8a1/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-04-12 01:14:12.274125 reflex-0.4.8a1/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.8a1/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    47939 2024-04-12 01:14:12.274318 reflex-0.4.8a1/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.8a1/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22784 2024-04-12 01:14:12.274470 reflex-0.4.8a1/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.8a1/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16697 2024-04-12 01:14:12.275306 reflex-0.4.8a1/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.8a1/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.8a1/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    24074 2024-04-12 01:14:12.275479 reflex-0.4.8a1/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.8a1/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    21283 2024-04-04 14:57:26.391843 reflex-0.4.8a1/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.8a1/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-04-04 14:57:26.391969 reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0    40237 2024-02-17 20:02:02.428774 reflex-0.4.8a1/reflex/components/radix/themes/components/alertdialog.pyi
+-rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-04-04 14:57:26.392096 reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0     5724 2024-02-17 20:02:02.429087 reflex-0.4.8a1/reflex/components/radix/themes/components/aspectratio.pyi
+-rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-04-04 14:57:26.392242 reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.8a1/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9315 2024-04-04 14:57:26.392362 reflex-0.4.8a1/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.8a1/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11758 2024-04-04 14:57:26.392476 reflex-0.4.8a1/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.8a1/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-04-04 14:57:26.392589 reflex-0.4.8a1/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.8a1/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-04-04 14:57:26.392715 reflex-0.4.8a1/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-04-04 14:57:26.392804 reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-04-04 14:57:26.392918 reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0    44130 2024-02-17 20:02:02.432309 reflex-0.4.8a1/reflex/components/radix/themes/components/contextmenu.pyi
+-rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-04-04 14:57:26.393065 reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-04-04 14:57:26.393223 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0    52185 2024-02-17 20:02:02.435613 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdownmenu.pyi
+-rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-04-04 14:57:26.393356 reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0    26453 2024-02-17 20:02:02.436260 reflex-0.4.8a1/reflex/components/radix/themes/components/hovercard.pyi
+-rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    11916 2024-04-04 14:57:26.393481 reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0    12021 2024-02-17 20:02:02.436631 reflex-0.4.8a1/reflex/components/radix/themes/components/iconbutton.pyi
+-rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.8a1/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-04-04 14:57:26.393614 reflex-0.4.8a1/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.8a1/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-04-04 14:57:26.393725 reflex-0.4.8a1/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-04-04 14:57:26.393848 reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0    26222 2024-03-20 23:54:55.854920 reflex-0.4.8a1/reflex/components/radix/themes/components/radiogroup.pyi
+-rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-04-04 14:57:26.393997 reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     6513 2024-02-17 20:02:02.439025 reflex-0.4.8a1/reflex/components/radix/themes/components/scrollarea.pyi
+-rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.4.8a1/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-04-04 14:57:26.394155 reflex-0.4.8a1/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.8a1/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-04-04 14:57:26.394306 reflex-0.4.8a1/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.8a1/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-04-04 14:57:26.394440 reflex-0.4.8a1/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.8a1/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-04-04 14:57:26.394593 reflex-0.4.8a1/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.8a1/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-04-04 14:57:26.394744 reflex-0.4.8a1/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    17321 2024-04-04 14:57:26.394873 reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-04-04 14:57:26.395020 reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    43043 2024-04-04 14:57:26.395140 reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0    43365 2024-02-17 20:02:02.442188 reflex-0.4.8a1/reflex/components/radix/themes/components/textfield.pyi
+-rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-04-04 14:57:26.395307 reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.4.8a1/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.8a1/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7643 2024-04-04 14:57:26.395455 reflex-0.4.8a1/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.8a1/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-04-04 14:57:26.395640 reflex-0.4.8a1/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.8a1/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.395883 reflex-0.4.8a1/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.8a1/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     6779 2024-04-04 14:57:26.396069 reflex-0.4.8a1/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-04-04 14:57:26.396231 reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-04-04 14:57:26.396387 reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4889 2024-04-04 14:19:59.341578 reflex-0.4.8a1/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    29367 2024-04-04 14:57:26.396553 reflex-0.4.8a1/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.8a1/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-04-04 14:57:26.396712 reflex-0.4.8a1/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.396834 reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-04-04 14:57:26.396967 reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.8a1/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.8a1/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-04-04 14:57:26.397104 reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.8a1/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-04-04 14:57:26.397215 reflex-0.4.8a1/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     8547 2024-02-17 20:02:02.446585 reflex-0.4.8a1/reflex/components/radix/themes/typography/em.pyi
+-rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-04-04 14:57:26.397327 reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     8872 2024-02-17 20:02:02.446866 reflex-0.4.8a1/reflex/components/radix/themes/typography/kbd.pyi
+-rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.8a1/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12063 2024-04-04 14:57:26.397447 reflex-0.4.8a1/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     8701 2024-02-17 20:02:02.447165 reflex-0.4.8a1/reflex/components/radix/themes/typography/quote.pyi
+-rw-r--r--   0        0        0     8563 2024-02-17 20:02:02.447296 reflex-0.4.8a1/reflex/components/radix/themes/typography/strong.pyi
+-rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.8a1/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-04-04 14:57:26.397579 reflex-0.4.8a1/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.8a1/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.8a1/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.275710 reflex-0.4.8a1/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.8a1/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-04-12 01:14:12.275922 reflex-0.4.8a1/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.8a1/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.276135 reflex-0.4.8a1/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.8a1/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.8a1/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84151 2024-04-12 01:14:12.276362 reflex-0.4.8a1/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.8a1/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-04-04 14:57:26.398259 reflex-0.4.8a1/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.8a1/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22787 2024-04-12 01:14:12.276538 reflex-0.4.8a1/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.8a1/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24326 2024-04-12 01:14:12.276828 reflex-0.4.8a1/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.8a1/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-04-12 01:14:12.277140 reflex-0.4.8a1/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.8a1/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.8a1/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-04-04 14:57:26.398718 reflex-0.4.8a1/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.8a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.8a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.8a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.8a1/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.8a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.8a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    11082 2024-04-05 17:14:06.328847 reflex-0.4.8a1/reflex/config.py
+-rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.4.8a1/reflex/config.pyi
+-rw-r--r--   0        0        0     2128 2024-04-12 01:14:12.277275 reflex-0.4.8a1/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5833 2024-04-12 01:14:12.277500 reflex-0.4.8a1/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-04-05 17:14:14.462329 reflex-0.4.8a1/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.8a1/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.4.8a1/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.8a1/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.8a1/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.8a1/reflex/constants/event.py
+-rw-r--r--   0        0        0     3223 2024-04-12 01:14:12.277858 reflex-0.4.8a1/reflex/constants/installer.py
+-rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.8a1/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.8a1/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.8a1/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    31705 2024-04-11 18:27:43.382941 reflex-0.4.8a1/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    26537 2024-04-12 01:14:12.278011 reflex-0.4.8a1/reflex/event.py
+-rw-r--r--   0        0        0      369 2024-04-12 01:14:12.278154 reflex-0.4.8a1/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     1647 2024-04-05 17:14:14.462793 reflex-0.4.8a1/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.4.8a1/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.8a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.8a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.8a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13116 2024-04-12 01:14:12.278614 reflex-0.4.8a1/reflex/model.py
+-rw-r--r--   0        0        0     1921 2024-04-05 17:14:14.463098 reflex-0.4.8a1/reflex/page.py
+-rw-r--r--   0        0        0    17828 2024-04-12 01:14:12.279090 reflex-0.4.8a1/reflex/reflex.py
+-rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.8a1/reflex/route.py
+-rw-r--r--   0        0        0   105642 2024-04-04 14:57:26.399697 reflex-0.4.8a1/reflex/state.py
+-rw-r--r--   0        0        0     8834 2024-04-04 14:57:26.399846 reflex-0.4.8a1/reflex/style.py
+-rw-r--r--   0        0        0    29808 2024-04-05 17:14:14.463602 reflex-0.4.8a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.8a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.8a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.4.8a1/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5168 2024-04-12 01:14:12.279640 reflex-0.4.8a1/reflex/utils/console.py
+-rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.8a1/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0     9969 2024-04-05 17:14:14.463946 reflex-0.4.8a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.4.8a1/reflex/utils/export.py
+-rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.8a1/reflex/utils/format.py
+-rw-r--r--   0        0        0     2277 2024-04-12 01:14:12.280013 reflex-0.4.8a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.8a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    46993 2024-04-12 01:14:12.280227 reflex-0.4.8a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    10050 2024-04-12 01:14:12.280420 reflex-0.4.8a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0    27674 2024-04-04 14:57:26.400476 reflex-0.4.8a1/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     8771 2024-04-11 18:27:43.383699 reflex-0.4.8a1/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     4013 2024-04-04 14:57:26.400591 reflex-0.4.8a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    13679 2024-04-12 01:14:12.280735 reflex-0.4.8a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.8a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    67152 2024-04-04 14:57:26.400899 reflex-0.4.8a1/reflex/vars.py
+-rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.4.8a1/reflex/vars.pyi
+-rw-r--r--   0        0        0    11764 1970-01-01 00:00:00.000000 reflex-0.4.8a1/PKG-INFO
```

### Comparing `reflex-0.4.8/LICENSE` & `reflex-0.4.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/README.md` & `reflex-0.4.8a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/pyproject.toml` & `reflex-0.4.8a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.4.8"
+version = "0.4.8a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.4.8/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.4.8a1/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.4.8a1/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.4.8a1/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.4.8a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.4.8a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/.templates/web/utils/state.js` & `reflex-0.4.8a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/__init__.py` & `reflex-0.4.8a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/__init__.pyi` & `reflex-0.4.8a1/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/app.py` & `reflex-0.4.8a1/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/app.pyi` & `reflex-0.4.8a1/reflex/app.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/app_module_for_backend.py` & `reflex-0.4.8a1/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/base.py` & `reflex-0.4.8a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/compiler/compiler.py` & `reflex-0.4.8a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/compiler/templates.py` & `reflex-0.4.8a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/compiler/utils.py` & `reflex-0.4.8a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/__init__.py` & `reflex-0.4.8a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/app_wrap.py` & `reflex-0.4.8a1/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/app_wrap.pyi` & `reflex-0.4.8a1/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/bare.py` & `reflex-0.4.8a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/body.pyi` & `reflex-0.4.8a1/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/document.py` & `reflex-0.4.8a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/document.pyi` & `reflex-0.4.8a1/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/fragment.pyi` & `reflex-0.4.8a1/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/head.pyi` & `reflex-0.4.8a1/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/link.py` & `reflex-0.4.8a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/link.pyi` & `reflex-0.4.8a1/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/meta.py` & `reflex-0.4.8a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/meta.pyi` & `reflex-0.4.8a1/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/script.py` & `reflex-0.4.8a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/base/script.pyi` & `reflex-0.4.8a1/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/__init__.py` & `reflex-0.4.8a1/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/base.py` & `reflex-0.4.8a1/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/base.pyi` & `reflex-0.4.8a1/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/list.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/table.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/transition.py` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/alert.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/progress.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/spinner.py` & `reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/__init__.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/button.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/button.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/checkbox.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/editable.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/editable.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/email.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/form.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/form.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/input.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/input.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/multiselect.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/numberinput.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/password.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/pininput.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/radio.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/radio.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/select.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/select.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/slider.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/slider.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/switch.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/switch.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/textarea.py` & `reflex-0.4.8a1/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/box.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/box.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/card.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/card.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/center.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/container.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/flex.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/flex.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/grid.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/grid.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/stack.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/stack.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/wrap.py` & `reflex-0.4.8a1/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.4.8a1/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/media/avatar.py` & `reflex-0.4.8a1/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/media/avatar.pyi` & `reflex-0.4.8a1/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/media/icon.py` & `reflex-0.4.8a1/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/media/icon.pyi` & `reflex-0.4.8a1/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/media/image.py` & `reflex-0.4.8a1/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/media/image.pyi` & `reflex-0.4.8a1/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/link.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/link.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/stepper.py` & `reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/__init__.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/drawer.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/menu.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/modal.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/popover.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/typography/heading.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/typography/highlight.py` & `reflex-0.4.8a1/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/typography/span.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/chakra/typography/text.pyi` & `reflex-0.4.8a1/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/component.py` & `reflex-0.4.8a1/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/__init__.py` & `reflex-0.4.8a1/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/banner.py` & `reflex-0.4.8a1/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/banner.pyi` & `reflex-0.4.8a1/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/client_side_routing.py` & `reflex-0.4.8a1/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/client_side_routing.pyi` & `reflex-0.4.8a1/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/colors.py` & `reflex-0.4.8a1/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/cond.py` & `reflex-0.4.8a1/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/debounce.py` & `reflex-0.4.8a1/reflex/components/core/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/debounce.pyi` & `reflex-0.4.8a1/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/foreach.py` & `reflex-0.4.8a1/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/html.py` & `reflex-0.4.8a1/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/html.pyi` & `reflex-0.4.8a1/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/match.py` & `reflex-0.4.8a1/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/responsive.py` & `reflex-0.4.8a1/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/upload.py` & `reflex-0.4.8a1/reflex/components/core/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/core/upload.pyi` & `reflex-0.4.8a1/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/datadisplay/code.py` & `reflex-0.4.8a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/datadisplay/code.pyi` & `reflex-0.4.8a1/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/datadisplay/dataeditor.py` & `reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/datadisplay/logo.py` & `reflex-0.4.8a1/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/constants/html.py` & `reflex-0.4.8a1/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/constants/react.py` & `reflex-0.4.8a1/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/constants/reflex.py` & `reflex-0.4.8a1/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/element.pyi` & `reflex-0.4.8a1/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/__init__.py` & `reflex-0.4.8a1/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/base.py` & `reflex-0.4.8a1/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/base.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/forms.py` & `reflex-0.4.8a1/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/forms.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/inline.py` & `reflex-0.4.8a1/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/inline.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/media.py` & `reflex-0.4.8a1/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/media.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/media.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/metadata.py` & `reflex-0.4.8a1/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/metadata.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/other.py` & `reflex-0.4.8a1/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/other.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/scripts.py` & `reflex-0.4.8a1/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/scripts.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/sectioning.py` & `reflex-0.4.8a1/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/sectioning.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/tables.py` & `reflex-0.4.8a1/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/tables.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/typography.py` & `reflex-0.4.8a1/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/el/elements/typography.pyi` & `reflex-0.4.8a1/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/gridjs/datatable.py` & `reflex-0.4.8a1/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/gridjs/datatable.pyi` & `reflex-0.4.8a1/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/lucide/icon.py` & `reflex-0.4.8a1/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/lucide/icon.pyi` & `reflex-0.4.8a1/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/markdown/markdown.py` & `reflex-0.4.8a1/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/markdown/markdown.pyi` & `reflex-0.4.8a1/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/moment/moment.py` & `reflex-0.4.8a1/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/moment/moment.pyi` & `reflex-0.4.8a1/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/next/base.pyi` & `reflex-0.4.8a1/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/next/image.py` & `reflex-0.4.8a1/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/next/image.pyi` & `reflex-0.4.8a1/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/next/link.pyi` & `reflex-0.4.8a1/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/next/video.py` & `reflex-0.4.8a1/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/next/video.pyi` & `reflex-0.4.8a1/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/plotly/plotly.py` & `reflex-0.4.8a1/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/plotly/plotly.pyi` & `reflex-0.4.8a1/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/accordion.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/base.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/base.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/drawer.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/form.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/form.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/progress.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/progress.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/slider.py` & `reflex-0.4.8a1/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/primitives/slider.pyi` & `reflex-0.4.8a1/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/base.py` & `reflex-0.4.8a1/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/base.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/color_mode.py` & `reflex-0.4.8a1/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/__init__.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/alertdialog.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/aspectratio.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/aspectratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/avatar.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/badge.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/button.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/button.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/callout.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/card.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/card.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/contextmenu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/contextmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/dialog.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/dropdownmenu.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdownmenu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/hovercard.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/hovercard.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/iconbutton.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/inset.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/popover.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/radiogroup.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/radiogroup.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/scrollarea.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/scrollarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/select.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/select.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/separator.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/slider.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/switch.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/table.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/table.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/tabs.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/text_area.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/text_field.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/textfield.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/textfield.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/base.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/container.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/flex.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/grid.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/list.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/stack.py` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/code.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/em.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/em.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/heading.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/kbd.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/kbd.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/link.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/quote.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/quote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/strong.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/strong.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/text.py` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.4.8a1/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/react_player/audio.pyi` & `reflex-0.4.8a1/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/react_player/react_player.py` & `reflex-0.4.8a1/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/react_player/react_player.pyi` & `reflex-0.4.8a1/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/react_player/video.pyi` & `reflex-0.4.8a1/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/__init__.py` & `reflex-0.4.8a1/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/cartesian.py` & `reflex-0.4.8a1/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/cartesian.pyi` & `reflex-0.4.8a1/reflex/components/recharts/cartesian.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/charts.py` & `reflex-0.4.8a1/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/charts.pyi` & `reflex-0.4.8a1/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/general.py` & `reflex-0.4.8a1/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/general.pyi` & `reflex-0.4.8a1/reflex/components/recharts/general.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/polar.py` & `reflex-0.4.8a1/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/polar.pyi` & `reflex-0.4.8a1/reflex/components/recharts/polar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/recharts.py` & `reflex-0.4.8a1/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/recharts/recharts.pyi` & `reflex-0.4.8a1/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/suneditor/editor.py` & `reflex-0.4.8a1/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/suneditor/editor.pyi` & `reflex-0.4.8a1/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/tags/iter_tag.py` & `reflex-0.4.8a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/tags/tag.py` & `reflex-0.4.8a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/components/tags/tagless.py` & `reflex-0.4.8a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/config.py` & `reflex-0.4.8a1/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/config.pyi` & `reflex-0.4.8a1/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/__init__.py` & `reflex-0.4.8a1/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/base.py` & `reflex-0.4.8a1/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/base.pyi` & `reflex-0.4.8a1/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/colors.py` & `reflex-0.4.8a1/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/compiler.py` & `reflex-0.4.8a1/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/config.py` & `reflex-0.4.8a1/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/custom_components.py` & `reflex-0.4.8a1/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/event.py` & `reflex-0.4.8a1/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/installer.py` & `reflex-0.4.8a1/reflex/constants/installer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/route.py` & `reflex-0.4.8a1/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/constants/style.py` & `reflex-0.4.8a1/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/custom_components/custom_components.py` & `reflex-0.4.8a1/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/event.py` & `reflex-0.4.8a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/experimental/hooks.py` & `reflex-0.4.8a1/reflex/experimental/hooks.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/middleware/hydrate_middleware.py` & `reflex-0.4.8a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/middleware/middleware.py` & `reflex-0.4.8a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/model.py` & `reflex-0.4.8a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/page.py` & `reflex-0.4.8a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/reflex.py` & `reflex-0.4.8a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/route.py` & `reflex-0.4.8a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/state.py` & `reflex-0.4.8a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/style.py` & `reflex-0.4.8a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/testing.py` & `reflex-0.4.8a1/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/build.py` & `reflex-0.4.8a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/compat.py` & `reflex-0.4.8a1/reflex/utils/compat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/console.py` & `reflex-0.4.8a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/exec.py` & `reflex-0.4.8a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/export.py` & `reflex-0.4.8a1/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/format.py` & `reflex-0.4.8a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/imports.py` & `reflex-0.4.8a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/path_ops.py` & `reflex-0.4.8a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/prerequisites.py` & `reflex-0.4.8a1/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,25 +564,23 @@
 def update_next_config(export=False, transpile_packages: Optional[List[str]] = None):
     """Update Next.js config from Reflex config.
 
     Args:
         export: if the method run during reflex export.
         transpile_packages: list of packages to transpile via next.config.js.
     """
-    next_config_file = Path(constants.Dirs.WEB, constants.Next.CONFIG_FILE)
+    next_config_file = os.path.join(constants.Dirs.WEB, constants.Next.CONFIG_FILE)
 
     next_config = _update_next_config(
         get_config(), export=export, transpile_packages=transpile_packages
     )
 
-    # Overwriting the next.config.js triggers a full server reload, so make sure
-    # there is actually a diff.
-    orig_next_config = next_config_file.read_text() if next_config_file.exists() else ""
-    if orig_next_config != next_config:
-        next_config_file.write_text(next_config)
+    with open(next_config_file, "w") as file:
+        file.write(next_config)
+        file.write("\n")
 
 
 def _update_next_config(
     config: Config, export: bool = False, transpile_packages: Optional[List[str]] = None
 ):
     next_config = {
         "basePath": config.frontend_path or "",
```

### Comparing `reflex-0.4.8/reflex/utils/processes.py` & `reflex-0.4.8a1/reflex/utils/processes.py`

 * *Files 14% similar despite different names*

```diff
@@ -198,27 +198,21 @@
     Args:
         *fns: The functions to run.
     """
     with run_concurrently_context(*fns):
         pass
 
 
-def stream_logs(
-    message: str,
-    process: subprocess.Popen,
-    progress=None,
-    suppress_errors: bool = False,
-):
+def stream_logs(message: str, process: subprocess.Popen, progress=None):
     """Stream the logs for a process.
 
     Args:
         message: The message to display.
         process: The process.
         progress: The ongoing progress bar if one is being used.
-        suppress_errors: If True, do not exit if errors are encountered (for fallback).
 
     Yields:
         The lines of the process output.
 
     Raises:
         Exit: If the process failed.
     """
@@ -234,15 +228,15 @@
             yield line
 
     # Check if the process failed (not printing the logs for SIGINT).
 
     # Windows uvicorn bug
     # https://github.com/reflex-dev/reflex/issues/2335
     accepted_return_codes = [0, -2, 15] if constants.IS_WINDOWS else [0, -2]
-    if process.returncode not in accepted_return_codes and not suppress_errors:
+    if process.returncode not in accepted_return_codes:
         console.error(f"{message} failed with exit code {process.returncode}")
         for line in logs:
             console.error(line, end="")
         console.error("Run with [bold]--loglevel debug [/bold] for the full log.")
         raise typer.Exit(1)
 
 
@@ -253,24 +247,23 @@
         message: The message to display.
         process: The process.
     """
     for _ in stream_logs(message, process):
         pass
 
 
-def show_status(message: str, process: subprocess.Popen, suppress_errors: bool = False):
+def show_status(message: str, process: subprocess.Popen):
     """Show the status of a process.
 
     Args:
         message: The initial message to display.
         process: The process.
-        suppress_errors: If True, do not exit if errors are encountered (for fallback).
     """
     with console.status(message) as status:
-        for line in stream_logs(message, process, suppress_errors=suppress_errors):
+        for line in stream_logs(message, process):
             status.update(f"{message} {line}")
 
 
 def show_progress(message: str, process: subprocess.Popen, checkpoints: List[str]):
     """Show a progress bar for a process.
 
     Args:
@@ -301,26 +294,33 @@
 
     Args:
         args: A string, or a sequence of program arguments.
         show_status_message: The status message to be displayed in the console.
         fallback: The fallback command to run.
         kwargs: Kwargs to pass to new_process function.
     """
+
+    def execute_process(process):
+        if not constants.IS_WINDOWS:
+            show_status(show_status_message, process)
+        else:
+            process.wait()
+            if process.returncode != 0:
+                error_output = process.stderr if process.stderr else process.stdout
+                error_message = f"Error occurred during subprocess execution: {' '.join(args)}\n{error_output.read() if error_output else ''}"
+                # Only show error in debug mode.
+                if console.is_debug():
+                    console.error(error_message)
+
+                # retry with fallback command.
+                fallback_args = [fallback, *args[1:]] if fallback else None
+                console.warn(
+                    f"There was an error running command: {args}. Falling back to: {fallback_args}."
+                )
+                if fallback_args:
+                    process = new_process(fallback_args, **kwargs)
+                    execute_process(process)
+            else:
+                show_status(show_status_message, process)
+
     process = new_process(args, **kwargs)
-    if fallback is None:
-        # No fallback given, or this _is_ the fallback command.
-        show_status(show_status_message, process)
-    else:
-        # Suppress errors for initial command, because we will try to fallback
-        show_status(show_status_message, process, suppress_errors=True)
-        if process.returncode != 0:
-            # retry with fallback command.
-            fallback_args = [fallback, *args[1:]]
-            console.warn(
-                f"There was an error running command: {args}. Falling back to: {fallback_args}."
-            )
-            run_process_with_fallback(
-                fallback_args,
-                show_status_message=show_status_message,
-                fallback=None,
-                **kwargs,
-            )
+    execute_process(process)
```

### Comparing `reflex-0.4.8/reflex/utils/pyi_generator.py` & `reflex-0.4.8a1/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/serializers.py` & `reflex-0.4.8a1/reflex/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/telemetry.py` & `reflex-0.4.8a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/types.py` & `reflex-0.4.8a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/utils/watch.py` & `reflex-0.4.8a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/vars.py` & `reflex-0.4.8a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/reflex/vars.pyi` & `reflex-0.4.8a1/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8/PKG-INFO` & `reflex-0.4.8a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.4.8
+Version: 0.4.8a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.11.1,<2.0)
 Requires-Dist: build (>=1.0.3,<2.0)
 Requires-Dist: charset-normalizer (>=3.3.2,<4.0)
 Requires-Dist: dill (>=0.3.8,<0.4)
 Requires-Dist: distro (>=1.8.0,<2.0) ; sys_platform == "linux"
 Requires-Dist: fastapi (>=0.96.0,<1.0)
 Requires-Dist: gunicorn (>=20.1.0,<22.0)
```

