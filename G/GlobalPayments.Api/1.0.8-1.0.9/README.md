# Comparing `tmp/GlobalPayments.Api-1.0.8.tar.gz` & `tmp/GlobalPayments.Api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlobalPayments.Api-1.0.8.tar", last modified: Thu Aug  3 14:24:37 2023, max compression
+gzip compressed data, was "GlobalPayments.Api-1.0.9.tar", last modified: Tue Aug 22 13:05:13 2023, max compression
```

## Comparing `GlobalPayments.Api-1.0.8.tar` & `GlobalPayments.Api-1.0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/
--rw-rw-rw-   0        0        0      910 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15439 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      910 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/globalpayments/
--rw-rw-rw-   0        0        0       36 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/globalpayments/api/
--rw-rw-rw-   0        0        0    10064 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/globalpayments/api/builders/
--rw-rw-rw-   0        0        0    13980 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/__init__.py
--rw-rw-rw-   0        0        0     2807 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/management_builder.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.164099 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/
--rw-rw-rw-   0        0        0      322 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/__init__.py
--rw-rw-rw-   0        0        0     2742 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_clause.py
--rw-rw-rw-   0        0        0     1125 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_target.py
--rw-rw-rw-   0        0        0     2194 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validations.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.171340 GlobalPayments.Api-1.0.8/globalpayments/api/entities/
--rw-rw-rw-   0        0        0    15101 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/__init__.py
--rw-rw-rw-   0        0        0    18729 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/address.py
--rw-rw-rw-   0        0        0      176 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/batch_summary.py
--rw-rw-rw-   0        0        0      244 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/debit_mac.py
--rw-rw-rw-   0        0        0      658 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/ecommerce_info.py
--rw-rw-rw-   0        0        0      601 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/encryption_data.py
--rw-rw-rw-   0        0        0    12813 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/enums.py
--rw-rw-rw-   0        0        0     1837 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/exceptions.py
--rw-rw-rw-   0        0        0      300 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/hosted_payment_data.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.177003 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/base_table_service_response.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/bump_status_collection.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/login_response.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/server_assignment_response.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/server_list_response.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/shift_assignments.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/table_service_response.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/ticket.py
--rw-rw-rw-   0        0        0      211 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/three_d_secure.py
--rw-rw-rw-   0        0        0      640 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/transaction_summary.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.177003 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/
--rw-rw-rw-   0        0        0   100825 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/__init__.py
--rw-rw-rw-   0        0        0       81 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/gateway_response.py
--rw-rw-rw-   0        0        0       48 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/table_service_connector.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.177003 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/
--rw-rw-rw-   0        0        0      583 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/cash.py
--rw-rw-rw-   0        0        0     8601 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/credit.py
--rw-rw-rw-   0        0        0     2256 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/debit.py
--rw-rw-rw-   0        0        0     2202 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/ebt.py
--rw-rw-rw-   0        0        0     1259 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/echeck.py
--rw-rw-rw-   0        0        0     3302 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/giftcard.py
--rw-rw-rw-   0        0        0     1274 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/payment_interfaces.py
--rw-rw-rw-   0        0        0      173 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/transaction_reference.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/globalpayments/api/services/
--rw-rw-rw-   0        0        0      220 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/__init__.py
--rw-rw-rw-   0        0        0      354 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/batch_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/credit_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/debit_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/device_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/ebt_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/gift_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/hosted_service.py
--rw-rw-rw-   0        0        0     1127 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/recurring_service.py
--rw-rw-rw-   0        0        0      589 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/reporting_service.py
--rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/table_service.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/globalpayments/api/utils/
--rw-rw-rw-   0        0        0     6127 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1159 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.315665 GlobalPayments.Api-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.128701 GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-08-22 13:05:12.000000 GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2023-08-22 13:05:12.000000 GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-22 13:05:12.000000 GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-08-22 13:05:12.000000 GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-22 13:05:12.000000 GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15439 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      910 2023-08-22 13:05:13.315665 GlobalPayments.Api-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.131700 GlobalPayments.Api-1.0.9/globalpayments/
+-rw-rw-rw-   0        0        0       36 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.135702 GlobalPayments.Api-1.0.9/globalpayments/api/
+-rw-rw-rw-   0        0        0    10064 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.143665 GlobalPayments.Api-1.0.9/globalpayments/api/builders/
+-rw-rw-rw-   0        0        0    13980 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/builders/__init__.py
+-rw-rw-rw-   0        0        0     2807 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/builders/management_builder.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.158664 GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/
+-rw-rw-rw-   0        0        0      322 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/__init__.py
+-rw-rw-rw-   0        0        0     2742 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/validation_clause.py
+-rw-rw-rw-   0        0        0     1125 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/validation_target.py
+-rw-rw-rw-   0        0        0     2194 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/validations.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.204665 GlobalPayments.Api-1.0.9/globalpayments/api/entities/
+-rw-rw-rw-   0        0        0    15101 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/__init__.py
+-rw-rw-rw-   0        0        0    18729 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/address.py
+-rw-rw-rw-   0        0        0      176 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/batch_summary.py
+-rw-rw-rw-   0        0        0      244 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/debit_mac.py
+-rw-rw-rw-   0        0        0      658 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/ecommerce_info.py
+-rw-rw-rw-   0        0        0      601 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/encryption_data.py
+-rw-rw-rw-   0        0        0    12813 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/enums.py
+-rw-rw-rw-   0        0        0     1837 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/exceptions.py
+-rw-rw-rw-   0        0        0      300 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/hosted_payment_data.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.227668 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/base_table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/bump_status_collection.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/login_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/server_assignment_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/server_list_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/shift_assignments.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/table_service/ticket.py
+-rw-rw-rw-   0        0        0      211 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/three_d_secure.py
+-rw-rw-rw-   0        0        0      640 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/entities/transaction_summary.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.239665 GlobalPayments.Api-1.0.9/globalpayments/api/gateways/
+-rw-rw-rw-   0        0        0   101378 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/gateways/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/gateways/gateway_response.py
+-rw-rw-rw-   0        0        0       48 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/gateways/table_service_connector.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.276665 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/
+-rw-rw-rw-   0        0        0      583 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/cash.py
+-rw-rw-rw-   0        0        0     8601 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/credit.py
+-rw-rw-rw-   0        0        0     2256 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/debit.py
+-rw-rw-rw-   0        0        0     2202 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/ebt.py
+-rw-rw-rw-   0        0        0     1259 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/echeck.py
+-rw-rw-rw-   0        0        0     3302 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/giftcard.py
+-rw-rw-rw-   0        0        0     1274 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/payment_interfaces.py
+-rw-rw-rw-   0        0        0      173 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/transaction_reference.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.309667 GlobalPayments.Api-1.0.9/globalpayments/api/services/
+-rw-rw-rw-   0        0        0      220 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/batch_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/credit_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/debit_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/device_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/ebt_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/gift_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/hosted_service.py
+-rw-rw-rw-   0        0        0     1127 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/recurring_service.py
+-rw-rw-rw-   0        0        0      589 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/reporting_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/services/table_service.py
+drwxrwxrwx   0        0        0        0 2023-08-22 13:05:13.312665 GlobalPayments.Api-1.0.9/globalpayments/api/utils/
+-rw-rw-rw-   0        0        0     6127 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/globalpayments/api/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-22 13:05:13.316667 GlobalPayments.Api-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2023-08-22 13:03:01.000000 GlobalPayments.Api-1.0.9/setup.py
```

### Comparing `GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/PKG-INFO` & `GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlobalPayments.Api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Global Payments Python SDK for integrating with Heartland and Global Payments merchant services APIs.
 Home-page: https://developer.heartlandpaymentsystems.com/
 Author: Heartland Payment Systems
 Author-email: EntApp_DevPortal@e-hps.com
 License: LICENSE.md
 License-File: LICENSE.md
