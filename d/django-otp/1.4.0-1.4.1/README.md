# Comparing `tmp/django_otp-1.4.0.tar.gz` & `tmp/django_otp-1.4.1.tar.gz`

## Comparing `django_otp-1.4.0.tar` & `django_otp-1.4.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    18115 2020-02-02 00:00:00.000000 django_otp-1.4.0/CHANGES.rst
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 django_otp-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/Makefile
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/ext/otpdocs.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/.spell.utf-8.add
--rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/auth.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/changes.rst
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/conf.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/contributing.rst
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/extend.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/index.rst
--rw-r--r--   0        0        0    19957 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/overview.rst
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/admin.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/conf.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/decorators.py
--rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/forms.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/middleware.py
--rw-r--r--   0        0        0    19417 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/models.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/oath.py
--rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/tests.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/util.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/views.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/admin.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/apps.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/conf.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/models.py
--rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/tests.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0005_emaildevice_last_generated_timestamp.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0006_add_timestamps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/__init__.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/admin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/apps.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/models.py
--rw-r--r--   0        0        0    13619 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/tests.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0003_add_timestamps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/__init__.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/admin.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/apps.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/lib.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/models.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/management/commands/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0003_add_timestamps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/__init__.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/admin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/apps.py
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/models.py
--rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/tests.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0003_add_timestamps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/templates/otp/admin111/login.html
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/config/github.toml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/config/sample.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/backends.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/config.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/settings.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/urls.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/views.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/about.html
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/home.html
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/navbar.html
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/root.html
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/bs5/input.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/bs5/select.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/otp/email/custom.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/otp/email/custom_html.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/otp/email/token.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/registration/login.html
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.4.0/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.4.0/.hgignore
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.4.0/LICENSE
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 django_otp-1.4.0/README.rst
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_otp-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 django_otp-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 django_otp-1.4.1/CHANGES.rst
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 django_otp-1.4.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/ext/otpdocs.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/.spell.utf-8.add
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/auth.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/changes.rst
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/conf.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/extend.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/index.rst
+-rw-r--r--   0        0        0    19957 2020-02-02 00:00:00.000000 django_otp-1.4.1/docs/source/overview.rst
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/admin.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/conf.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/decorators.py
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/forms.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/middleware.py
+-rw-r--r--   0        0        0    19417 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/models.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/oath.py
+-rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/tests.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/util.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/views.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/admin.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/apps.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/conf.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/models.py
+-rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/tests.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0005_emaildevice_last_generated_timestamp.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0006_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/__init__.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/apps.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/models.py
+-rw-r--r--   0        0        0    13619 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/tests.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/0003_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/__init__.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/admin.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/apps.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/lib.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/models.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/management/commands/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/0001_initial.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/0003_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/__init__.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/apps.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/models.py
+-rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/tests.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/0003_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.4.1/src/django_otp/templates/otp/admin111/login.html
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/config/github.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/config/sample.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/backends.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/config.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/settings.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/urls.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/views.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/about.html
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/home.html
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/navbar.html
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/root.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/bs5/input.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/bs5/select.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/otp/email/custom.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/otp/email/custom_html.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/otp/email/token.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.4.1/test/test_project/templates/registration/login.html
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.4.1/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.4.1/.hgignore
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.4.1/LICENSE
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 django_otp-1.4.1/README.rst
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_otp-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 django_otp-1.4.1/PKG-INFO
```

### Comparing `django_otp-1.4.0/CHANGES.rst` & `django_otp-1.4.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+v1.4.1 - April 10, 2024 - Minor EmailDevice updates
+--------------------------------------------------------------------------------
+
+- `#140`_: Support customization of email delivery.
+
+  See the :class:`~django_otp.plugins.otp_email.models.EmailDevice`
+  documentation for API details.
+
+- Support translation of the "sent by email" message.
+
+.. _#140: https://github.com/django-otp/django-otp/pull/140
+
+
 v1.4.0 - April 09, 2024 - Add TimestampMixin
 --------------------------------------------------------------------------------
 
 - `#137`_: Add TimestampMixin
 
   Add a new TimestampMixin with ``created_at`` and ``last_used_at`` fields for
   device models.
