# Comparing `tmp/omaslib-0.1.8.tar.gz` & `tmp/omaslib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omaslib-0.1.8.tar", max compression
+gzip compressed data, was "omaslib-0.1.9.tar", max compression
```

## Comparing `omaslib-0.1.8.tar` & `omaslib-0.1.9.tar`

### file list

```diff
@@ -1,106 +1,107 @@
--rw-r--r--   0        0        0     1394 2023-07-19 13:14:08.057542 omaslib-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-19 09:37:36.845775 omaslib-0.1.8/omaslib/__init__.py
--rw-r--r--   0        0        0     9506 2024-03-22 15:16:31.222840 omaslib-0.1.8/omaslib/ontologies/admin.trig
--rw-r--r--   0        0        0    29093 2024-03-18 17:17:31.083072 omaslib-0.1.8/omaslib/ontologies/omas.shacl.trig
--rw-r--r--   0        0        0    30563 2024-03-18 17:26:49.584475 omaslib-0.1.8/omaslib/ontologies/omas.ttl
--rw-r--r--   0        0        0    15377 2024-03-22 15:23:01.271860 omaslib-0.1.8/omaslib/src/PermissionSet.py
--rw-r--r--   0        0        0        0 2023-07-19 09:39:12.241227 omaslib-0.1.8/omaslib/src/__init__.py
--rw-r--r--   0        0        0    18561 2024-03-26 23:21:13.443162 omaslib-0.1.8/omaslib/src/connection.py
--rw-r--r--   0        0        0    11535 2024-03-19 21:45:20.909010 omaslib-0.1.8/omaslib/src/datamodel.py
--rw-r--r--   0        0        0        0 2024-03-19 21:42:26.409233 omaslib-0.1.8/omaslib/src/dtypes/__init__.py
--rw-r--r--   0        0        0     1299 2024-03-26 17:36:02.455594 omaslib-0.1.8/omaslib/src/dtypes/bnode.py
--rw-r--r--   0        0        0     4197 2024-03-25 22:11:53.316173 omaslib-0.1.8/omaslib/src/dtypes/languagein.py
--rw-r--r--   0        0        0     1027 2024-03-22 14:04:00.182587 omaslib-0.1.8/omaslib/src/dtypes/namespaceiri.py
--rw-r--r--   0        0        0     1942 2024-03-26 22:43:23.464379 omaslib-0.1.8/omaslib/src/dtypes/rdfset.py
--rw-r--r--   0        0        0        0 2024-02-28 22:00:05.689069 omaslib-0.1.8/omaslib/src/enums/__init__.py
--rw-r--r--   0        0        0      827 2024-03-19 21:45:21.136713 omaslib-0.1.8/omaslib/src/enums/action.py
--rw-r--r--   0        0        0     4495 2024-03-18 18:13:34.816988 omaslib-0.1.8/omaslib/src/enums/language.py
--rw-r--r--   0        0        0     2180 2024-03-19 21:45:21.100258 omaslib-0.1.8/omaslib/src/enums/permissions.py
--rw-r--r--   0        0        0     1589 2024-02-06 14:31:59.876895 omaslib-0.1.8/omaslib/src/enums/propertyclassattr.py
--rw-r--r--   0        0        0      603 2024-02-29 21:30:27.350277 omaslib-0.1.8/omaslib/src/enums/propertyrestrictiontype.py
--rw-r--r--   0        0        0      191 2023-11-19 22:36:11.323046 omaslib-0.1.8/omaslib/src/enums/resourceclassattr.py
--rw-r--r--   0        0        0      636 2024-02-26 11:30:51.117127 omaslib-0.1.8/omaslib/src/enums/sparql_result_format.py
--rw-r--r--   0        0        0     6037 2024-03-12 23:45:44.382638 omaslib-0.1.8/omaslib/src/enums/xsd_datatypes.py
--rw-r--r--   0        0        0     2144 2024-03-19 21:45:20.915841 omaslib-0.1.8/omaslib/src/helpers/Notify.py
--rw-r--r--   0        0        0        0 2023-07-25 12:46:05.035356 omaslib-0.1.8/omaslib/src/helpers/__init__.py
--rw-r--r--   0        0        0    10491 2024-03-19 21:45:20.966581 omaslib-0.1.8/omaslib/src/helpers/context.py
--rw-r--r--   0        0        0    28910 2024-03-23 23:36:20.908154 omaslib-0.1.8/omaslib/src/helpers/langstring.py
--rw-r--r--   0        0        0     1735 2024-02-01 22:20:27.005301 omaslib-0.1.8/omaslib/src/helpers/observable_dict.py
--rw-r--r--   0        0        0     5354 2024-03-26 22:22:33.108155 omaslib-0.1.8/omaslib/src/helpers/observable_set.py
--rw-r--r--   0        0        0     6203 2024-03-09 23:34:07.127540 omaslib-0.1.8/omaslib/src/helpers/oldap_string_literal.py
--rw-r--r--   0        0        0     1127 2024-03-25 22:10:21.902526 omaslib-0.1.8/omaslib/src/helpers/omaserror.py
--rw-r--r--   0        0        0     1140 2024-03-19 21:45:20.993649 omaslib-0.1.8/omaslib/src/helpers/propertyclass_singleton.py
--rw-r--r--   0        0        0     9682 2024-03-26 17:36:47.000762 omaslib-0.1.8/omaslib/src/helpers/query_processor.py
--rw-r--r--   0        0        0     2850 2024-03-18 17:15:30.716301 omaslib-0.1.8/omaslib/src/helpers/semantic_version.py
--rw-r--r--   0        0        0     4086 2024-03-18 23:09:37.706102 omaslib-0.1.8/omaslib/src/helpers/serializer.py
--rw-r--r--   0        0        0     8929 2024-03-19 21:45:21.189013 omaslib-0.1.8/omaslib/src/helpers/tools.py
--rw-r--r--   0        0        0     2393 2024-03-19 21:45:21.196972 omaslib-0.1.8/omaslib/src/iconnection.py
--rw-r--r--   0        0        0     8003 2024-03-26 21:46:53.793720 omaslib-0.1.8/omaslib/src/in_project.py
--rw-r--r--   0        0        0     2877 2024-03-23 23:06:12.998163 omaslib-0.1.8/omaslib/src/model.py
--rw-r--r--   0        0        0    29500 2024-03-23 23:28:36.948163 omaslib-0.1.8/omaslib/src/project.py
--rw-r--r--   0        0        0    53549 2024-03-19 21:45:21.009162 omaslib-0.1.8/omaslib/src/propertyclass.py
--rw-r--r--   0        0        0    25088 2024-03-25 23:53:12.310439 omaslib-0.1.8/omaslib/src/propertyrestrictions.py
--rw-r--r--   0        0        0    47549 2024-03-19 21:45:21.124760 omaslib-0.1.8/omaslib/src/resourceclass.py
--rw-r--r--   0        0        0    26873 2024-03-26 22:30:01.629227 omaslib-0.1.8/omaslib/src/user.py
--rw-r--r--   0        0        0    31434 2024-03-26 22:28:35.112582 omaslib-0.1.8/omaslib/src/user_dataclass.py
--rw-r--r--   0        0        0        0 2024-03-19 21:08:19.995067 omaslib-0.1.8/omaslib/src/xsd/__init__.py
--rw-r--r--   0        0        0      528 2024-03-20 22:11:54.235531 omaslib-0.1.8/omaslib/src/xsd/xsd.py
--rw-r--r--   0        0        0     4401 2024-03-25 14:41:04.700572 omaslib-0.1.8/omaslib/src/xsd/xsd_anyuri.py
--rw-r--r--   0        0        0     1897 2024-03-25 14:41:30.517930 omaslib-0.1.8/omaslib/src/xsd/xsd_base64binary.py
--rw-r--r--   0        0        0     1418 2024-03-25 14:41:56.308454 omaslib-0.1.8/omaslib/src/xsd/xsd_boolean.py
--rw-r--r--   0        0        0      510 2024-03-21 22:55:42.981054 omaslib-0.1.8/omaslib/src/xsd/xsd_byte.py
--rw-r--r--   0        0        0     2319 2024-03-25 14:42:26.431353 omaslib-0.1.8/omaslib/src/xsd/xsd_date.py
--rw-r--r--   0        0        0     2151 2024-03-25 22:59:45.003373 omaslib-0.1.8/omaslib/src/xsd/xsd_datetime.py
--rw-r--r--   0        0        0     2235 2024-03-25 21:41:29.920797 omaslib-0.1.8/omaslib/src/xsd/xsd_datetimestamp.py
--rw-r--r--   0        0        0     3200 2024-03-25 14:43:40.810349 omaslib-0.1.8/omaslib/src/xsd/xsd_decimal.py
--rw-r--r--   0        0        0     3793 2024-03-25 14:44:01.773408 omaslib-0.1.8/omaslib/src/xsd/xsd_double.py
--rw-r--r--   0        0        0     1655 2024-03-25 14:50:20.414476 omaslib-0.1.8/omaslib/src/xsd/xsd_duration.py
--rw-r--r--   0        0        0     4075 2024-03-25 08:23:39.469297 omaslib-0.1.8/omaslib/src/xsd/xsd_float.py
--rw-r--r--   0        0        0     2219 2024-03-25 14:59:12.257020 omaslib-0.1.8/omaslib/src/xsd/xsd_gday.py
--rw-r--r--   0        0        0     2252 2024-03-25 15:00:24.848621 omaslib-0.1.8/omaslib/src/xsd/xsd_gmonth.py
--rw-r--r--   0        0        0     2497 2024-03-25 15:00:58.657826 omaslib-0.1.8/omaslib/src/xsd/xsd_gmonthday.py
--rw-r--r--   0        0        0     2466 2024-03-25 21:23:06.633703 omaslib-0.1.8/omaslib/src/xsd/xsd_gyear.py
--rw-r--r--   0        0        0     2803 2024-03-25 21:55:29.227682 omaslib-0.1.8/omaslib/src/xsd/xsd_gyearmonth.py
--rw-r--r--   0        0        0     1541 2024-03-25 21:28:40.157435 omaslib-0.1.8/omaslib/src/xsd/xsd_hexbinary.py
--rw-r--r--   0        0        0      329 2024-03-20 22:13:19.596239 omaslib-0.1.8/omaslib/src/xsd/xsd_id.py
--rw-r--r--   0        0        0      338 2024-03-20 22:20:21.227288 omaslib-0.1.8/omaslib/src/xsd/xsd_idref.py
--rw-r--r--   0        0        0      537 2024-03-21 22:57:19.550358 omaslib-0.1.8/omaslib/src/xsd/xsd_int.py
--rw-r--r--   0        0        0     3189 2024-03-24 23:44:17.374880 omaslib-0.1.8/omaslib/src/xsd/xsd_integer.py
--rw-r--r--   0        0        0     1733 2024-03-25 21:29:32.817304 omaslib-0.1.8/omaslib/src/xsd/xsd_language.py
--rw-r--r--   0        0        0      582 2024-03-21 22:58:44.561967 omaslib-0.1.8/omaslib/src/xsd/xsd_long.py
--rw-r--r--   0        0        0     1578 2024-03-25 21:30:03.610189 omaslib-0.1.8/omaslib/src/xsd/xsd_name.py
--rw-r--r--   0        0        0     4045 2024-03-25 21:30:26.057437 omaslib-0.1.8/omaslib/src/xsd/xsd_ncname.py
--rw-r--r--   0        0        0      486 2024-03-21 22:59:53.743467 omaslib-0.1.8/omaslib/src/xsd/xsd_negativeinteger.py
--rw-r--r--   0        0        0     1514 2024-03-25 21:31:09.506502 omaslib-0.1.8/omaslib/src/xsd/xsd_nmtoken.py
--rw-r--r--   0        0        0      512 2024-03-21 23:01:52.092177 omaslib-0.1.8/omaslib/src/xsd/xsd_nonnegativeinteger.py
--rw-r--r--   0        0        0      495 2024-03-21 23:11:35.886844 omaslib-0.1.8/omaslib/src/xsd/xsd_nonpositiveinteger.py
--rw-r--r--   0        0        0     1806 2024-03-25 21:31:35.613664 omaslib-0.1.8/omaslib/src/xsd/xsd_normalizedstring.py
--rw-r--r--   0        0        0      490 2024-03-21 23:18:50.245317 omaslib-0.1.8/omaslib/src/xsd/xsd_positiveinteger.py
--rw-r--r--   0        0        0     5077 2024-03-25 21:32:04.984450 omaslib-0.1.8/omaslib/src/xsd/xsd_qname.py
--rw-r--r--   0        0        0      527 2024-03-21 23:32:43.599106 omaslib-0.1.8/omaslib/src/xsd/xsd_short.py
--rw-r--r--   0        0        0     1581 2024-03-25 21:32:41.554635 omaslib-0.1.8/omaslib/src/xsd/xsd_string.py
--rw-r--r--   0        0        0     1901 2024-03-25 21:33:13.434341 omaslib-0.1.8/omaslib/src/xsd/xsd_time.py
--rw-r--r--   0        0        0     1935 2024-03-25 21:33:31.292614 omaslib-0.1.8/omaslib/src/xsd/xsd_token.py
--rw-r--r--   0        0        0      521 2024-03-22 13:19:53.077640 omaslib-0.1.8/omaslib/src/xsd/xsd_unsignedbyte.py
--rw-r--r--   0        0        0      501 2024-03-22 13:21:21.441751 omaslib-0.1.8/omaslib/src/xsd/xsd_unsignedint.py
--rw-r--r--   0        0        0      522 2024-03-22 13:28:34.021182 omaslib-0.1.8/omaslib/src/xsd/xsd_unsignedlong.py
--rw-r--r--   0        0        0      493 2024-03-22 13:51:43.880313 omaslib-0.1.8/omaslib/src/xsd/xsd_unsignedshort.py
--rw-r--r--   0        0        0        0 2023-10-06 22:30:58.619397 omaslib-0.1.8/omaslib/test/__init__.py
--rw-r--r--   0        0        0    12927 2024-03-19 21:45:21.130368 omaslib-0.1.8/omaslib/test/test_connection.py
--rw-r--r--   0        0        0     4882 2024-03-19 21:45:21.074877 omaslib-0.1.8/omaslib/test/test_context.py
--rw-r--r--   0        0        0    17281 2024-03-19 21:45:21.143058 omaslib-0.1.8/omaslib/test/test_datamodel.py
--rw-r--r--   0        0        0     7059 2024-03-22 15:02:49.171505 omaslib-0.1.8/omaslib/test/test_dtypes.py
--rw-r--r--   0        0        0     7458 2024-03-26 21:55:50.661965 omaslib-0.1.8/omaslib/test/test_in_project.py
--rw-r--r--   0        0        0    10378 2024-03-23 23:36:20.886138 omaslib-0.1.8/omaslib/test/test_langstring.py
--rw-r--r--   0        0        0     6267 2024-03-23 23:31:34.934369 omaslib-0.1.8/omaslib/test/test_project.py
--rw-r--r--   0        0        0    25578 2024-03-19 21:45:21.067865 omaslib-0.1.8/omaslib/test/test_propertyclass.py
--rw-r--r--   0        0        0     5176 2024-03-25 23:41:48.108294 omaslib-0.1.8/omaslib/test/test_propertyrestriction.py
--rw-r--r--   0        0        0    22560 2024-03-19 21:45:21.060269 omaslib-0.1.8/omaslib/test/test_propertyrestriction_old.py
--rw-r--r--   0        0        0    41881 2024-03-19 21:45:21.176880 omaslib-0.1.8/omaslib/test/test_resourceclass.py
--rw-r--r--   0        0        0    34330 2024-03-26 23:03:48.320880 omaslib-0.1.8/omaslib/test/test_user.py
--rw-r--r--   0        0        0    58180 2024-03-25 21:55:49.223371 omaslib-0.1.8/omaslib/test/test_xsd_datatypes.py
--rw-r--r--   0        0        0     9258 2024-01-19 23:02:01.035244 omaslib-0.1.8/omaslib/testdata/connection_test.trig
--rw-r--r--   0        0        0     1330 2024-01-19 23:02:01.075132 omaslib-0.1.8/omaslib/testdata/datamodel_test.trig
--rw-r--r--   0        0        0      301 2023-10-08 19:44:33.602019 omaslib-0.1.8/omaslib/testit.http
--rw-r--r--   0        0        0      881 2024-03-26 23:27:00.091047 omaslib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 omaslib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1394 2023-07-19 13:14:08.057542 omaslib-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 09:37:36.845775 omaslib-0.1.9/omaslib/__init__.py
+-rw-r--r--   0        0        0     9506 2024-03-22 15:16:31.222840 omaslib-0.1.9/omaslib/ontologies/admin.trig
+-rw-r--r--   0        0        0    29093 2024-03-18 17:17:31.083072 omaslib-0.1.9/omaslib/ontologies/omas.shacl.trig
+-rw-r--r--   0        0        0    30563 2024-03-18 17:26:49.584475 omaslib-0.1.9/omaslib/ontologies/omas.ttl
+-rw-r--r--   0        0        0    15377 2024-03-22 15:23:01.271860 omaslib-0.1.9/omaslib/src/PermissionSet.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:39:12.241227 omaslib-0.1.9/omaslib/src/__init__.py
+-rw-r--r--   0        0        0    18561 2024-03-26 23:21:13.443162 omaslib-0.1.9/omaslib/src/connection.py
+-rw-r--r--   0        0        0    11535 2024-03-19 21:45:20.909010 omaslib-0.1.9/omaslib/src/datamodel.py
+-rw-r--r--   0        0        0        0 2024-03-19 21:42:26.409233 omaslib-0.1.9/omaslib/src/dtypes/__init__.py
+-rw-r--r--   0        0        0     1299 2024-03-26 17:36:02.455594 omaslib-0.1.9/omaslib/src/dtypes/bnode.py
+-rw-r--r--   0        0        0     4489 2024-04-01 22:37:11.732849 omaslib-0.1.9/omaslib/src/dtypes/languagein.py
+-rw-r--r--   0        0        0     1027 2024-03-22 14:04:00.182587 omaslib-0.1.9/omaslib/src/dtypes/namespaceiri.py
+-rw-r--r--   0        0        0     2831 2024-04-03 22:19:58.153423 omaslib-0.1.9/omaslib/src/dtypes/rdfset.py
+-rw-r--r--   0        0        0     6570 2024-04-01 21:34:10.586708 omaslib-0.1.9/omaslib/src/dtypes/string_literal.py
+-rw-r--r--   0        0        0        0 2024-02-28 22:00:05.689069 omaslib-0.1.9/omaslib/src/enums/__init__.py
+-rw-r--r--   0        0        0      827 2024-03-19 21:45:21.136713 omaslib-0.1.9/omaslib/src/enums/action.py
+-rw-r--r--   0        0        0     4495 2024-03-18 18:13:34.816988 omaslib-0.1.9/omaslib/src/enums/language.py
+-rw-r--r--   0        0        0     2180 2024-03-19 21:45:21.100258 omaslib-0.1.9/omaslib/src/enums/permissions.py
+-rw-r--r--   0        0        0     1580 2024-04-03 20:57:25.058560 omaslib-0.1.9/omaslib/src/enums/propertyclassattr.py
+-rw-r--r--   0        0        0      603 2024-02-29 21:30:27.350277 omaslib-0.1.9/omaslib/src/enums/propertyrestrictiontype.py
+-rw-r--r--   0        0        0      191 2023-11-19 22:36:11.323046 omaslib-0.1.9/omaslib/src/enums/resourceclassattr.py
+-rw-r--r--   0        0        0      636 2024-02-26 11:30:51.117127 omaslib-0.1.9/omaslib/src/enums/sparql_result_format.py
+-rw-r--r--   0        0        0     6099 2024-03-31 21:43:37.967373 omaslib-0.1.9/omaslib/src/enums/xsd_datatypes.py
+-rw-r--r--   0        0        0     2119 2024-04-05 21:07:48.406756 omaslib-0.1.9/omaslib/src/helpers/Notify.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:46:05.035356 omaslib-0.1.9/omaslib/src/helpers/__init__.py
+-rw-r--r--   0        0        0    10491 2024-03-19 21:45:20.966581 omaslib-0.1.9/omaslib/src/helpers/context.py
+-rw-r--r--   0        0        0    29879 2024-04-04 21:43:44.593027 omaslib-0.1.9/omaslib/src/helpers/langstring.py
+-rw-r--r--   0        0        0     1735 2024-02-01 22:20:27.005301 omaslib-0.1.9/omaslib/src/helpers/observable_dict.py
+-rw-r--r--   0        0        0     5354 2024-03-26 22:22:33.108155 omaslib-0.1.9/omaslib/src/helpers/observable_set.py
+-rw-r--r--   0        0        0     1127 2024-03-25 22:10:21.902526 omaslib-0.1.9/omaslib/src/helpers/omaserror.py
+-rw-r--r--   0        0        0     1140 2024-03-19 21:45:20.993649 omaslib-0.1.9/omaslib/src/helpers/propertyclass_singleton.py
+-rw-r--r--   0        0        0     9950 2024-04-03 16:02:57.926422 omaslib-0.1.9/omaslib/src/helpers/query_processor.py
+-rw-r--r--   0        0        0     2850 2024-03-18 17:15:30.716301 omaslib-0.1.9/omaslib/src/helpers/semantic_version.py
+-rw-r--r--   0        0        0     4086 2024-03-18 23:09:37.706102 omaslib-0.1.9/omaslib/src/helpers/serializer.py
+-rw-r--r--   0        0        0     9132 2024-04-02 20:27:13.341537 omaslib-0.1.9/omaslib/src/helpers/tools.py
+-rw-r--r--   0        0        0     2422 2024-04-05 21:07:48.415634 omaslib-0.1.9/omaslib/src/iconnection.py
+-rw-r--r--   0        0        0     7423 2024-04-04 22:12:09.667057 omaslib-0.1.9/omaslib/src/in_project.py
+-rw-r--r--   0        0        0     2898 2024-04-02 22:28:37.209679 omaslib-0.1.9/omaslib/src/model.py
+-rw-r--r--   0        0        0    30342 2024-04-04 21:53:13.299918 omaslib-0.1.9/omaslib/src/project.py
+-rw-r--r--   0        0        0    57975 2024-04-05 21:52:18.606124 omaslib-0.1.9/omaslib/src/propertyclass.py
+-rw-r--r--   0        0        0    24816 2024-04-04 22:32:47.101490 omaslib-0.1.9/omaslib/src/propertyrestrictions.py
+-rw-r--r--   0        0        0    48511 2024-04-07 22:53:37.879544 omaslib-0.1.9/omaslib/src/resourceclass.py
+-rw-r--r--   0        0        0    26660 2024-04-02 23:31:30.583912 omaslib-0.1.9/omaslib/src/user.py
+-rw-r--r--   0        0        0    31251 2024-04-02 23:25:20.684578 omaslib-0.1.9/omaslib/src/user_dataclass.py
+-rw-r--r--   0        0        0        0 2024-03-19 21:08:19.995067 omaslib-0.1.9/omaslib/src/xsd/__init__.py
+-rw-r--r--   0        0        0     3150 2024-04-03 22:31:10.660409 omaslib-0.1.9/omaslib/src/xsd/iri.py
+-rw-r--r--   0        0        0      585 2024-04-04 22:05:10.973300 omaslib-0.1.9/omaslib/src/xsd/xsd.py
+-rw-r--r--   0        0        0     4407 2024-04-02 21:16:38.198722 omaslib-0.1.9/omaslib/src/xsd/xsd_anyuri.py
+-rw-r--r--   0        0        0     1897 2024-03-25 14:41:30.517930 omaslib-0.1.9/omaslib/src/xsd/xsd_base64binary.py
+-rw-r--r--   0        0        0     1418 2024-03-25 14:41:56.308454 omaslib-0.1.9/omaslib/src/xsd/xsd_boolean.py
+-rw-r--r--   0        0        0      509 2024-03-30 23:29:35.613772 omaslib-0.1.9/omaslib/src/xsd/xsd_byte.py
+-rw-r--r--   0        0        0     2319 2024-03-25 14:42:26.431353 omaslib-0.1.9/omaslib/src/xsd/xsd_date.py
+-rw-r--r--   0        0        0     2151 2024-03-25 22:59:45.003373 omaslib-0.1.9/omaslib/src/xsd/xsd_datetime.py
+-rw-r--r--   0        0        0     2235 2024-03-25 21:41:29.920797 omaslib-0.1.9/omaslib/src/xsd/xsd_datetimestamp.py
+-rw-r--r--   0        0        0     3215 2024-04-02 20:24:36.018905 omaslib-0.1.9/omaslib/src/xsd/xsd_decimal.py
+-rw-r--r--   0        0        0     3793 2024-03-25 14:44:01.773408 omaslib-0.1.9/omaslib/src/xsd/xsd_double.py
+-rw-r--r--   0        0        0     1655 2024-03-25 14:50:20.414476 omaslib-0.1.9/omaslib/src/xsd/xsd_duration.py
+-rw-r--r--   0        0        0     4075 2024-03-25 08:23:39.469297 omaslib-0.1.9/omaslib/src/xsd/xsd_float.py
+-rw-r--r--   0        0        0     2219 2024-03-25 14:59:12.257020 omaslib-0.1.9/omaslib/src/xsd/xsd_gday.py
+-rw-r--r--   0        0        0     2252 2024-03-25 15:00:24.848621 omaslib-0.1.9/omaslib/src/xsd/xsd_gmonth.py
+-rw-r--r--   0        0        0     2497 2024-03-25 15:00:58.657826 omaslib-0.1.9/omaslib/src/xsd/xsd_gmonthday.py
+-rw-r--r--   0        0        0     2466 2024-03-25 21:23:06.633703 omaslib-0.1.9/omaslib/src/xsd/xsd_gyear.py
+-rw-r--r--   0        0        0     2803 2024-03-25 21:55:29.227682 omaslib-0.1.9/omaslib/src/xsd/xsd_gyearmonth.py
+-rw-r--r--   0        0        0     1541 2024-03-25 21:28:40.157435 omaslib-0.1.9/omaslib/src/xsd/xsd_hexbinary.py
+-rw-r--r--   0        0        0      329 2024-03-20 22:13:19.596239 omaslib-0.1.9/omaslib/src/xsd/xsd_id.py
+-rw-r--r--   0        0        0      338 2024-03-20 22:20:21.227288 omaslib-0.1.9/omaslib/src/xsd/xsd_idref.py
+-rw-r--r--   0        0        0      536 2024-03-30 23:29:35.681168 omaslib-0.1.9/omaslib/src/xsd/xsd_int.py
+-rw-r--r--   0        0        0     3188 2024-03-30 23:27:43.895979 omaslib-0.1.9/omaslib/src/xsd/xsd_integer.py
+-rw-r--r--   0        0        0     1733 2024-03-25 21:29:32.817304 omaslib-0.1.9/omaslib/src/xsd/xsd_language.py
+-rw-r--r--   0        0        0      581 2024-03-30 23:29:35.639195 omaslib-0.1.9/omaslib/src/xsd/xsd_long.py
+-rw-r--r--   0        0        0     1485 2024-04-01 21:10:04.545903 omaslib-0.1.9/omaslib/src/xsd/xsd_name.py
+-rw-r--r--   0        0        0     4045 2024-03-25 21:30:26.057437 omaslib-0.1.9/omaslib/src/xsd/xsd_ncname.py
+-rw-r--r--   0        0        0      485 2024-03-30 23:29:35.655963 omaslib-0.1.9/omaslib/src/xsd/xsd_negativeinteger.py
+-rw-r--r--   0        0        0     1514 2024-03-25 21:31:09.506502 omaslib-0.1.9/omaslib/src/xsd/xsd_nmtoken.py
+-rw-r--r--   0        0        0      511 2024-03-30 23:27:43.879079 omaslib-0.1.9/omaslib/src/xsd/xsd_nonnegativeinteger.py
+-rw-r--r--   0        0        0      494 2024-03-30 23:29:35.664142 omaslib-0.1.9/omaslib/src/xsd/xsd_nonpositiveinteger.py
+-rw-r--r--   0        0        0     1784 2024-04-01 21:10:04.630637 omaslib-0.1.9/omaslib/src/xsd/xsd_normalizedstring.py
+-rw-r--r--   0        0        0      489 2024-03-30 23:29:35.624181 omaslib-0.1.9/omaslib/src/xsd/xsd_positiveinteger.py
+-rw-r--r--   0        0        0     5083 2024-04-02 21:16:38.219339 omaslib-0.1.9/omaslib/src/xsd/xsd_qname.py
+-rw-r--r--   0        0        0      526 2024-03-30 23:29:35.668965 omaslib-0.1.9/omaslib/src/xsd/xsd_short.py
+-rw-r--r--   0        0        0     1736 2024-04-01 22:00:51.642696 omaslib-0.1.9/omaslib/src/xsd/xsd_string.py
+-rw-r--r--   0        0        0     1901 2024-03-25 21:33:13.434341 omaslib-0.1.9/omaslib/src/xsd/xsd_time.py
+-rw-r--r--   0        0        0     1903 2024-04-01 21:10:04.595263 omaslib-0.1.9/omaslib/src/xsd/xsd_token.py
+-rw-r--r--   0        0        0      520 2024-03-30 23:29:35.648134 omaslib-0.1.9/omaslib/src/xsd/xsd_unsignedbyte.py
+-rw-r--r--   0        0        0      507 2024-03-30 23:29:35.672649 omaslib-0.1.9/omaslib/src/xsd/xsd_unsignedint.py
+-rw-r--r--   0        0        0      528 2024-03-30 23:29:35.676496 omaslib-0.1.9/omaslib/src/xsd/xsd_unsignedlong.py
+-rw-r--r--   0        0        0      499 2024-03-30 23:29:42.742906 omaslib-0.1.9/omaslib/src/xsd/xsd_unsignedshort.py
+-rw-r--r--   0        0        0        0 2023-10-06 22:30:58.619397 omaslib-0.1.9/omaslib/test/__init__.py
+-rw-r--r--   0        0        0    12866 2024-04-03 10:18:18.922297 omaslib-0.1.9/omaslib/test/test_connection.py
+-rw-r--r--   0        0        0     4882 2024-04-03 10:26:55.118128 omaslib-0.1.9/omaslib/test/test_context.py
+-rw-r--r--   0        0        0    16695 2024-04-03 20:57:25.119264 omaslib-0.1.9/omaslib/test/test_datamodel.py
+-rw-r--r--   0        0        0     7227 2024-04-03 22:21:04.178656 omaslib-0.1.9/omaslib/test/test_dtypes.py
+-rw-r--r--   0        0        0     7462 2024-04-04 22:12:45.311011 omaslib-0.1.9/omaslib/test/test_in_project.py
+-rw-r--r--   0        0        0    10350 2024-04-08 09:32:15.986406 omaslib-0.1.9/omaslib/test/test_langstring.py
+-rw-r--r--   0        0        0     8174 2024-04-04 21:28:55.158333 omaslib-0.1.9/omaslib/test/test_project.py
+-rw-r--r--   0        0        0    27909 2024-04-05 20:26:11.354450 omaslib-0.1.9/omaslib/test/test_propertyclass.py
+-rw-r--r--   0        0        0    12215 2024-04-04 22:31:31.034974 omaslib-0.1.9/omaslib/test/test_propertyrestriction.py
+-rw-r--r--   0        0        0    18018 2024-04-07 22:48:38.670685 omaslib-0.1.9/omaslib/test/test_resourceclass.py
+-rw-r--r--   0        0        0    40382 2024-04-03 20:57:25.107225 omaslib-0.1.9/omaslib/test/test_resourceclass_old.py
+-rw-r--r--   0        0        0    34016 2024-04-02 23:51:08.583653 omaslib-0.1.9/omaslib/test/test_user.py
+-rw-r--r--   0        0        0    59280 2024-04-03 16:05:31.943675 omaslib-0.1.9/omaslib/test/test_xsd_datatypes.py
+-rw-r--r--   0        0        0     9741 2024-04-01 21:46:51.953917 omaslib-0.1.9/omaslib/testdata/connection_test.trig
+-rw-r--r--   0        0        0     1330 2024-01-19 23:02:01.075132 omaslib-0.1.9/omaslib/testdata/datamodel_test.trig
+-rw-r--r--   0        0        0      301 2023-10-08 19:44:33.602019 omaslib-0.1.9/omaslib/testit.http
+-rw-r--r--   0        0        0      881 2024-04-08 13:25:17.895007 omaslib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 omaslib-0.1.9/PKG-INFO
```

### Comparing `omaslib-0.1.8/README.md` & `omaslib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/ontologies/admin.trig` & `omaslib-0.1.9/omaslib/ontologies/admin.trig`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/ontologies/omas.shacl.trig` & `omaslib-0.1.9/omaslib/ontologies/omas.shacl.trig`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/ontologies/omas.ttl` & `omaslib-0.1.9/omaslib/ontologies/omas.ttl`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/PermissionSet.py` & `omaslib-0.1.9/omaslib/src/PermissionSet.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/connection.py` & `omaslib-0.1.9/omaslib/src/connection.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/datamodel.py` & `omaslib-0.1.9/omaslib/src/datamodel.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/dtypes/bnode.py` & `omaslib-0.1.9/omaslib/src/dtypes/bnode.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/dtypes/languagein.py` & `omaslib-0.1.9/omaslib/src/dtypes/languagein.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterator, Self
 
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.omaserror import OmasErrorValue, OmasErrorType
+from omaslib.src.xsd.xsd_string import Xsd_string
 
 
 class LanguageIn:
     """
     This class implements the SHACL sh:languageIn datatype. It completely validates the input.
     If the validations failes, an OmasErrorValue is raised.
     """
@@ -40,23 +41,29 @@
                         if isinstance(arg, Language):
                             self.__data.add(arg)
                         elif isinstance(arg, str):
                             self.__data.add(Language[arg.upper()])
         except KeyError:
             raise OmasErrorValue("Non valid language in set.")
 
-    def __eq__(self, other: Self | None) -> bool:
+    def __eq__(self, other: Self | set | None) -> bool:
         if other is None:
             return False
-        return self.__data == other.__data
+        if isinstance(other, LanguageIn):
+            return self.__data == other.__data
+        else:
+            return self.__data == other
 
     def __ne__(self, other: Self | None):
         if other is None:
             return False
-        return self.__data != other.__data
+        if isinstance(other, LanguageIn):
+            return self.__data != other.__data
+        else:
+            return self.__data != other
 
     def __gt__(self, other: Self) -> bool:
         if not isinstance(other, LanguageIn):
             raise OmasErrorType(f'Cannot compare {type(self).__name__} to {type(other).__name__}')
         return self.__data > other.__data
 
     def __ge__(self, other: Self) -> bool:
@@ -84,26 +91,26 @@
 
     def __contains__(self, language: Language):
         return language in self.__data
 
     def __iter__(self) -> Iterator[Language]:
         return iter(self.__data)
 
-    def add(self, language: Language | str):
+    def add(self, language: Language | Xsd_string | str):
         if not isinstance(language, Language):
             try:
-                language = Language[language.upper()]
+                language = Language[str(language).upper()]
             except ValueError as err:
                 raise OmasErrorValue(str(err))
         self.__data.add(language)
 
-    def discard(self, language: Language | str):
+    def discard(self, language: Language | Xsd_string | str):
         if not isinstance(language, Language):
             try:
-                language = Language[language.upper()]
+                language = Language[str(language).upper()]
             except ValueError as err:
                 raise OmasErrorValue(str(err))
         self.__data.discard(language)
 
     @property
     def toRdf(self) -> str:
         langlist = {f'"{x.name.lower()}"^^xsd:string' for x in self}
```

### Comparing `omaslib-0.1.8/omaslib/src/dtypes/namespaceiri.py` & `omaslib-0.1.9/omaslib/src/dtypes/namespaceiri.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/dtypes/rdfset.py` & `omaslib-0.1.9/omaslib/src/dtypes/rdfset.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,41 @@
 
 
 @strict
 @serializer
 class RdfSet:
     __data: Set[Xsd]
 
-    def __init__(self, value: Iterable[Xsd]):
+    def __init__(self, value: Iterable[Xsd] | Xsd | None = None, *args: Iterable[Xsd] | Xsd) -> None:
         self.__data: Set[Xsd] = set()
-        for val in value:
-            if not isinstance(val, Xsd):
+        if len(args) == 0:
+            if value is None:
+                return
+            else:
+                if isinstance(value, Iterable):
+                    values: Iterable[Xsd] = value
+                    for val in values:
+                        if not isinstance(val, Xsd):
+                            raise OmasErrorValue("Set elements must be of Subclasses of Xsd.")
+                        self.__data.add(val)
+                elif isinstance(value, Xsd):
+                    self.__data.add(value)
+                else:
+                    raise OmasErrorValue("Set elements must be of Subclasses of Xsd.")
+        else:
+            if isinstance(value, Xsd):
+                self.__data.add(value)
+            else:
                 raise OmasErrorValue("Set elements must be of Subclasses of Xsd.")
-            self.__data.add(val)
+            for arg in args:
+                if not isinstance(arg, Xsd):
+                    raise OmasErrorValue("Set elements must be of Subclasses of Xsd.")
+                self.__data.add(arg)
 
-    def __eq__(self, other: Self | Set[Xsd] | None) -> bool:
+    def __eq__(self, other: Self | set[Xsd] | None) -> bool:
         if other is None:
             return False
         if isinstance(other, RdfSet):
             return self.__data == other.__data
         elif isinstance(other, set):
             return self.__data == other
         else:
```

### Comparing `omaslib-0.1.8/omaslib/src/enums/action.py` & `omaslib-0.1.9/omaslib/src/enums/action.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/enums/language.py` & `omaslib-0.1.9/omaslib/src/enums/language.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/enums/permissions.py` & `omaslib-0.1.9/omaslib/src/enums/permissions.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/enums/propertyclassattr.py` & `omaslib-0.1.9/omaslib/src/enums/propertyclassattr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import unique, Enum
 
 
 @unique
-class PropertyClassAttribute(Enum):
+class PropClassAttr(Enum):
     """
     Enumeration of all the attributes of a property. Please note that the `omas:restriction` attribute
     itself is a complex onbject defining restrictions to the property.
     The following attributes are defined:
 
     - `PropertyClassAttribute.SUBPROPERTY_OF`: The given property is a specialization of the property given here
     - `PropertyClassAttribute.PROPERTY_OF`: The given property is either a `owl:ObjectProperty` or
```

### Comparing `omaslib-0.1.8/omaslib/src/enums/propertyrestrictiontype.py` & `omaslib-0.1.9/omaslib/src/enums/propertyrestrictiontype.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/enums/sparql_result_format.py` & `omaslib-0.1.9/omaslib/src/enums/sparql_result_format.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/enums/xsd_datatypes.py` & `omaslib-0.1.9/omaslib/src/enums/xsd_datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,18 @@
     unsignedShort = 'xsd:unsignedShort'
     unsignedByte = 'xsd:unsignedByte'
     positiveInteger = 'xsd:positiveInteger'
 
     def __str__(self):
         return self.value
 
+    @property
+    def toRdf(self):
+        return self.value
+
 
 @strict
 class IriValidator:
     """
     Calls to validate the syntax of an IRI
     """
     @classmethod
```

### Comparing `omaslib-0.1.8/omaslib/src/helpers/Notify.py` & `omaslib-0.1.9/omaslib/src/helpers/Notify.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from typing import Callable, Optional, Union
 
 from pystrict import strict
 
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_qname import Xsd_QName
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.enums.resourceclassattr import ResourceClassAttribute
 
 
 @strict
 class Notify:
     """
     This class can be used as super-class for a classes used as real (sh:name, sh:description) or
     virtual (Restrictions) props of a PropertyClass. It allows these non-primitive values such
     as of type LangString or PropertyRestriction to notify PropertyClass that something has changed,
     e.g. the change of value
     """
-    _notifier: Callable[[PropertyClassAttribute], None]
-    _data: PropertyClassAttribute
+    _notifier: Callable[[PropClassAttr], None]
+    _data: PropClassAttr
 
     def __init__(self,
-                 notifier: Optional[Callable[[Union[PropertyClassAttribute, ResourceClassAttribute, Xsd_QName]], None]],
-                 data: Union[PropertyClassAttribute, ResourceClassAttribute, Xsd_QName, None] = None):
+                 notifier: Optional[Callable[[Union[PropClassAttr, ResourceClassAttribute, Xsd_QName]], None]],
+                 data: Union[PropClassAttr, ResourceClassAttribute, Xsd_QName, None] = None):
         """
         Constructor of the notifier. Usually, the notifier is only used a base class and not used directly.
         :param notifier: The callable that is to be called by the subclass when an item is beeing chaged
         :param data: Arbitrary data that will be given to the callback
         """
         self._notifier = notifier
         self._data = data
 
     def set_notifier(self,
-                     notifier: Callable[[Union[PropertyClassAttribute, ResourceClassAttribute, Xsd_QName]], None],
-                     data: Union[PropertyClassAttribute, ResourceClassAttribute, Xsd_QName, None] = None) -> None:
+                     notifier: Callable[[Union[PropClassAttr, ResourceClassAttribute, Xsd_QName]], None],
+                     data: PropClassAttr | ResourceClassAttribute | Iri | Xsd_QName | None = None) -> None:
         """
         Sets the notifier callback function and the data it should return...
         :param notifier: A callable that is to be called by the subclass when an item changes
         :param data: Data to be given to the callback
         :return: None
         """
         self._notifier = notifier
```

### Comparing `omaslib-0.1.8/omaslib/src/helpers/context.py` & `omaslib-0.1.9/omaslib/src/helpers/context.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/langstring.py` & `omaslib-0.1.9/omaslib/src/helpers/langstring.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 """
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Dict, List, Optional, Callable, Self
 
 from pystrict import strict
 
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.Notify import Notify
 from omaslib.src.enums.action import Action
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.omaserror import OmasError
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.helpers.serializer import serializer
+from omaslib.src.xsd.xsd_string import Xsd_string
 
 
 @dataclass
 class LangStringChange:
     old_value: str | None
     action: Action
 
@@ -68,16 +71,16 @@
     _priorities: List[Language]
     _changeset: Dict[Language, LangStringChange]
     _notifier: Callable[[type], None] | None
 
     def __init__(self,
                  langstring: Optional[str | List[str] | Dict[str, str] | Dict[Language, str]] = None,
                  priorities: Optional[List[Language]] = None,
-                 notifier: Optional[Callable[[PropertyClassAttribute], None]] = None,
-                 notify_data: Optional[PropertyClassAttribute] = None):
+                 notifier: Optional[Callable[[PropClassAttr], None]] = None,
+                 notify_data: Optional[PropClassAttr] = None):
         """
         Implements language dependent strings.
 
         The parameter `langstring`can either be
 
         - a string in the form `"string@ll"`, eg `"Lastname@en"`. A string without language qualifier has the
             language `Language.XX` associated.
@@ -249,22 +252,27 @@
         :return: language string
         :rtype: str
         """
         if isinstance(lang, str):
             lang = Language[lang.upper()]
         return self._langstring.get(lang, default)
 
-    def __eq__(self, other: Self) -> bool:
+    def __bool__(self) -> bool:
+        return len(self._langstring) > 0
+
+    def __eq__(self, other: Self | None) -> bool:
         """
         Test for equality of two language strings
         :param other: The other Language string to compare to
         :type other: LanguageString
         :return: True or False
         :rtype: bool
         """
+        if other is None:
+            return False
         if len(self._langstring) != len(other._langstring):
             return False
         for lang in self._langstring:
             if other.langstring.get(lang) is None:
                 return False
             if self._langstring.get(lang) != other.langstring.get(lang):
                 return False
@@ -300,28 +308,28 @@
         """
         All language strings as Dict
         :return: A dictionary of all language strings
         :rtype: Dict
         """
         return self._langstring
 
-    def add(self, langs: str | List[str] | Dict[str, str] | Dict[Language, str]) -> None:
+    def add(self, langs: str | Xsd_string | List[str | Xsd_string | StringLiteral] | Dict[str, str] | Dict[Language, str]) -> None:
         """
         Add one or several new languages to a lang string. The method accepts several forms:
         * ``mylstr.add("a new string@en")``
         * ``mylstr.add(["a new string@en", "eine neue Zeichenketter@de])``
         * ``mylstr.add({"fr": "Nouveau", "de": "Neue Zeichenketter"})``
         * ``mylstr.add({Language.FR: "Nouveau", Language.DE: "Neue Zeichenketter"})
         As this, it's a very versatile method for adding new languages to a LanguageString instance
         :param langs: The language/string pairs as single value, list or dict
         :type langs: str | List[str] | Dict[str, str] | Dict[Language, str]
         :return: No return value
         :rtype: None
         """
-        if isinstance(langs, str):
+        if isinstance(langs, (str, Xsd_string)):
             if langs[-3] == "@":
                 lstr = langs[-2:].upper()
                 lobj = None
                 try:
                     lobj = Language[lstr]
                 except KeyError:
                     raise OmasError(f'Language "{lstr}" is invalid')
@@ -335,32 +343,39 @@
                 if self._changeset.get(Language.XX) is None:  # only the first change is recorded
                     self._changeset[Language.XX] = LangStringChange(self._langstring.get(Language.XX),
                                                                     Action.REPLACE if self._langstring.get(Language.XX) is not None else Action.CREATE)
                 self._langstring[Language.XX] = langs
             self.notify()
         elif isinstance(langs, List):
             for lang in langs:
-                if lang[-3] == "@":
-                    lstr = lang[-2:].upper()
-                    lobj = None
-                    try:
-                        lobj = Language[lstr]
-                    except KeyError:
-                        raise OmasError(f'Language "{lstr}" is invalid')
-                    if self._changeset.get(lobj) is None:  # only the first change is recorded
-                        self._changeset[lobj] = LangStringChange(self._langstring.get(lobj),
-                                                                 Action.REPLACE if self._langstring.get(lobj) is not None else Action.CREATE)
-                    self._langstring[lobj] = lang[:-3]
-                    self.notify()
+                if isinstance(lang, StringLiteral):
+                    if self._changeset.get(lang.lang) is None:  # only the first change is recorded
+                        self._changeset[lang.lang] = LangStringChange(self._langstring.get(lang.lang),
+                                                                      Action.REPLACE if self._langstring.get(lang.lang) is not None else Action.CREATE)
+                    self._langstring[lang.lang] = lang.value
+                elif isinstance(lang, (str, Xsd_string)):
+                    if lang[-3] == "@":
+                        lstr = lang[-2:].upper()
+                        lobj = None
+                        try:
+                            lobj = Language[lstr]
+                        except KeyError:
+                            raise OmasError(f'Language "{lstr}" is invalid')
+                        if self._changeset.get(lobj) is None:  # only the first change is recorded
+                            self._changeset[lobj] = LangStringChange(self._langstring.get(lobj),
+                                                                     Action.REPLACE if self._langstring.get(lobj) is not None else Action.CREATE)
+                        self._langstring[lobj] = lang[:-3]
+                    else:
+                        lobj = Language.XX
+                        if self._changeset.get(lobj) is None:  # only the first change is recorded
+                            self._changeset[lobj] = LangStringChange(self._langstring.get(lobj),
+                                                                     Action.REPLACE if self._langstring.get(lobj) is not None else Action.CREATE)
+                        self._langstring[lobj] = lang
                 else:
-                    lobj = Language.XX
-                    if self._changeset.get(lobj) is None:  # only the first change is recorded
-                        self._changeset[lobj] = LangStringChange(self._langstring.get(lobj),
-                                                                 Action.REPLACE if self._langstring.get(lobj) is not None else Action.CREATE)
-                    self._langstring[lobj] = lang
+                    raise OmasError(f'Inconsistent LangString (lang="{lang}", type="{type(lang).__name__}")')
             self.notify()
         elif isinstance(langs, Dict):
             for lang, value in langs.items():
                 lobj = None
                 if isinstance(lang, Language):
                     lobj = lang
                 else:
@@ -404,68 +419,68 @@
         :return: Nothing
         :rtype: None
         """
         self._changeset = {}
 
     def create(self, *,
                graph: Xsd_QName,
-               subject: Xsd_QName | Xsd_anyURI,
+               subject: Iri,
                field: Xsd_QName,
                indent: int = 0, indent_inc: int = 4):
         blank = ''
         sparql_list = []
         sparql = ''
         sparql += f'{blank:{indent * indent_inc}}INSERT DATA {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH {graph} {{\n'
-        sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.resUri} {field.toRdf} {self.toRdf} .\n'
+        sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.toRdf} {field.toRdf} {self.toRdf} .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         return sparql
 
     def delete(self, *,
                graph: Xsd_QName,
-               subject: Xsd_QName | Xsd_anyURI,
+               subject: Iri,
                field: Xsd_QName,
                indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql_list = []
         sparql = ''
         sparql += f'{blank:{indent * indent_inc}}DELETE WHERE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH {graph} {{\n'
-        sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.resUri} {field.toRdf} ?o .\n'
+        sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.toRdf} {field.toRdf} ?o .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         return sparql
 
     def update(self, *,
                graph: Xsd_QName,
-               subject: Xsd_QName | Xsd_anyURI,
+               subject: Iri,
                subjectvar: str,
                field: Xsd_QName,
                indent: int = 0, indent_inc: int = 4) -> List[str]:
         blank = ''
         sparql_list = []
         for lang, change in self._changeset.items():
             if change.action != Action.CREATE:
                 sparql = f'{blank:{indent * indent_inc}}DELETE DATA {{\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH {graph} {{\n'
                 tmpstr = f'"{change.old_value}"'
                 if lang != Language.XX:
                     tmpstr += "@" + lang.name.lower()
-                sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.resUri} {field.toRdf} {tmpstr} .\n'
+                sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.toRdf} {field.toRdf} {tmpstr} .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 sparql_list.append(sparql)
             if change.action != Action.DELETE:
                 sparql = f'{blank:{indent * indent_inc}}INSERT DATA {{\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH {graph} {{\n'
                 langstr = f'"{self._langstring[lang]}"'
                 if lang != Language.XX:
                     langstr += "@" + lang.name.lower()
-                sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.resUri} {field.toRdf} {langstr} .\n'
+                sparql += f'{blank:{(indent + 2) * indent_inc}}{subject.toRdf} {field.toRdf} {langstr} .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 sparql_list.append(sparql)
 
             # sparql = ''
             # sparql += f'{blank:{indent * indent_inc}}WITH {graph}\n'
             # if change.action != Action.CREATE:
@@ -493,17 +508,17 @@
             #     sparql += f'{blank:{(indent + 1) * indent_inc}}{subjectvar} {repr(field)} {tmpstr} .\n'
             # sparql += f'{blank:{indent * indent_inc}}}}'
             # sparql_list.append(sparql)
         return sparql_list
 
     def update_shacl(self, *,
                      graph: Xsd_NCName,
-                     owlclass_iri: Optional[Xsd_QName] = None,
-                     prop_iri: Xsd_QName,
-                     attr: PropertyClassAttribute,
+                     owlclass_iri: Iri | None = None,
+                     prop_iri: Iri,
+                     attr: PropClassAttr,
                      modified: Xsd_dateTime,
                      indent: int = 0, indent_inc: int = 4) -> str:
         """
         Return the SPARQL code piece that updates a Language string SHACL part of the triple store.
         :param graph: SPARQL graph as described in the introduction to OMASLIB
         :type graph: Xsd_NCName
         :param owlclass_iri: The OWL class IRI of the associated ResourceClass. May be omitted for standalone properties
@@ -542,15 +557,15 @@
                     langstr += "@" + lang.name.lower()
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {attr.value} {langstr} .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
 
             sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
             if owlclass_iri:
                 sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri}Shape sh:property ?prop .\n'
-                sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri} .\n'
+                sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri.toRdf} .\n'
             else:
                 sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri}Shape as ?prop) .\n'
             if change.action != Action.CREATE:
                 tmpstr = f'"{change.old_value}"'
                 if lang != Language.XX:
                     tmpstr += "@" + lang.name.lower()
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {attr.value} {tmpstr} .\n'
@@ -559,17 +574,17 @@
             sparql += f'{blank:{indent * indent_inc}}}}'
             sparql_list.append(sparql)
         sparql = ";\n".join(sparql_list)
         return sparql
 
     def delete_shacl(self, *,
                      graph: Xsd_NCName,
-                     owlclass_iri: Optional[Xsd_QName] = None,
-                     prop_iri: Xsd_QName,
-                     attr: Xsd_QName,
+                     owlclass_iri: Iri | None = None,
+                     prop_iri: Iri,
+                     attr: PropClassAttr,
                      modified: datetime,
                      indent: int = 0, indent_inc: int = 4) -> str:
         # TODO: Include into unit tests!
         """
         Return the SPARQL code piece that deletes an LanguageString
         :param graph: SPARQL graph as described in the introduction to OMASLIB
         :type graph: Xsd_NCName
@@ -585,31 +600,33 @@
         :type indent: int
         :param indent_inc: The indent increment for the generated SPARQL code
         :type indent_inc: int
         :return: Piece of SPARQL code that deletes the Language String from the SHACL definition
         :rtype: str
         """
         blank = ''
-        sparql = f'#\n# Deleting the complete LangString data for {prop_iri} {attr}\n#\n'
+        sparql = f'#\n# Deleting the complete LangString data for {prop_iri} {attr.value}\n#\n'
         sparql += f'{blank:{indent * indent_inc}}WITH {graph}:shacl'
         sparql += f'{blank:{indent * indent_inc}}DELETE {{'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {attr} ?langval'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {attr.value} ?langval'
         sparql += f'{blank:{indent * indent_inc}}}}'
         sparql += f'{blank:{indent * indent_inc}}WHERE {{'
         if owlclass_iri:
             sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri}Shape sh:property ?prop .\n'
-            sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri} .\n'
+            sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri.toRdf} .\n'
         else:
             sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri}Shape as ?prop)\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {attr} ?langval'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {attr.value} ?langval'
         sparql += f'{blank:{indent * indent_inc}}}}'
         return sparql
 
 
 if __name__ == '__main__':
+    l0 = LangString()
+    print(l0)
     ls1 = LangString("gaga")
     print(str(ls1))
     ls2 = LangString({
         Language.DE: "Deutsch....",
         Language.EN: "German...."
     })
     print(str(ls2))
```

### Comparing `omaslib-0.1.8/omaslib/src/helpers/observable_dict.py` & `omaslib-0.1.9/omaslib/src/helpers/observable_dict.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/observable_set.py` & `omaslib-0.1.9/omaslib/src/helpers/observable_set.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/oldap_string_literal.py` & `omaslib-0.1.9/omaslib/src/dtypes/string_literal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Optional, Self
 from pystrict import strict
 
 from omaslib.src.enums.language import Language
+from omaslib.src.helpers.omaserror import OmasErrorValue
 from omaslib.src.helpers.serializer import serializer
 
 
 @strict
 @serializer
-class OldapStringLiteral:
+class StringLiteral:
     """
     # OoldapStringLiteral class
 
     This class implements the handling of a single RDF/TRIG string that may have a language tag. It is
     serializable and manages the escaping/un-escaing of strings transfered to the triple store. This is
     an important part of the security conecpt of OLDAP.
 
@@ -76,28 +77,31 @@
         :param lang: Language the sting is in [optional]
         :type lang: str | Language
         """
         self.__value = value
         if isinstance(lang, Language):
             self.__lang = lang
         else:
-            self.__lang = Language[lang.upper()] if lang else None
+            try:
+                self.__lang = Language[lang.upper()] if lang else None
+            except ValueError as err:
+                raise OmasErrorValue(str(err))
 
     @classmethod
     def fromRdf(cls, value: str, lang: Optional[str] = None):
         """
         Constructor of OldapStringLiteral that takes a RDF/SPARQL representation of the string and un-escapes it
         :param value: String from RDF/SPARQL representation
         :type value: str
         :param lang: Language ISO short (lowercased) [optional]
         :type lang: str
         :return: OldapStringLiteral instance
-        :rtype: OldapStringLiteral
+        :rtype: StringLiteral
         """
-        value = OldapStringLiteral.unescaping(value)
+        value = StringLiteral.unescaping(value)
         return cls(value, lang)
 
     def __str__(self) -> str:
         """
         Returns the string representation of the OldapStringLiteral instance with the languages appended "@ll"
         :return: Language string
         :rtype: str
@@ -110,27 +114,27 @@
     def __repr__(self) -> str:
         """
         Returns the OldapStringLiteral instance as string as used in a RDF/SPARQL representation
         :return: SPARQL/RDF/TRIG representation of the language string
         :rtype: str
         """
         if self.__lang:
-            return f'"{OldapStringLiteral.escaping(self.__value)}"@{self.__lang.name.lower()}'
+            return f'"{StringLiteral.escaping(self.__value)}"@{self.__lang.name.lower()}'
         else:
-            return f'"{OldapStringLiteral.escaping(self.__value)}"'
+            return f'"{StringLiteral.escaping(self.__value)}"'
 
     def __eq__(self, other: str | Self) -> bool:
         """
         Check for equality of two OldapStringLiterals (both strings and languages must be equal)
         :param other: Other OldapStringLiteral
-        :type other: OldapStringLiteral
+        :type other: StringLiteral
         :return: True or False
         :rtype: bool
         """
-        if isinstance(other, OldapStringLiteral):
+        if isinstance(other, StringLiteral):
             return self.__value == other.__value and self.__lang == other.__lang
         elif isinstance(other, str):
             return self.__value == other
 
     def __hash__(self) -> int:
         """
         Returns the OldapStringLiteral hash value as an integer
@@ -138,14 +142,21 @@
         :rtype: int
         """
         if self.__lang:
             return hash(self.__value + '@' + self.__lang.value)
         else:
             return hash(self.__value)
 
+    @property
+    def toRdf(self):
+        if self.__lang:
+            return f'"{StringLiteral.escaping(self.__value)}"@{self.__lang.name.lower()}'
+        else:
+            return f'"{StringLiteral.escaping(self.__value)}"^^xsd:string'
+
     def _as_dict(self) -> dict:
         """
         Used for the JSON serializer
         :return: Dictionary representation of the OldapStringLiteral
         :rtype: Dict[str,str]
         """
         return {
```

### Comparing `omaslib-0.1.8/omaslib/src/helpers/omaserror.py` & `omaslib-0.1.9/omaslib/src/helpers/omaserror.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/propertyclass_singleton.py` & `omaslib-0.1.9/omaslib/src/helpers/propertyclass_singleton.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/query_processor.py` & `omaslib-0.1.9/omaslib/src/helpers/query_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from dataclasses import dataclass
-from datetime import datetime, time, date, timedelta
 from typing import List, Dict
 
-from isodate import Duration
 from pystrict import strict
 
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.context import Context
 from omaslib.src.dtypes.bnode import BNode
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
+from omaslib.src.xsd.xsd_gmonthday import Xsd_gMonthDay
+from omaslib.src.xsd.xsd_id import Xsd_ID
+from omaslib.src.xsd.xsd_idref import Xsd_IDREF
 from omaslib.src.xsd.xsd_name import Xsd_name
 from omaslib.src.xsd.xsd_nmtoken import Xsd_NMTOKEN
 from omaslib.src.xsd.xsd_positiveinteger import Xsd_positiveInteger
 from omaslib.src.xsd.xsd_unsignedbyte import Xsd_unsignedByte
 from omaslib.src.xsd.xsd_unsignedshort import Xsd_unsignedShort
 from omaslib.src.xsd.xsd_unsignedint import Xsd_unsignedInt
 from omaslib.src.xsd.xsd_unsignedlong import Xsd_unsignedLong
@@ -43,15 +45,15 @@
 from omaslib.src.xsd.xsd_double import Xsd_double
 from omaslib.src.xsd.xsd_float import Xsd_float
 from omaslib.src.xsd.xsd_decimal import Xsd_decimal
 from omaslib.src.xsd.xsd_string import Xsd_string
 from omaslib.src.xsd.xsd_boolean import Xsd_boolean
 from omaslib.src.xsd.xsd import Xsd
 
-RowElementType = bool | int | float | str | datetime | time | date | Duration | timedelta | Xsd_QName | BNode | Xsd_anyURI | Xsd_NCName | OldapStringLiteral | Xsd
+RowElementType = Xsd | BNode | StringLiteral
 RowType = Dict[str, RowElementType]
 
 
 @dataclass
 @strict
 class QueryProcessor:
     __names: List[str]
@@ -64,24 +66,26 @@
         self.__pos = 0
         self.__rows = []
         self.__names = query_result["head"]["vars"]
         for tmprow in query_result["results"]["bindings"]:
             row: Dict[str, RowElementType] = {}
             for name, valobj in tmprow.items():
                 if valobj["type"] == "uri":
-                    row[name] = context.iri2qname(valobj["value"])
-                    if row[name] is None:
-                        row[name] = Xsd_anyURI(valobj["value"])
+                    tmp = context.iri2qname(valobj["value"])
+                    if tmp is None:
+                        row[name] = Iri(valobj["value"])
+                    else:
+                        row[name] = Iri(tmp)
                 elif valobj["type"] == "bnode":
                     row[name] = BNode(f'_:{valobj["value"]}')
                 elif valobj["type"] == "literal":
                     dt = valobj.get("datatype")
                     if dt is None:
                         if valobj.get("xml:lang") is not None:
-                            row[name] = OldapStringLiteral.fromRdf(valobj["value"], valobj.get("xml:lang"))
+                            row[name] = StringLiteral.fromRdf(valobj["value"], valobj.get("xml:lang"))
                         else:
                             row[name] = Xsd_string.fromRdf(valobj["value"])
                     else:
                         dt = context.iri2qname(dt)
                         match str(dt):
                             case 'xsd:string':
                                 row[name] = Xsd_string.fromRdf(valobj["value"])
@@ -107,14 +111,20 @@
                                 row[name] = Xsd_gYearMonth.fromRdf(valobj["value"])
                             case 'xsd:gYear':
                                 row[name] = Xsd_gYear.fromRdf(valobj["value"])
                             case 'xsd:gDay':
                                 row[name] = Xsd_gDay.fromRdf(valobj["value"])
                             case 'xsd:gMonth':
                                 row[name] = Xsd_gMonth.fromRdf(valobj["value"])
+                            case 'xsd:gMonthDay':
+                                row[name] = Xsd_gMonthDay.fromRdf(valobj["value"])
+                            case 'xsd:ID':
+                                row[name] = Xsd_ID.fromRdf(valobj["value"])
+                            case 'xsd:IDREF':
+                                row[name] = Xsd_IDREF.fromRdf(valobj["value"])
                             case 'xsd:hexBinary':
                                 row[name] = Xsd_hexBinary.fromRdf(valobj["value"])
                             case 'xsd:base64Binary':
                                 row[name] = Xsd_base64Binary.fromRdf(valobj["value"])
                             case 'xsd:anyURI':
                                 row[name] = Xsd_anyURI.fromRdf(valobj["value"])
                             case 'xsd:QName':
@@ -153,18 +163,16 @@
                                 row[name] = Xsd_unsignedInt(valobj["value"])
                             case 'xsd:unsignedShort':
                                 row[name] = Xsd_unsignedShort(valobj["value"])
                             case 'xsd:unsignedByte':
                                 row[name] = Xsd_unsignedByte(valobj["value"])
                             case 'xsd:positiveInteger':
                                 row[name] = Xsd_positiveInteger(valobj["value"])
-                            case 'xsd:dateTime':
-                                row[name] = datetime.fromisoformat(valobj["value"])
                             case _:
-                                row[name] = str(valobj["value"])
+                                row[name] = Xsd_string(valobj["value"])
             self.__rows.append(row)
 
     def __len__(self) -> int:
         return len(self.__rows)
 
     def __iter__(self):
         self.__pos = 0
```

### Comparing `omaslib-0.1.8/omaslib/src/helpers/semantic_version.py` & `omaslib-0.1.9/omaslib/src/helpers/semantic_version.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/serializer.py` & `omaslib-0.1.9/omaslib/src/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/helpers/tools.py` & `omaslib-0.1.9/omaslib/src/helpers/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import re
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional, List, Tuple, Union
 
 from omaslib.src.enums.action import Action
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
+from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 
 
 def lprint(text: str):
     lines = text.split('\n')
     for i, line in enumerate(lines, start=1):
         print(f"{i}: {line}")
 
 
-def str2qname_anyiri(s: str) -> Xsd_QName | Xsd_anyURI:
+def str2qname_anyiri(s: Xsd_QName | Xsd_anyURI | str) -> Xsd_QName | Xsd_anyURI:
     try:
         return Xsd_QName(s)
     except:
         return Xsd_anyURI(s)
 
 
 @dataclass
@@ -100,22 +101,23 @@
 
 class RdfModifyProp:
 
     @classmethod
     def __rdf_modify_property(cls, *,
                               shacl: bool,
                               action: Action,
-                              owlclass_iri: Optional[Xsd_QName] = None,
+                              owlclass_iri: Xsd_QName | None = None,
                               pclass_iri: Xsd_QName,
                               graph: Xsd_QName,
                               ele: RdfModifyItem,
-                              last_modified: datetime,
+                              last_modified: Xsd_dateTime,
                               indent: int = 0, indent_inc: int = 4) -> str:
-        sparql = f'WITH {graph}\n'
-        blank = ' '
+        blank = ''
+        sparql = f'# __rdf_modify_property of "{pclass_iri}"\n'
+        sparql += f'WITH {graph}\n'
         if action != Action.CREATE:
             sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {ele.property} {ele.old_value} .\n'
             sparql += f'{blank:{indent * indent_inc}}}}\n'
 
         if action != Action.DELETE:
             sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
@@ -134,75 +136,75 @@
                 sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({pclass_iri}Shape as ?prop)\n'
             else:
                 sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({pclass_iri} as ?prop)\n'
         if action != Action.CREATE:
             sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {ele.property} {ele.old_value} .\n'
         if ele.property != 'dcterms:modified':
             sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified ?modified .\n'
-            sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {repr(last_modified)})\n'
+            sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {last_modified.toRdf})\n'
         sparql += f'{blank:{indent * indent_inc}}}}'
         return sparql
 
     @classmethod
     def shacl(cls, *,
               action: Action,
               graph: Xsd_NCName,
-              owlclass_iri: Optional[Xsd_QName] = None,
+              owlclass_iri: Xsd_QName | None = None,
               pclass_iri: Xsd_QName,
               ele: RdfModifyItem,
-              last_modified: datetime,
+              last_modified: Xsd_dateTime,
               indent: int = 0, indent_inc: int = 4) -> str:
         graph = Xsd_QName(str(graph) + ':shacl')
         return cls.__rdf_modify_property(shacl=True, action=action, owlclass_iri=owlclass_iri,
                                          pclass_iri=pclass_iri, graph=graph, ele=ele, last_modified=last_modified,
                                          indent=indent, indent_inc=indent_inc)
 
     @classmethod
     def onto(cls, *,
              action: Action,
              graph: Xsd_NCName,
              owlclass_iri: Optional[Xsd_QName] = None,
              pclass_iri: Xsd_QName,
              ele: RdfModifyItem,
-             last_modified: datetime,
+             last_modified: Xsd_dateTime,
              indent: int = 0, indent_inc: int = 4) -> str:
         graph = Xsd_QName(str(graph) + ':onto')
         return cls.__rdf_modify_property(shacl=False, action=action, owlclass_iri=owlclass_iri,
                                          pclass_iri=pclass_iri, graph=graph, ele=ele, last_modified=last_modified,
                                          indent=indent, indent_inc=indent_inc)
 
 
 class DataModelModtime:
 
     @classmethod
-    def __set_dm_modtime(cls, shacl: bool, graph: Xsd_NCName, timestamp: datetime, contributor: str) -> str:
+    def __set_dm_modtime(cls, shacl: bool, graph: Xsd_NCName, timestamp: Xsd_dateTime, contributor: Xsd_QName | Xsd_anyURI) -> str:
         graphname = f"{graph}:shacl" if shacl else f"{graph}:onto"
         element = f"{graph}:shapes" if shacl else f"{graph}:ontology"
         return f"""
         DELETE {{
             GRAPH {graphname} {{ {element} dcterms:modified ?value . }}
         }}
         INSERT {{
-            GRAPH {graphname} {{ {element} dcterms:modified "{timestamp.isoformat()}"^^xsd:dateTime . }}
+            GRAPH {graphname} {{ {element} dcterms:modified {timestamp.toRdf} . }}
         }}
         WHERE {{
             GRAPH {graphname} {{ {element} dcterms:modified ?value . }}
         }} ;
         DELETE {{
             GRAPH {graphname} {{ {element} dcterms:contributor ?value . }}
         }}
         INSERT {{
-            GRAPH {graphname} {{ {element} dcterms:contributor "{contributor}" . }}
+            GRAPH {graphname} {{ {element} dcterms:contributor "{contributor.resUri}" . }}
         }}
         WHERE {{
             GRAPH {graphname} {{ {element} dcterms:contributor ?value . }}
         }}
         """
 
     @classmethod
-    def set_dm_modtime_shacl(cls, graph: Xsd_NCName, timestamp: datetime, contributor: str) -> str:
+    def set_dm_modtime_shacl(cls, graph: Xsd_NCName, timestamp: Xsd_dateTime, contributor: Xsd_QName | Xsd_anyURI) -> str:
         return cls.__set_dm_modtime(True, graph, timestamp, contributor)
 
     @classmethod
-    def set_dm_modtime_onto(cls, graph: Xsd_NCName, timestamp: datetime, contributor: str) -> str:
+    def set_dm_modtime_onto(cls, graph: Xsd_NCName, timestamp: Xsd_dateTime, contributor: Xsd_QName | Xsd_anyURI) -> str:
         return cls.__set_dm_modtime(False, graph, timestamp, contributor)
```

### Comparing `omaslib-0.1.8/omaslib/src/iconnection.py` & `omaslib-0.1.9/omaslib/src/iconnection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Any, Dict
 
 from pystrict import strict
 
 from omaslib.src.helpers.context import DEFAULT_CONTEXT
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.enums.sparql_result_format import SparqlResultFormat
 from omaslib.src.user_dataclass import UserDataclass
 
 
@@ -30,15 +31,15 @@
         return self._userdata
 
     @property
     def userid(self) -> Xsd_NCName:
         return self._userdata.userId
 
     @property
-    def userIri(self) -> Xsd_anyURI:
+    def userIri(self) -> Iri:
         return self._userdata.userIri
 
     @property
     def login(self) -> bool:
         return self._userIri is not None
 
     @property
```

### Comparing `omaslib-0.1.8/omaslib/src/in_project.py` & `omaslib-0.1.9/omaslib/src/in_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """
 # InProject Class
 
 The InProject class is a helper class that is used to record the per-project administrative permissions for
 a particular user. It's not meant to be used without the context of a user, that is as a _property_ of a User.
 """
-from copy import deepcopy
 from typing import Dict, Callable, Set, Self, ItemsView, KeysView
 
 from pystrict import strict
 
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.helpers.observable_set import ObservableSet
 from omaslib.src.enums.permissions import AdminPermission
 from omaslib.src.helpers.omaserror import OmasErrorValue, OmasErrorKey
 from omaslib.src.helpers.serializer import serializer
 import json
 
+
 @strict
 @serializer
 class InProjectClass:
     """
     Implements the administrative permission a user has for the projects the user is associated with.
     """
-    __data: Dict[Xsd_QName | Xsd_anyURI, ObservableSet[AdminPermission]]
-    __on_change: Callable[[Xsd_QName | Xsd_anyURI, ObservableSet[AdminPermission] | None], None] | None
+    __data: Dict[Iri, ObservableSet[AdminPermission]]
+    __on_change: Callable[[Iri, ObservableSet[AdminPermission] | None], None] | None
 
     def __init__(self,
-                 data: Self | Dict[Xsd_QName | Xsd_anyURI | str, set[AdminPermission | str] | ObservableSet[AdminPermission]] | None = None,
-                 on_change: Callable[[Xsd_QName | Xsd_anyURI, ObservableSet[AdminPermission] | None], None] = None) -> None:
+                 data: Self | Dict[Iri | str, set[AdminPermission | str] | ObservableSet[AdminPermission]] | None = None,
+                 on_change: Callable[[Iri, ObservableSet[AdminPermission] | None], None] = None) -> None:
         """
         Constructor of the class. The class acts like a dictionary and allows the access to the permission
         set for a project using the QName of the project as the key: ```perms = t.in_project[QName('ex:proj')]```.
         It supports the getting, setting and deleting a permission set.
         In addition, the following methods are implemented:
 
         - _get()_: gets the permission set or returns `None`if it doesn't exist for the given project'
@@ -48,30 +49,20 @@
         self.__data = {}
         self.__on_change = None
         if data is not None:
             if isinstance(data, InProjectClass):
                 self.__data = data.__data
             else:
                 for key, value in data.items():
-                    key = self.__key(key)
+                    key = Iri(key)
                     self.__data[key] = self.__perms(key, value)
         self.__on_change = on_change
 
-    def __key(self, key: Xsd_QName | Xsd_anyURI | str) -> Xsd_QName | Xsd_anyURI:
-        if isinstance(key, str):
-            try:
-                key = Xsd_QName(key)
-            except OmasErrorValue:
-                key = Xsd_anyURI(key)
-        elif not isinstance(key, Xsd_QName) and not isinstance(key, Xsd_anyURI):
-            raise OmasErrorValue(f'{key} is not a valid XSD QName or XSD anyURI')
-        return key
-
     def __perms(self,
-                key: Xsd_QName | Xsd_anyURI,
+                key: Iri,
                 value: set[AdminPermission | str] | ObservableSet[AdminPermission] | None) -> ObservableSet[AdminPermission]:
         perms = ObservableSet(on_change=self.__on_set_changed, on_change_data=key)
         if value is None:
             return perms
         for permission in value:
             if isinstance(permission, str):
                 try:
@@ -83,58 +74,60 @@
                     raise OmasErrorValue(str(err))
             elif permission in AdminPermission:
                 perms.add(permission)
             else:
                 raise OmasErrorValue(f'{permission} is not a valid AdminPermission')
         return perms
 
-    def __on_set_changed(self, oldset: ObservableSet[AdminPermission], key: Xsd_QName | str):
+    def __on_set_changed(self, oldset: ObservableSet[AdminPermission], key: Iri | str):
         if self.__on_change is not None:
             self.__on_change(key, oldset) ## Action.MODIFY
 
-    def __getitem__(self, key: Xsd_QName | Xsd_anyURI | str) -> ObservableSet[AdminPermission]:
-        key = self.__key(key)
+    def __getitem__(self, key: Iri | str) -> ObservableSet[AdminPermission]:
+        if not isinstance(key, Iri):
+            key = Iri(key)
         try:
             return self.__data[key]
-        except KeyError as err:
+        except (KeyError, AttributeError) as err:
             raise OmasErrorKey(str(err), key)
 
-    def __setitem__(self, key: Xsd_QName | Xsd_anyURI, value: set[AdminPermission | str] | ObservableSet[AdminPermission]) -> None:
-        key = self.__key(key)
+    def __setitem__(self, key: Iri | str, value: set[AdminPermission | str] | ObservableSet[AdminPermission]) -> None:
+        if not isinstance(key, Iri):
+            key = Iri(key)
         if self.__data.get(key) is None:
             if self.__on_change is not None:
                 self.__on_change(key, None) ## Action.CREATE: Create a new inProject connection to a new project and add permissions
         else:
             if self.__on_change is not None:
                 self.__on_change(key, self.__data[key].copy())  ## Action.REPLACE Replace all the permission of the given connection to a project
         self.__data[key] = self.__perms(key, value)
 
-    def __delitem__(self, key: Xsd_QName | Xsd_anyURI | str) -> None:
-        key = self.__key(key)
+    def __delitem__(self, key: Iri | str) -> None:
+        if not isinstance(key, Iri):
+            key = Iri(key)
         if self.__data.get(key) is not None:
             if self.__on_change is not None:
                 self.__on_change(key, self.__data[key].copy())  ## Action.DELETE
             del self.__data[key]
         else:
             raise OmasErrorKey(f'Can\'t delete key "{key}" – does not exist')
 
-
     def __str__(self) -> str:
         s = ''
         for k, v in self.__data.items():
             l = [x.value for x in v]
             l.sort()
             s += f'{k} : {l}\n'
         return s
 
     def __bool__(self) -> bool:
         return bool(self.__data)
 
     def copy(self) -> Self:
-        data_copy: dict[Xsd_QName | Xsd_anyURI | str, set[AdminPermission | str] | ObservableSet[AdminPermission]] = {}
+        data_copy: dict[Iri, set[AdminPermission | str] | ObservableSet[AdminPermission]] = {}
         tmp = self.__on_change
         self.__on_change = None
         for key, val in self.__data.items():
             data_copy[key] = val
         self.__on_change = tmp
         return InProjectClass(data_copy, self.__on_change)
 
@@ -148,33 +141,32 @@
     def __ne__(self, other: Self | None) -> bool:
         if other is None:
             return True
         if not isinstance(other, InProjectClass):
             raise OmasErrorValue(f'"Other must be an instance of InProjectClass, not {type(other)}"')
         return self.__data != other.__data
 
-    def get(self, key: Xsd_anyURI | Xsd_QName) -> ObservableSet[AdminPermission] | None:
+    def get(self, key: Iri) -> ObservableSet[AdminPermission] | None:
         return self.__data.get(key)
 
-    def items(self) -> ItemsView[Xsd_anyURI | Xsd_QName, ObservableSet[AdminPermission]]:
+    def items(self) -> ItemsView[Iri, ObservableSet[AdminPermission]]:
         return self.__data.items()
 
     def keys(self) -> KeysView:
         return self.__data.keys()
 
     def _as_dict(self) -> dict:
         tmp = {f'{str(key)}': value for key, value in self.__data.items()}
-        #return {'data': self.__data}
         return {'data': tmp}
 
-    def add_admin_permission(self, project: Xsd_anyURI | Xsd_QName, permission: AdminPermission) -> None:
+    def add_admin_permission(self, project: Iri, permission: AdminPermission) -> None:
         pass
 
 
 if __name__ == '__main__':
-    in_proj = InProjectClass({Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+    in_proj = InProjectClass({Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                               AdminPermission.ADMIN_RESOURCES,
                                                               AdminPermission.ADMIN_CREATE}})
     jsonstr = json.dumps(in_proj, default=serializer.encoder_default)
     in_proj2 = json.loads(jsonstr, object_hook=serializer.decoder_hook)
     for k, v in in_proj2.items():
         print(f'{k} ({type(k)}) = {v}')
```

### Comparing `omaslib-0.1.8/omaslib/src/model.py` & `omaslib-0.1.9/omaslib/src/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 from typing import List, Set, Dict, Tuple, Optional, Any, Union
 
 from pystrict import strict
 
 from omaslib.src.helpers.context import Context
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.helpers.omaserror import OmasError, OmasErrorNotFound
 from omaslib.src.helpers.query_processor import QueryProcessor
 from omaslib.src.helpers.tools import lprint
 from omaslib.src.iconnection import IConnection
@@ -28,54 +29,55 @@
 
     def has_changed(self) -> bool:
         if self._changed:
             return True
         else:
             return False
 
-    def get_modified_by_iri(self, graph: Xsd_QName, iri: Xsd_anyURI | Xsd_QName) -> Xsd_dateTime:
+    def get_modified_by_iri(self, graph: Xsd_QName, iri: Iri) -> Xsd_dateTime:
         context = Context(name=self._con.context_name)
         sparql = context.sparql_context
         sparql += f"""
         SELECT ?modified
         FROM {graph}
         WHERE {{
-            {iri.resUri} dcterms:modified ?modified
+            {iri.toRdf} dcterms:modified ?modified
         }}
         """
         jsonobj = None
         if self._con.in_transaction():
             jsonobj = self._con.transaction_query(sparql)
         else:
             jsonobj = self._con.query(sparql)
         res = QueryProcessor(context, jsonobj)
         if len(res) != 1:
+            print(sparql)
             raise OmasErrorNotFound(f'No resource found with iri "{iri}".')
         for r in res:
             return r['modified']
 
     def set_modified_by_iri(self,
                             graph: Xsd_QName,
-                            iri: Xsd_anyURI | Xsd_QName,
+                            iri: Iri,
                             old_timestamp: Xsd_dateTime,
                             timestamp: Xsd_dateTime) -> None:
         context = Context(name=self._con.context_name)
         sparql = context.sparql_context
         sparql += f"""
         WITH {graph}
         DELETE {{
             ?res dcterms:modified {old_timestamp.toRdf} .
             ?res dcterms:contributor ?contributor .
         }}
         INSERT {{
             ?res dcterms:modified {timestamp.toRdf} .
-            ?res dcterms:contributor {self._con.userIri.resUri} .
+            ?res dcterms:contributor {self._con.userIri.toRdf} .
         }}
         WHERE {{
-            BIND({iri.resUri} as ?res)
+            BIND({iri.toRdf} as ?res)
             ?res dcterms:modified {old_timestamp.toRdf} .
             ?res dcterms:contributor ?contributor .
         }}
         """
         if self._con.in_transaction():
             self._con.transaction_update(sparql)
         else:
```

### Comparing `omaslib-0.1.8/omaslib/src/project.py` & `omaslib-0.1.9/omaslib/src/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 from typing import List, Dict, Optional, Self
 from datetime import date, datetime
 
 from omaslib.src.enums.permissions import AdminPermission
 from omaslib.src.helpers.context import Context
 from omaslib.src.enums.action import Action
 from omaslib.src.dtypes.namespaceiri import NamespaceIRI
+from omaslib.src.helpers.tools import lprint
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_date import Xsd_date
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd import Xsd
 from omaslib.src.helpers.langstring import LangString
 from omaslib.src.helpers.omaserror import OmasError, OmasErrorValue, OmasErrorAlreadyExists, OmasErrorNoPermission, \
     OmasErrorUpdateFailed, OmasErrorImmutable, OmasErrorNotFound
 from omaslib.src.helpers.query_processor import QueryProcessor
 from omaslib.src.iconnection import IConnection
 from omaslib.src.model import Model
 
-ProjectFieldTypes = Xsd_anyURI | Xsd_QName | Xsd_NCName | LangString | NamespaceIRI | Xsd | None
+ProjectFieldTypes = LangString | Xsd | None
 
 @dataclass
 class ProjectFieldChange:
     """
     A dataclass used to represent the changes made to a field.
     """
     old_value: ProjectFieldTypes
@@ -53,23 +55,24 @@
     # Project
 
     This class implements the Project model. A Project is a distinct research space within Oldap
     framework that offers dedicated space for data, its own data modeling and access control. A project
     needs the following metadata:
 
     - `projectIri`: The IRI that uniquely identifies this project. This can be an
-      [AnyIRI](/python_docstrings/datatypes#omaslib.src.helpers.datatypes.AnyIRI) or
+      [Iri](/python_docstrings/datatypes#omaslib.src.helpers.datatypes.Iri) instance or a string with either an Iri or Qname [mandatory]
       [QName](/python_docstrings/datatypes#omaslib.src.helpers.datatypes.QName).
     - `projectShortName`: The short name of the project that must be a NCName
-    - `label`: A multilingual string with a human-readable label for the project (`rdfs:label`)
-    - `comment`: A multilingual description of the project (`rdfs:comment`)
+    - `label`: A multilingual string with a human-readable label for the project (`rdfs:label`) [optional]
+    - `comment`: A multilingual description of the project (`rdfs:comment`) [optional]
     - `namespaceIri`: The namespace that the project uses for its data and data model. Must be
        a [NamespaceIRI](/python_docstrings/datatypes#omaslib.src.helpers.datatypes.NamespaceIRI).
-    - `projectStart`: The start date of the project.  Must be a Python `date` type.
-    - `projectEnd`: The optional end date of the project.Must be a Python `date` type.
+    - `projectStart`: The start date of the project.  Must be a Python `date` type. If not set,
+       the current date will be used. [optional]
+    - `projectEnd`: The optional end date of the project.Must be a Python `date` type. [optional]
 
     The class provides the following methods:
 
     - [Project(...)](/python_docstrings/project#omaslib.src.project.Project.__init__)): Constructor
     - [read(...)](/python_docstrings/project#omaslib.src.project.Project.read):
       Read project form triplestore and return a Project-instance
     - [search(...)](/python_docstrings/project#omaslib.src.project.Project.search):
@@ -98,65 +101,65 @@
     - `contributor`: The person which made the last changes to the project data. Must be a
       [AnyIRI](/python_docstrings/datatypes#omaslib.src.helpers.datatypes.AnyIRI) or
       [QName](/python_docstrings/datatypes#omaslib.src.helpers.datatypes.AnyIRI) [read only]
     - `modified`: The modification date of the project. Must be a Python `date` type [read only]
 
     """
     __datatypes = {
-        ProjectFields.PROJECT_IRI: {Xsd_anyURI, Xsd_QName},
+        ProjectFields.PROJECT_IRI: Iri,
         ProjectFields.PROJECT_SHORTNAME: Xsd_NCName,
         ProjectFields.LABEL: LangString,
         ProjectFields.COMMENT: LangString,
         ProjectFields.NAMESPACE_IRI: NamespaceIRI,
         ProjectFields.PROJECT_START: Xsd_date,
         ProjectFields.PROJECT_END: Xsd_date,
     }
 
-    __creator: Xsd_anyURI | None
+    __creator: Iri | None
     __created: Xsd_dateTime | None
-    __contributor: Xsd_anyURI | None
+    __contributor: Iri | None
     __modified: Xsd_dateTime | None
 
     __fields: Dict[ProjectFields, ProjectFieldTypes]
 
     __change_set: Dict[ProjectFields, ProjectFieldChange]
 
     def __init__(self, *,
                  con: IConnection,
-                 creator: Optional[Xsd_anyURI | Xsd_QName] = None,
-                 created: Optional[Xsd_dateTime] = None,
-                 contributor: Optional[Xsd_anyURI | Xsd_QName] = None,
-                 modified: Optional[Xsd_dateTime] = None,
-                 projectIri: Optional[Xsd_anyURI | Xsd_QName] = None,
+                 creator: Iri | None = None,
+                 created: Xsd_dateTime | None = None,
+                 contributor: Iri | None = None,
+                 modified: Xsd_dateTime | None = None,
+                 projectIri: Iri | str | None = None,
                  projectShortName: Xsd_NCName | str,
                  namespaceIri: NamespaceIRI,
-                 label: Optional[LangString | str],
-                 comment: Optional[LangString | str],
-                 projectStart: Optional[Xsd_date] = None,
-                 projectEnd: Optional[Xsd_date] = None):
+                 label: LangString | str | None = None,
+                 comment: LangString | str | None = None,
+                 projectStart: Xsd_date | None = None,
+                 projectEnd: Xsd_date | None = None):
         """
         Constructs a new Project
         :param con: [Connection](/python_docstrings/iconnection) instance
-        :param creator: Creator of the project  [Optional, usually not set!]
+        :param creator: Creator of the project  [DO NOT SET!]
         :type creator: Xsd_anyURI | None
-        :param created: Date the project was created  [Optional, usually not set!]
+        :param created: Date the project was created  [DO NOT SET!]
         :type created: datetime | None
-        :param contributor: person that made the last change  [Optional, usually not set!]
+        :param contributor: person that made the last change  [DO NOT SET!]
         :type contributor: Xsd_anyURI
-        :param modified: Last date the project was modified  [Optional, usually not set!]
+        :param modified: Last date the project was modified  [DO NOT SET!]
         :type modified: date | None
         :param projectIri: IRI to be used for the project. If no projectIRI is provied, the constrctor
-         will create an arbitrary IRI based on thr URN scheme and a UUID. [Optional].
-        :type projectIri: AnyIRI | Xsd_QName
+         will create an arbitrary IRI based on thr URN scheme and a UUID. [optional].
+        :type projectIri: Iri
         :param projectShortName: A short name for the project. Is used as prefix for named graphs that
-           are being used for the project.
+           are being used for the project. [mandatory]
         :type projectShortName: NCname (strings are accepted only if conform to NCName syntax)
-        :param namespaceIri: The namespace for the project
+        :param namespaceIri: The namespace to be used for the projects data [mandatory]
         :type namespaceIri: NamespaceIRI
-        :param label: Human-readable name for the project (multi-language) (`rdfs:label`)
+        :param label: Human-readable name for the project (multi-language) (`rdfs:label`) [optional]
         :type label: LangString
         :param comment: Description of the project (multi-language) (`rdfs:comment`)
         :type comment: LangString
         :param projectStart: Start date of the project
         :type projectStart: Python date
         :param projectEnd: End date of the project [Optional]
         :type projectEnd: Python date
@@ -169,22 +172,20 @@
         self.__contributor = contributor if contributor is not None else con.userIri
         if modified and not isinstance(modified, Xsd_dateTime):
             raise OmasErrorValue(f'Modified must be "Xsd_dateTime", not "{type(modified)}".')
         self.__modified = modified
         self.__fields = {}
 
         if projectIri:
-            if isinstance(projectIri, Xsd_anyURI):
-                self.__fields[ProjectFields.PROJECT_IRI] = projectIri
-            elif isinstance(projectIri, Xsd_QName):
-                self.__fields[ProjectFields.PROJECT_IRI] = projectIri
+            if not isinstance(projectIri, Iri):
+                self.__fields[ProjectFields.PROJECT_IRI] = Iri(projectIri)
             else:
-                raise OmasErrorValue(f'projectIri {projectIri} must be an instance of AnyIRI, not {type(projectIri)}')
+                self.__fields[ProjectFields.PROJECT_IRI] = projectIri
         else:
-            self.__fields[ProjectFields.PROJECT_IRI] = Xsd_anyURI(uuid.uuid4().urn)
+            self.__fields[ProjectFields.PROJECT_IRI] = Iri()
 
         self.__fields[ProjectFields.PROJECT_SHORTNAME] = projectShortName if isinstance(projectShortName, Xsd_NCName) else Xsd_NCName(projectShortName)
 
         if namespaceIri and isinstance(namespaceIri, NamespaceIRI):
             self.__fields[ProjectFields.NAMESPACE_IRI] = namespaceIri
         else:
             raise OmasErrorValue(f'Invalid namespace iri: {namespaceIri}')
@@ -209,15 +210,18 @@
             setattr(Project, name, property(
                 partial(Project.__get_value, field=field),
                 partial(Project.__set_value, field=field),
                 partial(Project.__del_value, field=field)))
         self.__change_set = {}
 
     def __get_value(self: Self, field: ProjectFields) -> ProjectFieldTypes | None:
-        return self.__fields.get(field)
+        tmp = self.__fields.get(field)
+        if not tmp:
+            return None
+        return tmp
 
     def __set_value(self: Self, value: ProjectFieldTypes, field: ProjectFields) -> None:
         self.__change_setter(field, value)
 
     def __del_value(self: Self, field: ProjectFields) -> None:
         del self.__fields[field]
 
@@ -227,15 +231,15 @@
     # action into the changeset.
     #
     def __change_setter(self, field: ProjectFields, value: ProjectFieldTypes) -> None:
         if self.__fields[field] == value:
             return
         if field == ProjectFields.PROJECT_IRI or field == ProjectFields.NAMESPACE_IRI or field == ProjectFields.PROJECT_SHORTNAME:
             raise OmasErrorImmutable(f'Field {field.value} is immutable.')
-        if self.__fields[field] is None:
+        if self.__fields.get(field) is None:
             if self.__change_set.get(field) is None:
                 self.__change_set[field] = ProjectFieldChange(None, Action.CREATE)
         else:
             if value is None:
                 if self.__change_set.get(field) is None:
                     self.__change_set[field] = ProjectFieldChange(self.__fields[field], Action.DELETE)
             else:
@@ -257,23 +261,23 @@
               f'  Namespace IRI: {self.__fields[ProjectFields.NAMESPACE_IRI]}\n'\
               f'  Project start: {self.__fields[ProjectFields.PROJECT_START]}\n'
         if self.__fields.get(ProjectFields.PROJECT_END) is not None:
             res += f'  Project end: {self.__fields[ProjectFields.PROJECT_END]}\n'
         return res
 
     @property
-    def creator(self) -> Xsd_anyURI | None:
+    def creator(self) -> Iri | None:
         return self.__creator
 
     @property
     def created(self) -> Xsd_dateTime | None:
         return self.__created
 
     @property
-    def contributor(self) -> Xsd_anyURI | None:
+    def contributor(self) -> Iri | None:
         return self.__contributor
 
     @property
     def modified(self) -> Xsd_dateTime | None:
         return self.__modified
 
     @property
@@ -293,38 +297,61 @@
 
     def notifier(self, fieldname: Xsd_QName):
         field = ProjectFields(fieldname)
         self.__change_set[field] = ProjectFieldChange(self.__fields[field], Action.MODIFY)
         pass
 
     @classmethod
-    def read(cls, con: IConnection, projectIri: Xsd_anyURI | Xsd_QName) -> Self:
+    def read(cls, con: IConnection, projectIri_SName: Iri | Xsd_NCName | str) -> Self:
         """
         Read the project from the triplestore and return an instance of the project
         :param con: A valid Connection object
         :type con: IConnection
         :param projectIri: The IRI/QName of the project to be read
         :type projectIri: Xsd_anyURI | Xsd_QName
         :return: Project instance
         """
         context = Context(name=con.context_name)
-        if isinstance(projectIri, Xsd_QName):
-            projectIri = context.qname2iri(projectIri)
         query = context.sparql_context
-        query += f"""
-            SELECT ?prop ?val
-            FROM omas:admin
-            WHERE {{
-                {projectIri.resUri} ?prop ?val
-            }}
-        """
+
+        projectIri: Iri | None = None
+        shortname: Xsd_NCName | None = None
+        if isinstance(projectIri_SName, Iri):
+            projectIri = projectIri_SName
+        elif isinstance(projectIri_SName, Xsd_NCName):
+            shortname = Xsd_NCName(projectIri_SName)
+        else:
+            if ':' in str(projectIri_SName):  # must be IRI or QName
+                projectIri = Iri(projectIri_SName)
+            else:
+                shortname = Xsd_NCName(projectIri_SName)
+
+        if projectIri is not None:
+            query += f"""
+                SELECT ?prop ?val
+                FROM omas:admin
+                WHERE {{
+                    {projectIri.toRdf} ?prop ?val
+                }}
+            """
+        elif shortname is not None:
+            query += f"""
+                SELECT ?prop ?val
+                FROM omas:admin
+                WHERE {{
+                    ?proj a omas:Project .
+                    ?proj omas:projectShortName ?shortname .
+                    ?proj ?prop ?val .
+                    FILTER(?shortname = {shortname.toRdf})
+                }}
+            """
         jsonobj = con.query(query)
         res = QueryProcessor(context, jsonobj)
         if len(res) == 0:
-            raise OmasErrorNotFound(f'Project with IRI "{projectIri}" not found.')
+            raise OmasErrorNotFound(f'Project with IRI/shortname "{projectIri_SName}" not found.')
         creator = None
         created = None
         contributor = None
         modified = None
         projectShortName = None
         namespaceIri = None
         label = LangString()
@@ -369,15 +396,15 @@
                    comment=comment,
                    projectStart=projectStart,
                    projectEnd=projectEnd)
 
     @staticmethod
     def search(con: IConnection,
                label: Optional[str] = None,
-               comment: Optional[str] = None) -> List[Xsd_anyURI | Xsd_QName]:
+               comment: Optional[str] = None) -> List[Iri]:
         """
         Search for a given project. If no label or comment is given, all existing projects are returned. If both
         a search term for the label and comment are given, they will be combined by *AND*.
         :param con: Valid Connection object
         :type con: IConnection
         :param label: A string to search for in the labels. The search will check if the label of a project
         **contains** the string given here.
@@ -409,15 +436,15 @@
         #     FILTER(STRSTARTS(?label, "{label}"))
         # }}
         # """
         jsonobj = con.query(sparql)
         res = QueryProcessor(context, jsonobj)
         if len(res) == 0:
             raise OmasErrorNotFound('No matching Pprojects not found.')
-        projects = []
+        projects: List[Iri] = []
         for r in res:
             projects.append(r['project'])
         return projects
 
     def create(self, indent: int = 0, indent_inc: int = 4) -> None:
         """
         Create a new project in the triple store
@@ -430,15 +457,15 @@
         :raises OmasError: All other errors
         """
         #
         # First we check if the logged-in user ("actor") has the permission to create a user for
         # the given project!
         #
         actor = self._con.userdata
-        sysperms = actor.inProject.get(Xsd_QName('omas:SystemProject'))
+        sysperms = actor.inProject.get(Iri('omas:SystemProject'))
         is_root: bool = False
         if sysperms and AdminPermission.ADMIN_OLDAP in sysperms:
             is_root = True
         if not is_root:
             raise OmasErrorNoPermission(f'No permission to create a new project.')
 
         timestamp = Xsd_dateTime.now()
@@ -451,34 +478,37 @@
 
         sparql1 = context.sparql_context
         sparql1 += f"""
         SELECT ?project
         FROM omas:admin
         WHERE {{
             ?project a omas:Project .
-            FILTER(?project = {self.projectIri.resUri})
+            FILTER(?project = {self.projectIri.toRdf})
         }}
         """
 
         blank = ''
         sparql2 = context.sparql_context
-        sparql2 += f'{blank:{indent * indent_inc}}INSERT DATA {{\n'
-        sparql2 += f'{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{\n'
-        sparql2 += f'{blank:{(indent + 2) * indent_inc}}{self.projectIri.resUri} a omas:Project ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}dcterms:creator {self._con.userIri.resUri} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}dcterms:created {timestamp.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}dcterms:contributor {self._con.userIri.resUri} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}dcterms:modified {timestamp.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}omas:projectShortName {self.projectShortName.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}rdfs:label {self.label.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}rdfs:comment {self.comment.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}omas:namespaceIri {self.namespaceIri.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}omas:projectStart {self.projectStart.toRdf} ;\n'
-        sparql2 += f'{blank:{(indent + 3) * indent_inc}}omas:projectEnd {self.projectEnd.toRdf} .\n'
-        sparql2 += f'{blank:{(indent + 1) * indent_inc}}}}\n'
+        sparql2 += f'{blank:{indent * indent_inc}}INSERT DATA {{'
+        sparql2 += f'\n{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{'
+        sparql2 += f'\n{blank:{(indent + 2) * indent_inc}}{self.projectIri.toRdf} a omas:Project'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:creator {self._con.userIri.toRdf}'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:created {timestamp.toRdf}'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:contributor {self._con.userIri.toRdf}'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:modified {timestamp.toRdf}'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:projectShortName {self.projectShortName.toRdf}'
+        if self.label:
+            sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}rdfs:label {self.label.toRdf}'
+        if self.comment:
+            sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}rdfs:comment {self.comment.toRdf}'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:namespaceIri {self.namespaceIri.toRdf}'
+        sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:projectStart {self.projectStart.toRdf}'
+        if self.projectEnd is not None:
+            sparql2 += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:projectEnd {self.projectEnd.toRdf}'
+        sparql2 += f' .\n{blank:{(indent + 1) * indent_inc}}}}\n'
         sparql2 += f'{blank:{indent * indent_inc}}}}\n'
 
         self._con.transaction_start()
         try:
             jsonobj = self._con.transaction_query(sparql1)
         except OmasError:
             self._con.transaction_abort()
@@ -508,15 +538,15 @@
         :type indent_inc: int
         :return: None
         :Raises: OmasErrorNoPermission: No permission for operation
         :Raises: OmasErrorUpdateFailed: Update failed
         :Raises: Omas Error: Other Internal error
         """
         actor = self._con.userdata
-        sysperms = actor.inProject.get(Xsd_QName('omas:SystemProject'))
+        sysperms = actor.inProject.get(Iri('omas:SystemProject'))
         is_root: bool = False
         if sysperms and AdminPermission.ADMIN_OLDAP in sysperms:
             is_root = True
         if not is_root:
             raise OmasErrorNoPermission(f'No permission to create a new project.')
 
         timestamp = Xsd_dateTime.now()
@@ -548,15 +578,15 @@
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?project {field.value} {change.old_value.toRdf} .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
             if change.action != Action.DELETE:
                 sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?project {field.value} {self.__fields[field].toRdf} .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
             sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
-            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self.projectIri.resUri} as ?project)\n'
+            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self.projectIri.toRdf} as ?project)\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}?project {field.value} {change.old_value.toRdf} .\n'
             sparql += f'{blank:{indent * indent_inc}}}}'
             sparql_list.append(sparql)
         sparql = context.sparql_context
         sparql += " ;\n".join(sparql_list)
 
         self._con.transaction_start()
@@ -582,30 +612,30 @@
         """
         Delete the given user from the triplestore
         :return: None
         :raises OmasErrorNoPermission: No permission for operation
         :raises OmasError: generic internal error
         """
         actor = self._con.userdata
-        sysperms = actor.inProject.get(Xsd_QName('omas:SystemProject'))
+        sysperms = actor.inProject.get(Iri('omas:SystemProject'))
         is_root: bool = False
         if sysperms and AdminPermission.ADMIN_OLDAP in sysperms:
             is_root = True
         if not is_root:
             raise OmasErrorNoPermission(f'No permission to delete project "{str(self.projectIri)}".')
 
         #
         # TODO: Check if project as any datamodel and/or data. Decline the deletion if this is the case
         #
         context = Context(name=self._con.context_name)
         sparql = context.sparql_context
         sparql += f"""
         DELETE WHERE {{
-            {self.projectIri.resUri} a omas:Project .
-            {self.projectIri.resUri} ?prop ?val .
+            {self.projectIri.toRdf} a omas:Project .
+            {self.projectIri.toRdf} ?prop ?val .
         }} 
         """
         # TODO: use transaction for error handling
         self._con.update_query(sparql)
 
 
 if __name__ == "__main__":
```

### Comparing `omaslib-0.1.8/omaslib/src/propertyclass.py` & `omaslib-0.1.9/omaslib/src/propertyclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 """
 :Author: Lukas Rosenthaler <lukas.rosenthaler@unibas.ch>
 :Copyright: © Lukas Rosenthaler (2023, 2024)
 """
 from dataclasses import dataclass
-from datetime import datetime
 from enum import Enum, unique
-from typing import Set, Optional, Any, Dict, Callable, List, Self
+from functools import partial
+from typing import Optional, Dict, Callable, List, Self
 
 from pystrict import strict
 
+from omaslib.src.dtypes.languagein import LanguageIn
+from omaslib.src.dtypes.rdfset import RdfSet
+from omaslib.src.dtypes.string_literal import StringLiteral
+from omaslib.src.enums.language import Language
 from omaslib.src.helpers.Notify import Notify
 from omaslib.src.helpers.context import Context
 from omaslib.src.dtypes.bnode import BNode
 from omaslib.src.enums.action import Action
+from omaslib.src.xsd.iri import Iri
+from omaslib.src.xsd.xsd import Xsd
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
+from omaslib.src.xsd.xsd_decimal import Xsd_decimal
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.helpers.langstring import LangString
-from omaslib.src.enums.language import Language
-from omaslib.src.helpers.omaserror import OmasError, OmasErrorNotFound, OmasErrorAlreadyExists, OmasErrorUpdateFailed
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.helpers.omaserror import OmasError, OmasErrorNotFound, OmasErrorAlreadyExists, OmasErrorUpdateFailed, OmasErrorValue
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.helpers.query_processor import RowType, QueryProcessor
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
 from omaslib.src.helpers.semantic_version import SemanticVersion
-from omaslib.src.helpers.tools import RdfModifyItem, RdfModifyProp, lprint
+from omaslib.src.helpers.tools import RdfModifyItem, RdfModifyProp, str2qname_anyiri, lprint
 from omaslib.src.enums.xsd_datatypes import XsdDatatypes
 from omaslib.src.iconnection import IConnection
 from omaslib.src.model import Model
 from omaslib.src.propertyrestrictions import PropertyRestrictions
 from omaslib.src.enums.propertyrestrictiontype import PropertyRestrictionType
+from omaslib.src.xsd.xsd_string import Xsd_string
 
 
 @unique
 class OwlPropertyType(Enum):
     OwlDataProperty = 'owl:DatatypeProperty'
     OwlObjectProperty = 'owl:ObjectProperty'
 
+    @property
+    def toRdf(self):
+        return self.value
+
 
-PropTypes = Xsd_QName | Xsd_anyURI | OwlPropertyType | XsdDatatypes | PropertyRestrictions | LangString | int | float | None
-PropertyClassAttributesContainer = Dict[PropertyClassAttribute, PropTypes]
-Attributes = Dict[Xsd_QName, List[Any] | Set[Any]]
+PropTypes = Iri | OwlPropertyType | XsdDatatypes | PropertyRestrictions | LangString | Xsd_decimal | None
+PropClassAttrContainer = Dict[PropClassAttr, PropTypes]
+Attributes = Dict[Xsd_QName, LangString | RdfSet | LanguageIn | List[Xsd]]
 
 
 @dataclass
-class PropertyClassAttributeChange:
+class PropClassAttrChange:
     old_value: PropTypes
     action: Action
     test_in_use: bool
 
 
 @strict
 class PropertyClass(Model, Notify):
@@ -63,50 +73,56 @@
 
     *NOTE*: External properties have to be defined and created before being referenced as
     property within a resource definition. In order to reference an external property, the
     QName has to be used!
 
     """
     _graph: Xsd_NCName
-    _property_class_iri: Xsd_QName | None
-    _internal: Xsd_QName | None
+    _property_class_iri: Iri | None
+    _internal: Iri | None
     _force_external: bool
-    _attributes: PropertyClassAttributesContainer
-    _changeset: Dict[PropertyClassAttribute, PropertyClassAttributeChange]
+    _attributes: PropClassAttrContainer
+    _changeset: Dict[PropClassAttr, PropClassAttrChange]
     _test_in_use: bool
     _notifier: Callable[[type], None] | None
     #
     # The following attributes of this class cannot be set explicitely by the used
     # They are automatically managed by the OMAS system
     #
-    __creator: Optional[Xsd_anyURI]
-    __created: Optional[Xsd_dateTime]
-    __contributor: Optional[Xsd_anyURI]
-    __modified: Optional[Xsd_dateTime]
+    __creator: Iri | None
+    __created: Xsd_dateTime | None
+    __contributor: Iri | None
+    __modified: Xsd_dateTime | None
     __version: SemanticVersion
     __from_triplestore: bool
 
-    __datatypes: Dict[PropertyClassAttribute, PropTypes] = {
-        PropertyClassAttribute.SUBPROPERTY_OF: {Xsd_QName},
-        PropertyClassAttribute.PROPERTY_TYPE: {OwlPropertyType},
-        PropertyClassAttribute.TO_NODE_IRI: {Xsd_QName, Xsd_anyURI},
-        PropertyClassAttribute.DATATYPE: {XsdDatatypes},
-        PropertyClassAttribute.RESTRICTIONS: {PropertyRestrictions},
-        PropertyClassAttribute.NAME: {LangString},
-        PropertyClassAttribute.DESCRIPTION: {LangString},
-        PropertyClassAttribute.ORDER: {int, float}
+    __datatypes: Dict[PropClassAttr, PropTypes] = {
+        PropClassAttr.SUBPROPERTY_OF: Iri,
+        PropClassAttr.PROPERTY_TYPE: OwlPropertyType,
+        PropClassAttr.TO_NODE_IRI: Iri,
+        PropClassAttr.DATATYPE: XsdDatatypes,
+        PropClassAttr.RESTRICTIONS: PropertyRestrictions,
+        PropClassAttr.NAME: LangString,
+        PropClassAttr.DESCRIPTION: LangString,
+        PropClassAttr.ORDER: Xsd_decimal
     }
 
     def __init__(self, *,
                  con: IConnection,
-                 graph: Xsd_NCName,
-                 property_class_iri: Optional[Xsd_QName] = None,
-                 attrs: Optional[PropertyClassAttributesContainer] = None,
-                 notifier: Optional[Callable[[PropertyClassAttribute], None]] = None,
-                 notify_data: Optional[PropertyClassAttribute] = None):
+                 graph: Xsd_NCName | str,
+                 property_class_iri: Iri | str | None = None,
+                 subPropertyOf: Iri | str | None = None,
+                 toNodeIri: Iri | str | None = None,
+                 datatype: XsdDatatypes | None = None,
+                 restrictions: PropertyRestrictions | None = None,
+                 name: LangString | str | None = None,
+                 description: LangString | str | None = None,
+                 order: Xsd_decimal | None = None,
+                 notifier: Callable[[PropClassAttr], None] | None = None,
+                 notify_data: PropClassAttr | None = None):
         """
         TODO: 1) check if a valid datatype is defined!
         Constructor for a PropertyClass instance. It represents all the information about a PropertyClass
         necessary to perform the CRUD (Create, Read, Update and Delete) operations in both the SHACL and
         OWL representations.
 
         :param con: A valid IConnection instance
@@ -115,207 +131,242 @@
         :param attrs: A PropertyClassAttributesContainer containing all the attributes
         :param notifier: The notifier which is called when an complex atribute such as a LangString or
                          a restriction has changed
         :param notify_data: The data that should be given to the notifier
         """
         Model.__init__(self, con)
         Notify.__init__(self, notifier, notify_data)
-        self._graph = graph
-        self._property_class_iri = property_class_iri
-        if attrs is None:
-            self._attributes = {}
-        else:
-            for attr, value in attrs.items():
-                if type(attr) is not PropertyClassAttribute:
-                    raise OmasError(f'Unsupported Property prop "{attr}"')
-                if type(value) not in PropertyClass.__datatypes[attr]:
-                    raise OmasError(f'Datatype of prop "{attr.value}": "{type(value)}", should be {PropertyClass.__datatypes[attr]} ({value}) is not valid')
-                #
-                # if the "value"-class is a subclass of Notify, it has the method "set_notifier".
-                # we need to set it!
-                #
-                if getattr(value, 'set_notifier', None) is not None:
-                    value.set_notifier(self.notifier, attr)
-            self._attributes = attrs
+        self._graph = Xsd_NCName(graph)
+        self._property_class_iri = Iri(property_class_iri)
+        self._attributes: PropClassAttrContainer = {}
+        if subPropertyOf is not None:
+            self._attributes[PropClassAttr.SUBPROPERTY_OF] = Iri(subPropertyOf)
+        if toNodeIri is not None:
+            self._attributes[PropClassAttr.TO_NODE_IRI] = Iri(toNodeIri)
+        if datatype is not None:
+            if isinstance(datatype, XsdDatatypes):
+                self._attributes[PropClassAttr.DATATYPE] = datatype
+            else:
+                try:
+                    self._attributes[PropClassAttr.DATATYPE] = XsdDatatypes(datatype)
+                except ValueError as err:
+                    raise OmasErrorValue(str(err))
+        if restrictions is not None:
+            if not isinstance(restrictions, PropertyRestrictions):
+                raise OmasErrorValue(f'restrictions must be a "PropertyRestrictions" object, is "{type(restrictions).__name__}"')
+            self._attributes[PropClassAttr.RESTRICTIONS] = restrictions
+            self._attributes[PropClassAttr.RESTRICTIONS].set_notifier(self.notifier, PropClassAttr.RESTRICTIONS)
+        if name is not None:
+            self._attributes[PropClassAttr.NAME] = name if isinstance(name, LangString) else LangString(name)
+            self._attributes[PropClassAttr.NAME].set_notifier(self.notifier, PropClassAttr.NAME)
+        if description is not None:
+            self._attributes[PropClassAttr.DESCRIPTION] = description if isinstance(description, LangString) else LangString(description)
+            self._attributes[PropClassAttr.DESCRIPTION].set_notifier(self.notifier, PropClassAttr.DESCRIPTION)
+        if order is not None:
+            self._attributes[PropClassAttr.ORDER] = order if isinstance(order, Xsd_decimal) else Xsd_decimal(order)
 
         # setting property type for OWL which distinguished between Data- and Object-properties
-        if self._attributes:
-            if self._attributes.get(PropertyClassAttribute.TO_NODE_IRI) is not None:
-                self._attributes[PropertyClassAttribute.PROPERTY_TYPE] = OwlPropertyType.OwlObjectProperty
-                dt = self._attributes.get(PropertyClassAttribute.DATATYPE)
-                if dt and (dt != XsdDatatypes.anyURI and dt != XsdDatatypes.QName):
-                    raise OmasError(f'Datatype "{dt}" not valid for OwlObjectProperty')
-            else:
-                self._attributes[PropertyClassAttribute.PROPERTY_TYPE] = OwlPropertyType.OwlDataProperty
+        if self._attributes.get(PropClassAttr.TO_NODE_IRI) is not None:
+            self._attributes[PropClassAttr.PROPERTY_TYPE] = OwlPropertyType.OwlObjectProperty
+            if self._attributes.get(PropClassAttr.DATATYPE) is not None:
+                raise OmasError(f'Datatype not possible for OwlObjectProperty')
+        else:
+            self._attributes[PropClassAttr.PROPERTY_TYPE] = OwlPropertyType.OwlDataProperty
+
+        for attr in PropClassAttr:
+            prefix, name = attr.value.split(':')
+            if name == 'type':
+                name = 'propertyType'
+            elif name == 'class':
+                name = 'toNodeIri'
+            setattr(PropertyClass, name, property(
+                partial(PropertyClass.__get_value, attr=attr),
+                partial(PropertyClass.__set_value, attr=attr),
+                partial(PropertyClass.__del_value, attr=attr)))
+
         self._changeset = {}  # initialize changeset to empty set
         self._test_in_use = False
         self._internal = None
         self._force_external = False
         self.__creator = None
         self.__created = None
         self.__contributor = None
         self.__modified = None
         self.__version = SemanticVersion()
         self.__from_triplestore = False
 
+    def __get_value(self: Self, attr: PropClassAttr) -> PropTypes | None:
+        return self._attributes.get(attr)
+
+    def __set_value(self: Self, value: PropTypes, attr: PropClassAttr) -> None:
+        self.__change_setter(attr, value)
+
+    def __del_value(self: Self, attr: PropClassAttr) -> None:
+        if self._attributes.get(attr) is not None:
+            self._changeset[attr] = PropClassAttrChange(self._attributes[attr], Action.DELETE, True)
+            del self._attributes[attr]
+            self.notify()
+
+    def __change_setter(self: Self, attr: PropClassAttr, value: PropTypes) -> None:
+        if not isinstance(attr, PropClassAttr):
+            raise OmasError(f'Unsupported prop {attr}')
+        if not isinstance(value, PropertyClass.__datatypes[attr]):
+            raise OmasError(f'Datatype of {attr.value} is not in {PropertyClass.__datatypes[attr]}')
+        if self._attributes.get(attr) == value:
+            return
+        if getattr(value, 'set_notifier', None) is not None:
+            value.set_notifier(self.notifier, attr)
+
+        if attr == PropClassAttr.TO_NODE_IRI:
+            if self._attributes.get(PropClassAttr.DATATYPE) is not None:
+                self._changeset[PropClassAttr.DATATYPE] = PropClassAttrChange(self._attributes[PropClassAttr.DATATYPE], Action.DELETE, True)
+                del self._attributes[PropClassAttr.DATATYPE]
+            if self._attributes.get(PropClassAttr.TO_NODE_IRI) is not None:
+                self._changeset[PropClassAttr.TO_NODE_IRI] = PropClassAttrChange(self._attributes[PropClassAttr.TO_NODE_IRI], Action.REPLACE, True)
+            else:
+                self._changeset[PropClassAttr.TO_NODE_IRI] = PropClassAttrChange(None, Action.CREATE, True)
+            self._attributes[PropClassAttr.TO_NODE_IRI] = value
+        elif attr == PropClassAttr.DATATYPE:
+            if self._attributes.get(PropClassAttr.TO_NODE_IRI) is not None:
+                self._changeset[PropClassAttr.TO_NODE_IRI] = PropClassAttrChange(self._attributes[PropClassAttr.TO_NODE_IRI], Action.DELETE, True)
+                del self._attributes[PropClassAttr.TO_NODE_IRI]
+            if self._attributes.get(PropClassAttr.DATATYPE) is not None:
+                self._changeset[PropClassAttr.DATATYPE] = PropClassAttrChange(self._attributes[PropClassAttr.DATATYPE], Action.REPLACE, True)
+            else:
+                self._changeset[PropClassAttr.DATATYPE] = PropClassAttrChange(None, Action.CREATE, True)
+            self._attributes[PropClassAttr.DATATYPE] = value
+        else:
+            if self._changeset.get(attr) is None:
+                if self._attributes.get(attr) is not None:
+                    self._changeset[attr] = PropClassAttrChange(self._attributes[attr], Action.REPLACE, True)
+                else:
+                    self._changeset[attr] = PropClassAttrChange(None, Action.CREATE, True)
+            self._attributes[attr] = value
+        self.notify()
+
     def __len__(self) -> int:
         return len(self._attributes)
 
     def __str__(self) -> str:
         propstr = f'Property: {str(self._property_class_iri)};'
         for attr, value in self._attributes.items():
             propstr += f' {attr.value}: {value};'
         return propstr
 
-    def __getitem__(self, attr: PropertyClassAttribute) -> PropTypes:
+    def __getitem__(self, attr: PropClassAttr) -> PropTypes:
         return self._attributes[attr]
 
-    def get(self, attr: PropertyClassAttribute) -> PropTypes | None:
+    def get(self, attr: PropClassAttr) -> PropTypes | None:
         return self._attributes.get(attr)
 
-    def __setitem__(self, attr: PropertyClassAttribute, value: PropTypes) -> None:
-        if type(attr) is not PropertyClassAttribute:
-            raise OmasError(f'Unsupported prop {attr}')
-        if type(value) not in PropertyClass.__datatypes[attr]:
-            raise OmasError(f'Datatype of {attr.value} is not in {PropertyClass.__datatypes[attr]}')
+    def __setitem__(self, attr: PropClassAttr, value: PropTypes) -> None:
+        self.__change_setter(attr, value)
 
-        if self._attributes.get(attr) is None:
-            if getattr(value, 'set_notifier', None) is not None:
-                value.set_notifier(self.notifier, attr)
-            if self._changeset.get(attr) is None:
-                self._changeset[attr] = PropertyClassAttributeChange(None, Action.CREATE, True)
-            self._attributes[attr] = value
-            self.notify()
-        else:
-            if self._attributes.get(attr) != value:  # we do nothing if nothing changes
-                if attr == PropertyClassAttribute.TO_NODE_IRI \
-                        and self._attributes.get(PropertyClassAttribute.DATATYPE) \
-                        and self._attributes[PropertyClassAttribute.DATATYPE] != XsdDatatypes.anyURI \
-                        and self._attributes[PropertyClassAttribute.DATATYPE] != XsdDatatypes.QName:
-                    # We have to delete the DATATYPE
-                    self._changeset[PropertyClassAttribute.DATATYPE] = PropertyClassAttributeChange(self._attributes[PropertyClassAttribute.DATATYPE], Action.DELETE, True)
-                    del self._attributes[PropertyClassAttribute.DATATYPE]
-                    self._changeset[attr] = PropertyClassAttributeChange(self._attributes[attr], Action.CREATE, True)
-                    self.notify()
-                elif attr == PropertyClassAttribute.DATATYPE \
-                        and self._attributes.get(PropertyClassAttribute.TO_NODE_IRI) \
-                        and value != XsdDatatypes.anyURI \
-                        and value != XsdDatatypes.QName:
-                    self._changeset[PropertyClassAttribute.TO_NODE_IRI] = PropertyClassAttributeChange(self._attributes[PropertyClassAttribute.TO_NODE_IRI],
-                                                                                                    Action.DELETE, True)
-                    del self._attributes[PropertyClassAttribute.TO_NODE_IRI]
-                    self._changeset[attr] = PropertyClassAttributeChange(self._attributes[attr], Action.CREATE, True)
-                    self.notify()
-                elif self._changeset.get(attr) is None:
-                    self._changeset[attr] = PropertyClassAttributeChange(self._attributes[attr], Action.REPLACE, True)
-                self._attributes[attr] = value
-                self.notify()
-
-    def __delitem__(self, attr: PropertyClassAttribute) -> None:
+    def __delitem__(self, attr: PropClassAttr) -> None:
         if self._attributes.get(attr) is not None:
-            self._changeset[attr] = PropertyClassAttributeChange(self._attributes[attr], Action.DELETE, True)
+            self._changeset[attr] = PropClassAttrChange(self._attributes[attr], Action.DELETE, True)
             del self._attributes[attr]
             self.notify()
 
     @property
-    def property_class_iri(self) -> Xsd_QName:
+    def property_class_iri(self) -> Iri:
         return self._property_class_iri
 
     @property
     def version(self) -> SemanticVersion:
         return self.__version
 
     @property
-    def creator(self) -> Optional[Xsd_anyURI]:
+    def creator(self) -> Iri | None:
         return self.__creator
 
     @property
-    def created(self) -> Optional[datetime]:
+    def created(self) -> Xsd_dateTime | None:
         return self.__created
 
     @property
-    def contributor(self) -> Optional[Xsd_anyURI]:
+    def contributor(self) -> Iri | None:
         return self.__contributor
 
     @property
-    def modified(self):
+    def modified(self) -> Xsd_dateTime | None:
         return self.__modified
 
     @property
-    def changeset(self) -> Dict[PropertyClassAttribute, PropertyClassAttributeChange]:
+    def changeset(self) -> Dict[PropClassAttr, PropClassAttrChange]:
         return self._changeset
 
     @property
-    def internal(self) -> Xsd_QName:
+    def internal(self) -> Iri:
         return self._internal
 
     def force_external(self):
         self._force_external = True
 
     def changeset_clear(self):
         self._changeset = {}
 
     @property
     def from_triplestore(self) -> bool:
         return self.__from_triplestore
 
-    def undo(self, attr: Optional[PropertyClassAttribute | PropertyRestrictionType] = None) -> None:
+    def undo(self, attr: Optional[PropClassAttr | PropertyRestrictionType] = None) -> None:
         if attr is None:
             for p, change in self._changeset.items():
                 if change.action == Action.MODIFY:
                     self._attributes[p].undo()
                     if len(self._attributes[p]) == 0:
                         del self._attributes[p]
                 else:
                     if change.action == Action.CREATE:
                         del self._attributes[p]
                     else:
                         self._attributes[p] = change.old_value
             self._changeset = {}
         else:
-            if type(attr) is PropertyClassAttribute:
+            if type(attr) is PropClassAttr:
                 if self._changeset.get(attr) is not None:  # this prop really changed...
                     if self._changeset[attr].action == Action.MODIFY:
                         self._attributes[attr].undo()
                         if len(self._attributes[attr]) == 0:
                             del self._attributes[attr]
                     elif self._changeset[attr].action == Action.CREATE:
                         del self._attributes[attr]
                     else:
                         self._attributes[attr] = self._changeset[attr].old_value
                     del self._changeset[attr]
             elif type(attr) is PropertyRestrictionType:
-                if self._attributes.get(PropertyClassAttribute.RESTRICTIONS) is None:
+                if self._attributes.get(PropClassAttr.RESTRICTIONS) is None:
                     return
-                self._attributes[PropertyClassAttribute.RESTRICTIONS].undo(attr)
-                if len(self._attributes[PropertyClassAttribute.RESTRICTIONS].changeset) == 0:
-                    if self._changeset.get(PropertyClassAttribute.RESTRICTIONS) is not None:
-                        del self._changeset[PropertyClassAttribute.RESTRICTIONS]
-                if self._attributes.get(PropertyClassAttribute.RESTRICTIONS) is not None:
-                    if len(self._attributes[PropertyClassAttribute.RESTRICTIONS]) == 0:
-                        del self._attributes[PropertyClassAttribute.RESTRICTIONS]
+                self._attributes[PropClassAttr.RESTRICTIONS].undo(attr)
+                if len(self._attributes[PropClassAttr.RESTRICTIONS].changeset) == 0:
+                    if self._changeset.get(PropClassAttr.RESTRICTIONS) is not None:
+                        del self._changeset[PropClassAttr.RESTRICTIONS]
+                if self._attributes.get(PropClassAttr.RESTRICTIONS) is not None:
+                    if len(self._attributes[PropClassAttr.RESTRICTIONS]) == 0:
+                        del self._attributes[PropClassAttr.RESTRICTIONS]
 
     def __changeset_clear(self) -> None:
         for attr, change in self._changeset.items():
             if change.action == Action.MODIFY:
                 self._attributes[attr].changeset_clear()
         self._changeset = {}
 
-    def notifier(self, attr: PropertyClassAttribute) -> None:
-        self._changeset[attr] = PropertyClassAttributeChange(None, Action.MODIFY, True)
+    def notifier(self, attr: PropClassAttr) -> None:
+        self._changeset[attr] = PropClassAttrChange(None, Action.MODIFY, True)
         self.notify()
 
     @property
     def in_use(self):
         context = Context(name=self._con.context_name)
         query = context.sparql_context
         query += f"""
         SELECT (COUNT(?rinstances) as ?nrinstances)
         WHERE {{
-            ?rinstances {self._property_class_iri} ?value
+            ?rinstances {self._property_class_iri.toRdf} ?value
         }} LIMIT 2
         """
         jsonres = self._con.query(query)
         res = QueryProcessor(jsonres)
         if len(res) != 1:
             raise OmasError('Internal Error in "propertyClass.in_use"')
         for r in res:
@@ -323,39 +374,54 @@
                 return True
             else:
                 return False
 
     @staticmethod
     def process_triple(r: RowType, attributes: Attributes) -> None:
         attriri = r['attriri']
-        if isinstance(r['value'], Xsd_QName):
+        if r['attriri'].fragment == 'languageIn':
             if attributes.get(attriri) is None:
-                attributes[attriri] = []
-            attributes[attriri].append(r['value'])
-        elif isinstance(r['value'], OldapStringLiteral):
+                attributes[attriri] = LanguageIn()
+            attributes[attriri].add(r['oo'])
+        elif r['attriri'].fragment == 'in':
             if attributes.get(attriri) is None:
-                attributes[attriri] = []
-            attributes[attriri].append(str(r['value']))
-        elif isinstance(r['value'], BNode):
-            pass
+                attributes[attriri] = RdfSet()
+            attributes[attriri].add(r['oo'])
         else:
             if attributes.get(attriri) is None:
                 attributes[attriri] = []
             attributes[attriri].append(r['value'])
-        if r['attriri'].fragment == 'languageIn':
-            if not attributes.get(attriri):
-                attributes[attriri] = set()
-            attributes[attriri].add(Language[str(r['oo']).upper()])
-        if r['attriri'].fragment == 'in':
-            if not attributes.get(attriri):
-                attributes[attriri] = set()
-            attributes[attriri].add(r['oo'])
+
+        # attriri = r['attriri']
+        # if isinstance(r['value'], Xsd_QName):
+        #     if attributes.get(attriri) is None:
+        #         attributes[attriri] = []
+        #     attributes[attriri].append(r['value'])
+        # elif isinstance(r['value'], StringLiteral):
+        #     if attributes.get(attriri) is None:
+        #         attributes[attriri] = []
+        #     attributes[attriri].append(str(r['value']))
+        # elif isinstance(r['value'], BNode):
+        #     pass
+        # else:
+        #     if attributes.get(attriri) is None:
+        #         attributes[attriri] = []
+        #     attributes[attriri].append(r['value'])
+        # if r['attriri'].fragment == 'languageIn':
+        #     #print("\n===>", r['attriri'], r['oo'])
+        #     if not attributes.get(attriri):
+        #         attributes[attriri] = set()
+        #     attributes[attriri].add(Language[str(r['oo']).upper()])
+        # if r['attriri'].fragment == 'in':
+        #     if not attributes.get(attriri):
+        #         attributes[attriri] = set()
+        #     attributes[attriri].add(r['oo'])
 
     @staticmethod
-    def __query_shacl(con: IConnection, graph: Xsd_NCName, property_class_iri: Xsd_QName) -> Attributes:
+    def __query_shacl(con: IConnection, graph: Xsd_NCName, property_class_iri: Iri) -> Attributes:
         context = Context(name=con.context_name)
         query = context.sparql_context
         query += f"""
         SELECT ?attriri ?value ?oo
         FROM {graph}:shacl
         WHERE {{
             BIND({property_class_iri}Shape AS ?shape)
@@ -375,66 +441,97 @@
         return attributes
 
     def parse_shacl(self, attributes: Attributes) -> None:
         """
         Read the SHACL of a non-exclusive (shared) property (that is a sh:PropertyNode definition)
         :return:
         """
-        self._attributes[PropertyClassAttribute.RESTRICTIONS] = PropertyRestrictions()
+        self._attributes[PropClassAttr.RESTRICTIONS] = PropertyRestrictions()
         #
         # Create a set of all PropertyClassProp-strings, e.g. {"sh:path", "sh:datatype" etc.}
         #
-        propkeys = {Xsd_QName(x.value) for x in PropertyClassAttribute}
+        propkeys = {Iri(x.value) for x in PropClassAttr}
         for key, val in attributes.items():
             if key == 'rdf:type':
-                if val[0] == 'sh:PropertyShape':
-                    continue
-                else:
+                if val[0] != 'sh:PropertyShape':
                     raise OmasError(f'Inconsistency, expected "sh:PropertyType", got "{val[0]}".')
+                continue
             elif key == 'sh:path':
-                self._property_class_iri = val[0]
+                if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Iri):
+                    self._property_class_iri = val[0]
+                else:
+                    raise OmasError(f'Inconsistency in SHACL "sh:path"')
             elif key == 'dcterms:hasVersion':
-                self.__version = SemanticVersion.fromString(val[0])
+                if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Xsd_string):
+                    self.__version = SemanticVersion.fromString(str(val[0]))
+                else:
+                    raise OmasError(f'Inconsistency in SHACL "dcterms:hasVersion"')
             elif key == 'dcterms:creator':
-                self.__creator = val[0]
+                if isinstance(val, list) and isinstance(val[0], Iri):
+                    self.__creator = val[0]
+                else:
+                    raise OmasError(f'Inconsistency in SHACL "dcterms:creator"')
             elif key == 'dcterms:created':
-                self.__created = val[0]
+                if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Xsd_dateTime):
+                    self.__created = val[0]
+                else:
+                    raise OmasError(f'Inconsistency in SHACL "dcterms:created"')
             elif key == 'dcterms:contributor':
-                self.__contributor = val[0]
+                if isinstance(val, list) and isinstance(val[0], Iri):
+                    self.__contributor = val[0]
+                else:
+                    raise OmasError(f'Inconsistency in SHACL "dcterms:contributor"')
             elif key == 'dcterms:modified':
-                self.__modified = val[0]
+                if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Xsd_dateTime):
+                    self.__modified = val[0]
+                else:
+                    raise OmasError(f'Inconsistency in SHACL "dcterms:modified"')
             elif key == 'sh:group':
                 pass  # TODO: Process property group correctly.... (at Moment only omas:SystemPropGroup)
             elif key in propkeys:
-                attr = PropertyClassAttribute(key)
-                if {Xsd_QName, Xsd_anyURI} == self.__datatypes[attr]:
-                    self._attributes[attr] = val[0]  # is already QName or AnyIRI from preprocessing
-                elif {XsdDatatypes} == self.__datatypes[attr]:
-                    self._attributes[attr] = XsdDatatypes(str(val[0]))
-                elif {LangString} == self.__datatypes[attr]:
-                    self._attributes[attr] = LangString(val)
-                elif {int, float} == self.__datatypes[attr]:
-                    self._attributes[attr] = val[0]
+                attr = PropClassAttr(key)
+                if self.__datatypes[attr] == Iri:
+                    if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Iri):
+                        self._attributes[attr] = val[0]  # is already QName or AnyIRI from preprocessing
+                    else:
+                        raise OmasError(f'Inconsistency in SHACL "{attr.value}" (got {val[0]} of type {type(val[0]).__name__})')
+                elif self.__datatypes[attr] == XsdDatatypes:
+                    if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Iri):
+                        self._attributes[attr] = XsdDatatypes(str(val[0]))
+                    else:
+                        raise OmasError(f'Inconsistency in SHACL "{attr.value}" (got {val[0]} of type {type(val[0]).__name__})')
+                elif self.__datatypes[attr] == LangString:
+                    if isinstance(val, list):
+                        if self._attributes.get(attr) is None:
+                            self._attributes[attr] = LangString()
+                        self._attributes[attr].add(val)
+                    else:
+                        raise OmasError(f'Inconsistency in SHACL "{attr.value}" (got {val} of type {type(val[0]).__name__})')
+                elif self.__datatypes[attr] == Xsd_decimal:
+                    if isinstance(val, list) and len(val) == 1 and isinstance(val[0], Xsd_decimal):
+                        self._attributes[attr] = val[0]
+                    else:
+                        raise OmasError(f'Inconsistency in SHACL "{attr.value}" (got {val[0]} of type {type(val[0]).__name__})')
             else:
                 try:
-                    self._attributes[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType(key)] = val if (key == "sh:languageIn") or (key == "sh:in") else val[0]
+                    self._attributes[PropClassAttr.RESTRICTIONS][PropertyRestrictionType(key)] = val if (key == "sh:languageIn") or (key == "sh:in") else val[0]
                 except (ValueError, TypeError) as err:
-                    raise OmasError(f'Invalid shacl definition of PropertyClass attribute: "{key} {val}"')
-        if self._attributes.get(PropertyClassAttribute.RESTRICTIONS):
-            self._attributes[PropertyClassAttribute.RESTRICTIONS].changeset_clear()
+                    raise OmasError(f'Invalid shacl definition of PropertyClass attribute: "{key}" "{val}"')
+        if self._attributes.get(PropClassAttr.RESTRICTIONS):
+            self._attributes[PropClassAttr.RESTRICTIONS].changeset_clear()
         #
         # setting property type for OWL which distinguished between Data- and Object-properties
         #
-        if self._attributes.get(PropertyClassAttribute.TO_NODE_IRI) is not None:
-            self._attributes[PropertyClassAttribute.PROPERTY_TYPE] = OwlPropertyType.OwlObjectProperty
-            dt = self._attributes.get(PropertyClassAttribute.DATATYPE)
+        if self._attributes.get(PropClassAttr.TO_NODE_IRI) is not None:
+            self._attributes[PropClassAttr.PROPERTY_TYPE] = OwlPropertyType.OwlObjectProperty
+            dt = self._attributes.get(PropClassAttr.DATATYPE)
             if dt and (dt != XsdDatatypes.anyURI and dt != XsdDatatypes.QName):
                 raise OmasError(f'Datatype "{dt}" not valid for OwlObjectProperty')
         else:
-            self._attributes[PropertyClassAttribute.PROPERTY_TYPE] = OwlPropertyType.OwlDataProperty
+            self._attributes[PropClassAttr.PROPERTY_TYPE] = OwlPropertyType.OwlDataProperty
         for attr, value in self._attributes.items():
             if getattr(value, 'set_notifier', None) is not None:
                 value.set_notifier(self.notifier, attr)
         self.__from_triplestore = True
 
     def read_owl(self):
         context = Context(name=self._con.context_name)
@@ -452,19 +549,19 @@
         to_node_iri = None
         for r in res:
             attr = r['p']
             obj = r['o']
             match attr:
                 case 'rdf:type':
                     if obj == 'owl:DatatypeProperty':
-                        self._attributes[PropertyClassAttribute.PROPERTY_TYPE] = OwlPropertyType.OwlDataProperty
+                        self._attributes[PropClassAttr.PROPERTY_TYPE] = OwlPropertyType.OwlDataProperty
                     elif obj == 'owl:ObjectProperty':
-                        self._attributes[PropertyClassAttribute.PROPERTY_TYPE] = OwlPropertyType.OwlObjectProperty
+                        self._attributes[PropClassAttr.PROPERTY_TYPE] = OwlPropertyType.OwlObjectProperty
                 case 'owl:subPropertyOf':
-                    self._attributes[PropertyClassAttribute.SUBPROPERTY_OF] = obj
+                    self._attributes[PropClassAttr.SUBPROPERTY_OF] = obj
                 case 'rdfs:range':
                     if obj.prefix == 'xsd':
                         datatype = obj
                     else:
                         to_node_iri = obj
                 case 'rdfs:domain':
                     self._internal = obj
@@ -481,29 +578,29 @@
                 case 'dcterms:modified':
                     dt = obj
                     if self.__modified != dt:
                         raise OmasError(f'Inconsistency between SHACL and OWL: created "{self.__modified}" vs "{dt}".')
         #
         # Consistency checks
         #
-        if self._attributes[PropertyClassAttribute.PROPERTY_TYPE] == OwlPropertyType.OwlDataProperty:
+        if self._attributes[PropClassAttr.PROPERTY_TYPE] == OwlPropertyType.OwlDataProperty:
             if not datatype:
                 raise OmasError(f'OwlDataProperty "{self._property_class_iri}" has no rdfs:range datatype defined!')
-            if datatype != self._attributes.get(PropertyClassAttribute.DATATYPE).value:
+            if datatype != self._attributes.get(PropClassAttr.DATATYPE).value:
                 raise OmasError(
-                    f'Property "{self._property_class_iri}" has inconsistent datatype definitions: OWL: "{datatype}" vs. SHACL: "{self._attributes[PropertyClassAttribute.DATATYPE].value}"')
-        if self._attributes[PropertyClassAttribute.PROPERTY_TYPE] == OwlPropertyType.OwlObjectProperty:
+                    f'Property "{self._property_class_iri}" has inconsistent datatype definitions: OWL: "{datatype}" vs. SHACL: "{self._attributes[PropClassAttr.DATATYPE].value}"')
+        if self._attributes[PropClassAttr.PROPERTY_TYPE] == OwlPropertyType.OwlObjectProperty:
             if not to_node_iri:
                 raise OmasError(f'OwlObjectProperty "{self._property_class_iri}" has no rdfs:range resource class defined!')
-            if to_node_iri != self._attributes.get(PropertyClassAttribute.TO_NODE_IRI):
+            if to_node_iri != self._attributes.get(PropClassAttr.TO_NODE_IRI):
                 raise OmasError(
-                    f'Property "{self._property_class_iri}" has inconsistent object type definition: OWL: "{to_node_iri}" vs. SHACL: "{self._attributes.get(PropertyClassAttribute.TO_NODE_IRI)}".')
+                    f'Property "{self._property_class_iri}" has inconsistent object type definition: OWL: "{to_node_iri}" vs. SHACL: "{self._attributes.get(PropClassAttr.TO_NODE_IRI)}".')
 
     @classmethod
-    def read(cls, con: IConnection, graph: Xsd_NCName, property_class_iri: Xsd_QName) -> Self:
+    def read(cls, con: IConnection, graph: Xsd_NCName, property_class_iri: Iri) -> Self:
         property = cls(con=con, graph=graph, property_class_iri=property_class_iri)
         attributes = PropertyClass.__query_shacl(con, graph, property_class_iri)
         property.parse_shacl(attributes=attributes)
         property.read_owl()
         return property
 
     def read_modified_shacl(self, *,
@@ -546,78 +643,78 @@
         res = QueryProcessor(context, jsonobj)
         if len(res) != 1:
             return None
         return res[0].get('modified')
 
 
     def property_node_shacl(self, *,
-                            timestamp: datetime,
+                            timestamp: Xsd_dateTime,
                             bnode: Optional[Xsd_QName] = None,
                             indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql = f'{blank:{(indent + 1) * indent_inc}}# PropertyClass.property_node_shacl()'
         if bnode:
-            sparql += f'\n{blank:{(indent + 1) * indent_inc}} {bnode} sh:path {self._property_class_iri}'
+            sparql += f'\n{blank:{(indent + 1) * indent_inc}} {bnode} sh:path {self._property_class_iri.toRdf}'
         else:
-            sparql += f'\n{blank:{(indent + 1) * indent_inc}}sh:path {self._property_class_iri}'
+            sparql += f'\n{blank:{(indent + 1) * indent_inc}}sh:path {self._property_class_iri.toRdf}'
         sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:hasVersion "{str(self.__version)}"'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:creator {self._con.userIri.resUri()}'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:created {repr(timestamp)}'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:contributor <{self._con.userIri}>'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:modified {repr(timestamp)}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:creator {self._con.userIri.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:created {timestamp.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:contributor {self._con.userIri.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:modified {timestamp.toRdf}'
         for prop, value in self._attributes.items():
-            if prop == PropertyClassAttribute.PROPERTY_TYPE:
+            if prop == PropClassAttr.PROPERTY_TYPE:
                 continue
-            if prop != PropertyClassAttribute.RESTRICTIONS:
+            if prop != PropClassAttr.RESTRICTIONS:
                 sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}{prop.value} {value.value if isinstance(value, Enum) else value}'
             else:
-                sparql += self._attributes[PropertyClassAttribute.RESTRICTIONS].create_shacl(indent + 1, indent_inc)
+                sparql += self._attributes[PropClassAttr.RESTRICTIONS].create_shacl(indent + 1, indent_inc)
         #sparql += f' .\n'
         return sparql
 
     def create_shacl(self, *,
-                     timestamp: datetime,
-                     owlclass_iri: Optional[Xsd_QName] = None,
+                     timestamp: Xsd_dateTime,
+                     owlclass_iri: Iri | None = None,
                      indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql = f'\n{blank:{indent * indent_inc}}# PropertyClass.create_shacl()'
         if owlclass_iri is None:
             sparql += f'\n{blank:{indent * indent_inc}}{self._property_class_iri}Shape a sh:PropertyShape ;\n'
             sparql += self.property_node_shacl(timestamp=timestamp, indent=indent, indent_inc=indent_inc)
         else:
             bnode = Xsd_QName('_:propnode')
             sparql += f'\n{blank:{indent * indent_inc}}{owlclass_iri}Shape sh:property {bnode} .\n'
             sparql += self.property_node_shacl(timestamp=timestamp, bnode=bnode, indent=indent, indent_inc=indent_inc)
         sparql += ' .\n'
         return sparql
 
-    def create_owl_part1(self, timestamp: datetime, indent: int = 0, indent_inc: int = 4) -> str:
+    def create_owl_part1(self, timestamp: Xsd_dateTime, indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
-        sparql = f'{blank:{indent * indent_inc}}{self._property_class_iri.resUri()} rdf:type {self._attributes[PropertyClassAttribute.PROPERTY_TYPE].value}'
-        if self._attributes.get(PropertyClassAttribute.SUBPROPERTY_OF):
-            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:subPropertyOf {self._attributes[PropertyClassAttribute.SUBPROPERTY_OF]}'
+        sparql = f'{blank:{indent * indent_inc}}{self._property_class_iri.toRdf} rdf:type {self._attributes[PropClassAttr.PROPERTY_TYPE].value}'
+        if self._attributes.get(PropClassAttr.SUBPROPERTY_OF):
+            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:subPropertyOf {self._attributes[PropClassAttr.SUBPROPERTY_OF].toRdf}'
         if self._internal:
-            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:domain {self._internal}'
-        if self._attributes.get(PropertyClassAttribute.PROPERTY_TYPE) == OwlPropertyType.OwlDataProperty:
-            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:range {self._attributes[PropertyClassAttribute.DATATYPE].value}'
-        elif self._attributes.get(PropertyClassAttribute.PROPERTY_TYPE) == OwlPropertyType.OwlObjectProperty:
-            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:range {self._attributes[PropertyClassAttribute.TO_NODE_IRI]}'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:creator <{self._con.userIri}>'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:created {repr(timestamp)}'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:contributor <{self._con.userIri}>'
-        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:modified {repr(timestamp)}'
+            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:domain {self._internal.toRdf}'
+        if self._attributes.get(PropClassAttr.PROPERTY_TYPE) == OwlPropertyType.OwlDataProperty:
+            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:range {self._attributes[PropClassAttr.DATATYPE].value}'
+        elif self._attributes.get(PropClassAttr.PROPERTY_TYPE) == OwlPropertyType.OwlObjectProperty:
+            sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}rdfs:range {self._attributes[PropClassAttr.TO_NODE_IRI].toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:creator {self._con.userIri.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:created {timestamp.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:contributor {self._con.userIri.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 1) * indent_inc}}dcterms:modified {timestamp.toRdf}'
         sparql += ' .\n'
         return sparql
 
     def create_owl_part2(self, indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql = f'{blank:{indent * indent_inc}}[\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}rdf:type owl:Restriction ;\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}owl:onProperty {self._property_class_iri}'
-        sparql += self._attributes[PropertyClassAttribute.RESTRICTIONS].create_owl(indent + 1, indent_inc)
+        sparql += f'{blank:{(indent + 1) * indent_inc}}owl:onProperty {self._property_class_iri.toRdf}'
+        sparql += self._attributes[PropClassAttr.RESTRICTIONS].create_owl(indent + 1, indent_inc)
         #
         # TODO: Add the possibility to use owl:onClass or owl:onDataRage instead of rdfs:range
         # (NOTE: owl:onClass and owl:onDataRange can be used only in a restriction and are "local" to the use
         # of the property within the given resource. However, rdfs:range is "global" for all use of this property!
         #
         # if self._attributes[PropertyClassAttribute.PROPERTY_TYPE] == OwlPropertyType.OwlDataProperty:
         #     sparql += f' ;\n{blank:{(indent + 1) * indent_inc}} owl:onDataRange {self._attributes[PropertyClassAttribute.DATATYPE].value}'
@@ -687,15 +784,15 @@
             self._con.transaction_commit()
         else:
             self._con.transaction_abort()
             raise OmasErrorUpdateFailed(f"Update of RDF didn't work!")
 
     def write_as_trig(self, filename: str, indent: int = 0, indent_inc: int = 4) -> None:
         with open(filename, 'w') as f:
-            timestamp = datetime.now()
+            timestamp = Xsd_dateTime().now()
             blank = ''
             context = Context(name=self._con.context_name)
             f.write(context.turtle_context)
 
             f.write(f'{blank:{indent * indent_inc}}{self._graph}:shacl {{\n')
             if self._internal is not None:
                 f.write(self.create_shacl(timestamp=timestamp, owlclass_iri=self._internal, indent=2))
@@ -704,50 +801,50 @@
             f.write(f'{blank:{indent * indent_inc}}}}\n')
 
             f.write(f'{blank:{indent * indent_inc}}{self._graph}:onto {{\n')
             f.write(self.create_owl_part1(timestamp=timestamp, indent=2))
             f.write(f'{blank:{indent * indent_inc}}}}\n')
 
     def update_shacl(self, *,
-                     owlclass_iri: Optional[Xsd_QName] = None,
+                     owlclass_iri: Iri | None = None,
                      timestamp: Xsd_dateTime,
                      indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql_list = []
         for prop, change in self._changeset.items():
             sparql = f'#\n# SHACL\n# Process "{prop.value}" with Action "{change.action.value}"\n#\n'
             if change.action == Action.MODIFY:
-                if PropertyClass.__datatypes[prop] == {LangString}:
+                if PropertyClass.__datatypes[prop] == LangString:
                     sparql += self._attributes[prop].update_shacl(graph=self._graph,
                                                                   owlclass_iri=owlclass_iri,
                                                                   prop_iri=self._property_class_iri,
                                                                   attr=prop,
                                                                   modified=self.__modified,
                                                                   indent=indent, indent_inc=indent_inc)
-                elif PropertyClass.__datatypes[prop] == {PropertyRestrictions}:
+                elif PropertyClass.__datatypes[prop] == PropertyRestrictions:
                     sparql += self._attributes[prop].update_shacl(graph=self._graph,
                                                                   owlclass_iri=owlclass_iri,
                                                                   prop_iri=self._property_class_iri,
                                                                   modified=self.__modified,
                                                                   indent=indent, indent_inc=indent_inc)
                 else:
-                    raise OmasError(f'SHACL property {prop.value} should not have update action "Update".')
+                    raise OmasError(f'SHACL property {prop.value} should not have update action "Update" ({PropertyClass.__datatypes[prop]}).')
                 sparql_list.append(sparql)
             else:
-                old_value = None
-                new_value = None
                 if change.action == Action.DELETE:
                     old_value = '?val'
                     new_value = None
                 elif change.action == Action.CREATE:
                     old_value = None
-                    new_value = str(self._attributes[prop])
+                    new_value = self._attributes[prop].toRdf
                 elif change.action == Action.REPLACE:
-                    old_value = str(change.old_value)
-                    new_value = str(self._attributes[prop])
+                    old_value = change.old_value.toRdf
+                    new_value = self._attributes[prop].toRdf
+                else:
+                    raise OmasError(f'==========UNEXPECTED ACTION============')
                 ele = RdfModifyItem(prop.value, old_value, new_value)
                 sparql += RdfModifyProp.shacl(action=change.action,
                                               graph=self._graph,
                                               owlclass_iri=owlclass_iri,
                                               pclass_iri=self._property_class_iri,
                                               ele=ele,
                                               last_modified=self.__modified)
@@ -757,44 +854,44 @@
         # Updating the timestamp and contributor ID
         #
         sparql = f'#\n# Update/add dcterms:contributor in {self._graph}:shacl\n#\n'
         sparql += RdfModifyProp.shacl(action=Action.REPLACE if self.__contributor else Action.CREATE,
                                       graph=self._graph,
                                       owlclass_iri=owlclass_iri,
                                       pclass_iri=self._property_class_iri,
-                                      ele=RdfModifyItem('dcterms:contributor', f'<{self.__contributor}>', f'<{self._con.userIri}>'),
+                                      ele=RdfModifyItem('dcterms:contributor', f'{self.__contributor.toRdf}', f'{self._con.userIri.toRdf}'),
                                       last_modified=self.__modified)
         sparql_list.append(sparql)
 
         sparql = f'#\n# Update/add dcterms:modified in {self._graph}:shacl\n#\n'
         sparql += RdfModifyProp.shacl(action=Action.REPLACE if self.__modified else Action.CREATE,
                                       graph=self._graph,
                                       owlclass_iri=owlclass_iri,
                                       pclass_iri=self._property_class_iri,
-                                      ele=RdfModifyItem('dcterms:modified', f'{repr(self.__modified)}', f'{repr(timestamp)}'),
+                                      ele=RdfModifyItem('dcterms:modified', f'{self.__modified.toRdf}', f'{timestamp.toRdf}'),
                                       last_modified=self.__modified)
         sparql_list.append(sparql)
 
         sparql = " ;\n".join(sparql_list)
         return sparql
 
     def update_owl(self, *,
                    owlclass_iri: Optional[Xsd_QName] = None,
-                   timestamp: datetime,
+                   timestamp: Xsd_dateTime,
                    indent: int = 0, indent_inc: int = 4) -> str:
-        owl_propclass_attributes = {PropertyClassAttribute.SUBPROPERTY_OF,  # should be in OWL ontology
-                                    PropertyClassAttribute.DATATYPE,  # used for rdfs:range in OWL ontology
-                                    PropertyClassAttribute.TO_NODE_IRI}  # used for rdfs:range in OWL ontology
-        owl_prop = {PropertyClassAttribute.SUBPROPERTY_OF: PropertyClassAttribute.SUBPROPERTY_OF.value,
-                    PropertyClassAttribute.DATATYPE: "rdfs:range",
-                    PropertyClassAttribute.TO_NODE_IRI: "rdfs:range"}
+        owl_propclass_attributes = {PropClassAttr.SUBPROPERTY_OF,  # should be in OWL ontology
+                                    PropClassAttr.DATATYPE,  # used for rdfs:range in OWL ontology
+                                    PropClassAttr.TO_NODE_IRI}  # used for rdfs:range in OWL ontology
+        owl_prop = {PropClassAttr.SUBPROPERTY_OF: PropClassAttr.SUBPROPERTY_OF.value,
+                    PropClassAttr.DATATYPE: "rdfs:range",
+                    PropClassAttr.TO_NODE_IRI: "rdfs:range"}
         blank = ''
         sparql_list = []
         for prop, change in self._changeset.items():
-            if prop == PropertyClassAttribute.RESTRICTIONS and change.action == Action.MODIFY:
+            if prop == PropClassAttr.RESTRICTIONS and change.action == Action.MODIFY:
                 sparql = self._attributes[prop].update_owl(graph=self._graph,
                                                            owlclass_iri=owlclass_iri,
                                                            prop_iri=self._property_class_iri,
                                                            modified=self.__modified,
                                                            indent=indent, indent_inc=indent_inc)
                 if sparql:
                     sparql_list.append(sparql)
@@ -808,17 +905,17 @@
                                              owlclass_iri=owlclass_iri,
                                              pclass_iri=self._property_class_iri,
                                              ele=ele,
                                              last_modified=self.__modified,
                                              indent=indent, indent_inc=indent_inc)
                 sparql_list.append(sparql)
 
-            if prop == PropertyClassAttribute.DATATYPE or prop == PropertyClassAttribute.TO_NODE_IRI:
+            if prop == PropClassAttr.DATATYPE or prop == PropClassAttr.TO_NODE_IRI:
                 ele: RdfModifyItem
-                if self._attributes.get(PropertyClassAttribute.TO_NODE_IRI):
+                if self._attributes.get(PropClassAttr.TO_NODE_IRI):
                     ele = RdfModifyItem('rdf:type', 'owl:DatatypeProperty', 'owl:ObjectProperty')
                 else:
                     ele = RdfModifyItem('rdf:type', 'owl:ObjectProperty', 'owl:DatatypeProperty')
                 sparql = f'#\n# OWL:\n# Correct OWL property type with Action "{change.action.value}\n#\n'
                 sparql += RdfModifyProp.onto(action=Action.REPLACE,
                                              graph=self._graph,
                                              owlclass_iri=owlclass_iri,
@@ -831,38 +928,38 @@
 
         #
         # Updating the timestamp and contributor ID
         #
         sparql = f'#\n# Update/add dcterms:contributor {self._graph}:onto\n#\n'
         sparql += f'{blank:{indent * indent_inc}}WITH {self._graph}:onto\n'
         sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:contributor <{self.__contributor}>\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:contributor {self.__contributor.toRdf}\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:contributor <{self._con.userIri}>\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:contributor {self._con.userIri.toRdf}\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self._property_class_iri} AS ?prop)\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified ?modified .\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {repr(self.__modified)})\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {self.__modified.toRdf})\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql_list.append(sparql)
 
         sparql = f'#\n# Update/add dcterms:modified in {self._graph}:onto\n#\n'
         sparql += f'{blank:{indent * indent_inc}}WITH {self._graph}:onto\n'
         sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified ?modified\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified {repr(timestamp)}\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified {timestamp.toRdf}\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self._property_class_iri} AS ?prop)\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified ?modified .\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {repr(self.__modified)})\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {self.__modified.toRdf})\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql_list.append(sparql)
 
         sparql = " ;\n".join(sparql_list)
         return sparql
 
     def update(self) -> None:
@@ -891,15 +988,14 @@
             raise
         try:
             modtime_owl = self.read_modified_owl(context=context, graph=self._graph)
         except OmasError as e:
             self._con.transaction_abort()
             raise
 
-        print("\n=============>", modtime_shacl, modtime_owl)
         if modtime_shacl == timestamp and modtime_owl == timestamp:
             self._con.transaction_commit()
             self.__modified = timestamp
             self.__contributor = self._con.userIri
             for prop, change in self._changeset.items():
                 if change.action == Action.MODIFY:
                     self._attributes[prop].changeset_clear()
@@ -933,15 +1029,15 @@
             sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self._property_class_iri}Shape as ?propnode)\n'
         #sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode sh:languageIn ?list .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode ?listprop ?list .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?list rdf:rest* ?z .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?z rdf:first ?head ;\n'
         sparql += f'{blank:{(indent + 2) * indent_inc}}rdf:rest ?tail .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode dcterms:modified ?modified .\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {repr(self.__modified)})\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {self.__modified.toRdf})\n'
         sparql += f'{blank:{indent * indent_inc}}}}'
         sparql_list.append(sparql)
 
         sparql = ''
         #
         # Now we delete the remaining triples
         #
@@ -955,15 +1051,15 @@
         if owlclass_iri is not None:
             sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri}Shape sh:property ?propnode .\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode sh:path {self._property_class_iri} .\n'
         else:
             sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self._property_class_iri}Shape as ?propnode)\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode ?p ?v .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode dcterms:modified ?modified .\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {repr(self.__modified)})\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {self.__modified.toRdf})\n'
         sparql += f'{blank:{indent * indent_inc}}}}'
         sparql_list.append(sparql)
 
         sparql = " ;\n".join(sparql_list)
         return sparql
 
     def delete_owl_subclass_str(self, *,
@@ -974,15 +1070,15 @@
         sparql += f'{blank:{indent * indent_inc}}WITH {self._graph}:onto\n'
         sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri} rdfs:subClassOf ?propnode .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode ?p ?v .\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri} rdfs:subClassOf ?propnode .\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode owl:onProperty {self._property_class_iri} .\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode owl:onProperty {self._property_class_iri.toRdf} .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode ?p ?v .\n'
         sparql += f'{blank:{indent * indent_inc}}}}'
         return sparql
 
     def __delete_owl(self, *,
                      indent: int = 0, indent_inc: int = 4) -> str:
         owlclass_iri = self._internal
@@ -993,15 +1089,15 @@
         sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode ?p ?v\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
         sparql += f'{blank:{indent * indent_inc}}BIND({self._property_class_iri} as ?propnode)\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode ?p ?v .\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?propnode dcterms:modified ?modified .\n'
-        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {repr(self.__modified)})\n'
+        sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {self.__modified.toRdf})\n'
         sparql += f'{blank:{indent * indent_inc}}}}'
         sparql_list.append(sparql)
 
         if owlclass_iri is not None:
             sparql = self.delete_owl_subclass_str(owlclass_iri=owlclass_iri)
             sparql_list.append(sparql)
```

### Comparing `omaslib-0.1.8/omaslib/src/propertyrestrictions.py` & `omaslib-0.1.9/omaslib/src/propertyrestrictions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from pystrict import strict
 
 from omaslib.src.dtypes.rdfset import RdfSet
 from omaslib.src.enums.propertyrestrictiontype import PropertyRestrictionType
 from omaslib.src.helpers.Notify import Notify
 from omaslib.src.enums.action import Action
 from omaslib.src.dtypes.languagein import LanguageIn
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_integer import Xsd_integer
+from omaslib.src.xsd.xsd_nonnegativeinteger import Xsd_nonNegativeInteger
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_float import Xsd_float
 from omaslib.src.xsd.xsd_string import Xsd_string
 from omaslib.src.xsd.xsd_boolean import Xsd_boolean
 from omaslib.src.xsd.xsd import Xsd
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.omaserror import OmasError
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 
 
 @unique
 class Compare(Enum):
     LT = '__lt__'
     LE = '__le__'
     GT = '__gt__'
@@ -93,16 +95,16 @@
         PropertyRestrictionType.MIN_LENGTH: {Xsd_integer},
         PropertyRestrictionType.MAX_LENGTH: {Xsd_integer},
         PropertyRestrictionType.PATTERN: {Xsd_string},
         PropertyRestrictionType.MIN_EXCLUSIVE: {Xsd_integer, Xsd_float},
         PropertyRestrictionType.MIN_INCLUSIVE: {Xsd_integer, Xsd_float},
         PropertyRestrictionType.MAX_EXCLUSIVE: {Xsd_integer, Xsd_float},
         PropertyRestrictionType.MAX_INCLUSIVE: {Xsd_integer, Xsd_float},
-        PropertyRestrictionType.LESS_THAN: {Xsd_QName},
-        PropertyRestrictionType.LESS_THAN_OR_EQUALS: {Xsd_QName},
+        PropertyRestrictionType.LESS_THAN: {Iri},
+        PropertyRestrictionType.LESS_THAN_OR_EQUALS: {Iri},
     }
     compare = {
         PropertyRestrictionType.LANGUAGE_IN: Compare.XX,
         PropertyRestrictionType.IN: Compare.XX,
         PropertyRestrictionType.UNIQUE_LANG: Compare.XX,
         PropertyRestrictionType.MIN_COUNT: Compare.GT,
         PropertyRestrictionType.MAX_COUNT: Compare.LT,
@@ -115,16 +117,16 @@
         PropertyRestrictionType.MAX_INCLUSIVE: Compare.LE,
         PropertyRestrictionType.LESS_THAN: Compare.XX,
         PropertyRestrictionType.LESS_THAN_OR_EQUALS: Compare.XX
     }
 
     def __init__(self, *,
                  restrictions: Optional[RestrictionContainer] = None,
-                 notifier: Optional[Callable[[PropertyClassAttribute], None]] = None,
-                 notify_data: Optional[PropertyClassAttribute] = None):
+                 notifier: Optional[Callable[[PropClassAttr], None]] = None,
+                 notify_data: Optional[PropClassAttr] = None):
         """
         Constructor for restrictions
         :param restrictions: A Dict of restriction. See ~PropertyRestrictionType for SHACL-restriction supported
         """
         super().__init__(notifier, notify_data)
         self._changeset = {}
         if restrictions is None:
@@ -262,81 +264,65 @@
         :param indent_inc: Indent increment for formatting
         :return: SHACL fragment string
         """
         blank = ''
         shacl = ''
         for name, rval in self._restrictions.items():
             shacl += f' ;\n{blank:{indent * indent_inc}}{name.value} {rval.toRdf}'
-            # if type(rval) is set:
-            #     tmp = list(rval)
-            #     if isinstance(tmp[0], Language):
-            #         tmp = [f'"{x.name.lower()}"' for x in rval]
-            #     elif isinstance(tmp[0], str):
-            #         tmp = [f'"{x}"' for x in rval]
-            #     else:
-            #         tmp = [f'{x}' for x in rval]
-            #     value = '(' + ' '.join(tmp) + ')'
-            # elif type(rval) is bool:
-            #     value = 'true' if rval else 'false'
-            # elif type(rval) in {int, float}:
-            #     value = rval
-            # elif type(rval) is str:
-            #     value = f'"{rval}"'
-            # elif type(rval) is Xsd_QName:
-            #     value = str(rval)
-            # else:
-            #     value = rval
-            # shacl += f' ;\n{blank:{indent*indent_inc}}{name.value} {value}'
         return shacl
 
     def create_owl(self, indent: int = 0, indent_inc: int = 4) -> str:
         """
         Return OWL fragment for creating the ontology of the restrictions
         :param indent: Indent for formatting
         :param indent_inc: Indent increment for formatting
         :return: OWL fragment string
         """
         blank = ''
         sparql = ''
-        mincnt = self._restrictions.get(PropertyRestrictionType.MIN_COUNT)
-        maxcnt = self._restrictions.get(PropertyRestrictionType.MAX_COUNT)
+        mincnt = None
+        if self._restrictions.get(PropertyRestrictionType.MIN_COUNT) is not None:
+            mincnt = Xsd_nonNegativeInteger(self._restrictions[PropertyRestrictionType.MIN_COUNT])
+        maxcnt = None
+        if self._restrictions.get(PropertyRestrictionType.MAX_COUNT) is not None:
+            maxcnt = Xsd_nonNegativeInteger(self._restrictions[PropertyRestrictionType.MAX_COUNT])
         if mincnt is not None and maxcnt is not None and mincnt == maxcnt:
-            sparql += f' ;\n{blank:{indent*indent_inc}}owl:cardinality {mincnt}'
+            sparql += f' ;\n{blank:{indent*indent_inc}}owl:cardinality {mincnt.toRdf}'
         else:
             if mincnt is not None:
-                sparql += f' ;\n{blank:{indent*indent_inc}}owl:minCardinality {mincnt}'
+                sparql += f' ;\n{blank:{indent*indent_inc}}owl:minCardinality {mincnt.toRdf}'
             if maxcnt is not None:
-                sparql += f' ;\n{blank:{indent*indent_inc}}owl:maxCardinality {maxcnt}'
+                sparql += f' ;\n{blank:{indent*indent_inc}}owl:maxCardinality {maxcnt.toRdf}'
         return sparql
 
     def update_shacl(self, *,
                      graph: Xsd_NCName,
-                     owlclass_iri: Optional[Xsd_QName] = None,
-                     prop_iri: Xsd_QName,
+                     owlclass_iri: Iri | None = None,
+                     prop_iri: Iri,
                      modified: Xsd_dateTime,
                      indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql_list = []
         for restriction_type, change in self._changeset.items():
-            sparql = f'#\n# Process "{restriction_type.value}" with Action "{change.action.value}"\n#\n'
+            sparql = f'#\n# (X) Process "{restriction_type.value}" with Action "{change.action.value}"\n#\n'
             sparql += f'WITH {graph}:shacl\n'
             if restriction_type == PropertyRestrictionType.LANGUAGE_IN or restriction_type == PropertyRestrictionType.IN:
                 #
                 # The SHACL property sh:languageIn is implemented as a RDF List with blank nodes having
                 # a rdf:first and rdf:rest property. This makes the manipulation a bit complicated. If
                 # sh:languageIn is modified we delete the complete list and replace it by the new list.
                 #
                 sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?z rdf:first ?head ;\n'
                 sparql += f'{blank:{(indent + 2) * indent_inc}}rdf:rest ?tail .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
                 if owlclass_iri:
                     sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri}Shape sh:property ?prop .\n'
-                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri.resUri} .\n'
+                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri.toRdf} .\n'
                 else:
                     sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri}Shape as ?prop)\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {restriction_type.value} ?bnode .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?bnode rdf:rest* ?z .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?z rdf:first ?head ;\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}rdf:rest ?tail .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}'
@@ -352,30 +338,30 @@
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {restriction_type.value} {self._restrictions[restriction_type].toRdf} .\n'
 
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
 
             sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
             if owlclass_iri:
                 sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri}Shape sh:property ?prop .\n'
-                sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri} .\n'
+                sparql += f'{blank:{(indent + 1) * indent_inc}}?prop sh:path {prop_iri.toRdf} .\n'
             else:
                 sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri}Shape as ?prop)\n'
             if change.action != Action.CREATE:
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {restriction_type.value} ?rval .\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified ?modified .\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {modified.toRdf})\n'
             sparql += f'{blank:{indent * indent_inc}}}}'
             sparql_list.append(sparql)
         sparql = ";\n".join(sparql_list)
         return sparql
 
     def update_owl(self, *,
                    graph: Xsd_NCName,
-                   owlclass_iri: Optional[Xsd_QName] = None,
-                   prop_iri: Xsd_QName,
+                   owlclass_iri: Iri | None = None,
+                   prop_iri: Iri,
                    modified: Xsd_dateTime,
                    indent: int = 0, indent_inc: int = 4) -> str:
         """
         Updates the OWL restriction classes for the cardinality
 
         :param owlclass_iri:
         :param prop_iri:
@@ -387,106 +373,106 @@
         blank = ' '
         minmax_done = False
         sparql = ''
         for restriction_type, change in self._changeset.items():
             if minmax_done:
                 continue
             if restriction_type == PropertyRestrictionType.MAX_COUNT or restriction_type == PropertyRestrictionType.MIN_COUNT:
-                old_min_count: Union[int, None]
-                old_max_count: Union[int, None]
+                old_min_count: Union[Xsd_nonNegativeInteger, None]
+                old_max_count: Union[Xsd_nonNegativeInteger, None]
                 if self._changeset.get(PropertyRestrictionType.MIN_COUNT) is None:
-                    old_min_count = int(self._restrictions.get(PropertyRestrictionType.MIN_COUNT))
+                    old_min_count = Xsd_nonNegativeInteger(self._restrictions.get(PropertyRestrictionType.MIN_COUNT))
                 else:
-                    old_min_count = self._changeset[PropertyRestrictionType.MIN_COUNT].old_value
+                    old_min_count = Xsd_nonNegativeInteger(self._changeset[PropertyRestrictionType.MIN_COUNT].old_value)
                 if self._changeset.get(PropertyRestrictionType.MAX_COUNT) is None:
-                    old_max_count = self._restrictions.get(PropertyRestrictionType.MAX_COUNT)
+                    old_max_count = Xsd_nonNegativeInteger(self._restrictions.get(PropertyRestrictionType.MAX_COUNT))
                 else:
-                    old_max_count = self._changeset[PropertyRestrictionType.MAX_COUNT].old_value
+                    old_max_count = Xsd_nonNegativeInteger(self._changeset[PropertyRestrictionType.MAX_COUNT].old_value)
                 sparql += f'#\n# Process "sh:maxCount"/"sh:minCount"...\n#\n'
                 sparql += f'WITH {graph}:onto\n'
                 if old_max_count is not None and old_max_count == old_min_count:
                     sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
-                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:cardinality {old_max_count} .\n'
+                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:cardinality {old_max_count.toRdf} .\n'
                     sparql += f'{blank:{indent * indent_inc}}}}\n'
                 else:
                     sparql += f'{blank:{indent * indent_inc}}DELETE {{\n'
                     if old_min_count is not None:
-                        sparql += f'{blank:{(indent + 2) * indent_inc}}?prop owl:minCardinality {old_min_count} .\n'
+                        sparql += f'{blank:{(indent + 2) * indent_inc}}?prop owl:minCardinality {old_min_count.toRdf} .\n'
                     if old_max_count is not None:
-                        sparql += f'{blank:{(indent + 2) * indent_inc}}?prop owl:maxCardinality {old_max_count} .\n'
+                        sparql += f'{blank:{(indent + 2) * indent_inc}}?prop owl:maxCardinality {old_max_count.toRdf} .\n'
                     sparql += f'{blank:{indent * indent_inc}}}}\n'
                 # we have now removed all cardinality information
-                new_max_count: Union[int, None]
-                new_min_count: Union[int, None]
+                new_max_count: Union[Xsd_nonNegativeInteger, None]
+                new_min_count: Union[Xsd_nonNegativeInteger, None]
                 if self._restrictions.get(PropertyRestrictionType.MIN_COUNT) is None:
                     new_min_count = None
                 else:
-                    new_min_count = self._restrictions[PropertyRestrictionType.MIN_COUNT]
+                    new_min_count = Xsd_nonNegativeInteger(self._restrictions[PropertyRestrictionType.MIN_COUNT])
                 if self._restrictions.get(PropertyRestrictionType.MAX_COUNT) is None:
                     new_max_count = None
                 else:
-                    new_max_count = self._restrictions[PropertyRestrictionType.MAX_COUNT]
+                    new_max_count = Xsd_nonNegativeInteger(self._restrictions[PropertyRestrictionType.MAX_COUNT])
                 if new_max_count is not None and new_max_count == new_min_count:
                     sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
-                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:cardinality {new_max_count} .\n'
+                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:cardinality {new_max_count.toRdf} .\n'
                     sparql += f'{blank:{indent * indent_inc}}}}\n'
                 else:
                     sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
                     if new_max_count is not None:
-                        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:maxCardinality {new_max_count} .\n'
+                        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:maxCardinality {new_max_count.toRdf} .\n'
                     if new_min_count is not None and new_min_count > 0:
-                        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:minCardinality {new_min_count} .\n'
+                        sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:minCardinality {new_min_count.toRdf} .\n'
                     sparql += f'{blank:{indent * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
                 if owlclass_iri:
                     sparql += f'{blank:{(indent + 1) * indent_inc}}{owlclass_iri} rdfs:subClassOf ?prop .\n'
-                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:onProperty {prop_iri} .\n'
+                    sparql += f'{blank:{(indent + 1) * indent_inc}}?prop owl:onProperty {prop_iri.toRdf} .\n'
                 else:
-                    sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri} as ?prop)\n'
+                    sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri.toRdf} as ?prop)\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?prop dcterms:modified ?modified .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}FILTER(?modified = {modified.toRdf})\n'
                 sparql += f'{blank:{indent * indent_inc}}}}'
-            minmax_done = True
+                minmax_done = True
         return sparql
 
     def delete_shacl(self, *,
                      graph: Xsd_NCName,
-                     owlclass_iri: Optional[Xsd_QName] = None,
-                     prop_iri: Xsd_QName,
+                     owlclass_iri: Iri | None = None,
+                     prop_iri: Iri,
                      restriction_type: PropertyRestrictionType,
                      indent: int = 0, indent_inc: int = 4) -> str:
         # TODO: Include into unittest!
         blank = ''
         sparql = f'WITH {graph}:shacl\n'
         if restriction_type == PropertyRestrictionType.LANGUAGE_IN or restriction_type == PropertyRestrictionType.MIN_COUNT:
             sparql += f'{blank:{indent*indent_inc}}DELETE {{\n'
             sparql += f'{blank:{(indent + 1)*indent_inc}}?z rdf:first ?head ;\n'
             sparql += f'{blank:{(indent + 2)*indent_inc}}rdf:rest ?tail .\n'
             sparql += f'{blank:{indent*indent_inc}}}}\n'
             sparql += f'{blank:{indent*indent_inc}}WHERE {{\n'
             if owlclass_iri:
                 sparql += f'{blank:{(indent + 1)*indent_inc}}{owlclass_iri}Shape sh:property ?prop .\n'
-                sparql += f'{blank:{(indent + 1)*indent_inc}}?prop sh:path {prop_iri} .\n'
+                sparql += f'{blank:{(indent + 1)*indent_inc}}?prop sh:path {prop_iri.toRdf} .\n'
             else:
-                sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri} as ?prop)\n'
+                sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri.toRdf} as ?prop)\n'
             sparql += f'{blank:{(indent + 1)*indent_inc}}?prop {restriction_type.value} ?bnode .\n'
             sparql += f'{blank:{(indent + 1)*indent_inc}}?bnode rdf:rest* ?z .\n'
             sparql += f'{blank:{(indent + 1)*indent_inc}}?z rdf:first ?head ;\n'
             sparql += f'{blank:{(indent + 1)*indent_inc}}rdf:rest ?tail .\n'
             sparql += f'{blank:{indent*indent_inc}}}} ;\n'
 
         sparql += f'{blank:{indent*indent_inc}}DELETE {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}?prop {restriction_type.value} ?rval .\n'
         sparql += f'{blank:{indent*indent_inc}}}}\n'
         sparql += f'{blank:{indent*indent_inc}}WHERE {{\n'
         if owlclass_iri:
             sparql += f'{blank:{(indent + 1)*indent_inc}}{owlclass_iri}Shape sh:property ?prop .\n'
-            sparql += f'{blank:{(indent + 1)*indent_inc}}?prop sh:path {prop_iri} .\n'
+            sparql += f'{blank:{(indent + 1)*indent_inc}}?prop sh:path {prop_iri.toRdf} .\n'
         else:
-            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri} as ?prop)\n'
+            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({prop_iri.toRdf} as ?prop)\n'
         sparql += f'{blank:{(indent + 1)*indent_inc}}?prop {restriction_type.value} ?rval\n'
         sparql += f'{blank:{indent*indent_inc}}}}\n'
         return sparql
 
     def delete_owl(self, indent: int = 0, indent_inc: int = 4):
         # TODO: Include into unittest!
         pass
```

### Comparing `omaslib-0.1.8/omaslib/src/resourceclass.py` & `omaslib-0.1.9/omaslib/src/resourceclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,155 +1,175 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Union, Optional, List, Dict, Callable
+from functools import partial
+from typing import Union, Optional, List, Dict, Callable, Self
 from pystrict import strict
 
 from omaslib.src.helpers.Notify import Notify
 from omaslib.src.helpers.omaserror import OmasError, OmasErrorNotFound, OmasErrorAlreadyExists, OmasErrorInconsistency, OmasErrorUpdateFailed
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.helpers.query_processor import QueryProcessor
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.enums.resourceclassattr import ResourceClassAttribute
 from omaslib.src.helpers.semantic_version import SemanticVersion
 from omaslib.src.helpers.tools import RdfModifyRes, RdfModifyItem
 from omaslib.src.enums.xsd_datatypes import XsdDatatypes
 from omaslib.src.dtypes.bnode import BNode
 from omaslib.src.enums.action import Action
-from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
-from omaslib.src.xsd.xsd_qname import Xsd_QName
+from omaslib.src.xsd.iri import Iri
+from omaslib.src.xsd.xsd_boolean import Xsd_boolean
+from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.helpers.langstring import LangString
 from omaslib.src.helpers.context import Context
 from omaslib.src.iconnection import IConnection
 from omaslib.src.model import Model
 from omaslib.src.propertyclass import PropertyClass, Attributes
 
 #
 # Datatype definitions
 #
-AttributeTypes = Union[Xsd_QName, LangString, bool, None]
+AttributeTypes = Union[Iri, LangString, Xsd_boolean, None]
 ResourceClassAttributesContainer = Dict[ResourceClassAttribute, AttributeTypes]
 Properties = Dict[BNode, Attributes]
 
 
 @dataclass
 class ResourceClassAttributeChange:
-    old_value: Union[AttributeTypes, PropertyClass, Xsd_QName, None]
+    old_value: Union[AttributeTypes, PropertyClass, Iri, None]
     action: Action
     test_in_use: bool
 
+
 @dataclass
 class ResourceClassPropertyChange:
-    old_value: Union[PropertyClass, Xsd_QName, None]
+    old_value: Union[PropertyClass, Iri, None]
     action: Action
     test_in_use: bool
 
 
 @strict
 class ResourceClass(Model, Notify):
     _graph: Xsd_NCName
-    _owlclass_iri: Union[Xsd_QName, None]
+    _owlclass_iri: Iri | None
     _attributes: ResourceClassAttributesContainer
-    _properties: Dict[Xsd_QName, PropertyClass]
+    _properties: Dict[Iri, PropertyClass]
     _attr_changeset: Dict[ResourceClassAttribute, ResourceClassAttributeChange]
-    _prop_changeset: Dict[Xsd_QName, ResourceClassPropertyChange]
-    __creator: Optional[Xsd_anyURI]
-    __created: Optional[datetime]
-    __contributor: Optional[Xsd_anyURI]
-    __modified: Optional[datetime]
+    _prop_changeset: Dict[Iri, ResourceClassPropertyChange]
+    __creator: Iri | None
+    __created: Xsd_dateTime | None
+    __contributor: Iri | None
+    __modified: Xsd_dateTime | None
     __version: SemanticVersion
     __from_triplestore: bool
 
-    __datatypes: Dict[ResourceClassAttribute, Union[Xsd_QName, LangString, bool]] = {
-        ResourceClassAttribute.SUBCLASS_OF: Xsd_QName,
+    __datatypes: Dict[ResourceClassAttribute, Union[Iri, LangString, Xsd_boolean]] = {
+        ResourceClassAttribute.SUBCLASS_OF: Iri,
         ResourceClassAttribute.LABEL: LangString,
         ResourceClassAttribute.COMMENT: LangString,
-        ResourceClassAttribute.CLOSED: bool
+        ResourceClassAttribute.CLOSED: Xsd_boolean
     }
 
     def __init__(self, *,
                  con: IConnection,
                  graph: Xsd_NCName,
-                 owlclass_iri: Optional[Xsd_QName] = None,
-                 attrs: Optional[ResourceClassAttributesContainer] = None,
-                 properties: Optional[List[Union[PropertyClass, Xsd_QName]]] = None,
-                 notifier: Optional[Callable[[PropertyClassAttribute], None]] = None,
-                 notify_data: Optional[PropertyClassAttribute] = None):
+                 owlclass_iri: Iri | str |None = None,
+                 subClassOf: Iri | str | None = None,
+                 label: LangString | str | None = None,
+                 comment: LangString | str | None = None,
+                 closed: Xsd_boolean | bool | None = None,
+                 properties: List[PropertyClass | Iri] | None = None,
+                 notifier: Callable[[PropClassAttr], None] | None = None,
+                 notify_data: PropClassAttr | None = None):
         Model.__init__(self, con)
         Notify.__init__(self, notifier, notify_data)
-        self._graph = graph
-        self._owlclass_iri = owlclass_iri
+        self._graph = graph if isinstance(graph, Xsd_NCName) else Xsd_NCName(graph)
+
+        self._attributes = {}
+        if isinstance(owlclass_iri, Iri):
+            self._owlclass_iri = owlclass_iri
+        elif owlclass_iri is not None:
+            self._owlclass_iri = Iri(owlclass_iri)
+        else:
+            self._owlclass_iri = None
+        if subClassOf is not None:
+            self._attributes[ResourceClassAttribute.SUBCLASS_OF] = subClassOf if isinstance(subClassOf, Iri) else Iri(subClassOf)
+        if label is not None:
+            self._attributes[ResourceClassAttribute.LABEL] = label if isinstance(label, LangString) else LangString(label)
+        if comment is not None:
+            self._attributes[ResourceClassAttribute.COMMENT] = comment if isinstance(comment, LangString) else LangString(comment)
+        if closed is not None:
+            self._attributes[ResourceClassAttribute.CLOSED] = closed if isinstance(closed, Xsd_boolean) else Xsd_boolean(closed)
         self.__creator = con.userIri
         self.__created = None
         self.__contributor = con.userIri
         self.__modified = None
         self.__version = SemanticVersion()
-        self._attributes = {}
-        if attrs is not None:
-            for attr, value in attrs.items():
-                if (attr == ResourceClassAttribute.LABEL or attr == ResourceClassAttribute.COMMENT) and type(value) != LangString:
-                    raise OmasError(f'Attribute "{attr.value}" must be a "LangString", but is "{type(value)}"!')
-                if attr == ResourceClassAttribute.SUBCLASS_OF and type(value) != Xsd_QName:
-                    raise OmasError(f'Attribute "{attr.value}" must be a "QName", but is "{type(value)}"!')
-                if attr == ResourceClassAttribute.CLOSED and type(value) != bool:
-                    raise OmasError(f'Attribute "{attr.value}" must be a "bool", but is "{type(value)}"!')
-                if getattr(value, 'set_notifier', None) is not None:
-                    value.set_notifier(self.notifier, attr)
-                self._attributes[attr] = value
         self._properties = {}
         if properties is not None:
             for prop in properties:
-                newprop: Union[PropertyClass, Xsd_QName]
-                if isinstance(prop, Xsd_QName):  # Reference to an external, standalone property definition
-                    fixed_prop = Xsd_QName(str(prop).removesuffix("Shape"))
+                newprop: PropertyClass | Iri | None = None
+                if isinstance(prop, Iri):  # Reference to an external, standalone property definition
+                    fixed_prop = Iri(str(prop).removesuffix("Shape"))
                     try:
                         newprop = PropertyClass.read(self._con, self._graph, fixed_prop)
                     except OmasErrorNotFound as err:
                         newprop = fixed_prop
                 elif isinstance(prop, PropertyClass):  # an internal, private property definition
                     if not prop._force_external:
                         prop._internal = owlclass_iri
                     newprop = prop
-                self._properties[newprop.property_class_iri] = newprop
-                newprop.set_notifier(self.notifier, newprop.property_class_iri)
+                else:
+                    newprop = None
+                if newprop is not None:
+                    self._properties[newprop.property_class_iri] = newprop
+                    newprop.set_notifier(self.notifier, newprop.property_class_iri)
+        for attr in ResourceClassAttribute:
+            prefix, name = attr.value.split(':')
+            setattr(ResourceClass, name, property(
+                partial(ResourceClass.__get_value, attr=attr),
+                partial(ResourceClass.__set_value, attr=attr),
+                partial(ResourceClass.__del_value, attr=attr)))
+
         self._attr_changeset = {}
         self._prop_changeset = {}
         self.__from_triplestore = False
 
-    def __getitem__(self, key: Union[ResourceClassAttribute, Xsd_QName]) -> Union[AttributeTypes, PropertyClass, Xsd_QName]:
-        if isinstance(key, ResourceClassAttribute):
-            return self._attributes[key]
-        elif isinstance(key, Xsd_QName):
-            return self._properties[key]
-        else:
-            raise ValueError(f'Invalid key type {type(key)} of key {key}')
+    def __get_value(self: Self, attr: ResourceClassAttribute) -> AttributeTypes | PropertyClass | Iri | None:
+        return self.__getter(attr)
 
-    def get(self, key: Union[ResourceClassAttribute, Xsd_QName]) -> Union[AttributeTypes, PropertyClass, Xsd_QName, None]:
+    def __set_value(self: Self, attr: ResourceClassAttribute, value: AttributeTypes | PropertyClass | Iri) -> None:
+        self.__setter(attr, value)
+
+    def __del_value(self: Self, attr: ResourceClassAttribute) -> None:
+        self.__deleter(attr)
+
+    def __getter(self, key: ResourceClassAttribute | Iri) -> AttributeTypes | PropertyClass | Iri:
         if isinstance(key, ResourceClassAttribute):
             return self._attributes.get(key)
-        elif isinstance(key, Xsd_QName):
+        elif isinstance(key, Iri):
             return self._properties.get(key)
         else:
             return None
 
-    def __setitem__(self, key: Union[ResourceClassAttribute, Xsd_QName], value: Union[AttributeTypes, PropertyClass, Xsd_QName]) -> None:
-        if type(key) not in {ResourceClassAttribute, PropertyClass, Xsd_QName}:
+    def __setter(self, key: ResourceClassAttribute | Iri, value: AttributeTypes | PropertyClass | Iri) -> None:
+        if type(key) not in {ResourceClassAttribute, PropertyClass, Iri}:
             raise ValueError(f'Invalid key type {type(key)} of key {key}')
         if getattr(value, 'set_notifier', None) is not None:
             value.set_notifier(self.notifier, key)
         if isinstance(key, ResourceClassAttribute):
             if self._attributes.get(key) is None:  # Attribute not yet set
                 self._attr_changeset[key] = ResourceClassAttributeChange(None, Action.CREATE, False)  # TODO: Check if "check_in_use" must be set
             else:
                 if self._attr_changeset.get(key) is None:  # Only first change is recorded
                     self._attr_changeset[key] = ResourceClassAttributeChange(self._attributes[key], Action.REPLACE, False)  # TODO: Check if "check_in_use" must be set
                 else:
                     self._attr_changeset[key] = ResourceClassAttributeChange(self._attr_changeset[key].old_value, Action.REPLACE, False)  # TODO: Check if "check_in_use" must be set
             self._attributes[key] = value
-        elif isinstance(key, Xsd_QName):  # QName
+        elif isinstance(key, Iri):  # Iri
             if self._properties.get(key) is None:  # Property not set -> CREATE action
                 self._prop_changeset[key] = ResourceClassPropertyChange(None, Action.CREATE, False)
                 if value is None:
                     try:
                         self._properties[key] = PropertyClass.read(self._con, graph=self._graph, property_class_iri=key)
                     except OmasErrorNotFound as err:
                         self._properties[key] = key
@@ -167,55 +187,75 @@
                         self._properties[key] = PropertyClass.read(self._con, graph=self._graph, property_class_iri=key)
                     except OmasErrorNotFound as err:
                         self._properties[key] = key
                 else:
                     value._internal = self._owlclass_iri  # we need to access the private variable here
                     value._property_class_iri = key  # we need to access the private variable here
                     self._properties[key] = value
+        else:
+            raise OmasError(f'Invalid key type {type(key).__name__} of key {key}')
         self.notify()
 
-    def __delitem__(self, key: Union[ResourceClassAttribute, Xsd_QName]) -> None:
-        if type(key) not in {ResourceClassAttribute, Xsd_QName}:
-            raise ValueError(f'Invalid key type {type(key)} of key {key}')
+    def __deleter(self, key: ResourceClassAttribute | Iri) -> None:
+        if not isinstance(key, (ResourceClassAttribute, Iri)):
+            raise ValueError(f'Invalid key type {type(key).__name__} of key {key}')
         if isinstance(key, ResourceClassAttribute):
             if self._attr_changeset.get(key) is None:
                 self._attr_changeset[key] = ResourceClassAttributeChange(self._attributes[key], Action.DELETE, False)
             else:
                 self._attr_changeset[key] = ResourceClassAttributeChange(self._attr_changeset[key].old_value, Action.DELETE, False)
             del self._attributes[key]
-        elif isinstance(key, Xsd_QName):
+        elif isinstance(key, Iri):
             if self._prop_changeset.get(key) is None:
                 self._prop_changeset[key] = ResourceClassPropertyChange(self._properties[key], Action.DELETE, False)
             else:
                 self._prop_changeset[key] = ResourceClassPropertyChange(self._prop_changeset[key].old_value, Action.DELETE, False)
             del self._properties[key]
         self.notify()
 
+
+    def __getitem__(self, key: ResourceClassAttribute | Iri) -> AttributeTypes | PropertyClass | Iri:
+        return self.__getter(key)
+
+    def get(self, key: ResourceClassAttribute | Iri) -> AttributeTypes | PropertyClass | Iri | None:
+        if isinstance(key, ResourceClassAttribute):
+            return self._attributes.get(key)
+        elif isinstance(key, Iri):
+            return self._properties.get(key)
+        else:
+            return None
+
+    def __setitem__(self, key: ResourceClassAttribute | Iri, value: AttributeTypes | PropertyClass | Iri) -> None:
+        self.__setter(key, value)
+
+    def __delitem__(self, key: ResourceClassAttribute | Iri) -> None:
+        self.__deleter(key)
+
     @property
-    def owl_class_iri(self) -> Xsd_QName:
+    def owl_class_iri(self) -> Iri:
         return self._owlclass_iri
 
     @property
     def version(self) -> SemanticVersion:
         return self.__version
 
     @property
-    def creator(self) -> Optional[Xsd_anyURI]:
+    def creator(self) -> Iri | None:
         return self.__creator
 
     @property
-    def created(self) -> Optional[datetime]:
+    def created(self) -> Xsd_dateTime | None:
         return self.__created
 
     @property
-    def contributor(self) -> Optional[Xsd_anyURI]:
+    def contributor(self) -> Iri | None:
         return self.__contributor
 
     @property
-    def modified(self) -> Optional[datetime]:
+    def modified(self) -> Xsd_dateTime | None:
         return self.__modified
 
     def properties_items(self):
         return self._properties.items()
 
     def attributes_items(self):
         return self._attributes.items()
@@ -239,18 +279,18 @@
                 self._attributes[attr].changeset_clear()
         self._attr_changeset = {}
         for prop, change in self._prop_changeset.items():
             if change.action == Action.MODIFY:
                 self._properties[prop].changeset_clear()
         self._prop_changeset = {}
 
-    def notifier(self, what: ResourceClassAttribute | Xsd_QName):
+    def notifier(self, what: ResourceClassAttribute | Iri):
         if isinstance(what, ResourceClassAttribute):
             self._attr_changeset[what] = ResourceClassAttributeChange(None, Action.MODIFY, True)
-        elif isinstance(what, Xsd_QName):
+        elif isinstance(what, Iri):
             self._prop_changeset[what] = ResourceClassPropertyChange(None, Action.MODIFY, True)
         self.notify()
 
     @property
     def in_use(self) -> bool:
         context = Context(name=self._con.context_name)
         query = context.sparql_context
@@ -268,15 +308,15 @@
         for r in res:
             if int(r.nresinstances) > 0:
                 return True
             else:
                 return False
 
     @staticmethod
-    def __query_shacl(con: IConnection, graph: Xsd_NCName, owl_class_iri: Xsd_QName) -> Attributes:
+    def __query_shacl(con: IConnection, graph: Xsd_NCName, owl_class_iri: Iri) -> Attributes:
         context = Context(name=con.context_name)
         query = context.sparql_context
         query += f"""
         SELECT ?attriri ?value
         FROM {graph}:shacl
         WHERE {{
             BIND({owl_class_iri}Shape AS ?shape)
@@ -294,19 +334,19 @@
                     continue
                 if tmp_owl_class_iri != owl_class_iri:
                     raise OmasError(f'Inconsistent Shape for "{owl_class_iri}": rdf:type="{tmp_owl_class_iri}"')
             elif attriri == 'sh:property':
                 continue  # processes later – points to a BNode containing
             else:
                 attriri = r['attriri']
-                if isinstance(r['value'], Xsd_QName):
+                if isinstance(r['value'], Iri):
                     if attributes.get(attriri) is None:
                         attributes[attriri] = []
                     attributes[attriri].append(r['value'])
-                elif isinstance(r['value'], OldapStringLiteral):
+                elif isinstance(r['value'], StringLiteral):
                     if attributes.get(attriri) is None:
                         attributes[attriri] = []
                     attributes[attriri].append(str(r['value']))
                 elif isinstance(r['value'], BNode):
                     pass
                 else:
                     if attributes.get(attriri) is None:
@@ -326,29 +366,29 @@
                 self.__created = val[0]
             elif key == 'dcterms:contributor':
                 self.__contributor = val[0]
             elif key == 'dcterms:modified':
                 self.__modified = val[0]
             else:
                 attr = ResourceClassAttribute(key)
-                if Xsd_QName == self.__datatypes[attr]:
+                if Iri == self.__datatypes[attr]:
                     self._attributes[attr] = val[0]  # is already QName or AnyIRI from preprocessing
                 elif XsdDatatypes == self.__datatypes[attr]:
                     self._attributes[attr] = XsdDatatypes(str(val[0]))
                 elif LangString == self.__datatypes[attr]:
                     self._attributes[attr] = LangString(val)
-                elif bool == self.__datatypes[attr]:
+                elif Xsd_boolean == self.__datatypes[attr]:
                     self._attributes[attr] = bool(val[0])
                 if getattr(self._attributes[attr], 'set_notifier', None) is not None:
                     self._attributes[attr].set_notifier(self.notifier, attr)
 
         self.__from_triplestore = True
 
     @staticmethod
-    def __query_resource_props(con: IConnection, graph: Xsd_NCName, owlclass_iri: Xsd_QName) -> List[Union[PropertyClass, Xsd_QName]]:
+    def __query_resource_props(con: IConnection, graph: Xsd_NCName, owlclass_iri: Iri) -> List[PropertyClass | Iri]:
         """
         This method queries and returns a list of properties defined in a sh:NodeShape. The properties may be
         given "inline" as BNode or may be a reference to an external sh:PropertyShape. These external shapes will be
         read when the ResourceClass is constructed (see __init__() of ResourceClass).
 
         :param con: IConnection instance
         :param graph: Name of the graph
@@ -370,44 +410,44 @@
                     ?value rdf:rest*/rdf:first ?oo
                 }}
             }}
         }}
         """
         jsonobj = con.query(query)
         res = QueryProcessor(context=context, query_result=jsonobj)
-        propinfos: Dict[Xsd_QName, Attributes] = {}
+        propinfos: Dict[Iri, Attributes] = {}
         #
         # first we run over all triples to gather the information about the properties of the possible
         # BNode based sh:property-Shapes.
         # NOTE: some of the nodes may actually be QNames referencing shapes defines as "standalone" sh:PropertyShape's.
         #
         for r in res:
-            if r['value'] == 'rdf:type':
+            if isinstance(r['value'], Iri) and r['value'] == 'rdf:type':
                 continue
-            if not isinstance(r['attriri'], Xsd_QName):
+            if not isinstance(r['attriri'], Iri):
                 raise OmasError(f"There is some inconsistency in this shape! ({r['attriri']})")
             propnode = r['prop']  # usually a BNode, but may be a reference to a standalone sh:PropertyShape definition
-            prop: Union[PropertyClass, Xsd_QName]
-            if isinstance(propnode, Xsd_QName):
+            prop: PropertyClass | Iri
+            if isinstance(propnode, Iri):
                 qname = propnode
                 propinfos[qname] = propnode
             elif isinstance(propnode, BNode):
                 if propinfos.get(propnode) is None:
                     propinfos[propnode]: Attributes = {}
                 attributes: Attributes = propinfos[propnode]
                 PropertyClass.process_triple(r, propinfos[propnode])
             else:
                 raise OmasError(f'Unexpected type for propnode in SHACL. Type = "{type(propnode)}".')
         #
         # now we collected all the information from the triple store. Let's process the information into
         # a list of full PropertyClasses or QName's to external definitions
         #
-        proplist: List[Union[Xsd_QName, PropertyClass]] = []
+        proplist: List[Iri | PropertyClass] = []
         for prop_iri, attributes in propinfos.items():
-            if isinstance(attributes, Xsd_QName):
+            if isinstance(attributes, Iri):
                 proplist.append(prop_iri)
             else:
                 prop = PropertyClass(con=con, graph=graph)
                 prop.parse_shacl(attributes=attributes)
                 prop.read_owl()
                 if prop._internal != owlclass_iri:
                     OmasErrorInconsistency(f'ERRROR ERROR ERROR')
@@ -456,17 +496,17 @@
             property_iri = pp['property_iri']
             prop = [x for x in self._properties if x == property_iri]
             if len(prop) != 1:
                 OmasError(f'Property "{property_iri}" from OWL has no SHACL definition!')
             self._properties[prop[0]].prop.read_owl()
 
     @classmethod
-    def read(cls, con: IConnection, graph: Xsd_NCName, owl_class_iri: Xsd_QName) -> 'ResourceClass':
+    def read(cls, con: IConnection, graph: Xsd_NCName, owl_class_iri: Iri) -> 'ResourceClass':
         attributes = ResourceClass.__query_shacl(con, graph=graph, owl_class_iri=owl_class_iri)
-        properties: List[Union[PropertyClass, Xsd_QName]] = ResourceClass.__query_resource_props(con=con, graph=graph, owlclass_iri=owl_class_iri)
+        properties: List[Union[PropertyClass, Iri]] = ResourceClass.__query_resource_props(con=con, graph=graph, owlclass_iri=owl_class_iri)
         resclass = cls(con=con, graph=graph, owlclass_iri=owl_class_iri, properties=properties)
         for prop in properties:
             if isinstance(prop, PropertyClass):
                 prop.set_notifier(resclass.notifier, prop.property_class_iri)
         resclass._parse_shacl(attributes=attributes)
         resclass.__read_owl()
         return resclass
@@ -503,40 +543,38 @@
         sparql += f"{blank:{indent * indent_inc}}}}"
         jsonobj = self._con.transaction_query(sparql)
         res = QueryProcessor(context, jsonobj)
         if len(res) != 1:
             return None
         return res[0].get('modified')
 
-    def create_shacl(self, timestamp: datetime, indent: int = 0, indent_inc: int = 4) -> str:
+    def create_shacl(self, timestamp: Xsd_dateTime, indent: int = 0, indent_inc: int = 4) -> str:
         blank = ''
         sparql = ''
         # for iri, p in self._properties.items():
         #     if p.internal is None and not p.from_triplestore:
         #         #sparql += p.create_shacl(timestamp=timestamp)
         #         sparql += f'{blank:{(indent + 2)*indent_inc}}{iri}Shape a sh:PropertyShape ;\n'
         #         sparql += p.property_node_shacl(timestamp=timestamp, indent=3) + " .\n"
         #         sparql += "\n"
 
-        sparql += f'{blank:{(indent + 1)*indent_inc}}{self._owlclass_iri}Shape a sh:NodeShape, {self._owlclass_iri}'
-        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}sh:targetClass {self._owlclass_iri}'
+        sparql += f'{blank:{(indent + 1)*indent_inc}}{self._owlclass_iri}Shape a sh:NodeShape, {self._owlclass_iri.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}sh:targetClass {self._owlclass_iri.toRdf}'
         sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:hasVersion "{self.__version}"'
         self.__created = timestamp
-        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:created "{timestamp.isoformat()}"^^xsd:dateTime'
-        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:creator <{self.__creator}>'
+        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:created {timestamp.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:creator {self.__creator.toRdf}'
         self.__modified = timestamp
-        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:modified "{timestamp.isoformat()}"^^xsd:dateTime'
-        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:contributor <{self.__contributor}>'
+        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:modified {timestamp.toRdf}'
+        sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}dcterms:contributor {self.__contributor.toRdf}'
         for attr, value in self._attributes.items():
             if attr == ResourceClassAttribute.SUBCLASS_OF:
                 sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}{attr.value} {value}Shape'
-            elif attr == ResourceClassAttribute.CLOSED:
-                sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}sh:closed {"true" if value else "false"}'
             else:
-                sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}{attr.value} {value}'
+                sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}{attr.value} {value.toRdf}'
 
         sparql += f' ;\n{blank:{(indent + 2) * indent_inc}}sh:property'
         sparql += f'\n{blank:{(indent + 3) * indent_inc}}['
         sparql += f'\n{blank:{(indent + 4) * indent_inc}}sh:path rdf:type'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}]'
 
         for iri, p in self._properties.items():
@@ -547,27 +585,27 @@
                 sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}]'
             else:
                 sparql += f' ;\n{blank:{(indent + 2)*indent_inc}}sh:property {iri}Shape'
         if len(self._properties) > 0:
             sparql += ' .\n'
         return sparql
 
-    def create_owl(self, timestamp: datetime, indent: int = 0, indent_inc: int = 4):
+    def create_owl(self, timestamp: Xsd_dateTime, indent: int = 0, indent_inc: int = 4):
         blank = ''
         sparql = ''
         for iri, p in self._properties.items():
             if not p.from_triplestore:
                 sparql += p.create_owl_part1(timestamp, indent + 2) + '\n'
 
         sparql += f'{blank:{(indent + 2) * indent_inc}}{self._owlclass_iri} rdf:type owl:Class ;\n'
         sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:hasVersion "{self.__version}" ;\n'
-        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:created "{timestamp.isoformat()}"^^xsd:dateTime ;\n'
-        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:creator <{self.__creator}> ;\n'
-        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:modified "{timestamp.isoformat()}"^^xsd:dateTime ;\n'
-        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:contributor <{self.__contributor}> ;\n'
+        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:created {timestamp.toRdf} ;\n'
+        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:creator {self.__creator.toRdf} ;\n'
+        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:modified {timestamp.toRdf} ;\n'
+        sparql += f'{blank:{(indent + 3) * indent_inc}}dcterms:contributor {self.__contributor.toRdf} ;\n'
         if self._attributes.get(ResourceClassAttribute.SUBCLASS_OF) is not None:
             sparql += f'{blank:{(indent + 3)*indent_inc}}rdfs:subClassOf {self._attributes[ResourceClassAttribute.SUBCLASS_OF]} ,\n'
         else:
             sparql += f'{blank:{(indent + 3)*indent_inc}}rdfs:subClassOf\n'
         i = 0
         for iri, p in self._properties.items():
             sparql += p.create_owl_part2(indent + 4)
@@ -585,15 +623,15 @@
         self.__contributor = self._con.userIri
         self.__from_triplestore = True
 
 
     def create(self, indent: int = 0, indent_inc: int = 4) -> None:
         if self.__from_triplestore:
             raise OmasErrorAlreadyExists(f'Cannot create property that was read from triplestore before (property: {self._owlclass_iri}')
-        timestamp = datetime.now()
+        timestamp = Xsd_dateTime.now()
         blank = ''
         context = Context(name=self._con.context_name)
         sparql = context.sparql_context
         sparql += f'{blank:{indent * indent_inc}}INSERT DATA {{\n'
 
         sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH {self._graph}:shacl {{\n'
         sparql += self.create_shacl(timestamp=timestamp)
@@ -795,15 +833,15 @@
                     # TODO: Add here the OWL rdfs:subClassOf to the owl ontology
             elif change.action == Action.REPLACE:
                 if change.old_value.internal is not None:
                     change.old_value.delete()
                 if not self._properties[prop].from_triplestore:
                     self._properties[prop].create()
                 else:
-                    if self._properties[prop].get(PropertyClassAttribute.EXCLUSIVE_FOR) is None:
+                    if self._properties[prop].get(PropClassAttr.EXCLUSIVE_FOR) is None:
                         continue  # TODO: replace reference in __update_shacl and __update_owl
                     else:
                         raise OmasErrorInconsistency(f'Property is exclusive – simple reference not allowed')
             elif change.action == Action.MODIFY:
                 self._properties[prop].update()
             elif change.action == Action.DELETE:
                 if change.old_value.internal is not None:
```

### Comparing `omaslib-0.1.8/omaslib/src/user.py` & `omaslib-0.1.9/omaslib/src/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,52 +142,52 @@
 """
 
 import uuid
 from datetime import datetime
 from typing import List, Self, Dict, Set, Optional
 
 from omaslib.src.helpers.context import Context
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_boolean import Xsd_boolean
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_string import Xsd_string
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
 from omaslib.src.helpers.omaserror import OmasError, OmasErrorAlreadyExists, OmasErrorNotFound, OmasErrorUpdateFailed, \
     OmasErrorValue, OmasErrorNoPermission
 from omaslib.src.helpers.query_processor import QueryProcessor
 from omaslib.src.enums.permissions import AdminPermission
-from omaslib.src.helpers.tools import lprint, str2qname_anyiri
+from omaslib.src.helpers.tools import str2qname_anyiri, lprint
 from omaslib.src.iconnection import IConnection
 from omaslib.src.model import Model
 from omaslib.src.user_dataclass import UserDataclass
 
 
 # @serializer
 class User(Model, UserDataclass):
     """
     The OLDAP user class is based on the [UserDataclass](/python_docstrings/userdataclass#UserDataclass). It implements together with the UserDataclass
     all the methods ot manage OLDAP users. I also uses the [InProject](/python_docstrings/in_project) class.
     """
 
     def __init__(self, *,
                  con: IConnection | None = None,
-                 creator: Xsd_anyURI | str | None = None,
+                 creator: Iri | str | None = None,
                  created: Xsd_dateTime | str | str | None = None,
-                 contributor: Xsd_anyURI | str | None = None,
+                 contributor: Iri | str | None = None,
                  modified: Xsd_dateTime | str | None = None,
-                 userIri: Xsd_anyURI | str | None = None,
+                 userIri: Iri | str | None = None,
                  userId: Xsd_NCName | str | None = None,
                  familyName: Xsd_string | str | None = None,
                  givenName: Xsd_string | str | None = None,
                  credentials: Xsd_string | str | str | None = None,
                  isActive: Xsd_boolean | bool | None = None,
-                 inProject: Dict[Xsd_QName | Xsd_anyURI, Set[AdminPermission]] | None = None,
-                 hasPermissions: Set[Xsd_QName] | None = None):
+                 inProject: Dict[Iri, Set[AdminPermission]] | None = None,
+                 hasPermissions: Set[Iri] | None = None):
         """
         Constructor for the User class
         :param con: IConnection instance
         :type con: IConnection | None
         :param creator: AnyIRI of the creator
         :type creator: Xsd_anyURI | None
         :param created: DateTime of the creation of the user
@@ -210,15 +210,15 @@
         :type isActive: bool
         :param inProject: Membership and admin permissions the user has in the given projects
         :type inProject: InProjectType
         :param hasPermissions: IConnection to permission sets
         :type hasPermissions: PermissionSet
         """
         if userIri is None:
-            userIri = Xsd_anyURI(uuid.uuid4().urn)
+            userIri = Iri()
         Model.__init__(self, connection=con)
         UserDataclass.__init__(self,
                                creator=creator,
                                created=created,
                                contributor=contributor,
                                modified=modified,
                                userIri=userIri,
@@ -244,27 +244,27 @@
         if self._con is None:
             raise OmasError("Cannot create: no connection")
         #
         # First we check if the logged-in user ("actor") has the permission to create a user for
         # the given project!
         #
         actor = self._con.userdata
-        sysperms = actor.inProject.get(Xsd_QName('omas:SystemProject'))
+        sysperms = actor.inProject.get(Iri('omas:SystemProject'))
         is_root: bool = False
         if sysperms and AdminPermission.ADMIN_OLDAP in sysperms:
             is_root = True
         if not is_root:
             for proj in self.inProject.keys():
                 if actor.inProject.get(proj) is None:
                     raise OmasErrorNoPermission(f'No permission to create user in project {proj}.')
                 if AdminPermission.ADMIN_USERS not in actor.inProject.get(proj):
                     raise OmasErrorNoPermission(f'No permission to create user in project {proj}.')
 
         if self.userIri is None:
-            self.userIri = Xsd_anyURI(uuid.uuid4().urn)
+            self.userIri = Iri()
         context = Context(name=self._con.context_name)
         sparql1 = context.sparql_context
         sparql1 += f"""
         SELECT ?user
         FROM omas:admin
         WHERE {{
             ?user a omas:User .
@@ -274,19 +274,19 @@
 
         sparql2 = context.sparql_context
         sparql2 += f"""
         SELECT ?user
         FROM omas:admin
         WHERE {{
             ?user a omas:User .
-            FILTER(?user = {self.userIri.resUri})
+            FILTER(?user = {self.userIri.toRdf})
         }}
         """
 
-        projs = [x.resUri for x in self.inProject.keys()]
+        projs = [x.toRdf for x in self.inProject.keys()]
         projslist = ", ".join(projs)
         proj_test = context.sparql_context
         proj_test += f"""
         SELECT ?project
         FROM omas:admin
         WHERE {{
             ?project a omas:Project .
@@ -308,33 +308,33 @@
 
         timestamp = Xsd_dateTime.now()
         blank = ''
         sparql = context.sparql_context
         sparql += f'{blank:{indent * indent_inc}}INSERT DATA {{\n'
         sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{\n'
 
-        sparql += f'{blank:{(indent + 2) * indent_inc}}{self.userIri.resUri} a omas:User'
-        sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:creator {self._con.userIri.resUri}'
+        sparql += f'{blank:{(indent + 2) * indent_inc}}{self.userIri.toRdf} a omas:User'
+        sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:creator {self._con.userIri.toRdf}'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:created {timestamp.toRdf}'
-        sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:contributor {self._con.userIri.resUri}'
+        sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:contributor {self._con.userIri.toRdf}'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}dcterms:modified {timestamp.toRdf}'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:userId {self.userId.toRdf}'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}foaf:familyName {self.familyName.toRdf}'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}foaf:givenName {self.givenName.toRdf}'
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:credentials {self.credentials.toRdf}'
         activeval = "true" if self.isActive else "false"
         sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:isActive {activeval}'
         star = ''
         if self.inProject:
-            project = [p.resUri for p in self.inProject.keys()]
+            project = [p.toRdf for p in self.inProject.keys()]
             rdfstr = ", ".join(project)
             sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:inProject {rdfstr}'
             for p in self.inProject.keys():
                 for admin_p in self.inProject[p]:  # TODO: May be use .get() instead of [] !!!!!!!!!!!!!!!!!!!!!!!!!
-                    star += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.resUri} omas:inProject {p.resUri}>> omas:hasAdminPermission {admin_p.value} .\n'
+                    star += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.toRdf} omas:inProject {p.toRdf}>> omas:hasAdminPermission {admin_p.value} .\n'
         if self.hasPermissions:
             rdfstr = ", ".join([str(x) for x in self.hasPermissions])
             sparql += f' ;\n{blank:{(indent + 3) * indent_inc}}omas:hasPermissions {rdfstr}'
         sparql += " .\n\n"
         sparql += star
         sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
         sparql += f'{blank:{indent * indent_inc}}}}\n'
@@ -402,28 +402,28 @@
         :return: Self
         :raises OmasErrorNotFound: Required user does ot exist
         """
         if isinstance(userId, str):
             userId = Xsd_NCName(userId)
 
         context = Context(name=con.context_name)
-        jsonobj = con.query(cls.sparql_query(context, userId))
+        jsonobj = con.query(UserDataclass.sparql_query(context, userId))
         res = QueryProcessor(context, jsonobj)
         if len(res) == 0:
             raise OmasErrorNotFound(f'User "{userId}" not found.')
         instance = cls(con=con)
         instance._create_from_queryresult(res)
         return instance
 
     @staticmethod
     def search(*, con: IConnection,
                userId: Optional[Xsd_NCName | str] = None,
                familyName: Optional[str | Xsd_string] = None,
                givenName: Optional[str | Xsd_string] = None,
-               inProject: Optional[Xsd_anyURI | Xsd_QName | str] = None) -> List[Xsd_anyURI]:
+               inProject: Optional[Iri | str] = None) -> List[Xsd_anyURI]:
         """
         Search for a user in the database. The user can be found by the
 
         - userId
         - familyName
         - givenName
         - inProject
@@ -443,16 +443,16 @@
         :return: List of users
         :rtype: List[AnyIRI]
         """
         if userId and not isinstance(userId, Xsd_NCName):
             userId = Xsd_NCName(userId)
         familyName = Xsd_string(familyName) if familyName else None
         givenName = Xsd_string(givenName) if givenName else None
-        if not isinstance(inProject, Xsd_anyURI) and not isinstance(inProject, Xsd_QName):
-            inProject = str2qname_anyiri(inProject) if inProject else None
+        if not isinstance(inProject, Iri):
+            inProject = Iri(inProject) if inProject else None
         context = Context(name=con.context_name)
         sparql = context.sparql_context
         sparql += 'SELECT DISTINCT ?user\n'
         sparql += 'FROM omas:admin\n'
         sparql += 'WHERE {\n'
         sparql += '   ?user a omas:User .\n'
         if userId is not None:
@@ -462,15 +462,15 @@
             sparql += '   ?user foaf:familyName ?family_name .\n'
             sparql += f'   FILTER(STR(?family_name) = {familyName.toRdf})\n'
         if givenName is not None:
             sparql += '   ?user foaf:givenName ?given_name .\n'
             sparql += f'   FILTER(STR(?given_name) = {givenName.toRdf})\n'
         if inProject is not None:
             sparql += '   ?user omas:inProject ?project .\n'
-            sparql += f'   FILTER(?project = {inProject.resUri})\n'
+            sparql += f'   FILTER(?project = {inProject.toRdf})\n'
         sparql += '}\n'
         jsonobj = con.query(sparql)
         res = QueryProcessor(context, jsonobj)
         users = []
         for r in res:
             users.append(r['user'])
         return users
```

### Comparing `omaslib-0.1.8/omaslib/src/user_dataclass.py` & `omaslib-0.1.9/omaslib/src/user_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,43 +28,42 @@
 ## Helper classes
 
 - `UserFieldChange`: Bookkeeping of changes to the fields
 - `UserFields`: Enum class of the data fields provided by the `UserDataclass`
 
 """
 from dataclasses import dataclass
-from datetime import datetime
 from enum import unique, Enum
 from functools import partial
 from typing import Dict, Self, Set, Tuple, Any
 
 import bcrypt
 
 from omaslib.src.helpers.context import Context
 from omaslib.src.enums.action import Action
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_boolean import Xsd_boolean
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_string import Xsd_string
 from omaslib.src.xsd.xsd import Xsd
 from omaslib.src.helpers.observable_set import ObservableSet
 from omaslib.src.helpers.omaserror import OmasErrorAlreadyExists, OmasErrorValue, OmasErrorNotFound
 from omaslib.src.enums.permissions import AdminPermission
 from omaslib.src.helpers.query_processor import QueryProcessor
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.serializer import serializer
-from omaslib.src.helpers.tools import lprint
 from omaslib.src.in_project import InProjectClass
 
 # InProjectType = Dict[str, ObservableSet[AdminPermission]]
 
 
-UserFieldTypes = Xsd | ObservableSet[Xsd_QName] | InProjectClass | str | bool | None
+UserFieldTypes = Xsd | ObservableSet[Iri] | InProjectClass | str | bool | None
 
 
 @dataclass
 class UserFieldChange:
     """
     A dataclass used to represent the changes made to a field.
     """
@@ -138,46 +137,46 @@
     - *UserDataclass(...)*: Constructor method for the class
     - *str()*: String representation of the class for printing
     - *add_project_permission(...)*: If the project does already exists, adds the given permission.
       If the project does not exist, it also adds the project.
     - *remove_project_permission(...)*: Removes the given permission
     """
     __datatypes = {
-        UserFields.USER_IRI: Xsd_anyURI,
+        UserFields.USER_IRI: Iri,
         UserFields.USER_ID: Xsd_NCName,
         UserFields.FAMILY_NAME: Xsd_string,
         UserFields.GIVEN_NAME: Xsd_string,
         UserFields.CREDENTIALS: Xsd_string,
         UserFields.ACTIVE: Xsd_boolean,
         UserFields.IN_PROJECT: dict,
-        UserFields.HAS_PERMISSIONS: ObservableSet[Xsd_QName]
+        UserFields.HAS_PERMISSIONS: ObservableSet[Iri]
     }
 
-    __creator: Xsd_anyURI | None
+    __creator: Iri | None
     __created: Xsd_dateTime | None
-    __contributor: Xsd_anyURI | None
+    __contributor: Iri | None
     __modified: Xsd_dateTime | None
 
     __fields: Dict[UserFields, UserFieldTypes]
 
     __change_set: Dict[UserFields, UserFieldChange]
 
     def __init__(self, *,
-                 creator: Xsd_anyURI | str | None = None,
+                 creator: Iri | str | None = None,
                  created: Xsd_dateTime | str | None = None,
-                 contributor: Xsd_anyURI | str | None = None,
+                 contributor: Iri | str | None = None,
                  modified: Xsd_dateTime | str | None = None,
-                 userIri: Xsd_anyURI | str | None = None,
+                 userIri: Iri | str | None = None,
                  userId: Xsd_NCName | str | None = None,
                  familyName: Xsd_string | str | None = None,
                  givenName: Xsd_string | str | None = None,
                  credentials: Xsd_string | str | None = None,
                  isActive: Xsd_boolean | bool | None = None,
-                 inProject: Dict[Xsd_QName | Xsd_anyURI | str, Set[AdminPermission]] | None = None,
-                 hasPermissions: Set[Xsd_QName] | None = None):
+                 inProject: Dict[Iri | str, Set[AdminPermission]] | None = None,
+                 hasPermissions: Set[Iri] | None = None):
         """
         Constructs a new UserDataclass
         :param creator: AnyIRI of the creator of this UserDataclass
         :param created: datetime of the creation of this UserDataclass
         :param contributor: AnyIRI of the contributor of this UserDataclass
         :param modified: datetime of the modification of this UserDataclass
         :param userIri: AnyIRI of the User to be used for this UserDataclass
@@ -197,19 +196,19 @@
             inProjectTmp = InProjectClass()
         if not isinstance(hasPermissions, ObservableSet):
             hasPermissions = ObservableSet(hasPermissions, on_change=self.__hasPermission_cb)
         if credentials is not None:
             salt = bcrypt.gensalt()
             credentials = Xsd_string(bcrypt.hashpw(str(credentials).encode('utf-8'), salt).decode('utf-8'))
 
-        self.__creator = Xsd_anyURI(creator) if creator else None
+        self.__creator = Iri(creator) if creator else None
         self.__created = Xsd_dateTime(created) if created else None
-        self.__contributor = Xsd_anyURI(contributor) if contributor else None
+        self.__contributor = Iri(contributor) if contributor else None
         self.__modified = Xsd_dateTime(modified) if modified else None
-        self.__fields[UserFields.USER_IRI] = Xsd_anyURI(userIri) if userIri else None
+        self.__fields[UserFields.USER_IRI] = Iri(userIri) if userIri else None
         self.__fields[UserFields.USER_ID] = Xsd_NCName(userId) if userId else None
         self.__fields[UserFields.FAMILY_NAME] = Xsd_string(familyName) if familyName else None
         self.__fields[UserFields.GIVEN_NAME] = Xsd_string(givenName) if givenName else None
         self.__fields[UserFields.CREDENTIALS] = Xsd_string(credentials) if credentials else None
         self.__fields[UserFields.ACTIVE] = Xsd_boolean(isActive) if isActive is not None else None
         self.__fields[UserFields.IN_PROJECT] = inProjectTmp if inProjectTmp is not None else None
         self.__fields[UserFields.HAS_PERMISSIONS] = hasPermissions if hasPermissions is not None else None
@@ -272,15 +271,15 @@
             f'  Has permissions: {self.__fields[UserFields.HAS_PERMISSIONS]}\n'
 
     #
     # The fields of the class can either be accessed using the dict-semantic or as
     # named properties. Here we implement the dict semantic
     #
     def __getitem__(self, item: UserFields) -> UserFieldTypes:
-        if isinstance(self.__fields.get(item), OldapStringLiteral):
+        if isinstance(self.__fields.get(item), StringLiteral):
             return str(self.__fields[item])
         return self.__fields.get(item)
 
     def __setitem__(self, field: UserFields, value: UserFieldTypes) -> None:
         if field == UserFields.CREDENTIALS:
             salt = bcrypt.gensalt()
             value = bcrypt.hashpw(str(value).encode('utf-8'), salt).decode('utf-8')
@@ -335,42 +334,42 @@
     # Callbacks for the `ObservableSet`class. This is used whenever the `hasPermission`or
     # `inProject`properties are being modified
     #
     def __hasPermission_cb(self, oldset: ObservableSet, data: Any = None) -> None:
         if self.__change_set.get(UserFields.HAS_PERMISSIONS) is None:
             self.__change_set[UserFields.HAS_PERMISSIONS] = UserFieldChange(oldset, Action.MODIFY)
 
-    def __inProject_cb(self, key: Xsd_QName | Xsd_anyURI, old: ObservableSet[AdminPermission] | None = None) -> None:
+    def __inProject_cb(self, key: Iri, old: ObservableSet[AdminPermission] | None = None) -> None:
         if self.__change_set.get(UserFields.IN_PROJECT) is None:
             old = None
             if self.__fields.get(UserFields.IN_PROJECT) is not None:
                 old = self.__fields[UserFields.IN_PROJECT].copy()
             self.__change_set[UserFields.IN_PROJECT] = UserFieldChange(old, Action.MODIFY)
 
     @property
-    def creator(self) -> Xsd_anyURI | None:
+    def creator(self) -> Iri | None:
         return self.__creator
 
     @property
     def created(self) -> Xsd_dateTime | None:
         return self.__created
 
     @property
-    def contributor(self) -> Xsd_anyURI | None:
+    def contributor(self) -> Iri | None:
         return self.__contributor
 
     @property
     def modified(self) -> Xsd_dateTime | None:
         return self.__modified
 
     @modified.setter
     def modified(self, value: Xsd_dateTime) -> None:
         self.__modified = value
 
-    def add_project_permission(self, project: Xsd_QName | Xsd_anyURI | str, permission: AdminPermission | None) -> None:
+    def add_project_permission(self, project: Iri | str, permission: AdminPermission | None) -> None:
         """
         Adds a new administraive permission to the user. If the user is not yet member of the project, he
         will automatically become a member.
 
         :param project: Name of the project to add the permission
         :type project: Xsd_QName
         :param permission: The admin permission to be added
@@ -382,25 +381,27 @@
                 self.__change_set[UserFields.IN_PROJECT] = UserFieldChange(self.__fields[UserFields.IN_PROJECT], Action.CREATE)
             self.__fields[UserFields.IN_PROJECT][project] = ObservableSet({permission})
         else:
             if self.__change_set.get(UserFields.IN_PROJECT) is None:
                 self.__change_set[UserFields.IN_PROJECT] = UserFieldChange(self.__fields[UserFields.IN_PROJECT], Action.MODIFY)
             self.__fields[UserFields.IN_PROJECT][project].add(permission)
 
-    def remove_project_permission(self, project: Xsd_QName | Xsd_anyURI | str, permission: AdminPermission | None) -> None:
+    def remove_project_permission(self, project: Iri | str, permission: AdminPermission | None) -> None:
         """
         Remove the given Permission from the user (for the given project)
 
         :param project: Name of the project
         :type project: Xsd_QName
         :param permission: The permission to be removed
         :type permission: AdminPermission | None
         :return:
         """
-        if self.__fields[UserFields.IN_PROJECT].get(str(project)) is None:
+        if not isinstance(project, Iri):
+            project = Iri(project)
+        if self.__fields[UserFields.IN_PROJECT].get(project) is None:
             raise OmasErrorValue(f"Project '{project}' does not exist")
         if self.__change_set.get(UserFields.IN_PROJECT) is None:
             self.__change_set[UserFields.IN_PROJECT] = UserFieldChange(self.__fields[UserFields.IN_PROJECT], Action.MODIFY)
         self.__fields[UserFields.IN_PROJECT][project].remove(permission)
 
     @property
     def changeset(self) -> Dict[UserFields, UserFieldChange]:
@@ -520,15 +521,15 @@
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?user {field.value} {change.old_value.toRdf} .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
             if change.action != Action.DELETE:
                 sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}?user {field.value} {self.__fields[field].toRdf} .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
             sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
-            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self.userIri.resUri} as ?user)\n'
+            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self.userIri.toRdf} as ?user)\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}?user {field.value} {change.old_value.toRdf} .\n'
             sparql += f'{blank:{indent * indent_inc}}}}'
             sparql_list.append(sparql)
         if UserFields.HAS_PERMISSIONS in self.__change_set:
             new_set = self.__fields[UserFields.HAS_PERMISSIONS]
             old_set = self.__change_set[UserFields.HAS_PERMISSIONS].old_value
             added = new_set - old_set
@@ -542,15 +543,15 @@
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
             if added:
                 sparql += f'{blank:{indent * indent_inc}}INSERT {{\n'
                 for perm in added:
                     sparql += f'{blank:{(indent + 1) * indent_inc}}?user omas:hasPermissions {perm} .\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
             sparql += f'{blank:{indent * indent_inc}}WHERE {{\n'
-            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self.userIri.resUri} as ?user)\n'
+            sparql += f'{blank:{(indent + 1) * indent_inc}}BIND({self.userIri.toRdf} as ?user)\n'
             sparql += f'{blank:{(indent + 1) * indent_inc}}?user a omas:User .\n'
             sparql += f'{blank:{indent * indent_inc}}}}'
             if removed or added:
                 sparql_list.append(sparql)
 
             #
             # check if existing :PermissionSet's have been given!
@@ -573,68 +574,68 @@
             changedprojs = self.__fields[UserFields.IN_PROJECT].keys() & self.__change_set[UserFields.IN_PROJECT].old_value.keys()
 
             # add projects
             if addedprojs:
                 sparql = f"{blank:{indent * indent_inc}}INSERT DATA {{\n"
                 sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{\n'
                 for proj in addedprojs:
-                    sparql += f'{blank:{(indent + 2) * indent_inc}}{self.userIri.resUri} omas:inProject {proj.resUri} .\n'
+                    sparql += f'{blank:{(indent + 2) * indent_inc}}{self.userIri.toRdf} omas:inProject {proj.toRdf} .\n'
                     for perm in self.__fields[UserFields.IN_PROJECT][proj]:
-                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.resUri} omas:inProject {proj.resUri}>> omas:hasAdminPermission {perm.value} .\n'
+                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.toRdf} omas:inProject {proj.toRdf}>> omas:hasAdminPermission {perm.value} .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 sparql_list.append(sparql)
 
             # delete projects
             if deletedprojs:
                 sparql = f"{blank:{indent * indent_inc}}DELETE DATA {{\n"
                 sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{\n'
                 for proj in deletedprojs:
-                    sparql += f'{blank:{(indent + 2) * indent_inc}}{self.userIri.resUri} omas:inProject {proj.resUri} .\n'
+                    sparql += f'{blank:{(indent + 2) * indent_inc}}{self.userIri.toRdf} omas:inProject {proj.toRdf} .\n'
                     for perm in self.__change_set[UserFields.IN_PROJECT].old_value[proj]:
-                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.resUri} omas:inProject {proj.resUri}>> omas:hasAdminPermission {perm.value} .\n'
+                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.toRdf} omas:inProject {proj.toRdf}>> omas:hasAdminPermission {perm.value} .\n'
                 sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 sparql_list.append(sparql)
 
             if changedprojs:
                 doit = False
                 sparql = f"{blank:{indent * indent_inc}}INSERT DATA {{\n"
                 sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{\n'
                 for proj in changedprojs:
                     perms = self.__fields[UserFields.IN_PROJECT][proj] - self.__change_set[UserFields.IN_PROJECT].old_value[proj]
                     for perm in perms:
-                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.resUri} omas:inProject {proj.resUri}>> omas:hasAdminPermission {perm.value} .\n'
+                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.toRdf} omas:inProject {proj.toRdf}>> omas:hasAdminPermission {perm.value} .\n'
                         doit = True
                 sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 if doit:
                     sparql_list.append(sparql)
 
                 doit = False
                 sparql = f"{blank:{indent * indent_inc}}DELETE DATA {{\n"
                 sparql += f'{blank:{(indent + 1) * indent_inc}}GRAPH omas:admin {{\n'
                 for proj in changedprojs:
                     perms = self.__change_set[UserFields.IN_PROJECT].old_value[proj] - self.__fields[UserFields.IN_PROJECT][proj]
                     for perm in perms:
-                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.resUri} omas:inProject {proj.resUri}>> omas:hasAdminPermission {perm.value} .\n'
+                        sparql += f'{blank:{(indent + 2) * indent_inc}}<<{self.userIri.toRdf} omas:inProject {proj.toRdf}>> omas:hasAdminPermission {perm.value} .\n'
                         doit = True
                 sparql += f'{blank:{(indent + 1) * indent_inc}}}}\n'
                 sparql += f'{blank:{indent * indent_inc}}}}\n'
                 if doit:
                     sparql_list.append(sparql)
         return ptest, ptest_len, " ;\n".join(sparql_list)
 
 
 if __name__ == "__main__":
     gaga = UserDataclass()
     user_dataclass = UserDataclass(
-        userIri=Xsd_anyURI("https://orcid.org/0000-0002-9991-2055"),
+        userIri=Iri("https://orcid.org/0000-0002-9991-2055"),
         userId=Xsd_NCName("edison"),
         familyName="Edison",
         givenName="Thomas A.",
         credentials="Lightbulb&Phonograph",
-        inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+        inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                    AdminPermission.ADMIN_RESOURCES,
                                                    AdminPermission.ADMIN_CREATE}},
         hasPermissions={Xsd_QName('omas:GenericView')})
     print(user_dataclass.userId)
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Self, Dict
 
 
 class Xsd(ABC):
+    """
+    Abstract base class for XSD classes.
+    """
 
     @abstractmethod
     def __init__(self, value: Self | str):
         pass
 
     @abstractmethod
     def __str__(self) -> str:
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_anyuri.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_anyuri.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,17 +108,17 @@
     def _as_dict(self) -> dict[str, str]:
         return {'value': self._value}
 
     @property
     def toRdf(self) -> str:
         return f'"{self._value}"^^xsd:anyURI'
 
-    @property
-    def resUri(self) -> str:
-        return f'<{self._value}>'
+    # @property
+    # def resUri(self) -> str:
+    #     return f'<{self._value}>'
 
     @property
     def append_allowed(self) -> bool:
         """
         Property which is "True" if the AnyURI is ending with "#" or "/"
         :return: True of False
         """
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_base64binary.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_base64binary.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_boolean.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_boolean.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_date.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_date.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_datetime.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_datetime.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_datetimestamp.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_datetimestamp.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_decimal.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_decimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             raise OmasErrorValue(f'Cannot compare Xsd_decimal("{self._value}") to {type(other)}')
 
     def __float__(self) -> float:
         return self.__value
 
     @property
     def toRdf(self) -> str:
-        return str(self.__value)
+        return f'"{self.__value}"^^xsd:decimal'
 
     def _as_dict(self) -> dict[str, float]:
         return {'value': self.__value}
 
     @property
     def value(self) -> float:
         return self.__value
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_double.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_double.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_duration.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_duration.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_float.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_float.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_gday.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_gday.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_gmonth.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_gmonth.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_gmonthday.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_gmonthday.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_gyear.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_gyear.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_gyearmonth.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_gyearmonth.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_hexbinary.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_hexbinary.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_int.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_int.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 from omaslib.src.xsd.xsd_integer import Xsd_integer
 
 
 @strict
 @serializer
 class Xsd_int(Xsd_integer):
 
-    def __init__(self, value: Self | int | str):
+    def __init__(self, value: Xsd | int | str):
         super().__init__(value)
         if self._value < -2147483648 or self._value > 2147483647:
             raise OmasErrorValue(f"Value must be between -2147483648 and 2147483647")
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_integer.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_integer.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @strict
 @serializer
 class Xsd_integer(Xsd):
     _value: int
 
-    def __init__(self, value: Self | int | str):
+    def __init__(self, value: Xsd | int | str):
         if isinstance(value, Xsd_integer):
             self._value = value._value
         elif isinstance(value, int):
             self._value = value
         else:
             try:
                 self._value = int(value)
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_language.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_language.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_long.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_long.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 from omaslib.src.xsd.xsd_integer import Xsd_integer
 
 
 @strict
 @serializer
 class Xsd_long(Xsd_integer):
 
-    def __init__(self, value: Self | int | str):
+    def __init__(self, value: Xsd | int | str):
         super().__init__(value)
         if self._value < -9223372036854775808 or self._value > 9223372036854775807:
             raise OmasErrorValue('Value must be in the range of [-9223372036854775808 - 9223372036854775807].')
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_name.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 from typing import Self
 
 from pystrict import strict
 
-from omaslib.src.enums.xsd_datatypes import XsdValidator, XsdDatatypes
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.omaserror import OmasErrorValue
 from omaslib.src.helpers.serializer import serializer
 from omaslib.src.xsd.xsd import Xsd
 
 
 @strict
 @serializer
@@ -21,15 +20,15 @@
         else:
             if not re.match("^[a-zA-Z_][\\w.\\-:_]*$", value):
                 raise OmasErrorValue(f'Invalid string "{value}" for xsd:name.')
             self.__value = value
 
     @classmethod
     def fromRdf(cls, value: str) -> Self:
-        value = OldapStringLiteral.unescaping(value)
+        value = StringLiteral.unescaping(value)
         return cls(value)
 
     def __str__(self):
         return self.__value
 
     def __repr__(self):
         return f'Xsd_name("{self.__value}")'
@@ -46,12 +45,12 @@
         return hash(self.__value)
 
     def _as_dict(self) -> dict[str, str]:
         return {'value': self.__value}
 
     @property
     def toRdf(self) -> str:
-        return f'"{OldapStringLiteral.escaping(self.__value)}"^^xsd:name'
+        return f'"{StringLiteral.escaping(self.__value)}"^^xsd:name'
 
     @property
     def value(self) -> str:
         return self.__value
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_ncname.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_ncname.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_nmtoken.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_nmtoken.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_normalizedstring.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_normalizedstring.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import Self
 
 from pystrict import strict
 
 from omaslib.src.enums.xsd_datatypes import XsdValidator, XsdDatatypes
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.omaserror import OmasErrorValue
 from omaslib.src.helpers.serializer import serializer
 from omaslib.src.xsd.xsd import Xsd
 
 
 @strict
 @serializer
@@ -23,15 +23,15 @@
                 raise OmasErrorValue(f'Invalid string "{value}" for xsd:normalizedString.')
             if re.match("^[^\r\n\t]*$", value) is None:
                 raise OmasErrorValue(f'Invalid string "{value}" for xsd:normalizedString.')
             self.__value = value
 
     @classmethod
     def fromRdf(cls, value: str) -> Self:
-        value = OldapStringLiteral.unescaping(value)
+        value = StringLiteral.unescaping(value)
         return cls(value)
 
     def __str__(self):
         return self.__value
 
     def __repr__(self):
         return f'{type(self).__name__}("{self.__value}")'
@@ -44,15 +44,15 @@
         return self.__value == other.__value
 
     def __hash__(self) -> int:
         return super().__hash__()
 
     @property
     def toRdf(self) -> str:
-        return f'"{OldapStringLiteral.escaping(str(self))}"^^xsd:normalizedString'
+        return f'"{StringLiteral.escaping(str(self))}"^^xsd:normalizedString'
 
     def _as_dict(self) -> dict[str, str]:
         return {'value': self.__value}
 
     @property
     def value(self) -> str:
         return self.__value
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_qname.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_qname.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
     def __str__(self):
         """
         Return the string representation of the QName
         :return: String representation of the QName
         """
         return self._value
 
-    @property
-    def resUri(self) -> str:
-        return self._value
+    # @property
+    # def resUri(self) -> str:
+    #     return self._value
 
     def __eq__(self, other: Any | None) -> bool:
         """
         Test for equality of two QNames
         :param other: Another QName/str to compare with
         :return: True of False
         """
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_short.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_unsignedlong.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from typing import Self
-
 from pystrict import strict
 
 from omaslib.src.helpers.omaserror import OmasErrorValue
 from omaslib.src.helpers.serializer import serializer
 from omaslib.src.xsd.xsd import Xsd
 from omaslib.src.xsd.xsd_integer import Xsd_integer
 
 
 @strict
 @serializer
-class Xsd_short(Xsd_integer):
+class Xsd_unsignedLong(Xsd_integer):
 
-    def __init__(self, value: Self | int | str):
+    def __init__(self, value: Xsd | int | str):
         super().__init__(value)
-        if self._value < -32768 or self._value > 32767:
-            raise OmasErrorValue('Value must be in the range of [-32768 - 32767].')
+        if self._value < 0 or self._value > 18446744073709551615:
+            raise OmasErrorValue('Value must be in the range of [0 - 18446744073709551615].')
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_string.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Self, Dict
 
 from pystrict import strict
 
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.serializer import serializer
 from omaslib.src.xsd.xsd import Xsd
 
 
 @strict
 @serializer
 class Xsd_string(Xsd):
@@ -17,14 +17,17 @@
             self.__value = value
         else:
             self.__value = str(value)
 
     def __str__(self) -> str:
         return self.__value
 
+    def __getitem__(self, key: int | slice) -> str:
+        return self.__value[key]
+
     def __eq__(self, other: Self | str | None) -> bool:
         if other is None:
             return False
         if isinstance(other, self.__class__):
             return self.__value == other.__value
         else:
             return self.__value == str(other)
@@ -42,20 +45,23 @@
         return f'Xsd_string("{self.__value}")'
 
     def __hash__(self) -> int:
         return hash(self.__value)
 
     @classmethod
     def fromRdf(cls, value: str) -> Self:
-        return cls(OldapStringLiteral.unescaping(value))
+        return cls(StringLiteral.unescaping(value))
 
     @property
     def toRdf(self) -> str:
-        return f'"{OldapStringLiteral.escaping(str.__str__(self.__value))}"^^xsd:string'
+        return f'"{StringLiteral.escaping(str.__str__(self.__value))}"^^xsd:string'
 
     def _as_dict(self) -> Dict[str, str]:
         return {'value': self.__value}
 
     @property
     def value(self) -> str:
         return self.__value
 
+if __name__ == '__main__':
+    s = Xsd_string("abcdefghijklmnop")
+    print(s[-2:].upper())
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_time.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_time.py`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_token.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import Self
 
 from pystrict import strict
 
 from omaslib.src.enums.xsd_datatypes import XsdValidator, XsdDatatypes
-from omaslib.src.helpers.oldap_string_literal import OldapStringLiteral
+from omaslib.src.dtypes.string_literal import StringLiteral
 from omaslib.src.helpers.omaserror import OmasErrorValue
 from omaslib.src.helpers.serializer import serializer
 from omaslib.src.xsd.xsd import Xsd
 
 
 @strict
 @serializer
@@ -27,15 +27,15 @@
                 raise OmasErrorValue(f'Invalid string "{value}" for xsd:token.')
             self.__value = value
 
     def __str__(self):
         return self.__value
 
     def __repr__(self):
-        return f'Xsd_token("{OldapStringLiteral.escaping(str(self))}")'
+        return f'Xsd_token("{StringLiteral.escaping(str(self))}")'
 
     def __eq__(self, other: Self | str | None) -> bool:
         if other is None:
             return False
         if isinstance(other, Xsd_token):
             return self.__value == other.__value
         else:
@@ -43,21 +43,21 @@
 
 
     def __hash__(self) -> int:
         return super().__hash__()
 
     @classmethod
     def fromRdf(cls, value: str) -> Self:
-        value = OldapStringLiteral.unescaping(value)
-        return cls(OldapStringLiteral.unescaping(value))
+        value = StringLiteral.unescaping(value)
+        return cls(StringLiteral.unescaping(value))
 
 
     def _as_dict(self) -> dict[str, str]:
         return {'value': self.__value}
 
     @property
     def toRdf(self) -> str:
-        return f'"{OldapStringLiteral.escaping(str(self))}"^^xsd:token'
+        return f'"{StringLiteral.escaping(str(self))}"^^xsd:token'
 
     @property
     def value(self) -> str:
         return self.__value
```

### Comparing `omaslib-0.1.8/omaslib/src/xsd/xsd_unsignedbyte.py` & `omaslib-0.1.9/omaslib/src/xsd/xsd_unsignedbyte.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 from omaslib.src.xsd.xsd_integer import Xsd_integer
 
 
 @strict
 @serializer
 class Xsd_unsignedByte(Xsd_integer):
 
-    def __init__(self, value: Self | int | str):
+    def __init__(self, value: Xsd | int | str):
         super().__init__(value)
         if self._value < 0 or self._value > 255:
             raise OmasErrorValue('Value must be in the range of [0 - 255].')
```

### Comparing `omaslib-0.1.8/omaslib/test/test_connection.py` & `omaslib-0.1.9/omaslib/test/test_connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from time import sleep
 
 from omaslib.src.connection import Connection
 from omaslib.src.enums.sparql_result_format import SparqlResultFormat
 from omaslib.src.helpers.context import Context
 from omaslib.src.dtypes.bnode import BNode
 from omaslib.src.dtypes.namespaceiri import NamespaceIRI
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_boolean import Xsd_boolean
 from omaslib.src.helpers.omaserror import OmasError, OmasErrorNotFound
 from omaslib.src.helpers.query_processor import QueryProcessor
@@ -154,25 +155,25 @@
         }
         self.maxDiff = None
         self.assertDictEqual(res, expected)
 
     #@unittest.skip('Work in progress')
     def test_json_query(self):
         expected = {
-            Xsd_QName('rdf:type'): {Xsd_QName('test:testMyRes'), Xsd_QName('sh:NodeShape')},
-            Xsd_QName("rdfs:comment"): "Resource for testing...",
-            Xsd_QName("rdfs:label"): {"My Resource@en", "Meine Ressource@de", "Ma Resource@fr"},
-            Xsd_QName("sh:property"): Xsd_QName("test:testShape"),
-            Xsd_QName("sh:closed"): Xsd_boolean(True),
-            Xsd_QName("sh:targetClass"): Xsd_QName("test:testMyRes"),
-            Xsd_QName("dcterms:hasVersion"): '1.0.0',
-            Xsd_QName("dcterms:creator"): Xsd_anyURI("https://orcid.org/0000-0003-1681-4036"),
-            Xsd_QName("dcterms:created"): Xsd_dateTime(datetime(2023, 11, 4, 12, 0, tzinfo=timezone.utc)),
-            Xsd_QName("dcterms:contributor"):  Xsd_anyURI("https://orcid.org/0000-0003-1681-4036"),
-            Xsd_QName("dcterms:modified"): Xsd_dateTime(datetime(2023, 11, 4, 12, 0, tzinfo=timezone.utc))
+            Iri('rdf:type'): {Iri('test:testMyRes'), Iri('sh:NodeShape')},
+            Iri("rdfs:comment"): "Resource for testing...",
+            Iri("rdfs:label"): {"My Resource@en", "Meine Ressource@de", "Ma Resource@fr"},
+            Iri("sh:property"): Xsd_QName("test:testShape"),
+            Iri("sh:closed"): Xsd_boolean(True),
+            Iri("sh:targetClass"): Xsd_QName("test:testMyRes"),
+            Iri("dcterms:hasVersion"): '1.0.0',
+            Iri("dcterms:creator"): Iri("https://orcid.org/0000-0003-1681-4036"),
+            Iri("dcterms:created"): Xsd_dateTime(datetime(2023, 11, 4, 12, 0, tzinfo=timezone.utc)),
+            Iri("dcterms:contributor"):  Iri("https://orcid.org/0000-0003-1681-4036"),
+            Iri("dcterms:modified"): Xsd_dateTime(datetime(2023, 11, 4, 12, 0, tzinfo=timezone.utc))
         }
         query = self._context.sparql_context
         query += """
         SELECT ?prop ?value ?oo
         FROM test:shacl
         WHERE {
             test:testMyResShape ?prop ?value .
@@ -185,15 +186,15 @@
         result = QueryProcessor(self._context, res)
         for r in result:
             if isinstance(r['prop'], BNode) or isinstance(r['value'], BNode):
                 continue
             if r['prop'] == 'rdfs:label':
                 self.assertTrue(str(r['value']) in expected[r['prop']])
             elif r['prop'] == 'rdf:type':
-                self.assertTrue(str(r['value']) in expected[r['prop']])
+                self.assertTrue(r['value'] in expected[r['prop']])
             else:
                 self.assertEqual(r['value'], expected[r['prop']])
 
     def test_update_query(self):
         query1 = self._context.sparql_context
         query1 += """
         INSERT DATA {
```

### Comparing `omaslib-0.1.8/omaslib/test/test_context.py` & `omaslib-0.1.9/omaslib/test/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,25 @@
         self.assertEqual(qn, 'rdfs:label')
         qn = context.iri2qname(Xsd_anyURI('http://www.w3.org/2004/02/skos/core#node'))
         self.assertEqual(qn, 'skos:node')
         qn = context.iri2qname(Xsd_anyURI('http://www.gaga.org#label'))
         self.assertIsNone(qn)
         with self.assertRaises(OmasError) as ex:
             qn = context.iri2qname('waseliwas/soll')
-        self.assertEqual(str(ex.exception), 'Invalid string "waseliwas/soll" for anyIRI')
+        self.assertEqual(str(ex.exception), 'Invalid string "waseliwas/soll" for anyURI')
 
     def test_context_qname2iri(self):
         context = Context(name='qname2iri')
         self.assertEqual(context.qname2iri(Xsd_QName('skos:gaga')), 'http://www.w3.org/2004/02/skos/core#gaga')
         with self.assertRaises(OmasError) as ex:
             qn = context.iri2qname('gaga')
-        self.assertEqual(str(ex.exception), 'Invalid string "gaga" for anyIRI')
+        self.assertEqual(str(ex.exception), 'Invalid string "gaga" for anyURI')
         with self.assertRaises(OmasError) as ex:
             qn = context.iri2qname('abc:def')
-        self.assertEqual(str(ex.exception), 'Invalid string "abc:def" for anyIRI')
+        self.assertEqual(str(ex.exception), 'Invalid string "abc:def" for anyURI')
         t = Xsd_QName('xml:integer')
         self.assertEqual(context.qname2iri(t), 'http://www.w3.org/XML/1998/namespace#integer')
 
     def test_context_sparql(self):
         context = Context(name='sparql')
         context['test'] = "http://www.test.org/gaga#"
         expected ="""PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
```

### Comparing `omaslib-0.1.8/omaslib/test/test_datamodel.py` & `omaslib-0.1.9/omaslib/test/test_datamodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from omaslib.src.helpers.context import Context
 from omaslib.src.enums.action import Action
 from omaslib.src.dtypes.namespaceiri import NamespaceIRI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.helpers.langstring import LangString
 from omaslib.src.enums.language import Language
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.enums.resourceclassattr import ResourceClassAttribute
 from omaslib.src.enums.xsd_datatypes import XsdDatatypes
-from omaslib.src.propertyclass import PropertyClassAttributesContainer, PropertyClass
+from omaslib.src.propertyclass import PropClassAttrContainer, PropertyClass
 from omaslib.src.propertyrestrictions import PropertyRestrictions
 from omaslib.src.enums.propertyrestrictiontype import PropertyRestrictionType
 from omaslib.src.resourceclass import ResourceClass
 
 
 class TestDataModel(unittest.TestCase):
     _context: Context
@@ -42,58 +42,58 @@
     def tearDown(self):
         pass
 
     def generate_a_datamodel(self, dm_name: Xsd_NCName) -> DataModel:
         #
         # define an external standalone property
         #
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Comment@en", "Kommentar@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Comment@en", "Kommentar@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
         }
         comment = PropertyClass(con=self._connection,
                                 graph=dm_name,
                                 property_class_iri=Xsd_QName(f'{dm_name}:comment'),
                                 attrs=attrs)
         comment.force_external()
 
         #
         # Define the properties for the "Book"
         #
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Title@en", "Titel@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString(["Title of book@en", "Titel des Buches@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Title@en", "Titel@de"]),
+            PropClassAttr.DESCRIPTION: LangString(["Title of book@en", "Titel des Buches@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 1
+            PropClassAttr.ORDER: 1
         }
         title = PropertyClass(con=self._connection,
                               graph=dm_name,
                               property_class_iri=Xsd_QName(f'{dm_name}:title'),
                               attrs=attrs)
 
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.TO_NODE_IRI: Xsd_QName('omas:Person'),
-            PropertyClassAttribute.NAME: LangString(["Author(s)@en", "Autor(en)@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString(["Writers of the Book@en", "Schreiber des Buchs@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.TO_NODE_IRI: Xsd_QName('omas:Person'),
+            PropClassAttr.NAME: LangString(["Author(s)@en", "Autor(en)@de"]),
+            PropClassAttr.DESCRIPTION: LangString(["Writers of the Book@en", "Schreiber des Buchs@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MIN_COUNT: 1,
                 }),
-            PropertyClassAttribute.ORDER: 2
+            PropClassAttr.ORDER: 2
         }
         authors = PropertyClass(con=self._connection,
                                 graph=dm_name,
                                 property_class_iri=Xsd_QName(f'{dm_name}:authors'),
                                 attrs=attrs)
 
         rattrs = ResourceClassAttributesContainer = {
@@ -103,40 +103,40 @@
         }
         book = ResourceClass(con=self._connection,
                              graph=dm_name,
                              owlclass_iri=Xsd_QName(f'{dm_name}:Book'),
                              attrs=rattrs,
                              properties=[title, authors, comment])
 
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.int,
-            PropertyClassAttribute.NAME: LangString(["Pagenumber@en", "Seitennummer@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.int,
+            PropClassAttr.NAME: LangString(["Pagenumber@en", "Seitennummer@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 1
+            PropClassAttr.ORDER: 1
         }
         pagenum = PropertyClass(con=self._connection,
                                 graph=dm_name,
                                 property_class_iri=Xsd_QName(f'{dm_name}:pagenum'),
                                 attrs=attrs)
 
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.TO_NODE_IRI: Xsd_QName(f'{dm_name}:Book'),
-            PropertyClassAttribute.NAME: LangString(["Pagenumber@en", "Seitennummer@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.TO_NODE_IRI: Xsd_QName(f'{dm_name}:Book'),
+            PropClassAttr.NAME: LangString(["Pagenumber@en", "Seitennummer@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                 }),
-            PropertyClassAttribute.ORDER: 1
+            PropClassAttr.ORDER: 1
         }
         inbook = PropertyClass(con=self._connection,
                                graph=dm_name,
                                property_class_iri=Xsd_QName(f'{dm_name}:inbook'),
                                attrs=attrs)
 
         rattrs = ResourceClassAttributesContainer = {
@@ -164,42 +164,42 @@
         dm = self.generate_a_datamodel(dm_name)
         dm.create()
 
         del dm
 
         dm2 = DataModel.read(con=self._connection, graph=dm_name)
         p1 = dm2[Xsd_QName(f'{dm_name}:comment')]
-        self.assertEqual(p1[PropertyClassAttribute.DATATYPE], XsdDatatypes.string)
-        self.assertEqual(p1[PropertyClassAttribute.NAME], LangString(["Comment@en", "Kommentar@de"]))
-        self.assertTrue(p1[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.UNIQUE_LANG])
+        self.assertEqual(p1[PropClassAttr.DATATYPE], XsdDatatypes.string)
+        self.assertEqual(p1[PropClassAttr.NAME], LangString(["Comment@en", "Kommentar@de"]))
+        self.assertTrue(p1[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.UNIQUE_LANG])
 
         r1 = dm2[Xsd_QName(f'{dm_name}:Book')]
         r1p1 = r1[Xsd_QName(f'{dm_name}:title')]
         self.assertEqual(r1p1.internal, Xsd_QName(f'{dm_name}:Book'))
-        self.assertEqual(r1p1[PropertyClassAttribute.DATATYPE], XsdDatatypes.string)
-        self.assertEqual(r1p1[PropertyClassAttribute.NAME], LangString(["Title@en", "Titel@de"]))
-        self.assertEqual(r1p1[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(r1p1[PropClassAttr.DATATYPE], XsdDatatypes.string)
+        self.assertEqual(r1p1[PropClassAttr.NAME], LangString(["Title@en", "Titel@de"]))
+        self.assertEqual(r1p1[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
         r1p2 = r1[Xsd_QName(f'{dm_name}:authors')]
         self.assertEqual(r1p2.internal, Xsd_QName(f'{dm_name}:Book'))
-        self.assertEqual(r1p2[PropertyClassAttribute.TO_NODE_IRI], Xsd_QName('omas:Person'))
-        self.assertEqual(r1p2[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(r1p2[PropClassAttr.TO_NODE_IRI], Xsd_QName('omas:Person'))
+        self.assertEqual(r1p2[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
         r1p3 = r1[Xsd_QName(f'{dm_name}:comment')]
         self.assertIsNone(r1p3.internal)
-        self.assertEqual(r1p3[PropertyClassAttribute.DATATYPE], XsdDatatypes.string)
+        self.assertEqual(r1p3[PropClassAttr.DATATYPE], XsdDatatypes.string)
 
         r2 = dm2[Xsd_QName(f'{dm_name}:Page')]
         r2p1 = r2[Xsd_QName(f'{dm_name}:pagenum')]
         self.assertEqual(r2p1.internal, Xsd_QName(f'{dm_name}:Page'))
-        self.assertEqual(r2p1[PropertyClassAttribute.DATATYPE], XsdDatatypes.int)
+        self.assertEqual(r2p1[PropClassAttr.DATATYPE], XsdDatatypes.int)
         r2p2 = r2[Xsd_QName(f'{dm_name}:inbook')]
         self.assertEqual(r2p2.internal, Xsd_QName(f'{dm_name}:Page'))
-        self.assertEqual(r2p2[PropertyClassAttribute.TO_NODE_IRI], Xsd_QName(f'{dm_name}:Book'))
+        self.assertEqual(r2p2[PropClassAttr.TO_NODE_IRI], Xsd_QName(f'{dm_name}:Book'))
         r2p3 = r1[Xsd_QName(f'{dm_name}:comment')]
         self.assertIsNone(r2p3.internal)
-        self.assertEqual(r2p3[PropertyClassAttribute.DATATYPE], XsdDatatypes.string)
+        self.assertEqual(r2p3[PropClassAttr.DATATYPE], XsdDatatypes.string)
 
     #@unittest.skip('Work in progress')
     def test_datamodel_read(self):
         model = DataModel.read(self._connection, "omas")
         self.assertTrue(set(model.get_propclasses()) == {
             #QName("omas:comment"),
             Xsd_QName("omas:test"),
@@ -227,37 +227,37 @@
         dm.create()
         dm_name = Xsd_NCName("dmtest")
         dm = DataModel.read(self._connection, dm_name)
 
         #
         # define an external standalone property
         #
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.gYear,
-            PropertyClassAttribute.NAME: LangString(["Publication Year@en", "Publikationsjahr@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.gYear,
+            PropClassAttr.NAME: LangString(["Publication Year@en", "Publikationsjahr@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1
                 }),
         }
         pubyear = PropertyClass(con=self._connection,
                                 graph=dm_name,
                                 property_class_iri=Xsd_QName(f'{dm_name}:pubYear'),
                                 attrs=attrs)
         pubyear.force_external()
         dm[Xsd_QName(f'{dm_name}:pubYear')] = pubyear
         self.assertEqual({Xsd_QName(f'{dm_name}:pubYear'): PropertyClassChange(None, Action.CREATE)}, dm.changeset)
 
-        dm[Xsd_QName(f'{dm_name}:comment')][PropertyClassAttribute.NAME][Language.FR] = 'Commentaire'
+        dm[Xsd_QName(f'{dm_name}:comment')][PropClassAttr.NAME][Language.FR] = 'Commentaire'
         self.assertEqual({
             Xsd_QName(f'{dm_name}:pubYear'): PropertyClassChange(None, Action.CREATE),
             Xsd_QName(f'{dm_name}:comment'): PropertyClassChange(None, Action.MODIFY)
         }, dm.changeset)
 
-        dm[Xsd_QName(f'{dm_name}:Book')][Xsd_QName(f'{dm_name}:authors')][PropertyClassAttribute.NAME][Language.FR] = "Ecrivain(s)"
+        dm[Xsd_QName(f'{dm_name}:Book')][Xsd_QName(f'{dm_name}:authors')][PropClassAttr.NAME][Language.FR] = "Ecrivain(s)"
         self.assertEqual({
             Xsd_QName(f'{dm_name}:pubYear'): PropertyClassChange(None, Action.CREATE),
             Xsd_QName(f'{dm_name}:comment'): PropertyClassChange(None, Action.MODIFY),
             Xsd_QName(f'{dm_name}:Book'): ResourceClassChange(None, Action.MODIFY)
         }, dm.changeset)
 
         del dm[Xsd_QName(f'{dm_name}:Page')][Xsd_QName(f'{dm_name}:comment')]
@@ -265,18 +265,18 @@
         self.assertEqual({
             Xsd_QName(f'{dm_name}:pubYear'): PropertyClassChange(None, Action.CREATE),
             Xsd_QName(f'{dm_name}:comment'): PropertyClassChange(None, Action.MODIFY),
             Xsd_QName(f'{dm_name}:Book'): ResourceClassChange(None, Action.MODIFY),
             Xsd_QName(f'{dm_name}:Page'): ResourceClassChange(None, Action.MODIFY)
         }, dm.changeset)
 
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Page name@en", "Seitenbezeichnung@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Page name@en", "Seitenbezeichnung@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                 }),
         }
         pagename = PropertyClass(con=self._connection,
                                  graph=dm_name,
@@ -300,37 +300,37 @@
 
         dm_name = Xsd_NCName("dmtest")
         dm = DataModel.read(self._connection, dm_name)
 
         #
         # define an external standalone property
         #
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.gYear,
-            PropertyClassAttribute.NAME: LangString(["Publication Year@en", "Publikationsjahr@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.gYear,
+            PropClassAttr.NAME: LangString(["Publication Year@en", "Publikationsjahr@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1
                 }),
         }
         pubyear = PropertyClass(con=self._connection,
                                 graph=dm_name,
                                 property_class_iri=Xsd_QName(f'{dm_name}:pubYear'),
                                 attrs=attrs)
         pubyear.force_external()
 
         dm[Xsd_QName(f'{dm_name}:pubYear')] = pubyear
-        dm[Xsd_QName(f'{dm_name}:comment')][PropertyClassAttribute.NAME][Language.FR] = 'Commentaire'
-        dm[Xsd_QName(f'{dm_name}:Book')][Xsd_QName(f'{dm_name}:authors')][PropertyClassAttribute.NAME][Language.FR] = "Ecrivain(s)"
+        dm[Xsd_QName(f'{dm_name}:comment')][PropClassAttr.NAME][Language.FR] = 'Commentaire'
+        dm[Xsd_QName(f'{dm_name}:Book')][Xsd_QName(f'{dm_name}:authors')][PropClassAttr.NAME][Language.FR] = "Ecrivain(s)"
         del dm[Xsd_QName(f'{dm_name}:Page')][Xsd_QName(f'{dm_name}:comment')]
 
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Page name@en", "Seitenbezeichnung@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Page name@en", "Seitenbezeichnung@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                 }),
         }
         pagename = PropertyClass(con=self._connection,
                                  graph=dm_name,
@@ -341,15 +341,15 @@
 
         dm.update()
 
         del dm
 
         dm = DataModel.read(self._connection, dm_name)
         self.assertIsNotNone(dm.get(Xsd_QName(f'{dm_name}:pubYear')))
-        self.assertEqual(dm[Xsd_QName(f'{dm_name}:pubYear')][PropertyClassAttribute.DATATYPE], XsdDatatypes.gYear)
-        self.assertEqual(dm[Xsd_QName(f'{dm_name}:pubYear')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 1)
-        self.assertEqual(dm[Xsd_QName(f'{dm_name}:comment')][PropertyClassAttribute.NAME][Language.FR], 'Commentaire')
-        self.assertEqual(dm[Xsd_QName(f'{dm_name}:Book')][Xsd_QName(f'{dm_name}:authors')][PropertyClassAttribute.NAME][Language.FR], "Ecrivain(s)")
+        self.assertEqual(dm[Xsd_QName(f'{dm_name}:pubYear')][PropClassAttr.DATATYPE], XsdDatatypes.gYear)
+        self.assertEqual(dm[Xsd_QName(f'{dm_name}:pubYear')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 1)
+        self.assertEqual(dm[Xsd_QName(f'{dm_name}:comment')][PropClassAttr.NAME][Language.FR], 'Commentaire')
+        self.assertEqual(dm[Xsd_QName(f'{dm_name}:Book')][Xsd_QName(f'{dm_name}:authors')][PropClassAttr.NAME][Language.FR], "Ecrivain(s)")
         self.assertIsNotNone(dm[Xsd_QName(f'{dm_name}:Page')][Xsd_QName(f'{dm_name}:pageName')])
         self.assertIsNone(dm[Xsd_QName(f'{dm_name}:Page')].get(Xsd_QName(f'{dm_name}:comment')))
```

### Comparing `omaslib-0.1.8/omaslib/test/test_dtypes.py` & `omaslib-0.1.9/omaslib/test/test_dtypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         """
 
     def test_namespace(self):
         ns1 = NamespaceIRI('http://www.org/test/')
         self.assertEqual(str(ns1), 'http://www.org/test/')
         self.assertEqual(repr(ns1), 'NamespaceIRI("http://www.org/test/")')
         self.assertEqual(ns1.toRdf, '"http://www.org/test/"^^xsd:anyURI')
-        self.assertEqual(ns1.resUri, '<http://www.org/test/>')
         self.assertEqual(ns1 + "gaga", Xsd_anyURI("http://www.org/test/gaga"))
 
         ns2 = NamespaceIRI('http://www.org/test#')
         self.assertEqual(str(ns2), 'http://www.org/test#')
         self.assertEqual(ns2 + "gaga", Xsd_anyURI("http://www.org/test#gaga"))
 
         jsonstr = json.dumps(ns1, default=serializer.encoder_default)
@@ -178,14 +177,19 @@
 
         val.add(Xsd_integer(42))
         self.assertTrue(Xsd_integer(42) in val)
 
         val.discard(Xsd_string("ist"))
         self.assertFalse(Xsd_string("ist") in val)
 
+        val = RdfSet(Xsd_string("was"), Xsd_string("ist"), Xsd_string("das?"))
+        self.assertTrue(Xsd_string("was") in val)
+        self.assertTrue(Xsd_string("ist") in val)
+        self.assertTrue(Xsd_string("das?") in val)
+
     def test_bnode(self):
         val = BNode("_:node42")
         self.assertEqual(str(val), "_:node42")
 
         jsonstr = json.dumps(val, default=serializer.encoder_default)
         val2 = json.loads(jsonstr, object_hook=serializer.decoder_hook)
         self.assertEqual(val, val2)
```

### Comparing `omaslib-0.1.8/omaslib/test/test_in_project.py` & `omaslib-0.1.9/omaslib/test/test_in_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import unittest
 
 from omaslib.src.enums.permissions import AdminPermission
 from omaslib.src.helpers.omaserror import OmasErrorValue, OmasErrorKey
 from omaslib.src.helpers.serializer import serializer
 from omaslib.src.in_project import InProjectClass
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_string import Xsd_string
 
 
 class TestInproject(unittest.TestCase):
     def test_creation(self):
         ip = InProjectClass({'test:proj': {AdminPermission.ADMIN_PERMISSION_SETS, 'omas:ADMIN_RESOURCES'},
@@ -20,24 +21,24 @@
 
         with self.assertRaises(OmasErrorValue) as ex:
             ip = InProjectClass({'test:proj': {'MODEL_T'}})
 
     def test_get_item(self):
         ip = InProjectClass({'test:proj': {AdminPermission.ADMIN_PERMISSION_SETS, 'omas:ADMIN_RESOURCES'},
                              'https://gaga.com/test': {'ADMIN_MODEL'},
-                             Xsd_QName('gaga:gugus'): set()})
+                             Iri('gaga:gugus'): set()})
         self.assertEqual(ip['test:proj'], {AdminPermission.ADMIN_PERMISSION_SETS, AdminPermission.ADMIN_RESOURCES})
         self.assertEqual(ip['https://gaga.com/test'], {AdminPermission.ADMIN_MODEL})
-        self.assertEqual(ip[Xsd_QName('gaga:gugus')], set())
+        self.assertEqual(ip[Iri('gaga:gugus')], set())
 
         with self.assertRaises(OmasErrorValue) as ex:
             tmp = ip['gaga']
         with self.assertRaises(OmasErrorValue) as ex:
             tmp = ip['$<>12']
-        with self.assertRaises(OmasErrorValue) as ex:
+        with self.assertRaises(OmasErrorKey) as ex:
             tmp = ip[Xsd_string('test:proj')]
 
     def test_set_item(self):
         ip = InProjectClass({'test:proj': {AdminPermission.ADMIN_PERMISSION_SETS, 'omas:ADMIN_RESOURCES'},
                              'https://gaga.com/test': {'ADMIN_MODEL'},
                              Xsd_QName('gaga:gugus'): set()})
         ip['test:proj'] = {AdminPermission.ADMIN_OLDAP}
@@ -125,19 +126,19 @@
 
 
     def test_items(self):
         ip = InProjectClass({'test:proj': {AdminPermission.ADMIN_PERMISSION_SETS, 'omas:ADMIN_RESOURCES'},
                              'https://gaga.com/test': {'ADMIN_MODEL'},
                              Xsd_QName('gaga:gugus'): set()})
         for proj, perms in ip.items():
-            self.assertTrue(proj in ['test:proj', 'https://gaga.com/test', Xsd_QName('gaga:gugus')])
+            self.assertTrue(proj in ['test:proj', 'https://gaga.com/test', Iri('gaga:gugus')])
 
     def test_keys(self):
         ip = InProjectClass({'test:proj': {AdminPermission.ADMIN_PERMISSION_SETS, 'omas:ADMIN_RESOURCES'},
                              'https://gaga.com/test': {'ADMIN_MODEL'},
-                             Xsd_QName('gaga:gugus'): set()})
+                             Iri('gaga:gugus'): set()})
         keys = set(ip.keys())
-        self.assertEqual(keys, {'test:proj', 'https://gaga.com/test', Xsd_QName('gaga:gugus')})
+        self.assertEqual(keys, {'test:proj', 'https://gaga.com/test', Iri('gaga:gugus')})
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `omaslib-0.1.8/omaslib/test/test_langstring.py` & `omaslib-0.1.9/omaslib/test/test_langstring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import unittest
 from datetime import datetime
 
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.enums.action import Action
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.helpers.langstring import LangString, LangStringChange
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.omaserror import OmasError
 
 
 class TestLangstring(unittest.TestCase):
 
     def test_langstring_constructor(self):
         ls1 = LangString("english@en")
         self.assertEqual(ls1['en'], 'english')
-        ls2 = LangString('nolanguage')
+        ls2 = LangString(ls)
         self.assertEqual(ls2['xx'], 'nolanguage')
         self.assertEqual(ls2[Language.XX], 'nolanguage')
         ls3 = LangString(ls1)
         self.assertEqual(ls3['en'], 'english')
 
         ls4 = LangString({
             'en': 'english',
@@ -218,15 +218,15 @@
     }
 }
 """
         self.assertEqual(qstr, expected)
 
         sstr = ls1.update_shacl(graph=Xsd_NCName("test"),
                                 prop_iri=Xsd_QName('omas:prop'),
-                                attr=PropertyClassAttribute.NAME,
+                                attr=PropClassAttr.NAME,
                                 modified=Xsd_dateTime("2023-11-04T12:00:00Z"))
         expected = """# LangString: Process "FR" with Action "create"
 WITH test:shacl
 INSERT {
     ?prop sh:name "français"@fr .
 }
 WHERE {
```

### Comparing `omaslib-0.1.8/omaslib/test/test_project.py` & `omaslib-0.1.9/omaslib/test/test_project.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import date
 from time import sleep
 
 from omaslib.src.connection import Connection
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.context import Context
 from omaslib.src.dtypes.namespaceiri import NamespaceIRI
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.xsd.xsd_date import Xsd_date
 from omaslib.src.helpers.langstring import LangString
 from omaslib.src.helpers.omaserror import OmasErrorNotFound
 from omaslib.src.project import Project
 
@@ -42,24 +43,30 @@
     @classmethod
     def tearDownClass(cls):
         cls._connection.clear_graph(Xsd_QName('omas:admin'))
         cls._connection.upload_turtle("omaslib/ontologies/admin.trig")
         sleep(1)  # upload may take a while...
 
     def test_project_read(self):
-        project = Project.read(con=self._connection, projectIri=Xsd_QName("omas:SystemProject"))
+        project = Project.read(con=self._connection, projectIri_SName=Iri("omas:SystemProject"))
         self.assertEqual(Xsd_NCName("system"), project.projectShortName)
         self.assertEqual(LangString(["System@en",
                                      "System@de",
                                      "Système@fr",
                                      "Systema@it"]), project.label)
         self.assertEqual(NamespaceIRI("http://omas.org/base#"), project.namespaceIri)
         self.assertEqual(LangString(["Project for system administration@en"]), project.comment)
         self.assertEqual(Xsd_date("2024-01-01"), project.projectStart)
 
+        project = Project.read(con=self._connection, projectIri_SName='http://www.salsah.org/version/2.0/SwissBritNet')
+        self.assertEqual(Xsd_NCName("britnet"), project.projectShortName)
+
+        project2 = Project.read(con=self._connection, projectIri_SName='hyha')
+        self.assertEqual(Xsd_NCName("hyha"), project2.projectShortName)
+
     # @unittest.skip('Work in progress')
     def test_project_search(self):
         projects = Project.search(con=self._connection, label="HyperHamlet")
         self.assertEqual(["omas:HyperHamlet"], projects)
 
     # @unittest.skip('Work in progress')
     def test_project_search_fail(self):
@@ -75,21 +82,48 @@
                           projectStart=Xsd_date(2024, 1, 1),
                           projectEnd=Xsd_date(2025, 12, 31)
                           )
         project.create()
         projectIri = project.projectIri
         del project
 
-        project2 = Project.read(con=self._connection, projectIri=projectIri)
+        project2 = Project.read(con=self._connection, projectIri_SName=projectIri)
         self.assertEqual("unittest", project2.projectShortName)
         self.assertEqual(LangString(["unittest@en", "unittest@de"]), project2.label)
         self.assertEqual(LangString(["For testing@en", "Für Tests@de"]), project2.comment)
         self.assertEqual(Xsd_date(2024, 1, 1), project2.projectStart)
         self.assertEqual(Xsd_date(2025, 12, 31), project2.projectEnd)
 
+        project3 = Project(con=self._connection,
+                           projectShortName="unittest3",
+                           label=LangString(["unittest3@en", "unittest3@de"]),
+                           namespaceIri=NamespaceIRI("http://unitest.org/project/unittest3#"),
+                           comment=LangString(["For testing3@en", "Für Tests3@de"]),
+                           projectStart=Xsd_date(2024, 3, 3),
+                           projectEnd=None)
+        project3.create()
+        projectIri3 = project3.projectIri
+        project3 = Project.read(con=self._connection, projectIri_SName=projectIri3)
+        self.assertEqual("unittest3", project3.projectShortName)
+        self.assertEqual(LangString(["unittest3@en", "unittest3@de"]), project3.label)
+        self.assertEqual(LangString(["For testing3@en", "Für Tests3@de"]), project3.comment)
+        self.assertEqual(Xsd_date(2024, 3, 3), project3.projectStart)
+
+        project4 = Project(con=self._connection,
+                           projectShortName="unittest4",
+                           namespaceIri=NamespaceIRI("http://unitest.org/project/unittest4#"))
+        project4.create()
+        projectIri4 = project4.projectIri
+        project4 = Project.read(con=self._connection, projectIri_SName=projectIri4)
+        self.assertEqual("unittest4", project4.projectShortName)
+        self.assertIsNone(project4.label)
+        self.assertIsNone(project4.comment)
+        self.assertIsNotNone(project4.projectStart)
+
+
     # @unittest.skip('Work in progress')
     def test_project_modify(self):
         project = Project(con=self._connection,
                           projectShortName="updatetest",
                           label=LangString(["updatetest@en", "updatetest@de"]),
                           namespaceIri=NamespaceIRI("http://unitest.org/project/updatetest#"),
                           comment=LangString(["For testing@en", "Für Tests@de"]),
@@ -97,15 +131,15 @@
                           projectEnd=Xsd_date(2025, 12, 31)
                           )
         project.create()
 
         projectIri = project.projectIri
         del project
 
-        project = Project.read(con=self._connection, projectIri=projectIri)
+        project = Project.read(con=self._connection, projectIri_SName=projectIri)
         project.comment[Language.FR] = "Pour les tests"
         project.comment[Language.DE] = "FÜR DAS TESTEN"
         project.label = LangString(["UPDATETEST@en", "UP-DATE-TEST@fr"])
         project.projectEnd = Xsd_date(date(2026, 6, 30))
         project.update()
         self.assertEqual(project.comment, LangString(["For testing@en", "FÜR DAS TESTEN@de", "Pour les tests@fr"]))
         self.assertEqual(project.label, LangString(["UPDATETEST@en", "UP-DATE-TEST@fr"]))
@@ -115,22 +149,22 @@
     def test_project_delete(self):
         project = Project(con=self._connection,
                           projectShortName="deletetest",
                           label=LangString(["deletetest@en", "deletetest@de"]),
                           namespaceIri=NamespaceIRI("http://unitest.org/project/deletetest#"),
                           comment=LangString(["For deleting@en", "Für Löschung@de"]),
                           projectStart=Xsd_date(2024, 1, 1),
-                          projectEnd=Xsd_date(2025, 12, 31)
+                          #projectEnd=Xsd_date(2025, 12, 31)
                           )
         project.create()
         projectIri = project.projectIri
         del project
 
-        project = Project.read(con=self._connection, projectIri=projectIri)
+        project = Project.read(con=self._connection, projectIri_SName=projectIri)
         project.delete()
         del project
 
         with self.assertRaises(OmasErrorNotFound) as ex:
-            project = Project.read(con=self._connection, projectIri=projectIri)
+            project = Project.read(con=self._connection, projectIri_SName=projectIri)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `omaslib-0.1.8/omaslib/test/test_resourceclass.py` & `omaslib-0.1.9/omaslib/test/test_resourceclass_old.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from omaslib.src.dtypes.namespaceiri import NamespaceIRI
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.helpers.langstring import LangString
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.omaserror import OmasErrorAlreadyExists
-from omaslib.src.enums.propertyclassattr import PropertyClassAttribute
+from omaslib.src.enums.propertyclassattr import PropClassAttr
 from omaslib.src.helpers.query_processor import QueryProcessor
 from omaslib.src.helpers.semantic_version import SemanticVersion
 from omaslib.src.enums.xsd_datatypes import XsdDatatypes
-from omaslib.src.propertyclass import PropertyClassAttributesContainer, PropertyClass, OwlPropertyType
+from omaslib.src.propertyclass import PropClassAttrContainer, PropertyClass, OwlPropertyType
 from omaslib.src.propertyrestrictions import PropertyRestrictions
 from omaslib.src.enums.propertyrestrictiontype import PropertyRestrictionType
 from omaslib.src.resourceclass import ResourceClassAttributesContainer, ResourceClass
 from omaslib.src.enums.resourceclassattr import ResourceClassAttribute
 
 
 class Graph(Enum):
@@ -101,41 +101,41 @@
     def tearDownClass(cls):
         #cls._connection.clear_graph(QName('test:shacl'))
         #cls._connection.clear_graph(QName('test:onto'))
         pass
 
     #@unittest.skip('Work in progress')
     def test_constructor(self):
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.SUBPROPERTY_OF: Xsd_QName('test:comment'),
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Test property@en", "Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("A property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.SUBPROPERTY_OF: Xsd_QName('test:comment'),
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Test property@en", "Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("A property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 5
+            PropClassAttr.ORDER: 5
         }
         p1 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:testprop'), attrs=attrs)
 
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Test enum@en", "Enumerationen@de"]),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Test enum@en", "Enumerationen@de"]),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.IN: {"yes", "maybe", "no"}
                 }),
-            PropertyClassAttribute.ORDER: 6
+            PropClassAttr.ORDER: 6
         }
         p2 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:enumprop'), attrs=attrs)
 
         properties: List[Union[PropertyClass, Xsd_QName]] = [
             Xsd_QName("test:comment"),
@@ -156,42 +156,42 @@
         self.assertEqual(r1[ResourceClassAttribute.LABEL], LangString(["Test resource@en", "Resource de test@fr"]))
         self.assertEqual(r1[ResourceClassAttribute.COMMENT], LangString("For testing purposes@en"))
         self.assertTrue(r1[ResourceClassAttribute.CLOSED])
 
         prop1 = r1[Xsd_QName("test:comment")]
         self.assertIsNone(prop1.internal)
         self.assertEqual(prop1.property_class_iri, Xsd_QName("test:comment"))
-        self.assertEqual(prop1[PropertyClassAttribute.DATATYPE], XsdDatatypes.string)
-        self.assertEqual(prop1[PropertyClassAttribute.NAME], LangString(["comment@en", "Kommentar@de"]))
-        self.assertEqual(prop1[PropertyClassAttribute.DESCRIPTION], LangString("This is a test property@de"))
-        self.assertEqual(prop1[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 1)
-        self.assertEqual(prop1[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.UNIQUE_LANG], True)
+        self.assertEqual(prop1[PropClassAttr.DATATYPE], XsdDatatypes.string)
+        self.assertEqual(prop1[PropClassAttr.NAME], LangString(["comment@en", "Kommentar@de"]))
+        self.assertEqual(prop1[PropClassAttr.DESCRIPTION], LangString("This is a test property@de"))
+        self.assertEqual(prop1[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 1)
+        self.assertEqual(prop1[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.UNIQUE_LANG], True)
 
         prop2 = r1[Xsd_QName("test:test")]
         self.assertIsNone(prop2.internal)
         self.assertEqual(prop2.property_class_iri, Xsd_QName("test:test"))
-        self.assertEqual(prop2.get(PropertyClassAttribute.TO_NODE_IRI), Xsd_QName('test:comment'))
-        self.assertEqual(prop2.get(PropertyClassAttribute.DESCRIPTION), LangString("Property shape for testing purposes"))
-        self.assertEqual(prop2[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.MIN_COUNT), 1)
-        self.assertEqual(prop2.get(PropertyClassAttribute.ORDER), 3)
+        self.assertEqual(prop2.get(PropClassAttr.TO_NODE_IRI), Xsd_QName('test:comment'))
+        self.assertEqual(prop2.get(PropClassAttr.DESCRIPTION), LangString("Property shape for testing purposes"))
+        self.assertEqual(prop2[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.MIN_COUNT), 1)
+        self.assertEqual(prop2.get(PropClassAttr.ORDER), 3)
 
         prop3 = r1[Xsd_QName("test:testprop")]
         self.assertEqual(prop3.internal, Xsd_QName('test:TestResource'))
         self.assertEqual(prop3.property_class_iri, Xsd_QName("test:testprop"))
-        self.assertEqual(prop3.get(PropertyClassAttribute.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
-        self.assertEqual(prop3.get(PropertyClassAttribute.DATATYPE), XsdDatatypes.string)
-        self.assertEqual(prop3.get(PropertyClassAttribute.NAME), LangString(["Test property@en", "Testprädikat@de"]))
-        self.assertEqual(prop3.get(PropertyClassAttribute.ORDER), 5)
-        self.assertEqual(prop3.get(PropertyClassAttribute.SUBPROPERTY_OF), Xsd_QName("test:comment"))
-        self.assertEqual(prop3[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.MAX_COUNT), 1)
-        self.assertEqual(prop3[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.UNIQUE_LANG], True)
-        self.assertEqual(prop3[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE, Language.FR, Language.IT})
+        self.assertEqual(prop3.get(PropClassAttr.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
+        self.assertEqual(prop3.get(PropClassAttr.DATATYPE), XsdDatatypes.string)
+        self.assertEqual(prop3.get(PropClassAttr.NAME), LangString(["Test property@en", "Testprädikat@de"]))
+        self.assertEqual(prop3.get(PropClassAttr.ORDER), 5)
+        self.assertEqual(prop3.get(PropClassAttr.SUBPROPERTY_OF), Xsd_QName("test:comment"))
+        self.assertEqual(prop3[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.MAX_COUNT), 1)
+        self.assertEqual(prop3[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.UNIQUE_LANG], True)
+        self.assertEqual(prop3[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE, Language.FR, Language.IT})
 
         prop4 = r1[Xsd_QName("test:enumprop")]
-        self.assertEqual(prop4[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.IN],
+        self.assertEqual(prop4[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.IN],
                          {"yes", "maybe", "no"})
 
     #@unittest.skip('Work in progress')
     def test_reading(self):
         r1 = ResourceClass.read(con=self._connection,
                                 graph=Xsd_NCName('test'),
                                 owl_class_iri=Xsd_QName('test:testMyRes'))
@@ -209,89 +209,89 @@
         self.assertIsNone(prop1.internal)
         self.assertEqual(prop1.property_class_iri, Xsd_QName("test:test"))
         self.assertEqual(prop1.version, SemanticVersion(1, 0, 0))
         self.assertEqual(prop1.creator, Xsd_anyURI('https://orcid.org/0000-0003-1681-4036'))
         self.assertEqual(prop1.created, datetime.fromisoformat('2023-11-04T12:00:00Z'))
         self.assertEqual(prop1.contributor, Xsd_anyURI('https://orcid.org/0000-0003-1681-4036'))
         self.assertEqual(prop1.modified, datetime.fromisoformat('2023-11-04T12:00:00Z'))
-        self.assertEqual(prop1.get(PropertyClassAttribute.PROPERTY_TYPE), OwlPropertyType.OwlObjectProperty)
-        self.assertEqual(prop1.get(PropertyClassAttribute.TO_NODE_IRI), Xsd_QName('test:comment'))
-        self.assertEqual(prop1.get(PropertyClassAttribute.DESCRIPTION), LangString("Property shape for testing purposes"))
-        self.assertEqual(prop1[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.MIN_COUNT), 1)
-        self.assertEqual(prop1.get(PropertyClassAttribute.ORDER), 3)
+        self.assertEqual(prop1.get(PropClassAttr.PROPERTY_TYPE), OwlPropertyType.OwlObjectProperty)
+        self.assertEqual(prop1.get(PropClassAttr.TO_NODE_IRI), Xsd_QName('test:comment'))
+        self.assertEqual(prop1.get(PropClassAttr.DESCRIPTION), LangString("Property shape for testing purposes"))
+        self.assertEqual(prop1[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.MIN_COUNT), 1)
+        self.assertEqual(prop1.get(PropClassAttr.ORDER), 3)
 
         prop2 = r1[Xsd_QName('test:hasText')]
         self.assertEqual(prop2.internal, Xsd_QName('test:testMyRes'))
         self.assertEqual(prop2.property_class_iri, Xsd_QName("test:hasText"))
         self.assertEqual(prop2.version, SemanticVersion(1, 0, 0))
         self.assertEqual(prop2.creator, Xsd_anyURI('https://orcid.org/0000-0003-1681-4036'))
         self.assertEqual(prop2.created, datetime.fromisoformat('2023-11-04T12:00:00Z'))
         self.assertEqual(prop2.contributor, Xsd_anyURI('https://orcid.org/0000-0003-1681-4036'))
         self.assertEqual(prop2.modified, datetime.fromisoformat('2023-11-04T12:00:00Z'))
-        self.assertEqual(prop2.get(PropertyClassAttribute.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
-        self.assertEqual(prop2.get(PropertyClassAttribute.DATATYPE), XsdDatatypes.string)
-        self.assertEqual(prop2.get(PropertyClassAttribute.NAME), LangString(["A text", "Ein Text@de"]))
-        self.assertEqual(prop2.get(PropertyClassAttribute.DESCRIPTION), LangString("A longer text..."))
-        self.assertEqual(prop2.get(PropertyClassAttribute.ORDER), 1)
-        self.assertEqual(prop2[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.MIN_COUNT), 1)
-        self.assertEqual(prop2[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.MAX_COUNT), 1)
+        self.assertEqual(prop2.get(PropClassAttr.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
+        self.assertEqual(prop2.get(PropClassAttr.DATATYPE), XsdDatatypes.string)
+        self.assertEqual(prop2.get(PropClassAttr.NAME), LangString(["A text", "Ein Text@de"]))
+        self.assertEqual(prop2.get(PropClassAttr.DESCRIPTION), LangString("A longer text..."))
+        self.assertEqual(prop2.get(PropClassAttr.ORDER), 1)
+        self.assertEqual(prop2[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.MIN_COUNT), 1)
+        self.assertEqual(prop2[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.MAX_COUNT), 1)
 
         prop3 = r1[Xsd_QName('test:hasEnum')]
-        self.assertEqual(prop3.get(PropertyClassAttribute.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
-        self.assertEqual(prop3.get(PropertyClassAttribute.DATATYPE), XsdDatatypes.string)
-        self.assertEqual(prop3[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.IN),
+        self.assertEqual(prop3.get(PropClassAttr.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
+        self.assertEqual(prop3.get(PropClassAttr.DATATYPE), XsdDatatypes.string)
+        self.assertEqual(prop3[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.IN),
                          {'red', 'green', 'blue', 'yellow'})
 
     #@unittest.skip('Work in progress')
     def test_creating(self):
-        props1: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.SUBPROPERTY_OF: Xsd_QName('test:comment'),
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Test property@en", "Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("A property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        props1: PropClassAttrContainer = {
+            PropClassAttr.SUBPROPERTY_OF: Xsd_QName('test:comment'),
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Test property@en", "Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("A property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 1
+            PropClassAttr.ORDER: 1
         }
         p1 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:testone'),
                            attrs=props1)
 
-        props2: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.TO_NODE_IRI: Xsd_QName('test:testMyRes'),
-            PropertyClassAttribute.NAME: LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("An exclusive property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        props2: PropClassAttrContainer = {
+            PropClassAttr.TO_NODE_IRI: Xsd_QName('test:testMyRes'),
+            PropClassAttr.NAME: LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("An exclusive property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 2
+            PropClassAttr.ORDER: 2
         }
         p2 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:testtwo'),
                            attrs=props2)
 
-        props3: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.int,
-            PropertyClassAttribute.NAME: LangString(["E.N.U.M@en"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("An exclusive enum testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        props3: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.int,
+            PropClassAttr.NAME: LangString(["E.N.U.M@en"]),
+            PropClassAttr.DESCRIPTION: LangString("An exclusive enum testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.IN: {1, 2, 3}
                 }),
-            PropertyClassAttribute.ORDER: 3
+            PropClassAttr.ORDER: 3
         }
         p3 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:testthree'),
                            attrs=props3)
 
         properties: List[Union[PropertyClass, Xsd_QName]] = [
@@ -319,60 +319,60 @@
         self.assertEqual(r2[ResourceClassAttribute.LABEL], LangString(["CreateResTest@en", "CréationResTeste@fr"]))
         self.assertEqual(r2[ResourceClassAttribute.COMMENT], LangString("For testing purposes@en"))
         self.assertTrue(r2[ResourceClassAttribute.COMMENT])
 
         prop1 = r2[Xsd_QName("test:comment")]
         self.assertIsNone(prop1.internal)
         self.assertEqual(prop1.property_class_iri, Xsd_QName('test:comment'))
-        self.assertEqual(prop1.get(PropertyClassAttribute.DATATYPE), XsdDatatypes.string)
-        self.assertTrue(prop1.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.UNIQUE_LANG])
-        self.assertEqual(prop1.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.MAX_COUNT], 1)
-        self.assertEqual(prop1.get(PropertyClassAttribute.NAME), LangString(["comment@en", "Kommentar@de"]))
-        self.assertEqual(prop1.get(PropertyClassAttribute.DESCRIPTION), LangString("This is a test property@de"))
-        self.assertIsNone(prop1.get(PropertyClassAttribute.SUBPROPERTY_OF))
-        self.assertEqual(prop1[PropertyClassAttribute.ORDER], 2)
-        self.assertEqual(prop1.get(PropertyClassAttribute.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
+        self.assertEqual(prop1.get(PropClassAttr.DATATYPE), XsdDatatypes.string)
+        self.assertTrue(prop1.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.UNIQUE_LANG])
+        self.assertEqual(prop1.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.MAX_COUNT], 1)
+        self.assertEqual(prop1.get(PropClassAttr.NAME), LangString(["comment@en", "Kommentar@de"]))
+        self.assertEqual(prop1.get(PropClassAttr.DESCRIPTION), LangString("This is a test property@de"))
+        self.assertIsNone(prop1.get(PropClassAttr.SUBPROPERTY_OF))
+        self.assertEqual(prop1[PropClassAttr.ORDER], 2)
+        self.assertEqual(prop1.get(PropClassAttr.PROPERTY_TYPE), OwlPropertyType.OwlDataProperty)
         self.assertEqual(prop1.creator, Xsd_anyURI('https://orcid.org/0000-0003-1681-4036'))
         self.assertEqual(prop1.created, datetime.fromisoformat("2023-11-04T12:00:00Z"))
 
         prop2 = r2[Xsd_QName("test:test")]
         self.assertIsNone(prop1.internal)
         self.assertEqual(prop2.property_class_iri, Xsd_QName('test:test'))
-        self.assertEqual(prop2[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
-        self.assertEqual(prop2[PropertyClassAttribute.NAME], LangString("Test"))
-        self.assertEqual(prop2[PropertyClassAttribute.DESCRIPTION], LangString("Property shape for testing purposes"))
-        self.assertEqual(prop2[PropertyClassAttribute.TO_NODE_IRI], Xsd_QName('test:comment'))
-        self.assertEqual(prop2[PropertyClassAttribute.ORDER], 3)
-        self.assertEqual(prop2[PropertyClassAttribute.PROPERTY_TYPE], OwlPropertyType.OwlObjectProperty)
+        self.assertEqual(prop2[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(prop2[PropClassAttr.NAME], LangString("Test"))
+        self.assertEqual(prop2[PropClassAttr.DESCRIPTION], LangString("Property shape for testing purposes"))
+        self.assertEqual(prop2[PropClassAttr.TO_NODE_IRI], Xsd_QName('test:comment'))
+        self.assertEqual(prop2[PropClassAttr.ORDER], 3)
+        self.assertEqual(prop2[PropClassAttr.PROPERTY_TYPE], OwlPropertyType.OwlObjectProperty)
 
         prop3 = r2[Xsd_QName("test:testone")]
         self.assertEqual(prop3.internal, Xsd_QName("test:TestResource"))
         self.assertEqual(prop3.property_class_iri, Xsd_QName("test:testone"))
-        self.assertEqual(prop3.get(PropertyClassAttribute.DATATYPE), XsdDatatypes.string)
-        self.assertEqual(prop3.get(PropertyClassAttribute.NAME), LangString(["Test property@en", "Testprädikat@de"]))
-        self.assertEqual(prop3.get(PropertyClassAttribute.DESCRIPTION), LangString("A property for testing...@en"))
-        self.assertEqual(prop3.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.MAX_COUNT], 1)
-        self.assertEqual(prop3.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.MIN_COUNT], 1)
-        self.assertEqual(prop3.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE, Language.FR, Language.IT})
-        self.assertTrue(prop3.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.UNIQUE_LANG])
-        self.assertEqual(prop3.get(PropertyClassAttribute.ORDER), 1)
+        self.assertEqual(prop3.get(PropClassAttr.DATATYPE), XsdDatatypes.string)
+        self.assertEqual(prop3.get(PropClassAttr.NAME), LangString(["Test property@en", "Testprädikat@de"]))
+        self.assertEqual(prop3.get(PropClassAttr.DESCRIPTION), LangString("A property for testing...@en"))
+        self.assertEqual(prop3.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.MAX_COUNT], 1)
+        self.assertEqual(prop3.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(prop3.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE, Language.FR, Language.IT})
+        self.assertTrue(prop3.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.UNIQUE_LANG])
+        self.assertEqual(prop3.get(PropClassAttr.ORDER), 1)
 
         prop4 = r2[Xsd_QName("test:testtwo")]
         self.assertEqual(prop4.internal, Xsd_QName("test:TestResource"))
         self.assertEqual(prop4.property_class_iri, Xsd_QName("test:testtwo"))
-        self.assertEqual(prop4.get(PropertyClassAttribute.TO_NODE_IRI), Xsd_QName('test:testMyRes'))
-        self.assertEqual(prop4.get(PropertyClassAttribute.NAME), LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]))
-        self.assertEqual(prop4.get(PropertyClassAttribute.DESCRIPTION), LangString("An exclusive property for testing...@en"))
-        self.assertEqual(prop4.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.MIN_COUNT], 1)
-        self.assertEqual(prop4.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE, Language.FR, Language.IT})
-        self.assertTrue(prop4.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.UNIQUE_LANG])
-        self.assertEqual(prop4.get(PropertyClassAttribute.ORDER), 2)
+        self.assertEqual(prop4.get(PropClassAttr.TO_NODE_IRI), Xsd_QName('test:testMyRes'))
+        self.assertEqual(prop4.get(PropClassAttr.NAME), LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]))
+        self.assertEqual(prop4.get(PropClassAttr.DESCRIPTION), LangString("An exclusive property for testing...@en"))
+        self.assertEqual(prop4.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(prop4.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE, Language.FR, Language.IT})
+        self.assertTrue(prop4.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.UNIQUE_LANG])
+        self.assertEqual(prop4.get(PropClassAttr.ORDER), 2)
 
         prop5 = r2[Xsd_QName("test:testthree")]
-        self.assertEqual(prop5.get(PropertyClassAttribute.RESTRICTIONS)[PropertyRestrictionType.IN], {1, 2, 3})
+        self.assertEqual(prop5.get(PropClassAttr.RESTRICTIONS)[PropertyRestrictionType.IN], {1, 2, 3})
 
     #@unittest.skip('Work in progress')
     def test_double_creation(self):
         properties: List[Union[PropertyClass, Xsd_QName]] = [
             Xsd_QName("test:comment"),
             Xsd_QName("test:test"),
         ]
@@ -405,27 +405,27 @@
         # Add an external, shared property defined by its own sh:PropertyShape instance
         #
         r1[Xsd_QName('test:test')] = None
 
         #
         # Adding an internal, private property
         #
-        attrs: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.TO_NODE_IRI: Xsd_QName('test:Person'),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs: PropClassAttrContainer = {
+            PropClassAttr.TO_NODE_IRI: Xsd_QName('test:Person'),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={PropertyRestrictionType.MAX_COUNT: 1}),
         }
         p = PropertyClass(con=self._connection,
                           graph=Xsd_NCName('test'),
                           attrs=attrs)
         r1[Xsd_QName('dcterms:creator')] = p
 
-        attrs2: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs2: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={PropertyRestrictionType.IN: {'A', 'B', 'C', 'D'}}),
         }
         p2 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            attrs=attrs2)
         r1[Xsd_QName('test:color')] = p2
         r1.update()
@@ -437,30 +437,30 @@
         self.assertEqual(r2.get(ResourceClassAttribute.COMMENT), LangString("Eine Beschreibung einer minimalen Ressource"))
         self.assertEqual(r2.get(ResourceClassAttribute.SUBCLASS_OF), Xsd_QName('test:testMyRes'))
         self.assertTrue(r2.get(ResourceClassAttribute.CLOSED))
 
         prop1 = r2[Xsd_QName('test:test')]
         self.assertIsNone(prop1.internal)
         self.assertEqual(prop1.property_class_iri, Xsd_QName('test:test'))
-        self.assertEqual(prop1[PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
-        self.assertEqual(prop1[PropertyClassAttribute.NAME], LangString("Test"))
-        self.assertEqual(prop1[PropertyClassAttribute.DESCRIPTION], LangString("Property shape for testing purposes"))
-        self.assertEqual(prop1[PropertyClassAttribute.TO_NODE_IRI], Xsd_QName('test:comment'))
-        self.assertEqual(prop1[PropertyClassAttribute.ORDER], 3)
-        self.assertEqual(prop1[PropertyClassAttribute.PROPERTY_TYPE], OwlPropertyType.OwlObjectProperty)
+        self.assertEqual(prop1[PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(prop1[PropClassAttr.NAME], LangString("Test"))
+        self.assertEqual(prop1[PropClassAttr.DESCRIPTION], LangString("Property shape for testing purposes"))
+        self.assertEqual(prop1[PropClassAttr.TO_NODE_IRI], Xsd_QName('test:comment'))
+        self.assertEqual(prop1[PropClassAttr.ORDER], 3)
+        self.assertEqual(prop1[PropClassAttr.PROPERTY_TYPE], OwlPropertyType.OwlObjectProperty)
 
         prop2 = r2[Xsd_QName('dcterms:creator')]
         self.assertEqual(prop2.internal, Xsd_QName("test:testMyResMinimal"))
-        self.assertEqual(prop2.get(PropertyClassAttribute.TO_NODE_IRI), Xsd_QName('test:Person'))
-        self.assertEqual(prop2[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.MAX_COUNT), 1)
-        self.assertEqual(prop1[PropertyClassAttribute.PROPERTY_TYPE], OwlPropertyType.OwlObjectProperty)
+        self.assertEqual(prop2.get(PropClassAttr.TO_NODE_IRI), Xsd_QName('test:Person'))
+        self.assertEqual(prop2[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.MAX_COUNT), 1)
+        self.assertEqual(prop1[PropClassAttr.PROPERTY_TYPE], OwlPropertyType.OwlObjectProperty)
 
         prop3 = r2[Xsd_QName('test:color')]
         self.assertEqual(prop3.internal, Xsd_QName("test:testMyResMinimal"))
-        self.assertEqual(prop3[PropertyClassAttribute.RESTRICTIONS].get(PropertyRestrictionType.IN),
+        self.assertEqual(prop3[PropClassAttr.RESTRICTIONS].get(PropertyRestrictionType.IN),
                          {'A', 'B', 'C', 'D'})
 
         sparql = self._context.sparql_context
         sparql += """
         SELECT ?p ?v
         FROM test:onto
         WHERE {
@@ -504,78 +504,78 @@
             self.assertEqual(result[p], v)
 
     #@unittest.skip('Work in progress')
     def test_updating(self):
         r1 = ResourceClass.read(con=self._connection,
                                 graph=Xsd_NCName('test'),
                                 owl_class_iri=Xsd_QName("test:testMyRes"))
-        self.assertEqual(r1[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 1)
-        self.assertEqual(r1[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
-        self.assertEqual(r1[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE})
+        self.assertEqual(r1[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 1)
+        self.assertEqual(r1[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MIN_COUNT], 1)
+        self.assertEqual(r1[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN], {Language.EN, Language.DE})
         r1[ResourceClassAttribute.LABEL][Language.IT] = "La mia risorsa"
         r1[ResourceClassAttribute.CLOSED] = False
         r1[ResourceClassAttribute.SUBCLASS_OF] = Xsd_QName('test:TopGaga')
-        r1[Xsd_QName('test:hasText')][PropertyClassAttribute.NAME][Language.FR] = "Un Texte Français"
-        r1[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT] = 12
-        r1[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN] = {Language.DE, Language.FR, Language.IT}
-        r1[Xsd_QName('test:hasEnum')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.IN] = {'L', 'a', 'b'}
+        r1[Xsd_QName('test:hasText')][PropClassAttr.NAME][Language.FR] = "Un Texte Français"
+        r1[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT] = 12
+        r1[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN] = {Language.DE, Language.FR, Language.IT}
+        r1[Xsd_QName('test:hasEnum')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.IN] = {'L', 'a', 'b'}
         r1.update()
 
         r2 = ResourceClass.read(con=self._connection,
                                 graph=Xsd_NCName('test'),
                                 owl_class_iri=Xsd_QName("test:testMyRes"))
         self.assertEqual(r2.get(ResourceClassAttribute.LABEL), LangString(["My Resource@en", "Meine Ressource@de", "Ma Resource@fr", "La mia risorsa@it"]))
         self.assertFalse(r2.get(ResourceClassAttribute.CLOSED))
         self.assertEqual(r2.get(ResourceClassAttribute.SUBCLASS_OF), Xsd_QName('test:TopGaga'))
-        self.assertEqual(r2[Xsd_QName('test:hasText')][PropertyClassAttribute.NAME], LangString(["A text", "Ein Text@de", "Un Texte Français@fr"]))
-        self.assertEqual(r2[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 12)
-        self.assertEqual(r2[Xsd_QName('test:hasText')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN], {Language.DE, Language.FR, Language.IT})
-        self.assertEqual(r2[Xsd_QName('test:hasEnum')][PropertyClassAttribute.RESTRICTIONS][PropertyRestrictionType.IN], {'L', 'a', 'b'})
+        self.assertEqual(r2[Xsd_QName('test:hasText')][PropClassAttr.NAME], LangString(["A text", "Ein Text@de", "Un Texte Français@fr"]))
+        self.assertEqual(r2[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.MAX_COUNT], 12)
+        self.assertEqual(r2[Xsd_QName('test:hasText')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.LANGUAGE_IN], {Language.DE, Language.FR, Language.IT})
+        self.assertEqual(r2[Xsd_QName('test:hasEnum')][PropClassAttr.RESTRICTIONS][PropertyRestrictionType.IN], {'L', 'a', 'b'})
 
     #@unittest.skip('Work in progress')
     def test_delete_props(self):
-        attrs1: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.SUBPROPERTY_OF: Xsd_QName('test:comment'),
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Test property@en", "Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("A property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs1: PropClassAttrContainer = {
+            PropClassAttr.SUBPROPERTY_OF: Xsd_QName('test:comment'),
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Test property@en", "Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("A property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 1
+            PropClassAttr.ORDER: 1
         }
         p1 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:propA'),
                            attrs=attrs1)
 
-        attrs2: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.TO_NODE_IRI: Xsd_QName('test:testMyRes'),
-            PropertyClassAttribute.NAME: LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("An exclusive property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs2: PropClassAttrContainer = {
+            PropClassAttr.TO_NODE_IRI: Xsd_QName('test:testMyRes'),
+            PropClassAttr.NAME: LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("An exclusive property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 2
+            PropClassAttr.ORDER: 2
         }
         p2 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:propB'),
                            attrs=attrs2)
 
-        attrs3: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.int,
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs3: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.int,
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.IN: {10, 20, 30}
                 }),
         }
         p3 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:propC'),
@@ -618,53 +618,53 @@
         self.assertTrue(check_prop_empty(self._connection, self._context, Graph.ONTO, 'test:testMyResMinimal', 'test:test'))
 
         self.assertTrue(check_prop_empty(self._connection, self._context, Graph.SHACL, 'test:testMyResMinimal', 'test:propC'))
         self.assertTrue(check_prop_empty(self._connection, self._context, Graph.ONTO, 'test:testMyResMinimal', 'test:propC'))
 
     #@unittest.skip('Work in progress')
     def test_delete(self):
-        attrs1: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.SUBPROPERTY_OF: Xsd_QName('test:comment'),
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-            PropertyClassAttribute.NAME: LangString(["Test property@en", "Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("A property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs1: PropClassAttrContainer = {
+            PropClassAttr.SUBPROPERTY_OF: Xsd_QName('test:comment'),
+            PropClassAttr.DATATYPE: XsdDatatypes.string,
+            PropClassAttr.NAME: LangString(["Test property@en", "Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("A property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MAX_COUNT: 1,
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 1
+            PropClassAttr.ORDER: 1
         }
         p1 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:deleteA'),
                            attrs=attrs1)
 
-        attrs2: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.TO_NODE_IRI: Xsd_QName('test:testMyRes'),
-            PropertyClassAttribute.NAME: LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]),
-            PropertyClassAttribute.DESCRIPTION: LangString("An exclusive property for testing...@en"),
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs2: PropClassAttrContainer = {
+            PropClassAttr.TO_NODE_IRI: Xsd_QName('test:testMyRes'),
+            PropClassAttr.NAME: LangString(["Excl. Test property@en", "Exkl. Testprädikat@de"]),
+            PropClassAttr.DESCRIPTION: LangString("An exclusive property for testing...@en"),
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.MIN_COUNT: 1,
                     PropertyRestrictionType.UNIQUE_LANG: True,
                     PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT}
                 }),
-            PropertyClassAttribute.ORDER: 2
+            PropClassAttr.ORDER: 2
         }
         p2 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:deleteB'),
                            attrs=attrs2)
 
-        attrs3: PropertyClassAttributesContainer = {
-            PropertyClassAttribute.DATATYPE: XsdDatatypes.int,
-            PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(
+        attrs3: PropClassAttrContainer = {
+            PropClassAttr.DATATYPE: XsdDatatypes.int,
+            PropClassAttr.RESTRICTIONS: PropertyRestrictions(
                 restrictions={
                     PropertyRestrictionType.IN: {10, 20, 30}
                 }),
         }
         p3 = PropertyClass(con=self._connection,
                            graph=Xsd_NCName('test'),
                            property_class_iri=Xsd_QName('test:deleteC'),
@@ -699,45 +699,45 @@
 
     #@unittest.skip('Work in progress')
     def test_write_trig(self):
         project_id = PropertyClass(con=self._connection,
                                    graph=Xsd_NCName('test'),
                                    property_class_iri=Xsd_QName('test:projectId'),
                                    attrs={
-                                       PropertyClassAttribute.DATATYPE: XsdDatatypes.NCName,
-                                       PropertyClassAttribute.NAME: LangString([
+                                       PropClassAttr.DATATYPE: XsdDatatypes.NCName,
+                                       PropClassAttr.NAME: LangString([
                                            "Project ID@en", "Projekt ID@de"
                                        ]),
-                                       PropertyClassAttribute.DESCRIPTION: LangString([
+                                       PropClassAttr.DESCRIPTION: LangString([
                                            "Unique ID for project@en", "Eindeutige ID für Projekt@de"
                                        ]),
-                                       PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(restrictions={
+                                       PropClassAttr.RESTRICTIONS: PropertyRestrictions(restrictions={
                                            PropertyRestrictionType.MIN_COUNT: 1,
                                            PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT},
                                            PropertyRestrictionType.UNIQUE_LANG: True
                                        }),
-                                       PropertyClassAttribute.ORDER: 1
+                                       PropClassAttr.ORDER: 1
                                    })
         project_name = PropertyClass(con=self._connection,
                                      graph=Xsd_NCName('test'),
                                      property_class_iri=Xsd_QName('test:projectName'),
                                      attrs={
-                                         PropertyClassAttribute.DATATYPE: XsdDatatypes.string,
-                                         PropertyClassAttribute.NAME: LangString([
+                                         PropClassAttr.DATATYPE: XsdDatatypes.string,
+                                         PropClassAttr.NAME: LangString([
                                              "Project name@en", "Projektname@de"
                                          ]),
-                                         PropertyClassAttribute.DESCRIPTION: LangString([
+                                         PropClassAttr.DESCRIPTION: LangString([
                                              "A description of the project@en", "EineBeschreibung des Projekts@de"
                                          ]),
-                                         PropertyClassAttribute.RESTRICTIONS: PropertyRestrictions(restrictions={
+                                         PropClassAttr.RESTRICTIONS: PropertyRestrictions(restrictions={
                                              PropertyRestrictionType.MIN_COUNT: 1,
                                              PropertyRestrictionType.LANGUAGE_IN: {Language.EN, Language.DE, Language.FR, Language.IT},
                                              PropertyRestrictionType.UNIQUE_LANG: True
                                          }),
-                                         PropertyClassAttribute.ORDER: 2
+                                         PropClassAttr.ORDER: 2
                                      })
 
         properties: List[Union[PropertyClass, Xsd_QName]] = [
             project_id, project_name
         ]
         attrs: ResourceClassAttributesContainer = {
             ResourceClassAttribute.LABEL: LangString(["Project@en", "Projekt@de"]),
```

### Comparing `omaslib-0.1.8/omaslib/test/test_user.py` & `omaslib-0.1.9/omaslib/test/test_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 from time import sleep
 
 from omaslib.src.connection import Connection
 from omaslib.src.helpers.context import Context
 from omaslib.src.helpers.tools import str2qname_anyiri
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_qname import Xsd_QName
 from omaslib.src.xsd.xsd_ncname import Xsd_NCName
 from omaslib.src.helpers.omaserror import OmasErrorNotFound, OmasErrorAlreadyExists, OmasErrorValue, OmasErrorNoPermission, OmasError
 from omaslib.src.enums.permissions import AdminPermission
 from omaslib.src.user import User
 from omaslib.src.in_project import InProjectClass
@@ -39,72 +40,73 @@
         cls._connection.clear_graph(Xsd_QName('omas:admin'))
         cls._connection.upload_turtle("omaslib/ontologies/admin.trig")
         sleep(1)  # upload may take a while...
 
     def tearDown(self):
         pass
 
+    # @unittest.skip('Work in progress')
     def test_constructor(self):
         user = User(con=self._connection,
                     userId=Xsd_NCName("testuser"),
                     familyName="Test",
                     givenName="Test",
                     credentials="Ein@geheimes&Passw0rt",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
-                                                               AdminPermission.ADMIN_RESOURCES,
-                                                               AdminPermission.ADMIN_CREATE}},
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                                                         AdminPermission.ADMIN_RESOURCES,
+                                                         AdminPermission.ADMIN_CREATE}},
                     hasPermissions={Xsd_QName('omas:GenericView')})
 
         self.assertEqual(user.userId, Xsd_NCName("testuser"))
         self.assertEqual(user.familyName, "Test")
         self.assertEqual(user.givenName, "Test")
-        self.assertEqual(user.inProject, InProjectClass({Xsd_QName("omas:HyperHamlet"): {
+        self.assertEqual(user.inProject, InProjectClass({Iri("omas:HyperHamlet"): {
             AdminPermission.ADMIN_USERS,
             AdminPermission.ADMIN_RESOURCES,
             AdminPermission.ADMIN_CREATE
         }}))
         self.assertEqual(user.hasPermissions, {Xsd_QName('omas:GenericView')})
 
     # @unittest.skip('Work in progress')
     def test_read_user(self):
         user = User.read(con=self._connection, userId="rosenth")
         self.assertEqual(user.userId, Xsd_NCName("rosenth"))
-        self.assertEqual(user.userIri, Xsd_anyURI("https://orcid.org/0000-0003-1681-4036"))
+        self.assertEqual(user.userIri, Iri("https://orcid.org/0000-0003-1681-4036"))
         self.assertEqual(user.familyName, Xsd_string("Rosenthaler"))
         self.assertEqual(user.givenName, Xsd_string("Lukas"))
         self.assertEqual(user.inProject, InProjectClass({
-            Xsd_QName("omas:SystemProject"): {AdminPermission.ADMIN_OLDAP},
-            Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_RESOURCES}
+            Iri("omas:SystemProject"): {AdminPermission.ADMIN_OLDAP},
+            Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_RESOURCES}
         }))
-        self.assertEqual(user.hasPermissions, {Xsd_QName("omas:GenericRestricted"), Xsd_QName('omas:GenericView')})
+        self.assertEqual(user.hasPermissions, {Iri("omas:GenericRestricted"), Iri('omas:GenericView')})
 
     # @unittest.skip('Work in progress')
     def test_read_unknown_user(self):
         with self.assertRaises(OmasErrorNotFound) as ex:
             user = User.read(con=self._connection, userId="nosuchuser")
         self.assertEqual(str(ex.exception), 'User "nosuchuser" not found.')
 
     # @unittest.skip('Work in progress')
     def test_search_user(self):
         users = User.search(con=self._connection, userId="fornaro")
-        self.assertEqual([Xsd_anyURI("https://orcid.org/0000-0003-1485-4923")], users)
+        self.assertEqual([Iri("https://orcid.org/0000-0003-1485-4923")], users)
 
         users = User.search(con=self._connection, familyName="Rosenthaler")
-        self.assertEqual([Xsd_anyURI("https://orcid.org/0000-0003-1681-4036")], users)
+        self.assertEqual([Iri("https://orcid.org/0000-0003-1681-4036")], users)
 
         users = User.search(con=self._connection, givenName="John")
-        self.assertEqual([Xsd_anyURI("urn:uuid:7e56b6c4-42e5-4a9d-94cf-d6e22577fb4b")], users)
+        self.assertEqual([Iri("urn:uuid:7e56b6c4-42e5-4a9d-94cf-d6e22577fb4b")], users)
 
         users = User.search(con=self._connection, inProject=Xsd_QName("omas:HyperHamlet"))
-        self.assertEqual([Xsd_anyURI("https://orcid.org/0000-0003-1681-4036"),
-                          Xsd_anyURI("https://orcid.org/0000-0003-1485-4923"),
-                          Xsd_anyURI("https://orcid.org/0000-0001-9277-3921")], users)
+        self.assertEqual([Iri("https://orcid.org/0000-0003-1681-4036"),
+                          Iri("https://orcid.org/0000-0003-1485-4923"),
+                          Iri("https://orcid.org/0000-0001-9277-3921")], users)
 
         users = User.search(con=self._connection, inProject=Xsd_anyURI("http://www.salsah.org/version/2.0/SwissBritNet"))
-        self.assertEqual([Xsd_anyURI("urn:uuid:7e56b6c4-42e5-4a9d-94cf-d6e22577fb4b")], users)
+        self.assertEqual([Iri("urn:uuid:7e56b6c4-42e5-4a9d-94cf-d6e22577fb4b")], users)
 
         users = User.search(con=self._connection, userId="GAGA")
         self.assertEqual([], users)
 
     # @unittest.skip('Work in progress')
     def test_search_user_injection(self):
         with self.assertRaises(OmasErrorValue) as ex:
@@ -114,28 +116,28 @@
         users = User.search(con=self._connection, familyName="Rosenthaler\".}\nSELECT * WHERE{?s ?p ?s})#")
         self.assertEqual(len(users), 0)
         users = User.search(con=self._connection, givenName="John\".}\nSELECT * WHERE{?s ?p ?s})#")
         self.assertEqual(len(users), 0)
 
         with self.assertRaises(OmasErrorValue) as ex:
             users = User.search(con=self._connection, inProject="omas:HyperHamlet\".}\nSELECT * WHERE{?s ?p ?s})#")
-        self.assertEqual(str(ex.exception), 'Invalid string "omas:HyperHamlet".}\nSELECT * WHERE{?s ?p ?s})#" for anyURI')
+        self.assertEqual(str(ex.exception), 'Invalid string for IRI: "omas:HyperHamlet".}\nSELECT * WHERE{?s ?p ?s})#"')
 
     # @unittest.skip('Work in progress')
     def test_create_user(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0003-3478-9313"),
+                    userIri=Iri("https://orcid.org/0000-0003-3478-9313"),
                     userId=Xsd_NCName("coyote"),
                     familyName="Coyote",
                     givenName="Wiley E.",
                     credentials="Super-Genius",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')},
+                    hasPermissions={Iri('omas:GenericView')},
                     isActive=True)
         user.create()
         user2 = User.read(con=self._connection, userId="coyote")
         self.assertEqual(user2.userId, user.userId)
         self.assertEqual(user2.userIri, user.userIri)
         self.assertEqual(user2.familyName, user.familyName)
         self.assertEqual(user2.givenName, user.givenName)
@@ -146,45 +148,45 @@
     # @unittest.skip('Work in progress')
     def test_create_user_no_admin_perms(self):
         user = User(con=self._connection,
                     userId=Xsd_NCName("birdy"),
                     familyName="Birdy",
                     givenName="Tweetie",
                     credentials="Sylvester",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {}},
-                    hasPermissions={Xsd_QName('omas:GenericView')},
+                    inProject={Iri('omas:HyperHamlet'): set()},
+                    hasPermissions={Iri('omas:GenericView')},
                     isActive=True)
         user.create()
         del user
         user = User.read(con=self._connection, userId=Xsd_NCName("birdy"))
         self.assertEqual(user.familyName, "Birdy")
 
     # @unittest.skip('Work in progress')
     def test_create_user_no_in_project(self):
         user = User(con=self._connection,
                     userId=Xsd_NCName("yogi"),
                     familyName="Baer",
                     givenName="Yogi",
                     credentials="BuBu",
-                    hasPermissions={Xsd_QName('omas:GenericView')},
+                    hasPermissions={Iri('omas:GenericView')},
                     isActive=True)
         user.create()
         del user
         user = User.read(con=self._connection, userId=Xsd_NCName("yogi"))
         self.assertEqual(user.familyName, "Baer")
 
     # @unittest.skip('Work in progress')
     def test_create_user_no_permset(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0003-3478-9313"),
+                    userIri=Iri("https://orcid.org/0000-0003-3478-9313"),
                     userId=Xsd_NCName("speedy"),
                     familyName="Ganzales",
                     givenName="Speedy",
                     credentials="fasterthanlight",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
                     isActive=True)
         user.create()
         del user
         user = User.read(con=self._connection, userId=Xsd_NCName("speedy"))
         self.assertEqual(user.familyName, "Ganzales")
@@ -193,124 +195,124 @@
     # @unittest.skip('Work in progress')
     def test_create_user_no_useriri(self):
         user = User(con=self._connection,
                     userId=Xsd_NCName("sylvester"),
                     familyName="Sylvester",
                     givenName="Cat",
                     credentials="Birdy",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')},
+                    hasPermissions={Iri('omas:GenericView')},
                     isActive=False)
         user.create()
         del user
         user = User.read(con=self._connection, userId=Xsd_NCName("sylvester"))
         self.assertTrue(str(user.userIri).startswith("urn:uuid:"))
         self.assertFalse(user.isActive)
 
     # @unittest.skip('Work in progress')
     def test_create_user_duplicate_userid(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0003-3478-9314"),
+                    userIri=Iri("https://orcid.org/0000-0003-3478-9314"),
                     userId=Xsd_NCName("fornaro"),
                     familyName="di Fornaro",
                     givenName="Petri",
                     credentials="Genius",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         with self.assertRaises(OmasErrorAlreadyExists) as ex:
             user.create()
         self.assertEqual(str(ex.exception), 'A user with a user ID "fornaro" already exists')
 
     # @unittest.skip('Work in progress')
     def test_create_user_duplicate_useriri(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0003-1681-4036"),
+                    userIri=Iri("https://orcid.org/0000-0003-1681-4036"),
                     userId=Xsd_NCName("brown"),
                     familyName="Brown",
                     givenName="Emmett",
                     credentials="Time-Machine@1985",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         with self.assertRaises(OmasErrorAlreadyExists) as ex:
             user.create()
         self.assertEqual(str(ex.exception), 'A user with a user IRI "https://orcid.org/0000-0003-1681-4036" already exists')
 
     # @unittest.skip('Work in progress')
     def test_create_user_invalid_project(self):
         user = User(con=self._connection,
                     userId=Xsd_NCName("donald"),
                     familyName="Duck",
                     givenName="Donald",
                     credentials="Entenhausen@for&Ever",
-                    inProject={Xsd_QName('omas:NotExistingproject'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:NotExistingproject'): {AdminPermission.ADMIN_USERS,
                                                                       AdminPermission.ADMIN_RESOURCES,
                                                                       AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         with self.assertRaises(OmasErrorValue) as ex:
             user.create()
         self.assertEqual(str(ex.exception), 'One of the projects is not existing!')
 
     # @unittest.skip('Work in progress')
     def test_create_user_invalid_permset(self):
         user = User(con=self._connection,
                     userId=Xsd_NCName("donald"),
                     familyName="Duck",
                     givenName="Donald",
                     credentials="Entenhausen@for&Ever",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView'), Xsd_QName('omas:Gaga')})
+                    hasPermissions={Iri('omas:GenericView'), Xsd_QName('omas:Gaga')})
         with self.assertRaises(OmasErrorValue) as ex:
             user.create()
         self.assertEqual(str(ex.exception), 'One of the permission sets is not existing!')
 
     # @unittest.skip('Work in progress')
     def test_create_user_no_privilege(self):
         user = User(con=self._unpriv,
                     userId=Xsd_NCName("donald"),
                     familyName="Duck",
                     givenName="Donald",
                     credentials="Entenhausen@for&Ever",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_CREATE}},
+                    hasPermissions={Iri('omas:GenericView')})
         with self.assertRaises(OmasErrorNoPermission) as ex:
             user.create()
         self.assertEqual(str(ex.exception), 'No permission to create user in project http://www.salsah.org/version/2.0/SwissBritNet.')
 
     # @unittest.skip('Work in progress')
     def test_create_user_no_connection(self):
         user = User(userId=Xsd_NCName("brown"),
                     familyName="Dock",
                     givenName="Donald",
                     credentials="Entenhausen@for&Ever",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_CREATE}},
+                    hasPermissions={Iri('omas:GenericView')})
         with self.assertRaises(OmasError) as ex:
             user.create()
         self.assertEqual(str(ex.exception), 'Cannot create: no connection')
 
     # @unittest.skip('Work in progress')
     def test_delete_user(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0002-9991-2055"),
+                    userIri=Iri("https://orcid.org/0000-0002-9991-2055"),
                     userId=Xsd_NCName("edison"),
                     familyName="Edison",
                     givenName="Thomas A.",
                     credentials="Lightbulb&Phonograph",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         user2 = User.read(con=self._connection, userId="edison")
         self.assertEqual(user2.userIri, user.userIri)
         user2.delete()
         with self.assertRaises(OmasErrorNotFound) as ex:
             user = User.read(con=self._connection, userId="edison")
         self.assertEqual(str(ex.exception), 'User "edison" not found.')
@@ -321,353 +323,364 @@
         with self.assertRaises(OmasErrorNoPermission) as ex:
             user.delete()
         self.assertEqual(str(ex.exception), 'No permission to delete user in project omas:HyperHamlet.')
 
     # @unittest.skip('Work in progress')
     def test_update_user(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0002-9991-2055"),
+                    userIri=Iri("https://orcid.org/0000-0002-9991-2055"),
                     userId=Xsd_NCName("edison"),
                     familyName="Edison",
                     givenName="Thomas A.",
                     credentials="Lightbulb&Phonograph",
-                    inProject={Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
+                    inProject={Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS,
                                                                AdminPermission.ADMIN_RESOURCES,
                                                                AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         user2 = User.read(con=self._connection, userId="edison")
         user2.userId = "aedison"
         user2.familyName = "Edison et al."
         user2.givenName = "Thomas"
-        user2.hasPermissions.add(Xsd_QName('omas:GenericRestricted'))
-        user2.hasPermissions.add(Xsd_QName('omas:HyperHamletMember'))
-        user2.hasPermissions.remove(Xsd_QName('omas:GenericView'))
-        user2.inProject[Xsd_QName('omas:SystemProject')] = {AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES}
-        user2.inProject[Xsd_QName('omas:HyperHamlet')].remove(AdminPermission.ADMIN_USERS)
+        user2.hasPermissions.add(Iri('omas:GenericRestricted'))
+        user2.hasPermissions.add(Iri('omas:HyperHamletMember'))
+        user2.hasPermissions.remove(Iri('omas:GenericView'))
+        user2.inProject[Iri('omas:SystemProject')] = {AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES}
+        user2.inProject[Iri('omas:HyperHamlet')].remove(AdminPermission.ADMIN_USERS)
         user2.update()
         user3 = User.read(con=self._connection, userId="aedison")
-        self.assertEqual({Xsd_QName('omas:GenericRestricted'), Xsd_QName('omas:HyperHamletMember')}, user3.hasPermissions)
-        user3.hasPermissions.add(Xsd_QName('omas:DoesNotExist'))
+        self.assertEqual({Iri('omas:GenericRestricted'), Iri('omas:HyperHamletMember')}, user3.hasPermissions)
+        user3.hasPermissions.add(Iri('omas:DoesNotExist'))
         with self.assertRaises(OmasErrorValue) as ex:
             user3.update()
             self.assertEqual(str(ex.exception), 'One of the permission sets is not existing!')
-        self.assertEqual(InProjectClass({Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_RESOURCES,
+        self.assertEqual(InProjectClass({Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_RESOURCES,
                                                                          AdminPermission.ADMIN_CREATE},
-                                         Xsd_QName('omas:SystemProject'): {AdminPermission.ADMIN_USERS,
+                                         Iri('omas:SystemProject'): {AdminPermission.ADMIN_USERS,
                                                                            AdminPermission.ADMIN_RESOURCES}}), user3.inProject)
         del user3
         user4 = User.read(con=self._connection, userId="aedison")
-        user4.inProject = InProjectClass({Xsd_QName('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS}})
+        user4.inProject = InProjectClass({Iri('omas:HyperHamlet'): {AdminPermission.ADMIN_USERS}})
         user4.update()
         del user4
 
     # @unittest.skip('Work in progress')
     def test_update_user_unpriv(self):
         user = User.read(con=self._unpriv, userId="bugsbunny")
         user.credentials = "ChangedPassword"
         with self.assertRaises(OmasErrorNoPermission) as ex:
             user.update()
         self.assertEqual(str(ex.exception), 'No permission to modify user in project omas:HyperHamlet.')
 
     # @unittest.skip('Work in progress')
     def test_update_user_change_in_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        user.inProject = InProjectClass({str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_OLDAP}})
+        user.inProject = InProjectClass({Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_OLDAP}})
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        self.assertEqual(user.inProject, InProjectClass({str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_OLDAP}}))
+        self.assertEqual(user.inProject, InProjectClass({Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {AdminPermission.ADMIN_OLDAP}}))
 
+    # @unittest.skip('Work in progress')
     def test_update_user_empty_in_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0002-2553-8814"),
+                    userIri=Iri("https://orcid.org/0000-0002-2553-8814"),
                     userId=Xsd_NCName("bsimpson"),
                     familyName="Simpson",
                     givenName="Bart",
                     credentials="AtomicPower",
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
-        user.inProject = InProjectClass({str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {
+        user.inProject = InProjectClass({Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
             AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES
         }})
         user.update()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
-        self.assertEqual(user.inProject, InProjectClass({str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {
+        self.assertEqual(user.inProject, InProjectClass({Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
             AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES
         }}))
 
+    # @unittest.skip('Work in progress')
     def test_update_user_rm_in_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
         user.inProject = None
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
         self.assertFalse(user.inProject)
 
+    # @unittest.skip('Work in progress')
     def test_update_user_del_in_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
         del user.inProject
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
         self.assertFalse(user.inProject)
 
+    # @unittest.skip('Work in progress')
     def test_update_user_add_to_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0002-2553-8814"),
+                    userIri=Iri("https://orcid.org/0000-0002-2553-8814"),
                     userId=Xsd_NCName("bsimpson"),
                     familyName="Simpson",
                     givenName="Bart",
                     credentials="AtomicPower",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
-        user.inProject[Xsd_QName('omas:HyperHamlet')] = {AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE}
+        user.inProject[Iri('omas:HyperHamlet')] = {AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE}
         user.update()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
         self.assertEqual(user.inProject, InProjectClass(
             {
-                str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                     AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE
                 },
-                str2qname_anyiri('omas:HyperHamlet'): {
+                Iri('omas:HyperHamlet'): {
                     AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE
                 }
             }
         ))
 
+    # @unittest.skip('Work in progress')
     def test_update_user_rm_from_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0002-2553-8814"),
+                    userIri=Iri("https://orcid.org/0000-0002-2553-8814"),
                     userId=Xsd_NCName("bsimpson"),
                     familyName="Simpson",
                     givenName="Bart",
                     credentials="AtomicPower",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE},
-                        str2qname_anyiri('omas:HyperHamlet'): {
+                        Iri('omas:HyperHamlet'): {
                             AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE
                         }
                     },
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
-        user.inProject[Xsd_QName('omas:HyperHamlet')] = None
+        user.inProject[Iri('omas:HyperHamlet')] = None
         user.update()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
         self.assertEqual(user.inProject, InProjectClass(
             {
-                str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                     AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE
                 }
             }
         ))
 
+    # @unittest.skip('Work in progress')
     def test_update_user_del_from_project(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0002-2553-8814"),
+                    userIri=Iri("https://orcid.org/0000-0002-2553-8814"),
                     userId=Xsd_NCName("bsimpson"),
                     familyName="Simpson",
                     givenName="Bart",
                     credentials="AtomicPower",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE},
-                        str2qname_anyiri('omas:HyperHamlet'): {
+                        Iri('omas:HyperHamlet'): {
                             AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE
                         }
                     },
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
-        del user.inProject[Xsd_QName('omas:HyperHamlet')]
+        del user.inProject[Iri('omas:HyperHamlet')]
         user.update()
         del user
         user = User.read(con=self._connection, userId="bsimpson")
         self.assertEqual(user.inProject, InProjectClass(
             {
-                str2qname_anyiri('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                     AdminPermission.ADMIN_USERS, AdminPermission.ADMIN_RESOURCES, AdminPermission.ADMIN_CREATE
                 }
             }
         ))
 
     # @unittest.skip('Work in progress')
     def test_update_user_del_has_permissions(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
         del user.hasPermissions
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
         self.assertFalse(user.hasPermissions)
 
+    # @unittest.skip('Work in progress')
     def test_update_user_add_has_permissions(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView')})
+                    hasPermissions={Iri('omas:GenericView')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        user.hasPermissions.add(Xsd_QName('omas:HyperHamletMember'))
+        user.hasPermissions.add(Iri('omas:HyperHamletMember'))
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        self.assertEqual(user.hasPermissions, {Xsd_QName('omas:GenericView'), Xsd_QName('omas:HyperHamletMember')})
+        self.assertEqual(user.hasPermissions, {Iri('omas:GenericView'), Iri('omas:HyperHamletMember')})
 
+    # @unittest.skip('Work in progress')
     def test_update_user_add_has_permissions(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        user.hasPermissions = {Xsd_QName('omas:GenericView'), Xsd_QName('omas:HyperHamletMember')}
+        user.hasPermissions = {Iri('omas:GenericView'), Iri('omas:HyperHamletMember')}
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        self.assertEqual(user.hasPermissions, {Xsd_QName('omas:GenericView'), Xsd_QName('omas:HyperHamletMember')})
+        self.assertEqual(user.hasPermissions, {Iri('omas:GenericView'), Iri('omas:HyperHamletMember')})
 
+    # @unittest.skip('Work in progress')
     def test_update_user_add_bad_has_permissions(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        user.hasPermissions = {Xsd_QName('omas:GAGA'), Xsd_QName('omas:HyperHamletMember')}
+        user.hasPermissions = {Iri('omas:GAGA'), Iri('omas:HyperHamletMember')}
         with self.assertRaises(OmasErrorValue) as err:
             user.update()
 
+    # @unittest.skip('Work in progress')
     def test_update_user_rm_has_permissions(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView'), Xsd_QName('omas:HyperHamletMember')})
+                    hasPermissions={Iri('omas:GenericView'), Iri('omas:HyperHamletMember')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        user.hasPermissions.discard(Xsd_QName('omas:HyperHamletMember'))
+        user.hasPermissions.discard(Iri('omas:HyperHamletMember'))
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        self.assertEqual(user.hasPermissions, {Xsd_QName('omas:GenericView')})
+        self.assertEqual(user.hasPermissions, {Iri('omas:GenericView')})
 
+    # @unittest.skip('Work in progress')
     def test_update_user_unexisting_has_permissions(self):
         user = User(con=self._connection,
-                    userIri=Xsd_anyURI("https://orcid.org/0000-0001-5925-2956"),
+                    userIri=Iri("https://orcid.org/0000-0001-5925-2956"),
                     userId=Xsd_NCName("chiquet"),
                     familyName="Chiquet",
                     givenName="Vera",
                     credentials="Photography",
-                    inProject={Xsd_anyURI('http://www.salsah.org/version/2.0/SwissBritNet'): {
+                    inProject={Iri('http://www.salsah.org/version/2.0/SwissBritNet'): {
                         AdminPermission.ADMIN_USERS,
                         AdminPermission.ADMIN_RESOURCES,
                         AdminPermission.ADMIN_CREATE}},
-                    hasPermissions={Xsd_QName('omas:GenericView'), Xsd_QName('omas:HyperHamletMember')})
+                    hasPermissions={Iri('omas:GenericView'), Iri('omas:HyperHamletMember')})
         user.create()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        user.hasPermissions.discard(Xsd_QName('omas:GenericRestricted'))
+        user.hasPermissions.discard(Iri('omas:GenericRestricted'))
         user.update()
         del user
         user = User.read(con=self._connection, userId="chiquet")
-        self.assertEqual(user.hasPermissions, {Xsd_QName('omas:GenericView'), Xsd_QName('omas:HyperHamletMember')})
+        self.assertEqual(user.hasPermissions, {Iri('omas:GenericView'), Iri('omas:HyperHamletMember')})
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `omaslib-0.1.8/omaslib/test/test_xsd_datatypes.py` & `omaslib-0.1.9/omaslib/test/test_xsd_datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from omaslib.src.dtypes.namespaceiri import NamespaceIRI
 from omaslib.src.dtypes.rdfset import RdfSet
 from omaslib.src.enums.language import Language
 from omaslib.src.helpers.context import Context
 from omaslib.src.helpers.omaserror import OmasErrorValue, OmasError
 from omaslib.src.helpers.query_processor import QueryProcessor
 from omaslib.src.helpers.serializer import serializer
+from omaslib.src.xsd.iri import Iri
 from omaslib.src.xsd.xsd import Xsd
 from omaslib.src.xsd.xsd_anyuri import Xsd_anyURI
 from omaslib.src.xsd.xsd_base64binary import Xsd_base64Binary
 from omaslib.src.xsd.xsd_boolean import Xsd_boolean
 from omaslib.src.xsd.xsd_byte import Xsd_byte
 from omaslib.src.xsd.xsd_date import Xsd_date
 from omaslib.src.xsd.xsd_datetime import Xsd_dateTime
@@ -107,22 +108,50 @@
         sparql = self._context.sparql_context
         sparql += f"""
         DELETE FROM test:test {{
             test:{name} test:prop ?value
         }}
         """
 
+    def test_iri(self):
+        val = Iri("test:whatiri")
+        self.assertEqual(str(val), 'test:whatiri')
+        self.assertEqual(repr(val), 'Iri("test:whatiri")')
+        self.assertEqual(val.toRdf, "test:whatiri")
+
+        jsonstr = json.dumps(val, default=serializer.encoder_default)
+        val2 = json.loads(jsonstr, object_hook=serializer.decoder_hook)
+        self.assertEqual(val, val2)
+
+        self.create_triple("Iri", val)
+        valx = self.get_triple("Iri")
+        self.assertEqual(val, valx)
+
+        val = Iri("http://this.is.not/gaga")
+        self.assertEqual(str(val), 'http://this.is.not/gaga')
+        self.assertEqual(repr(val), 'Iri("http://this.is.not/gaga")')
+        self.assertEqual(val.toRdf, "<http://this.is.not/gaga>")
+
+        jsonstr = json.dumps(val, default=serializer.encoder_default)
+        val2 = json.loads(jsonstr, object_hook=serializer.decoder_hook)
+        self.assertEqual(val, val2)
+
+        self.create_triple("Iri2", val)
+        valx = self.get_triple("Iri2")
+        self.assertEqual(val, valx)
+
+
+
     def test_xsd_anyuri(self):
         val = Xsd_anyURI('http://www.org/test')
         self.assertEqual(str(val), 'http://www.org/test')
         self.assertEqual(repr(val), 'Xsd_anyURI("http://www.org/test")')
         self.assertEqual(len(val), 19)
         self.assertFalse(val.append_allowed)
         self.assertEqual(val.toRdf, '"http://www.org/test"^^xsd:anyURI')
-        self.assertEqual(val.resUri, '<http://www.org/test>')
         self.assertEqual(val.value, 'http://www.org/test')
         nnn = None
         self.assertFalse(val == nnn)
 
         jsonstr = json.dumps(val, default=serializer.encoder_default)
         val2 = json.loads(jsonstr, object_hook=serializer.decoder_hook)
         self.assertEqual(val, val2)
@@ -368,14 +397,15 @@
             val = Xsd_dateTime('01-10-26T21:32')
 
     def test_xsd_decimal(self):
         val = Xsd_decimal(3.141592653589793)
         self.assertEqual(float(val), 3.141592653589793)
         self.assertEqual(str(val), '3.141592653589793')
         self.assertEqual(repr(val), 'Xsd_decimal("3.141592653589793")')
+        self.assertEqual(val.toRdf, '"3.141592653589793"^^xsd:decimal')
         nnn: Xsd_decimal | None = None
         self.assertFalse(val == nnn)
 
         valc = Xsd_decimal(val)
         self.assertEqual(val, valc)
 
         jsonstr = json.dumps(val, default=serializer.encoder_default)
```

### Comparing `omaslib-0.1.8/omaslib/testdata/connection_test.trig` & `omaslib-0.1.9/omaslib/testdata/connection_test.trig`

 * *Files 20% similar despite different names*

```diff
@@ -9,120 +9,120 @@
 @prefix omas: <http://omas.org/base#> .
 @prefix test: <http://omas.org/test#> .
 @prefix : <http://omas.org/test#> .
 
 
 :shacl {
 
-    :shapes dcterms:hasVersion "1.0.0" ;
+    :shapes dcterms:hasVersion "1.0.0"^^xsd:string ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime .
 
-    :shaclinfo dcterms:hasVersion "1.0.0" .
+    :shaclinfo dcterms:hasVersion "1.0.0"^^xsd:string .
 
     :commentShape a sh:PropertyShape ;
         sh:path :comment ;
         sh:name "comment"@en, "Kommentar"@de ;
         sh:description "This is a test property"@de ;
         sh:datatype xsd:string ;
         sh:uniqueLang true ;
-        sh:languageIn ("de" "fr" "en") ;
-        sh:maxCount 1 ;
-        sh:order 2 ;
-        dcterms:hasVersion "1.0.0" ;
+        sh:languageIn ("de"^^xsd:string "fr"^^xsd:string "en"^^xsd:string) ;
+        sh:maxCount "1"^^xsd:integer ;
+        sh:order "2"^^xsd:decimal ;
+        dcterms:hasVersion "1.0.0"^^xsd:string ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime .
 
     :testShape a sh:PropertyShape ;
         sh:path :test ;
         sh:name "Test" ;
-        sh:description "Property shape for testing purposes" ;
+        sh:description "Property shape for testing purposes";
         sh:class :comment ;
-        sh:minCount 1 ;
-        sh:order 3 ;
-        dcterms:hasVersion "1.0.0" ;
+        sh:minCount "1"^^xsd:integer ;
+        sh:order "3"^^xsd:decimal ;
+        dcterms:hasVersion "1.0.0"^^xsd:string ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime .
 
     :enumShape a sh:PropertyShape ;
         sh:path :enum ;
         sh:name "Enum" ;
         sh:datatype xsd:string ;
-        sh:in ( "very good" "good" "fair" "insufficient" ) ;
-        sh:order 4 ;
-        dcterms:hasVersion "1.0.0" ;
+        sh:in ( "very good"^^xsd:string "good"^^xsd:string "fair"^^xsd:string "insufficient"^^xsd:string ) ;
+        sh:order "4"^^xsd:decimal ;
+        dcterms:hasVersion "1.0.0"^^xsd:string ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime .
 
     :testMyResShape a sh:NodeShape, :testMyRes ;
         sh:targetClass :testMyRes ;
-        dcterms:hasVersion "1.0.0" ;
+        dcterms:hasVersion "1.0.0"^^xsd:string ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         rdfs:label "My Resource"@en, "Meine Ressource"@de, "Ma Resource"@fr ;
-        rdfs:comment "Resource for testing..." ;
+        rdfs:comment "Resource for testing..."^^xsd:string ;
         sh:property
             [
                 sh:path rdf:type ;
             ] ;
         sh:property :testShape ;
         sh:property
             [
                 sh:path :hasText ;
-                dcterms:hasVersion "1.0.0" ;
+                dcterms:hasVersion "1.0.0"^^xsd:string ;
                 dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
                 dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
                 dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
                 dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
                 sh:datatype xsd:string ;
-                sh:languageIn ("de" "en") ;
-                sh:maxCount 1 ;
-                sh:minCount 1 ;
-                sh:name "A text", "Ein Text"@de ;
-                sh:description "A longer text..." ;
-                sh:order 1 ;
+                sh:languageIn ("de"^^xsd:string "en"^^xsd:string) ;
+                sh:maxCount "1"^^xsd:integer ;
+                sh:minCount "1"^^xsd:integer ;
+                sh:name "A text"^^xsd:string, "Ein Text"@de ;
+                sh:description "A longer text..."^^xsd:string ;
+                sh:order "1"^^xsd:decimal ;
             ] ;
         sh:property
             [
                 sh:path :hasEnum ;
-                dcterms:hasVersion "1.0.0" ;
+                dcterms:hasVersion "1.0.0"^^xsd:string ;
                 dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
                 dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
                 dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
                 dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
                 sh:datatype xsd:string ;
-                sh:in ('red' 'green' 'blue' 'yellow')
+                sh:in ('red'^^xsd:string 'green'^^xsd:string 'blue'^^xsd:string 'yellow'^^xsd:string)
             ] ;
         sh:closed true .
 
     :testMyResMinimalShape a sh:NodeShape, :testMyResMinimal ;
         sh:targetClass :testMyResMinimal ;
-        dcterms:hasVersion "1.0.0" ;
+        dcterms:hasVersion "1.0.0"^^xsd:string ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         sh:property
             [
                 sh:path rdf:type ;
             ] ;
         sh:property
             [
                 sh:path :hasMinimal ;
-                dcterms:hasVersion "1.0.0" ;
+                dcterms:hasVersion "1.0.0"^^xsd:string ;
                 dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
                 dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
                 dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
                 dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
                 sh:datatype xsd:string ;
             ] ;
         sh:closed true .
@@ -192,20 +192,20 @@
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         rdfs:subClassOf
             [
                 rdf:type owl:Restriction ;
                 owl:onProperty :test ;
-                owl:minCardinality 1 ;
+                owl:minCardinality "1"^^xsd:nonNegativeInteger ;
             ],
             [
                 rdf:type owl:Restriction ;
                 owl:onProperty :hasText ;
-                owl:cardinality 1 ;
+                owl:cardinality "1"^^xsd:nonNegativeInteger ;
             ] .
 
     :testMyResMinimal a owl:Class ;
         dcterms:creator <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:created "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
         dcterms:contributor <https://orcid.org/0000-0003-1681-4036> ;
         dcterms:modified "2023-11-04T12:00:00+00:00"^^xsd:dateTime ;
```

### Comparing `omaslib-0.1.8/omaslib/testdata/datamodel_test.trig` & `omaslib-0.1.9/omaslib/testdata/datamodel_test.trig`

 * *Files identical despite different names*

### Comparing `omaslib-0.1.8/pyproject.toml` & `omaslib-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omaslib"
-version = "0.1.8"
+version = "0.1.9"
 description = "Open Media Access Server Library (Linked Open Data middleware/RESTApi)"
 authors = ["Lukas Rosenthaler <lukas.rosenthaler@unibas.ch>"]
 license = "GNU Affero General Public License version 3"
 readme = "README.md"
 
 [tool.mkdocs]
 plugins = ["mkdocs-material", "mkdocstrings"]
```

### Comparing `omaslib-0.1.8/PKG-INFO` & `omaslib-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omaslib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Media Access Server Library (Linked Open Data middleware/RESTApi)
 License: GNU Affero General Public License version 3
 Author: Lukas Rosenthaler
 Author-email: lukas.rosenthaler@unibas.ch
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