```

### Comparing `GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/SOURCES.txt` & `GlobalPayments.Api-1.0.9/GlobalPayments.Api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/LICENSE.md` & `GlobalPayments.Api-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/PKG-INFO` & `GlobalPayments.Api-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlobalPayments.Api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Global Payments Python SDK for integrating with Heartland and Global Payments merchant services APIs.
 Home-page: https://developer.heartlandpaymentsystems.com/
 Author: Heartland Payment Systems
 Author-email: EntApp_DevPortal@e-hps.com
 License: LICENSE.md
 License-File: LICENSE.md
```

### Comparing `GlobalPayments.Api-1.0.8/README.txt` & `GlobalPayments.Api-1.0.9/README.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/__init__.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/builders/__init__.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/builders/management_builder.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/builders/management_builder.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_clause.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/validation_clause.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_target.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/validation_target.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validations.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/builders/validations/validations.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/__init__.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/address.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/address.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/ecommerce_info.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/ecommerce_info.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/encryption_data.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/encryption_data.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/enums.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/enums.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/exceptions.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/entities/transaction_summary.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/entities/transaction_summary.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/gateways/__init__.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/gateways/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,15 +844,14 @@
 
         elif isinstance(builder.payment_method, ECheck):
             check = builder.payment_method
 
             # check action
             et.SubElement(block1, 'CheckAction').text = 'SALE'
 
-            # account info
             if not has_token:
                 account_info = et.SubElement(block1, 'AccountInfo')
                 if check.routing_number:
                     et.SubElement(account_info,
                                   'RoutingNumber').text = check.routing_number
                 if check.account_number:
                     et.SubElement(account_info,
@@ -865,14 +864,25 @@
                                   'MICRData').text = check.micr_number
                 if check.account_type:
                     et.SubElement(
                         account_info,
                         'AccountType').text = check.account_type.value
             else:
                 et.SubElement(block1, 'TokenValue').text = token_value
+                account_info = et.SubElement(block1, 'AccountInfo')
+                if check.check_number:
+                    et.SubElement(account_info,
+                                  'CheckNumber').text = check.check_number
+                if check.micr_number:
+                    et.SubElement(account_info,
+                                  'MICRData').text = check.micr_number
+                if check.account_type:
+                    et.SubElement(
+                        account_info,
+                        'AccountType').text = check.account_type.value
 
             if check.entry_mode:
                 et.SubElement(
                     block1,
                     'DataEntryMode').text = check.entry_mode.value.upper()
             if check.check_type:
                 et.SubElement(block1,
```

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/__init__.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/credit.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/credit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/debit.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/debit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/ebt.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/ebt.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/echeck.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/echeck.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/giftcard.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/giftcard.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/payment_interfaces.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/payment_methods/payment_interfaces.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/services/recurring_service.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/services/recurring_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/services/reporting_service.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/services/reporting_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/globalpayments/api/utils/__init__.py` & `GlobalPayments.Api-1.0.9/globalpayments/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.8/setup.py` & `GlobalPayments.Api-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='GlobalPayments.Api',
-    version='1.0.8',
+    version='1.0.9',
     author='Heartland Payment Systems',
     author_email='EntApp_DevPortal@e-hps.com',
     packages=[
         'globalpayments', 'globalpayments.api', 'globalpayments.api.builders',
         'globalpayments.api.builders.validations',
         'globalpayments.api.entities',
         'globalpayments.api.entities.table_service',
```