```

### Comparing `django_otp-1.4.0/CONTRIBUTING.rst` & `django_otp-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/docs/Makefile` & `django_otp-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/docs/source/.spell.utf-8.add` & `django_otp-1.4.1/docs/source/.spell.utf-8.add`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/docs/source/auth.rst` & `django_otp-1.4.1/docs/source/auth.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/docs/source/conf.py` & `django_otp-1.4.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 #  copyright = ''
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.4.0'
+release = '1.4.1'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `django_otp-1.4.0/docs/source/extend.rst` & `django_otp-1.4.1/docs/source/extend.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/docs/source/overview.rst` & `django_otp-1.4.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/__init__.py` & `django_otp-1.4.1/src/django_otp/__init__.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/admin.py` & `django_otp-1.4.1/src/django_otp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/conf.py` & `django_otp-1.4.1/src/django_otp/conf.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/decorators.py` & `django_otp-1.4.1/src/django_otp/decorators.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/forms.py` & `django_otp-1.4.1/src/django_otp/forms.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/middleware.py` & `django_otp-1.4.1/src/django_otp/middleware.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/models.py` & `django_otp-1.4.1/src/django_otp/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/oath.py` & `django_otp-1.4.1/src/django_otp/oath.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/tests.py` & `django_otp-1.4.1/src/django_otp/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/util.py` & `django_otp-1.4.1/src/django_otp/util.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/views.py` & `django_otp-1.4.1/src/django_otp/views.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.mo` & `django_otp-1.4.1/src/django_otp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.po` & `django_otp-1.4.1/src/django_otp/locale/de/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -3,92 +3,99 @@
 # This file is distributed under the same license as the django-otp package.
 # Mats Stottmeister <mats@mtn-media.de>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-otp master\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-07 11:23+0100\n"
+"POT-Creation-Date: 2024-04-10 09:55-0500\n"
 "PO-Revision-Date: 2023-03-07 11:23+0100\n"
 "Last-Translator: Mats Stottmeister <mats@mtn-media.de>\n"
 "Language-Team: \n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: .\src\django_otp\forms.py:59
+#: src/django_otp/forms.py:60
 msgid "Please enter your OTP token."
 msgstr "Bitte gebe das Einmalpasswort ein."
 
-#: .\src\django_otp\forms.py:60
+#: src/django_otp/forms.py:61
 #, python-brace-format
 msgid "Error generating challenge: {0}"
 msgstr "Fehler beim Generieren der Challenge: {0}"
 
-#: .\src\django_otp\forms.py:61
+#: src/django_otp/forms.py:62
 msgid "The selected OTP device is not interactive"
 msgstr "Das ausgewählte Einmalpasswort-Gerät ist nicht interaktiv."
 
-#: .\src\django_otp\forms.py:62
+#: src/django_otp/forms.py:63
 #, python-brace-format
 msgid "OTP Challenge: {0}"
 msgstr "Einmalpasswort-Challenge: {0}"
 
-#: .\src\django_otp\forms.py:63
+#: src/django_otp/forms.py:65
 msgid "Invalid token. Please make sure you have entered it correctly."
 msgstr "Ungültiges Einmalpasswort. Bitte überprüfe die Eingabe."
 
-#: .\src\django_otp\forms.py:65
+#: src/django_otp/forms.py:68
 #, python-format
 msgid ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempt, please try again soon."
 msgid_plural ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempts, please try again soon."
 msgstr[0] ""
-"Verifikation vorübergehend deaktiviert wegen %(failure_count)d fehlgeschlagenem "
-"Versuch, bitte versuche es gleich erneut."
+"Verifikation vorübergehend deaktiviert wegen %(failure_count)d "
+"fehlgeschlagenem Versuch, bitte versuche es gleich erneut."
 msgstr[1] ""
-"Verifikation vorübergehend deaktiviert wegen %(failure_count)d fehlgeschlagenen "
-"Versuchen, bitte versuche es gleich erneut."
+"Verifikation vorübergehend deaktiviert wegen %(failure_count)d "
+"fehlgeschlagenen Versuchen, bitte versuche es gleich erneut."
 
-#: .\src\django_otp\forms.py:68
+#: src/django_otp/forms.py:73
 msgid "Verification of the token is currently disabled"
 msgstr "Verifikation des Einmalpassworts ist derzeit deaktiviert"
 
-#: .\src\django_otp\templates\otp\admin111\login.html:38
+#: src/django_otp/plugins/otp_email/models.py:105
+msgid "sent by email"
+msgstr ""
+
+#: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the error below."
 msgstr "Bitte korrigiere den Fehler unter dieser Nachricht."
 
-#: .\src\django_otp\templates\otp\admin111\login.html:38
+#: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the errors below."
 msgstr "Bitte korrigiere die Fehler unter dieser Nachricht."
 
