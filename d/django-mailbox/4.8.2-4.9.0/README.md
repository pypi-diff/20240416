# Comparing `tmp/django-mailbox-4.8.2.tar.gz` & `tmp/django-mailbox-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mailbox-4.8.2.tar", last modified: Mon Dec  7 02:11:55 2020, max compression
+gzip compressed data, was "django-mailbox-4.9.0.tar", last modified: Sun Dec 10 03:12:01 2023, max compression
```

## Comparing `django-mailbox-4.8.2.tar` & `django-mailbox-4.9.0.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.521401 django-mailbox-4.8.2/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1057 2020-12-07 02:10:36.000000 django-mailbox-4.8.2/.travis.yml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2161 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/CHANGELOG.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      269 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/MANIFEST.in
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1464 2020-12-07 02:11:55.521401 django-mailbox-4.8.2/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.497401 django-mailbox-4.8.2/django_mailbox/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       80 2020-12-07 02:11:32.000000 django-mailbox-4.8.2/django_mailbox/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2645 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/admin.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      184 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/apps.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3117 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/google_utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.493401 django-mailbox-4.8.2/django_mailbox/locale/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.493401 django-mailbox-4.8.2/django_mailbox/locale/ru_RU/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.497401 django-mailbox-4.8.2/django_mailbox/locale/ru_RU/LC_MESSAGES/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5329 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/locale/ru_RU/LC_MESSAGES/django.mo
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6634 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/locale/ru_RU/LC_MESSAGES/django.po
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.497401 django-mailbox-4.8.2/django_mailbox/management/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/management/__init__.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.497401 django-mailbox-4.8.2/django_mailbox/management/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/management/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      820 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/management/commands/getmail.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1492 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/management/commands/processincomingmessage.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2772 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/management/commands/rebuildmessageattachments.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.501401 django-mailbox-4.8.2/django_mailbox/migrations/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4021 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0001_initial.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      463 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0002_add_eml_to_message.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      444 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0003_auto_20150409_0316.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      662 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0004_bytestring_to_unicode.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      455 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0005_auto_20160523_2240.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      599 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0006_mailbox_last_polling.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      765 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0007_auto_20180421_0026.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      913 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/0008_auto_20190219_1553.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/migrations/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    26542 2020-12-07 02:10:36.000000 django-mailbox-4.8.2/django_mailbox/models.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      101 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/signals.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.501401 django-mailbox-4.8.2/django_mailbox/south_migrations/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2749 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0001_initial.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1807 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0002_auto__chg_field_mailbox_uri.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1867 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0003_auto__add_field_mailbox_active.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1969 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0004_auto__add_field_message_outgoing.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1934 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0005_rename_fields.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3085 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0006_auto__add_field_message_in_reply_to.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3100 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0007_auto__del_field_message_address__add_field_message_from_header__add_fi.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2492 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0008_populate_from_to_fields.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2520 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0009_remove_references_table.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2409 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0010_auto__add_field_mailbox_from_email.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2494 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0011_auto__add_field_message_read.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3748 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0012_auto__add_messageattachment.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3295 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0013_auto__add_field_messageattachment_message.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3283 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0014_migrate_message_attachments.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3762 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0015_auto__add_field_messageattachment_headers.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3153 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0016_auto__add_field_message_encoded.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3294 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/0017_auto__add_field_message_eml.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/south_migrations/__init__.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.505401 django-mailbox-4.8.2/django_mailbox/tests/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6862 2020-12-07 01:57:41.000000 django-mailbox-4.8.2/django_mailbox/tests/base.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.517401 django-mailbox-4.8.2/django_mailbox/tests/messages/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1742 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/email_issue_82.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      432 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/generic_message.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1168 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_attachment.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1150 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_defective_attachment_association.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1173 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_defective_attachment_association_result.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5561 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_image_jpg_mimetype.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      267 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_invalid_content_for_declared_encoding.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_invalid_encoding.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)  4050754 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_koi8r_filename_attachments.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    20095 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_long_content.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      513 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_long_text_lines.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1224 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_many_multiparts.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1227 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_many_multiparts_stripped_html.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1180 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_not_decoded_attachment_header.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      259 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_single_byte_encoding.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3321 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_single_byte_extended_subject_encoding.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1133 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_text_attachment.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2070 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_utf8_attachment.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4027 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_utf8_char.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1086 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/messages/multipart_text.eml
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      247 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/settings.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2066 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/test_integration_imap.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1358 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/test_mailbox.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4021 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/test_message_flattening.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    14082 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/test_process_email.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3161 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/test_processincomingmessage.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5037 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/tests/test_transports.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.517401 django-mailbox-4.8.2/django_mailbox/transports/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      535 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      156 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/babyl.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      294 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/base.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      633 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/generic.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1966 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/gmail.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4441 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/imap.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      238 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/maildir.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      153 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/mbox.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      147 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/mh.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      153 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/mmdf.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1345 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/transports/pop3.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4640 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/django_mailbox/utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.497401 django-mailbox-4.8.2/django_mailbox.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1464 2020-12-07 02:11:55.000000 django-mailbox-4.8.2/django_mailbox.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4912 2020-12-07 02:11:55.000000 django-mailbox-4.8.2/django_mailbox.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2020-12-07 02:11:55.000000 django-mailbox-4.8.2/django_mailbox.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       46 2020-12-07 02:11:55.000000 django-mailbox-4.8.2/django_mailbox.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       15 2020-12-07 02:11:55.000000 django-mailbox-4.8.2/django_mailbox.egg-info/top_level.txt
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.517401 django-mailbox-4.8.2/docs/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5596 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/Makefile
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10097 2020-12-07 02:10:36.000000 django-mailbox-4.8.2/docs/conf.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1494 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/index.rst
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.517401 django-mailbox-4.8.2/docs/topics/
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2020-12-07 02:11:55.521401 django-mailbox-4.8.2/docs/topics/appendix/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      357 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/topics/appendix/instance-documentation.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5865 2020-12-07 02:10:36.000000 django-mailbox-4.8.2/docs/topics/appendix/message-storage.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3243 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/topics/appendix/settings.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       73 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/topics/appendix.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2450 2020-12-07 02:10:36.000000 django-mailbox-4.8.2/docs/topics/development.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1172 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/topics/installation.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5326 2020-12-07 02:10:36.000000 django-mailbox-4.8.2/docs/topics/mailbox_types.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3847 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/topics/polling.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      765 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/docs/topics/signal.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1439 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/readme.rst
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      164 2020-12-07 02:11:55.521401 django-mailbox-4.8.2/setup.cfg
--rwxrwxr-x   0 acoddington  (1000) acoddington  (1000)     1872 2020-12-07 00:59:28.000000 django-mailbox-4.8.2/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.745954 django-mailbox-4.9.0/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1057 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/.travis.yml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2370 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/CHANGELOG.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1082 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/LICENSE
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      269 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/MANIFEST.in
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1484 2023-12-10 03:12:01.745954 django-mailbox-4.9.0/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.725955 django-mailbox-4.9.0/django_mailbox/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       80 2023-12-10 03:11:20.000000 django-mailbox-4.9.0/django_mailbox/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2645 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/admin.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      239 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/apps.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3117 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/google_utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.721955 django-mailbox-4.9.0/django_mailbox/locale/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.721955 django-mailbox-4.9.0/django_mailbox/locale/ru_RU/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.725955 django-mailbox-4.9.0/django_mailbox/locale/ru_RU/LC_MESSAGES/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5329 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6634 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/locale/ru_RU/LC_MESSAGES/django.po
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.725955 django-mailbox-4.9.0/django_mailbox/management/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/management/__init__.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.725955 django-mailbox-4.9.0/django_mailbox/management/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/management/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      278 2023-12-10 03:00:37.000000 django-mailbox-4.9.0/django_mailbox/management/commands/getmail.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1492 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/management/commands/processincomingmessage.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2772 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/management/commands/rebuildmessageattachments.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.729955 django-mailbox-4.9.0/django_mailbox/migrations/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4021 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0001_initial.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      463 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0002_add_eml_to_message.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      444 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0003_auto_20150409_0316.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      662 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0004_bytestring_to_unicode.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      455 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0005_auto_20160523_2240.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      599 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0006_mailbox_last_polling.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      765 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0007_auto_20180421_0026.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      913 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/0008_auto_20190219_1553.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/migrations/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    28196 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/models.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      105 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/signals.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.729955 django-mailbox-4.9.0/django_mailbox/south_migrations/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2749 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0001_initial.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1807 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0002_auto__chg_field_mailbox_uri.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1867 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0003_auto__add_field_mailbox_active.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1969 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0004_auto__add_field_message_outgoing.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1934 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0005_rename_fields.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3085 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0006_auto__add_field_message_in_reply_to.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3100 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0007_auto__del_field_message_address__add_field_message_from_header__add_fi.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2492 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0008_populate_from_to_fields.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2520 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0009_remove_references_table.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2409 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0010_auto__add_field_mailbox_from_email.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2494 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0011_auto__add_field_message_read.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3748 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0012_auto__add_messageattachment.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3295 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0013_auto__add_field_messageattachment_message.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3283 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0014_migrate_message_attachments.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3762 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0015_auto__add_field_messageattachment_headers.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3153 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0016_auto__add_field_message_encoded.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3294 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/0017_auto__add_field_message_eml.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/south_migrations/__init__.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.729955 django-mailbox-4.9.0/django_mailbox/tests/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6862 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/base.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.741954 django-mailbox-4.9.0/django_mailbox/tests/messages/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1742 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/email_issue_82.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      432 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/generic_message.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1168 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_attachment.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1150 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_defective_attachment_association.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1173 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_defective_attachment_association_result.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5561 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_image_jpg_mimetype.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      267 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_invalid_content_for_declared_encoding.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_invalid_encoding.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)  4050754 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_koi8r_filename_attachments.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    20095 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_long_content.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      513 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_long_text_lines.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1224 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_many_multiparts.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1227 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_many_multiparts_stripped_html.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1180 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_not_decoded_attachment_header.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      259 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_single_byte_encoding.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3321 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_single_byte_extended_subject_encoding.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1133 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_text_attachment.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2070 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_utf8_attachment.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4027 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_utf8_char.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1086 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/messages/multipart_text.eml
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      247 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/settings.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2066 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/test_integration_imap.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1358 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/test_mailbox.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4021 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/tests/test_message_flattening.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    14066 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/tests/test_process_email.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1677 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/tests/test_processincomingmessage.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5036 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/tests/test_transports.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.745954 django-mailbox-4.9.0/django_mailbox/transports/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      602 2023-12-10 03:00:37.000000 django-mailbox-4.9.0/django_mailbox/transports/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      156 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/babyl.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      294 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/transports/base.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      623 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/transports/generic.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1966 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/gmail.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4441 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/imap.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      238 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/maildir.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      153 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/mbox.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      147 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/mh.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      153 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/mmdf.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2064 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/django_mailbox/transports/office365.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1345 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/transports/pop3.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4640 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/django_mailbox/utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.725955 django-mailbox-4.9.0/django_mailbox.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1484 2023-12-10 03:12:01.000000 django-mailbox-4.9.0/django_mailbox.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4959 2023-12-10 03:12:01.000000 django-mailbox-4.9.0/django_mailbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-12-10 03:12:01.000000 django-mailbox-4.9.0/django_mailbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       60 2023-12-10 03:12:01.000000 django-mailbox-4.9.0/django_mailbox.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       15 2023-12-10 03:12:01.000000 django-mailbox-4.9.0/django_mailbox.egg-info/top_level.txt
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.745954 django-mailbox-4.9.0/docs/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5596 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/Makefile
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10094 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/docs/conf.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1494 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/index.rst
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.745954 django-mailbox-4.9.0/docs/topics/
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-12-10 03:12:01.745954 django-mailbox-4.9.0/docs/topics/appendix/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      357 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/appendix/instance-documentation.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5865 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/appendix/message-storage.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3243 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/appendix/settings.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       73 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/appendix.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2450 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/development.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1172 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/installation.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6151 2023-12-10 03:00:37.000000 django-mailbox-4.9.0/docs/topics/mailbox_types.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3847 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/polling.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      765 2023-09-28 23:25:50.000000 django-mailbox-4.9.0/docs/topics/signal.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1453 2023-12-10 03:00:37.000000 django-mailbox-4.9.0/readme.rst
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      164 2023-12-10 03:12:01.749954 django-mailbox-4.9.0/setup.cfg
+-rwxrwxr-x   0 acoddington  (1000) acoddington  (1000)     1924 2023-12-10 03:08:47.000000 django-mailbox-4.9.0/setup.py
```

### Comparing `django-mailbox-4.8.2/.travis.yml` & `django-mailbox-4.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/CHANGELOG.rst` & `django-mailbox-4.9.0/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+Unreleased
+-----
+
+* Add Django 3.2, 4.0, 4.1, 4.2, 5.0 support
+* Remove support for deprecated Django versions
+
+* Add Python 3.8, 3.9, 3.10, 3.11, 3.12 support
+* Remove support for deprecated Python versions
+
 4.8.1
 -----
 
 * Add missing migration
 
 4.8.0
 -----
