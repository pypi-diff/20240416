# Comparing `tmp/bpkio_python_sdk-1.8.0.tar.gz` & `tmp/bpkio_python_sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_python_sdk-1.8.0.tar", max compression
+gzip compressed data, was "bpkio_python_sdk-1.9.0.tar", max compression
```

## Comparing `bpkio_python_sdk-1.8.0.tar` & `bpkio_python_sdk-1.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.8.0/README.md
--rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.8.0/bpkio_api/__init__.py
--rw-r--r--   0        0        0     6518 2023-10-31 10:18:56.705893 bpkio_python_sdk-1.8.0/bpkio_api/api.py
--rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.8.0/bpkio_api/caching.py
--rw-r--r--   0        0        0      506 2023-06-09 11:08:00.617751 bpkio_python_sdk-1.8.0/bpkio_api/consumer.py
--rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.8.0/bpkio_api/credential_provider.py
--rw-r--r--   0        0        0      178 2023-06-09 11:21:14.279980 bpkio_python_sdk-1.8.0/bpkio_api/defaults.py
--rw-r--r--   0        0        0      444 2023-10-31 10:15:29.436282 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/__init__.py
--rw-r--r--   0        0        0     4563 2023-06-09 11:03:02.185931 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/categories.py
--rw-r--r--   0        0        0      747 2023-10-31 20:54:31.990996 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/consumption.py
--rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/enums.py
--rw-r--r--   0        0        0    23864 2023-10-02 19:38:25.172620 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/services.py
--rw-r--r--   0        0        0    21784 2023-07-07 15:36:34.794515 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/sources.py
--rw-r--r--   0        0        0      673 2023-10-31 10:29:42.726038 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/support.py
--rw-r--r--   0        0        0     3036 2023-10-06 15:11:59.099783 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/tenants.py
--rw-r--r--   0        0        0     6014 2023-06-09 11:05:16.807277 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/transcoding_profiles.py
--rw-r--r--   0        0        0     2673 2023-06-09 11:05:32.498036 bpkio_python_sdk-1.8.0/bpkio_api/endpoints/users.py
--rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.8.0/bpkio_api/exceptions.py
--rw-r--r--   0        0        0     2920 2023-10-03 11:26:01.321710 bpkio_python_sdk-1.8.0/bpkio_api/helpers/codecstrings.py
--rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/__init__.py
--rw-r--r--   0        0        0     4578 2023-09-08 15:27:59.221650 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/dash.py
--rw-r--r--   0        0        0     3532 2023-10-10 10:01:16.119352 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/factory.py
--rw-r--r--   0        0        0     3060 2023-09-08 15:26:52.457406 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/generic.py
--rw-r--r--   0        0        0     4798 2023-10-17 15:26:02.257420 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/hls.py
--rw-r--r--   0        0        0      446 2023-06-09 11:39:02.452951 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/jpeg.py
--rw-r--r--   0        0        0      472 2023-06-09 11:40:16.383318 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/mp4.py
--rw-r--r--   0        0        0      434 2023-06-09 11:40:11.132158 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/png.py
--rw-r--r--   0        0        0     1976 2023-06-09 11:39:37.280020 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/vast.py
--rw-r--r--   0        0        0     2325 2023-06-09 11:39:46.049574 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/vmap.py
--rw-r--r--   0        0        0      580 2023-06-09 11:39:59.258206 bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/xml.py
--rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.8.0/bpkio_api/helpers/list.py
--rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.8.0/bpkio_api/helpers/objects.py
--rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/__init__.py
--rw-r--r--   0        0        0      540 2023-09-20 08:12:04.165050 bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/analyser.py
--rw-r--r--   0        0        0     1740 2023-10-18 08:06:25.968329 bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/dash.py
--rw-r--r--   0        0        0     4184 2023-09-25 09:07:42.265344 bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/hls.py
--rw-r--r--   0        0        0     1728 2023-06-16 10:38:47.386661 bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/profile_generator.py
--rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/__init__.py
--rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/curl.py
--rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/exporter.py
--rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/markdown.py
--rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/postman.py
--rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/session_items.py
--rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/session_recorder.py
--rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/text.py
--rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.8.0/bpkio_api/helpers/search.py
--rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.8.0/bpkio_api/helpers/source_type.py
--rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.8.0/bpkio_api/helpers/times.py
--rw-r--r--   0        0        0     2623 2023-09-13 09:12:58.107935 bpkio_python_sdk-1.8.0/bpkio_api/mappings.py
--rw-r--r--   0        0        0      103 2023-10-31 10:30:22.593469 bpkio_python_sdk-1.8.0/bpkio_api/models/BkYouSupportPackage.py
--rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.8.0/bpkio_api/models/Categories.py
--rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.8.0/bpkio_api/models/Consumption.py
--rw-r--r--   0        0        0     5803 2023-10-30 12:19:27.204290 bpkio_python_sdk-1.8.0/bpkio_api/models/Services.py
--rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.8.0/bpkio_api/models/Slots.py
--rw-r--r--   0        0        0     3384 2023-10-16 13:14:04.832412 bpkio_python_sdk-1.8.0/bpkio_api/models/Sources.py
--rw-r--r--   0        0        0      530 2023-10-06 15:00:31.426961 bpkio_python_sdk-1.8.0/bpkio_api/models/Tenants.py
--rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.8.0/bpkio_api/models/TranscodingProfiles.py
--rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.8.0/bpkio_api/models/Users.py
--rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.8.0/bpkio_api/models/__init__.py
--rw-r--r--   0        0        0      917 2023-10-17 09:12:00.328311 bpkio_python_sdk-1.8.0/bpkio_api/models/common.py
--rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.8.0/bpkio_api/models/model_graph.py
--rw-r--r--   0        0        0     2152 2023-06-09 10:37:32.988041 bpkio_python_sdk-1.8.0/bpkio_api/response_handler.py
--rw-r--r--   0        0        0     1195 2023-10-31 20:56:02.206403 bpkio_python_sdk-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.9.0/README.md
+-rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.9.0/bpkio_api/__init__.py
+-rw-r--r--   0        0        0     6518 2023-10-31 10:18:56.705893 bpkio_python_sdk-1.9.0/bpkio_api/api.py
+-rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.9.0/bpkio_api/caching.py
+-rw-r--r--   0        0        0      506 2023-06-09 11:08:00.617751 bpkio_python_sdk-1.9.0/bpkio_api/consumer.py
+-rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.9.0/bpkio_api/credential_provider.py
+-rw-r--r--   0        0        0      178 2023-06-09 11:21:14.279980 bpkio_python_sdk-1.9.0/bpkio_api/defaults.py
+-rw-r--r--   0        0        0      444 2023-10-31 10:15:29.436282 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4563 2023-06-09 11:03:02.185931 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/categories.py
+-rw-r--r--   0        0        0      747 2023-10-31 20:54:31.990996 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/consumption.py
+-rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/enums.py
+-rw-r--r--   0        0        0    23864 2023-11-02 20:49:41.023584 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/services.py
+-rw-r--r--   0        0        0    21784 2023-07-07 15:36:34.794515 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/sources.py
+-rw-r--r--   0        0        0      673 2023-10-31 10:29:42.726038 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/support.py
+-rw-r--r--   0        0        0     3036 2023-10-06 15:11:59.099783 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/tenants.py
+-rw-r--r--   0        0        0     6014 2023-06-09 11:05:16.807277 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/transcoding_profiles.py
+-rw-r--r--   0        0        0     2673 2023-06-09 11:05:32.498036 bpkio_python_sdk-1.9.0/bpkio_api/endpoints/users.py
+-rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.9.0/bpkio_api/exceptions.py
+-rw-r--r--   0        0        0     2920 2023-10-03 11:26:01.321710 bpkio_python_sdk-1.9.0/bpkio_api/helpers/codecstrings.py
+-rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/__init__.py
+-rw-r--r--   0        0        0     4578 2023-09-08 15:27:59.221650 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/dash.py
+-rw-r--r--   0        0        0     3532 2023-10-10 10:01:16.119352 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/factory.py
+-rw-r--r--   0        0        0     3060 2023-09-08 15:26:52.457406 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/generic.py
+-rw-r--r--   0        0        0     4798 2023-10-17 15:26:02.257420 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/hls.py
+-rw-r--r--   0        0        0      446 2023-06-09 11:39:02.452951 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/jpeg.py
+-rw-r--r--   0        0        0      472 2023-06-09 11:40:16.383318 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/mp4.py
+-rw-r--r--   0        0        0      434 2023-06-09 11:40:11.132158 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/png.py
+-rw-r--r--   0        0        0     1976 2023-06-09 11:39:37.280020 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/vast.py
+-rw-r--r--   0        0        0     2325 2023-06-09 11:39:46.049574 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/vmap.py
+-rw-r--r--   0        0        0      580 2023-06-09 11:39:59.258206 bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/xml.py
+-rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.9.0/bpkio_api/helpers/list.py
+-rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.9.0/bpkio_api/helpers/objects.py
+-rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/__init__.py
+-rw-r--r--   0        0        0      540 2023-09-20 08:12:04.165050 bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/analyser.py
+-rw-r--r--   0        0        0     1740 2023-10-18 08:06:25.968329 bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/dash.py
+-rw-r--r--   0        0        0     4184 2023-09-25 09:07:42.265344 bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/hls.py
+-rw-r--r--   0        0        0     1728 2023-06-16 10:38:47.386661 bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/profile_generator.py
+-rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/__init__.py
+-rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/curl.py
+-rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/exporter.py
+-rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/markdown.py
+-rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/postman.py
+-rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/session_items.py
+-rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/session_recorder.py
+-rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/text.py
+-rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.9.0/bpkio_api/helpers/search.py
+-rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.9.0/bpkio_api/helpers/source_type.py
+-rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.9.0/bpkio_api/helpers/times.py
+-rw-r--r--   0        0        0     2623 2023-09-13 09:12:58.107935 bpkio_python_sdk-1.9.0/bpkio_api/mappings.py
+-rw-r--r--   0        0        0      103 2023-10-31 10:30:22.593469 bpkio_python_sdk-1.9.0/bpkio_api/models/BkYouSupportPackage.py
+-rw-r--r--   0        0        0      431 2023-11-01 21:39:35.203219 bpkio_python_sdk-1.9.0/bpkio_api/models/Categories.py
+-rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.9.0/bpkio_api/models/Consumption.py
+-rw-r--r--   0        0        0     5803 2023-10-30 12:19:27.204290 bpkio_python_sdk-1.9.0/bpkio_api/models/Services.py
+-rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.9.0/bpkio_api/models/Slots.py
+-rw-r--r--   0        0        0     3384 2023-10-16 13:14:04.832412 bpkio_python_sdk-1.9.0/bpkio_api/models/Sources.py
+-rw-r--r--   0        0        0      530 2023-10-06 15:00:31.426961 bpkio_python_sdk-1.9.0/bpkio_api/models/Tenants.py
+-rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.9.0/bpkio_api/models/TranscodingProfiles.py
+-rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.9.0/bpkio_api/models/Users.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.9.0/bpkio_api/models/__init__.py
+-rw-r--r--   0        0        0      917 2023-10-17 09:12:00.328311 bpkio_python_sdk-1.9.0/bpkio_api/models/common.py
+-rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.9.0/bpkio_api/models/model_graph.py
+-rw-r--r--   0        0        0     2238 2023-11-01 18:35:51.420652 bpkio_python_sdk-1.9.0/bpkio_api/response_handler.py
+-rw-r--r--   0        0        0     1195 2023-11-06 18:25:04.542823 bpkio_python_sdk-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.9.0/PKG-INFO
```

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/api.py` & `bpkio_python_sdk-1.9.0/bpkio_api/api.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/caching.py` & `bpkio_python_sdk-1.9.0/bpkio_api/caching.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/credential_provider.py` & `bpkio_python_sdk-1.9.0/bpkio_api/credential_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/categories.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/consumption.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/services.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/sources.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/support.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/support.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/tenants.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/tenants.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/transcoding_profiles.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/transcoding_profiles.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/endpoints/users.py` & `bpkio_python_sdk-1.9.0/bpkio_api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/exceptions.py` & `bpkio_python_sdk-1.9.0/bpkio_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/codecstrings.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/codecstrings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/dash.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/factory.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/factory.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/generic.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/generic.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/hls.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/vast.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/vast.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/vmap.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/vmap.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/handlers/xml.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/list.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/analyser.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/analyser.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/dash.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/hls.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/profile_generator/profile_generator.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/profile_generator/profile_generator.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/curl.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/curl.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/exporter.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/exporter.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/markdown.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/markdown.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/postman.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/postman.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/session_items.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/session_items.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/session_recorder.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/recorder/text.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/recorder/text.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/search.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/source_type.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/source_type.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/helpers/times.py` & `bpkio_python_sdk-1.9.0/bpkio_api/helpers/times.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/mappings.py` & `bpkio_python_sdk-1.9.0/bpkio_api/mappings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/Services.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/Services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/Slots.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/Slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/Sources.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/Sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/Tenants.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/Tenants.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/__init__.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/common.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/common.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/models/model_graph.py` & `bpkio_python_sdk-1.9.0/bpkio_api/models/model_graph.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.8.0/bpkio_api/response_handler.py` & `bpkio_python_sdk-1.9.0/bpkio_api/response_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,18 @@
             message=response.text,
             reason=response.reason,
         )
 
     response_payload = json.loads(response.text)
 
     if response.status_code == 403:
-        if "existing" in response_payload["message"]:
+        if (
+            "existing" in response_payload["message"]
+            or "with the same" in response_payload["message"]
+        ):
             raise errors.ResourceExistsError(
                 url=response.url,
                 status_code=response.status_code,
                 message=response_payload["message"],
                 reason=response.reason,
             )
```

### Comparing `bpkio_python_sdk-1.8.0/pyproject.toml` & `bpkio_python_sdk-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-python-sdk"
-version = "1.8.0"
+version = "1.9.0"
 description = "An (opinionated) Python SDK for the broadpeak.io REST APIs"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bpkio_python_sdk-1.8.0/PKG-INFO` & `bpkio_python_sdk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-python-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: An (opinionated) Python SDK for the broadpeak.io REST APIs
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

