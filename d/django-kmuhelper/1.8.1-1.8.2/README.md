# Comparing `tmp/django-kmuhelper-1.8.1.tar.gz` & `tmp/django_kmuhelper-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-kmuhelper-1.8.1.tar", last modified: Sun Dec 24 20:31:51 2023, max compression
+gzip compressed data, was "django_kmuhelper-1.8.2.tar", last modified: Tue Apr 16 15:09:50 2024, max compression
```

## Comparing `django-kmuhelper-1.8.1.tar` & `django_kmuhelper-1.8.2.tar`

### file list

```diff
@@ -1,277 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.643504 django-kmuhelper-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    32587 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2023-12-24 20:31:51.643504 django-kmuhelper-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/README-EN.md
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.643504 django-kmuhelper-1.8.1/django_kmuhelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2023-12-24 20:31:51.000000 django-kmuhelper-1.8.1/django_kmuhelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2023-12-24 20:31:51.000000 django-kmuhelper-1.8.1/django_kmuhelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 20:31:51.000000 django-kmuhelper-1.8.1/django_kmuhelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-24 20:31:51.000000 django-kmuhelper-1.8.1/django_kmuhelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-24 20:31:51.000000 django-kmuhelper-1.8.1/django_kmuhelper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.607504 django-kmuhelper-1.8.1/kmuhelper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.607504 django-kmuhelper-1.8.1/kmuhelper/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.607504 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.607504 django-kmuhelper-1.8.1/kmuhelper/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/__qr_invoice_texts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.595504 django-kmuhelper-1.8.1/kmuhelper/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.611504 django-kmuhelper-1.8.1/kmuhelper/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.595504 django-kmuhelper-1.8.1/kmuhelper/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.611504 django-kmuhelper-1.8.1/kmuhelper/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.595504 django-kmuhelper-1.8.1/kmuhelper/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.611504 django-kmuhelper-1.8.1/kmuhelper/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.595504 django-kmuhelper-1.8.1/kmuhelper/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.611504 django-kmuhelper-1.8.1/kmuhelper/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.595504 django-kmuhelper-1.8.1/kmuhelper/management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.611504 django-kmuhelper-1.8.1/kmuhelper/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/management/commands/kmuhelper-import-customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/management/commands/model2csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.611504 django-kmuhelper-1.8.1/kmuhelper/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    81096 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0101_squashed_0100_to_0100.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0102_paymentreceiver_improvements.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0103_paymentreceiver_invoice_display_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0104_order_payment_purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0105_alter_setting_options_alter_settinghidden_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0106_alter_app_arrival_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0107_alter_emailtemplate_mail_subject_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0108_migrate_vat_rates_for_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/0109_contactperson_is_default_paymentreceiver_is_default.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.615504 django-kmuhelper-1.8.1/kmuhelper/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.615504 django-kmuhelper-1.8.1/kmuhelper/modules/api/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.615504 django-kmuhelper-1.8.1/kmuhelper/modules/app/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/app/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/app/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.615504 django-kmuhelper-1.8.1/kmuhelper/modules/emails/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/emails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/emails/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13951 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/emails/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/emails/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/emails/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/emails/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.615504 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.619504 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.619504 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28552 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.619504 django-kmuhelper-1.8.1/kmuhelper/modules/main/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38254 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/main/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/main/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    59060 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/main/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/main/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/main/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.619504 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.623504 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18828 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/swiss_qr_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.623504 django-kmuhelper-1.8.1/kmuhelper/modules/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/settings/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.623504 django-kmuhelper-1.8.1/kmuhelper/modules/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/stats/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/modules/stats/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.599504 django-kmuhelper-1.8.1/kmuhelper/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.599504 django-kmuhelper-1.8.1/kmuhelper/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.599504 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.623504 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/colors-kmuhelper.css
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/index-kmuhelper.css
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/pagechooser.css
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.623504 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/js/beforeunload.js
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/js/changelist_saveontop.js
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/js/collapse-open.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.623504 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.627504 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/css/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/css/details.css
--rw-r--r--   0 runner    (1001) docker     (127)   101750 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.599504 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.627504 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-384x384.png
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.627504 django-kmuhelper-1.8.1/kmuhelper/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.627504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.627504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/_confirm.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/_special/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/_special/app-index.html
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/_special/email-index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_arrival/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_arrival/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_arrival/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_shipping/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_shipping/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_shipping/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_stock/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_stock/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_stock/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_todo/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_todo/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/attachment/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/attachment/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/base_site.html
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/customer/
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/customer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/customer/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/delete_selected_confirmation.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/email/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/email/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/emailtemplate/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/note/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/note/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/object_history.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.631504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/order/
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/order/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/order/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/order/pdf_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/order/submit_line.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_entry.html
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order.html
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order_payment.html
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_payment.html
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/process.html
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/product/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/product/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/product/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/productcategory/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/productcategory/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/productcategory/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/setting/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/setting/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/supplier/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/supplier/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/supplier/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/supply/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/supply/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/supply/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.635504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/form.html
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/form_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/form_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/pagechooser.html
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/pwa_head.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/customer_registered.html
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/default.html
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/order_invoice.html
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/order_stock_warning.html
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/order_supply.html
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/error.html
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/home.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.603504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/integrations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/integrations/woocommerce/
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/integrations/woocommerce/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/settings/build_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/settings/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/best_products.html
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/products_price.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/kmuhelper/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templatetags/kmuhelper_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/templatetags/utiltags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/kmuhelper/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-12-24 20:31:51.643504 django-kmuhelper-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:51.639504 django-kmuhelper-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-12-24 20:31:41.000000 django-kmuhelper-1.8.1/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    32587 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/README-EN.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/django_kmuhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-16 15:09:50.000000 django_kmuhelper-1.8.2/django_kmuhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-04-16 15:09:50.000000 django_kmuhelper-1.8.2/django_kmuhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:09:50.000000 django_kmuhelper-1.8.2/django_kmuhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 15:09:50.000000 django_kmuhelper-1.8.2/django_kmuhelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 15:09:50.000000 django_kmuhelper-1.8.2/django_kmuhelper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.258959 django_kmuhelper-1.8.2/kmuhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.258959 django_kmuhelper-1.8.2/kmuhelper/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.258959 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.258959 django_kmuhelper-1.8.2/kmuhelper/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/__qr_invoice_texts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.246959 django_kmuhelper-1.8.2/kmuhelper/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.258959 django_kmuhelper-1.8.2/kmuhelper/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    64999 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.246959 django_kmuhelper-1.8.2/kmuhelper/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.262959 django_kmuhelper-1.8.2/kmuhelper/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.246959 django_kmuhelper-1.8.2/kmuhelper/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.262959 django_kmuhelper-1.8.2/kmuhelper/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.246959 django_kmuhelper-1.8.2/kmuhelper/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.262959 django_kmuhelper-1.8.2/kmuhelper/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.246959 django_kmuhelper-1.8.2/kmuhelper/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.262959 django_kmuhelper-1.8.2/kmuhelper/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/management/commands/kmuhelper-import-customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/management/commands/model2csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.266959 django_kmuhelper-1.8.2/kmuhelper/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    81096 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0101_squashed_0100_to_0100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0102_paymentreceiver_improvements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0103_paymentreceiver_invoice_display_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0104_order_payment_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0105_alter_setting_options_alter_settinghidden_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0106_alter_app_arrival_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0107_alter_emailtemplate_mail_subject_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0108_migrate_vat_rates_for_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0109_contactperson_is_default_paymentreceiver_is_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0110_orderitem_made_product_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0111_alter_order_tracking_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0112_product_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/0113_customer_woocommerce_deleted_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.266959 django_kmuhelper-1.8.2/kmuhelper/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.266959 django_kmuhelper-1.8.2/kmuhelper/modules/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.266959 django_kmuhelper-1.8.2/kmuhelper/modules/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/app/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.266959 django_kmuhelper-1.8.2/kmuhelper/modules/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/emails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/emails/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/emails/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/emails/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/emails/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/emails/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.266959 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.270959 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.270959 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.270959 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/product_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/api/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.274959 django_kmuhelper-1.8.2/kmuhelper/modules/main/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41495 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61832 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/main/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.274959 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.274959 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18838 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/swiss_qr_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.274959 django_kmuhelper-1.8.2/kmuhelper/modules/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/settings/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/modules/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/stats/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/modules/stats/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.250959 django_kmuhelper-1.8.2/kmuhelper/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.250959 django_kmuhelper-1.8.2/kmuhelper/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.250959 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/colors-kmuhelper.css
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/index-kmuhelper.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/pagechooser.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/js/beforeunload.js
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/js/changelist_saveontop.js
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/js/collapse-open.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/css/details.css
+-rw-r--r--   0 runner    (1001) docker     (127)   101750 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.250959 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-384x384.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.278959 django_kmuhelper-1.8.2/kmuhelper/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/_confirm.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/_special/app-index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/_special/email-index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_arrival/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_arrival/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_arrival/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_shipping/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_shipping/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_shipping/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_stock/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_stock/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_stock/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_todo/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_todo/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.282959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/attachment/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/attachment/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/customer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/customer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/customer/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/delete_selected_confirmation.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/email/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/emailtemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/note/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/note/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/object_history.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/order/
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/order/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/order/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/order/pdf_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/order/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_entry.html
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order_payment.html
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_payment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/process.html
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.286959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/product/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/product/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/product/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/productcategory/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/productcategory/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/productcategory/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/setting/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/setting/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/supplier/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/supplier/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/supplier/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/supply/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/supply/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/supply/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/form_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/form_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/pagechooser.html
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/pwa_head.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.290959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/customer_registered.html
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/order_invoice.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/order_stock_warning.html
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/order_supply.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/home.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.254959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/integrations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/integrations/woocommerce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/integrations/woocommerce/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/settings/build_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/settings/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/best_products.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/products_price.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/kmuhelper/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templatetags/kmuhelper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/templatetags/utiltags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/kmuhelper/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:50.294959 django_kmuhelper-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-16 15:09:38.000000 django_kmuhelper-1.8.2/tests/test_settings.py
```

### Comparing `django-kmuhelper-1.8.1/LICENSE` & `django_kmuhelper-1.8.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -617,15 +617,15 @@
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
 
  END OF TERMS AND CONDITIONS
 
 KMUHelper - Ein Tool für Schweizer KMU
-Copyright (C) 2020-2021 Rafael Urben
+Copyright (C) 2020-2024 Rafael Urben
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License,
 or any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `django-kmuhelper-1.8.1/PKG-INFO` & `django_kmuhelper-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-kmuhelper
-Version: 1.8.1
+Version: 1.8.2
 Summary: Ein Helfer für schweizer KMU
 Home-page: https://rafaelurben.github.io/django-kmuhelper
 Author: Rafael Urben
 Author-email: github@rafaelurben.ch
 Maintainer: Rafael Urben
 Maintainer-email: github@rafaelurben.ch
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `django-kmuhelper-1.8.1/README-EN.md` & `django_kmuhelper-1.8.2/README-EN.md`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/README.md` & `django_kmuhelper-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/django_kmuhelper.egg-info/PKG-INFO` & `django_kmuhelper-1.8.2/django_kmuhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-kmuhelper
-Version: 1.8.1
+Version: 1.8.2
 Summary: Ein Helfer für schweizer KMU
 Home-page: https://rafaelurben.github.io/django-kmuhelper
 Author: Rafael Urben
 Author-email: github@rafaelurben.ch
 Maintainer: Rafael Urben
 Maintainer-email: github@rafaelurben.ch
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `django-kmuhelper-1.8.1/django_kmuhelper.egg-info/SOURCES.txt` & `django_kmuhelper-1.8.2/django_kmuhelper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 kmuhelper/migrations/0103_paymentreceiver_invoice_display_mode.py
 kmuhelper/migrations/0104_order_payment_purpose.py
 kmuhelper/migrations/0105_alter_setting_options_alter_settinghidden_options.py
 kmuhelper/migrations/0106_alter_app_arrival_options_and_more.py
 kmuhelper/migrations/0107_alter_emailtemplate_mail_subject_and_more.py
 kmuhelper/migrations/0108_migrate_vat_rates_for_2024.py
 kmuhelper/migrations/0109_contactperson_is_default_paymentreceiver_is_default.py
+kmuhelper/migrations/0110_orderitem_made_product_optional.py
+kmuhelper/migrations/0111_alter_order_tracking_number.py
+kmuhelper/migrations/0112_product_parent.py
+kmuhelper/migrations/0113_customer_woocommerce_deleted_and_more.py
 kmuhelper/migrations/__init__.py
 kmuhelper/modules/__init__.py
 kmuhelper/modules/config.py
 kmuhelper/modules/api/__init__.py
 kmuhelper/modules/api/admin.py
 kmuhelper/modules/api/constants.py
 kmuhelper/modules/api/decorators.py
@@ -76,21 +80,31 @@
 kmuhelper/modules/integrations/__init__.py
 kmuhelper/modules/integrations/paymentimport/__init__.py
 kmuhelper/modules/integrations/paymentimport/admin.py
 kmuhelper/modules/integrations/paymentimport/forms.py
 kmuhelper/modules/integrations/paymentimport/models.py
 kmuhelper/modules/integrations/paymentimport/views.py
 kmuhelper/modules/integrations/woocommerce/__init__.py
-kmuhelper/modules/integrations/woocommerce/api.py
+kmuhelper/modules/integrations/woocommerce/filters.py
 kmuhelper/modules/integrations/woocommerce/forms.py
+kmuhelper/modules/integrations/woocommerce/mixins.py
 kmuhelper/modules/integrations/woocommerce/urls.py
 kmuhelper/modules/integrations/woocommerce/utils.py
 kmuhelper/modules/integrations/woocommerce/views.py
+kmuhelper/modules/integrations/woocommerce/api/__init__.py
+kmuhelper/modules/integrations/woocommerce/api/_base.py
+kmuhelper/modules/integrations/woocommerce/api/_utils.py
+kmuhelper/modules/integrations/woocommerce/api/customers.py
+kmuhelper/modules/integrations/woocommerce/api/general.py
+kmuhelper/modules/integrations/woocommerce/api/orders.py
+kmuhelper/modules/integrations/woocommerce/api/product_categories.py
+kmuhelper/modules/integrations/woocommerce/api/products.py
 kmuhelper/modules/main/__init__.py
 kmuhelper/modules/main/admin.py
