# Comparing `tmp/dimples-0.5.2.tar.gz` & `tmp/dimples-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.5.2.tar", last modified: Thu Apr 11 16:35:26 2024, max compression
+gzip compressed data, was "dist/dimples-0.5.3.tar", last modified: Tue Apr 16 07:18:12 2024, max compression
```

## Comparing `dimples-0.5.2.tar` & `dimples-0.5.3.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-11 16:35:26.000000 dimples-0.5.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.2/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.2/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.2/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.2/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2023-12-05 04:21:35.000000 dimples-0.5.2/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.2/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.2/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.2/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.2/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.2/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.2/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.2/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.2/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.2/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.2/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.2/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.2/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.2/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.2/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.2/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6632 2024-03-07 09:27:13.000000 dimples-0.5.2/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8578 2024-03-07 09:39:13.000000 dimples-0.5.2/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.2/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.2/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.2/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5494 2024-03-06 17:56:47.000000 dimples-0.5.2/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.2/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.2/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.2/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.2/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.2/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.2/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.2/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.2/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.2/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.2/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.2/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.2/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.2/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.5.2/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.2/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8856 2024-04-11 16:17:08.000000 dimples-0.5.2/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8480 2023-12-24 14:13:19.000000 dimples-0.5.2/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.2/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.2/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.2/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.2/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.2/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.2/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.2/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.2/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.2/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4531 2023-10-13 16:11:34.000000 dimples-0.5.2/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.2/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.2/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    11821 2024-03-13 10:54:50.000000 dimples-0.5.2/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.2/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.2/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.2/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6444 2023-11-08 09:04:27.000000 dimples-0.5.2/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.2/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     3819 2023-09-05 04:47:59.000000 dimples-0.5.2/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.2/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.2/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.2/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.2/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.2/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.2/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.2/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.2/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.2/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.2/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.2/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.2/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.2/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.2/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.2/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.2/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.2/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.2/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.2/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.2/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.2/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.2/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.2/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.2/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.2/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.2/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.2/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    14571 2024-03-02 09:28:05.000000 dimples-0.5.2/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.2/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.2/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.2/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.2/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.2/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.2/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12182 2024-04-11 16:01:09.000000 dimples-0.5.2/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.2/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.2/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.2/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.2/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.2/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.2/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.2/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.2/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7346 2024-02-18 04:20:32.000000 dimples-0.5.2/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.2/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.2/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.2/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.2/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.2/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.2/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13467 2024-03-01 07:38:11.000000 dimples-0.5.2/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4454 2024-02-17 18:19:10.000000 dimples-0.5.2/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6283 2023-12-24 14:13:42.000000 dimples-0.5.2/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    15634 2024-04-11 16:20:34.000000 dimples-0.5.2/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5502 2024-03-01 07:47:10.000000 dimples-0.5.2/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     9843 2024-03-13 14:34:33.000000 dimples-0.5.2/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.2/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.2/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3832 2023-12-05 08:43:48.000000 dimples-0.5.2/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.2/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.2/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     4692 2023-12-23 05:16:03.000000 dimples-0.5.2/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6324 2024-03-03 09:21:57.000000 dimples-0.5.2/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-29 14:16:57.000000 dimples-0.5.2/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.2/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.2/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-11 16:35:26.000000 dimples-0.5.2/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-11 16:35:26.000000 dimples-0.5.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-11 16:04:01.000000 dimples-0.5.2/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-16 07:18:12.000000 dimples-0.5.3/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.3/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.3/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.3/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.3/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2023-12-05 04:21:35.000000 dimples-0.5.3/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.3/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.3/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.3/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.3/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.3/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.3/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.3/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.3/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.3/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.3/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.3/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.3/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.3/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.3/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.3/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6632 2024-03-07 09:27:13.000000 dimples-0.5.3/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8578 2024-03-07 09:39:13.000000 dimples-0.5.3/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.3/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.3/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.3/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5494 2024-03-06 17:56:47.000000 dimples-0.5.3/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.3/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.3/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.3/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.3/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.3/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.3/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.3/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.3/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.3/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.3/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.3/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.3/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.3/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.5.3/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.3/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8860 2024-04-16 06:12:16.000000 dimples-0.5.3/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8480 2024-04-16 06:08:27.000000 dimples-0.5.3/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.3/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.3/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.3/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.3/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.3/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.3/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.3/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.3/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.3/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4531 2023-10-13 16:11:34.000000 dimples-0.5.3/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.3/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.3/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    11821 2024-03-13 10:54:50.000000 dimples-0.5.3/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.3/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.3/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.3/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6444 2023-11-08 09:04:27.000000 dimples-0.5.3/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.3/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     3819 2023-09-05 04:47:59.000000 dimples-0.5.3/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.3/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.3/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.3/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.3/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.3/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.3/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.3/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.3/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.3/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.3/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.3/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.3/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.3/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.3/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.3/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.3/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.3/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.3/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.3/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.3/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.3/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.3/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.3/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.3/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.3/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.3/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.3/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    14571 2024-03-02 09:28:05.000000 dimples-0.5.3/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.3/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.3/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.3/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.3/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.3/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.3/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12170 2024-04-16 07:10:33.000000 dimples-0.5.3/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.3/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.3/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.3/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.3/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.3/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.3/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.3/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.3/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7346 2024-02-18 04:20:32.000000 dimples-0.5.3/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.3/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.3/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.3/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.3/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.3/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.3/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13467 2024-03-01 07:38:11.000000 dimples-0.5.3/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4454 2024-02-17 18:19:10.000000 dimples-0.5.3/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6548 2024-04-16 07:12:40.000000 dimples-0.5.3/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    15437 2024-04-16 06:41:33.000000 dimples-0.5.3/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5502 2024-03-01 07:47:10.000000 dimples-0.5.3/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     9843 2024-03-13 14:34:33.000000 dimples-0.5.3/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.3/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.3/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3832 2023-12-05 08:43:48.000000 dimples-0.5.3/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.3/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.3/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4692 2023-12-23 05:16:03.000000 dimples-0.5.3/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6324 2024-03-03 09:21:57.000000 dimples-0.5.3/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-29 14:16:57.000000 dimples-0.5.3/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.3/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-16 07:18:12.000000 dimples-0.5.3/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-16 07:09:58.000000 dimples-0.5.3/setup.py
```

### Comparing `dimples-0.5.2/PKG-INFO` & `dimples-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.2
+Version: 0.5.3
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.2/README.md` & `dimples-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/__init__.py` & `dimples-0.5.3/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/__init__.py` & `dimples-0.5.3/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/archivist.py` & `dimples-0.5.3/dimples/client/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/checkpoint.py` & `dimples-0.5.3/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/__init__.py` & `dimples-0.5.3/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/commands.py` & `dimples-0.5.3/dimples/client/cpu/commands.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/creator.py` & `dimples-0.5.3/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/group.py` & `dimples-0.5.3/dimples/client/cpu/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_expel.py` & `dimples-0.5.3/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_invite.py` & `dimples-0.5.3/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_join.py` & `dimples-0.5.3/dimples/client/cpu/grp_join.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_query.py` & `dimples-0.5.3/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_quit.py` & `dimples-0.5.3/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_reset.py` & `dimples-0.5.3/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/grp_resign.py` & `dimples-0.5.3/dimples/client/cpu/grp_resign.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/cpu/handshake.py` & `dimples-0.5.3/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/facebook.py` & `dimples-0.5.3/dimples/client/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/messenger.py` & `dimples-0.5.3/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/network/__init__.py` & `dimples-0.5.3/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/network/session.py` & `dimples-0.5.3/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/network/state.py` & `dimples-0.5.3/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/network/transition.py` & `dimples-0.5.3/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/packer.py` & `dimples-0.5.3/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/processor.py` & `dimples-0.5.3/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/client/terminal.py` & `dimples-0.5.3/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/__init__.py` & `dimples-0.5.3/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/anonymous.py` & `dimples-0.5.3/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/ans.py` & `dimples-0.5.3/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/archivist.py` & `dimples-0.5.3/dimples/common/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/compat/__init__.py` & `dimples-0.5.3/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/compat/btc.py` & `dimples-0.5.3/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/compat/compatible.py` & `dimples-0.5.3/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/compat/entity.py` & `dimples-0.5.3/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/compat/meta.py` & `dimples-0.5.3/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/compat/network.py` & `dimples-0.5.3/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/dbi/__init__.py` & `dimples-0.5.3/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/dbi/account.py` & `dimples-0.5.3/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/dbi/message.py` & `dimples-0.5.3/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/dbi/session.py` & `dimples-0.5.3/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/facebook.py` & `dimples-0.5.3/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/messenger.py` & `dimples-0.5.3/dimples/common/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from abc import ABC, abstractmethod
 from typing import Optional, Union, Tuple
 
 from dimsdk import SymmetricKey
 from dimsdk import ID
 from dimsdk import Content, Envelope
