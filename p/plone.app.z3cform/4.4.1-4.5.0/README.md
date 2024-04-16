# Comparing `tmp/plone.app.z3cform-4.4.1.tar.gz` & `tmp/plone.app.z3cform-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.z3cform-4.4.1.tar", last modified: Tue Feb 27 16:11:32 2024, max compression
+gzip compressed data, was "plone.app.z3cform-4.5.0.tar", last modified: Tue Mar 19 21:33:45 2024, max compression
```

## Comparing `plone.app.z3cform-4.4.1.tar` & `plone.app.z3cform-4.5.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.890526 plone.app.z3cform-4.4.1/
--rw-r--r--   0 maurits    (501) staff       (20)    26489 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    50353 2024-02-27 16:11:32.890104 plone.app.z3cform-4.4.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13825 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.856748 plone.app.z3cform-4.4.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      749 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.857190 plone.app.z3cform-4.4.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.860540 plone.app.z3cform-4.4.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.866484 plone.app.z3cform-4.4.1/plone/app/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1965 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18525 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)     1312 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/converters.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      724 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      110 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     2349 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/inline_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7480 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/inline_validation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3859 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      212 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.852449 plone.app.z3cform-4.4.1/plone/app/z3cform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.867147 plone.app.z3cform-4.4.1/plone/app/z3cform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      163 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      635 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.878602 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      435 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/ajaxselect_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1560 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/contentprovider-widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)      324 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/date_time_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      280 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/email_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      209 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/error.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3452 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/file_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      829 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3560 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/image_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      677 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3356 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/link_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9654 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4033 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/multi_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1861 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/object_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2703 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      283 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/password_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      583 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/radio_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      937 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/radio_input_single.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/relateditems_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      295 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/richtext_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1465 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/select_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      976 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/singlecheckbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      290 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/singlecheckboxbool_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      371 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1380 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/singlecheckboxbool_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      334 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/submit_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      279 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/text_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      286 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/textarea_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      296 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/textlines_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1809 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/templates/widget.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.881450 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2421 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     7951 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     4921 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    69053 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1966 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     6162 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1657 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/views.py
--rw-r--r--   0 maurits    (501) staff       (20)     2961 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.886885 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5004 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/base.py
--rw-r--r--   0 maurits    (501) staff       (20)      728 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/checkbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     3579 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/datetime.py
--rw-r--r--   0 maurits    (501) staff       (20)      535 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/email.py
--rw-r--r--   0 maurits    (501) staff       (20)     2018 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/link.py
--rw-r--r--   0 maurits    (501) staff       (20)      901 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/orderedselect.py
--rw-r--r--   0 maurits    (501) staff       (20)      598 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/password.py
--rw-r--r--   0 maurits    (501) staff       (20)     9722 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     2051 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/querystring.py
--rw-r--r--   0 maurits    (501) staff       (20)      750 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/radio.py
--rw-r--r--   0 maurits    (501) staff       (20)     8104 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/relateditems.py
--rw-r--r--   0 maurits    (501) staff       (20)     5437 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     8792 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/select.py
--rw-r--r--   0 maurits    (501) staff       (20)     3165 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/singlecheckbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     1311 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/submit.py
--rw-r--r--   0 maurits    (501) staff       (20)     1449 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/text.py
--rw-r--r--   0 maurits    (501) staff       (20)    13282 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/widgets.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.887425 plone.app.z3cform-4.4.1/plone/app/z3cform/wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)      273 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/wysiwyg/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      391 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone/app/z3cform/wysiwyg/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:11:32.887836 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    50353 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3461 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      609 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4250 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-02-27 16:11:32.890606 plone.app.z3cform-4.4.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2661 2024-02-27 16:11:32.000000 plone.app.z3cform-4.4.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.529843 plone.app.z3cform-4.5.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    27209 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    51122 2024-03-19 21:33:45.529161 plone.app.z3cform-4.5.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13825 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.485195 plone.app.z3cform-4.5.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.485636 plone.app.z3cform-4.5.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.489431 plone.app.z3cform-4.5.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.496868 plone.app.z3cform-4.5.0/plone/app/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1965 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18525 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1312 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/converters.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      110 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2349 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/inline_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7480 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/inline_validation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3859 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.480244 plone.app.z3cform-4.5.0/plone/app/z3cform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.497826 plone.app.z3cform-4.5.0/plone/app/z3cform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.511574 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      435 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/ajaxselect_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1560 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/checkbox_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/contentprovider-widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      324 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/date_time_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      280 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/email_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3712 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/file_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3820 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/image_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3356 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/link_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9654 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4033 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/multi_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1861 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/object_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2703 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/orderedselect_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      283 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/password_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      583 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/radio_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      937 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/radio_input_single.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/relateditems_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      295 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/richtext_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1465 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/select_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/singlecheckbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      290 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      371 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1380 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      334 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/submit_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      279 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/text_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      286 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/textarea_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      296 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/textlines_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1809 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/templates/widget.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.515909 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2421 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1139 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7951 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4921 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    69170 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1966 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6162 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1657 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2961 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.524072 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5004 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/checkbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3579 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/datetime.py
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/email.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2018 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/link.py
+-rw-r--r--   0 maurits    (501) staff       (20)      901 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/orderedselect.py
+-rw-r--r--   0 maurits    (501) staff       (20)      598 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/password.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9722 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2051 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/querystring.py
+-rw-r--r--   0 maurits    (501) staff       (20)      750 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/radio.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8104 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/relateditems.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5437 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8840 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/select.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3165 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/singlecheckbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1311 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/submit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1449 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/text.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13282 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/widgets.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.524985 plone.app.z3cform-4.5.0/plone/app/z3cform/wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)      273 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/wysiwyg/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      391 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/plone/app/z3cform/wysiwyg/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:33:45.525565 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    51122 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3461 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      643 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-19 21:33:45.000000 plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4448 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-03-19 21:33:45.529971 plone.app.z3cform-4.5.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2706 2024-03-19 21:33:44.000000 plone.app.z3cform-4.5.0/setup.py
```

### Comparing `plone.app.z3cform-4.4.1/CHANGES.rst` & `plone.app.z3cform-4.5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,43 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.5.0 (2024-03-19)
+------------------
+
+New features:
+
+
+- Add support for the "accept" attribute on file inputs.
+
+  If the widget's field - if there is one - has the "accept" attribute set (the
+  `NamedImage` field has `image/*` set by default) then this is rendered as an
+  `accept` attribute on the file input.
+
+  This would restrict the allowed file types before uploading while still being
+  checked on the server side.
+
+  Fixes: https://github.com/plone/plone.formwidget.namedfile/issues/66
+  Depends on:
+  - https://github.com/plone/plone.namedfile/pull/158
+  - https://github.com/plone/plone.formwidget.namedfile/pull/67
+  [thet] (#198)
+
+
+Bug fixes:
+
+
+- Fix `SelectFieldWidget` factory call.
+  [petschki] (#192)
+
+
 4.4.1 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Add missing ``pattern_options`` multiadapter to new PatternFormElement base class.
```

### Comparing `plone.app.z3cform-4.4.1/PKG-INFO` & `plone.app.z3cform-4.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.4.1
+Version: 4.5.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: plone.app.textfield>=1.3.6
 Requires-Dist: plone.base
 Requires-Dist: plone.app.contentlisting
+Requires-Dist: plone.formwidget.namedfile>=3.1.0
 Requires-Dist: plone.i18n
 Requires-Dist: plone.protect
 Requires-Dist: plone.registry
 Requires-Dist: plone.schema
 Requires-Dist: plone.uuid
 Requires-Dist: plone.z3cform
 Requires-Dist: Products.GenericSetup
@@ -689,14 +690,43 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.5.0 (2024-03-19)
+------------------
+
+New features:
+
+
+- Add support for the "accept" attribute on file inputs.
+
+  If the widget's field - if there is one - has the "accept" attribute set (the
+  `NamedImage` field has `image/*` set by default) then this is rendered as an
+  `accept` attribute on the file input.
+
+  This would restrict the allowed file types before uploading while still being
+  checked on the server side.
+
+  Fixes: https://github.com/plone/plone.formwidget.namedfile/issues/66
+  Depends on:
+  - https://github.com/plone/plone.namedfile/pull/158
+  - https://github.com/plone/plone.formwidget.namedfile/pull/67
+  [thet] (#198)
+
+
+Bug fixes:
+
+
+- Fix `SelectFieldWidget` factory call.
+  [petschki] (#192)
+
+
 4.4.1 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Add missing ``pattern_options`` multiadapter to new PatternFormElement base class.
```

### Comparing `plone.app.z3cform-4.4.1/README.rst` & `plone.app.z3cform-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/docs/LICENSE.GPL` & `plone.app.z3cform-4.5.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/docs/LICENSE.txt` & `plone.app.z3cform-4.5.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/configure.zcml` & `plone.app.z3cform-4.5.0/plone/app/z3cform/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/converters.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/converters.zcml` & `plone.app.z3cform-4.5.0/plone/app/z3cform/converters.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/csrf.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/inline_validation.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/inline_validation.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/inline_validation.rst` & `plone.app.z3cform-4.5.0/plone/app/z3cform/inline_validation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/interfaces.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/profiles.zcml` & `plone.app.z3cform-4.5.0/plone/app/z3cform/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/checkbox_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/file_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/image_input.pt`

 * *Files 7% similar despite different names*

```diff
@@ -18,19 +18,22 @@
           tal:condition="up_id"
   >
     <input name="${view/name}.file_upload_id"
            type="hidden"
            value="${up_id}"
     />
     <span>
-      <tal:i18n i18n:translate="file_already_uploaded">File already uploaded:</tal:i18n>
+      <tal:i18n i18n:translate="image_already_uploaded">Image already uploaded:</tal:i18n>
         ${filename}
     </span>
   </tal:if>
   <span tal:condition="python:exists and download_url and action=='nochange'">
+    <a href="${download_url}">
+      <img tal:replace="structure view/thumb_tag" />
+    </a><br />
     <img alt="${doc_type}"
          src="${icon}"
          title="${filename}"
          tal:condition="icon"
     />
     <a href="${download_url}">${filename}</a>
     <span class="text-muted">
@@ -49,58 +52,67 @@
              name="${view/name}.action"
              onclick="document.getElementById('${view/id}-input').disabled=true;"
              type="radio"
              value="nochange"
       />
       <label class="form-check-label"
              for="${view/id}-nochange"
-             i18n:translate="file_keep"
-      >Keep existing file</label>
+             i18n:translate="image_keep"
+      >Keep existing image</label>
     </div>
     <div class="form-check"
          tal:condition="not:view/field/required"
     >
       <input class="form-check-input"
              id="${view/id}-remove"
              checked="${python:'checked' if action == 'remove' else None}"
              name="${view/name}.action"
              onclick="document.getElementById('${view/id}-input').disabled=true;"
              type="radio"
              value="remove"
       />
       <label class="form-check-label"
              for="${view/id}-remove"
-             i18n:translate="file_remove"
-      >Remove existing file</label>
+             i18n:translate="image_remove"
+      >Remove existing image</label>
     </div>
+
     <div class="form-check">
       <input class="form-check-input"
              id="${view/id}-replace"
              checked="${python:'checked' if action == 'replace' else None}"
              name="${view/name}.action"
              onclick="document.getElementById('${view/id}-input').disabled=false"
              type="radio"
              value="replace"
       />
       <label class="form-check-label"
              for="${view/id}-replace"
-             i18n:translate="file_replace"
-      >Replace with new file</label>
+             i18n:translate="image_replace"
+      >Replace with new image</label>
     </div>
   </tal:block>
 
   <input class="form-control ${python:view.error and 'is-invalid' or ''}"
          id="${view/id}-input"
+         accept="${view/accept|nothing}"
          disabled="${view/disabled}"
          maxlength="${view/maxlength}"
          name="${view/name}"
          required="${python:view.required and 'required' or None}"
          size="${view/size}"
          type="file"
   />
+  <div class="form-text"
+       tal:condition="view/accept|nothing"
+       i18n:translate="namedfile_accepted_types"
+  >
+      Allowed types:
+    <tal:i18n i18n:name="accepted_types">${view/accept}</tal:i18n>.
+  </div>
 
   <script type="text/javascript"
           tal:condition="python:allow_nochange and action != 'replace'"
           tal:content="string:document.getElementById('${view/id}-input').disabled=true;"
   >
   </script>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
-File already uploaded: ${filename} [${doc_type}]_$_{_f_i_l_e_n_a_m_e_} — ContentType, $
-{view/file_size}
-#Keep existing file
-#Remove existing file
-#Replace with new file
+Image already uploaded: ${filename} _[_I_m_a_g_e_]
+[${doc_type}]_$_{_f_i_l_e_n_a_m_e_} — ContentType, ${view/file_size}
+#Keep existing image
+#Remove existing image
+#Replace with new image
 [File]
+Allowed types: ${view/accept}.
```

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/form.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/image_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/file_input.pt`

 * *Files 10% similar despite different names*

```diff
@@ -18,22 +18,19 @@
           tal:condition="up_id"
   >
     <input name="${view/name}.file_upload_id"
            type="hidden"
            value="${up_id}"
     />
     <span>
-      <tal:i18n i18n:translate="image_already_uploaded">Image already uploaded:</tal:i18n>
+      <tal:i18n i18n:translate="file_already_uploaded">File already uploaded:</tal:i18n>
         ${filename}
     </span>
   </tal:if>
   <span tal:condition="python:exists and download_url and action=='nochange'">
-    <a href="${download_url}">
-      <img tal:replace="structure view/thumb_tag" />
-    </a><br />
     <img alt="${doc_type}"
          src="${icon}"
          title="${filename}"
          tal:condition="icon"
     />
     <a href="${download_url}">${filename}</a>
     <span class="text-muted">
@@ -52,59 +49,66 @@
              name="${view/name}.action"
              onclick="document.getElementById('${view/id}-input').disabled=true;"
              type="radio"
              value="nochange"
       />
       <label class="form-check-label"
              for="${view/id}-nochange"
-             i18n:translate="image_keep"
-      >Keep existing image</label>
+             i18n:translate="file_keep"
+      >Keep existing file</label>
     </div>
     <div class="form-check"
          tal:condition="not:view/field/required"
     >
       <input class="form-check-input"
              id="${view/id}-remove"
              checked="${python:'checked' if action == 'remove' else None}"
              name="${view/name}.action"
              onclick="document.getElementById('${view/id}-input').disabled=true;"
              type="radio"
              value="remove"
       />
       <label class="form-check-label"
              for="${view/id}-remove"
-             i18n:translate="image_remove"
-      >Remove existing image</label>
+             i18n:translate="file_remove"
+      >Remove existing file</label>
     </div>
-
     <div class="form-check">
       <input class="form-check-input"
              id="${view/id}-replace"
              checked="${python:'checked' if action == 'replace' else None}"
              name="${view/name}.action"
              onclick="document.getElementById('${view/id}-input').disabled=false"
              type="radio"
              value="replace"
       />
       <label class="form-check-label"
              for="${view/id}-replace"
-             i18n:translate="image_replace"
-      >Replace with new image</label>
+             i18n:translate="file_replace"
+      >Replace with new file</label>
     </div>
   </tal:block>
 
   <input class="form-control ${python:view.error and 'is-invalid' or ''}"
          id="${view/id}-input"
+         accept="${view/accept|nothing}"
          disabled="${view/disabled}"
          maxlength="${view/maxlength}"
          name="${view/name}"
          required="${python:view.required and 'required' or None}"
          size="${view/size}"
          type="file"
   />
+  <div class="form-text"
+       tal:condition="view/accept|nothing"
+       i18n:translate="namedfile_accepted_types"
+  >
+      Allowed types:
+    <tal:i18n i18n:name="accepted_types">${view/accept}</tal:i18n>.
+  </div>
 
   <script type="text/javascript"
           tal:condition="python:allow_nochange and action != 'replace'"
           tal:content="string:document.getElementById('${view/id}-input').disabled=true;"
   >
   </script>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
-Image already uploaded: ${filename} _[_I_m_a_g_e_]
-[${doc_type}]_$_{_f_i_l_e_n_a_m_e_} — ContentType, ${view/file_size}
-#Keep existing image
-#Remove existing image
-#Replace with new image
+File already uploaded: ${filename} [${doc_type}]_$_{_f_i_l_e_n_a_m_e_} — ContentType, $
+{view/file_size}
+#Keep existing file
+#Remove existing file
+#Replace with new file
 [File]
+Allowed types: ${view/accept}.
```

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/layout.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/link_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/macros.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/multi_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/object_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/orderedselect_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/radio_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/radio_input_single.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/relateditems_display.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/relateditems_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/select_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/singlecheckbox.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/singlecheckbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/singlecheckboxbool_input.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/templates/widget.pt` & `plone.app.z3cform-4.5.0/plone/app/z3cform/templates/widget.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/example.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/example.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/layer.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/layer.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_csrf.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_patterns.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_utils.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/test_widgets.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/test_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,25 +567,27 @@
 class SelectWidgetTests(unittest.TestCase):
     layer = PAZ3CForm_INTEGRATION_TESTING
 
     def setUp(self):
         self.request = self.layer["request"]
 
     def test_select_widget(self):
+        from plone.app.z3cform.widgets.select import SelectFieldWidget
         from plone.app.z3cform.widgets.select import SelectWidget
 
-        widget = SelectWidget(self.request)
-        widget.id = "test-widget"
-        widget.name = "selectfield-widget"
-        widget.field = Choice(
+        field = Choice(
             __name__="selectfield",
             values=["one", "two", "three"],
+            required=True,
         )
-        widget.terms = widget.field.vocabulary
-        widget.field.required = True
+        widget = SelectFieldWidget(field, self.request)
+        widget.id = "test-widget"
+        widget.name = "selectfield-widget"
+        widget.terms = field.vocabulary
+        self.assertTrue(isinstance(widget, SelectWidget))
         self.assertEqual(
             {
                 "pattern_options": {},
                 "pattern": None,
             },
             {
                 "pattern_options": widget.get_pattern_options(),
```

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/testing.zcml` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/tests/tests.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/utils.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/views.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/views.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widget.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/base.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/checkbox.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/datetime.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/datetime.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/email.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/email.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/link.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/link.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/orderedselect.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/orderedselect.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/password.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/password.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/patterns.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/patterns.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/querystring.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/querystring.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/radio.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/relateditems.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/relateditems.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/richtext.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/select.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,24 @@
 
 @implementer_only(ISelectWidget)
 class SelectWidget(HTMLSelectWidget, SelectWidgetBase):
     klass = "select-widget"
 
 
 @implementer(IFieldWidget)
-def SelectFieldWidget(field, source, request):
+def SelectFieldWidget(field, request, extra=None):
+    if extra is not None:
+        request = extra
     return FieldWidget(field, SelectWidget(request))
 
 
 @implementer(IFieldWidget)
 def CollectionChoiceSelectFieldWidget(field, value_type, request):
     """IFieldWidget factory for SelectWidget."""
-    return SelectFieldWidget(field, None, request)
+    return SelectFieldWidget(field, request)
 
 
 @implementer_only(ISelect2Widget)
 class Select2Widget(HTMLSelectWidget, SelectWidgetBase):
     """Select widget for z3c.form."""
 
     pattern = "select2"
```

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/singlecheckbox.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/singlecheckbox.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/submit.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/submit.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets/text.py` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets/text.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone/app/z3cform/widgets.zcml` & `plone.app.z3cform-4.5.0/plone/app/z3cform/widgets.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/PKG-INFO` & `plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.4.1
+Version: 4.5.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: plone.app.textfield>=1.3.6
 Requires-Dist: plone.base
 Requires-Dist: plone.app.contentlisting
+Requires-Dist: plone.formwidget.namedfile>=3.1.0
 Requires-Dist: plone.i18n
 Requires-Dist: plone.protect
 Requires-Dist: plone.registry
 Requires-Dist: plone.schema
 Requires-Dist: plone.uuid
 Requires-Dist: plone.z3cform
 Requires-Dist: Products.GenericSetup
@@ -689,14 +690,43 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.5.0 (2024-03-19)
+------------------
+
+New features:
+
+
+- Add support for the "accept" attribute on file inputs.
+
+  If the widget's field - if there is one - has the "accept" attribute set (the
+  `NamedImage` field has `image/*` set by default) then this is rendered as an
+  `accept` attribute on the file input.
+
+  This would restrict the allowed file types before uploading while still being
+  checked on the server side.
+
+  Fixes: https://github.com/plone/plone.formwidget.namedfile/issues/66
+  Depends on:
+  - https://github.com/plone/plone.namedfile/pull/158
+  - https://github.com/plone/plone.formwidget.namedfile/pull/67
+  [thet] (#198)
+
+
+Bug fixes:
+
+
+- Fix `SelectFieldWidget` factory call.
+  [petschki] (#192)
+
+
 4.4.1 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Add missing ``pattern_options`` multiadapter to new PatternFormElement base class.
```

### Comparing `plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/SOURCES.txt` & `plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.4.1/plone.app.z3cform.egg-info/requires.txt` & `plone.app.z3cform-4.5.0/plone.app.z3cform.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 plone.app.textfield>=1.3.6
 plone.base
 plone.app.contentlisting
+plone.formwidget.namedfile>=3.1.0
 plone.i18n
 plone.protect
 plone.registry
 plone.schema
 plone.uuid
 plone.z3cform
 Products.GenericSetup
```

### Comparing `plone.app.z3cform-4.4.1/pyproject.toml` & `plone.app.z3cform-4.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
+[build-system]
+requires = ["setuptools>=68.2"]
+
 [tool.towncrier]
 directory = "news/"
 filename = "CHANGES.rst"
 title_format = "{version} ({project_date})"
 underlines = ["-", ""]
 
 [[tool.towncrier.type]]
@@ -112,44 +115,50 @@
   'zope.sendmail', 'Zope'
 ]
 'plone.base' = [
   'plone.batching', 'plone.registry', 'plone.schema','plone.z3cform',
   'Products.CMFCore', 'Products.CMFDynamicViewFTI',
 ]
 python-dateutil = ['dateutil']
-ignore-packages = ['lxml', 'plone.app.vocabularies']
+ignore-packages = ['lxml', 'plone.app.vocabularies', 'plone.formwidget.namedfile']
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
 #    "pygithub = ['github']",
 #  ]
-#  """
 ##
 
 [tool.check-manifest]
 ignore = [
     ".editorconfig",
+    ".flake8",
     ".meta.toml",
     ".pre-commit-config.yaml",
-    "tox.ini",
-    ".flake8",
+    "dependabot.yml",
     "mx.ini",
+    "tox.ini",
 
 ]
+
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  check_manifest_ignores = """
 #      "*.map.js",
 #      "*.pyc",
 #  """
+#  check_manifest_extra_lines = """
+#  ignore-bad-ideas = [
+#      "some/test/file/PKG-INFO",
+#  ]
+#  """
 ##
 
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  extra_lines = """
```

### Comparing `plone.app.z3cform-4.4.1/setup.py` & `plone.app.z3cform-4.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.4.1"
+version = "4.5.0"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n"
     f"{(Path('plone') / 'app' / 'z3cform' / 'inline_validation.rst').read_text()}\n"
     f"{Path('CHANGES.rst').read_text()}"
 )
 
@@ -58,14 +58,15 @@
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "plone.app.textfield>=1.3.6",
         "plone.base",
         "plone.app.contentlisting",
+        "plone.formwidget.namedfile>=3.1.0",
         "plone.i18n",
         "plone.protect",
         "plone.registry",
         "plone.schema",
         "plone.uuid",
         "plone.z3cform",
         "Products.GenericSetup",
```