-#: .\src\django_otp\templates\otp\admin111\login.html:54
+#: src/django_otp/templates/otp/admin111/login.html:54
 #, python-format
 msgid ""
 "You are authenticated as %(username)s, but are not authorized to access this "
 "page. Would you like to login to a different account?"
-msgstr "Du bist mit dem Nutzer %(username)s authentifiziert, hast aber keine Berechtigung diese Seite aufzurufen. Möchtest du dich mit einem anderen Nutzer anmelden?"
+msgstr ""
+"Du bist mit dem Nutzer %(username)s authentifiziert, hast aber keine "
+"Berechtigung diese Seite aufzurufen. Möchtest du dich mit einem anderen "
+"Nutzer anmelden?"
 
-#: .\src\django_otp\templates\otp\admin111\login.html:74
+#: src/django_otp/templates/otp/admin111/login.html:74
 msgid "OTP Device:"
 msgstr "Einmalpasswort-Gerät:"
 
-#: .\src\django_otp\templates\otp\admin111\login.html:79
+#: src/django_otp/templates/otp/admin111/login.html:79
 msgid "OTP Token:"
 msgstr "Einmalpasswort:"
 
-#: .\src\django_otp\templates\otp\admin111\login.html:84
+#: src/django_otp/templates/otp/admin111/login.html:84
 msgid "Forgotten your password or username?"
 msgstr "Hast du dein Passwort oder deinen Nutzernamen vergessen?"
 
-#: .\src\django_otp\templates\otp\admin111\login.html:88
+#: src/django_otp/templates/otp/admin111/login.html:88
 msgid "Log in"
 msgstr "Anmelden"
 
-#: .\src\django_otp\templates\otp\admin111\login.html:90
+#: src/django_otp/templates/otp/admin111/login.html:90
 msgid "Get OTP Challenge"
 msgstr "Bekomme Einmalpasswort-Challenge"
```

### Comparing `django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.mo` & `django_otp-1.4.1/src/django_otp/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.po` & `django_otp-1.4.1/src/django_otp/locale/es/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -3,66 +3,70 @@
 # This file is distributed under the same license as the django-otp package.
 # Miguel González <migonzalvar@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-otp master\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-11-09 12:20-0600\n"
+"POT-Creation-Date: 2024-04-10 09:57-0500\n"
 "PO-Revision-Date: 2022-11-09 19:43+0100\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: src/django_otp/forms.py:59
+#: src/django_otp/forms.py:60
 msgid "Please enter your OTP token."
 msgstr "Por favor introduzca su token OTP."
 
-#: src/django_otp/forms.py:60
+#: src/django_otp/forms.py:61
 #, python-brace-format
 msgid "Error generating challenge: {0}"
 msgstr "Error al generar el reto: {0}"
 
-#: src/django_otp/forms.py:61
+#: src/django_otp/forms.py:62
 msgid "The selected OTP device is not interactive"
 msgstr "EL dispositivo OTP seleccionado no es interactivo"
 
-#: src/django_otp/forms.py:62
+#: src/django_otp/forms.py:63
 #, python-brace-format
 msgid "OTP Challenge: {0}"
 msgstr "Reto OTP: {0}"
 
-#: src/django_otp/forms.py:63
+#: src/django_otp/forms.py:65
 msgid "Invalid token. Please make sure you have entered it correctly."
 msgstr ""
 "Token no válido. Por favor asegúrese de que lo ha introducido correctamente."
 
-#: src/django_otp/forms.py:65
+#: src/django_otp/forms.py:68
 #, python-format
 msgid ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempt, please try again soon."
 msgid_plural ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempts, please try again soon."
 msgstr[0] ""
 "La verificación está temporalmente deshabilitada porque ha habido "
 "%(failure_count)d intento fallido, por favor inténtelo de nuevo más tarde."
 msgstr[1] ""
 "La verificación está temporalmente deshabilitada porque ha habido "
 "%(failure_count)d intentos fallidos, por favor inténtelo de nuevo más tarde."
 
-#: src/django_otp/forms.py:68
+#: src/django_otp/forms.py:73
 msgid "Verification of the token is currently disabled"
 msgstr "La verificación del token está desactivada en este momento"
 
+#: src/django_otp/plugins/otp_email/models.py:105
+msgid "sent by email"
+msgstr ""
+
 #: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the error below."
 msgstr "Por favor corrija el error abajo indicado."
 
 #: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the errors below."
 msgstr "Por favor corrija los errores abajo indicados."