```

### Comparing `django-mailbox-4.8.2/PKG-INFO` & `django-mailbox-4.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django-mailbox
-Version: 4.8.2
+Version: 4.9.0
 Summary: Import mail from POP3, IMAP, local mailboxes or directly from Postfix or Exim4 into your Django application automatically.
 Home-page: http://github.com/coddingtonbear/django-mailbox/
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Email :: Post-Office
 Classifier: Topic :: Communications :: Email :: Post-Office :: IMAP
 Classifier: Topic :: Communications :: Email :: Post-Office :: POP3
 Classifier: Topic :: Communications :: Email :: Email Clients (MUA)
-Requires-Python: >=3
+Requires-Python: >=3.8
 Provides-Extra: gmail-oauth2
+Provides-Extra: office365-oauth2
+License-File: LICENSE
```

### Comparing `django-mailbox-4.8.2/django_mailbox/admin.py` & `django-mailbox-4.9.0/django_mailbox/admin.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/google_utils.py` & `django-mailbox-4.9.0/django_mailbox/google_utils.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/locale/ru_RU/LC_MESSAGES/django.mo` & `django-mailbox-4.9.0/django_mailbox/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/locale/ru_RU/LC_MESSAGES/django.po` & `django-mailbox-4.9.0/django_mailbox/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/management/commands/processincomingmessage.py` & `django-mailbox-4.9.0/django_mailbox/management/commands/processincomingmessage.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/management/commands/rebuildmessageattachments.py` & `django-mailbox-4.9.0/django_mailbox/management/commands/rebuildmessageattachments.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/migrations/0001_initial.py` & `django-mailbox-4.9.0/django_mailbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/migrations/0004_bytestring_to_unicode.py` & `django-mailbox-4.9.0/django_mailbox/migrations/0004_bytestring_to_unicode.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/migrations/0006_mailbox_last_polling.py` & `django-mailbox-4.9.0/django_mailbox/migrations/0006_mailbox_last_polling.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/migrations/0007_auto_20180421_0026.py` & `django-mailbox-4.9.0/django_mailbox/migrations/0007_auto_20180421_0026.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/migrations/0008_auto_20190219_1553.py` & `django-mailbox-4.9.0/django_mailbox/migrations/0008_auto_20190219_1553.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/models.py` & `django-mailbox-4.9.0/django_mailbox/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from quopri import encode as encode_quopri
 from io import BytesIO
 import base64
 import email
 import logging
 import mimetypes
 import os.path
