# Comparing `tmp/htpy-24.3.9.tar.gz` & `tmp/htpy-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htpy-24.3.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "htpy-24.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `htpy-24.3.9.tar` & `htpy-24.4.0.tar`

### file list

```diff
@@ -1,71 +1,80 @@
--rw-r--r--   0        0        0       57 2024-03-03 13:00:59.192983 htpy-24.3.9/.envrc
--rw-r--r--   0        0        0       46 2024-03-09 13:39:41.722930 htpy-24.3.9/.gitignore
--rw-r--r--   0        0        0     1057 2023-10-29 21:51:04.877884 htpy-24.3.9/LICENSE
--rw-r--r--   0        0        0      322 2024-03-09 20:27:19.833957 htpy-24.3.9/README.md
--rw-r--r--   0        0        0       46 2024-03-10 21:34:04.445438 htpy-24.3.9/allowlist
--rw-r--r--   0        0        0      249 2024-03-03 13:33:34.150382 htpy-24.3.9/conftest.py
--rw-r--r--   0        0        0        9 2024-03-02 19:38:17.864052 htpy-24.3.9/docs/CNAME
--rw-r--r--   0        0        0    17486 2024-03-05 20:59:52.115770 htpy-24.3.9/docs/assets/htpy.webp
--rw-r--r--   0        0        0     3264 2024-03-09 19:38:20.478207 htpy-24.3.9/docs/common-patterns.md
--rw-r--r--   0        0        0     2557 2024-03-09 11:27:32.254799 htpy-24.3.9/docs/django.md
--rw-r--r--   0        0        0     2482 2024-03-09 19:46:12.386823 htpy-24.3.9/docs/faq.md
--rw-r--r--   0        0        0     3100 2024-03-09 20:23:00.454609 htpy-24.3.9/docs/index.md
--rw-r--r--   0        0        0     1767 2024-03-09 19:48:03.051069 htpy-24.3.9/docs/references.md
--rw-r--r--   0        0        0     7101 2024-03-09 14:23:14.104720 htpy-24.3.9/docs/usage.md
--rw-r--r--   0        0        0        0 2024-03-08 20:09:37.710488 htpy-24.3.9/examples/djangoproject/exampleproject/__init__.py
--rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153857 htpy-24.3.9/examples/djangoproject/exampleproject/asgi.py
--rw-r--r--   0        0        0     3215 2024-03-08 21:16:49.814277 htpy-24.3.9/examples/djangoproject/exampleproject/settings.py
--rw-r--r--   0        0        0      952 2024-03-08 21:10:49.153824 htpy-24.3.9/examples/djangoproject/exampleproject/urls.py
--rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153702 htpy-24.3.9/examples/djangoproject/exampleproject/wsgi.py
--rw-r--r--   0        0        0        0 2024-03-08 20:15:31.191691 htpy-24.3.9/examples/djangoproject/form/__init__.py
--rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415543 htpy-24.3.9/examples/djangoproject/form/admin.py
--rw-r--r--   0        0        0      140 2024-03-08 20:55:19.065671 htpy-24.3.9/examples/djangoproject/form/apps.py
--rw-r--r--   0        0        0      551 2024-03-08 21:09:54.963068 htpy-24.3.9/examples/djangoproject/form/components.py
--rw-r--r--   0        0        0       95 2024-03-08 20:31:59.157434 htpy-24.3.9/examples/djangoproject/form/forms.py
--rw-r--r--   0        0        0        0 2024-03-08 20:15:31.193856 htpy-24.3.9/examples/djangoproject/form/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415774 htpy-24.3.9/examples/djangoproject/form/models.py
--rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415536 htpy-24.3.9/examples/djangoproject/form/tests.py
--rw-r--r--   0        0        0      295 2024-03-08 20:30:30.923484 htpy-24.3.9/examples/djangoproject/form/views.py
--rw-r--r--   0        0        0        0 2024-03-08 20:10:21.327962 htpy-24.3.9/examples/djangoproject/index/__init__.py
--rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415912 htpy-24.3.9/examples/djangoproject/index/admin.py
--rw-r--r--   0        0        0      142 2024-03-08 20:15:01.419100 htpy-24.3.9/examples/djangoproject/index/apps.py
--rw-r--r--   0        0        0        0 2024-03-08 20:10:21.330107 htpy-24.3.9/examples/djangoproject/index/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415529 htpy-24.3.9/examples/djangoproject/index/models.py
--rw-r--r--   0        0        0      107 2024-03-08 20:12:51.957222 htpy-24.3.9/examples/djangoproject/index/templates/base.html
--rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415746 htpy-24.3.9/examples/djangoproject/index/tests.py
--rw-r--r--   0        0        0      159 2024-03-08 21:57:51.272614 htpy-24.3.9/examples/djangoproject/index/views.py
--rwxr-xr-x   0        0        0      671 2024-03-08 21:10:49.133835 htpy-24.3.9/examples/djangoproject/manage.py
--rw-r--r--   0        0        0        0 2024-03-08 20:38:21.778715 htpy-24.3.9/examples/djangoproject/widget/__init__.py
--rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415902 htpy-24.3.9/examples/djangoproject/widget/admin.py
--rw-r--r--   0        0        0      144 2024-03-08 20:55:19.065101 htpy-24.3.9/examples/djangoproject/widget/apps.py
--rw-r--r--   0        0        0        0 2024-03-08 20:38:21.780794 htpy-24.3.9/examples/djangoproject/widget/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415928 htpy-24.3.9/examples/djangoproject/widget/models.py
--rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415824 htpy-24.3.9/examples/djangoproject/widget/tests.py
--rw-r--r--   0        0        0      773 2024-03-08 21:14:26.968101 htpy-24.3.9/examples/djangoproject/widget/views.py
--rw-r--r--   0        0        0      348 2024-03-08 21:07:31.025272 htpy-24.3.9/examples/djangoproject/widget/widgets.py
--rw-r--r--   0        0        0     1042 2023-12-11 20:24:46.525531 htpy-24.3.9/examples/htmx_flask.py
--rw-r--r--   0        0        0      177 2024-03-09 20:19:16.408517 htpy-24.3.9/examples/index_example.py
--rw-r--r--   0        0        0     1217 2024-03-09 19:38:31.365824 htpy-24.3.9/examples/structure/boostrap_modal.py
--rw-r--r--   0        0        0      726 2024-03-08 22:27:23.834011 htpy-24.3.9/examples/structure/extends_base.py
--rw-r--r--   0        0        0     1023 2024-03-08 22:36:51.254744 htpy-24.3.9/examples/structure/extends_class.py
--rw-r--r--   0        0        0      384 2024-03-03 13:43:15.955057 htpy-24.3.9/htpy.code-workspace
--rw-r--r--   0        0        0     4195 2024-03-10 21:34:11.537898 htpy-24.3.9/htpy/__init__.py
--rw-r--r--   0        0        0     3443 2024-03-10 21:34:04.445818 htpy-24.3.9/htpy/__init__.pyi
--rw-r--r--   0        0        0     1735 2024-03-07 10:26:38.499381 htpy-24.3.9/htpy/_attrs.py
--rw-r--r--   0        0        0        0 2023-10-29 15:28:12.549039 htpy-24.3.9/htpy/py.typed
--rw-r--r--   0        0        0      543 2024-03-09 20:29:26.894374 htpy-24.3.9/mkdocs.yml
--rw-r--r--   0        0        0     1600 2024-03-09 14:43:49.883001 htpy-24.3.9/pyproject.toml
--rw-r--r--   0        0        0     1256 2024-03-09 13:37:51.172194 htpy-24.3.9/scripts/benchmark_big_table.py
--rwxr-xr-x   0        0        0       65 2024-03-02 18:11:27.585869 htpy-24.3.9/scripts/fix
--rwxr-xr-x   0        0        0       59 2024-03-10 18:34:51.540054 htpy-24.3.9/scripts/release
--rwxr-xr-x   0        0        0      286 2024-03-03 13:37:46.454442 htpy-24.3.9/scripts/test
--rw-r--r--   0        0        0     4187 2024-03-10 12:30:32.366729 htpy-24.3.9/tests/test_attributes.py
--rw-r--r--   0        0        0     2520 2024-03-10 12:31:53.604177 htpy-24.3.9/tests/test_children.py
--rw-r--r--   0        0        0      935 2024-03-10 12:32:49.438483 htpy-24.3.9/tests/test_django.py
--rw-r--r--   0        0        0      351 2024-03-10 18:36:07.188647 htpy-24.3.9/tests/test_element.py
--rw-r--r--   0        0        0      818 2024-03-03 18:10:59.058546 htpy-24.3.9/tests/test_escaping.py
--rw-r--r--   0        0        0      461 2023-11-01 19:49:28.962824 htpy-24.3.9/tests/test_iter.py
--rw-r--r--   0        0        0      371 2024-03-04 12:51:33.461811 htpy-24.3.9/tests/test_jinja2.py
--rw-r--r--   0        0        0      103 2023-11-01 20:01:02.686135 htpy-24.3.9/tests/test_repr.py
--rw-r--r--   0        0        0      592 2024-03-10 21:34:04.446097 htpy-24.3.9/tests/test_types.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 htpy-24.3.9/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-03-03 13:00:59.192983 htpy-24.4.0/.envrc
+-rw-r--r--   0        0        0     1368 2024-04-01 19:45:33.102218 htpy-24.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       46 2024-03-09 13:39:41.722930 htpy-24.4.0/.gitignore
+-rw-r--r--   0        0        0      387 2024-04-01 19:09:58.631500 htpy-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1057 2023-10-29 21:51:04.877884 htpy-24.4.0/LICENSE
+-rw-r--r--   0        0        0      249 2024-03-03 13:33:34.150382 htpy-24.4.0/conftest.py
+-rw-r--r--   0        0        0        9 2024-03-02 19:38:17.864052 htpy-24.4.0/docs/CNAME
+-rw-r--r--   0        0        0     3314 2024-04-13 11:31:46.251728 htpy-24.4.0/docs/README.md
+-rw-r--r--   0        0        0    10024 2024-03-19 21:10:29.686828 htpy-24.4.0/docs/assets/autocomplete.webp
+-rw-r--r--   0        0        0    17486 2024-03-05 20:59:52.115770 htpy-24.4.0/docs/assets/htpy.webp
+-rw-r--r--   0        0        0   233699 2024-03-20 20:47:38.601999 htpy-24.4.0/docs/assets/stream.webm
+-rw-r--r--   0        0        0     4020 2024-03-24 10:36:27.998769 htpy-24.4.0/docs/common-patterns.md
+-rw-r--r--   0        0        0     2947 2024-03-24 10:37:12.658920 htpy-24.4.0/docs/django.md
+-rw-r--r--   0        0        0     2606 2024-04-13 11:39:09.059085 htpy-24.4.0/docs/faq.md
+-rw-r--r--   0        0        0     2062 2024-04-04 19:36:28.687336 htpy-24.4.0/docs/references.md
+-rw-r--r--   0        0        0     2166 2024-03-20 20:13:10.808056 htpy-24.4.0/docs/static-typing.md
+-rw-r--r--   0        0        0     3211 2024-03-21 20:11:01.740542 htpy-24.4.0/docs/streaming.md
+-rw-r--r--   0        0        0     7617 2024-03-21 19:44:49.964800 htpy-24.4.0/docs/usage.md
+-rw-r--r--   0        0        0        0 2024-03-08 20:09:37.710488 htpy-24.4.0/examples/djangoproject/exampleproject/__init__.py
+-rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153857 htpy-24.4.0/examples/djangoproject/exampleproject/asgi.py
+-rw-r--r--   0        0        0     3215 2024-03-08 21:16:49.814277 htpy-24.4.0/examples/djangoproject/exampleproject/settings.py
+-rw-r--r--   0        0        0     1013 2024-04-01 12:33:49.967705 htpy-24.4.0/examples/djangoproject/exampleproject/urls.py
+-rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153702 htpy-24.4.0/examples/djangoproject/exampleproject/wsgi.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:15:31.191691 htpy-24.4.0/examples/djangoproject/form/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415543 htpy-24.4.0/examples/djangoproject/form/admin.py
+-rw-r--r--   0        0        0      140 2024-03-08 20:55:19.065671 htpy-24.4.0/examples/djangoproject/form/apps.py
+-rw-r--r--   0        0        0      745 2024-03-24 10:34:47.760023 htpy-24.4.0/examples/djangoproject/form/components.py
+-rw-r--r--   0        0        0       95 2024-03-08 20:31:59.157434 htpy-24.4.0/examples/djangoproject/form/forms.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:15:31.193856 htpy-24.4.0/examples/djangoproject/form/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415774 htpy-24.4.0/examples/djangoproject/form/models.py
+-rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415536 htpy-24.4.0/examples/djangoproject/form/tests.py
+-rw-r--r--   0        0        0      367 2024-03-24 10:36:12.829689 htpy-24.4.0/examples/djangoproject/form/views.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:10:21.327962 htpy-24.4.0/examples/djangoproject/index/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415912 htpy-24.4.0/examples/djangoproject/index/admin.py
+-rw-r--r--   0        0        0      142 2024-03-08 20:15:01.419100 htpy-24.4.0/examples/djangoproject/index/apps.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:10:21.330107 htpy-24.4.0/examples/djangoproject/index/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415529 htpy-24.4.0/examples/djangoproject/index/models.py
+-rw-r--r--   0        0        0      107 2024-03-08 20:12:51.957222 htpy-24.4.0/examples/djangoproject/index/templates/base.html
+-rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415746 htpy-24.4.0/examples/djangoproject/index/tests.py
+-rw-r--r--   0        0        0      159 2024-03-08 21:57:51.272614 htpy-24.4.0/examples/djangoproject/index/views.py
+-rwxr-xr-x   0        0        0      671 2024-03-08 21:10:49.133835 htpy-24.4.0/examples/djangoproject/manage.py
+-rw-r--r--   0        0        0        0 2024-03-14 20:34:00.963887 htpy-24.4.0/examples/djangoproject/stream/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-19 21:53:26.382528 htpy-24.4.0/examples/djangoproject/stream/admin.py
+-rw-r--r--   0        0        0      144 2024-03-19 21:52:57.553732 htpy-24.4.0/examples/djangoproject/stream/apps.py
+-rw-r--r--   0        0        0      913 2024-03-20 20:22:32.130981 htpy-24.4.0/examples/djangoproject/stream/components.py
+-rw-r--r--   0        0        0      339 2024-03-20 20:21:06.315642 htpy-24.4.0/examples/djangoproject/stream/items.py
+-rw-r--r--   0        0        0        0 2024-03-14 20:34:00.967282 htpy-24.4.0/examples/djangoproject/stream/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-19 21:53:26.382657 htpy-24.4.0/examples/djangoproject/stream/models.py
+-rw-r--r--   0        0        0       26 2024-03-19 21:53:26.382330 htpy-24.4.0/examples/djangoproject/stream/tests.py
+-rw-r--r--   0        0        0     1370 2024-03-21 19:47:35.614427 htpy-24.4.0/examples/djangoproject/stream/views.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:38:21.778715 htpy-24.4.0/examples/djangoproject/widget/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415902 htpy-24.4.0/examples/djangoproject/widget/admin.py
+-rw-r--r--   0        0        0      144 2024-03-08 20:55:19.065101 htpy-24.4.0/examples/djangoproject/widget/apps.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:38:21.780794 htpy-24.4.0/examples/djangoproject/widget/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415928 htpy-24.4.0/examples/djangoproject/widget/models.py
+-rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415824 htpy-24.4.0/examples/djangoproject/widget/tests.py
+-rw-r--r--   0        0        0      773 2024-03-08 21:14:26.968101 htpy-24.4.0/examples/djangoproject/widget/views.py
+-rw-r--r--   0        0        0      348 2024-03-13 19:37:40.202677 htpy-24.4.0/examples/djangoproject/widget/widgets.py
+-rw-r--r--   0        0        0     1042 2024-03-19 21:12:50.744420 htpy-24.4.0/examples/htmx_flask.py
+-rw-r--r--   0        0        0      267 2024-03-20 20:07:03.273126 htpy-24.4.0/examples/index_example.py
+-rw-r--r--   0        0        0      201 2024-03-19 21:22:31.191585 htpy-24.4.0/examples/static_typing/element_example.py
+-rw-r--r--   0        0        0      168 2024-03-19 21:25:09.204789 htpy-24.4.0/examples/static_typing/example_node.py
+-rw-r--r--   0        0        0      195 2024-03-19 21:04:13.715781 htpy-24.4.0/examples/static_typing_example.py
+-rw-r--r--   0        0        0      256 2024-03-21 20:00:01.393186 htpy-24.4.0/examples/stream_callable.py
+-rw-r--r--   0        0        0      321 2024-03-21 20:07:58.631733 htpy-24.4.0/examples/stream_lambda.py
+-rw-r--r--   0        0        0     1272 2024-03-18 21:17:59.006951 htpy-24.4.0/examples/structure/boostrap_modal.py
+-rw-r--r--   0        0        0      726 2024-03-08 22:27:23.834011 htpy-24.4.0/examples/structure/extends_base.py
+-rw-r--r--   0        0        0     1023 2024-03-08 22:36:51.254744 htpy-24.4.0/examples/structure/extends_class.py
+-rw-r--r--   0        0        0      384 2024-03-03 13:43:15.955057 htpy-24.4.0/htpy.code-workspace
+-rw-r--r--   0        0        0    11085 2024-04-16 12:29:47.664497 htpy-24.4.0/htpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 21:34:58.336256 htpy-24.4.0/htpy/py.typed
+-rw-r--r--   0        0        0      633 2024-04-10 07:02:14.977750 htpy-24.4.0/mkdocs.yml
+-rw-r--r--   0        0        0     1652 2024-04-01 19:33:35.137452 htpy-24.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1261 2024-03-13 14:42:01.352552 htpy-24.4.0/scripts/benchmark_big_table.py
+-rw-r--r--   0        0        0     5376 2024-03-20 19:35:24.750356 htpy-24.4.0/tests/test_attributes.py
+-rw-r--r--   0        0        0     4950 2024-04-01 12:53:59.048291 htpy-24.4.0/tests/test_children.py
+-rw-r--r--   0        0        0      896 2024-04-16 12:25:38.663272 htpy-24.4.0/tests/test_django.py
+-rw-r--r--   0        0        0     1099 2024-04-01 19:23:44.608916 htpy-24.4.0/tests/test_element.py
+-rw-r--r--   0        0        0      219 2024-03-12 19:16:25.144993 htpy-24.4.0/tests/test_jinja2.py
+-rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 htpy-24.4.0/PKG-INFO
```