```

### Comparing `django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo` & `django_otp-1.4.1/src/django_otp/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo` & `django_otp-1.4.1/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po` & `django_otp-1.4.1/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <alex@fabricadigital.com.br>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-otp master\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-24 12:34-0300\n"
+"POT-Creation-Date: 2024-04-10 09:57-0500\n"
 "PO-Revision-Date: 2023-05-24 12:34-0300\n"
 "Last-Translator: alex <alex@fabricadigital.com.br>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -43,36 +43,43 @@
 #, python-format
 msgid ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempt, please try again soon."
 msgid_plural ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempts, please try again soon."
-msgstr[0] "Verificação temporariamente desativada devido a %(failure_count)d tentativa(s) "
+msgstr[0] ""
+"Verificação temporariamente desativada devido a %(failure_count)d "
+"tentativa(s) "
 msgstr[1] "falha(s), por favor tente novamente em breve."
 
 #: src/django_otp/forms.py:73
 msgid "Verification of the token is currently disabled"
 msgstr "A verificação de código está desativada no momento"
 
+#: src/django_otp/plugins/otp_email/models.py:105
+msgid "sent by email"
+msgstr ""
+
 #: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the error below."
 msgstr "Por favor corrija o erro abaixo."
 
 #: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the errors below."
 msgstr "Por favor corrija os erros abaixo."
 
 #: src/django_otp/templates/otp/admin111/login.html:54
 #, python-format
 msgid ""
 "You are authenticated as %(username)s, but are not authorized to access this "
 "page. Would you like to login to a different account?"
-msgstr "Você está autenticado como %(username)s, mas não está autorizado a acessar essa "
-"página. Gostaria de autenticar-se com uma conta diferente?"
+msgstr ""
+"Você está autenticado como %(username)s, mas não está autorizado a acessar "
+"essa página. Gostaria de autenticar-se com uma conta diferente?"
 
 #: src/django_otp/templates/otp/admin111/login.html:74
 msgid "OTP Device:"
 msgstr "Dispositivo OTP:"
 
 #: src/django_otp/templates/otp/admin111/login.html:79
 msgid "OTP Token:"
```

### Comparing `django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo` & `django_otp-1.4.1/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po` & `django_otp-1.4.1/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # João Duarte <jduar@protonmail.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-otp master\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-02 11:00-0500\n"
+"POT-Creation-Date: 2024-04-10 09:57-0500\n"
 "PO-Revision-Date: 2023-10-02 11:00-0500\n"
 "Last-Translator: João Duarte <jduar@protonmail.com>\n"
 "Language-Team: \n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -33,15 +33,16 @@
 #: src/django_otp/forms.py:63
 #, python-brace-format
 msgid "OTP Challenge: {0}"
 msgstr "Desafio OTP: {0}"
 
 #: src/django_otp/forms.py:65
 msgid "Invalid token. Please make sure you have entered it correctly."
-msgstr "Código inválido. Certifique-se por favor de que o inseriu corretamente."
+msgstr ""
+"Código inválido. Certifique-se por favor de que o inseriu corretamente."
 
 #: src/django_otp/forms.py:68
 #, python-format
 msgid ""
 "Verification temporarily disabled because of %(failure_count)d failed "
 "attempt, please try again soon."
 msgid_plural ""
@@ -54,30 +55,34 @@
 "Verificação desativada temporariamente devido a %(failure_count)d tentativas "
 "falhadas, por favor tente novamente mais tarde."
 
 #: src/django_otp/forms.py:73
 msgid "Verification of the token is currently disabled"
 msgstr "A verificação do código está desativada de momento"
 
+#: src/django_otp/plugins/otp_email/models.py:105
+msgid "sent by email"
+msgstr ""
+
 #: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the error below."
 msgstr "Corrija por favor o erro abaixo."
 
 #: src/django_otp/templates/otp/admin111/login.html:38
 msgid "Please correct the errors below."
 msgstr "Corrija por favor os erros abaixo."
 
 #: src/django_otp/templates/otp/admin111/login.html:54
 #, python-format
 msgid ""
 "You are authenticated as %(username)s, but are not authorized to access this "
 "page. Would you like to login to a different account?"
 msgstr ""
-"Está autenticado como %(username)s, mas não está autorizado a aceder "
-"a esta página. Gostaria de autenticar-se com uma conta diferente?"
+"Está autenticado como %(username)s, mas não está autorizado a aceder a esta "
+"página. Gostaria de autenticar-se com uma conta diferente?"
 
 #: src/django_otp/templates/otp/admin111/login.html:74
 msgid "OTP Device:"
 msgstr "Dispositivo OTP:"
 
 #: src/django_otp/templates/otp/admin111/login.html:79
 msgid "OTP Token:"