-import sys
 import uuid
 from tempfile import NamedTemporaryFile
 
 import django
 from django.conf import settings as django_settings
 from django.core.files.base import ContentFile, File
 from django.core.mail.message import make_msgid
@@ -27,26 +26,26 @@
 from django.utils.translation import gettext_lazy as _
 from django.utils.timezone import now
 
 from django_mailbox import utils
 from django_mailbox.signals import message_received
 from django_mailbox.transports import Pop3Transport, ImapTransport, \
     MaildirTransport, MboxTransport, BabylTransport, MHTransport, \
-    MMDFTransport, GmailImapTransport
+    MMDFTransport, GmailImapTransport, Office365Transport
 
 logger = logging.getLogger(__name__)
 
 
 class MailboxQuerySet(models.QuerySet):
     def get_new_mail(self):
         count = 0
         for mailbox in self.all():
             logger.debug('Receiving mail for %s' % mailbox)
             count += sum(1 for i in mailbox.get_new_mail())
-        logger.debug('Received %d %s.', count, 'mails' if count != 1 else 'mail')
+        logger.debug('Received %d %s.', count, 'mail(s)')
 
 
 class MailboxManager(models.Manager):
     def get_queryset(self):
         return MailboxQuerySet(self.model, using=self._db)
 
 