-from dimsdk import Command
+from dimsdk import Command, DocumentCommand
 from dimsdk import InstantMessage, SecureMessage, ReliableMessage
 from dimsdk import EntityDelegate, CipherKeyDelegate
 from dimsdk import Messenger, Packer, Processor
 
 from ..utils import Logging, Converter
 
 from .dbi import MessageDBI
@@ -166,17 +166,17 @@
         env = Envelope.create(sender=sender, receiver=receiver)
         i_msg = InstantMessage.create(head=env, body=content)
         r_msg = self.send_instant_message(msg=i_msg, priority=priority)
         return i_msg, r_msg
 
     # private
     def _attach_visa_time(self, sender: ID, msg: InstantMessage) -> bool:
-        if isinstance(msg.content, Command):
+        if isinstance(msg.content, DocumentCommand):
             # no need to attach times for command
-            return False
+            return True
         doc = self.facebook.visa(identifier=sender)
         if doc is None:
             self.error(msg='failed to get visa document for sender: %s' % sender)
             return False
         # attach sender document time
         last_doc_time = doc.time
         if last_doc_time is None:
@@ -196,16 +196,16 @@
             # return None
         else:
             self.debug(msg='send instant message message (type=%d): %s => %s, %s'
                            % (msg.content.type, sender, msg.receiver, msg.group))
             # attach sender's document times
             # for the receiver to check whether user info synchronized
             ok = self._attach_visa_time(sender=sender, msg=msg)