```

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/admin.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/conf.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/conf.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/models.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib.humanize.templatetags.humanize import naturaltime
 from django.core.mail import send_mail
 from django.db import models
 from django.template import Context, Template
 from django.template.loader import get_template
+from django.utils.translation import gettext
 
 from django_otp.models import (
     CooldownMixin,
     GenerateNotAllowed,
     SideChannelDevice,
     ThrottlingMixin,
     TimestampMixin,
@@ -95,26 +96,35 @@
         elif settings.OTP_EMAIL_BODY_HTML_TEMPLATE_PATH:
             body_html = get_template(settings.OTP_EMAIL_BODY_HTML_TEMPLATE_PATH).render(
                 context
             )
         else:
             body_html = None
 
+        self.send_mail(body, html_message=body_html)
+
+        message = gettext("sent by email")
+
+        return message
+
+    def send_mail(self, body, **kwargs):
+        """
+        A simple wrapper for :func:`django.core.mail.send_mail`.
+
+        Subclasses (e.g. proxy models) may override this to customize delivery.
+
+        """
         send_mail(
             str(settings.OTP_EMAIL_SUBJECT),
             body,
             settings.OTP_EMAIL_SENDER,
             [self.email or self.user.email],
-            html_message=body_html,
+            **kwargs,
         )
 
-        message = "sent by email"
-
-        return message
-
     def verify_token(self, token):
         """"""
         verify_allowed, _ = self.verify_is_allowed()
         if verify_allowed:
             verified = super().verify_token(token)
 
             if verified:
```

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/tests.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0004_throttling.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0006_add_timestamps.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_email/migrations/0006_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/admin.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/models.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/tests.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0003_add_timestamps.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/migrations/0003_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html` & `django_otp-1.4.1/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/admin.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/lib.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/lib.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/models.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/tests.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/0002_throttling.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0003_add_timestamps.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_static/migrations/0003_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/admin.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/models.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/tests.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0003_add_timestamps.py` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/migrations/0003_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html` & `django_otp-1.4.1/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/src/django_otp/templates/otp/admin111/login.html` & `django_otp-1.4.1/src/django_otp/templates/otp/admin111/login.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/config/sample.toml` & `django_otp-1.4.1/test/config/sample.toml`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/config.py` & `django_otp-1.4.1/test/test_project/config.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/settings.py` & `django_otp-1.4.1/test/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/urls.py` & `django_otp-1.4.1/test/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/views.py` & `django_otp-1.4.1/test/test_project/views.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/templates/about.html` & `django_otp-1.4.1/test/test_project/templates/about.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/templates/home.html` & `django_otp-1.4.1/test/test_project/templates/home.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/templates/navbar.html` & `django_otp-1.4.1/test/test_project/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/templates/root.html` & `django_otp-1.4.1/test/test_project/templates/root.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/test/test_project/templates/registration/login.html` & `django_otp-1.4.1/test/test_project/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/LICENSE` & `django_otp-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/README.rst` & `django_otp-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.4.0/pyproject.toml` & `django_otp-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-otp"
-version = "1.4.0"
+version = "1.4.1"
 description = "A pluggable framework for adding two-factor authentication to Django using one-time passwords."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = "Unlicense"
 authors = [
     { name = "Peter Sagerson", email = "psagers@ignorare.net" },
 ]
```

### Comparing `django_otp-1.4.0/PKG-INFO` & `django_otp-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp
-Version: 1.4.0
+Version: 1.4.1
 Summary: A pluggable framework for adding two-factor authentication to Django using one-time passwords.
 Project-URL: Homepage, https://github.com/django-otp/django-otp
 Project-URL: Documentation, https://django-otp-official.readthedocs.io/
 Author-email: Peter Sagerson <psagers@ignorare.net>
 License-Expression: Unlicense
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_dzrcmf0i_/tmpd1f8lqye_TarContainer/0/106", line 173, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-otp Version: 1.4.0 Summary: A pluggable
+Metadata-Version: 2.1 Name: django-otp Version: 1.4.1 Summary: A pluggable
 framework for adding two-factor authentication to Django using one-time
 passwords. Project-URL: Homepage, https://github.com/django-otp/django-otp
 Project-URL: Documentation, https://django-otp-official.readthedocs.io/ Author-
 email: Peter Sagerson
 ignorare.net> License-Expression: Unlicense License-File: LICENSE Classifier:
 Development Status :: 5 - Production/Stable Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
```