@@ -119,14 +118,21 @@
         blank=True,
         null=True
     )
 
     objects = MailboxManager()
     active_mailboxes = ActiveMailboxManager()
 
+    class Meta:
+        verbose_name = _('Mailbox')
+        verbose_name_plural = _('Mailboxes')
+
+    def __str__(self):
+        return self.name
+
     @property
     def _protocol_info(self):
         return urlparse(self.uri)
 
     @property
     def _query_string(self):
         return parse_qs(self._protocol_info.query)
@@ -185,14 +191,38 @@
     def folder(self):
         """Returns (if specified) the folder to fetch mail from."""
         folder = self._query_string.get('folder', None)
         if not folder:
             return None
         return folder[0]
 
+    @property
+    def client_id(self):
+        """Returns (if specified) the client id for Office365."""
+        client_id = self._query_string.get('client_id', None)
+        if not client_id:
+            return None
+        return client_id[0]
+
+    @property
+    def client_secret(self):
+        """Returns (if specified) the client secret for Office365."""
+        client_secret = self._query_string.get('client_secret', None)
+        if not client_secret:
+            return None
+        return client_secret[0]
+
+    @property
+    def tenant_id(self):
+        """Returns (if specified) the tenant id for Office365."""
+        tenant_id = self._query_string.get('tenant_id', None)
+        if not tenant_id:
+            return None
+        return tenant_id[0]
+
     def get_connection(self):
         """Returns the transport instance for this mailbox.
 
         These will always be instances of
         `django_mailbox.transports.base.EmailTransport`.
 
         """
@@ -219,14 +249,22 @@
         elif self.type == 'pop3':
             conn = Pop3Transport(
                 self.location,
                 port=self.port if self.port else None,
                 ssl=self.use_ssl
             )
             conn.connect(self.username, self.password)