-            assert ok or isinstance(msg.content, Command), \
-                'failed to attach document time: %s => %s' % (sender, msg.content)
+            if not ok:
+                self.warning(msg='failed to attach document time: %s => %s' % (sender, msg.content))
         #
         #  1. encrypt message
         #
         s_msg = self.encrypt_message(msg=msg)
         if s_msg is None:
             # public key not found?
             return None
```

### Comparing `dimples-0.5.2/dimples/common/packer.py` & `dimples-0.5.3/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/processer.py` & `dimples-0.5.3/dimples/common/processer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/__init__.py` & `dimples-0.5.3/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/ans.py` & `dimples-0.5.3/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/block.py` & `dimples-0.5.3/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/handshake.py` & `dimples-0.5.3/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/login.py` & `dimples-0.5.3/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/mute.py` & `dimples-0.5.3/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/protocol/report.py` & `dimples-0.5.3/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/register.py` & `dimples-0.5.3/dimples/common/register.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/common/session.py` & `dimples-0.5.3/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/__init__.py` & `dimples-0.5.3/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/gate.py` & `dimples-0.5.3/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/gatekeeper.py` & `dimples-0.5.3/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/mars.py` & `dimples-0.5.3/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/mtp.py` & `dimples-0.5.3/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/protocol/__init__.py` & `dimples-0.5.3/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/protocol/mars.py` & `dimples-0.5.3/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/protocol/ws.py` & `dimples-0.5.3/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/queue.py` & `dimples-0.5.3/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/seeker.py` & `dimples-0.5.3/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/session.py` & `dimples-0.5.3/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/conn/ws.py` & `dimples-0.5.3/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/__init__.py` & `dimples-0.5.3/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/account.py` & `dimples-0.5.3/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/__init__.py` & `dimples-0.5.3/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/base.py` & `dimples-0.5.3/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/document.py` & `dimples-0.5.3/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/group.py` & `dimples-0.5.3/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/group_history.py` & `dimples-0.5.3/dimples/database/dos/group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/group_keys.py` & `dimples-0.5.3/dimples/database/dos/group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/login.py` & `dimples-0.5.3/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/meta.py` & `dimples-0.5.3/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/private.py` & `dimples-0.5.3/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/station.py` & `dimples-0.5.3/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/dos/user.py` & `dimples-0.5.3/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/message.py` & `dimples-0.5.3/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/session.py` & `dimples-0.5.3/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_cipherkey.py` & `dimples-0.5.3/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_document.py` & `dimples-0.5.3/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_group.py` & `dimples-0.5.3/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_group_history.py` & `dimples-0.5.3/dimples/database/t_group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_group_keys.py` & `dimples-0.5.3/dimples/database/t_group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_login.py` & `dimples-0.5.3/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_message.py` & `dimples-0.5.3/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_meta.py` & `dimples-0.5.3/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_private.py` & `dimples-0.5.3/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_station.py` & `dimples-0.5.3/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/database/t_user.py` & `dimples-0.5.3/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/edge/__init__.py` & `dimples-0.5.3/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/edge/octopus.py` & `dimples-0.5.3/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/edge/shared.py` & `dimples-0.5.3/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/edge/start.py` & `dimples-0.5.3/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/__init__.py` & `dimples-0.5.3/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/admin.py` & `dimples-0.5.3/dimples/group/admin.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/builder.py` & `dimples-0.5.3/dimples/group/builder.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/delegate.py` & `dimples-0.5.3/dimples/group/delegate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/emitter.py` & `dimples-0.5.3/dimples/group/emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def messenger(self) -> CommonMessenger:
         return self.delegate.messenger
 
     # private
     def _attach_group_times(self, group: ID, msg: InstantMessage) -> bool:
         if isinstance(msg.content, GroupCommand):
             # no need to attach times for group command