### Comparing `htpy-24.3.9/LICENSE` & `htpy-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/docs/assets/htpy.webp` & `htpy-24.4.0/docs/assets/htpy.webp`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/docs/common-patterns.md` & `htpy-24.4.0/docs/common-patterns.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,86 +15,97 @@
 
 In Django, this means that the view function should not directly generate the
 HTML.
 
 Using a file named `components.py` can be a good idea. If you have many
 components, you may create a `components` package instead.
 
-Your component functions can accept arbitrary argument with the required data:
+Your component functions can accept arbitrary argument with the required data.
+It is a good idea to only use keyword arguments (put a `*` in the argument list
+to force keyword arguments):
 
 ```py title="views.py"
-from django.http import HttpResponse
+from django.http import HttpRequest, HttpResponse
 
-from . import components
+from .components import greeting_page
 
-def greeting(request):
-    return HttpResponse(components.greeting(
+def greeting(request: HttpRequest) -> HttpResponse:
+    return HttpResponse(greeting_page(
         name=request.GET.get("name", "anonymous"),
     ))
 ```
 
 ```py title="components.py"
+from htpy import html, body, h1
 
-def greeting(*, name):
-    return html[body[f"hi {name}!"]]
+def greeting_page(*, name: str) -> Element:
+    return html[body[h1[f"hi {name}!"]]]
 ```
 
