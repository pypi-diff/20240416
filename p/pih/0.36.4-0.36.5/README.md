# Comparing `tmp/pih-0.36.4.tar.gz` & `tmp/pih-0.36.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.4.tar", last modified: Thu Apr 11 12:07:24 2024, max compression
+gzip compressed data, was "pih-0.36.5.tar", last modified: Mon Apr 15 00:26:27 2024, max compression
```

## Comparing `pih-0.36.4.tar` & `pih-0.36.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:24.276051 pih-0.36.4/
--rw-rw-rw-   0        0        0      249 2024-04-11 12:07:24.244802 pih-0.36.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:21.881553 pih-0.36.4/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.4/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:22.209636 pih-0.36.4/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.4/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.4/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.4/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.4/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:23.502491 pih-0.36.4/pih/consts/
--rw-rw-rw-   0        0        0    25249 2024-04-11 12:06:08.000000 pih-0.36.4/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.4/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.4/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.4/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.4/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.4/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36.4/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.4/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.4/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.4/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.4/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.4/pih/consts/password.py
--rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.4/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11096 2024-04-10 11:19:30.000000 pih-0.36.4/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.4/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.4/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.4/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.4/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.4/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.4/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.4/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.4/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.4/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   547821 2024-04-10 22:10:26.000000 pih-0.36.4/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:23.651073 pih-0.36.4/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.4/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.4/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.4/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.4/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:23.854207 pih-0.36.4/pih/tools/
--rw-rw-rw-   0        0        0    51601 2024-04-11 12:03:46.000000 pih-0.36.4/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.4/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.4/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:07:24.197931 pih-0.36.4/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-11 12:07:20.000000 pih-0.36.4/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-11 12:07:20.000000 pih-0.36.4/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 12:07:20.000000 pih-0.36.4/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-11 12:07:20.000000 pih-0.36.4/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-11 12:07:20.000000 pih-0.36.4/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 12:07:24.276051 pih-0.36.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:28.052590 pih-0.36.5/
+-rw-rw-rw-   0        0        0      249 2024-04-15 00:26:28.036934 pih-0.36.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:25.487167 pih-0.36.5/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.5/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:25.915098 pih-0.36.5/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.5/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.5/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.5/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.5/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:27.236048 pih-0.36.5/pih/consts/
+-rw-rw-rw-   0        0        0    25249 2024-04-15 00:24:39.000000 pih-0.36.5/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.5/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.5/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.5/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.5/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.5/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30001 2024-04-14 23:55:41.000000 pih-0.36.5/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.5/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.5/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.5/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.5/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.5/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.5/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11096 2024-04-10 11:19:30.000000 pih-0.36.5/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.5/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.5/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.5/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.5/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.5/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.5/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.5/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.5/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.5/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547832 2024-04-12 13:18:27.000000 pih-0.36.5/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:27.454668 pih-0.36.5/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.5/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.5/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.5/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.5/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:27.942164 pih-0.36.5/pih/tools/
+-rw-rw-rw-   0        0        0    51601 2024-04-11 12:03:46.000000 pih-0.36.5/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.5/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.5/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:26:28.004664 pih-0.36.5/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-15 00:26:23.000000 pih-0.36.5/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-15 00:26:24.000000 pih-0.36.5/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:26:23.000000 pih-0.36.5/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 00:26:23.000000 pih-0.36.5/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-15 00:26:23.000000 pih-0.36.5/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:26:28.068218 pih-0.36.5/setup.cfg
```

### Comparing `pih-0.36.4/pih/collections/__init__.py` & `pih-0.36.5/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/collections/service.py` & `pih-0.36.5/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/console_api.py` & `pih-0.36.5/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/console_api_wrapper.py` & `pih-0.36.5/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/__init__.py` & `pih-0.36.5/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36.4"
+VERSION: str = "0.36.5"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.36.4/pih/consts/ad.py` & `pih-0.36.5/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/addresses.py` & `pih-0.36.5/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/date_time.py` & `pih-0.36.5/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/errors.py` & `pih-0.36.5/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/events.py` & `pih-0.36.5/pih/consts/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
         "Создана полибейс персона: {name} ({pin})",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.NOTIFICATION,
         (PARAM_ITEMS.NAME, PARAM_ITEMS.PIN, PARAM_ITEMS.VALUE),
     )
 
     POLIBASE_PERSON_ANSWERED = EventDescription(
-        "Пациент: {} ({}) ответил: {} на получение ссылки",
+        "Клиент: {} ({}) ответил: {} на получение ссылки",
         LogMessageChannels.POLIBASE,
         (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE),
         (PARAM_ITEMS.PIN, PARAM_ITEMS.TELEPHONE_NUMBER, PARAM_ITEMS.VALUE),
     )
 
     MAIL_TO_POLIBASE_PERSON_WAS_SENT = EventDescription(
         "Почта с медицинской записью {id} была отправлена пациенту: {pin}",
@@ -500,15 +500,15 @@
         None,
         LogMessageChannels.POLIBASE,
         (LogMessageFlags.SAVE_ONCE, LogMessageFlags.SILENCE),
         (PARAM_ITEMS.PERSON_PIN.configurate(key=True), PARAM_ITEMS.INPATIENT),
     )
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_ANSWERED = EventDescription(
-        "Пациент: {}, ответил на уведомление об отзыве: {} ({})",
+        "Клиент: {}, ответил на уведомление об отзыве: {} ({})",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.SAVE_ONCE,
         (
             PARAM_ITEMS.PERSON_PIN.configurate(key=True),
             PARAM_ITEMS.VALUE,
             PARAM_ITEMS.STATUS,
         ),
@@ -517,60 +517,70 @@
     POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED = EventDescription(
         "Полибейс: обнаружены пациенты со старым форматом или отсутствующим штрих-кодом",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.SILENCE,
         (PARAM_ITEMS.PERSON_PIN,),
     )
 
+    POLIBASE_PERSONS_BONUS_CARD_WAS_CREATED = EventDescription(
+        "Бонусная карта для клиента {} была создана",
+        LogMessageChannels.POLIBASE,
+        (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE),
+        (
+            PARAM_ITEMS.PERSON_PIN.configurate(key=True),
+            ParamItem("url", "").configurate(visible=False),
+        ),
+    )
+
     POLIBASE_PERSON_BARCODES_WITH_OLD_FORMAT_WERE_CREATED = EventDescription(
-        "Полибейс: все новые штрих-коды созданы",
+        "Все штрих-коды для новых клиентов созданы",
         LogMessageChannels.POLIBASE,
         LogMessageFlags.SILENCE,
         (PARAM_ITEMS.PERSON_PIN,),
     )
 
     POLIBASE_PERSON_WITH_INACCESSABLE_EMAIL_WAS_DETECTED = EventDescription(
-        "Пациент {} ({}) имеет недоступную электронную почту: {}. Регистратор: {}, компьютер: {} ({})",
+        "Клиент {} ({}) имеет недоступную электронную почту: {}. Регистратор: {}, компьютер: {} ({})",
         LogMessageChannels.POLIBASE_ERROR,
         LogMessageFlags.SAVE,
         (
             PARAM_ITEMS.PERSON_NAME,
             PARAM_ITEMS.PERSON_PIN,
             PARAM_ITEMS.EMAIL,
             PARAM_ITEMS.REGISTRATOR_PERSON_NAME,
             ParamItem(FIELD_NAME_COLLECTION.WORKSTATION_NAME, ""),
             ParamItem(FIELD_NAME_COLLECTION.WORKSTATION_DESCRIPTION, ""),
         ),
     )
 
     POLIBASE_PERSON_EMAIL_WAS_ADDED = EventDescription(
-        "Электронная почта пациента {} ({}): {} была добавлена",
+        "Электронная почта клиента {} ({}): {} была добавлена",
         LogMessageChannels.POLIBASE,
         (LogMessageFlags.RESULT, LogMessageFlags.SAVE),
         (
             PARAM_ITEMS.PERSON_NAME,
             PARAM_ITEMS.PERSON_PIN,
             PARAM_ITEMS.EMAIL,
         ),
     )
 
     ASK_FOR_POLIBASE_PERSON_EMAIL = EventDescription(
-        "Запрос электронной почта у пациента {} ({}). Локально: {}",
+        "Запрос электронной почта у клиента {} ({}). Локально: {}",
         LogMessageChannels.POLIBASE,
         (LogMessageFlags.NOTIFICATION, LogMessageFlags.SEND_ONCE),
         (
             PARAM_ITEMS.PERSON_NAME.configurate(saved=False),
             PARAM_ITEMS.PERSON_PIN.configurate(key=True),
             PARAM_ITEMS.LOCALY,
             PARAM_ITEMS.SECRET.configurate(visible=False),
         ),
     )
 
     POLIBASE_PERSON_BONUSES_WAS_UPDATED = EventDescription(
-        "Бонусы пациента {} обновились",
+        "Бонусы клиента {} обновились",
         LogMessageChannels.POLIBASE,
         (LogMessageFlags.NOTIFICATION, LogMessageFlags.SILENCE),
         (PARAM_ITEMS.PERSON_PIN,),
     )
 
     ACTION_WAS_DONE = EventDescription(
         'Совершено действие "{}"➜{}.\nДействие совершил: {} ({}).\nПараметры действия: {}.\nПринудительное действие: {}.',
```

### Comparing `pih-0.36.4/pih/consts/hosts.py` & `pih-0.36.5/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/names.py` & `pih-0.36.5/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/password.py` & `pih-0.36.5/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/paths.py` & `pih-0.36.5/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/polibase.py` & `pih-0.36.5/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/service.py` & `pih-0.36.5/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/service_commands.py` & `pih-0.36.5/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/service_roles.py` & `pih-0.36.5/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/consts/settings.py` & `pih-0.36.5/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/pih.py` & `pih-0.36.5/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1829,15 +1829,15 @@
                     value := (
                         self.input(index_caption)
                         if n(text_after)
                         else self.input(j((index_caption, text_after)))
                     ),
                     min_value,
                     max_value,
-                    simple=False,
+                    simple=True,
                 )
                 if e(selected_index):
                     if use_free_input:
                         return value
                     selected_index = -1
                 try:
                     selected_index = int(selected_index) - min_value
@@ -2515,14 +2515,16 @@
     def convert_to_reverse_login(login_list: FullName) -> FullName:
         return FullName(
             login_list.middle_name, login_list.first_name, login_list.last_name
         )
 
 
 class PIH:
+    
+    
     NAME: str = "pih"
     NAME_ALT: str = "пих"
 
     def __init__(
         self,
         input: InputBase | None = None,
         output: OutputBase | None = None,
```

### Comparing `pih-0.36.4/pih/rpc/__init__.py` & `pih-0.36.5/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36.5/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36.5/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/tools/__init__.py` & `pih-0.36.5/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/tools/service.py` & `pih-0.36.5/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih/widgets.py` & `pih-0.36.5/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.4/pih.egg-info/SOURCES.txt` & `pih-0.36.5/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