-            return False
+            return True
         facebook = self.facebook
         doc = facebook.bulletin(identifier=group)
         if doc is None:
             self.error(msg='failed to get bulletin document for group: %s' % group)
             return False
         # attach group document time
         last_doc_time = doc.time
@@ -126,15 +126,16 @@
         if group is None:
             self.error(msg='not a group message')
             return None
         assert msg.receiver == group, 'group message error: %s' % msg
         # attach group document & history times
         # for the receiver to check whether group info synchronized
         ok = self._attach_group_times(group=group, msg=msg)
-        assert ok or isinstance(msg.content, GroupCommand), 'failed to attach group times: %s => %s' % (group, content)
+        if not ok:
+            self.warning(msg='failed to attach group times: %s => %s' % (group, content))
         # TODO: if it's a file message
         #       please upload the file data first
         #       before calling this
         assert not isinstance(content, FileContent) or 'data' not in content, 'content error: %s' % content
         #
         #   1. check group bots
         #
```

### Comparing `dimples-0.5.2/dimples/group/helper.py` & `dimples-0.5.3/dimples/group/helper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/manager.py` & `dimples-0.5.3/dimples/group/manager.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/group/packer.py` & `dimples-0.5.3/dimples/group/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/register/__init__.py` & `dimples-0.5.3/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/register/base.py` & `dimples-0.5.3/dimples/register/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/register/ext.py` & `dimples-0.5.3/dimples/register/ext.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/register/run.py` & `dimples-0.5.3/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/register/shared.py` & `dimples-0.5.3/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/__init__.py` & `dimples-0.5.3/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/archivist.py` & `dimples-0.5.3/dimples/server/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/cpu/__init__.py` & `dimples-0.5.3/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/cpu/ans.py` & `dimples-0.5.3/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/cpu/document.py` & `dimples-0.5.3/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/cpu/handshake.py` & `dimples-0.5.3/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/cpu/login.py` & `dimples-0.5.3/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/cpu/report.py` & `dimples-0.5.3/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/dispatcher.py` & `dimples-0.5.3/dimples/server/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/messenger.py` & `dimples-0.5.3/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/packer.py` & `dimples-0.5.3/dimples/server/packer.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,30 +73,36 @@
         if user.type == EntityType.STATION:
             # if it's a roaming message delivered from another neighbor station,
             # shall we trust that neighbor totally and skip verifying too ???
             # TODO: trusted station list
             return True
 
     # Override