-## Creating a base layout
+## Using a base layout
 
 A common feature of template languages is to "extend" a base/parent template and specify placeholders. This can be achieved with a `base_layout` function:
 
 ```py title="components.py"
 import datetime
 
-from htpy import body, div, h1, head, html, p, title
+from htpy import body, div, h1, head, html, p, title, Node, Element
 
 
-def base_layout(*, page_title=None, extra_head=None, content=None, body_class=None):
+def base_page(*,
+    page_title: str | None = None,
+    extra_head: Node = None,
+    content: Node = None,
+    body_class: str | None = None,
+) -> Element:
     return html[
         head[title[page_title], extra_head],
         body(class_=body_class)[
             content,
             div("#footer")[f"Copyright {datetime.date.today().year} by Foo Inc."],
         ],
     ]
 
 
-def index():
-    return base_layout(
+def index_page() -> Element:
+    return base_page(
         page_title="Welcome!",
         body_class="green",
-        content=[h1["Welcome to my site!"], p["Hello and welcome!"]],
+        content=[
+            h1["Welcome to my site!"],
+            p["Hello and welcome!"],
+        ],
     )
 
 
-def about():
-    return base_layout(
+def about_page() -> Element:
+    return base_page(
         page_title="About us",
         content=[
             h1["About us"],
             p["We love creating web sites!"],
         ],
     )
 
 ```
 
 ## UI components
 