+        elif self.type == 'office365':
+            conn = Office365Transport(
+                self.location,
+                self.username,
+                folder=self.folder,
+                archive=self.archive
+            )
+            conn.connect(self.client_id, self.client_secret, self.tenant_id)
         elif self.type == 'maildir':
             conn = MaildirTransport(self.location)
         elif self.type == 'mbox':
             conn = MboxTransport(self.location)
         elif self.type == 'babyl':
             conn = BabylTransport(self.location)
         elif self.type == 'mh':
@@ -412,34 +450,46 @@
                 '%s.eml' % uuid.uuid4(),
                 ContentFile(message.as_string()),
                 save=False
             )
 
     def get_new_mail(self, condition=None):
         """Connect to this transport and fetch new messages."""
-        new_mail = []
         connection = self.get_connection()
         if not connection:
             return
         for message in connection.get_message(condition):
             msg = self.process_incoming_message(message)
-            if not msg is None:
+            if msg is not None:
                 yield msg
         self.last_polling = now()
         if django.VERSION >= (1, 5):  # Django 1.5 introduces update_fields
             self.save(update_fields=['last_polling'])
         else:
             self.save()
 
-    def __str__(self):
-        return self.name
-
-    class Meta:
-        verbose_name = _('Mailbox')
-        verbose_name_plural = _('Mailboxes')
+    @staticmethod
+    def get_new_mail_all_mailboxes(args=None):
+        mailboxes = Mailbox.active_mailboxes.all()
+        if args:
+            mailboxes = mailboxes.filter(
+                name=' '.join(args)
+            )
+        for mailbox in mailboxes:
+            logger.info(
+                'Gathering messages for %s',
+                mailbox.name
+            )
+            messages = mailbox.get_new_mail()
+            for message in messages:
+                logger.info(
+                    'Received %s (from %s)',
+                    message.subject,
+                    message.from_address
+                )
 
 
 class IncomingMessageManager(models.Manager):
     def get_queryset(self):
         return super().get_queryset().filter(
             outgoing=False,
         )