+    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+        msg = super().deserialize_message(data=data)
+        if msg is not None:
+            sender = msg.sender
+            receiver = msg.receiver
+            # check duplicated
+            if self.__is_traced(msg=msg):
+                # cycled message
+                if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
+                    # ignore cycled station message
+                    self.warning(msg='drop cycled station message: %s -> %s' % (sender, receiver))
+                    return None
+                elif receiver.is_broadcast:
+                    # ignore cycled broadcast message
+                    self.warning(msg='drop cycled broadcast message: %s -> %s' % (sender, receiver))
+                    return None
+                self.warning(msg='cycled message: %s -> %s' % (sender, receiver))
+        return msg
+
+    # Override
     def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
-        sender = msg.sender
-        receiver = msg.receiver
-        # check duplicated
-        if self.__is_traced(msg=msg):
-            # cycled message
-            if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
-                # ignore cycled station message
-                self.warning(msg='cycled station message: %s -> %s' % (sender, receiver))
-                return None
-            elif receiver.is_broadcast:
-                # ignore cycled broadcast message
-                self.warning(msg='cycled broadcast message: %s -> %s' % (sender, receiver))
-                return None
-            self.warning(msg='cycled message: %s -> %s' % (sender, receiver))
-        # check session
+        # check session ready
         if self.__is_trusted(sender=msg.sender):
             # no need to verify message from this sender
             self.debug(msg='trusted sender: %s' % msg.sender)
             return msg
         # verify after sender is OK
         return super().verify_message(msg=msg)
```

### Comparing `dimples-0.5.2/dimples/server/processor.py` & `dimples-0.5.3/dimples/server/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 from dimsdk import Envelope
 from dimsdk import Content, ContentType, Command
 from dimsdk import TextContent, ReceiptCommand
 from dimsdk import ContentProcessor, ContentProcessorCreator
 
 from dimsdk.cpu import BaseContentProcessor, BaseContentProcessorCreator
 
-from ..utils import get_msg_info
 from ..common import HandshakeCommand, LoginCommand
 from ..common import ReportCommand, AnsCommand
 from ..common import CommonFacebook, CommonMessenger
 from ..common import CommonMessagePacker
 from ..common import CommonMessageProcessor
 
 from .cpu import HandshakeCommandProcessor
@@ -161,17 +160,14 @@
             signed = messenger.sign_message(msg=res)
             if signed is not None:
                 messages.append(signed)
         return messages
         # TODO: override to deliver to the receiver when catch exception "receiver error ..."
 
     def _force_handshake(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        if self.messenger.verify_message(msg=msg) is None:
-            assert False, 'failed to verify message: %s' % get_msg_info(msg=msg)
-            # return []
         session = self.messenger.session
         sess_id = session.identifier
         current = self.facebook.current_user
         sid = current.identifier
         sender = msg.sender
         if sess_id is not None:
             assert sess_id == sender, 'sender error: %s, %s' % (sender, sess_id)
```

### Comparing `dimples-0.5.2/dimples/server/push.py` & `dimples-0.5.3/dimples/server/push.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/session.py` & `dimples-0.5.3/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/session_center.py` & `dimples-0.5.3/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/server/trace.py` & `dimples-0.5.3/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/station/__init__.py` & `dimples-0.5.3/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/station/handler.py` & `dimples-0.5.3/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/station/shared.py` & `dimples-0.5.3/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/station/start.py` & `dimples-0.5.3/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/utils/__init__.py` & `dimples-0.5.3/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/utils/cache.py` & `dimples-0.5.3/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/utils/config.py` & `dimples-0.5.3/dimples/utils/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/utils/dos.py` & `dimples-0.5.3/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/utils/log.py` & `dimples-0.5.3/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples/utils/singleton.py` & `dimples-0.5.3/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/dimples.egg-info/PKG-INFO` & `dimples-0.5.3/dimples.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.2
+Version: 0.5.3
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.2/dimples.egg-info/SOURCES.txt` & `dimples-0.5.3/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-0.5.2/setup.py` & `dimples-0.5.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