+kmuhelper/modules/main/filters.py
 kmuhelper/modules/main/mixins.py
 kmuhelper/modules/main/models.py
 kmuhelper/modules/main/urls.py
 kmuhelper/modules/main/views.py
 kmuhelper/modules/pdfgeneration/__init__.py
 kmuhelper/modules/pdfgeneration/base.py
 kmuhelper/modules/pdfgeneration/swiss_qr_invoice.py
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/admin.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/decorators.py` & `django_kmuhelper-1.8.2/kmuhelper/decorators.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/LICENSE` & `django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/LICENSE`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/README.md` & `django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/README.md`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/fields.py` & `django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/fields.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/forms.py` & `django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/external/multi_email_field/widgets.py` & `django_kmuhelper-1.8.2/kmuhelper/external/multi_email_field/widgets.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/__qr_invoice_texts.json` & `django_kmuhelper-1.8.2/kmuhelper/locale/__qr_invoice_texts.json`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/de/LC_MESSAGES/django.mo` & `django_kmuhelper-1.8.2/kmuhelper/locale/en/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,196 +1,195 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: de\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Enter valid email addresses."
-msgstr "Geben Sie bitte gültige E-Mail-Adressen ein."
+msgstr "Enter valid email addresses."
 
 msgid ""
 "Geschätzter Kunde\n"
 "\n"
 "Vermutlich ist Ihnen entgangen, diese Rechnung vom %(original_date)s innert "
 "der gewährten Frist zu begleichen.\n"
 "Wir bitten Sie, dies innert %(days)d Tagen nachzuholen.\n"
 "\n"
 "Sollte sich Ihre Zahlung mit diesem Schreiben überkreuzen, so betrachten Sie "
 "dieses bitte als gegenstandslos."
 msgstr ""
-"Geschätzter Kunde\n"
+"Dear customer\n"
 "\n"
-"Vermutlich ist Ihnen entgangen, diese Rechnung vom %(original_date)s innert "
-"der gewährten Frist zu begleichen.\n"
-"Wir bitten Sie, dies innert %(days)d Tagen nachzuholen.\n"
+"You have probably forgotten to pay this invoice from %(original_date)s "
+"within the given time limit.\n"
+"We kindly ask you to do so within %(days)d days.\n"
 "\n"
-"Sollte sich Ihre Zahlung mit diesem Schreiben überkreuzen, so betrachten Sie "
-"dieses bitte als gegenstandslos."
+"Should your payment cross with this letter, please consider it as irrelevant."
 
 msgid "Lieferschein"
-msgstr "Lieferschein"
+msgstr "Delivery note"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Annahmestelle"
-msgstr "Annahmestelle"
+msgstr "Acceptance point"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Betrag"
-msgstr "Betrag"
+msgstr "Amount"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Empfangsschein"
-msgstr "Empfangsschein"
+msgstr "Receipt"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Konto / Zahlbar an"
-msgstr "Konto / Zahlbar an"
+msgstr "Account / Payable to"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Referenz"
-msgstr "Referenz"
+msgstr "Reference"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Vor der Einzahlung abzutrennen"
-msgstr "Vor der Einzahlung abzutrennen"
+msgstr "Separate before paying in"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Währung"
-msgstr "Währung"
+msgstr "Currency"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlbar durch"
-msgstr "Zahlbar durch"
+msgstr "Payable by"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlteil"
-msgstr "Zahlteil"
+msgstr "Payment part"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zusätzliche Informationen"
-msgstr "Zusätzliche Informationen"
+msgstr "Additional information"
 
 msgid "Rechnung"
-msgstr "Rechnung"
+msgstr "Invoice"
 
 msgid "Referenznummer"
-msgstr "Referenznummer"
+msgstr "Reference number"
 
 msgctxt "Text on generated order PDF"
 msgid "%(days)s Tage %(percent)s%% Skonto"
-msgstr "%(days)s Tage %(percent)s%% Skonto"
+msgstr "%(days)s days %(percent)s%% discount"
 
 msgctxt "Text on generated order PDF"
 msgid "Anzahl"
-msgstr "Anzahl"
+msgstr "Quantity"
 
 msgctxt "Text on generated order PDF"
 msgid "Anzahl Produkte"
-msgstr "Anzahl Produkte"
+msgstr "Number of products"
 
 msgctxt "Text on generated order PDF"
 msgid "Art-Nr."
-msgstr "Art-Nr."
+msgstr "Item No."
 
 msgctxt "Text on generated order PDF"
 msgid "Bestelldatum"
-msgstr "Bestelldatum"
+msgstr "Order date"
 
 msgctxt "Text on generated order PDF"
 msgid "Bestellnummer"
-msgstr "Bestellnummer"
+msgstr "Order number"
 
 msgctxt "Text on generated order PDF"
 msgid "Bezeichnung"
-msgstr "Bezeichnung"
+msgstr "Name"
 
 msgctxt "Text on generated order PDF"
 msgid "Datum"
-msgstr "Datum"
+msgstr "Date"
 
 msgctxt "Text on generated order PDF"
 msgid "E-Mail"
 msgstr "E-Mail"
 
 msgctxt "Text on generated order PDF"
 msgid "Einheit"
-msgstr "Einheit"
+msgstr "Unit"
 
 msgctxt "Text on generated order PDF"
 msgid "Ihre Kundennummer"
-msgstr "Ihre Kundennummer"
+msgstr "Your customer number"
 
 msgctxt "Text on generated order PDF"
 msgid "MwSt"
-msgstr "MwSt"
+msgstr "VAT"
 
 msgctxt "Text on generated order PDF"
 msgid "Preis"
-msgstr "Preis"
+msgstr "Price"
 
 msgctxt "Text on generated order PDF"
 msgid "Rabatt"
-msgstr "Rabatt"
+msgstr "Discount"
 
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag"
-msgstr "Rechnungsbetrag"
+msgstr "Invoice amount"
 
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag, zahlbar netto innert %s Tagen"
-msgstr "Rechnungsbetrag, zahlbar netto innert %s Tagen"
+msgstr "Net amount, payable within %s days"
 
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsdatum"
-msgstr "Rechnungsdatum"
+msgstr "Invoice date"
 
 msgctxt "Text on generated order PDF"
 msgid "Tel."
-msgstr "Tel"
+msgstr "Tel."
 
 msgctxt "Text on generated order PDF"
 msgid "Total"
 msgstr "Total"
 
 msgctxt "Text on generated order PDF"
 msgid "Web"
 msgstr "Web"
 
 msgid "Zahlungserinnerung"
-msgstr "Zahlungserinnerung"
+msgstr "Payment reminder"
 
 msgctxt "quantity description"
 msgid "Einheit"
 msgid_plural "Einheiten"
-msgstr[0] "Einheit"
-msgstr[1] "Einheiten"
+msgstr[0] "Unit"
+msgstr[1] "Units"
 
 msgctxt "quantity description"
 msgid "Flasche"
 msgid_plural "Flaschen"
-msgstr[0] "Flsche"
-msgstr[1] "Flaschen"
+msgstr[0] "Bottle"
+msgstr[1] "Bottles"
 
 msgctxt "quantity description"
 msgid "Stunde"
 msgid_plural "Stunden"
-msgstr[0] "Stunde"
-msgstr[1] "Stunden"
+msgstr[0] "Hour"
+msgstr[1] "Hours"
 
 msgctxt "quantity description"
 msgid "Stück"
 msgid_plural "Stück"
-msgstr[0] "Stück"
-msgstr[1] "Stück"
+msgstr[0] "Piece"
+msgstr[1] "Pieces"
 
 msgctxt "quantity description"
 msgid "Tube"
 msgid_plural "Tuben"
 msgstr[0] "Tube"
-msgstr[1] "Tuben"
+msgstr[1] "Tubes"
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/de/LC_MESSAGES/django.po` & `django_kmuhelper-1.8.2/kmuhelper/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -8,257 +8,257 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-05 14:13+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: de\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: .\kmuhelper\external\multi_email_field\forms.py:10
 msgid "Enter valid email addresses."
-msgstr "Geben Sie bitte gültige E-Mail-Adressen ein."
+msgstr "Entrez des adresses électroniques valides."
 
 #: .\kmuhelper\modules\main\models.py:654
 msgid "Referenznummer"
-msgstr "Referenznummer"
+msgstr "Numéro de référence"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:32
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:204
 msgctxt "Text on generated order PDF"
 msgid "Art-Nr."
 msgstr "Art-Nr."
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:33
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:205
 msgctxt "Text on generated order PDF"
 msgid "Bezeichnung"
-msgstr "Bezeichnung"
+msgstr "Appellation"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:34
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:206
 msgctxt "Text on generated order PDF"
 msgid "Anzahl"
-msgstr "Anzahl"
+msgstr "Quantité"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:35
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:207
 msgctxt "Text on generated order PDF"
 msgid "Einheit"
-msgstr "Einheit"
+msgstr "Unité"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:36
 msgctxt "Text on generated order PDF"
 msgid "Preis"
-msgstr "Preis"
+msgstr "Prix"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:37
 msgctxt "Text on generated order PDF"
 msgid "Total"
 msgstr "Total"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:58
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:93
 msgctxt "Text on generated order PDF"
 msgid "Rabatt"
-msgstr "Rabatt"
+msgstr "Réduction"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:119
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:572
 msgctxt "Text on generated order PDF"
 msgid "MwSt"
-msgstr "MwSt"
+msgstr "TVA"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:136
 #, python-format
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag, zahlbar netto innert %s Tagen"
-msgstr "Rechnungsbetrag, zahlbar netto innert %s Tagen"
+msgstr "Montant net, payable à %s jours"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:138
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag"
-msgstr "Rechnungsbetrag"
+msgstr "Montant de la facture"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:154
 #, python-format
 msgctxt "Text on generated order PDF"
 msgid "%(days)s Tage %(percent)s%% Skonto"
-msgstr "%(days)s Tage %(percent)s%% Skonto"
+msgstr "%(days)s jours %(percent)s%% de remise"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:234
 msgctxt "Text on generated order PDF"
 msgid "Anzahl Produkte"
-msgstr "Anzahl Produkte"
+msgstr "Nombre de produits"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:433
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Vor der Einzahlung abzutrennen"
-msgstr "Vor der Einzahlung abzutrennen"
+msgstr "A détacher avant le versement"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:445
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:463
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Konto / Zahlbar an"
-msgstr "Konto / Zahlbar an"
+msgstr "Compte / Payable à"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:452
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:470
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Referenz"
-msgstr "Referenz"
+msgstr "Référence"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:455
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:478
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlbar durch"
-msgstr "Zahlbar durch"
+msgstr "Payable par"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:473
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zusätzliche Informationen"
-msgstr "Zusätzliche Informationen"
+msgstr "Informations additionnelles"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:486
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Empfangsschein"
-msgstr "Empfangsschein"
+msgstr "Récépissé"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:487
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlteil"
-msgstr "Zahlteil"
+msgstr "Section paiement"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:490
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:499
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Währung"
-msgstr "Währung"
+msgstr "Monnaie"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:491
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:500
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Betrag"
-msgstr "Betrag"
+msgstr "Montant"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:492
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Annahmestelle"
-msgstr "Annahmestelle"
+msgstr "Point de dépôt"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:567
 msgctxt "Text on generated order PDF"
 msgid "Tel."
-msgstr "Tel"
+msgstr "Tel."
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:568
 msgctxt "Text on generated order PDF"
 msgid "E-Mail"
 msgstr "E-Mail"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:570
 msgctxt "Text on generated order PDF"
 msgid "Web"
 msgstr "Web"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:589
 msgctxt "Text on generated order PDF"
 msgid "Ihre Kundennummer"
-msgstr "Ihre Kundennummer"
+msgstr "Votre numéro de client"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:590
 msgctxt "Text on generated order PDF"
 msgid "Bestellnummer"
-msgstr "Bestellnummer"
+msgstr "Numéro de commande"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:591
 msgctxt "Text on generated order PDF"
 msgid "Bestelldatum"
-msgstr "Bestelldatum"
+msgstr "Date de commande"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:593
 msgctxt "Text on generated order PDF"
 msgid "Datum"
-msgstr "Datum"
+msgstr "Date"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:595
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsdatum"
-msgstr "Rechnungsdatum"
+msgstr "Date de facture"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:48
 msgid "Rechnung"
-msgstr "Rechnung"
+msgstr "Facture"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:52
 msgid "Lieferschein"
-msgstr "Lieferschein"
+msgstr "Bon de livraison"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:57
 msgid "Zahlungserinnerung"
-msgstr "Zahlungserinnerung"
+msgstr "Rappel de paiement"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:58
 #, python-format
 msgid ""
 "Geschätzter Kunde\n"
 "\n"
 "Vermutlich ist Ihnen entgangen, diese Rechnung vom %(original_date)s innert "
 "der gewährten Frist zu begleichen.\n"
 "Wir bitten Sie, dies innert %(days)d Tagen nachzuholen.\n"
 "\n"
 "Sollte sich Ihre Zahlung mit diesem Schreiben überkreuzen, so betrachten Sie "
 "dieses bitte als gegenstandslos."
 msgstr ""
-"Geschätzter Kunde\n"
+"Cher client\n"
 "\n"
-"Vermutlich ist Ihnen entgangen, diese Rechnung vom %(original_date)s innert "
-"der gewährten Frist zu begleichen.\n"
-"Wir bitten Sie, dies innert %(days)d Tagen nachzuholen.\n"
+"Vous n'avez probablement pas réglé cette facture du %(original_date)s dans "
+"le délai imparti.\n"
+"Nous vous prions de bien vouloir le faire dans les %(days)d jours.\n"
 "\n"
-"Sollte sich Ihre Zahlung mit diesem Schreiben überkreuzen, so betrachten Sie "
-"dieses bitte als gegenstandslos."
+"Si votre paiement devait se recouper avec cette lettre, veuillez considérer "
+"que celle-ci est sans objet."
 
 #: .\kmuhelper\translations.py:23
 msgctxt "quantity description"
 msgid "Stück"
 msgid_plural "Stück"
-msgstr[0] "Stück"
-msgstr[1] "Stück"
+msgstr[0] "Pièce"
+msgstr[1] "Pièces"
 
 #: .\kmuhelper\translations.py:31
 msgctxt "quantity description"
 msgid "Stunde"
 msgid_plural "Stunden"
-msgstr[0] "Stunde"
-msgstr[1] "Stunden"
+msgstr[0] "Heure"
+msgstr[1] "Heures"
 
 #: .\kmuhelper\translations.py:39
 msgctxt "quantity description"
 msgid "Einheit"
 msgid_plural "Einheiten"
-msgstr[0] "Einheit"
-msgstr[1] "Einheiten"
+msgstr[0] "Unité"
+msgstr[1] "Unités"
 
 #: .\kmuhelper\translations.py:47
 msgctxt "quantity description"
 msgid "Flasche"
 msgid_plural "Flaschen"
-msgstr[0] "Flsche"
-msgstr[1] "Flaschen"
+msgstr[0] "Bouteille"
+msgstr[1] "Bouteilles"
 
 #: .\kmuhelper\translations.py:55
 msgctxt "quantity description"
 msgid "Tube"
 msgid_plural "Tuben"
 msgstr[0] "Tube"
-msgstr[1] "Tuben"
+msgstr[1] "Tubes"
 
 #~ msgid "Ihr/e Ansprechpartner/in"
-#~ msgstr "Ihr/e Ansprechpartner/in"
+#~ msgstr "Votre interlocuteur"
 
 #~ msgid "Ihre Bestellung vom"
-#~ msgstr "Ihre Bestellung vom"
+#~ msgstr "Votre commande du"
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/en/LC_MESSAGES/django.mo` & `django_kmuhelper-1.8.2/kmuhelper/locale/it/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,188 +8,189 @@
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Enter valid email addresses."
-msgstr "Enter valid email addresses."
+msgstr "Inserire indirizzi e-mail validi."
 
 msgid ""
 "Geschätzter Kunde\n"
 "\n"
 "Vermutlich ist Ihnen entgangen, diese Rechnung vom %(original_date)s innert "
 "der gewährten Frist zu begleichen.\n"
 "Wir bitten Sie, dies innert %(days)d Tagen nachzuholen.\n"
 "\n"
 "Sollte sich Ihre Zahlung mit diesem Schreiben überkreuzen, so betrachten Sie "
 "dieses bitte als gegenstandslos."
 msgstr ""
-"Dear customer\n"
+"Gentile Cliente\n"
 "\n"
-"You have probably forgotten to pay this invoice from %(original_date)s "
-"within the given time limit.\n"
-"We kindly ask you to do so within %(days)d days.\n"
+"Riteniamo che non abbiate pagato questa fattura dell' %(original_date)s "
+"entro i termini previsti.\n"
+"Vi chiediamo gentilmente di farlo entro %(days)d giorni.\n"
 "\n"
-"Should your payment cross with this letter, please consider it as irrelevant."
+"Se il vostro pagamento dovesse incrociarsi con questa lettera, consideratela "
+"irrilevante."
 
 msgid "Lieferschein"
-msgstr "Delivery note"
+msgstr "Nota di consegna"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Annahmestelle"
-msgstr "Acceptance point"
+msgstr "Punto di accettazione"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Betrag"
-msgstr "Amount"
+msgstr "Importo"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Empfangsschein"
-msgstr "Receipt"
+msgstr "Ricevuta"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Konto / Zahlbar an"
-msgstr "Account / Payable to"
+msgstr "Conto / Pagabile a"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Referenz"
-msgstr "Reference"
+msgstr "Riferimento"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Vor der Einzahlung abzutrennen"
-msgstr "Separate before paying in"
+msgstr "Da staccare prima del versamento"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Währung"
-msgstr "Currency"
+msgstr "Valuta"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlbar durch"
-msgstr "Payable by"
+msgstr "Pagabile da"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlteil"
-msgstr "Payment part"
+msgstr "Sezione pagamento"
 
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zusätzliche Informationen"
-msgstr "Additional information"
+msgstr "Informazioni aggiuntive"
 
 msgid "Rechnung"
-msgstr "Invoice"
+msgstr "Fattura"
 
 msgid "Referenznummer"
-msgstr "Reference number"
+msgstr "Numero di riferimento"
 
 msgctxt "Text on generated order PDF"
 msgid "%(days)s Tage %(percent)s%% Skonto"
-msgstr "%(days)s days %(percent)s%% discount"
+msgstr "%(days)s giorni %(percent)s%% di sconto"
 
 msgctxt "Text on generated order PDF"
 msgid "Anzahl"
-msgstr "Quantity"
+msgstr "Quantità"
 
 msgctxt "Text on generated order PDF"
 msgid "Anzahl Produkte"
-msgstr "Number of products"
+msgstr "Numero di prodotti"
 
 msgctxt "Text on generated order PDF"
 msgid "Art-Nr."
-msgstr "Item No."
+msgstr "Articolo n."
 
 msgctxt "Text on generated order PDF"
 msgid "Bestelldatum"
-msgstr "Order date"
+msgstr "Data dell'ordine"
 
 msgctxt "Text on generated order PDF"
 msgid "Bestellnummer"
-msgstr "Order number"
+msgstr "Numero d'ordine"
 
 msgctxt "Text on generated order PDF"
 msgid "Bezeichnung"
-msgstr "Name"
+msgstr "Denominazione"
 
 msgctxt "Text on generated order PDF"
 msgid "Datum"
-msgstr "Date"
+msgstr "Data"
 
 msgctxt "Text on generated order PDF"
 msgid "E-Mail"
 msgstr "E-Mail"
 
 msgctxt "Text on generated order PDF"
 msgid "Einheit"
-msgstr "Unit"
+msgstr "Unità"
 
 msgctxt "Text on generated order PDF"
 msgid "Ihre Kundennummer"
-msgstr "Your customer number"
+msgstr "Il Suo codice cliente"
 
 msgctxt "Text on generated order PDF"
 msgid "MwSt"
-msgstr "VAT"
+msgstr "IVA"
 
 msgctxt "Text on generated order PDF"
 msgid "Preis"
-msgstr "Price"
+msgstr "Prezzo"
 
 msgctxt "Text on generated order PDF"
 msgid "Rabatt"
-msgstr "Discount"
+msgstr "Sconto"
 
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag"
-msgstr "Invoice amount"
+msgstr "Importo della fattura"
 
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag, zahlbar netto innert %s Tagen"
-msgstr "Net amount, payable within %s days"
+msgstr "Importo netto, pagabile entro %s giorni"
 
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsdatum"
-msgstr "Invoice date"
+msgstr "Data della fattura"
 
 msgctxt "Text on generated order PDF"
 msgid "Tel."
 msgstr "Tel."
 
 msgctxt "Text on generated order PDF"
 msgid "Total"
-msgstr "Total"
+msgstr "Totale"
 
 msgctxt "Text on generated order PDF"
 msgid "Web"
 msgstr "Web"
 
 msgid "Zahlungserinnerung"
-msgstr "Payment reminder"
+msgstr "Promemoria di pagamento"
 
 msgctxt "quantity description"
 msgid "Einheit"
 msgid_plural "Einheiten"
-msgstr[0] "Unit"
-msgstr[1] "Units"
+msgstr[0] "Unità"
+msgstr[1] "Unità"
 
 msgctxt "quantity description"
 msgid "Flasche"
 msgid_plural "Flaschen"
-msgstr[0] "Bottle"
-msgstr[1] "Bottles"
+msgstr[0] "Bottiglia"
+msgstr[1] "Bottiglie"
 
 msgctxt "quantity description"
 msgid "Stunde"
 msgid_plural "Stunden"
-msgstr[0] "Hour"
-msgstr[1] "Hours"
+msgstr[0] "Ora"
+msgstr[1] "Ore"
 
 msgctxt "quantity description"
 msgid "Stück"
 msgid_plural "Stück"
-msgstr[0] "Piece"
-msgstr[1] "Pieces"
+msgstr[0] "Pezzo"
+msgstr[1] "Pezzi"
 
 msgctxt "quantity description"
 msgid "Tube"
 msgid_plural "Tuben"
-msgstr[0] "Tube"
-msgstr[1] "Tubes"
+msgstr[0] "Tubo"
+msgstr[1] "Tubi"
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/en/LC_MESSAGES/django.po` & `django_kmuhelper-1.8.2/kmuhelper/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/fr/LC_MESSAGES/django.mo` & `django_kmuhelper-1.8.2/kmuhelper/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/locale/fr/LC_MESSAGES/django.po` & `django_kmuhelper-1.8.2/kmuhelper/locale/it/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,146 +12,146 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: .\kmuhelper\external\multi_email_field\forms.py:10
 msgid "Enter valid email addresses."
-msgstr "Entrez des adresses électroniques valides."
+msgstr "Inserire indirizzi e-mail validi."
 
 #: .\kmuhelper\modules\main\models.py:654
 msgid "Referenznummer"
-msgstr "Numéro de référence"
+msgstr "Numero di riferimento"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:32
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:204
 msgctxt "Text on generated order PDF"
 msgid "Art-Nr."
-msgstr "Art-Nr."
+msgstr "Articolo n."
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:33
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:205
 msgctxt "Text on generated order PDF"
 msgid "Bezeichnung"
-msgstr "Appellation"
+msgstr "Denominazione"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:34
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:206
 msgctxt "Text on generated order PDF"
 msgid "Anzahl"
-msgstr "Quantité"
+msgstr "Quantità"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:35
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:207
 msgctxt "Text on generated order PDF"
 msgid "Einheit"
-msgstr "Unité"
+msgstr "Unità"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:36
 msgctxt "Text on generated order PDF"
 msgid "Preis"
-msgstr "Prix"
+msgstr "Prezzo"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:37
 msgctxt "Text on generated order PDF"
 msgid "Total"
-msgstr "Total"
+msgstr "Totale"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:58
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:93
 msgctxt "Text on generated order PDF"
 msgid "Rabatt"
-msgstr "Réduction"
+msgstr "Sconto"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:119
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:572
 msgctxt "Text on generated order PDF"
 msgid "MwSt"
-msgstr "TVA"
+msgstr "IVA"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:136
 #, python-format
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag, zahlbar netto innert %s Tagen"
-msgstr "Montant net, payable à %s jours"
+msgstr "Importo netto, pagabile entro %s giorni"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:138
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsbetrag"
-msgstr "Montant de la facture"
+msgstr "Importo della fattura"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:154
 #, python-format
 msgctxt "Text on generated order PDF"
 msgid "%(days)s Tage %(percent)s%% Skonto"
-msgstr "%(days)s jours %(percent)s%% de remise"
+msgstr "%(days)s giorni %(percent)s%% di sconto"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:234
 msgctxt "Text on generated order PDF"
 msgid "Anzahl Produkte"
-msgstr "Nombre de produits"
+msgstr "Numero di prodotti"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:433
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Vor der Einzahlung abzutrennen"
-msgstr "A détacher avant le versement"
+msgstr "Da staccare prima del versamento"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:445
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:463
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Konto / Zahlbar an"
-msgstr "Compte / Payable à"
+msgstr "Conto / Pagabile a"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:452
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:470
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Referenz"
-msgstr "Référence"
+msgstr "Riferimento"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:455
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:478
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlbar durch"
-msgstr "Payable par"
+msgstr "Pagabile da"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:473
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zusätzliche Informationen"
-msgstr "Informations additionnelles"
+msgstr "Informazioni aggiuntive"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:486
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Empfangsschein"
-msgstr "Récépissé"
+msgstr "Ricevuta"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:487
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Zahlteil"
-msgstr "Section paiement"
+msgstr "Sezione pagamento"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:490
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:499
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Währung"
-msgstr "Monnaie"
+msgstr "Valuta"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:491
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:500
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Betrag"
-msgstr "Montant"
+msgstr "Importo"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:492
 msgctxt "QR-Invoice / fixed by SIX group style guide"
 msgid "Annahmestelle"
-msgstr "Point de dépôt"
+msgstr "Punto di accettazione"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:567
 msgctxt "Text on generated order PDF"
 msgid "Tel."
 msgstr "Tel."
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:568
@@ -163,102 +163,102 @@
 msgctxt "Text on generated order PDF"
 msgid "Web"
 msgstr "Web"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:589
 msgctxt "Text on generated order PDF"
 msgid "Ihre Kundennummer"
-msgstr "Votre numéro de client"
+msgstr "Il Suo codice cliente"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:590
 msgctxt "Text on generated order PDF"
 msgid "Bestellnummer"
-msgstr "Numéro de commande"
+msgstr "Numero d'ordine"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:591
 msgctxt "Text on generated order PDF"
 msgid "Bestelldatum"
-msgstr "Date de commande"
+msgstr "Data dell'ordine"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:593
 msgctxt "Text on generated order PDF"
 msgid "Datum"
-msgstr "Date"
+msgstr "Data"
 
 #: .\kmuhelper\modules\pdfgeneration\order\generator.py:595
 msgctxt "Text on generated order PDF"
 msgid "Rechnungsdatum"
-msgstr "Date de facture"
+msgstr "Data della fattura"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:48
 msgid "Rechnung"
-msgstr "Facture"
+msgstr "Fattura"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:52
 msgid "Lieferschein"
-msgstr "Bon de livraison"
+msgstr "Nota di consegna"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:57
 msgid "Zahlungserinnerung"
-msgstr "Rappel de paiement"
+msgstr "Promemoria di pagamento"
 
 #: .\kmuhelper\modules\pdfgeneration\order\views.py:58
 #, python-format
 msgid ""
 "Geschätzter Kunde\n"
 "\n"
 "Vermutlich ist Ihnen entgangen, diese Rechnung vom %(original_date)s innert "
 "der gewährten Frist zu begleichen.\n"
 "Wir bitten Sie, dies innert %(days)d Tagen nachzuholen.\n"
 "\n"
 "Sollte sich Ihre Zahlung mit diesem Schreiben überkreuzen, so betrachten Sie "
 "dieses bitte als gegenstandslos."
 msgstr ""
-"Cher client\n"
+"Gentile Cliente\n"
 "\n"
-"Vous n'avez probablement pas réglé cette facture du %(original_date)s dans "
-"le délai imparti.\n"
-"Nous vous prions de bien vouloir le faire dans les %(days)d jours.\n"
+"Riteniamo che non abbiate pagato questa fattura dell' %(original_date)s "
+"entro i termini previsti.\n"
+"Vi chiediamo gentilmente di farlo entro %(days)d giorni.\n"
 "\n"
-"Si votre paiement devait se recouper avec cette lettre, veuillez considérer "
-"que celle-ci est sans objet."
+"Se il vostro pagamento dovesse incrociarsi con questa lettera, consideratela "
+"irrilevante."
 
 #: .\kmuhelper\translations.py:23
 msgctxt "quantity description"
 msgid "Stück"
 msgid_plural "Stück"
-msgstr[0] "Pièce"
-msgstr[1] "Pièces"
+msgstr[0] "Pezzo"
+msgstr[1] "Pezzi"
 
 #: .\kmuhelper\translations.py:31
 msgctxt "quantity description"
 msgid "Stunde"
 msgid_plural "Stunden"
-msgstr[0] "Heure"
-msgstr[1] "Heures"
+msgstr[0] "Ora"
+msgstr[1] "Ore"
 
 #: .\kmuhelper\translations.py:39
 msgctxt "quantity description"
 msgid "Einheit"
 msgid_plural "Einheiten"
-msgstr[0] "Unité"
-msgstr[1] "Unités"
+msgstr[0] "Unità"
+msgstr[1] "Unità"
 
 #: .\kmuhelper\translations.py:47
 msgctxt "quantity description"
 msgid "Flasche"
 msgid_plural "Flaschen"
-msgstr[0] "Bouteille"
-msgstr[1] "Bouteilles"
+msgstr[0] "Bottiglia"
+msgstr[1] "Bottiglie"
 
 #: .\kmuhelper\translations.py:55
 msgctxt "quantity description"
 msgid "Tube"
 msgid_plural "Tuben"
-msgstr[0] "Tube"
-msgstr[1] "Tubes"
+msgstr[0] "Tubo"
+msgstr[1] "Tubi"
 
 #~ msgid "Ihr/e Ansprechpartner/in"
-#~ msgstr "Votre interlocuteur"
+#~ msgstr "La Sua controparte"
 
 #~ msgid "Ihre Bestellung vom"
-#~ msgstr "Votre commande du"
+#~ msgstr "La Sua ordinazione del"
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/management/commands/kmuhelper-import-customers.py` & `django_kmuhelper-1.8.2/kmuhelper/management/commands/kmuhelper-import-customers.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/management/commands/model2csv.py` & `django_kmuhelper-1.8.2/kmuhelper/management/commands/model2csv.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0101_squashed_0100_to_0100.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0101_squashed_0100_to_0100.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0102_paymentreceiver_improvements.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0102_paymentreceiver_improvements.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0103_paymentreceiver_invoice_display_mode.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0103_paymentreceiver_invoice_display_mode.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0104_order_payment_purpose.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0104_order_payment_purpose.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0105_alter_setting_options_alter_settinghidden_options.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0105_alter_setting_options_alter_settinghidden_options.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0106_alter_app_arrival_options_and_more.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0106_alter_app_arrival_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0107_alter_emailtemplate_mail_subject_and_more.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0107_alter_emailtemplate_mail_subject_and_more.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0108_migrate_vat_rates_for_2024.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0108_migrate_vat_rates_for_2024.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/migrations/0109_contactperson_is_default_paymentreceiver_is_default.py` & `django_kmuhelper-1.8.2/kmuhelper/migrations/0109_contactperson_is_default_paymentreceiver_is_default.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/api/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/api/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     fieldsets = [
         ("Settings", {"fields": ("name", "user", ("read", "write"))}),
         ("Key", {"fields": ("key",), "classes": ("collapse",)}),
     ]
 
     ordering = ("id",)
 
-    hidden = True
+    HIDDEN = True
 
 
 #
 
 
 modeladmins = [
     (ApiKey, ApiKeyAdmin),
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/api/constants.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/api/constants.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/api/decorators.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/api/decorators.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/api/models.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/api/models.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/api/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/api/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/app/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/app/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,87 +16,88 @@
 from kmuhelper.overrides import CustomModelAdmin
 
 
 #######
 
 
 class App_AdminBase(CustomModelAdmin):
-    hidden = True
+    HIDDEN = True
 
 
 @admin.register(App_ToDo)
 class App_ToDoAdmin(App_AdminBase, NoteAdmin):
+    list_display = ["pkfill", "name", "description", "priority", "done", "created_at"]
     list_editable = ["priority", "done"]
     list_filter = ["priority"]
 
     ordering = ["-priority", "created_at"]
 
 
 @admin.register(App_Shipping)
 class App_ShippingAdmin(App_AdminBase, OrderAdmin):
-    list_display = (
-        "id",
+    list_display = [
+        "pkfill",
         "info",
         "status",
         "shipped_on",
         "is_shipped",
         "tracking_number",
         "linked_note_html",
-    )
-    list_editable = ("shipped_on", "is_shipped", "status", "tracking_number")
-    list_filter = ("status", "is_paid")
+    ]
+    list_editable = ["shipped_on", "is_shipped", "status", "tracking_number"]
+    list_filter = ["status", "is_paid"]
 
-    ordering = ("is_paid", "-date")
+    ordering = ["is_paid", "-date"]
 
-    actions = ()
+    actions = []
 
 
 @admin.register(App_IncomingPayments)
 class App_IncomingPaymentsAdmin(App_AdminBase, OrderAdmin):
-    list_display = (
-        "id",
+    list_display = [
+        "pkfill",
         "info",
         "status",
         "paid_on",
         "is_paid",
         "display_cached_sum",
         "display_payment_conditions",
         "linked_note_html",
-    )
-    list_editable = ("paid_on", "is_paid", "status")
-    list_filter = ("status", "is_shipped", "payment_method")
+    ]
+    list_editable = ["paid_on", "is_paid", "status"]
+    list_filter = ["status", "is_shipped", "payment_method"]
 
-    ordering = (
+    ordering = [
         "status",
         "invoice_date",
-    )
+    ]
 
-    actions = ()
+    actions = []
 
 
 @admin.register(App_Stock)
 class App_StockAdmin(App_AdminBase, ProductAdmin):
-    list_display = (
-        "nr",
+    list_display = [
+        "pkfill",
+        "display_article_number",
         "clean_name",
         "stock_current",
-        "get_current_price",
+        "display_current_price",
         "note",
         "linked_note_html",
-    )
-    list_display_links = ("nr",)
+    ]
     list_editable = ["stock_current"]
 
     actions = ["reset_stock"]
 
 
 @admin.register(App_Arrival)
 class App_ArrivalAdmin(App_AdminBase, SupplyAdmin):
-    list_display = ("name", "date", "total_quantity", "linked_note_html")
-    list_filter = ()
+    list_display = ["pkfill", "name", "date", "total_quantity", "linked_note_html"]
+    list_filter = []
 
 
 #
 
 
 modeladmins = [
     (App_ToDo, App_ToDoAdmin),
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/app/models.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/app/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django.contrib import admin
 from django.db import models
 from django.utils.translation import gettext_lazy
 
 from kmuhelper.modules.main.models import Note, Order, Product, Supply
 
 _ = gettext_lazy
 
@@ -21,16 +20,16 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Notiz")
         verbose_name_plural = _("Notizen")
         default_permissions = []
 
-    admin_title = _("ToDo-Liste")
-    admin_description = _("Unerledigten Notizen")
+    ADMIN_TITLE = _("ToDo-Liste")
+    ADMIN_DESCRIPTION = _("Unerledigten Notizen")
 
 
 class App_ShippingManager(models.Manager):
     def get_queryset(self):
         return super().get_queryset().filter(is_shipped=False)
 
 
@@ -41,17 +40,17 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Bestellung")
         verbose_name_plural = _("Bestellungen")
         default_permissions = []
 
-    admin_title = _("Warenausgang")
-    admin_description = _("Nicht versendete Bestellungen")
-    admin_icon = "fas fa-box-open"
+    ADMIN_TITLE = _("Warenausgang")
+    ADMIN_DESCRIPTION = _("Nicht versendete Bestellungen")
+    ADMIN_ICON = "fa-solid fa-box-open"
 
 
 class App_IncomingPaymentsManager(models.Manager):
     def get_queryset(self):
         return super().get_queryset().filter(is_paid=False)
 
 
@@ -62,38 +61,33 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Bestellung")
         verbose_name_plural = _("Bestellungen")
         default_permissions = []
 
-    admin_title = _("Zahlungseingang")
-    admin_description = _("Nicht bezahlte Bestellungen")
-    admin_icon = "fas fa-hand-holding-dollar"
+    ADMIN_TITLE = _("Zahlungseingang")
+    ADMIN_DESCRIPTION = _("Nicht bezahlte Bestellungen")
+    ADMIN_ICON = "fa-solid fa-hand-holding-dollar"
 
 
 class App_Stock(Product):
     IS_APP_MODEL = True
 
-    @admin.display(description=_("Preis"))
-    def get_current_price(self, *args, **kwargs):
-        return super().get_current_price(*args, **kwargs)
-
-    @admin.display(description=_("Nr."), ordering="article_number")
-    def nr(self):
-        return self.article_number
+    display_current_price = Product.display_current_price
+    display_article_number = Product.display_article_number
 
     class Meta:
         proxy = True
         verbose_name = _("Produkt")
         verbose_name_plural = _("Produkte")
         default_permissions = []
 
-    admin_title = _("Lagerbestand")
-    admin_description = _("Alle Produkte im Lager")
+    ADMIN_TITLE = _("Lagerbestand")
+    ADMIN_DESCRIPTION = _("Alle Produkte im Lager")
 
 
 class App_ArrivalManager(models.Manager):
     def get_queryset(self):
         return super().get_queryset().filter(is_added_to_stock=False)
 
 
@@ -104,9 +98,9 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Lieferung")
         verbose_name_plural = _("Lieferungen")
         default_permissions = []
 
-    admin_title = _("Wareneingang")
-    admin_description = _("Nicht eingelagerte Lieferungen")
+    ADMIN_TITLE = _("Wareneingang")
+    ADMIN_DESCRIPTION = _("Nicht eingelagerte Lieferungen")
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/app/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/app/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/config.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/config.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/emails/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/emails/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,33 @@
 _ = gettext_lazy
 
 #######
 
 
 @admin.register(Attachment)
 class AttachmentAdmin(CustomModelAdmin):
-    list_display = ["filename", "description", "time_created", "autocreated", "id"]
-    list_display_links = ["filename"]
+    list_display = [
+        "pkfill",
+        "filename",
+        "description",
+        "time_created",
+        "autocreated",
+        "id",
+    ]
 
     search_fields = (
         "filename",
         "description",
     )
 
     ordering = ["-time_created"]
 
     save_on_top = True
 
-    hidden = True
+    HIDDEN = True
 
     def get_readonly_fields(self, request, obj=None):
         if obj:
             return ["time_created", "file", "autocreated"]
 
         return ["time_created", "autocreated"]
 
@@ -103,14 +109,15 @@
         return default
 
     readonly_fields = ("time_created", "time_sent")
 
     ordering = ("sent", "-time_sent", "-time_created")
 
     list_display = (
+        "pkfill",
         "subject",
         "to",
         "html_template",
         "time_created",
         "sent",
         "time_sent",
     )
@@ -118,15 +125,15 @@
 
     search_fields = ["subject", "to", "cc", "bcc", "html_context", "text", "notes"]
 
     inlines = (EMailAdminAttachmentInline,)
 
     save_on_top = True
 
-    hidden = True
+    HIDDEN = True
 
     # Views
 
     def get_urls(self):
         info = self.model._meta.app_label, self.model._meta.model_name
 
         urls = super().get_urls()
@@ -156,15 +163,15 @@
         if obj:
             obj.is_valid(request)
         super().save_model(request, obj, form, change)
 
 
 @admin.register(EMailTemplate)
 class EMailTemplateAdmin(CustomModelAdmin):
-    list_display = ["title", "description", "get_use_link"]
+    list_display = ["pkfill", "title", "description", "get_use_link"]
 
     search_fields = (
         "title",
         "description",
     )
 
     ordering = ["title"]
@@ -173,15 +180,15 @@
         (_("Infos"), {"fields": ["title", "description"]}),
         (_("Inhalt"), {"fields": ["mail_to", "mail_subject", "mail_text"]}),
         (_("Optionen"), {"fields": ["mail_template", "mail_context"]}),
     ]
 
     save_on_top = True
 
-    hidden = True
+    HIDDEN = True
 
     # Views
 
     def get_urls(self):
         info = self.model._meta.app_label, self.model._meta.model_name
 
         urls = super().get_urls()
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/emails/models.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/emails/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 from django.http import FileResponse
 from django.template import TemplateDoesNotExist, TemplateSyntaxError, Template, Context
 from django.template.loader import get_template
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy, gettext
-from rich import print
-
 from kmuhelper import settings, constants
 from kmuhelper.external.multi_email_field.fields import MultiEmailField
 from kmuhelper.overrides import CustomModel
 from kmuhelper.translations import Language
+from rich import print
 
 _ = gettext_lazy
 
 
 def log(string, *args):
     print("[deep_pink4][KMUHelper E-Mails][/] -", string, *args)
 
@@ -105,15 +104,15 @@
     class Meta:
         verbose_name = _("Anhang")
         verbose_name_plural = _("Anhänge")
         default_permissions = ("add", "change", "view", "delete", "download")
 
     objects = AttachmentManager()
 
-    admin_icon = "fas fa-paperclip"
+    ADMIN_ICON = "fa-solid fa-paperclip"
 
     # Custom delete
 
     def delete(self, *args, **kwargs):
         """Delete the associated file before deleting the model object"""
 
         self.file.delete()
@@ -386,20 +385,22 @@
     class Meta:
         verbose_name = _("E-Mail")
         verbose_name_plural = _("E-Mails")
         default_permissions = ("add", "change", "view", "delete", "send")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-envelope"
+    ADMIN_ICON = "fa-solid fa-envelope"
 
 
 class EMailTemplate(CustomModel):
     """Model representing an email template (not to confuse with design template)"""
 
+    PKFILL_WIDTH = 3
+
     title = models.CharField(
         verbose_name=_("Titel"),
         max_length=50,
     )
     description = models.TextField(
         verbose_name=_("Beschreibung"),
         default="",
@@ -485,8 +486,8 @@
 
     class Meta:
         verbose_name = _("E-Mail-Vorlage")
         verbose_name_plural = _("E-Mail-Vorlagen")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-envelope-open-text"
+    ADMIN_ICON = "fa-solid fa-envelope-open-text"
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/emails/utils.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/emails/utils.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/emails/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/emails/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         ("Infos", {"fields": ["is_processed", "time_imported"]}),
         ("Daten", {"fields": ["data_msgid", "data_creationdate"]}),
     ]
 
     ordering = ("is_processed",)
 
     list_display = (
+        "pkfill",
         "time_imported",
         "entrycount",
         "is_processed",
         "data_msgid",
     )
     list_filter = ("is_processed",)
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/forms.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/forms.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/models.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 _ = gettext_lazy
 
 
 #############
 
 
 class PaymentImport(CustomModel):
+    PKFILL_WIDTH = 5
+
     time_imported = models.DateTimeField(
         verbose_name=_("Importiert am"),
         auto_now_add=True,
     )
     is_processed = models.BooleanField(
         verbose_name=_("Verarbeitet?"),
         default=False,
@@ -95,15 +97,15 @@
                     context["notfound"].append(data)
         return context
 
     class Meta:
         verbose_name = _("Zahlungsimport")
         verbose_name_plural = _("Zahlungsimporte")
 
-    admin_icon = "fas fa-file-import"
+    ADMIN_ICON = "fa-solid fa-file-import"
 
 
 class PaymentImportEntry(models.Model):
     parent = models.ForeignKey(
         to="PaymentImport",
         on_delete=models.CASCADE,
         related_name="entries",
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/paymentimport/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/paymentimport/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/forms.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/forms.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/urls.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/urls.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/integrations/woocommerce/utils.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/integrations/woocommerce/utils.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/main/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/main/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from django.contrib import admin, messages
 from django.db.models import Count
-from django.urls import path
+from django.urls import path, reverse
 from django.utils import timezone
+from django.utils.html import format_html
 from django.utils.translation import gettext_lazy, ngettext
-
 from kmuhelper import constants
-from kmuhelper.modules.integrations.woocommerce import WooCommerce
+from kmuhelper.modules.integrations.woocommerce.api import (
+    WCCustomersAPI,
+    WCOrdersAPI,
+    WCProductsAPI,
+    WCProductCategoriesAPI,
+)
+from kmuhelper.modules.integrations.woocommerce.filters import WooCommerceStateFilter
+from kmuhelper.modules.integrations.woocommerce.utils import is_connected
 from kmuhelper.modules.main import views
+from kmuhelper.modules.main.filters import ProductTypeFilter
 from kmuhelper.modules.main.models import (
     ContactPerson,
     Order,
     ProductCategory,
     Fee,
     Customer,
     Supplier,
@@ -21,14 +29,15 @@
 )
 from kmuhelper.modules.pdfgeneration.order import views as pdf_order_views
 from kmuhelper.overrides import (
     CustomModelAdmin,
     CustomTabularInline,
     CustomStackedInline,
 )
+from kmuhelper.utils import formatprice
 
 _ = gettext_lazy
 
 #######
 
 
 @admin.register(ContactPerson)
@@ -37,15 +46,15 @@
         (_("Name"), {"fields": ["name"]}),
         (_("Kontaktinformationen"), {"fields": ["phone", "email"]}),
         (_("Optionen"), {"fields": ["is_default"]}),
     ]
 
     ordering = ("name",)
 
-    list_display = ("name", "phone", "email", "is_default")
+    list_display = ("pkfill", "name", "phone", "email", "is_default")
     search_fields = ["name", "phone", "email"]
 
     def save_model(self, request, obj, form, change):
         super().save_model(request, obj, form, change)
         if obj.is_default:
             ContactPerson.objects.filter(is_default=True).exclude(pk=obj.pk).update(
                 is_default=False
@@ -55,64 +64,93 @@
 class OrderAdminOrderItemInline(CustomTabularInline):
     model = Order.products.through
     verbose_name = _("Bestellungsposten")
     verbose_name_plural = _("Bestellungsposten")
     extra = 0
 
     fields = (
-        "product",
+        "display_product_link",
+        "article_number",  # hidden by default
+        "name",
         "note",
         "product_price",
         "quantity",
+        "quantity_description",  # hidden by default
         "discount",
         "display_subtotal",
-        "display_vat_rate",
+        "vat_rate",
     )
 
     readonly_fields = (
+        "display_product_link",
         "display_subtotal",
-        "display_vat_rate",
-        "product",
     )
 
     def get_additional_readonly_fields(self, request, obj=None):
-        fields = ["product_price"]
+        fields = []
         if obj and (obj.is_shipped or obj.is_paid):
             fields += ["quantity"]
         if obj and obj.is_paid:
-            fields += ["discount"]
+            fields += ["product_price", "vat_rate", "discount"]
         return fields
 
+    # Display items
+
+    @admin.display(description=_("Produkt"), ordering="linked_product")
+    def display_product_link(self, obj):
+        if obj.linked_product_id is None:
+            return "-"
+
+        link = reverse("admin:kmuhelper_product_change", args=(obj.linked_product_id,))
+
+        return format_html(
+            '<a href="{}">{}</a>', link, str(obj.linked_product_id).zfill(6)
+        )
+
+    @admin.display(description=_("Summe (exkl. MwSt)"))
+    def display_subtotal(self, obj):
+        return formatprice(obj.calc_subtotal()) + " CHF"
+
     # Permissions
 
-    NO_ADD = True
+    def has_add_permission(self, request, obj=None):
+        return (
+            False
+            if (obj and (obj.is_paid or obj.is_shipped))
+            else super().has_add_permission(request, obj)
+        )
 
     def has_delete_permission(self, request, obj=None):
         return (
             False
             if (obj and (obj.is_shipped or obj.is_paid))
             else super().has_delete_permission(request, obj)
         )
 
     # Custom queryset
 
     def get_queryset(self, request):
         qs = super().get_queryset(request)
-        return qs.select_related("product")
+        return qs.select_related("linked_product")
 
 
-class OrderAdminOrderItemInlineAdd(CustomTabularInline):
+class OrderAdminOrderItemInlineImport(CustomTabularInline):
     model = Order.products.through
     verbose_name = _("Bestellungsposten")
-    verbose_name_plural = _("Bestellungsposten hinzufügen")
+    verbose_name_plural = _("Bestellungsposten importieren")
     extra = 0
 
-    autocomplete_fields = ("product",)
+    autocomplete_fields = ("linked_product",)
 
-    fieldsets = [(None, {"fields": ["product", "note", "quantity", "discount"]})]
+    fields = (
+        "linked_product",
+        "note",
+        "quantity",
+        "discount",
+    )
 
     # Permissions
 
     NO_CHANGE = True
     NO_DELETE = True
     NO_VIEW = True
 
@@ -127,33 +165,48 @@
 class OrderAdminOrderFeeInline(CustomTabularInline):
     model = Order.fees.through
     verbose_name = _("Bestellungskosten")
     verbose_name_plural = _("Bestellungskosten")
     extra = 0
 
     fields = (
-        "linked_fee",
+        "display_fee_link",
         "name",
+        "note",
         "price",
         "discount",
-        "note",
         "display_subtotal",
         "vat_rate",
     )
 
     readonly_fields = (
-        "linked_fee",
+        "display_fee_link",
         "display_subtotal",
     )
 
     def get_additional_readonly_fields(self, request, obj=None):
         if obj and obj.is_paid:
             return ["price", "vat_rate", "discount"]
         return []
 
+    # Display items
+
+    @admin.display(description=_("Kosten"), ordering="linked_fee")
+    def display_fee_link(self, obj):
+        if obj.linked_fee_id is None:
+            return "-"
+
+        link = reverse("admin:kmuhelper_fee_change", args=(obj.linked_fee_id,))
+
+        return format_html('<a href="{}">{}</a>', link, str(obj.linked_fee_id).zfill(4))
+
+    @admin.display(description=_("Summe (exkl. MwSt)"))
+    def display_subtotal(self, obj):
+        return formatprice(obj.calc_subtotal()) + " CHF"
+
     # Permissions
 
     def has_add_permission(self, request, obj=None):
         return (
             False if (obj and obj.is_paid) else super().has_add_permission(request, obj)
         )
 
@@ -195,29 +248,31 @@
         return (
             False if (obj and obj.is_paid) else super().has_add_permission(request, obj)
         )
 
 
 @admin.register(Order)
 class OrderAdmin(CustomModelAdmin):
-    list_display = (
-        "id",
+    list_display = [
+        "pkfill",
         "date",
-        "customer",
+        "display_customer",
         "status",
         "payment_method",
-        "is_shipped",
-        "is_paid",
+        "display_is_shipped",
+        "display_is_paid",
         "display_cached_sum",
         "linked_note_html",
-    )
+    ]
+
     list_filter = (
         "status",
         "is_paid",
         "is_shipped",
+        WooCommerceStateFilter,
         "payment_method",
         "payment_receiver",
         "contact_person",
     )
     search_fields = (
         [
             "id",
@@ -241,17 +296,24 @@
 
     save_on_top = True
 
     list_select_related = ["customer", "linked_note"]
 
     date_hierarchy = "date"
 
+    def get_list_display(self, request):
+        if is_connected():
+            ls = self.list_display.copy()
+            ls.insert(1, "display_woocommerce_state")
+            return ls
+        return self.list_display
+
     def get_fieldsets(self, request, obj=None):
         if obj:
-            return [
+            fieldsets = [
                 (
                     _("Einstellungen"),
                     {"fields": ["payment_receiver", "contact_person"]},
                 ),
                 (_("Infos"), {"fields": ["name", "date", "status"]}),
                 (_("Kunde"), {"fields": ["customer"]}),
                 (
@@ -301,14 +363,21 @@
                         if obj.is_shipped
                         else constants.ADDR_SHIPPING_FIELDS_CATEGORIZED,
                         "classes": ["collapse start-open addr-shipping-fieldset"],
                     },
                 ),
             ]
 
+            if obj.woocommerceid:
+                fieldsets.insert(
+                    1, (_("Verknüpfungen"), {"fields": ["display_woocommerce_id"]})
+                )
+
+            return fieldsets
+
         return [
             (_("Einstellungen"), {"fields": ["payment_receiver", "contact_person"]}),
             (_("Infos"), {"fields": ["status"]}),
             (_("Kunde"), {"fields": ["customer"]}),
             (
                 _("Bezahlungsoptionen"),
                 {
@@ -329,14 +398,15 @@
 
     readonly_fields = (
         "linked_note_html",
         "name",
         "tracking_link",
         "display_total_breakdown",
         "display_payment_conditions",
+        "display_woocommerce_id",
     )
 
     def get_additional_readonly_fields(self, request, obj=None):
         fields = []
         if obj:
             if obj.is_shipped:
                 fields += [
@@ -352,15 +422,15 @@
             if obj.woocommerceid:
                 fields += ["customer_note"]
         return fields
 
     def get_inlines(self, request, obj=None):
         inlines = [OrderAdminOrderItemInline]
         if request.user.has_perm("kmuhelper.view_product"):
-            inlines += [OrderAdminOrderItemInlineAdd]
+            inlines += [OrderAdminOrderItemInlineImport]
         inlines += [OrderAdminOrderFeeInline]
         if request.user.has_perm("kmuhelper.view_fee"):
             inlines += [OrderAdminOrderFeeInlineImport]
         return inlines
 
     # Actions
 
@@ -373,55 +443,42 @@
                 errorcount += 1
             else:
                 order.is_paid = True
                 if order.is_shipped:
                     order.status = "completed"
                 order.save()
                 successcount += 1
-        messages.success(
-            request,
-            ngettext(
-                "%d Bestellung wurde als bezahlt markiert.",
-                "%d Bestellungen wurden als bezahlt markiert.",
-                successcount,
-            ),
-        )
+
+        if successcount:
+            messages.success(
+                request,
+                ngettext(
+                    "%d Bestellung wurde als bezahlt markiert.",
+                    "%d Bestellungen wurden als bezahlt markiert.",
+                    successcount,
+                )
+                % successcount,
+            )
         if errorcount:
             messages.warning(
                 request,
                 ngettext(
                     "%d Bestellung war bereits als bezahlt markiert.",
                     "%d Bestellungen waren bereits als bezahlt markiert.",
                     errorcount,
-                ),
+                )
+                % errorcount,
             )
 
     @admin.action(
         description=_("Bestellungen von WooCommerce aktualisieren"),
         permissions=["change"],
     )
     def wc_update(self, request, queryset):
-        successcount, errorcount = WooCommerce.order_bulk_update(queryset.all())
-        messages.success(
-            request,
-            ngettext(
-                "%d Bestellung wurde von WooCommerce aktualisiert.",
-                "%d Bestellungen wurden von WooCommerce aktualisiert.",
-                successcount,
-            ),
-        )
-        if errorcount:
-            messages.error(
-                request,
-                ngettext(
-                    "%d Bestellung konnte nicht von WooCommerce aktualisiert werden.",
-                    "%d Bestellungen konnten nicht von WooCommerce aktualisiert werden.",
-                    errorcount,
-                ),
-            )
+        WCOrdersAPI().bulk_update_objects_from_api(queryset.all(), request)
 
     actions = [mark_as_paid, wc_update]
 
     # Save
 
     def save_model(self, request, obj, form, change):
         super().save_model(request, obj, form, change)
@@ -476,15 +533,15 @@
             ),
         ]
         return my_urls + urls
 
 
 @admin.register(Fee)
 class FeeAdmin(CustomModelAdmin):
-    list_display = ["clean_name", "price", "vat_rate"]
+    list_display = ["pkfill", "clean_name", "price", "vat_rate"]
 
     search_fields = ("name", "price")
 
     ordering = (
         "price",
         "vat_rate",
     )
@@ -523,57 +580,28 @@
     NO_CHANGE = True
     NO_ADD = True
     NO_DELETE = True
 
 
 @admin.register(Customer)
 class CustomerAdmin(CustomModelAdmin):
-    def get_fieldsets(self, request, obj=None):
-        default = [
-            (
-                _("Infos"),
-                {"fields": ["first_name", "last_name", "company", "email", "language"]},
-            ),
-            (
-                _("Rechnungsadresse"),
-                {
-                    "fields": constants.ADDR_BILLING_FIELDS_CATEGORIZED,
-                    "classes": ["addr-billing-fieldset"],
-                },
-            ),
-            (
-                _("Lieferadresse"),
-                {
-                    "fields": constants.ADDR_SHIPPING_FIELDS_CATEGORIZED,
-                    "classes": ["addr-shipping-fieldset"],
-                },
-            ),
-        ]
-
-        if obj:
-            return default + [
-                (_("Diverses"), {"fields": ["website", "note", "linked_note_html"]}),
-                (_("Erweitert"), {"fields": ["combine_with"], "classes": ["collapse"]}),
-            ]
-
-        return default + [(_("Diverses"), {"fields": ["website", "note"]})]
-
-    ordering = ("addr_billing_postcode", "company", "last_name", "first_name")
-
-    list_display = (
-        "id",
+    list_display = [
+        "pkfill",
         "company",
         "last_name",
         "first_name",
         "addr_billing_postcode",
         "addr_billing_city",
         "email",
         "avatar",
         "linked_note_html",
-    )
+    ]
+
+    ordering = ("addr_billing_postcode", "company", "last_name", "first_name")
+
     search_fields = (
         [
             "id",
             "last_name",
             "first_name",
             "company",
             "email",
@@ -582,48 +610,74 @@
             "linked_note__name",
             "linked_note__description",
         ]
         + constants.ADDR_BILLING_FIELDS
         + constants.ADDR_SHIPPING_FIELDS
     )
 
-    readonly_fields = ["linked_note_html"]
+    readonly_fields = ["linked_note_html", "display_woocommerce_id"]
+
+    list_filter = [WooCommerceStateFilter]
 
     list_select_related = ["linked_note"]
 
     autocomplete_fields = ["combine_with"]
 
     inlines = [CustomerAdminOrderInline]
 
     save_on_top = True
 
+    def get_list_display(self, request):
+        if is_connected():
+            ls = self.list_display.copy()
+            ls.insert(1, "display_woocommerce_state")
+            return ls
+        return self.list_display
+
+    def get_fieldsets(self, request, obj=None):
+        fieldsets = [
+            (
+                _("Infos"),
+                {"fields": ["first_name", "last_name", "company", "email", "language"]},
+            ),
+            (
+                _("Rechnungsadresse"),
+                {
+                    "fields": constants.ADDR_BILLING_FIELDS_CATEGORIZED,
+                    "classes": ["addr-billing-fieldset"],
+                },
+            ),
+            (
+                _("Lieferadresse"),
+                {
+                    "fields": constants.ADDR_SHIPPING_FIELDS_CATEGORIZED,
+                    "classes": ["addr-shipping-fieldset"],
+                },
+            ),
+        ]
+
+        if obj:
+            if obj.woocommerceid:
+                fieldsets.insert(
+                    0, (_("Verknüpfungen"), {"fields": ["display_woocommerce_id"]})
+                )
+            return fieldsets + [
+                (_("Diverses"), {"fields": ["website", "note", "linked_note_html"]}),
+                (_("Erweitert"), {"fields": ["combine_with"], "classes": ["collapse"]}),
+            ]
+
+        return fieldsets + [(_("Diverses"), {"fields": ["website", "note"]})]
+
     # Actions
 
     @admin.action(
         description=_("Kunden von WooCommerce aktualisieren"), permissions=["change"]
     )
     def wc_update(self, request, queryset):
-        successcount, errorcount = WooCommerce.customer_bulk_update(queryset.all())
-        messages.success(
-            request,
-            ngettext(
-                "%d Kunde wurde von WooCommerce aktualisiert.",
-                "%d Kunden wurden von WooCommerce aktualisiert.",
-                successcount,
-            ),
-        )
-        if errorcount:
-            messages.error(
-                request,
-                ngettext(
-                    "%d Kunde konnte nicht von WooCommerce aktualisiert werden.",
-                    "%d Kunden konnten nicht von WooCommerce aktualisiert werden.",
-                    errorcount,
-                ),
-            )
+        WCCustomersAPI().bulk_update_objects_from_api(queryset.all(), request)
 
     actions = ["wc_update"]
 
     # Views
 
     def get_urls(self):
         info = self.model._meta.app_label, self.model._meta.model_name
@@ -662,15 +716,15 @@
             },
         ),
         (_("Notiz"), {"fields": ["note"], "classes": ["collapse", "start-open"]}),
     ]
 
     ordering = ("abbreviation",)
 
-    list_display = ("abbreviation", "name", "note")
+    list_display = ("pkfill", "abbreviation", "name", "note")
     search_fields = ["abbreviation", "name", "address", "note"]
 
     # Views
 
     def get_urls(self):
         info = self.model._meta.app_label, self.model._meta.model_name
 
@@ -749,14 +803,15 @@
             else super().has_add_permission(request, obj)
         )
 
 
 @admin.register(Supply)
 class SupplyAdmin(CustomModelAdmin):
     list_display = (
+        "pkfill",
         "name",
         "date",
         "total_quantity",
         "supplier",
         "is_added_to_stock",
         "linked_note_html",
     )
@@ -801,30 +856,34 @@
         successcount = 0
         errorcount = 0
         for supply in queryset.all():
             if supply.add_to_stock():
                 successcount += 1
             else:
                 errorcount += 1
-        messages.success(
-            request,
-            ngettext(
-                "%d Lieferung wurde als eingelagert markiert.",
-                "%d Lieferungen wurden als eingelagert markiert.",
-                successcount,
-            ),
-        )
+
+        if successcount:
+            messages.success(
+                request,
+                ngettext(
+                    "%d Lieferung wurde als eingelagert markiert.",
+                    "%d Lieferungen wurden als eingelagert markiert.",
+                    successcount,
+                )
+                % successcount,
+            )
         if errorcount:
             messages.error(
                 request,
                 ngettext(
                     "%d Lieferung konnte nicht eingelagert werden.",
                     "%d Lieferungen konnten nicht eingelagert werden.",
                     errorcount,
-                ),
+                )
+                % errorcount,
             )
 
     actions = ["add_to_stock"]
 
     # Views
 
     def get_urls(self):
@@ -840,15 +899,15 @@
             ),
         ]
         return my_urls + urls
 
 
 @admin.register(Note)
 class NoteAdmin(CustomModelAdmin):
-    list_display = ["name", "description", "priority", "done", "created_at"]
+    list_display = ["pkfill", "name", "description", "priority", "done", "created_at"]
     list_filter = ["done", "priority"]
 
     readonly_fields = ["links"]
 
     ordering = ["done", "-priority", "created_at"]
 
     search_fields = ("name", "description")
@@ -969,14 +1028,17 @@
                     )
 
 
 class ProductAdminProductCategoryInline(CustomTabularInline):
     model = Product.categories.through
     extra = 0
 
+    verbose_name = _("Verknüpfte Kategorie")
+    verbose_name_plural = _("Verknüpfte Kategorien")
+
     autocomplete_fields = ("category",)
 
     # Custom queryset
 
     def get_queryset(self, request):
         qs = super().get_queryset(request)
         return qs.select_related("category", "product")
@@ -987,18 +1049,105 @@
 
     def has_add_permission(self, request, obj=None):
         if not request.user.has_perm("kmuhelper.view_productcategory"):
             return False
         return super().has_add_permission(request, obj)
 
 
+class ProductAdminChildrenInline(CustomTabularInline):
+    model = Product
+    extra = 0
+    show_change_link = True
+
+    fk_name = "parent"
+    verbose_name = _("Untergeordnetes Produkt")
+    verbose_name_plural = _("Untergeordnete Produkte")
+
+    fields = [
+        "pkfill",
+        "article_number",
+        "name",
+        "selling_price",
+    ]
+
+    readonly_fields = ["pkfill", "display_woocommerce_state"]
+
+    def get_fields(self, request, obj=None):
+        if is_connected():
+            ls = self.fields.copy()
+            ls.insert(1, "display_woocommerce_state")
+            return ls
+        return self.fields
+
+    # Permissions
+
+    NO_ADD = True
+    NO_CHANGE = True
+
+
 @admin.register(Product)
 class ProductAdmin(CustomModelAdmin):
+    list_display = [
+        "pkfill",
+        "display_article_number",
+        "clean_name",
+        "clean_short_description",
+        "clean_description",
+        "html_image",
+        "display_current_price",
+        "is_on_sale",
+        "linked_note_html",
+    ]
+
+    ordering = ("article_number", "name")
+
+    list_filter = (
+        ProductTypeFilter,
+        WooCommerceStateFilter,
+        "supplier",
+        "categories",
+    )
+    search_fields = [
+        "pk",
+        "article_number",
+        "name",
+        "short_description",
+        "description",
+        "note",
+        "linked_note__name",
+        "linked_note__description",
+    ]
+
+    readonly_fields = ["pkfill", "linked_note_html", "display_woocommerce_id"]
+
+    autocomplete_fields = ("supplier",)
+
+    inlines = (ProductAdminProductCategoryInline, ProductAdminChildrenInline)
+
+    save_on_top = True
+
+    list_select_related = ["linked_note"]
+
+    def get_list_display(self, request):
+        if is_connected():
+            ls = self.list_display.copy()
+            ls.insert(1, "display_woocommerce_state")
+            return ls
+        return self.list_display
+
     def get_fieldsets(self, request, obj=None):
-        return [
+        fieldsets = [
+            (
+                _("Verknüpfungen"),
+                {
+                    "fields": ["display_woocommerce_id", "parent"]
+                    if obj and obj.woocommerceid
+                    else ["parent"]
+                },
+            ),
             (_("Infos"), {"fields": ["article_number", "name"]}),
             (
                 _("Beschrieb"),
                 {
                     "fields": ["short_description", "description"],
                     "classes": ["collapse start-open"],
                 },
@@ -1043,115 +1192,85 @@
                 {
                     "fields": ["note", "linked_note_html"] if obj else ["note"],
                     "classes": ["collapse start-open"],
                 },
             ),
         ]
 
-    ordering = ("article_number", "name")
-
-    list_display = (
-        "article_number",
-        "clean_name",
-        "clean_short_description",
-        "clean_description",
-        "get_current_price",
-        "is_on_sale",
-        "stock_current",
-        "html_image",
-        "linked_note_html",
-    )
-    list_display_links = (
-        "article_number",
-        "is_on_sale",
-    )
-    list_filter = ("supplier", "categories", "stock_current")
-    search_fields = [
-        "article_number",
-        "name",
-        "short_description",
-        "description",
-        "note",
-        "linked_note__name",
-        "linked_note__description",
-    ]
-
-    readonly_fields = ["linked_note_html"]
-
-    autocomplete_fields = ("supplier",)
-
-    inlines = (ProductAdminProductCategoryInline,)
-
-    save_on_top = True
-
-    list_select_related = ["linked_note"]
+        return fieldsets
 
     # Actions
 
     @admin.action(
         description=_("Produkte von WooCommerce aktualisieren"), permissions=["change"]
     )
     def wc_update(self, request, queryset):
-        successcount, errorcount = WooCommerce.product_bulk_update(queryset.all())
-        messages.success(
-            request,
-            ngettext(
-                "%d Produkt wurde von WooCommerce aktualisiert.",
-                "%d Produkte wurden von WooCommerce aktualisiert.",
-                successcount,
-            ),
-        )
-        if errorcount:
-            messages.error(
-                request,
-                ngettext(
-                    "%d Produkt konnte nicht von WooCommerce aktualisiert werden.",
-                    "%d Produkte konnten nicht von WooCommerce aktualisiert werden.",
-                    errorcount,
-                ),
-            )
+        WCProductsAPI().bulk_update_objects_from_api(queryset.all(), request)
 
     @admin.action(description=_("Lagerbestand zurücksetzen"), permissions=["change"])
     def reset_stock(self, request, queryset):
         for product in queryset.all():
             product.stock_current = 0
             product.save()
+        count = queryset.count()
         messages.success(
             request,
             ngettext(
                 "Lagerbestand von %d Produkt zurückgesetzt.",
                 "Lagerbestand von %d Produkten zurückgesetzt.",
-                queryset.count(),
-            ),
+                count,
+            )
+            % count,
         )
 
     @admin.action(description=_("Aktion beenden"), permissions=["change"])
     def end_sale(self, request, queryset):
         for product in queryset.all():
             product.sale_to = timezone.now()
             product.save()
+        count = queryset.count()
         messages.success(
             request,
             ngettext(
                 "Aktion von %d Produkt beendet.",
                 "Aktion von %d Produkten beendet.",
-                queryset.count(),
-            ),
+                count,
+            )
+            % count,
         )
 
     actions = ["wc_update", "reset_stock", "end_sale"]
 
     # Save
 
     def save_model(self, request, obj, form, change):
         super().save_model(request, obj, form, change)
         if obj:
             obj.show_stock_warning(request)
 
 
+class ProductCategoryAdminChildrenInline(CustomTabularInline):
+    model = ProductCategory
+    verbose_name = _("Unterkategorie")
+    verbose_name_plural = _("Unterkategorien")
+    extra = 0
+
+    fields = ("pkfill", "clean_name", "clean_description", "html_image")
+    readonly_fields = ("pkfill", "clean_name", "clean_description", "html_image")
+
+    show_change_link = True
+    show_full_result_count = True
+
+    # Permissions
+
+    NO_CHANGE = True
+    NO_DELETE = True
+    NO_ADD = True
+
+
 class ProductCategoryAdminProductInline(CustomStackedInline):
     model = Product.categories.through
     verbose_name = _("Produkt in dieser Kategorie")
     verbose_name_plural = _("Produkte in dieser Kategorie")
     extra = 0
 
     autocomplete_fields = ("product",)
@@ -1173,67 +1292,69 @@
         ):
             return False
         return super().has_add_permission(request, obj)
 
 
 @admin.register(ProductCategory)
 class ProductCategoryAdmin(CustomModelAdmin):
-    fieldsets = [
-        (_("Infos"), {"fields": ["name", "description", "image_url"]}),
-        (_("Übergeordnete Kategorie"), {"fields": ["parent_category"]}),
-    ]
-
-    list_display = (
+    list_display = [
+        "pkfill",
         "clean_name",
         "clean_description",
         "parent_category",
         "html_image",
         "total_quantity",
-    )
+    ]
+
     search_fields = ["name", "description"]
 
     ordering = ("parent_category", "name")
 
-    inlines = [ProductCategoryAdminProductInline]
+    readonly_fields = ("display_woocommerce_id",)
+
+    inlines = [ProductCategoryAdminChildrenInline, ProductCategoryAdminProductInline]
 
     list_select_related = ("parent_category",)
 
     autocomplete_fields = ("parent_category",)
 
+    def get_list_display(self, request):
+        if is_connected():
+            ls = self.list_display.copy()
+            ls.insert(1, "display_woocommerce_state")
+            return ls
+        return self.list_display
+
+    def get_fieldsets(self, request, obj=None):
+        fieldsets = [
+            (_("Infos"), {"fields": ["name", "description", "image_url"]}),
+            (_("Übergeordnete Kategorie"), {"fields": ["parent_category"]}),
+        ]
+
+        if obj and obj.woocommerceid:
+            fieldsets.insert(
+                0, (_("Verknüpfungen"), {"fields": ["display_woocommerce_id"]})
+            )
+
+        return fieldsets
+
     # Custom queryset
 
     def get_queryset(self, request):
         qs = super().get_queryset(request)
         return qs.annotate(total_quantity=Count("products"))
 
     # Actions
 
     @admin.action(
         description=_("Kategorien von WooCommerce aktualisieren"),
         permissions=["change"],
     )
     def wc_update(self, request, queryset):
-        successcount, errorcount = WooCommerce.category_bulk_update(queryset.all())
-        messages.success(
-            request,
-            ngettext(
-                "%d Kategorie wurde von WooCommerce aktualisiert.",
-                "%d Kategorien wurden von WooCommerce aktualisiert.",
-                successcount,
-            ),
-        )
-        if errorcount:
-            messages.error(
-                request,
-                ngettext(
-                    "%d Kategorie konnte nicht von WooCommerce aktualisiert werden.",
-                    "%d Kategorien konnten nicht von WooCommerce aktualisiert werden.",
-                    errorcount,
-                ),
-            )
+        WCProductCategoriesAPI().bulk_update_objects_from_api(queryset.all(), request)
 
     actions = ["wc_update"]
 
 
 @admin.register(PaymentReceiver)
 class PaymentReceiverAdmin(CustomModelAdmin):
     fieldsets = [
@@ -1258,14 +1379,15 @@
         (
             _("Weitere Informationen & Darstellung"),
             {"fields": ["swiss_uid", "website", "logourl"]},
         ),
     ]
 
     list_display = (
+        "pkfill",
         "admin_name",
         "mode",
         "active_iban",
         "invoice_display_mode",
         "is_default",
     )
     list_filter = (
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/main/mixins.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/main/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,11 +158,21 @@
     addr_shipping_phone = models.CharField(
         verbose_name=pgettext_lazy("address", "Telefon"),
         max_length=50,
         default="",
         blank=True,
     )
 
+    # Check function
+
+    def addresses_are_equal(self):
+        for field in constants.ADDR_FIELDS:
+            if getattr(self, f"addr_billing_{field}") != getattr(
+                self, f"addr_shipping_{field}"
+            ):
+                return False
+        return True
+
     # Meta
 
     class Meta:
         abstract = True
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/main/models.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/main/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 from django.utils import timezone
 from django.utils.html import mark_safe, format_html
 from django.utils.translation import (
     gettext_lazy,
     gettext,
     npgettext,
 )
-from rich import print
-
 from kmuhelper import settings, constants
 from kmuhelper.modules.emails.models import EMail, Attachment
+from kmuhelper.modules.integrations.woocommerce.mixins import WooCommerceModelMixin
 from kmuhelper.modules.main.mixins import AddressModelMixin
 from kmuhelper.modules.pdfgeneration import PDFOrder
 from kmuhelper.overrides import CustomModel
 from kmuhelper.translations import langselect, I18N_HELP_TEXT, Language
 from kmuhelper.utils import runden, formatprice, modulo10rekursiv, faq
+from rich import print
 
 _ = gettext_lazy
 
 
 def log(content, *args):
     print("[deep_pink4][KMUHelper Main][/] -", content, *args)
 
@@ -75,14 +75,16 @@
 
 #############
 
 
 class ContactPerson(CustomModel):
     """Model representing a contact person"""
 
+    PKFILL_WIDTH = 3
+
     name = models.CharField(
         verbose_name=_("Name"),
         max_length=50,
         help_text=_("Auf Rechnung ersichtlich!"),
     )
     phone = models.CharField(
         verbose_name=_("Telefon"),
@@ -103,23 +105,23 @@
             "Aktivieren, um diese Kontaktperson als Standard zu setzen. Die Standard-Kontaktperson wird bei "
             "der Erstellung einer neuen Bestellung sowie beim Import einer Bestellung von WooCommerce verwendet."
         ),
     )
 
     @admin.display(description=_("Ansprechpartner"), ordering="name")
     def __str__(self):
-        return f"{self.name} ({self.pk})"
+        return f"[{self.pk}] {self.name}"
 
     class Meta:
         verbose_name = _("Ansprechpartner")
         verbose_name_plural = _("Ansprechpartner")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-user-tie"
+    ADMIN_ICON = "fa-solid fa-user-tie"
 
 
 class OrderFee(CustomModel):
     """Model representing fees for an order (e.g. shipping costs)"""
 
     # Links to other models
     order = models.ForeignKey(
@@ -178,26 +180,21 @@
         return runden(self.price)
 
     def calc_discount(self):
         return runden(self.price * (self.discount / 100)) * -1
 
     # Display methods
     @admin.display(description=_("Name"), ordering="name")
-    def clean_name(self):
-        return langselect(self.name)
-
-    @admin.display(description=_("Zwischensumme (exkl. MwSt)"))
-    def display_subtotal(self):
-        return formatprice(self.calc_subtotal()) + " CHF"
+    def clean_name(self, lang="de"):
+        return langselect(self.name, lang)
 
-    @admin.display(description=_("Bestellungskosten"))
     def __str__(self):
         if self.linked_fee:
-            return f"({self.pk}) {self.clean_name()} ({self.linked_fee.pk})"
-        return f"({self.pk}) {self.clean_name()}"
+            return f"[{self.pk}] {self.clean_name()} (#{self.linked_fee.pk})"
+        return f"[{self.pk}] {self.clean_name()}"
 
     def save(self, *args, **kwargs):
         if self.pk is None and self.linked_fee is not None:
             self.name = self.linked_fee.name
             self.price = self.linked_fee.price
             self.vat_rate = self.linked_fee.vat_rate
         super().save(*args, **kwargs)
@@ -214,23 +211,29 @@
         self.order = order
         self.save()
 
 
 class OrderItem(CustomModel):
     """Model representing the connection between 'Order' and 'Product'"""
 
+    # Links to other models
     order = models.ForeignKey(
         to="Order",
         on_delete=models.CASCADE,
     )
-    product = models.ForeignKey(
+    linked_product = models.ForeignKey(
         to="Product",
-        verbose_name=_("Produkt"),
-        on_delete=models.PROTECT,
+        verbose_name=_("Verknüpftes Produkt"),
+        on_delete=models.SET_NULL,
+        null=True,
+        blank=True,
+        default=None,
     )
+
+    # Custom data printed on the invoice
     note = models.CharField(
         verbose_name=_("Bemerkung"),
         default="",
         max_length=250,
         blank=True,
         help_text=_("Wird auf die Rechnung gedruckt."),
     )
@@ -244,47 +247,78 @@
         default=0,
         validators=[
             MinValueValidator(0),
             MaxValueValidator(100),
         ],
     )
 
+    # Data copied from linked product
+    article_number = models.CharField(
+        verbose_name=_("Artikelnummer"),
+        max_length=25,
+    )
+    quantity_description = models.CharField(
+        verbose_name=_("Mengenbezeichnung"),
+        max_length=100,
+        default="Stück",
+        blank=True,
+        help_text=I18N_HELP_TEXT,
+    )
+    name = models.CharField(
+        verbose_name=_("Name"),
+        max_length=500,
+        default="",
+        help_text=I18N_HELP_TEXT,
+    )
     product_price = models.FloatField(
         verbose_name=_("Produktpreis (exkl. MwSt)"),
         default=0.0,
     )
+    vat_rate = models.FloatField(
+        verbose_name=_("MwSt-Satz"),
+        choices=constants.VAT_RATES,
+        default=constants.VAT_RATE_DEFAULT,
+    )
 
     # Calculated data
     def calc_subtotal(self):
         return runden(
             self.product_price * self.quantity * ((100 - self.discount) / 100)
         )
 
     def calc_subtotal_without_discount(self):
         return runden(self.product_price * self.quantity)
 
     def calc_discount(self):
         return runden(self.product_price * self.quantity * (self.discount / 100)) * -1
 
     # Display methods
+    @admin.display(description=_("Bezeichnung"), ordering="name")
+    def clean_name(self, lang="de"):
+        return langselect(self.name, lang)
+
     @admin.display(description=_("MwSt-Satz"))
     def display_vat_rate(self):
-        return formatprice(self.product.vat_rate)
-
-    @admin.display(description=_("Zwischensumme (exkl. MwSt)"))
-    def display_subtotal(self):
-        return formatprice(self.calc_subtotal()) + " CHF"
+        return formatprice(self.vat_rate)
 
-    @admin.display(description=_("Bestellungsposten"))
     def __str__(self):
-        return f"({self.pk}) {self.quantity}x {self.product.clean_name()} ({self.product.pk})"
+        if self.linked_product_id:
+            return (
+                f"[{self.pk}] {self.quantity}x {self.clean_name()} (Art. {self.article_number}, "
+                f"#{self.linked_product_id})"
+            )
+        return f"[{self.pk}] {self.quantity}x {self.clean_name()} (Art. {self.article_number})"
 
     def save(self, *args, **kwargs):
-        if not self.product_price:
-            self.product_price = runden(self.product.get_current_price())
+        if self.pk is None and self.linked_product is not None:
+            self.article_number = self.linked_product.article_number
+            self.quantity_description = self.linked_product.quantity_description
+            self.name = self.linked_product.name
+            self.product_price = runden(self.linked_product.get_current_price())
+            self.vat_rate = self.linked_product.vat_rate
         super().save(*args, **kwargs)
 
     class Meta:
         verbose_name = _("Bestellungsposten")
         verbose_name_plural = _("Bestellungsposten")
 
     objects = models.Manager()
@@ -292,24 +326,19 @@
     def copyto(self, order):
         self.pk = None
         self._state.adding = True
         self.order = order
         self.save()
 
 
-class Order(CustomModel, AddressModelMixin):
+class Order(CustomModel, AddressModelMixin, WooCommerceModelMixin):
     """Model representing an order"""
 
     NOTE_RELATION = "order"
 
-    woocommerceid = models.IntegerField(
-        verbose_name=_("WooCommerce ID"),
-        default=0,
-    )
-
     date = models.DateTimeField(
         verbose_name=_("Datum"),
         default=timezone.now,
     )
 
     invoice_date = models.DateField(
         verbose_name=_("Rechnungsdatum"),
@@ -358,24 +387,24 @@
         blank=True,
         null=True,
     )
     tracking_number = models.CharField(
         verbose_name=_("Trackingnummer"),
         default="",
         blank=True,
-        max_length=25,
+        max_length=35,
         validators=[
             RegexValidator(
-                r"^99\.[0-9]{2}\.[0-9]{6}\.[0-9]{8}$",
-                _("Bite benutze folgendes Format: 99.xx.xxxxxx.xxxxxxxx"),
+                r"^[A-Z0-9\.]{8,}$",
+                _(
+                    "Erlaubte Zeichen: Grossbuchstaben, Zahlen und Punkte. Länge: 8-35 Zeichen"
+                ),
             )
         ],
-        help_text=_(
-            "Bitte gib hier eine Trackingnummer der Schweizer Post ein. (optional)"
-        ),
+        help_text=_("Trackingnummer ohne Leerzeichen. (optional)"),
     )
 
     is_removed_from_stock = models.BooleanField(
         verbose_name=_("Ausgelagert?"),
         default=False,
     )
 
@@ -443,15 +472,15 @@
     )
 
     # Connections
 
     products = models.ManyToManyField(
         to="Product",
         through="OrderItem",
-        through_fields=("order", "product"),
+        through_fields=("order", "linked_product"),
     )
 
     fees = models.ManyToManyField(
         to="Fee",
         through="OrderFee",
         through_fields=("order", "linked_fee"),
     )
@@ -508,16 +537,17 @@
 
     def second_save(self, *args, **kwargs):
         "This HAS to be called after all related models have been saved."
 
         self.cached_sum = self.calc_total()
         if self.is_shipped and (not self.is_removed_from_stock):
             for i in self.products.through.objects.filter(order=self):
-                i.product.stock_current -= i.quantity
-                i.product.save()
+                if i.linked_product is not None:
+                    i.linked_product.stock_current -= i.quantity
+                    i.linked_product.save()
             self.is_removed_from_stock = True
 
         super().save(*args, **kwargs)
 
     def save(self, *args, **kwargs):
         if not self.pk and not self.woocommerceid and self.customer:
             self.import_customer_data()
@@ -593,43 +623,37 @@
                     "price": runden(self.cached_sum * (1 - (percent / 100))),
                 }
             )
         data.sort(key=lambda x: x["date"])
         return data
 
     def get_vat_dict(self):
-        "Get the VAT as a dictionary"
+        """Get the VAT as a dictionary
+
+        Format: { rate: total, rate2: total2 }"""
         vat_dict = {}
-        for p in self.products.through.objects.filter(order=self).select_related(
-            "product"
-        ):
-            if str(p.product.vat_rate) in vat_dict:
-                vat_dict[str(p.product.vat_rate)] += p.calc_subtotal()
+        for p in self.products.through.objects.filter(order=self):
+            if str(p.vat_rate) in vat_dict:
+                vat_dict[str(p.vat_rate)] += p.calc_subtotal()
             else:
-                vat_dict[str(p.product.vat_rate)] = p.calc_subtotal()
-        for k in self.fees.through.objects.filter(order=self).select_related(
-            "linked_fee"
-        ):
+                vat_dict[str(p.vat_rate)] = p.calc_subtotal()
+        for k in self.fees.through.objects.filter(order=self):
             if str(k.vat_rate) in vat_dict:
                 vat_dict[str(k.vat_rate)] += k.calc_subtotal()
             else:
                 vat_dict[str(k.vat_rate)] = k.calc_subtotal()
         for s in vat_dict:
             vat_dict[s] = runden(vat_dict[s])
         return vat_dict
 
     def calc_total_without_vat(self):
         total = 0
-        for i in self.products.through.objects.filter(order=self).select_related(
-            "product"
-        ):
+        for i in self.products.through.objects.filter(order=self):
             total += i.calc_subtotal()
-        for i in self.fees.through.objects.filter(order=self).select_related(
-            "linked_fee"
-        ):
+        for i in self.fees.through.objects.filter(order=self):
             total += i.calc_subtotal()
         return runden(total)
 
     def calc_total_vat(self):
         total_vat = 0
         vat_dict = self.get_vat_dict()
         for vat_rate in vat_dict:
@@ -652,39 +676,28 @@
         return (
             (
                 f"{self.date.year}-"
                 if self.date and not isinstance(self.date, str)
                 else ""
             )
             + (
-                f"{self.pkfill(6)}"
+                f"{self.pkfill()}"
                 + (f" (WC#{self.woocommerceid})" if self.woocommerceid else "")
             )
-            + (
-                f" - {self.customer}"
-                if self.customer is not None
-                else " " + gettext("Gast")
-            )
+            + " - "
+            + self.display_customer()
         )
 
     @admin.display(description=_("Info"))
     def info(self):
-        return f'{self.date.strftime("%d.%m.%Y")} - ' + (
-            (
-                self.customer.company
-                if self.customer.company
-                else (f"{self.customer.first_name} {self.customer.last_name}")
-            )
-            if self.customer
-            else "Gast"
-        )
+        return f'{self.date.strftime("%d.%m.%Y")} - ' + self.display_customer()
 
     @admin.display(description=_("Bezahlt nach"))
     def display_paid_after(self):
-        if self.paid_on is None:
+        if self.paid_on is None or self.invoice_date is None:
             return "-"
 
         daydiff = (self.paid_on - self.invoice_date).days
 
         return npgettext(
             "Paid after ...",
             _("%(count)d Tag") % {"count": daydiff},
@@ -703,14 +716,54 @@
             datestr = condition["date"].strftime("%d.%m.%Y")
             price = formatprice(condition["price"])
             percent = condition["percent"]
             output += f"{price} CHF " + gettext("bis") + f" {datestr} ({percent}%)<br>"
 
         return mark_safe(output)
 
+    @admin.display(description=_("Kunde"), ordering="customer")
+    def display_customer(self):
+        if self.customer:
+            return str(self.customer)
+
+        id0 = "0".zfill(Customer.PKFILL_WIDTH)
+        text = f"[{id0}] ({_('Gast')}) "
+        if self.addr_billing_first_name:
+            text += self.addr_billing_first_name + " "
+        if self.addr_billing_last_name:
+            text += self.addr_billing_last_name + " "
+        if self.addr_billing_company:
+            text += self.addr_billing_company + " "
+        if self.addr_billing_postcode and self.addr_billing_city:
+            text += f"({self.addr_billing_postcode} {self.addr_billing_city})"
+
+        return text
+
+    @admin.display(
+        description=format_html(
+            '<abbr title="{}"><i class="fa-solid fa-truck-fast"></i></abbr>',
+            _("Als versendet markiert?"),
+        ),
+        ordering="is_shipped",
+        boolean=True,
+    )
+    def display_is_shipped(self):
+        return self.is_shipped
+
+    @admin.display(
+        description=format_html(
+            '<abbr title="{}"><i class="fa-solid fa-hand-holding-dollar"></i></abbr>',
+            _("Als bezahlt markiert?"),
+        ),
+        ordering="is_paid",
+        boolean=True,
+    )
+    def display_is_paid(self):
+        return self.is_paid
+
     def is_correct_payment(self, amount: float, date: datetime):
         "Check if a payment made on a certain date has the correct amount for this order"
 
         if amount == self.cached_sum:
             return True
 
         for condition in self.get_payment_conditions_data():
@@ -894,21 +947,24 @@
         return new
 
     def copy_to_supply(self):
         new = Supply.objects.create(
             name=gettext("Rücksendung von Bestellung #%d") % self.pk,
         )
         for lp in self.products.through.objects.filter(order=self):
-            new.products.add(lp.product, through_defaults={"quantity": lp.quantity})
+            if lp.linked_product is not None:
+                new.products.add(
+                    lp.linked_product, through_defaults={"quantity": lp.quantity}
+                )
         new.save()
         return new
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-clipboard-list"
+    ADMIN_ICON = "fa-solid fa-clipboard-list"
 
     DICT_EXCLUDE_FIELDS = [
         "products",
         "fees",
         "email_link_invoice",
         "email_link_shipped",
         "customer",
@@ -921,14 +977,16 @@
         "order_key",
     ]
 
 
 class Fee(CustomModel):
     """Model representing additional costs"""
 
+    PKFILL_WIDTH = 3
+
     name = models.CharField(
         verbose_name=_("Bezeichnung"),
         max_length=500,
         default=_("Zusätzliche Kosten"),
         help_text=I18N_HELP_TEXT,
     )
     price = models.FloatField(
@@ -943,39 +1001,33 @@
 
     @admin.display(description=_("Bezeichnung"), ordering="name")
     def clean_name(self):
         return langselect(self.name)
 
     @admin.display(description=_("Kosten"))
     def __str__(self):
-        return (
-            f"{ self.clean_name() } ({ self.price } CHF"
-            + (f" + {self.vat_rate}% MwSt" if self.vat_rate else "")
-            + f") ({self.pk})"
-        )
+        vat_addition = f" + {self.vat_rate}% MwSt" if self.vat_rate else ""
+        return f"[{self.pk}] { self.clean_name() } ({ self.price } CHF{vat_addition})"
 
     class Meta:
         verbose_name = _("Kosten")
         verbose_name_plural = _("Kosten")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-coins"
+    ADMIN_ICON = "fa-solid fa-coins"
 
 
-class Customer(CustomModel, AddressModelMixin):
+class Customer(CustomModel, AddressModelMixin, WooCommerceModelMixin):
     """Model representing a customer"""
 
+    PKFILL_WIDTH = 8
+    WOOCOMMERCE_URL_FORMAT = "{}/wp-admin/user-edit.php?user_id={}"
     NOTE_RELATION = "customer"
 
-    woocommerceid = models.IntegerField(
-        verbose_name=_("WooCommerce ID"),
-        default=0,
-    )
-
     email = models.EmailField(
         verbose_name=_("E-Mail Adresse"),
         blank=True,
     )
     first_name = models.CharField(
         verbose_name=_("Vorname"),
         max_length=250,
@@ -1044,23 +1096,23 @@
     def avatar(self):
         if self.avatar_url:
             return mark_safe('<img src="' + self.avatar_url + '" width="50px">')
         return ""
 
     @admin.display(description=_("Kunde"))
     def __str__(self):
-        s = f"{self.pkfill(8)} "
+        s = f"[{self.pkfill()}] "
         if self.woocommerceid:
             s += f"(WC#{self.woocommerceid}) "
-        if self.first_name:
-            s += f"{self.first_name} "
-        if self.last_name:
-            s += f"{self.last_name} "
-        if self.company:
-            s += f"{self.company} "
+        if self.first_name or self.addr_billing_first_name:
+            s += f"{self.first_name or self.addr_billing_first_name} "
+        if self.last_name or self.addr_billing_last_name:
+            s += f"{self.last_name or self.addr_billing_last_name} "
+        if self.company or self.addr_billing_company:
+            s += f"{self.company or self.addr_billing_company} "
         if self.addr_billing_postcode and self.addr_billing_city:
             s += f"({self.addr_billing_postcode} {self.addr_billing_city})"
         return s
 
     class Meta:
         verbose_name = _("Kunde")
         verbose_name_plural = _("Kunden")
@@ -1137,22 +1189,24 @@
             )
 
             self.save()
             return self.email_link_registered
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-users"
+    ADMIN_ICON = "fa-solid fa-users"
 
     DICT_EXCLUDE_FIELDS = ["email_link_registered", "combine_with"]
 
 
 class Supplier(CustomModel):
     """Model representing a supplier (used only for categorizing)"""
 
+    PKFILL_WIDTH = 4
+
     abbreviation = models.CharField(
         verbose_name=_("Kürzel"),
         max_length=5,
     )
     name = models.CharField(
         verbose_name=_("Name"),
         max_length=50,
@@ -1202,30 +1256,30 @@
         null=True,
         default="",
         blank=True,
     )
 
     @admin.display(description=_("Lieferant"))
     def __str__(self):
-        return f"{self.name} ({self.pk})"
+        return f"[{self.pk}] {self.name}"
 
     def assign(self):
         products = Product.objects.filter(supplier=None)
         for product in products:
             product.supplier = self
             product.save()
         return products.count()
 
     class Meta:
         verbose_name = _("Lieferant")
         verbose_name_plural = _("Lieferanten")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-truck"
+    ADMIN_ICON = "fa-solid fa-truck"
 
 
 class SupplyItem(CustomModel):
     """Model representing the connection between 'Supply' and 'Product'"""
 
     supply = models.ForeignKey(
         to="Supply",
@@ -1239,15 +1293,15 @@
     quantity = models.IntegerField(
         verbose_name=_("Menge"),
         default=1,
     )
 
     @admin.display(description=_("Lieferungsposten"))
     def __str__(self):
-        return f"({self.supply.pk}) -> {self.quantity}x {self.product}"
+        return f"[{self.pk}] {self.quantity}x {self.product}"
 
     class Meta:
         verbose_name = _("Lieferungsposten")
         verbose_name_plural = _("Lieferungsposten")
 
     objects = models.Manager()
 
@@ -1299,23 +1353,23 @@
             self.is_added_to_stock = True
             self.save()
             return True
         return False
 
     @admin.display(description=_("Lieferung"))
     def __str__(self):
-        return f"{self.name} ({self.pk})"
+        return f"[{self.pk}] {self.name}"
 
     class Meta:
         verbose_name = _("Lieferung")
         verbose_name_plural = _("Lieferungen")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-truck-ramp-box"
+    ADMIN_ICON = "fa-solid fa-truck-ramp-box"
 
 
 class Note(CustomModel):
     """Model representing a note"""
 
     name = models.CharField(
         verbose_name=_("Name"),
@@ -1369,15 +1423,15 @@
         null=True,
         on_delete=models.CASCADE,
         related_name="linked_note",
     )
 
     @admin.display(description=_("🔗 Notiz"))
     def __str__(self):
-        return f"{self.name} ({self.pk})"
+        return f"[{self.pk}] {self.name}"
 
     def links(self):
         text = ""
         if self.linked_order:
             url = reverse(
                 "admin:kmuhelper_order_change",
                 kwargs={"object_id": self.linked_order.pk},
@@ -1409,32 +1463,27 @@
 
     class Meta:
         verbose_name = _("Notiz")
         verbose_name_plural = _("Notizen")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-note-sticky"
+    ADMIN_ICON = "fa-solid fa-note-sticky"
 
 
-class Product(CustomModel):
+class Product(CustomModel, WooCommerceModelMixin):
     """Model representing a product"""
 
     NOTE_RELATION = "product"
 
     article_number = models.CharField(
         verbose_name=_("Artikelnummer"),
         max_length=25,
     )
 
-    woocommerceid = models.IntegerField(
-        verbose_name=_("WooCommerce ID"),
-        default=0,
-    )
-
     name = models.CharField(
         verbose_name=_("Name"),
         max_length=500,
         help_text=I18N_HELP_TEXT,
     )
     short_description = models.TextField(
         verbose_name=_("Kurzbeschrieb"),
@@ -1531,14 +1580,23 @@
     )
     supplier_url = models.URLField(
         verbose_name=_("Lieferantenurl (Für Nachbestellungen)"),
         default="",
         blank=True,
     )
 
+    parent = models.ForeignKey(
+        to="self",
+        related_name="children",
+        verbose_name=_("Übergeordnetes Produkt"),
+        on_delete=models.SET_NULL,
+        blank=True,
+        null=True,
+    )
+
     categories = models.ManyToManyField(
         to="ProductCategory",
         through="ProductProductCategoryConnection",
         through_fields=("product", "category"),
         verbose_name=_("Kategorien"),
         related_name="products",
     )
@@ -1551,36 +1609,45 @@
     def clean_short_description(self, lang="de"):
         return langselect(self.short_description, lang)
 
     @admin.display(description=_("Beschrieb"), ordering="description")
     def clean_description(self, lang="de"):
         return langselect(self.description, lang)
 
-    @admin.display(description=_("In Aktion?"), boolean=True)
+    @admin.display(description=_("Aktion?"), boolean=True)
     def is_on_sale(self, zeitpunkt: datetime = None):
         zp = zeitpunkt or timezone.now()
         if self.sale_from and self.sale_to and self.sale_price:
             return bool((self.sale_from < zp) and (zp < self.sale_to))
         return False
 
-    @admin.display(description=_("Aktueller Preis in CHF (exkl. MwSt)"))
     def get_current_price(self, zeitpunkt: datetime = None):
         zp = zeitpunkt or timezone.now()
         return self.sale_price if self.is_on_sale(zp) else self.selling_price
 
-    @admin.display(description=_("Bild"), ordering="image_url")
+    @admin.display(description=_("Aktueller Preis"))
+    def display_current_price(self):
+        return formatprice(self.get_current_price()) + " CHF"
+
+    @admin.display(description=_("Nr."), ordering="article_number")
+    def display_article_number(self):
+        return self.article_number
+
+    @admin.display(description=_("Produktbild"), ordering="image_url")
     def html_image(self):
         if self.image_url:
             return format_html('<img src="{}" width="100px">', self.image_url)
         return ""
 
+    # Stock
+
     def get_reserved_stock(self):
         return (
             OrderItem.objects.filter(
-                order__is_shipped=False, product_id=self.pk
+                order__is_shipped=False, linked_product_id=self.pk
             ).aggregate(models.Sum("quantity"))["quantity__sum"]
             or 0
         )
 
     def get_incoming_stock(self):
         return (
             SupplyItem.objects.filter(
@@ -1646,32 +1713,32 @@
         if data["stock_overbooked"]:
             messages.error(request, data["message"])
         elif data["stock_in_danger"]:
             messages.warning(request, data["message"])
 
     @admin.display(description=_("Produkt"))
     def __str__(self):
-        return f"{self.article_number} - {self.clean_name()} ({self.pk})"
+        return f"[{self.pk}] {self.article_number} - {self.clean_name()}"
 
     class Meta:
         verbose_name = _("Produkt")
         verbose_name_plural = _("Produkte")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-cubes"
+    ADMIN_ICON = "fa-solid fa-cubes"
 
 
-class ProductCategory(CustomModel):
+class ProductCategory(CustomModel, WooCommerceModelMixin):
     """Model representing a category for products"""
 
-    woocommerceid = models.IntegerField(
-        verbose_name=_("WooCommerce ID"),
-        default=0,
+    WOOCOMMERCE_URL_FORMAT = (
+        "{}/wp-admin/term.php?taxonomy=product_cat&tag_ID={}&post_type=product"
     )
+    PKFILL_WIDTH = 4
 
     name = models.CharField(
         verbose_name=_("Bezeichnung"),
         max_length=250,
         default="",
     )
     description = models.TextField(
@@ -1708,23 +1775,23 @@
 
     @admin.display(description=_("Beschrieb"), ordering="description")
     def clean_description(self):
         return langselect(self.description)
 
     @admin.display(description=_("Kategorie"))
     def __str__(self):
-        return f"{self.clean_name()} ({self.pk})"
+        return f"[{self.pk}] {self.clean_name()}"
 
     class Meta:
         verbose_name = _("Produktkategorie")
         verbose_name_plural = _("Produktkategorien")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-folder-tree"
+    ADMIN_ICON = "fa-solid fa-folder-tree"
 
 
 class ProductProductCategoryConnection(CustomModel):
     """Model representing the connection between 'Product' and 'ProductCategory'"""
 
     product = models.ForeignKey(
         to="Product",
@@ -1735,26 +1802,28 @@
         to="ProductCategory",
         verbose_name=_("Produktkategorie"),
         on_delete=models.CASCADE,
     )
 
     @admin.display(description=_("Produkt-Kategorie-Verknüpfung"))
     def __str__(self):
-        return f"({self.category.pk}) {self.category.clean_name()} <-> {self.product}"
+        return f"{self.category.clean_name()} <- [{self.pk}] -> {self.product}"
 
     class Meta:
         verbose_name = _("Produkt-Kategorie-Verknüpfung")
         verbose_name_plural = _("Produkt-Kategorie-Verknüpfungen")
 
     objects = models.Manager()
 
 
 class PaymentReceiver(CustomModel):
     """Model representing a payment receiver for the qr bill"""
 
+    PKFILL_WIDTH = 3
+
     # Internal
 
     internal_name = models.CharField(
         verbose_name=_("Interne Bezeichnung"),
         max_length=250,
         default="",
     )
@@ -1966,15 +2035,15 @@
     def active_iban(self):
         return self.qriban if self.mode == "QRR" else self.iban
 
     # More
 
     @admin.display(description=_("Zahlungsempfänger"))
     def __str__(self):
-        return f"{self.admin_name} ({self.pk})"
+        return f"[{self.pk}] {self.admin_name}"
 
     def clean(self):
         super().clean()
 
         errors = {}
 
         if self.mode == "QRR" and not self.has_valid_qr_iban():
@@ -1995,8 +2064,8 @@
 
     class Meta:
         verbose_name = _("Zahlungsempfänger")
         verbose_name_plural = _("Zahlungsempfänger")
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-hand-holding-dollar"
+    ADMIN_ICON = "fa-solid fa-hand-holding-dollar"
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/main/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/main/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/base.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/base.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/forms.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/forms.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/generator.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """PDF creator for invoices and delivery notes"""
 
 from datetime import datetime
 
+from django.utils.translation import pgettext
 from kmuhelper import settings
+from kmuhelper.modules.pdfgeneration.base import PDFGenerator
+from kmuhelper.modules.pdfgeneration.swiss_qr_invoice import QRInvoiceFlowable
 from kmuhelper.translations import (
     autotranslate_quantity_description,
     autotranslate_fee_name,
     langselect,
 )
 from kmuhelper.utils import formatprice
-from kmuhelper.modules.pdfgeneration.base import PDFGenerator
-from kmuhelper.modules.pdfgeneration.swiss_qr_invoice import QRInvoiceFlowable
-
-from reportlab.platypus import Table, TableStyle, Paragraph, Spacer, TopPadder, Flowable
-from reportlab.lib.utils import ImageReader
-from reportlab.lib.units import mm
-from reportlab.lib.styles import ParagraphStyle
 from reportlab.lib.colors import black
-
-from django.utils.translation import pgettext
+from reportlab.lib.styles import ParagraphStyle
+from reportlab.lib.units import mm
+from reportlab.lib.utils import ImageReader
+from reportlab.platypus import Table, TableStyle, Paragraph, Spacer, TopPadder, Flowable
 
 style_default = ParagraphStyle("Normal", fontname="Helvetica")
 style_bold = ParagraphStyle("Bold", fontname="Helvetica-Bold")
 
 #####
 
 
@@ -42,78 +40,78 @@
             )
         ]
 
         # Products
 
         h_products = 0
 
-        for bp in order.products.through.objects.filter(order=order):
-            subtotal_without_discount = bp.calc_subtotal_without_discount()
+        for item in order.products.through.objects.filter(order=order):
+            subtotal_without_discount = item.calc_subtotal_without_discount()
             data.append(
                 (
-                    bp.product.article_number,
-                    Paragraph(langselect(bp.product.name, lang)),
-                    str(bp.quantity),
+                    item.article_number,
+                    Paragraph(langselect(item.name, lang)),
+                    str(item.quantity),
                     langselect(
                         autotranslate_quantity_description(
-                            bp.product.quantity_description, bp.quantity
+                            item.quantity_description, item.quantity
                         ),
                         lang,
                     ),
-                    formatprice(bp.product_price),
+                    formatprice(item.product_price),
                     formatprice(subtotal_without_discount),
                 )
             )
             h_products += 1
-            if bp.discount:
+            if item.discount:
                 data.append(
                     (
                         "",
                         "- " + pgettext("Text on generated order PDF", "Rabatt"),
-                        str(bp.discount),
+                        str(item.discount),
                         "%",
                         formatprice(subtotal_without_discount),
-                        formatprice(bp.calc_discount()),
+                        formatprice(item.calc_discount()),
                     )
                 )
                 h_products += 1
-            if bp.note:
-                data.append(("", Paragraph(f"- <b>{bp.note}</b>"), "", "", "", ""))
+            if item.note:
+                data.append(("", Paragraph(f"- <b>{item.note}</b>"), "", "", "", ""))
                 h_products += 1
 
         # Costs
 
         h_costs = 0
 
-        for bk in order.fees.through.objects.filter(order=order):
+        for item in order.fees.through.objects.filter(order=order):
             data.append(
                 (
                     "",
-                    Paragraph(langselect(autotranslate_fee_name(bk.name), lang)),
+                    Paragraph(langselect(autotranslate_fee_name(item.name), lang)),
                     "",
                     "",
                     "",
-                    formatprice(bk.price),
+                    formatprice(item.price),
                 )
             )
             h_costs += 1
-            if bk.discount:
+            if item.discount:
                 data.append(
                     (
                         "",
                         "- " + pgettext("Text on generated order PDF", "Rabatt"),
-                        str(bk.discount),
+                        str(item.discount),
                         "%",
-                        formatprice(bk.calc_subtotal_without_discount()),
-                        formatprice(bk.calc_discount()),
+                        formatprice(item.calc_subtotal_without_discount()),
+                        formatprice(item.calc_discount()),
                     )
                 )
                 h_costs += 1
-            if bk.note:
-                data.append(("", Paragraph(f"- <b>{bk.note}</b>"), "", "", "", ""))
+            if item.note:
+                data.append(("", Paragraph(f"- <b>{item.note}</b>"), "", "", "", ""))
                 h_costs += 1
 
         # VAT
 
         h_vat = 0
 
         vat_dict = dict(order.get_vat_dict())
@@ -243,32 +241,32 @@
             )
         ]
 
         productcount = 0
 
         # Products
 
-        for bp in order.products.through.objects.filter(order=order):
+        for item in order.products.through.objects.filter(order=order):
             data.append(
                 (
-                    bp.product.article_number,
-                    Paragraph(langselect(bp.product.name, lang)),
-                    str(bp.quantity),
+                    item.article_number,
+                    Paragraph(langselect(item.name, lang)),
+                    str(item.quantity),
                     langselect(
                         autotranslate_quantity_description(
-                            bp.product.quantity_description, bp.quantity
+                            item.quantity_description, item.quantity
                         ),
                         lang,
                     ),
                 )
             )
-            if bp.note:
-                data.append(("", Paragraph(f"- <b>{bp.note}</b>"), "", ""))
+            if item.note:
+                data.append(("", Paragraph(f"- <b>{item.note}</b>"), "", ""))
 
-            productcount += bp.quantity
+            productcount += item.quantity
 
         # Total
 
         data.append(
             (
                 pgettext("Text on generated order PDF", "Anzahl Produkte"),
                 "",
@@ -507,22 +505,22 @@
         c.drawString(12 * mm, 0 * mm, self.title)
 
         c.setFont("Helvetica", 10)
         if len(self.title) <= 23:
             c.drawString(
                 64 * mm,
                 0 * mm,
-                f"{order.date.year}-{order.pkfill(6)}"
+                f"{order.date.year}-{order.pkfill()}"
                 + (f" (Online #{order.woocommerceid})" if order.woocommerceid else ""),
             )
         else:
             c.drawString(
                 120 * mm,
                 0 * mm,
-                f"{order.date.year}-{order.pkfill(6)}"
+                f"{order.date.year}-{order.pkfill()}"
                 + (f" (Online #{order.woocommerceid})" if order.woocommerceid else ""),
             )
 
         c.restoreState()
 
     def draw(self):
         self.canv.translate(-12 * mm, -40 * mm)
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/order/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/order/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/pdfgeneration/swiss_qr_invoice.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/pdfgeneration/swiss_qr_invoice.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/settings/admin.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/settings/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     list_display = ("name", "content_display")
     ordering = ("id",)
 
     search_fields = []
 
     readonly_fields = ["id", "name", "description"]
 
-    hidden = True
+    HIDDEN = True
 
     def get_fields(self, request, obj=None):
         return ["description", f"content_{obj.typ}"]
 
     # Permissions
 
     NO_ADD = True
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/settings/constants.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/settings/constants.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/settings/forms.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/settings/forms.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/settings/models.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/settings/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 "Models for KMUHelper settings"
 
 from django import forms
-from django.db import models
 from django.contrib import admin
+from django.db import models
 from django.templatetags.static import static
 from django.utils.html import mark_safe, urlize
-from django.utils.translation import gettext_lazy, gettext
-
-from kmuhelper.overrides import CustomModel
+from django.utils.translation import gettext_lazy
 from kmuhelper.modules.settings.constants import SETTINGS
+from kmuhelper.overrides import CustomModel
 
 _ = gettext_lazy
 
 SETTINGTYPES = [
     ("char", _("Text")),
     ("text", _("Mehrzeiliger Text")),
     ("bool", _("Wahrheitswert")),
@@ -171,15 +170,15 @@
     class Meta:
         verbose_name = _("Einstellung")
         verbose_name_plural = _("Einstellungen")
         default_permissions = ("change",)
 
     objects = models.Manager()
 
-    admin_icon = "fas fa-cog"
+    ADMIN_ICON = "fa-solid fa-cog"
 
 
 class SettingHidden(SettingBase):
     """Model representing a hidden setting
 
     Hidden settings should only be edited through code and are not
     meant to be seen by the user.
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/settings/utils.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/settings/utils.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/settings/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/settings/views.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/modules/stats/views.py` & `django_kmuhelper-1.8.2/kmuhelper/modules/stats/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import datetime
 import json
 
-from django.contrib.auth.decorators import login_required, permission_required
+from django.contrib.auth.decorators import login_required
 from django.core.serializers.json import DjangoJSONEncoder
 from django.shortcuts import render
 from django.urls import reverse_lazy
 from django.utils import timezone
-from django.utils.translation import gettext_lazy, gettext
-
+from django.utils.translation import gettext_lazy
 from kmuhelper.decorators import require_all_kmuhelper_perms
-from kmuhelper.utils import render_error
-from kmuhelper.translations import langselect
 from kmuhelper.modules.main.models import OrderItem, Order
+from kmuhelper.translations import langselect
+from kmuhelper.utils import render_error
 
 _ = gettext_lazy
 
 #####
 
 
 @login_required(login_url=reverse_lazy("kmuhelper:login"))
@@ -117,21 +116,22 @@
     except (ValueError, IndexError):
         to_date = Order.objects.order_by("date").last().date
 
     products = {}
 
     for bp in (
         OrderItem.objects.filter(order__date__gte=from_date, order__date__lte=to_date)
-        .order_by("product__name")
-        .values("product__name", "quantity")
+        .order_by("linked_product__name")
+        .values("linked_product__name", "name", "quantity")
     ):
-        if bp["product__name"] in products:
-            products[langselect(bp["product__name"])] += bp["quantity"]
+        product_name = langselect(bp["linked_product__name"] or bp["name"])
+        if product_name in products:
+            products[product_name] += bp["quantity"]
         else:
-            products[langselect(bp["product__name"])] = bp["quantity"]
+            products[product_name] = bp["quantity"]
 
     products = sorted(products.items(), key=lambda x: x[1], reverse=True)
     products = products[:max_count] if len(products) > max_count else products
 
     context = {
         "has_permission": True,
         "product_names": [p[0] for p in products],
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/overrides.py` & `django_kmuhelper-1.8.2/kmuhelper/overrides.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,78 +3,93 @@
 from django.contrib import admin
 from django.db import models
 from django.forms.models import model_to_dict
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _, gettext
-
 from kmuhelper import widgets
 
 
 class CustomModel(models.Model):
     """django.db.models.Model with custom overrides"""
 
-    def pkfill(self, width=6):
+    PKFILL_WIDTH = 6
+
+    ADMIN_TITLE = None
+    ADMIN_DESCRIPTION = None
+    ADMIN_ICON = "fa-solid fa-circle-exclamation"
+
+    IS_APP_MODEL = False
+    NOTE_RELATION = None
+
+    DICT_FIELDS = []
+    DICT_EXCLUDE_FIELDS = []
+
+    @admin.display(description="ID", ordering="pk")
+    def pkfill(self, width=None):
         """Get the primary key of this object padded with zeros"""
 
-        return str(self.pk).zfill(width)
+        return str(self.pk).zfill(width or self.PKFILL_WIDTH)
 
     @property
     def to_dict(self):
         """Return the model fields as a dict"""
 
-        exclude = getattr(self.__class__, "DICT_EXCLUDE_FIELDS", list())
-        fields = getattr(self.__class__, "DICT_FIELDS", list())
+        exclude = self.DICT_EXCLUDE_FIELDS
+        fields = self.DICT_FIELDS
 
         if fields:
             return model_to_dict(self, fields=fields, exclude=exclude)
 
         return model_to_dict(self, exclude=exclude)
 
     @property
     def to_query_string(self):
         """Return the model fields as a query string"""
 
         return urlencode(self.to_dict)
 
     @admin.display(description=_("🔗 Notiz"), ordering="linked_note")
     def linked_note_html(self):
-        is_app = getattr(self.__class__, "IS_APP_MODEL", False)
-        relname = getattr(self.__class__, "NOTE_RELATION", None)
+        is_app = self.IS_APP_MODEL
+        rel_name = self.NOTE_RELATION
 
-        if relname is None:
+        if rel_name is None:
             return None
 
         if hasattr(self, "linked_note"):
             if is_app:
-                viewname = "admin:kmuhelper_app_todo_change"
+                view_name = "admin:kmuhelper_app_todo_change"
             else:
-                viewname = "admin:kmuhelper_note_change"
+                view_name = "admin:kmuhelper_note_change"
 
-            link = reverse(viewname, kwargs={"object_id": self.linked_note.pk})
-            text = gettext("Notiz ansehen")
+            link = reverse(view_name, kwargs={"object_id": self.linked_note.pk})
+            text = gettext("Notiz #%d") % self.linked_note.pk
         else:
             if is_app:
-                viewname = "admin:kmuhelper_app_todo_add"
+                view_name = "admin:kmuhelper_app_todo_add"
             else:
-                viewname = "admin:kmuhelper_note_add"
+                view_name = "admin:kmuhelper_note_add"
 
-            link = reverse(viewname) + f"?from_{relname}={self.pk}"
+            link = reverse(view_name) + f"?from_{rel_name}={self.pk}"
             text = gettext("Notiz erstellen")
         return format_html('<a target="_blank" href="{}">{}</a>', link, text)
 
     class Meta:
         abstract = True
 
 
 class CustomModelAdmin(admin.ModelAdmin):
     """django.contrib.admin.ModelAdmin with custom overrides"""
 
+    HIDDEN = False
+
     formfield_overrides = {models.JSONField: {"widget": widgets.PrettyJSONWidget}}
+    list_max_show_all = 1000
 
     def _get_obj_does_not_exist_redirect(self, request, opts, object_id):
         """Redirect to changelist page instead of admin home if object is not found"""
 
         super()._get_obj_does_not_exist_redirect(request, opts, object_id)
         info = self.model._meta.app_label, self.model._meta.model_name
         return redirect(reverse("admin:%s_%s_changelist" % info))
@@ -89,15 +104,15 @@
             if not is_connected():
                 del actions["wc_update"]
         return actions
 
     def has_module_permission(self, request):
         """Add option to hide model in default admin"""
 
-        if getattr(self.__class__, "hidden", False):
+        if self.HIDDEN:
             return {}
 
         return super().has_module_permission(request)
 
     # Readonly fields
 
     def get_readonly_fields(self, request, obj=None) -> tuple:
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/index-kmuhelper.css` & `django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/index-kmuhelper.css`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/pagechooser.css` & `django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/pagechooser.css`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/admin/kmuhelper/css/style.css` & `django_kmuhelper-1.8.2/kmuhelper/static/admin/kmuhelper/css/style.css`

 * *Files 25% similar despite different names*

