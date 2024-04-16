# Comparing `tmp/DLMS_SPODES_client-0.7.7.tar.gz` & `tmp/DLMS_SPODES_client-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.7.7.tar", last modified: Mon Apr 15 08:14:36 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.7.8.tar", last modified: Mon Apr 15 10:21:13 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.7.7.tar` & `DLMS_SPODES_client-0.7.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.999681 DLMS_SPODES_client-0.7.7/
--rw-rw-rw-   0        0        0      526 2024-04-15 08:14:35.998679 DLMS_SPODES_client-0.7.7/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.7/README.md
--rw-rw-rw-   0        0        0      836 2024-04-15 08:12:48.000000 DLMS_SPODES_client-0.7.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 08:14:35.999681 DLMS_SPODES_client-0.7.7/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.850680 DLMS_SPODES_client-0.7.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.868678 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   113785 2024-04-12 08:17:20.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/client.py
--rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.839679 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.888710 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.933678 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.987711 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.989683 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5599 2024-04-11 08:53:09.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3956 2024-04-15 08:14:25.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    43047 2024-04-12 09:08:36.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.883683 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-15 08:14:35.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2024-04-15 08:14:35.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:14:35.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-15 08:14:35.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-15 08:14:35.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-15 08:14:35.000000 DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:35.996678 DLMS_SPODES_client-0.7.7/test/
--rw-rw-rw-   0        0        0     8082 2024-04-12 09:11:11.000000 DLMS_SPODES_client-0.7.7/test/test_Client.py
--rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.7.7/test/test_services.py
--rw-rw-rw-   0        0        0      215 2024-04-15 07:27:27.000000 DLMS_SPODES_client-0.7.7/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.675357 DLMS_SPODES_client-0.7.8/
+-rw-rw-rw-   0        0        0      526 2024-04-15 10:21:13.674356 DLMS_SPODES_client-0.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.8/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-15 08:50:52.000000 DLMS_SPODES_client-0.7.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:21:13.675357 DLMS_SPODES_client-0.7.8/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.514389 DLMS_SPODES_client-0.7.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.534357 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   113785 2024-04-12 08:17:20.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/client.py
+-rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.466535 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.553358 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.602392 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.663358 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.665359 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5599 2024-04-11 08:53:09.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    43047 2024-04-12 09:08:36.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.548390 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-15 10:21:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2024-04-15 10:21:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:21:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-15 10:21:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-15 10:21:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:21:13.000000 DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:21:13.671357 DLMS_SPODES_client-0.7.8/test/
+-rw-rw-rw-   0        0        0     8082 2024-04-12 09:11:11.000000 DLMS_SPODES_client-0.7.8/test/test_Client.py
+-rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.7.8/test/test_services.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.7.8/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.7.7/PKG-INFO` & `DLMS_SPODES_client-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.7.7
+Version: 0.7.8
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.7/pyproject.toml` & `DLMS_SPODES_client-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.7.7"
+version = "0.7.8"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS-SPODES == 0.69.5",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
```

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/client.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/servers.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/services.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .client import Client, AsyncNetwork
 import csv
 from itertools import count
+from DLMS_SPODES.config_parser import get_values
 
 
-PASS_VARIANT = 'pass', 'secret'
-IP_VARIANT = 'ip', 'addr'
-NAME_VARIANT = 'пу', 'имя'
-PORT_VARIANT = 'port',
-MECHANISM_ID = 'm_id', 'mechanism_id'
-SAP = "sap",
-DA = "da",
+_h: dict[str, [str]] = {val: [val] for val in ("secret", "ip", "name", "port", "m_id", "sap", "da", "timeout")}
+"""header names"""
+if _par_variants := get_values("DLMSClient", "from_csv", "header_names"):
+    for name, variable in _par_variants.items():
+        if name in _h:
+            _h[name].extend(variable)
 
 
 class IpAddress:
     __value: list[int]
 
     def __init__(self, value: str = '127.0.0.1'):
         self.__value = list()
@@ -53,41 +53,32 @@
             # header is absence
             raise ValueError('Не найден заголовок таблицы')
         else:  # header is exist
             # search column by name
             column_name_count = count()
             field_names: list[str] = list()
             for index, cell in enumerate(first_row):
-                if any(map(cell.lower().startswith, PASS_VARIANT)):
-                    field_names.append('secret')
-                elif any(map(cell.lower().startswith, IP_VARIANT)):
-                    field_names.append('ip')
-                elif any(map(cell.lower().startswith, NAME_VARIANT)):
-                    field_names.append('name')
-                elif any(map(cell.lower().startswith, MECHANISM_ID)):
-                    field_names.append('m_id')
-                elif any(map(cell.lower().startswith, SAP)):
-                    field_names.append('sap')
-                elif any(map(cell.lower().startswith, DA)):
-                    field_names.append('da')
-                elif any(map(cell.lower().startswith, PORT_VARIANT)):
-                    field_names.append('port')
+                for column in _h:
+                    if any(map(cell.lower().startswith, _h[column])):
+                        field_names.append(_h[column][0])
+                        break
                 else:
                     field_names.append(F'unknown{next(column_name_count)}')
             if all(map(lambda name: name in field_names, ('ip',))):
                 csv_file.seek(0)
                 reader = csv.DictReader(csv_file, fieldnames=field_names, dialect=dialect)
                 next(reader)
                 res: list[Client] = list()
                 for i in reader:
                     if IpAddress.is_valid(i['ip']):
                         res.append(c := Client(
                             media=AsyncNetwork(
                                 host=i.get("ip", "127.0.0.1"),
-                                port=8888),
+                                port=8888,
+                                inactivity_timeout=i.get("timeout", 120)),
                         ))
                         c.secret = bytes(i.get('secret', '0000000000000000'), 'utf-8')
                         if m_id := i.get('m_id'):
                             c.m_id.set(m_id)
                         if port := i.get('port'):
                             c.media.port = port
                         if sap := i.get('sap'):
```

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client/task.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.7.7
+Version: 0.7.8
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.7.8/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.7/test/test_Client.py` & `DLMS_SPODES_client-0.7.8/test/test_Client.py`

 * *Files identical despite different names*