@@ -700,15 +750,15 @@
         self.encoded = True
         self.body = base64.b64encode(body.encode('utf-8')).decode('ascii')
 
     def get_email_object(self):
         """Returns an `email.message.EmailMessage` instance representing the
         contents of this message and all attachments.
 
-        See [email.message.EmailMessage]_ for more information as to what methods
+        See [email.message.EmailMessage]_ for more information like what methods
         and properties are available on `email.message.EmailMessage` instances.
 
         .. note::
 
            Depending upon the storage methods in use (specifically --
            whether ``DJANGO_MAILBOX_STORE_ORIGINAL_MESSAGE`` is set
            to ``True``, this may either create a "rehydrated" message
```

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0001_initial.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0002_auto__chg_field_mailbox_uri.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0002_auto__chg_field_mailbox_uri.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0003_auto__add_field_mailbox_active.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0003_auto__add_field_mailbox_active.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0004_auto__add_field_message_outgoing.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0004_auto__add_field_message_outgoing.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0005_rename_fields.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0005_rename_fields.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0006_auto__add_field_message_in_reply_to.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0006_auto__add_field_message_in_reply_to.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0007_auto__del_field_message_address__add_field_message_from_header__add_fi.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0007_auto__del_field_message_address__add_field_message_from_header__add_fi.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0008_populate_from_to_fields.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0008_populate_from_to_fields.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0009_remove_references_table.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0009_remove_references_table.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0010_auto__add_field_mailbox_from_email.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0010_auto__add_field_mailbox_from_email.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0011_auto__add_field_message_read.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0011_auto__add_field_message_read.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0012_auto__add_messageattachment.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0012_auto__add_messageattachment.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0013_auto__add_field_messageattachment_message.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0013_auto__add_field_messageattachment_message.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0014_migrate_message_attachments.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0014_migrate_message_attachments.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0015_auto__add_field_messageattachment_headers.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0015_auto__add_field_messageattachment_headers.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0016_auto__add_field_message_encoded.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0016_auto__add_field_message_encoded.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/south_migrations/0017_auto__add_field_message_eml.py` & `django-mailbox-4.9.0/django_mailbox/south_migrations/0017_auto__add_field_message_eml.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/base.py` & `django-mailbox-4.9.0/django_mailbox/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/email_issue_82.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/email_issue_82.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_attachment.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_attachment.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_defective_attachment_association.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_defective_attachment_association.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_defective_attachment_association_result.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_defective_attachment_association_result.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_image_jpg_mimetype.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_image_jpg_mimetype.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_koi8r_filename_attachments.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_koi8r_filename_attachments.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_long_content.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_long_content.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_long_text_lines.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_long_text_lines.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_many_multiparts.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_many_multiparts.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_many_multiparts_stripped_html.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_many_multiparts_stripped_html.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_not_decoded_attachment_header.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_not_decoded_attachment_header.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_single_byte_extended_subject_encoding.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_single_byte_extended_subject_encoding.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_text_attachment.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_text_attachment.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_utf8_attachment.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_utf8_attachment.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/message_with_utf8_char.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/message_with_utf8_char.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/messages/multipart_text.eml` & `django-mailbox-4.9.0/django_mailbox/tests/messages/multipart_text.eml`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/test_integration_imap.py` & `django-mailbox-4.9.0/django_mailbox/tests/test_integration_imap.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/test_mailbox.py` & `django-mailbox-4.9.0/django_mailbox/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/test_message_flattening.py` & `django-mailbox-4.9.0/django_mailbox/tests/test_message_flattening.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/test_process_email.py` & `django-mailbox-4.9.0/django_mailbox/tests/test_process_email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import gzip
 import os.path
-import sys
 
 import copy
 from unittest import mock
 
 from django_mailbox.models import Mailbox, Message
 from django_mailbox.utils import convert_header_to_unicode
 from django_mailbox import utils
 from django_mailbox.tests.base import EmailMessageTestCase
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.core.mail import EmailMessage
 
 __all__ = ['TestProcessEmail']
 
 
 class TestProcessEmail(EmailMessageTestCase):
     def test_message_without_attachments(self):
@@ -363,34 +362,34 @@
         self.assertEqual(msg.attachments.all().count(), 1)
         self.assertEqual('Has an attached text document, too!', msg.text)
 
     def test_message_with_long_content(self):
         email_object = self._get_email_object(
             'message_with_long_content.eml',
         )
-        size = len(force_text(email_object.as_string()))
+        size = len(force_str(email_object.as_string()))
 
         msg = self.mailbox.process_incoming_message(email_object)
 
         self.assertEqual(size,
-                         len(force_text(msg.get_email_object().as_string())))
+                         len(force_str(msg.get_email_object().as_string())))
 
     def test_message_saved(self):
         message = self._get_email_object('generic_message.eml')
 
         default_settings = utils.get_settings()
 
         with mock.patch('django_mailbox.utils.get_settings') as get_settings:
             altered = copy.deepcopy(default_settings)
             altered['store_original_message'] = True
             get_settings.return_value = altered
 
             msg = self.mailbox.process_incoming_message(message)
 
-        self.assertNotEquals(msg.eml, None)
+        self.assertNotEqual(msg.eml, None)
 
         self.assertTrue(msg.eml.name.endswith('.eml'))
 
         with open(msg.eml.name, 'rb') as f:
             self.assertEqual(
                 f.read(),
                 self._get_email_as_text('generic_message.eml')
@@ -404,15 +403,15 @@
         with mock.patch('django_mailbox.utils.get_settings') as get_settings:
             altered = copy.deepcopy(default_settings)
             altered['store_original_message'] = False
             get_settings.return_value = altered
 
             msg = self.mailbox.process_incoming_message(message)
 
-        self.assertEquals(msg.eml, None)
+        self.assertEqual(msg.eml, None)
 
     def test_message_compressed(self):
         message = self._get_email_object('generic_message.eml')
 
         default_settings = utils.get_settings()
 
         with mock.patch('django_mailbox.utils.get_settings') as get_settings:
```

### Comparing `django-mailbox-4.8.2/django_mailbox/tests/test_transports.py` & `django-mailbox-4.9.0/django_mailbox/tests/test_transports.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from django_mailbox.tests.base import EmailMessageTestCase, get_email_as_text
 from django_mailbox.transports import ImapTransport, Pop3Transport
 
 FAKE_UID_SEARCH_ANSWER = (
     'OK',
     [
-        b'18 19 20 21 22 23 24 25 26 27 28 29 ' + 
+        b'18 19 20 21 22 23 24 25 26 27 28 29 ' +
         b'30 31 32 33 34 35 36 37 38 39 40 41 42 43 44'
     ]
 )
 FAKE_UID_FETCH_SIZES = (
     'OK',
     [
         b'1 (UID 18 RFC822.SIZE 58070000000)',
```

### Comparing `django-mailbox-4.8.2/django_mailbox/transports/__init__.py` & `django-mailbox-4.9.0/django_mailbox/transports/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 from django_mailbox.transports.pop3 import Pop3Transport
 from django_mailbox.transports.maildir import MaildirTransport
 from django_mailbox.transports.mbox import MboxTransport
 from django_mailbox.transports.babyl import BabylTransport
 from django_mailbox.transports.mh import MHTransport
 from django_mailbox.transports.mmdf import MMDFTransport
 from django_mailbox.transports.gmail import GmailImapTransport
+from django_mailbox.transports.office365 import Office365Transport
```

### Comparing `django-mailbox-4.8.2/django_mailbox/transports/generic.py` & `django-mailbox-4.9.0/django_mailbox/transports/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import sys
+
 
 from .base import EmailTransport
 
 
 class GenericFileMailbox(EmailTransport):
     _variant = None
     _path = None
```

### Comparing `django-mailbox-4.8.2/django_mailbox/transports/gmail.py` & `django-mailbox-4.9.0/django_mailbox/transports/gmail.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/transports/imap.py` & `django-mailbox-4.9.0/django_mailbox/transports/imap.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/transports/pop3.py` & `django-mailbox-4.9.0/django_mailbox/transports/pop3.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox/utils.py` & `django-mailbox-4.9.0/django_mailbox/utils.py`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/django_mailbox.egg-info/PKG-INFO` & `django-mailbox-4.9.0/django_mailbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django-mailbox
-Version: 4.8.2
+Version: 4.9.0
 Summary: Import mail from POP3, IMAP, local mailboxes or directly from Postfix or Exim4 into your Django application automatically.
 Home-page: http://github.com/coddingtonbear/django-mailbox/
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Email :: Post-Office
 Classifier: Topic :: Communications :: Email :: Post-Office :: IMAP
 Classifier: Topic :: Communications :: Email :: Post-Office :: POP3
 Classifier: Topic :: Communications :: Email :: Email Clients (MUA)
-Requires-Python: >=3
+Requires-Python: >=3.8
 Provides-Extra: gmail-oauth2
+Provides-Extra: office365-oauth2
+License-File: LICENSE
```

### Comparing `django-mailbox-4.8.2/django_mailbox.egg-info/SOURCES.txt` & `django-mailbox-4.9.0/django_mailbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .travis.yml
 CHANGELOG.rst
+LICENSE
 MANIFEST.in
 readme.rst
 setup.cfg
 setup.py
 django_mailbox/__init__.py
 django_mailbox/admin.py
 django_mailbox/apps.py
@@ -85,14 +86,15 @@
 django_mailbox/transports/generic.py
 django_mailbox/transports/gmail.py
 django_mailbox/transports/imap.py
 django_mailbox/transports/maildir.py
 django_mailbox/transports/mbox.py
 django_mailbox/transports/mh.py
 django_mailbox/transports/mmdf.py
+django_mailbox/transports/office365.py
 django_mailbox/transports/pop3.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/topics/appendix.rst
 docs/topics/development.rst
 docs/topics/installation.rst
```

### Comparing `django-mailbox-4.8.2/docs/Makefile` & `django-mailbox-4.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/conf.py` & `django-mailbox-4.9.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 sys.path.insert(0, os.path.abspath('..'))
 import inspect
 import django
 from django.utils.html import strip_tags
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.conf import settings
 settings.configure(INSTALLED_APPS=['django_mailbox', ])
 django.setup()
 
 def process_docstring(app, what, name, obj, options, lines):
     # Source: https://gist.github.com/abulka/48b54ea4cbc7eb014308
     # This causes import errors if left outside the function
@@ -261,19 +261,19 @@
 
         for field in fields:
             # Skip ManyToOneRel and ManyToManyRel fields which have no 'verbose_name' or 'help_text'
             if not hasattr(field, 'verbose_name'):
                 continue
 
             # Decode and strip any html out of the field's help text
-            help_text = strip_tags(force_text(field.help_text))
+            help_text = strip_tags(force_str(field.help_text))
 
             # Decode and capitalize the verbose name, for use if there isn't
             # any help text
-            verbose_name = force_text(field.verbose_name).capitalize()
+            verbose_name = force_str(field.verbose_name).capitalize()
 
             if help_text:
                 # Add the model field to the end of the docstring as a param
                 # using the help text as the description
                 lines.append(':param {}: {}'.format(field.attname, help_text))
             else:
                 # Add the model field to the end of the docstring as a param
```

### Comparing `django-mailbox-4.8.2/docs/index.rst` & `django-mailbox-4.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/topics/appendix/message-storage.rst` & `django-mailbox-4.9.0/docs/topics/appendix/message-storage.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/topics/appendix/settings.rst` & `django-mailbox-4.9.0/docs/topics/appendix/settings.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/topics/development.rst` & `django-mailbox-4.9.0/docs/topics/development.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/topics/installation.rst` & `django-mailbox-4.9.0/docs/topics/installation.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/topics/mailbox_types.rst` & `django-mailbox-4.9.0/docs/topics/mailbox_types.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
   ============ ================ ====================================================================================================================================================================
   Mailbox Type 'Protocol'://    Notes
   ============ ================ ====================================================================================================================================================================
   POP3         ``pop3://``      Can also specify SSL with ``pop3+ssl://``
   IMAP         ``imap://``      Can also specify SSL with ``imap+ssl://`` or STARTTLS with ``imap+tls``; additional configuration is also possible: see :ref:`pop3-and-imap-mailboxes` for details.
   Gmail IMAP   ``gmail+ssl://`` Uses OAuth authentication for  Gmail's IMAP transport.  See :ref:`gmail-oauth` for details.
+  Office365 API``office365://`` Uses OAuth authentication for  Office365 API transport.  See :ref:`office365-oauth` for details.
   Maildir      ``maildir://``
   Mbox         ``mbox://``
   Babyl        ``babyl://``
   MH           ``mh://``
   MMDF         ``mmdf://``
   Piped Mail   *empty*          See :ref:`receiving-mail-from-exim4-or-postfix`
   ============ ================ ====================================================================================================================================================================
@@ -111,14 +112,33 @@
 It will fall back to use your specified password as needed.
 
 Build your URI accordingly::
 
     gmail+ssl://youremailaddress%40gmail.com:oauth2@imap.gmail.com?archive=Archived
 
 
+.. _office365-oauth:
+Office 365 API
+-------------------------------------
+
+Office 365 allows through the API to read a mailbox with Oauth.
+The O365_ library is used.
+
+.. _O365: https://github.com/O365/python-o365
+.. _configuration: https://github.com/O365/python-o365#authentication
+
+For the configuration_ you need to register an application and get a client_id, client_secret and tenant_id.
+
+This implementation uses the client credentials grant flow and the password you specify will be ignored.
+
+Build your URI accordingly::
+
+    office365://youremailaddress%40yourdomain.com:oauth2@outlook.office365.com?client_id=client_id&client_secret=client_secret&tenant_id=tenant_id&archive=Archived
+
+
 Local File-based Mailboxes
 --------------------------
 
 If you happen to want to consume a file-based mailbox like an Maildir, Mbox,
 Babyl, MH, or MMDF mailbox, you can use this too by entering the appropriate
 'protocol' in the URI.  If you had a maildir, for example, at ``/var/mail/``,
 you would enter a URI like::
```

### Comparing `django-mailbox-4.8.2/docs/topics/polling.rst` & `django-mailbox-4.9.0/docs/topics/polling.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/docs/topics/signal.rst` & `django-mailbox-4.9.0/docs/topics/signal.rst`

 * *Files identical despite different names*

### Comparing `django-mailbox-4.8.2/readme.rst` & `django-mailbox-4.9.0/readme.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .. image:: https://badge.fury.io/py/django-mailbox.png
     :target: http://badge.fury.io/py/django-mailbox
 
 .. image:: https://pypip.in/d/django-mailbox/badge.png
     :target: https://pypi.python.org/pypi/django-mailbox
 
 
-Easily ingest messages from POP3, IMAP, or local mailboxes into your Django application.
+Easily ingest messages from POP3, IMAP, Office365 API or local mailboxes into your Django application.
 
 This app allows you to either ingest e-mail content from common e-mail services (as long as the service provides POP3 or IMAP support),
 or directly receive e-mail messages from ``stdin`` (for locally processing messages from Postfix or Exim4).
 
 These ingested messages will be stored in the database in Django models and you can process their content at will,
 or -- if you're in a hurry -- by using a signal receiver.
```

### Comparing `django-mailbox-4.8.2/setup.py` & `django-mailbox-4.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,52 +9,54 @@
     'unittest2',
 ]
 
 gmail_oauth2_require = [
     'python-social-auth',
 ]
 
+office365_oauth2_require = [
+    'O365',
+]
+
 setup(
     name='django-mailbox',
     version=version_string,
     url='http://github.com/coddingtonbear/django-mailbox/',
     description=(
         'Import mail from POP3, IMAP, local mailboxes or directly from '
         'Postfix or Exim4 into your Django application automatically.'
     ),
     license='MIT',
     author='Adam Coddington',
     author_email='me@adamcoddington.net',
     extras_require={
-        'gmail-oauth2': gmail_oauth2_require
+        'gmail-oauth2': gmail_oauth2_require,
+        'office365-oauth2': office365_oauth2_require
     },
-    python_requires=">=3",
+    python_requires=">=3.8",
     classifiers=[
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 1.11',
-        'Framework :: Django :: 2.0',
-        'Framework :: Django :: 2.1',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Communications :: Email',
         'Topic :: Communications :: Email :: Post-Office',
         'Topic :: Communications :: Email :: Post-Office :: IMAP',
         'Topic :: Communications :: Email :: Post-Office :: POP3',
         'Topic :: Communications :: Email :: Email Clients (MUA)',
     ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=[
-        'six>=1.6.1'
-    ]
 )
```