```diff
@@ -59,17 +59,41 @@
 /* Margin fix for textarea */
 
 form .wide textarea + p.help,
 form .wide textarea + div.help {
     margin-left: 200px;
 }
 
+/* More styling */
+
+.field-display_customer {
+    white-space: nowrap;
+}
+
+/* ID styling */
+
+.field-pkfill {
+    font-family: "Courier New", monospace;
+    text-align: right;
+}
+
+/* Icon columns width fix for boolean columns */
+
+.column-pkfill,
+.column-display_woocommerce_state,
+.column-display_is_paid,
+.column-display_is_shipped {
+    width: 1px;
+}
+
 /* Price styling */
 
 .text-align-right,
+.field-display_current_price,
+.column-display_current_price,
 .field-display_cached_sum,
 .column-display_cached_sum,
 .field-display_subtotal,
 .column-display_subtotal {
     text-align: end;
 }
 
@@ -79,29 +103,37 @@
     margin-bottom: 2px;
 }
 
 /* Additional app index style */
 
 #pageinfo {
     padding-bottom: 10px;
+    line-height: 1.75;
 }
 
 #pageinfo a {
     border-radius: 5px;
     color: white !important;
     background-color: var(--kmuhelper-dark);
     transition-duration: 0.5s;
     text-decoration: none !important;
-    padding: 2px 6px;
+    padding: 0 0.3em;
+    margin: 0.1em 0.2em;
+    white-space: nowrap;
+    display: inline-block;
 }
 
 #pageinfo a:hover {
     background-color: var(--kmuhelper-darkest);
 }
 
+#pageinfo a i {
+    margin-right: 0.2em;
+}
+
 /* Fix overlapping object-tools buttons */
 
 @media (min-width: 768px) {
     .change-form #content-main {
         margin-top: 50px;
     }
 
@@ -115,14 +147,17 @@
 }
 
 /* Dropdowns in object tools */
 
 .object-tools {
     overflow-inline: visible !important;
     display: inline-block;
+
+    /* Object tools overflow */
+    overflow-y: visible !important;
 }
 
 .object-tools .dropdown {
     position: relative;
     display: inline-block;
 }
 
@@ -167,32 +202,19 @@
     border-radius: 0 0 10px 10px;
 }
 
 .object-tools .dropdown div a.disabled {
     color: grey;
 }
 
-.object-tools .dropdown div a.disabled:hover {
-    background-color: none !important;
-}
-
 .object-tools .dropdown div hr {
     color: lightgray;
     background-color: lightgray;
 }
 
-/*
-.object-tools .dropdown > a {
-    padding: 3px 18px 3px 12px;
-    background-image: url(../../img/selector-icons.svg);
-    background-repeat: no-repeat;
-    background-position-x: right;
-    background-position-y: -160px;
-} */
-
 .dropdown > a::after, .dropdown > div > b:first-child::after {
     content: "▼";
     padding-left: 0.5em;
 }
 
 /* Additional buttons in submit row */
 
@@ -208,12 +230,7 @@
 
     -webkit-user-select: none;
     -moz-user-select: none;
     -ms-user-select: none;
     user-select: none;
 }
 
-/* Object tools overflow */
-
-.object-tools {
-    overflow-y: visible !important;
-}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/css/details.css` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/css/details.css`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 }
 
 details > summary {
     padding: 8px;
     border-radius: 5px;
     position: sticky;
     background-color: var(--body-bg);
+
+    --details-level: 0;
+
+    /* Make all summaries sticky */
+    top: calc(var(--details-level) * 32px);
+    z-index: calc(100 - var(--details-level));
 }
 
 details[open] > summary {
     border-bottom: 1px solid gray;
     border-radius: 5px 5px 0 0;
 }
 
@@ -27,21 +33,15 @@
     margin-bottom: 10px;
 }
 
 details > div > *:last-child {
     margin-bottom: 0;
 }
 
-/* Stick to top for embedded details */
-
-details > summary {
-    --details-level: 0;
-    top: calc(var(--details-level) * 32px);
-    z-index: calc(100 - var(--details-level));
-}
+/* Detail levels */
 
 details details > summary {
     --details-level: 1;
 }
 
 details details details > summary {
     --details-level: 2;
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/favicon.ico` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-128x128.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-128x128.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-144x144.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-144x144.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-152x152.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-152x152.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-192x192.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-192x192.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-384x384.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-384x384.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-512x512.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-72x72.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-72x72.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/static/kmuhelper/images/icons/icon-96x96.png` & `django_kmuhelper-1.8.2/kmuhelper/static/kmuhelper/images/icons/icon-96x96.png`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/index.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/change_list.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-{% extends "admin/index.html" %}
-{% load static %}
+{% extends 'admin/kmuhelper/change_list.html' %}
 
-{% block extrastyle %}
-    {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static "admin/kmuhelper/css/index-kmuhelper.css" %}">
-    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.0.0/css/all.css"
-          integrity="sha384-3B6NwesSXE7YJlcLI9RpRqGf2p/EgVH8BgoKTaUrmKNDkHPStTQ3EyoYjCGXaOTS" crossorigin="anonymous"/>
-{% endblock %}
+{% load kmuhelper_tags %}
 
-{% block content %}
+{% block pageinfo %}
+    <p id="pageinfo">
+        <b>Verwandte Seiten:</b>
+        <a href="{% url 'admin:kmuhelper_app_stock_changelist' %}">
+            <abbr title="App"><i class="fa-solid fa-desktop"></i></abbr> Zahlungseingang
+        </a>
+        <a href="{% docs_url 'integrations/paymentimport' %}" target="_blank">
+            <abbr title="Dokumentation"><i class="fa-solid fa-book"></i></abbr> Zahlungsimport
+        </a>
+    </p>
+{% endblock %}
 
-    {% if not app_label %}
-        {% if perms.kmuhelper %}
-            <div style="margin-bottom: 32px;">
-                <a href="{% url 'kmuhelper:home' %}" id="kmuhelperbutton">
-                    <i class="fa-fw fas fa-box-open"></i>
-                    <h2>KMUHelper öffnen</h2>
-                </a>
-            </div>
-        {% endif %}
+{% block object-tools-items %}
+    {% if perms.kmuhelper.add_paymentimport %}
+        <li><a href="{% url 'admin:kmuhelper_paymentimport_upload' %}">XML Datei hochladen</a></li>
     {% endif %}
-
     {{ block.super }}
-{% endblock %}
+{% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
-{% extends "admin/index.html" %} {% load static %} {% block extrastyle %} {
-{ block.super }}
-}">
-{% endblock %} {% block content %} {% if not app_label %} {% if perms.kmuhelper
-%}
-_**_**_**_**_**_ _KK_MM_UU_HH_ee_ll_pp_ee_rr_ _?Ã_?¶_ff_ff_nn_ee_nn_ _**_**_**_**_**
-{% endif %} {% endif %} {{ block.super }} {% endblock %}
+{% extends 'admin/kmuhelper/change_list.html' %} {% load kmuhelper_tags %} {%
+block pageinfo %}
+VVeerrwwaannddttee SSeeiitteenn::
+_Z_a_h_l_u_n_g_s_e_i_n_g_a_n_g
+_Z_a_h_l_u_n_g_s_i_m_p_o_r_t
+{% endblock %} {% block object-tools-items %} {% if
+perms.kmuhelper.add_paymentimport %}
+_X_M_L_ _D_a_t_e_i_ _h_o_c_h_l_a_d_e_n
+{% endif %} {{ block.super }} {% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/_confirm.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/_confirm.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_incomingpayments/change_list.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_shipping/change_list.html`

 * *Files 16% similar despite different names*