-Creating higher level wrappers for common UI components can be a good idea to reduce repitition.
+Creating higher level wrappers for common UI components can be a good idea to reduce repetition.
 
 Wrapping [Bootstrap Modal](https://getbootstrap.com/docs/4.0/components/modal/) could be achieved with a function like this:
 
 
 ```py title="Creating wrapper for Bootstrap Modal"
 from markupsafe import Markup
 
-from htpy import button, div, h5, span
+from htpy import Element, Node, button, div, h5, span
 
 
-def bootstrap_modal(*, title, body=None, footer=None):
+def bootstrap_modal(*, title: str, body: Node = None, footer: Node = None) -> Element:
     return div(".modal", tabindex="-1", role="dialog")[
         div(".modal-dialog", role="document")[
             div(".modal-content")[
                 div(".modal-header")[
                     div(".modal-title")[
                         h5(".modal-title")[title],
                         button(
@@ -107,7 +118,23 @@
                 ],
                 div(".modal-body")[body],
                 footer and div(".modal-footer")[footer],
             ]
         ]
     ]
 ```
+
+You would then use it like this:
+```py
+from htpy import button, p
+
+print(
+    bootstrap_modal(
+        title="Modal title",
+        body=p["Modal body text goes here."],
+        footer=[
+            button(".btn.btn-primary", type="button")["Save changes"],
+            button(".btn.btn-secondary", type="button")["Close"],
+        ],
+    )
+)
+```
```

### Comparing `htpy-24.3.9/docs/django.md` & `htpy-24.4.0/docs/django.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 on how to combine htpy and Django.
 
 ## Returning a htpy response
 htpy elements can be passed directly to `HttpResponse`:
 
 ```py title="views.py"
 from django.http import HttpResponse
-from htpy import div
+from htpy import html, body, div
 
 def my_view(request):
     return HttpResponse(html[body[div["Hi Django!"]]])
 ```
 
 ## Using htpy as part of an existing Django template
 
-htpy elements are marked as "safe" and can be injected directly into Django templates:
+htpy elements are marked as "safe" and can be injected directly into Django
+templates. This can be useful if you want to start using htpy gradually in an
+existing template based Django project:
 
 ```html title="base.html"
 <html>
     <head>
         <title>My Django Site</title>
     </head>
     <body>{{ content }}</body>
@@ -31,69 +33,77 @@
 ```py title="views.py"
 from django.shortcuts import render
 
 from htpy import h1
 
 
 def index(request):
-    return render(request, "base.html", {"content": h1["Welcome to my site!"]})
-
+    return render(request, "base.html", {
+        "content": h1["Welcome to my site!"],
+    })
 ```
 
-## Render a Django form with htpy
+## Render a Django form
 
 CSRF token, form widgets and errors can be directly used within htpy elements:
 
 ```py title="forms.py"
 from django import forms
 
 
 class MyForm(forms.Form):
     name = forms.CharField()
 ```
 
 ```py title="views.py"
-from django.http import HttpResponse
+from django.http import HttpRequest, HttpResponse
 
-from . import components
+from .components import my_form_page, my_form_success_page
 from .forms import MyForm
 
 
-def my_form(request):
+def my_form(request: HttpRequest) -> HttpResponse:
     form = MyForm(request.POST or None)
     if form.is_valid():
-        return HttpResponse(components.my_form_success())
+        return HttpResponse(my_form_success_page())
+
+    return HttpResponse(my_form_page(request, my_form=form))
 
-    return HttpResponse(components.my_form(request, form))
 ```
 
 ```py title="components.py"
+from django.http import HttpRequest
 from django.template.backends.utils import csrf_input
 
-from htpy import body, button, form, h1, head, html, title
+from htpy import Element, Node, body, button, form, h1, head, html, title
+
+from .forms import MyForm
 
 
-def base(page_title, content):
-    return html[head[title[page_title]], body[content]]
+def base_page(page_title: str, content: Node) -> Element:
+    return html[
+        head[title[page_title]],
+        body[content],
+    ]
 
 
-def my_form(request, my_form):
-    return base(
+def my_form_page(request: HttpRequest, *, my_form: MyForm) -> Element:
+    return base_page(
         "My form",
         form(method="post")[
             csrf_input(request),
             my_form.errors,
             my_form["name"],
             button["Submit!"],
         ],
     )
 
 
-def my_form_success():
-    return base(
+def my_form_success_page() -> Element:
+    return base_page(
         "Success!",
         h1["Success! The form was valid!"],
     )
 ```
 
 
 ## Implement custom form widgets with htpy
```

### Comparing `htpy-24.3.9/docs/faq.md` & `htpy-24.4.0/docs/faq.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 ## Can htpy generate XML/XHTML?
 
 No. Generating XML/XHTML is out of scope for this project. Use a XML library if
 you are looking to generate XML.
 
 htpy generates HTML, therefore "void elements" such as `<br>` does not include a trailing `/`.
 
-## Does not generating HTML from Python means that mixing up concerns between presentation and business logic?
+If you are looking to generate generic XML, [`lxml.builder`](https://lxml.de/apidoc/lxml.builder.html) could be a good alternative.
 
-With a template language, create HTML markup in separate files is enforced by
+## Does not generating HTML from Python mean mixing concerns between presentation and business logic?
+
+With a template language, putting HTML markup in separate files is enforced by
 design. Avoiding logic in the presentation layer is also mostly done by making
 the language very restrictive.
 
 It takes a little bit of planning and effort, but it is possible to have a
 nicely separated presentation layer that is free from logic. See [Common
 patterns](common-patterns.md) for more details on how you can structure your
 project.
 
-
 ## What kind of black magic makes `from htpy import whatever_element` work?
 
 htpy uses the [module level `__getattr__`](https://docs.python.org/3/reference/datamodel.html#customizing-module-attribute-access). It was [introduced in Python 3.7](https://docs.python.org/3/whatsnew/3.7.html#pep-562-customization-of-access-to-module-attributes). It allows [creating `Element` instances](https://github.com/pelme/htpy/blob/855a2a6648ce955be9730fe030a97930df42930a/htpy/__init__.py#L146-L147) for any elements that are imported.
 
 
-## Why does htpy not provide HTML like tag syntax with angel brackets like pyxl and JSX?
+## Why does htpy not provide HTML like tag syntax with angle brackets like pyxl and JSX?
 
 htpy must be compatible with standard Python code formatters, editors and static
 type checkers. Unfortunately, it is not possible to support those workflows with a custom
 syntax without a massive effort to change those tools to support that syntax.
```

### Comparing `htpy-24.3.9/docs/references.md` & `htpy-24.4.0/docs/references.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 htpy was heavily inspired by many other libraries and articles. This page lists some of them.
 
 ## Similar libraries and tools
 
 - [JSX/React](https://legacy.reactjs.org/docs/introducing-jsx.html) - Made writing HTML in a programming language popular.
 - [pyxl](https://github.com/dropbox/pyxl), [pyxl3](https://github.com/gvanrossum/pyxl3), [pyxl4](https://github.com/pyxl4/pyxl4) - Write HTML in Python with JSX-like syntax. Not actively maintained.
 - [htbuilder](https://github.com/tvst/htbuilder/) - Very similar to htpy but does not currently support automatic escaping.
-- [breve](https://github.com/cwells/breve) - An early implementation of HTML in Python. Using getattr `[]` syntax for children. Not actively maintained.
+- [nevow.stan](https://github.com/twisted/nevow/blob/master/nevow/stan.py) - Probably the earliest use of `[]` syntax for specifying children. Not actively maintained.
+- [breve](https://github.com/cwells/breve) - Another early implementation of HTML in Python,  Using getattr `[]` syntax for children. Not actively maintained.
 - [hyperscript](https://github.com/hyperhype/hyperscript) - JavaScript library that also uses CSS selector-like syntax for specifying id and classes.
 - [hyperpython](https://github.com/ejplatform/hyperpython) - A Python interpretation of hyperscript. Not actively maintained.
 - [h by Adam Johnson](https://github.com/adamchainz/h) - Similar to htpy, uses call syntax (`()`) for attributes and getitem (`[]`) for children.
+- [lxml.builder](https://lxml.de/apidoc/lxml.builder.html) - lxml's `E` allows creating XML/XHTML documents from Python.
 
 ## Articles about HTML generation without templates
 - [Jeff Atwood - You're Doing It Wrong](https://blog.codinghorror.com/youre-doing-it-wrong/) - Stack Overflow co-founder Jeff Atwood
 - [Tavis Rudd - Throw out your templates](https://github.com/tavisrudd/throw_out_your_templates) - Tavis Rudd, creator of Python template language "Cheetah" argues for creating HTML without templates.
 - [David Ford - 80% of my coding is doing this (or why templates are dead)](https://codeburst.io/80-of-my-coding-is-doing-this-or-why-templates-are-dead-b640fc149e22) - Discusses various techniques for rendering HTML.
```

### Comparing `htpy-24.3.9/docs/usage.md` & `htpy-24.4.0/docs/usage.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 >>> user_supplied_name = "bobby </h1>"
 >>> print(h1[f"hello {user_supplied_name}"])
 <h1>hello bobby &lt;/h1&gt;</h1>
 ```
 
 ### Conditional rendering
 
-`None` and `False` will not render anything. This can be useful to conditionally render some content.
+`None` will not render anything. This can be useful to conditionally render some content.
 
 ```pycon title="Conditional rendering"
 
 >>> from htpy import div, b
 >>> error = None
 
 >>> # No <b> tag will be rendered since error is None
@@ -67,14 +67,20 @@
 
 ```pycon title="Iterate over a generator"
 >>> from htpy import ul, li
 >>> print(ul[(li[letter] for letter in "abc")])
 <ul><li>a</li><li>b</li><li>c</li></ul>
 ```
 
+!!! note
+
+    The generator will be lazily evaluated when rendering the element, not
+    directly when the element is constructed. See [Streaming](streaming.md) for
+    more information.
+
 A `list` can be used similar to a [JSX fragment](https://react.dev/reference/react/Fragment):
 
 ```pycon title="Render a list of child elements"
 >>> from htpy import div, img
 >>> my_images = [img(src="a.jpg"), img(src="b.jpg")]
 >>> print(div[my_images])
 <div><img src="a.jpg"><img src="b.jpg"></div>
@@ -147,28 +153,26 @@
 >>> print(img(src="picture.jpg"))
 <img src="picture.jpg">
 ```
 
 In Python, `class` and `for` cannot be used as keyword arguments. Instead, they can be specified as `class_` or `for_` when using keyword arguments:
 
 ```pycon
->>> from htpy import img
+>>> from htpy import label
 >>> print(label(for_="myfield"))
 <label for="myfield"></label>
 ```
 
 Attributes that contains dashes `-` can be specified using underscores:
 ```pycon
 >>> from htpy import form
 >>> print(form(hx_post="/foo"))
 <form hx-post="/foo"></form>
 ```
 
-If you need attributes
-
 
 ### id/class shorthand
 
 Defining `id` and `class` attributes is common when writing HTML. A string shorthand
 that looks like a CSS selector can be used to quickly define id and classes:
 
 ```pycon title="Define id"
@@ -248,7 +252,24 @@
 
 ```pycon title="Specifying attribute via multiple arguments"
 >>> from htyp import label
 >>> print(label("#myid.foo.bar", {'for': "somefield"}, name="myname",))
 <label id="myid" class="foo bar" for="somefield" name="myname"></label>
 ```
 
+## Iterating of the output
+
+Iterating over a htpy element will yield the resulting contents in chunks as
+they are rendered:
+
+```pycon
+>>> from htpy import ul, li
+>>> for chunk in ul[li["a", "b"]]:
+...     print(f"got a chunk: {chunk!r}")
+...
+got a chunk: '<ul>'
+got a chunk: '<li>'
+got a chunk: 'a'
+got a chunk: 'b'
+got a chunk: '</li>'
+got a chunk: '</ul>'
+```
```

#### html2text {}

```diff
@@ -14,32 +14,34 @@
 ************ WWeellccoommee ttoo mmyy ssiittee!! ************
 ``` Strings are automatically escaped to avoid [XSS vulnerabilities](https://
 owasp.org/www-community/attacks/xss/). It is convenient and safe to directly
 insert variable data via f-strings: ```pycon >>> from htpy import h1 >>>
 user_supplied_name = "bobby
 " >>> print(h1[f"hello {user_supplied_name}"])
 ************ hheelllloo bboobbbbyy <<//hh11>> ************
-``` ### Conditional rendering `None` and `False` will not render anything. This
-can be useful to conditionally render some content. ```pycon title="Conditional
+``` ### Conditional rendering `None` will not render anything. This can be
+useful to conditionally render some content. ```pycon title="Conditional
 rendering" >>> from htpy import div, b >>> error = None >>> # No ttaagg wwiillll bbee
 rreennddeerreedd ssiinnccee eerrrroorr iiss NNoonnee >>>>>> pprriinntt((ddiivv[[eerrrroorr aanndd bb[[eerrrroorr]]]]))
 >>> error = 'Enter a valid email address.' >>> print(div[error and b[error]])
 EEnntteerr aa vvaalliidd eemmaaiill aaddddrreessss..
 # Inline if/else can also be used: >>> print(div[b[error] if error else None])
 EEnntteerr aa vvaalliidd eemmaaiill aaddddrreessss..
 ``` ### Loops / iterating over children You can pass a list, tuple or generator
 to generate multiple children: ```pycon title="Iterate over a generator" >>>
 from htpy import ul, li >>> print(ul[(li[letter] for letter in "abc")])
     * a
     * b
     * c
-``` A `list` can be used similar to a [JSX fragment](https://react.dev/
-reference/react/Fragment): ```pycon title="Render a list of child elements" >>>
-from htpy import div, img >>> my_images = [img(src="a.jpg"), img(src="b.jpg")]
->>> print(div[my_images])
+``` !!! note The generator will be lazily evaluated when rendering the element,
+not directly when the element is constructed. See [Streaming](streaming.md) for
+more information. A `list` can be used similar to a [JSX fragment](https://
+react.dev/reference/react/Fragment): ```pycon title="Render a list of child
+elements" >>> from htpy import div, img >>> my_images = [img(src="a.jpg"), img
+(src="b.jpg")] >>> print(div[my_images])
 [a.jpg][b.jpg]
 ``` ### Custom elements / web components [Custom elements / web components]
 (https://developer.mozilla.org/en-US/docs/Web/API/Web_components/
 Using_custom_elements) are HTML elements that contains at least one dash (`-`).
 Since `-` cannot be used in Python identifiers, use underscore (`_`) instead:
 ```pycon title="Using custom elements" >>> from htpy import my_custom_element
 >>> print(my_custom_element['hi!']) hi! ``` ### Injecting markup If you have
@@ -61,22 +63,22 @@
 Some elements do not have attributes, they can be specified by just the element
 itself: ```pycon >>> from htpy import hr >>> print(hr)
 ===============================================================================
 ``` ### Keyword arguments Attributes can be specified via keyword arguments:
 ```pycon >>> from htpy import img >>> print(img(src="picture.jpg"))
 [picture.jpg]``` In Python, `class` and `for` cannot be used as keyword
 arguments. Instead, they can be specified as `class_` or `for_` when using
-keyword arguments: ```pycon >>> from htpy import img >>> print(label
+keyword arguments: ```pycon >>> from htpy import label >>> print(label
 (for_="myfield")) ``` Attributes that contains dashes `-` can be specified
 using underscores: ```pycon >>> from htpy import form >>> print(form(hx_post="/
 foo"))
-``` If you need attributes ### id/class shorthand Defining `id` and `class`
-attributes is common when writing HTML. A string shorthand that looks like a
-CSS selector can be used to quickly define id and classes: ```pycon
-title="Define id" >>> from htpy import div >>> print(div("#myid"))
+``` ### id/class shorthand Defining `id` and `class` attributes is common when
+writing HTML. A string shorthand that looks like a CSS selector can be used to
+quickly define id and classes: ```pycon title="Define id" >>> from htpy import
+div >>> print(div("#myid"))
 ``` ```pycon title="Define multiple classes" >>> from htpy import div >>> print
 (div(".foo.bar"))
 ``` ```pycon title="Combining both id and classes" >>> from htpy import div >>>
 print(div("#myid.foo.bar"))
 ``` ### Attributes as dict Attributes can also be specified as a `dict`. This
 is useful when using attributes that are reserved Python keywords (like `for`
 or `class`), when the attribute name contains a dash (`-`) or when you want to
@@ -94,8 +96,15 @@
 accepts a list of class names or a dict. Falsey values will be ignored.
 ```pycon >>> from htpy import button >>> is_primary = True >>> print(button
 (class_=["btn", {"btn-primary": is_primary}])) >>> is_primary = False >>> print
 (button(class_=["btn", {"btn-primary": is_primary}])) >>> ``` ### Combining
 modes Attributes via id/class shorthand, keyword arguments and dictionary can
 be combined: ```pycon title="Specifying attribute via multiple arguments" >>>
 from htyp import label >>> print(label("#myid.foo.bar", {'for': "somefield"},
-name="myname",)) ```
+name="myname",)) ``` ## Iterating of the output Iterating over a htpy element
+will yield the resulting contents in chunks as they are rendered: ```pycon >>>
+from htpy import ul, li >>> for chunk in ul[li["a", "b"]]: ... print(f"got a
+chunk: {chunk!r}") ... got a chunk: '
+    * ' got a chunk: '
+    * ' got a chunk: 'a' got a chunk: 'b' got a chunk: '
+    * ' got a chunk: '
+' ```
```

### Comparing `htpy-24.3.9/examples/djangoproject/exampleproject/settings.py` & `htpy-24.4.0/examples/djangoproject/exampleproject/settings.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/examples/djangoproject/exampleproject/urls.py` & `htpy-24.4.0/examples/djangoproject/exampleproject/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 
 from django.contrib import admin
 from django.urls import path
 from form.views import my_form
 from index.views import index
+from stream.views import stream
 from widget.views import widget_view
 
 urlpatterns = [
     path("", index),
     path("form/", my_form),
     path("widget/", widget_view),
+    path("stream/", stream),
     path("admin/", admin.site.urls),
 ]
```

### Comparing `htpy-24.3.9/examples/djangoproject/manage.py` & `htpy-24.4.0/examples/djangoproject/manage.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/examples/djangoproject/widget/views.py` & `htpy-24.4.0/examples/djangoproject/widget/views.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/examples/htmx_flask.py` & `htpy-24.4.0/examples/htmx_flask.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/examples/structure/boostrap_modal.py` & `htpy-24.4.0/examples/structure/boostrap_modal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from markupsafe import Markup
 
-from htpy import button, div, h5, span
+from htpy import Element, Node, button, div, h5, span
 
 
-def bootstrap_modal(*, title, body=None, footer=None):
+def bootstrap_modal(*, title: str, body: Node = None, footer: Node = None) -> Element:
     return div(".modal", tabindex="-1", role="dialog")[
         div(".modal-dialog", role="document")[
             div(".modal-content")[
                 div(".modal-header")[
                     div(".modal-title")[
                         h5(".modal-title")[title],
                         button(
@@ -22,15 +22,15 @@
                 footer and div(".modal-footer")[footer],
             ]
         ]
     ]
 
 
 if __name__ == "__main__":
-    from htpy import p
+    from htpy import button, p
 
     print(
         bootstrap_modal(
             title="Modal title",
             body=p["Modal body text goes here."],
             footer=[
                 button(".btn.btn-primary", type="button")["Save changes"],
```

### Comparing `htpy-24.3.9/examples/structure/extends_base.py` & `htpy-24.4.0/examples/structure/extends_base.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/examples/structure/extends_class.py` & `htpy-24.4.0/examples/structure/extends_class.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.9/mkdocs.yml` & `htpy-24.4.0/mkdocs.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 site_name: htpy - HTML in Python
 repo_url: https://github.com/pelme/htpy
 theme:
   name: material
   features:
     - content.code.copy
+    - toc.integrate
   palette:
     scheme: slate
   icon:
     logo: material/code-tags
 nav:
-  - index.md
+  - README.md
   - usage.md
   - common-patterns.md
+  - static-typing.md
   - django.md
+  - streaming.md
   - faq.md
   - references.md
 markdown_extensions:
   - admonition
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
   - attr_list
   - md_in_html
+  - toc:
+      permalink: true
```

### Comparing `htpy-24.3.9/scripts/benchmark_big_table.py` & `htpy-24.4.0/scripts/benchmark_big_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 </table>
 """
 
 
 tests = [
     (
         "htpy",
-        lambda rows: str(table[thead[tr[th["Row #"]]], tbody[(tr[td[row]] for row in rows)]]),
+        lambda rows: str(table[thead[tr[th["Row #"]]], tbody[(tr[td[str(row)]] for row in rows)]]),
     ),
     (
         "django",
         lambda rows: DjangoTemplate(django_jinja_template).render(Context({"rows": rows})),
     ),
     ("jinja2", lambda rows: JinjaTemplate(django_jinja_template).render(rows=rows)),
 ]
```

### Comparing `htpy-24.3.9/tests/test_django.py` & `htpy-24.4.0/tests/test_django.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pytest
 from django.forms.utils import ErrorList
 from django.template import Context, Template
-from django.utils.html import escape as django__escape
-from django.utils.safestring import SafeString as django__SafeString
+from django.utils.html import escape
+from django.utils.safestring import SafeString
 
 from htpy import div, li, ul
 
 pytestmark = pytest.mark.usefixtures("django_env")
 
 
 def test_template_injection() -> None:
     t = Template("<ul>{{ stuff }}</ul>")
-    result = t.render(Context({"stuff": li["I am safe!"]}))
+    result = t.render(Context({"stuff": li(id="hi")["I am safe!"]}))
 
-    assert result == "<ul><li>I am safe!</li></ul>"
+    assert result == '<ul><li id="hi">I am safe!</li></ul>'
 
 
 def test_SafeString() -> None:
-    result = ul[django__SafeString("<li>hello</li>")]
+    result = ul[SafeString("<li>hello</li>")]
     assert str(result) == "<ul><li>hello</li></ul>"
 
 
 def test_explicit_escape() -> None:
-    result = ul[django__escape("<hello>")]
+    result = ul[escape("<hello>")]
     assert str(result) == "<ul>&lt;hello&gt;</ul>"
 
 
 def test_errorlist() -> None:
     result = div[ErrorList(["my error"])]
     assert str(result) == """<div><ul class="errorlist"><li>my error</li></ul></div>"""
```