```diff
@@ -7,12 +7,15 @@
 
     {% comment %} Load the changelist save on top script {% endcomment %}
     <script src="{% static 'admin/kmuhelper/js/changelist_saveontop.js' %}"></script>
 {% endblock %}
 
 {% block pageinfo %}
     <p id="pageinfo">
-        <b>Verwandte Seiten:</b> <a href="{% url 'admin:kmuhelper_order_changelist' %}">Admin: Bestellungen</a>
+        <b>Verwandte Seiten:</b>
+        <a href="{% url 'admin:kmuhelper_order_changelist' %}">
+            <abbr title="Admin"><i class="fa-solid fa-key"></i></abbr> Alle Bestellungen
+        </a>
     </p>
 {% endblock %}
 
 {% block unpaid_orders %}{% endblock %}
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 {% extends 'admin/kmuhelper/order/change_list.html' %} {% load static %} {%
 block extrahead %} {{ block.super }} {% comment %} Load the changelist save on
 top script {% endcomment %}
 {% endblock %} {% block pageinfo %}
-VVeerrwwaannddttee SSeeiitteenn:: _A_d_m_i_n_:_ _B_e_s_t_e_l_l_u_n_g_e_n
+VVeerrwwaannddttee SSeeiitteenn::
+_A_l_l_e_ _B_e_s_t_e_l_l_u_n_g_e_n
 {% endblock %} {% block unpaid_orders %}{% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/app_index.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/app_index.html`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
 {% block branding %}
     {% kmuhelper_branding %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/style.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/pagechooser.css' %}">
-    <link rel="stylesheet" type="text/css" href="https://use.fontawesome.com/releases/v6.0.0/css/all.css">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/pagechooser.css' %}">
+    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.5.2/css/all.css"
+          integrity="sha384-PPIZEGYM1v8zp5Py7UjFb79S58UeqCL9pYVnVPURKEqvioPROaVAJKKLzvH2rDnI" crossorigin="anonymous">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     {% include "kmuhelper/_includes/pwa_head.html" %}
 {% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/attachment/change_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/attachment/change_form.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/change_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/change_form.html`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,31 @@
     {% get_admin_module as module %}
     {% get_admin_model as model %}
 
     <div class="breadcrumbs">
         <a href="{% url module.viewname %}">KMUHelper {{ module.title }}</a>
         &rsaquo; {% if has_view_permission %}
         <a href="{% url opts|admin_urlname:'changelist' %}">
-            {{ model.admin_title | default:opts.verbose_name_plural }}</a>{% else %}
-        {{ model.admin_title | default:opts.verbose_name_plural }}{% endif %}
+            {{ model.ADMIN_TITLE | default:opts.verbose_name_plural }}</a>{% else %}
+        {{ model.ADMIN_TITLE | default:opts.verbose_name_plural }}{% endif %}
         &rsaquo;
         {% if add %}{% blocktranslate with name=opts.verbose_name %}Add {{ name }}{% endblocktranslate %}{% else %}
             {{ original|truncatewords:"18" }}{% endif %}
     </div>
 {% endblock %}
 
 {% block branding %}
     {% kmuhelper_branding %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.5.2/css/all.css"
+          integrity="sha384-PPIZEGYM1v8zp5Py7UjFb79S58UeqCL9pYVnVPURKEqvioPROaVAJKKLzvH2rDnI" crossorigin="anonymous">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     {% include "kmuhelper/_includes/pwa_head.html" %}
 
     {% comment %} Load the 'collapse-opem' schript {% endcomment %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% extends "admin/change_form.html" %} {% load i18n admin_urls static
 kmuhelper_tags %} {% block title %}{{ title }} | KMUHelper{% endblock %} {%
 block breadcrumbs %} {% get_admin_module as module %} {% get_admin_model as
 model %}
 _K_M_U_H_e_l_p_e_r_ _{_{_ _m_o_d_u_l_e_._t_i_t_l_e_ _}_} › {% if has_view_permission %} _{
-_{_ _m_o_d_e_l_._a_d_m_i_n___t_i_t_l_e_ _|_ _d_e_f_a_u_l_t_:_o_p_t_s_._v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_ _}_}{% else %} {
-{ model.admin_title | default:opts.verbose_name_plural }}{% endif %} › {% if
+_{_ _m_o_d_e_l_._A_D_M_I_N___T_I_T_L_E_ _|_ _d_e_f_a_u_l_t_:_o_p_t_s_._v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_ _}_}{% else %} {
+{ model.ADMIN_TITLE | default:opts.verbose_name_plural }}{% endif %} › {% if
 add %}{% blocktranslate with name=opts.verbose_name %}Add {{ name }}{%
 endblocktranslate %}{% else %} {{ original|truncatewords:"18" }}{% endif %}
 {% endblock %} {% block branding %} {% kmuhelper_branding %} {% endblock %} {%
 block extrastyle %} {{ block.super }}
 {% endblock %} {% block extrahead %} {{ block.super }} {% include "kmuhelper/
 _includes/pwa_head.html" %} {% comment %} Load the 'collapse-opem' schript {%
 endcomment %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/change_list.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/change_list.html`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 {% block breadcrumbs %}
     {% get_admin_module as module %}
     {% get_admin_model as model %}
 
     <div class="breadcrumbs">
         <a href="{% url module.viewname %}">KMUHelper {{ module.title }}</a>
-        &rsaquo; {{ model.admin_title | default:cl.opts.verbose_name_plural }}
+        &rsaquo; {{ model.ADMIN_TITLE | default:cl.opts.verbose_name_plural }}
     </div>
 {% endblock %}
 
 {% block branding %}
     {% kmuhelper_branding %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.5.2/css/all.css"
+          integrity="sha384-PPIZEGYM1v8zp5Py7UjFb79S58UeqCL9pYVnVPURKEqvioPROaVAJKKLzvH2rDnI" crossorigin="anonymous">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     {% include "kmuhelper/_includes/pwa_head.html" %}
 
     {% comment %} Add a custom blur function (for documentation screenshots) {% endcomment %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "admin/change_list.html" %} {% load admin_urls static kmuhelper_tags
 %} {% block title %}{{ title }} | KMUHelper{% endblock %} {% block breadcrumbs
 %} {% get_admin_module as module %} {% get_admin_model as model %}
-_K_M_U_H_e_l_p_e_r_ _{_{_ _m_o_d_u_l_e_._t_i_t_l_e_ _}_} › {{ model.admin_title | default:
+_K_M_U_H_e_l_p_e_r_ _{_{_ _m_o_d_u_l_e_._t_i_t_l_e_ _}_} › {{ model.ADMIN_TITLE | default:
 cl.opts.verbose_name_plural }}
 {% endblock %} {% block branding %} {% kmuhelper_branding %} {% endblock %} {%
 block extrastyle %} {{ block.super }}
 {% endblock %} {% block extrahead %} {{ block.super }} {% include "kmuhelper/
 _includes/pwa_head.html" %} {% comment %} Add a custom blur function (for
 documentation screenshots) {% endcomment %}
 {% comment %} Load the beforeunload script {% endcomment %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/customer/change_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/customer/change_form.html`

 * *Files 6% similar despite different names*

```diff
@@ -54,29 +54,30 @@
 {% endblock %}
 
 {% block after_field_sets %}
     {% if has_change_permission %}
         <div id="auto-copy-form-row" class="form-row">
             <div>
                 <div class="flex-container checkbox-row">
-                    <input type="checkbox" id="auto-copy"><label class="vCheckboxLabel" for="auto-copy">Von
-                    Rechnungsadresse übernehmen?</label>
+                    <input type="checkbox" id="auto-copy"
+                           {% if original.addresses_are_equal %}checked="checked"{% endif %}>
+                    <label class="vCheckboxLabel" for="auto-copy">Von Rechnungsadresse übernehmen?</label>
                 </div>
             </div>
         </div>
         <script>
             ADDR_FIELDS = ['first_name', 'last_name', 'company', 'address_1', 'address_2', 'postcode', 'city', 'state', 'country', 'email', 'phone'];
 
             $ = django.jQuery;
 
             function copyFormIfCheck() {
                 if ($("#auto-copy").prop("checked")) {
                     for (let field of ADDR_FIELDS) {
-                        $("#id_addr_shipping_" + field).val(
-                            $("#id_addr_billing_" + field).val()
+                        $(`#id_addr_shipping_${field}`).val(
+                            $(`#id_addr_billing_${field}`).val()
                         )
                     }
                 }
             }
 
             function updateShippingFormVisibility() {
                 if ($("#auto-copy").prop("checked")) {
@@ -84,14 +85,15 @@
                     copyFormIfCheck();
                 } else {
                     $(".addr-shipping-fieldset .form-row:not(#auto-copy-form-row)").show();
                 }
             }
 
             document.addEventListener("DOMContentLoaded", () => {
+                updateShippingFormVisibility();
                 $(".addr-shipping-fieldset h2").after(
                     document.getElementById("auto-copy-form-row")
                 )
 
                 $(".addr-billing-fieldset").on("input", copyFormIfCheck);
                 $("#auto-copy").on("input", updateShippingFormVisibility);
             });
```

#### html2text {}

```diff
@@ -17,9 +17,10 @@
       perms.kmuhelper.view_email %} _R_e_g_i_s_t_r_i_e_r_u_n_g_s_e_m_a_i_l_ _a_n_s_e_h_e_n {% endif %} {%
       if perms.kmuhelper.add_email and perms.kmuhelper.change_customer %}
       _R_e_g_i_s_t_r_i_e_r_u_n_g_s_e_m_a_i_l_ _g_e_n_e_r_i_e_r_e_n {% endif %} {% else %} Registrierungsemail
       {% endif %}
     * {% endif %} {% endif %} {{ block.super }} {% endblock %} {% endif %}{%
       endif %}
 {% endblock %} {% block after_field_sets %} {% if has_change_permission %}
-??Von Rechnungsadresse Ã¼bernehmen?
+% if original.addresses_are_equal %}checked="checked"{% endif %}> Von
+Rechnungsadresse Ã¼bernehmen?
 {% endif %} {% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/delete_confirmation.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/delete_confirmation.html`

 * *Files 22% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 {% block breadcrumbs %}
     {% get_admin_module as module %}
     {% get_admin_model as model %}
 
     <div class="breadcrumbs">
         <a href="{% url module.viewname %}">KMUHelper {{ module.title }}</a>
         &rsaquo; <a href="{% url opts|admin_urlname:'changelist' %}">
-        {{ model.admin_title | default:opts.verbose_name_plural }}</a>
+        {{ model.ADMIN_TITLE | default:opts.verbose_name_plural }}</a>
         &rsaquo; <a href="{% url opts|admin_urlname:'change' object.pk|admin_urlquote %}">
         {{ object|truncatewords:"18" }}</a>
         &rsaquo; {% translate 'Delete' %}
     </div>
 {% endblock %}
 
 {% block branding %}
     {% kmuhelper_branding %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.5.2/css/all.css"
+          integrity="sha384-PPIZEGYM1v8zp5Py7UjFb79S58UeqCL9pYVnVPURKEqvioPROaVAJKKLzvH2rDnI" crossorigin="anonymous">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     {% include "kmuhelper/_includes/pwa_head.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "admin/delete_confirmation.html" %} {% load i18n admin_urls static
 kmuhelper_tags %} {% block title %}{{ title }} | KMUHelper{% endblock %} {%
 block breadcrumbs %} {% get_admin_module as module %} {% get_admin_model as
 model %}
-_K_M_U_H_e_l_p_e_r_ _{_{_ _m_o_d_u_l_e_._t_i_t_l_e_ _}_} › _{_{_ _m_o_d_e_l_._a_d_m_i_n___t_i_t_l_e_ _|_ _d_e_f_a_u_l_t_:
+_K_M_U_H_e_l_p_e_r_ _{_{_ _m_o_d_u_l_e_._t_i_t_l_e_ _}_} › _{_{_ _m_o_d_e_l_._A_D_M_I_N___T_I_T_L_E_ _|_ _d_e_f_a_u_l_t_:
 _o_p_t_s_._v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_ _}_} › _{_{_ _o_b_j_e_c_t_|_t_r_u_n_c_a_t_e_w_o_r_d_s_:_"_1_8_"_ _}_} › {% translate
 'Delete' %}
 {% endblock %} {% block branding %} {% kmuhelper_branding %} {% endblock %} {%
 block extrastyle %} {{ block.super }}
 {% endblock %} {% block extrahead %} {{ block.super }} {% include "kmuhelper/
 _includes/pwa_head.html" %} {% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/delete_selected_confirmation.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/base_site.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,42 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6164 6d69  {% extends "admi
-00000010: 6e2f 6465 6c65 7465 5f73 656c 6563 7465  n/delete_selecte
-00000020: 645f 636f 6e66 6972 6d61 7469 6f6e 2e68  d_confirmation.h
-00000030: 746d 6c22 2025 7d0a 7b25 206c 6f61 6420  tml" %}.{% load 
-00000040: 6931 386e 2061 646d 696e 5f75 726c 7320  i18n admin_urls 
-00000050: 7374 6174 6963 206b 6d75 6865 6c70 6572  static kmuhelper
-00000060: 5f74 6167 7320 257d 0a0a 7b25 2062 6c6f  _tags %}..{% blo
-00000070: 636b 2074 6974 6c65 2025 7d7b 7b20 7469  ck title %}{{ ti
-00000080: 746c 6520 7d7d 207c 204b 4d55 4865 6c70  tle }} | KMUHelp
-00000090: 6572 7b25 2065 6e64 626c 6f63 6b20 257d  er{% endblock %}
-000000a0: 0a0a 7b25 2062 6c6f 636b 2062 7265 6164  ..{% block bread
-000000b0: 6372 756d 6273 2025 7d0a 2020 2020 7b25  crumbs %}.    {%
-000000c0: 2067 6574 5f61 646d 696e 5f6d 6f64 756c   get_admin_modul
-000000d0: 6520 6173 206d 6f64 756c 6520 257d 0a20  e as module %}. 
-000000e0: 2020 207b 2520 6765 745f 6164 6d69 6e5f     {% get_admin_
-000000f0: 6d6f 6465 6c20 6173 206d 6f64 656c 2025  model as model %
-00000100: 7d0a 0a20 2020 203c 6469 7620 636c 6173  }..    <div clas
-00000110: 733d 2262 7265 6164 6372 756d 6273 223e  s="breadcrumbs">
-00000120: 0a20 2020 2020 2020 203c 6120 6872 6566  .        <a href
-00000130: 3d22 7b25 2075 726c 206d 6f64 756c 652e  ="{% url module.
-00000140: 7669 6577 6e61 6d65 2025 7d22 3e4b 4d55  viewname %}">KMU
-00000150: 4865 6c70 6572 207b 7b20 6d6f 6475 6c65  Helper {{ module
-00000160: 2e74 6974 6c65 207d 7d3c 2f61 3e0a 2020  .title }}</a>.  
-00000170: 2020 2020 2020 2672 7361 7175 6f3b 203c        &rsaquo; <
-00000180: 6120 6872 6566 3d22 7b25 2075 726c 206f  a href="{% url o
-00000190: 7074 737c 6164 6d69 6e5f 7572 6c6e 616d  pts|admin_urlnam
-000001a0: 653a 2763 6861 6e67 656c 6973 7427 2025  e:'changelist' %
-000001b0: 7d22 3e0a 2020 2020 2020 2020 7b7b 206d  }">.        {{ m
-000001c0: 6f64 656c 2e61 646d 696e 5f74 6974 6c65  odel.admin_title
-000001d0: 207c 2064 6566 6175 6c74 3a6f 7074 732e   | default:opts.
-000001e0: 7665 7262 6f73 655f 6e61 6d65 5f70 6c75  verbose_name_plu
-000001f0: 7261 6c20 7d7d 3c2f 613e 0a20 2020 2020  ral }}</a>.     
-00000200: 2020 2026 7273 6171 756f 3b20 7b25 2074     &rsaquo; {% t
-00000210: 7261 6e73 6c61 7465 2027 4465 6c65 7465  ranslate 'Delete
-00000220: 206d 756c 7469 706c 6520 6f62 6a65 6374   multiple object
-00000230: 7327 2025 7d0a 2020 2020 3c2f 6469 763e  s' %}.    </div>
-00000240: 0a7b 2520 656e 6462 6c6f 636b 2025 7d0a  .{% endblock %}.
-00000250: 0a7b 2520 626c 6f63 6b20 6272 616e 6469  .{% block brandi
-00000260: 6e67 2025 7d0a 2020 2020 7b25 206b 6d75  ng %}.    {% kmu
-00000270: 6865 6c70 6572 5f62 7261 6e64 696e 6720  helper_branding 
-00000280: 257d 0a7b 2520 656e 6462 6c6f 636b 2025  %}.{% endblock %
-00000290: 7d0a 0a7b 2520 626c 6f63 6b20 6578 7472  }..{% block extr
-000002a0: 6173 7479 6c65 2025 7d0a 2020 2020 7b7b  astyle %}.    {{
-000002b0: 2062 6c6f 636b 2e73 7570 6572 207d 7d0a   block.super }}.
-000002c0: 2020 2020 3c6c 696e 6b20 7265 6c3d 2273      <link rel="s
-000002d0: 7479 6c65 7368 6565 7422 2074 7970 653d  tylesheet" type=
-000002e0: 2274 6578 742f 6373 7322 2068 7265 663d  "text/css" href=
-000002f0: 227b 2520 7374 6174 6963 2027 6164 6d69  "{% static 'admi
-00000300: 6e2f 6b6d 7568 656c 7065 722f 6373 732f  n/kmuhelper/css/
-00000310: 7374 796c 652e 6373 7327 2025 7d22 3e0a  style.css' %}">.
-00000320: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
-00000330: 7b25 2062 6c6f 636b 2065 7874 7261 6865  {% block extrahe
-00000340: 6164 2025 7d0a 2020 2020 7b7b 2062 6c6f  ad %}.    {{ blo
-00000350: 636b 2e73 7570 6572 207d 7d0a 2020 2020  ck.super }}.    
-00000360: 7b25 2069 6e63 6c75 6465 2022 6b6d 7568  {% include "kmuh
-00000370: 656c 7065 722f 5f69 6e63 6c75 6465 732f  elper/_includes/
-00000380: 7077 615f 6865 6164 2e68 746d 6c22 2025  pwa_head.html" %
-00000390: 7d0a 7b25 2065 6e64 626c 6f63 6b20 257d  }.{% endblock %}
-000003a0: 0a                                       .
+00000010: 6e2f 6261 7365 5f73 6974 652e 6874 6d6c  n/base_site.html
+00000020: 2220 257d 0a0a 7b25 206c 6f61 6420 7374  " %}..{% load st
+00000030: 6174 6963 206b 6d75 6865 6c70 6572 5f74  atic kmuhelper_t
+00000040: 6167 7320 257d 0a0a 7b25 2062 6c6f 636b  ags %}..{% block
+00000050: 2074 6974 6c65 2025 7d7b 7b20 7469 746c   title %}{{ titl
+00000060: 6520 7d7d 207c 204b 4d55 4865 6c70 6572  e }} | KMUHelper
+00000070: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+00000080: 7b25 2062 6c6f 636b 2062 7261 6e64 696e  {% block brandin
+00000090: 6720 257d 0a20 2020 207b 2520 6b6d 7568  g %}.    {% kmuh
+000000a0: 656c 7065 725f 6272 616e 6469 6e67 2025  elper_branding %
+000000b0: 7d0a 7b25 2065 6e64 626c 6f63 6b20 257d  }.{% endblock %}
+000000c0: 0a0a 7b25 2062 6c6f 636b 2065 7874 7261  ..{% block extra
+000000d0: 7374 796c 6520 257d 0a20 2020 207b 7b20  style %}.    {{ 
+000000e0: 626c 6f63 6b2e 7375 7065 7220 7d7d 0a20  block.super }}. 
+000000f0: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
+00000100: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
+00000110: 7b25 2073 7461 7469 6320 2761 646d 696e  {% static 'admin
+00000120: 2f6b 6d75 6865 6c70 6572 2f63 7373 2f73  /kmuhelper/css/s
+00000130: 7479 6c65 2e63 7373 2720 257d 223e 0a20  tyle.css' %}">. 
+00000140: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
+00000150: 796c 6573 6865 6574 2220 6872 6566 3d22  ylesheet" href="
+00000160: 6874 7470 733a 2f2f 7573 652e 666f 6e74  https://use.font
+00000170: 6177 6573 6f6d 652e 636f 6d2f 7265 6c65  awesome.com/rele
+00000180: 6173 6573 2f76 362e 352e 322f 6373 732f  ases/v6.5.2/css/
+00000190: 616c 6c2e 6373 7322 0a20 2020 2020 2020  all.css".       
+000001a0: 2020 2069 6e74 6567 7269 7479 3d22 7368     integrity="sh
+000001b0: 6133 3834 2d50 5049 5a45 4759 4d31 7638  a384-PPIZEGYM1v8
+000001c0: 7a70 3550 7937 556a 4662 3739 5335 3855  zp5Py7UjFb79S58U
+000001d0: 6571 434c 3970 5956 6e56 5055 524b 4571  eqCL9pYVnVPURKEq
+000001e0: 7669 6f50 524f 6156 414a 4b4b 4c7a 7648  vioPROaVAJKKLzvH
+000001f0: 3272 446e 4922 2063 726f 7373 6f72 6967  2rDnI" crossorig
+00000200: 696e 3d22 616e 6f6e 796d 6f75 7322 3e0a  in="anonymous">.
+00000210: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+00000220: 7b25 2062 6c6f 636b 2065 7874 7261 6865  {% block extrahe
+00000230: 6164 2025 7d0a 2020 2020 7b7b 2062 6c6f  ad %}.    {{ blo
+00000240: 636b 2e73 7570 6572 207d 7d0a 2020 2020  ck.super }}.    
+00000250: 7b25 2069 6e63 6c75 6465 2022 6b6d 7568  {% include "kmuh
+00000260: 656c 7065 722f 5f69 6e63 6c75 6465 732f  elper/_includes/
+00000270: 7077 615f 6865 6164 2e68 746d 6c22 2025  pwa_head.html" %
+00000280: 7d0a 7b25 2065 6e64 626c 6f63 6b20 257d  }.{% endblock %}
+00000290: 0a                                       .
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/email/change_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/email/change_form.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_form.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_list.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/emailtemplate/change_list.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/order/pdf_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/order/pdf_form.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_entry.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_entry.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order_payment.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_order_payment.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_payment.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/includes/process_table_payment.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/process.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/process.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/paymentimport/upload.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/paymentimport/upload.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/product/change_form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/product/change_form.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/admin/kmuhelper/product/change_list.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/admin/kmuhelper/productcategory/change_list.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 {% extends 'admin/kmuhelper/change_list.html' %}
 
 {% block pageinfo %}
     <p id="pageinfo">
-        <b>Verwandte Seiten:</b> <a href="{% url 'admin:kmuhelper_app_stock_changelist' %}">App: Lagerbestand</a>,
-        <a href="{% url 'admin:kmuhelper_productcategory_changelist' %}">Admin: Produktkategorien</a>
+        <b>Verwandte Seiten:</b>
+        <a href="{% url 'admin:kmuhelper_product_changelist' %}">
+            <abbr title="Admin"><i class="fa-solid fa-key"></i></abbr> Produkte
+        </a>
     </p>
 {% endblock %}
 
 {% block object-tools-items %}
     {% load kmuhelper_tags %}
     {% kmuhelper_woocommerce_connected as woocommerce_is_connected %}
-    {% if woocommerce_is_connected and perms.kmuhelper.add_product %}
+    {% if woocommerce_is_connected and perms.kmuhelper.add_productcategory %}
         <li>
-            <a onclick="woocommerce_loading_swal();" href="{% url 'kmuhelper:wc-import-products' %}" class="addlink">Produkte von
+            <a onclick="woocommerce_loading_swal();" href="{% url 'kmuhelper:wc-import-categories' %}" class="addlink">Kategorien von
                 WooCommerce importieren</a>
         </li>
     {% endif %}
     {{ block.super }}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends 'admin/kmuhelper/change_list.html' %} {% block pageinfo %}
-VVeerrwwaannddttee SSeeiitteenn:: _A_p_p_:_ _L_a_g_e_r_b_e_s_t_a_n_d, _A_d_m_i_n_:_ _P_r_o_d_u_k_t_k_a_t_e_g_o_r_i_e_n
+VVeerrwwaannddttee SSeeiitteenn::
+_P_r_o_d_u_k_t_e
 {% endblock %} {% block object-tools-items %} {% load kmuhelper_tags %} {%
 kmuhelper_woocommerce_connected as woocommerce_is_connected %} {% if
-woocommerce_is_connected and perms.kmuhelper.add_product %}
-_P_r_o_d_u_k_t_e_ _v_o_n_ _W_o_o_C_o_m_m_e_r_c_e_ _i_m_p_o_r_t_i_e_r_e_n
+woocommerce_is_connected and perms.kmuhelper.add_productcategory %}
+_K_a_t_e_g_o_r_i_e_n_ _v_o_n_ _W_o_o_C_o_m_m_e_r_c_e_ _i_m_p_o_r_t_i_e_r_e_n
 {% endif %} {{ block.super }} {% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/form.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/form_field.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/form_field.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/_includes/pagechooser.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/_includes/pagechooser.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/base.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/base.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/customer_registered.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/customer_registered.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/order_invoice.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/order_invoice.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/order_stock_warning.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/order_stock_warning.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/emails/order_supply.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/emails/order_supply.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/error.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/error.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/home.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/home.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <h1 id="site-name"><a target="_top" href="{% url 'kmuhelper:home' %}">KMUHelper</a></h1>
 {% endblock %}
 
 {% block breadcrumbs %}{% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/pagechooser.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/pagechooser.css' %}">
     <link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.0.0/css/all.css"
           integrity="sha384-3B6NwesSXE7YJlcLI9RpRqGf2p/EgVH8BgoKTaUrmKNDkHPStTQ3EyoYjCGXaOTS" crossorigin="anonymous"/>
 
 {% endblock %}
 
 {% block content %}
     <h1>Willkommen im KMUHelper!</h1>
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/integrations/woocommerce/settings.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/integrations/woocommerce/settings.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 {% block branding %}
     {% kmuhelper_branding module_name='settings' %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/css/forms.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/style.css' %}">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     <script src="{% static 'admin/kmuhelper/js/beforeunload.js' %}" type="text/javascript"></script>
     <script src="{% static 'admin/js/vendor/jquery/jquery.js' %}" type="text/javascript"></script>
 {% endblock %}
@@ -30,22 +30,31 @@
 {% block content %}
     {% include 'kmuhelper/_includes/form.html' with submit_text="Einstellungen speichern" %}
 
     <hr style="margin-top: 2em; margin-bottom: 2em;">
     <h2>Einrichtung</h2>
 
     <div style="margin-top: 2em;">
+        <h3>Schritt 0: Einstellungen festlegen</h3>
+        <p>
+            Als erstes müssen Sie ein paar Einstellungen vornehmen. Tragen Sie dazu oben die URL Ihrer WooCommerce
+            Installation ein (z. B. https://shop.example.com).
+            Geben sie ausserdem eine zufällig generierte Zeichenkette als Secret an, z. B.
+            <code>{{ random_secret }}</code> (Dieses Secret wird bei jedem Laden der Seite zufällig generiert.)
+            Klicken Sie anschliessend auf "Einstellungen speichern".
+        </p>
+
+        <hr>
+
         <h3>Schritt 1: WooCommerce verbinden</h3>
         <p>
             Um die WooCommerce Schnittstelle zu nutzen, muss diese zuerst mit dem KMUHelper verbunden werden.
             Dazu muss der KMUHelper <b>Lese-Zugriff</b> auf die WooCommerce API erhalten.
             Dieser Zugriff kann jederzeit widerrufen werden.
-            Tragen Sie dazu oben die URL Ihrer WooCommerce Installation ein und klicken Sie auf "Einstellungen
-            speichern".
-            Klicken Sie anschliessend auf folgenden Knopf und melden Sie sich mit Ihren WooCommerce/WordPress
+            Klicken Sie auf folgenden Knopf und melden Sie sich mit Ihren WooCommerce/WordPress
             Zugangsdaten an:
         </p>
         {% if is_url_valid %}
             {% if is_connected %}
                 <a href="{% url 'kmuhelper:wc-auth-start' %}">
                     <button class="button">API erneut verbinden</button>
                 </a>
@@ -86,32 +95,32 @@
             Damit Daten automatisch von WooCommerce an den KMUHelper übertragen werden können, müssen Webhooks
             eingerichtet werden.
             Dieser Schritt muss manuell durchgeführt werden.
             Öffnen Sie die WooCommerce Einstellungen via Knopf unten und folgen Sie folgenden Anweisungen:
         </p>
         <p>
             Erstellen Sie für die nachfolgende Themen je einen Webhook.
-            Wählen Sie jeweils den Status "Aktiviert" und die API-Version "v3".
-            Verwenden Sie überall dasselbe Secret wie oben, z. B. <code>{{ random_secret }}</code>
-            (Dieses Secret ist zufällig generiert und kann problemlos verwendet werden.
-            Nicht vergessen, es auch oben einzutragen und die Einstellungen zu speichern!)
-            und geben Sie als URL folgende Adresse an:
+            Wählen Sie jeweils den Status "Aktiviert" und die API-Version "WP REST-API Integration v3".
+            Verwenden Sie überall das Secret, welches sie oben gespeichert haben und verwenden Sie als
+            URL folgende Adresse:
             <code>https://{{ kmuhelper_url }}{% url 'kmuhelper:wc-webhooks' %}</code>
+        </p>
         <ul>
             <li>Bestellung erstellt (order.created)</li>
             <li>Bestellung aktualisiert (order.updated)</li>
             <li>Bestellung gelöscht (order.deleted)</li>
+            <li>Bestellung wiederhergestellt (order.restored)</li>
             <li>Kunde erstellt (customer.created)</li>
             <li>Kunde aktualisiert (customer.updated)</li>
             <li>Kunde gelöscht (customer.deleted)</li>
             <li>Produkt erstellt (product.created)</li>
             <li>Produkt aktualisiert (product.updated)</li>
             <li>Produkt entfernt (product.deleted)</li>
+            <li>Produkt wiederhergestellt (product.restored)</li>
         </ul>
-        </p>
         {% if is_connected %}
             <a href="{{ wc_url }}/wp-admin/admin.php?page=wc-settings&tab=advanced&section=webhooks" target="_blank"
                rel="noopener noreferrer">
                 <button class="button">Webhooks einrichten</button>
             </a>
         {% else %}
             <button class="button" disabled>Schritt 1 muss zuerst abgeschlossen werden</button>
```

#### html2text {}

```diff
@@ -6,21 +6,27 @@
 {% endblock %} {% block extrahead %} {{ block.super }}
 {% endblock %} {% block content_title %}
 ************ WWooooCCoommmmeerrccee--IInntteeggrraattiioonn ************
 {% endblock %} {% block content %} {% include 'kmuhelper/_includes/form.html'
 with submit_text="Einstellungen speichern" %}
 ===============================================================================
 ********** EEiinnrriicchhttuunngg **********
+******** SScchhrriitttt 00:: EEiinnsstteelllluunnggeenn ffeessttlleeggeenn ********
+Als erstes mÃ¼ssen Sie ein paar Einstellungen vornehmen. Tragen Sie dazu oben
+die URL Ihrer WooCommerce Installation ein (z. B. https://shop.example.com).
+Geben sie ausserdem eine zufÃ¤llig generierte Zeichenkette als Secret an, z. B.
+{{ random_secret }} (Dieses Secret wird bei jedem Laden der Seite zufÃ¤llig
+generiert.) Klicken Sie anschliessend auf "Einstellungen speichern".
+===============================================================================
 ******** SScchhrriitttt 11:: WWooooCCoommmmeerrccee vveerrbbiinnddeenn ********
 Um die WooCommerce Schnittstelle zu nutzen, muss diese zuerst mit dem KMUHelper
 verbunden werden. Dazu muss der KMUHelper LLeessee--ZZuuggrriiffff auf die WooCommerce API
-erhalten. Dieser Zugriff kann jederzeit widerrufen werden. Tragen Sie dazu oben
-die URL Ihrer WooCommerce Installation ein und klicken Sie auf "Einstellungen
-speichern". Klicken Sie anschliessend auf folgenden Knopf und melden Sie sich
-mit Ihren WooCommerce/WordPress Zugangsdaten an:
+erhalten. Dieser Zugriff kann jederzeit widerrufen werden. Klicken Sie auf
+folgenden Knopf und melden Sie sich mit Ihren WooCommerce/WordPress
+Zugangsdaten an:
 {% if is_url_valid %} {% if is_connected %} _A_P_I_ _e_r_n_e_u_t_ _v_e_r_b_i_n_d_e_n_ {% else %} _A_P_I
 _v_e_r_b_i_n_d_e_n_ {% endif %} {% else %} Die angegebene URL ist ungÃ¼ltig {% endif %}
 
 ******** SScchhrriitttt 22:: SSttaattuuss ?Ã?¼bbeerrpprr?Ã?¼ffeenn ((ooppttiioonnaall)) ********
 {% if is_connected %}
 Die WooCommerce-Schnittstelle wurde erfolgreich eingerichtet. Ãber folgenden
 Knopf kÃ¶nnen Sie Ã¼berprÃ¼fen, ob die Verbindung funktioniert:
@@ -31,29 +37,29 @@
 
 ******** SScchhrriitttt 33:: WWeebbhhooookkss eeiinnrriicchhtteenn ((ooppttiioonnaall,, aabbeerr eemmppffoohhlleenn)) ********
 Damit Daten automatisch von WooCommerce an den KMUHelper Ã¼bertragen werden
 kÃ¶nnen, mÃ¼ssen Webhooks eingerichtet werden. Dieser Schritt muss manuell
 durchgefÃ¼hrt werden. Ãffnen Sie die WooCommerce Einstellungen via Knopf unten
 und folgen Sie folgenden Anweisungen:
 Erstellen Sie fÃ¼r die nachfolgende Themen je einen Webhook. WÃ¤hlen Sie
-jeweils den Status "Aktiviert" und die API-Version "v3". Verwenden Sie Ã¼berall
-dasselbe Secret wie oben, z. B. {{ random_secret }} (Dieses Secret ist
-zufÃ¤llig generiert und kann problemlos verwendet werden. Nicht vergessen, es
-auch oben einzutragen und die Einstellungen zu speichern!) und geben Sie als
-URL folgende Adresse an: https://{{ kmuhelper_url }}{% url 'kmuhelper:wc-
-webhooks' %}
+jeweils den Status "Aktiviert" und die API-Version "WP REST-API Integration
+v3". Verwenden Sie Ã¼berall das Secret, welches sie oben gespeichert haben und
+verwenden Sie als URL folgende Adresse: https://{{ kmuhelper_url }}{% url
+'kmuhelper:wc-webhooks' %}
     * Bestellung erstellt (order.created)
     * Bestellung aktualisiert (order.updated)
     * Bestellung gelÃ¶scht (order.deleted)
+    * Bestellung wiederhergestellt (order.restored)
     * Kunde erstellt (customer.created)
     * Kunde aktualisiert (customer.updated)
     * Kunde gelÃ¶scht (customer.deleted)
     * Produkt erstellt (product.created)
     * Produkt aktualisiert (product.updated)
     * Produkt entfernt (product.deleted)
+    * Produkt wiederhergestellt (product.restored)
 {% if is_connected %} _W_e_b_h_o_o_k_s_ _e_i_n_r_i_c_h_t_e_n_ {% else %} Schritt 1 muss zuerst
 abgeschlossen werden {% endif %}
 
 ******** SScchhrriitttt 44:: SSttaattuuss ddeerr WWeebbhhooookkss ?Ã?¼bbeerrpprr?Ã?¼ffeenn ((ooppttiioonnaall)) ********
 Der Status der Webhooks kann nur manuell Ã¼berprÃ¼ft werden, indem Daten in
 WooCommerce verÃ¤ndert werden (z. B. eine Bestellung erstellen).
 ===============================================================================
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/manifest.json` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/manifest.json`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/settings/build_info.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/settings/build_info.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/settings/form.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/settings/form.html`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 {% block branding %}
     {% kmuhelper_branding module_name='settings' %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/kmuhelper/css/style.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/css/forms.css' %}">
+    <link rel="stylesheet" href="{% static 'admin/kmuhelper/css/style.css' %}">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     <script src="{% static 'admin/kmuhelper/js/beforeunload.js' %}" type="text/javascript"></script>
     <script src="{% static 'admin/js/vendor/jquery/jquery.js' %}" type="text/javascript"></script>
 {% endblock %}
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/base.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/base.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/best_products.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/best_products.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/index.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/index.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templates/kmuhelper/stats/products_price.html` & `django_kmuhelper-1.8.2/kmuhelper/templates/kmuhelper/stats/products_price.html`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/templatetags/kmuhelper_tags.py` & `django_kmuhelper-1.8.2/kmuhelper/templatetags/kmuhelper_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django import template
 from django.apps import apps
 from django.urls import reverse
 from django.utils.html import format_html
 
-from kmuhelper import settings
+from kmuhelper import settings, constants
 from kmuhelper.modules import config
 from kmuhelper.modules.integrations.woocommerce.utils import (
     is_connected as is_woocommerce_connected,
 )
 
 register = template.Library()
 
@@ -64,21 +64,26 @@
     for model in model_list:
         try:
             dbmodel = apps.get_model("kmuhelper", model["object_name"])
         except LookupError:
             dbmodel = None
         griddata.append(
             {
-                "title": getattr(dbmodel, "admin_title", "") or model["name"],
+                "title": getattr(dbmodel, "ADMIN_TITLE", "") or model["name"],
                 "url": model["admin_url"],
-                "subtitle": getattr(dbmodel, "admin_description", ""),
+                "subtitle": getattr(dbmodel, "ADMIN_DESCRIPTION", ""),
                 "icon": getattr(
-                    dbmodel, "admin_icon", "fa-solid fa-circle-exclamation"
+                    dbmodel, "ADMIN_ICON", "fa-solid fa-circle-exclamation"
                 ),
             }
         )
     return {"griddata": [griddata], "pagechooserclass": "smallboxes"}
 
 
 @register.inclusion_tag("kmuhelper/_includes/pagechooser.html", takes_context=False)
 def kmuhelper_pagechooser(griddata, pagechooserclass=""):
     return {"griddata": griddata, "pagechooserclass": pagechooserclass}
+
+
+@register.simple_tag(name="docs_url", takes_context=False)
+def docs_url(path=""):
+    return constants.URL_MANUAL + path
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/translations.py` & `django_kmuhelper-1.8.2/kmuhelper/translations.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/urls.py` & `django_kmuhelper-1.8.2/kmuhelper/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,21 @@
     path("manifest.json", views.manifest, name="manifest"),
     path("login", views.login, name="login"),
     # Developing tools
     path(
         "_templatetest/<path:templatename>", views._templatetest, name="_templatetest"
     ),
     # Main modules
-    path("main/", include("kmuhelper.modules.main")),
-    path("api/", include("kmuhelper.modules.api")),
-    path("app/", include("kmuhelper.modules.app")),
-    path("emails/", include("kmuhelper.modules.emails")),
-    path("stats/", include("kmuhelper.modules.stats")),
-    path("settings/", include("kmuhelper.modules.settings")),
-    # Deprecated urls
-    path("wc/", include("kmuhelper.modules.integrations.woocommerce")),
+    path("main/", include("kmuhelper.modules.main.urls")),
+    path("api/", include("kmuhelper.modules.api.urls")),
+    path("app/", include("kmuhelper.modules.app.urls")),
+    path("emails/", include("kmuhelper.modules.emails.urls")),
+    path("stats/", include("kmuhelper.modules.stats.urls")),
+    path("settings/", include("kmuhelper.modules.settings.urls")),
     # Integrations
     path(
         "integrations/woocommerce/",
-        include("kmuhelper.modules.integrations.woocommerce"),
+        include("kmuhelper.modules.integrations.woocommerce.urls"),
     ),
     # 404 Not found
     re_path("^.*$", views.error),
 ]
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/utils.py` & `django_kmuhelper-1.8.2/kmuhelper/utils.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/kmuhelper/views.py` & `django_kmuhelper-1.8.2/kmuhelper/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+import kmuhelper.modules.config as config
 from django.conf import settings
 from django.contrib.auth.decorators import login_required, permission_required
 from django.shortcuts import render, redirect
 from django.template import TemplateDoesNotExist, TemplateSyntaxError
 from django.template.loader import get_template
 from django.urls import NoReverseMatch, reverse_lazy, reverse
 from django.utils.translation import gettext
-
-import kmuhelper.modules.config as config
 from kmuhelper.constants import URL_MANUAL
 from kmuhelper.decorators import require_any_kmuhelper_perms
 from kmuhelper.utils import render_error
 
 _ = gettext
 
 # Create your views here.
@@ -21,58 +20,58 @@
 def home(request):
     grid = [
         [
             {
                 "title": _("Admin"),
                 "subtitle": _("Volle Kontrolle über die Hauptfunktionen"),
                 "url": reverse("admin:app_list", kwargs={"app_label": "kmuhelper"}),
-                "icon": "fas fa-key",
+                "icon": "fa-solid fa-key",
                 "hidden": not config.user_has_module_permission(request.user, "main"),
             },
             {
                 "title": _("App"),
                 "subtitle": _(
                     "Eingeschränkte Verwaltung von Daten in verschiedenen Arbeitsschritten"
                 ),
                 "url": reverse("kmuhelper:app-index"),
-                "icon": "fas fa-desktop",
+                "icon": "fa-solid fa-desktop",
                 "hidden": not config.user_has_module_permission(request.user, "app"),
             },
         ],
         [
             {
                 "title": _("E-Mails"),
                 "subtitle": _("Verwaltung und Erstellung von E-Mails"),
                 "url": reverse("kmuhelper:email-index"),
-                "icon": "fas fa-envelope-open",
+                "icon": "fa-solid fa-envelope-open",
                 "hidden": not config.user_has_module_permission(request.user, "emails"),
             },
             {
                 "title": _("Statistiken"),
                 "subtitle": _("Diagramme und co."),
                 "url": reverse("kmuhelper:stats"),
-                "icon": "fas fa-chart-pie",
+                "icon": "fa-solid fa-chart-pie",
                 "hidden": not config.user_has_module_permission(request.user, "main"),
             },
         ],
         [
             {
                 "title": _("Einstellungen"),
                 "subtitle": _("Einstellungen für den KMUHelper"),
                 "url": reverse("kmuhelper:settings"),
-                "icon": "fas fa-cog",
+                "icon": "fa-solid fa-cog",
                 "hidden": not config.user_has_module_permission(
                     request.user, "settings"
                 ),
             },
             {
                 "title": _("Handbuch"),
                 "subtitle": _("Dokumentation zum KMUHelper"),
                 "url": URL_MANUAL,
-                "icon": "fas fa-book",
+                "icon": "fa-solid fa-book",
             },
         ],
     ]
     return render(
         request, "kmuhelper/home.html", {"has_permission": True, "grid": grid}
     )
```

### Comparing `django-kmuhelper-1.8.1/kmuhelper/widgets.py` & `django_kmuhelper-1.8.2/kmuhelper/widgets.py`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/setup.cfg` & `django_kmuhelper-1.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-kmuhelper-1.8.1/tests/test_settings.py` & `django_kmuhelper-1.8.2/tests/test_settings.py`

 * *Files identical despite different names*

