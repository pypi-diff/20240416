# Comparing `tmp/moler-3.4.0.tar.gz` & `tmp/moler-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moler-3.4.0.tar", last modified: Tue Apr  9 08:07:52 2024, max compression
+gzip compressed data, was "moler-3.5.0.tar", last modified: Tue Apr 16 13:13:13 2024, max compression
```

## Comparing `moler-3.4.0.tar` & `moler-3.5.0.tar`

### file list

```diff
@@ -1,344 +1,344 @@
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.611000 moler-3.4.0/
--rw-r--r--   0 ute       (1000) ute       (1000)     1505 2024-02-06 08:16:12.000000 moler-3.4.0/LICENSE
--rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-04-09 08:07:52.611000 moler-3.4.0/PKG-INFO
--rw-r--r--   0 ute       (1000) ute       (1000)    24908 2024-04-09 07:12:07.000000 moler-3.4.0/README.md
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.423000 moler-3.4.0/moler/
--rw-r--r--   0 ute       (1000) ute       (1000)      143 2024-02-06 08:16:12.000000 moler-3.4.0/moler/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10606 2024-02-19 07:54:48.000000 moler-3.4.0/moler/abstract_moler_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)    49062 2024-02-19 07:54:48.000000 moler-3.4.0/moler/asyncio_runner.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.431000 moler-3.4.0/moler/cmd/
--rw-r--r--   0 ute       (1000) ute       (1000)     4140 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.431000 moler-3.4.0/moler/cmd/adb/
--rw-r--r--   0 ute       (1000) ute       (1000)      191 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/adb/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5686 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/adb/adb_shell.py
--rw-r--r--   0 ute       (1000) ute       (1000)      331 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/adb/generic_adb_command.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.467000 moler-3.4.0/moler/cmd/at/
--rw-r--r--   0 ute       (1000) ute       (1000)      369 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1588 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/at.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1553 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/attach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1826 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/create_pdu_session.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3604 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/cu.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1526 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/detach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1878 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/enable_echo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2808 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/exit_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3786 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/genericat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5005 2024-02-06 14:47:26.000000 moler-3.4.0/moler/cmd/at/get_apns.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3062 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_attach_state.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4770 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_cell_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9134 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_cell_id_gprs.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8605 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_cell_id_lte.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6797 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_cell_id_nr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2792 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_functionality_level.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5945 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/get_imei.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2654 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_imsi.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3226 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/get_ip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_manufacturer_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5128 2024-02-06 14:47:26.000000 moler-3.4.0/moler/cmd/at/get_product_info.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3294 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/get_revision_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3555 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/plink_serial.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2361 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/quectel_lock_nr_earfcn.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/quectel_network_preferences.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1828 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/at/release_pdu_session.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4632 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/run_script.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2570 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_apn.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2454 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_cell_id.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3066 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_cell_id_gprs.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3056 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_cell_id_lte.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2741 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_cell_id_nr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3367 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_functionality_level.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2231 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/at/set_mode.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11527 2024-03-27 09:23:44.000000 moler-3.4.0/moler/cmd/commandchangingprompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)    28640 2024-03-27 09:23:44.000000 moler-3.4.0/moler/cmd/commandtextualgeneric.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.471000 moler-3.4.0/moler/cmd/juniper/
--rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.471000 moler-3.4.0/moler/cmd/juniper/cli/
--rw-r--r--   0 ute       (1000) ute       (1000)      199 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper/cli/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2571 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper/cli/configure.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.479000 moler-3.4.0/moler/cmd/juniper/configure/
--rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper/configure/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2616 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper/configure/exit_configure.py
--rw-r--r--   0 ute       (1000) ute       (1000)      993 2024-02-06 14:47:26.000000 moler-3.4.0/moler/cmd/juniper/genericjuniper.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.479000 moler-3.4.0/moler/cmd/juniper_ex/
--rw-r--r--   0 ute       (1000) ute       (1000)      197 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper_ex/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.479000 moler-3.4.0/moler/cmd/juniper_ex/cli/
--rw-r--r--   0 ute       (1000) ute       (1000)      201 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper_ex/cli/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.479000 moler-3.4.0/moler/cmd/juniper_ex/configure/
--rw-r--r--   0 ute       (1000) ute       (1000)      207 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/juniper_ex/configure/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      404 2024-02-06 14:47:26.000000 moler-3.4.0/moler/cmd/juniper_ex/genericjuniperex.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.479000 moler-3.4.0/moler/cmd/pdu_aten/
--rw-r--r--   0 ute       (1000) ute       (1000)      192 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/pdu_aten/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      904 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/pdu_aten/generic_pdu_aten.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.483000 moler-3.4.0/moler/cmd/pdu_aten/pdu/
--rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1193 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/generic_pdu.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/quit.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2895 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/read_meter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2948 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/read_status.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1870 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/pdu_aten/pdu/sw.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.487000 moler-3.4.0/moler/cmd/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      370 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/scpi/genricscpi.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.491000 moler-3.4.0/moler/cmd/scpi/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      202 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/scpi/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/scpi/scpi/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)      969 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/scpi/scpi/genericscpistate.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1378 2024-02-06 14:47:26.000000 moler-3.4.0/moler/cmd/scpi/scpi/idn.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1598 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/scpi/scpi/read.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1921 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/scpi/scpi/run_command.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.579000 moler-3.4.0/moler/cmd/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)      194 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4744 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/adb_devices.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1957 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/adb_forward.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1465 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/adb_root.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1201 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/bash.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/cat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3342 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/cd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2004 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/chgrp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2158 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/chmod.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2507 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/chown.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1650 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/cp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2807 2024-03-11 13:43:51.000000 moler-3.4.0/moler/cmd/unix/ctrl_c.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-03-11 13:46:32.000000 moler-3.4.0/moler/cmd/unix/ctrl_z.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3554 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/cut.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5302 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/date.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3635 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/devmem.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6395 2024-02-06 14:47:26.000000 moler-3.4.0/moler/cmd/unix/df.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4384 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/dmesg.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4325 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/du.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4189 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/echo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1077 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/enter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/env.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10518 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ethtool.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1799 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/exit.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3769 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/exit_telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6520 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/export.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8513 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/find.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12697 2024-04-09 06:59:25.000000 moler-3.4.0/moler/cmd/unix/generictelnetssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5773 2024-03-11 12:51:33.000000 moler-3.4.0/moler/cmd/unix/genericunix.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9240 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/grep.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6109 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/gunzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4691 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/gzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7087 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/hciconfig.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4606 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/head.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4428 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/hexdump.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2527 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/history.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1417 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/hostname.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4940 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/id.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20386 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ifconfig.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6319 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ip_addr.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6423 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ip_link.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6554 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ip_neigh.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19050 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ip_route.py
--rw-r--r--   0 ute       (1000) ute       (1000)    40999 2024-03-01 08:45:11.000000 moler-3.4.0/moler/cmd/unix/iperf.py
--rw-r--r--   0 ute       (1000) ute       (1000)    96255 2024-03-01 08:01:14.000000 moler-3.4.0/moler/cmd/unix/iperf2.py
--rw-r--r--   0 ute       (1000) ute       (1000)   184933 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/iperf3.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17415 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ipsec.py
--rw-r--r--   0 ute       (1000) ute       (1000)    60585 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/iptables.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2096 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/kill.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2642 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/killall.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1545 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ln.py
--rw-r--r--   0 ute       (1000) ute       (1000)      432 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/logout.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17144 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ls.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8656 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/lsof.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6008 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/lxc_attach.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7348 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/lxc_info.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19755 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/lxc_ls.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1677 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/md5sum.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1854 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/mkdir.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5082 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/mount.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5753 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/mpstat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1986 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/mv.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20213 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/netstat.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7517 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/nft.py
--rw-r--r--   0 ute       (1000) ute       (1000)    39366 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/nmap.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12330 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/nping.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5168 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ntpq.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3907 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/openssl_s_client.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8259 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/openssl_x509_text_in.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9153 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/passwd.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17005 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ping.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1352 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/pkill.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ps.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2609 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/pwd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3048 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/reboot.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1706 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/rm.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7861 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/route.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4494 2024-03-18 09:44:23.000000 moler-3.4.0/moler/cmd/unix/run_script.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3743 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/run_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12696 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/scp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4191 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/sed.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8652 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/service.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10793 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/sftp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4883 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/shasum.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6854 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/socat.py
--rw-r--r--   0 ute       (1000) ute       (1000)    13026 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/ss.py
--rw-r--r--   0 ute       (1000) ute       (1000)    45078 2024-03-27 09:23:44.000000 moler-3.4.0/moler/cmd/unix/ssh.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4910 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/sshkeygen.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7129 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/su.py
--rw-r--r--   0 ute       (1000) ute       (1000)    21553 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/sudo.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1139 2024-02-06 08:16:12.000000 moler-3.4.0/moler/cmd/unix/sync.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3488 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/sysctl.py
--rw-r--r--   0 ute       (1000) ute       (1000)    16285 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/systemctl.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2509 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/tail.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5810 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/tail_latest_file.py
--rw-r--r--   0 ute       (1000) ute       (1000)      927 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/tar.py
--rw-r--r--   0 ute       (1000) ute       (1000)    25812 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/tcpdump.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3071 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/tee.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19408 2024-03-27 09:23:44.000000 moler-3.4.0/moler/cmd/unix/telnet.py
--rw-r--r--   0 ute       (1000) ute       (1000)    17342 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/top.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1686 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/touch.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7982 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/traceroute.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10992 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/tshark.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2890 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/uname.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1788 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/unxz.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10632 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/unzip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7243 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/uptime.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2946 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/useradd.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3577 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/userdel.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9935 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/w.py
--rw-r--r--   0 ute       (1000) ute       (1000)    40990 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/wget.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/which.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1215 2024-02-15 14:32:06.000000 moler-3.4.0/moler/cmd/unix/whoami.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1907 2024-02-19 07:54:48.000000 moler-3.4.0/moler/cmd/unix/zip.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2785 2024-02-19 07:54:48.000000 moler-3.4.0/moler/command.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9032 2024-02-19 07:54:48.000000 moler-3.4.0/moler/command_scheduler.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.583000 moler-3.4.0/moler/config/
--rw-r--r--   0 ute       (1000) ute       (1000)    12409 2024-03-06 09:25:24.000000 moler-3.4.0/moler/config/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11652 2024-02-19 07:54:48.000000 moler-3.4.0/moler/config/connections.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1534 2024-02-06 14:47:26.000000 moler-3.4.0/moler/config/devices.py
--rw-r--r--   0 ute       (1000) ute       (1000)    34368 2024-03-06 09:25:24.000000 moler-3.4.0/moler/config/loggers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-02-06 14:47:26.000000 moler-3.4.0/moler/config/runners.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1594 2024-02-06 08:16:12.000000 moler-3.4.0/moler/connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8517 2024-02-19 07:54:48.000000 moler-3.4.0/moler/connection_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    21922 2024-03-11 12:51:33.000000 moler-3.4.0/moler/connection_observer.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.587000 moler-3.4.0/moler/device/
--rw-r--r--   0 ute       (1000) ute       (1000)      425 2024-02-06 08:16:12.000000 moler-3.4.0/moler/device/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7194 2024-02-06 14:47:26.000000 moler-3.4.0/moler/device/abstract_device.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15911 2024-02-19 07:54:48.000000 moler-3.4.0/moler/device/adbremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    22324 2024-02-19 07:54:48.000000 moler-3.4.0/moler/device/adbremote2.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10517 2024-02-19 07:54:48.000000 moler-3.4.0/moler/device/atremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20904 2024-02-19 07:54:48.000000 moler-3.4.0/moler/device/device.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1581 2024-02-06 14:47:26.000000 moler-3.4.0/moler/device/juniper_ex.py
--rw-r--r--   0 ute       (1000) ute       (1000)    14312 2024-02-06 08:16:12.000000 moler-3.4.0/moler/device/junipergeneric.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12221 2024-02-06 08:16:12.000000 moler-3.4.0/moler/device/pdu_aten.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10797 2024-02-06 08:16:12.000000 moler-3.4.0/moler/device/proxy_pc.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20242 2024-02-19 07:54:48.000000 moler-3.4.0/moler/device/proxy_pc2.py
--rw-r--r--   0 ute       (1000) ute       (1000)    11861 2024-02-06 08:16:12.000000 moler-3.4.0/moler/device/scpi.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2339 2024-04-09 06:59:25.000000 moler-3.4.0/moler/device/state_machine.py
--rw-r--r--   0 ute       (1000) ute       (1000)    46259 2024-03-13 10:03:30.000000 moler-3.4.0/moler/device/textualdevice.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9625 2024-02-06 14:47:26.000000 moler-3.4.0/moler/device/unixlocal.py
--rw-r--r--   0 ute       (1000) ute       (1000)    19608 2024-02-06 08:16:12.000000 moler-3.4.0/moler/device/unixremote.py
--rw-r--r--   0 ute       (1000) ute       (1000)    25856 2024-02-19 07:54:48.000000 moler-3.4.0/moler/device/unixremote2.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5292 2024-02-19 07:54:48.000000 moler-3.4.0/moler/event.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5037 2024-03-06 09:25:24.000000 moler-3.4.0/moler/event_awaiter.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.591000 moler-3.4.0/moler/events/
--rw-r--r--   0 ute       (1000) ute       (1000)      134 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.591000 moler-3.4.0/moler/events/juniper/
--rw-r--r--   0 ute       (1000) ute       (1000)      193 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/juniper/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      898 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/juniper/genericshared_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      324 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/juniper/genericshared_textualevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.591000 moler-3.4.0/moler/events/juniper_ex/
--rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/juniper_ex/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      903 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      336 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/juniper_ex/genericjuniper_ex_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7401 2024-02-19 07:54:48.000000 moler-3.4.0/moler/events/lineevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.595000 moler-3.4.0/moler/events/pdu_aten/
--rw-r--r--   0 ute       (1000) ute       (1000)      190 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/pdu_aten/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.595000 moler-3.4.0/moler/events/scpi/
--rw-r--r--   0 ute       (1000) ute       (1000)      186 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/scpi/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)      892 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/scpi/genericscpi_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      325 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/scpi/genericscpi_textualevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.595000 moler-3.4.0/moler/events/shared/
--rw-r--r--   0 ute       (1000) ute       (1000)      180 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/shared/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1241 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/shared/genericshared_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      673 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/shared/genericshared_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2227 2024-02-06 14:47:26.000000 moler-3.4.0/moler/events/shared/password_prompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5516 2024-02-06 14:47:26.000000 moler-3.4.0/moler/events/shared/wait4.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5819 2024-02-19 07:54:48.000000 moler-3.4.0/moler/events/textualevent.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.603000 moler-3.4.0/moler/events/unix/
--rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2185 2024-02-06 14:47:26.000000 moler-3.4.0/moler/events/unix/advise_to_change_your_password.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2236 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/failed_login_counter.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1243 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/genericunix_lineevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      675 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/genericunix_textualevent.py
--rw-r--r--   0 ute       (1000) ute       (1000)      997 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/last_failed_login.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2968 2024-02-19 07:54:48.000000 moler-3.4.0/moler/events/unix/last_login.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4734 2024-02-06 14:47:26.000000 moler-3.4.0/moler/events/unix/ping_no_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2302 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/ping_response.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3599 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/private_system.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1317 2024-02-06 14:47:26.000000 moler-3.4.0/moler/events/unix/shutdown.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4639 2024-02-06 14:47:26.000000 moler-3.4.0/moler/events/unix/u_boot_crtm.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1463 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/wait4prompt.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4289 2024-02-19 07:54:48.000000 moler-3.4.0/moler/events/unix/wait4prompts.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1756 2024-02-06 08:16:12.000000 moler-3.4.0/moler/events/unix/warning_default_password.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5760 2024-02-19 07:54:48.000000 moler-3.4.0/moler/exceptions.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18197 2024-02-19 07:54:48.000000 moler-3.4.0/moler/helpers.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3176 2024-02-19 07:54:48.000000 moler-3.4.0/moler/instance_loader.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.603000 moler-3.4.0/moler/io/
--rw-r--r--   0 ute       (1000) ute       (1000)      499 2024-02-06 08:16:12.000000 moler-3.4.0/moler/io/__init__.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.603000 moler-3.4.0/moler/io/asyncio/
--rw-r--r--   0 ute       (1000) ute       (1000)      536 2024-02-06 14:47:26.000000 moler-3.4.0/moler/io/asyncio/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5954 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/asyncio/tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)    14931 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/asyncio/terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7222 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/io_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2156 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/io_exceptions.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.603000 moler-3.4.0/moler/io/raw/
--rw-r--r--   0 ute       (1000) ute       (1000)     1320 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/raw/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9652 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/raw/memory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    22609 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/raw/sshshell.py
--rw-r--r--   0 ute       (1000) ute       (1000)      741 2024-02-06 14:47:26.000000 moler-3.4.0/moler/io/raw/subprocess.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7554 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/raw/tcp.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9922 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/raw/tcpserverpiped.py
--rw-r--r--   0 ute       (1000) ute       (1000)     7325 2024-02-19 07:54:48.000000 moler-3.4.0/moler/io/raw/terminal.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5679 2024-02-06 14:47:26.000000 moler-3.4.0/moler/moler_connection_for_single_thread_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1672 2024-02-06 08:16:12.000000 moler-3.4.0/moler/observable_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4597 2024-02-19 07:54:48.000000 moler-3.4.0/moler/observer_thread_wrapper.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.603000 moler-3.4.0/moler/parser/
--rw-r--r--   0 ute       (1000) ute       (1000)      141 2024-02-06 08:16:12.000000 moler-3.4.0/moler/parser/__init__.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18614 2024-02-19 07:54:48.000000 moler-3.4.0/moler/parser/table_text.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5503 2024-02-06 14:47:26.000000 moler-3.4.0/moler/publisher.py
--rw-r--r--   0 ute       (1000) ute       (1000)    37230 2024-03-06 09:47:05.000000 moler-3.4.0/moler/runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3910 2024-02-19 07:54:48.000000 moler-3.4.0/moler/runner_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20412 2024-02-19 07:54:48.000000 moler-3.4.0/moler/runner_single_thread.py
--rw-r--r--   0 ute       (1000) ute       (1000)     6790 2024-02-19 07:54:48.000000 moler-3.4.0/moler/scheduler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8824 2024-02-19 07:54:48.000000 moler-3.4.0/moler/threaded_moler_connection.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.607000 moler-3.4.0/moler/util/
--rw-r--r--   0 ute       (1000) ute       (1000)      138 2024-02-06 08:16:12.000000 moler-3.4.0/moler/util/__init__.py
--rwxr-xr-x   0 ute       (1000) ute       (1000)    13210 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/cmds_events_doc.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2581 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/compressed_rotating_file_handler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1405 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/compressed_timed_rotating_file_handler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1255 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3436 2024-02-14 14:53:24.000000 moler-3.4.0/moler/util/connection_observer_life_status.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4520 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/converterhelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)    12576 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/devices_SM.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2987 2024-02-06 14:47:26.000000 moler-3.4.0/moler/util/loghelper.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9386 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/moler_serial_proxy.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10028 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/moler_test.py
--rw-r--r--   0 ute       (1000) ute       (1000)     1973 2024-02-19 07:54:48.000000 moler-3.4.0/moler/util/tracked_thread.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.611000 moler-3.4.0/moler.egg-info/
--rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-04-09 08:07:52.000000 moler-3.4.0/moler.egg-info/PKG-INFO
--rw-r--r--   0 ute       (1000) ute       (1000)     8786 2024-04-09 08:07:52.000000 moler-3.4.0/moler.egg-info/SOURCES.txt
--rw-r--r--   0 ute       (1000) ute       (1000)        1 2024-04-09 08:07:52.000000 moler-3.4.0/moler.egg-info/dependency_links.txt
--rw-r--r--   0 ute       (1000) ute       (1000)      157 2024-04-09 08:07:52.000000 moler-3.4.0/moler.egg-info/requires.txt
--rw-r--r--   0 ute       (1000) ute       (1000)        6 2024-04-09 08:07:52.000000 moler-3.4.0/moler.egg-info/top_level.txt
--rw-r--r--   0 ute       (1000) ute       (1000)      165 2024-04-09 08:07:52.611000 moler-3.4.0/setup.cfg
--rw-r--r--   0 ute       (1000) ute       (1000)     1932 2024-04-09 07:12:07.000000 moler-3.4.0/setup.py
-drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-09 08:07:52.611000 moler-3.4.0/test/
--rw-r--r--   0 ute       (1000) ute       (1000)    10233 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_cmds_events_doc.py
--rw-r--r--   0 ute       (1000) ute       (1000)    10694 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_command.py
--rw-r--r--   0 ute       (1000) ute       (1000)    20821 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_connection.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8679 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_connection_configuration.py
--rw-r--r--   0 ute       (1000) ute       (1000)     5284 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_connection_factory.py
--rw-r--r--   0 ute       (1000) ute       (1000)    24667 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_connection_observer.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8313 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_event.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4828 2024-03-06 09:25:24.000000 moler-3.4.0/test/test_event_awaiter.py
--rw-r--r--   0 ute       (1000) ute       (1000)    13445 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_helpers.py
--rw-r--r--   0 ute       (1000) ute       (1000)    15345 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_loggers.py
--rw-r--r--   0 ute       (1000) ute       (1000)      474 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_moler_sleep.py
--rw-r--r--   0 ute       (1000) ute       (1000)    18464 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_moler_test.py
--rw-r--r--   0 ute       (1000) ute       (1000)     9533 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_publisher.py
--rw-r--r--   0 ute       (1000) ute       (1000)     8171 2024-02-19 07:54:48.000000 moler-3.4.0/test/test_runner.py
--rw-r--r--   0 ute       (1000) ute       (1000)     3908 2024-03-01 08:45:11.000000 moler-3.4.0/test/test_scheduler.py
--rw-r--r--   0 ute       (1000) ute       (1000)     2845 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_table_read_parser.py
--rw-r--r--   0 ute       (1000) ute       (1000)     4260 2024-02-06 08:16:12.000000 moler-3.4.0/test/test_util_loghelper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.579968 moler-3.5.0/
+-rw-r--r--   0 ute       (1000) ute       (1000)     1505 2024-02-06 08:16:12.000000 moler-3.5.0/LICENSE
+-rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-04-16 13:13:13.579968 moler-3.5.0/PKG-INFO
+-rw-r--r--   0 ute       (1000) ute       (1000)    24908 2024-04-16 11:50:01.000000 moler-3.5.0/README.md
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.331968 moler-3.5.0/moler/
+-rw-r--r--   0 ute       (1000) ute       (1000)      143 2024-02-06 08:16:12.000000 moler-3.5.0/moler/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10606 2024-02-19 07:54:48.000000 moler-3.5.0/moler/abstract_moler_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    49062 2024-02-19 07:54:48.000000 moler-3.5.0/moler/asyncio_runner.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.339968 moler-3.5.0/moler/cmd/
+-rw-r--r--   0 ute       (1000) ute       (1000)     4140 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.347968 moler-3.5.0/moler/cmd/adb/
+-rw-r--r--   0 ute       (1000) ute       (1000)      191 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/adb/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5686 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/adb/adb_shell.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      331 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/adb/generic_adb_command.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.403968 moler-3.5.0/moler/cmd/at/
+-rw-r--r--   0 ute       (1000) ute       (1000)      369 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1588 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/at.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1553 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/attach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1826 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/create_pdu_session.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3604 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/cu.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1526 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/detach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1878 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/enable_echo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2808 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/exit_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3786 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/genericat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5005 2024-02-06 14:47:26.000000 moler-3.5.0/moler/cmd/at/get_apns.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3062 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_attach_state.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4770 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_cell_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9134 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_cell_id_gprs.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8605 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_cell_id_lte.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6797 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_cell_id_nr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2792 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_functionality_level.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5945 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/get_imei.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2654 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_imsi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3226 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/get_ip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_manufacturer_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5128 2024-02-06 14:47:26.000000 moler-3.5.0/moler/cmd/at/get_product_info.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3294 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/get_revision_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3555 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/plink_serial.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2361 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/quectel_lock_nr_earfcn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/quectel_network_preferences.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1828 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/at/release_pdu_session.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4632 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/run_script.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2570 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_apn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2454 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_cell_id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3066 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_cell_id_gprs.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3056 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_cell_id_lte.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2741 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_cell_id_nr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3367 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_functionality_level.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2231 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/at/set_mode.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11527 2024-03-27 09:23:44.000000 moler-3.5.0/moler/cmd/commandchangingprompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    28640 2024-03-27 09:23:44.000000 moler-3.5.0/moler/cmd/commandtextualgeneric.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.403968 moler-3.5.0/moler/cmd/juniper/
+-rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.403968 moler-3.5.0/moler/cmd/juniper/cli/
+-rw-r--r--   0 ute       (1000) ute       (1000)      199 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper/cli/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2571 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper/cli/configure.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.419968 moler-3.5.0/moler/cmd/juniper/configure/
+-rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper/configure/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2616 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper/configure/exit_configure.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      993 2024-02-06 14:47:26.000000 moler-3.5.0/moler/cmd/juniper/genericjuniper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.427968 moler-3.5.0/moler/cmd/juniper_ex/
+-rw-r--r--   0 ute       (1000) ute       (1000)      197 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper_ex/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.427968 moler-3.5.0/moler/cmd/juniper_ex/cli/
+-rw-r--r--   0 ute       (1000) ute       (1000)      201 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper_ex/cli/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.435968 moler-3.5.0/moler/cmd/juniper_ex/configure/
+-rw-r--r--   0 ute       (1000) ute       (1000)      207 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/juniper_ex/configure/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      404 2024-02-06 14:47:26.000000 moler-3.5.0/moler/cmd/juniper_ex/genericjuniperex.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.435968 moler-3.5.0/moler/cmd/pdu_aten/
+-rw-r--r--   0 ute       (1000) ute       (1000)      192 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/pdu_aten/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      904 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/pdu_aten/generic_pdu_aten.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.451968 moler-3.5.0/moler/cmd/pdu_aten/pdu/
+-rw-r--r--   0 ute       (1000) ute       (1000)      205 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1193 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/generic_pdu.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/quit.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2895 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/read_meter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2948 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/read_status.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1870 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/pdu_aten/pdu/sw.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.455968 moler-3.5.0/moler/cmd/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      370 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/scpi/genricscpi.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:12.467968 moler-3.5.0/moler/cmd/scpi/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      202 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/scpi/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      415 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/scpi/scpi/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      969 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/scpi/scpi/genericscpistate.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1378 2024-02-06 14:47:26.000000 moler-3.5.0/moler/cmd/scpi/scpi/idn.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1598 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/scpi/scpi/read.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1921 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/scpi/scpi/run_command.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.051968 moler-3.5.0/moler/cmd/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      194 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4744 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/adb_devices.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1957 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/adb_forward.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1465 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/adb_root.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1201 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/bash.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/cat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3342 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/cd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2004 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/chgrp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2158 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/chmod.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2507 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/chown.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1650 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/cp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2807 2024-03-11 13:43:51.000000 moler-3.5.0/moler/cmd/unix/ctrl_c.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2459 2024-03-11 13:46:32.000000 moler-3.5.0/moler/cmd/unix/ctrl_z.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3554 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/cut.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5302 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/date.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3635 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/devmem.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6395 2024-02-06 14:47:26.000000 moler-3.5.0/moler/cmd/unix/df.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4384 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/dmesg.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4325 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/du.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4189 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/echo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1077 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/enter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6135 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/env.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10518 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ethtool.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1799 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/exit.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3769 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/exit_telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6520 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/export.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8513 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/find.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12697 2024-04-09 06:59:25.000000 moler-3.5.0/moler/cmd/unix/generictelnetssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6381 2024-04-11 12:09:37.000000 moler-3.5.0/moler/cmd/unix/genericunix.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9240 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/grep.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6109 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/gunzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4691 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/gzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7087 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/hciconfig.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4606 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/head.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4428 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/hexdump.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2527 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/history.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1417 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/hostname.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4940 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/id.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20386 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ifconfig.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6319 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ip_addr.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6423 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ip_link.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6554 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ip_neigh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19050 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ip_route.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    40999 2024-03-01 08:45:11.000000 moler-3.5.0/moler/cmd/unix/iperf.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    96255 2024-03-01 08:01:14.000000 moler-3.5.0/moler/cmd/unix/iperf2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)   184934 2024-04-15 07:32:05.000000 moler-3.5.0/moler/cmd/unix/iperf3.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17415 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ipsec.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    60585 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/iptables.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2096 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/kill.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2642 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/killall.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1545 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ln.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      432 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/logout.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17144 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ls.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8656 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/lsof.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6108 2024-04-15 07:32:05.000000 moler-3.5.0/moler/cmd/unix/lxc_attach.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7388 2024-04-15 07:32:05.000000 moler-3.5.0/moler/cmd/unix/lxc_info.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19814 2024-04-15 07:32:05.000000 moler-3.5.0/moler/cmd/unix/lxc_ls.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1677 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/md5sum.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1854 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/mkdir.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5082 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/mount.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5753 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/mpstat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1986 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/mv.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20213 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/netstat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7517 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/nft.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    39366 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/nmap.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12330 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/nping.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5168 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ntpq.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3907 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/openssl_s_client.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8259 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/openssl_x509_text_in.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9153 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/passwd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17005 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ping.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1352 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/pkill.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ps.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2609 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/pwd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3048 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/reboot.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1706 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/rm.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7861 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/route.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4494 2024-03-18 09:44:23.000000 moler-3.5.0/moler/cmd/unix/run_script.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3743 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/run_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12696 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/scp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4191 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/sed.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8652 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/service.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10793 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/sftp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4883 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/shasum.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6854 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/socat.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    13026 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/ss.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    45078 2024-03-27 09:23:44.000000 moler-3.5.0/moler/cmd/unix/ssh.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4910 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/sshkeygen.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7129 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/su.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    21553 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/sudo.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1139 2024-02-06 08:16:12.000000 moler-3.5.0/moler/cmd/unix/sync.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3488 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/sysctl.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    16285 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/systemctl.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2509 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/tail.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5810 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/tail_latest_file.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      927 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/tar.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    25812 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/tcpdump.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3071 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/tee.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19408 2024-03-27 09:23:44.000000 moler-3.5.0/moler/cmd/unix/telnet.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    17342 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/top.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1686 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/touch.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7982 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/traceroute.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10992 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/tshark.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2890 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/uname.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1788 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/unxz.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10632 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/unzip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7243 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/uptime.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2946 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/useradd.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3577 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/userdel.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9935 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/w.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    40990 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/wget.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3125 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/which.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1215 2024-02-15 14:32:06.000000 moler-3.5.0/moler/cmd/unix/whoami.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1907 2024-02-19 07:54:48.000000 moler-3.5.0/moler/cmd/unix/zip.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2785 2024-02-19 07:54:48.000000 moler-3.5.0/moler/command.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9032 2024-02-19 07:54:48.000000 moler-3.5.0/moler/command_scheduler.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.067968 moler-3.5.0/moler/config/
+-rw-r--r--   0 ute       (1000) ute       (1000)    12409 2024-03-06 09:25:24.000000 moler-3.5.0/moler/config/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11652 2024-02-19 07:54:48.000000 moler-3.5.0/moler/config/connections.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1534 2024-02-06 14:47:26.000000 moler-3.5.0/moler/config/devices.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    34448 2024-04-15 07:32:05.000000 moler-3.5.0/moler/config/loggers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1589 2024-02-06 14:47:26.000000 moler-3.5.0/moler/config/runners.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1594 2024-02-06 08:16:12.000000 moler-3.5.0/moler/connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8517 2024-02-19 07:54:48.000000 moler-3.5.0/moler/connection_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    21922 2024-03-11 12:51:33.000000 moler-3.5.0/moler/connection_observer.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.159968 moler-3.5.0/moler/device/
+-rw-r--r--   0 ute       (1000) ute       (1000)      425 2024-02-06 08:16:12.000000 moler-3.5.0/moler/device/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7195 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/abstract_device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    16037 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/adbremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    22496 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/adbremote2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10575 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/atremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20904 2024-02-19 07:54:48.000000 moler-3.5.0/moler/device/device.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1663 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/juniper_ex.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    14312 2024-02-06 08:16:12.000000 moler-3.5.0/moler/device/junipergeneric.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12333 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/pdu_aten.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10797 2024-02-06 08:16:12.000000 moler-3.5.0/moler/device/proxy_pc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20245 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/proxy_pc2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    11991 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/scpi.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2339 2024-04-09 06:59:25.000000 moler-3.5.0/moler/device/state_machine.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    46259 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/textualdevice.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9696 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/unixlocal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    19845 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/unixremote.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    25983 2024-04-15 07:32:05.000000 moler-3.5.0/moler/device/unixremote2.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6418 2024-04-16 11:44:52.000000 moler-3.5.0/moler/event.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5038 2024-04-15 07:32:05.000000 moler-3.5.0/moler/event_awaiter.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.183968 moler-3.5.0/moler/events/
+-rw-r--r--   0 ute       (1000) ute       (1000)      134 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.207968 moler-3.5.0/moler/events/juniper/
+-rw-r--r--   0 ute       (1000) ute       (1000)      193 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/juniper/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      898 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/juniper/genericshared_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      324 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/juniper/genericshared_textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.223968 moler-3.5.0/moler/events/juniper_ex/
+-rw-r--r--   0 ute       (1000) ute       (1000)      195 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/juniper_ex/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      903 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      336 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/juniper_ex/genericjuniper_ex_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7401 2024-02-19 07:54:48.000000 moler-3.5.0/moler/events/lineevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.223968 moler-3.5.0/moler/events/pdu_aten/
+-rw-r--r--   0 ute       (1000) ute       (1000)      190 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/pdu_aten/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.239968 moler-3.5.0/moler/events/scpi/
+-rw-r--r--   0 ute       (1000) ute       (1000)      186 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/scpi/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      892 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/scpi/genericscpi_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      325 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/scpi/genericscpi_textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.275968 moler-3.5.0/moler/events/shared/
+-rw-r--r--   0 ute       (1000) ute       (1000)      180 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/shared/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1241 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/shared/genericshared_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      673 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/shared/genericshared_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2227 2024-02-06 14:47:26.000000 moler-3.5.0/moler/events/shared/password_prompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5516 2024-02-06 14:47:26.000000 moler-3.5.0/moler/events/shared/wait4.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5819 2024-04-15 10:55:18.000000 moler-3.5.0/moler/events/textualevent.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.339968 moler-3.5.0/moler/events/unix/
+-rw-r--r--   0 ute       (1000) ute       (1000)      188 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2185 2024-02-06 14:47:26.000000 moler-3.5.0/moler/events/unix/advise_to_change_your_password.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2236 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/failed_login_counter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1243 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/genericunix_lineevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      675 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/genericunix_textualevent.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      997 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/last_failed_login.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2968 2024-02-19 07:54:48.000000 moler-3.5.0/moler/events/unix/last_login.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4734 2024-02-06 14:47:26.000000 moler-3.5.0/moler/events/unix/ping_no_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2302 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/ping_response.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3599 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/private_system.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1317 2024-02-06 14:47:26.000000 moler-3.5.0/moler/events/unix/shutdown.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4641 2024-04-15 07:32:05.000000 moler-3.5.0/moler/events/unix/u_boot_crtm.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1463 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/wait4prompt.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4289 2024-02-19 07:54:48.000000 moler-3.5.0/moler/events/unix/wait4prompts.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1756 2024-02-06 08:16:12.000000 moler-3.5.0/moler/events/unix/warning_default_password.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5760 2024-02-19 07:54:48.000000 moler-3.5.0/moler/exceptions.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18298 2024-04-11 12:09:37.000000 moler-3.5.0/moler/helpers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3176 2024-02-19 07:54:48.000000 moler-3.5.0/moler/instance_loader.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.347968 moler-3.5.0/moler/io/
+-rw-r--r--   0 ute       (1000) ute       (1000)      499 2024-02-06 08:16:12.000000 moler-3.5.0/moler/io/__init__.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.355968 moler-3.5.0/moler/io/asyncio/
+-rw-r--r--   0 ute       (1000) ute       (1000)      536 2024-02-06 14:47:26.000000 moler-3.5.0/moler/io/asyncio/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5954 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/asyncio/tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    14931 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/asyncio/terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7222 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/io_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2156 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/io_exceptions.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.403968 moler-3.5.0/moler/io/raw/
+-rw-r--r--   0 ute       (1000) ute       (1000)     1320 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/raw/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9652 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/raw/memory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    22609 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/raw/sshshell.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      741 2024-02-06 14:47:26.000000 moler-3.5.0/moler/io/raw/subprocess.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7554 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/raw/tcp.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9922 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/raw/tcpserverpiped.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     7325 2024-02-19 07:54:48.000000 moler-3.5.0/moler/io/raw/terminal.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5679 2024-02-06 14:47:26.000000 moler-3.5.0/moler/moler_connection_for_single_thread_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1672 2024-02-06 08:16:12.000000 moler-3.5.0/moler/observable_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4597 2024-02-19 07:54:48.000000 moler-3.5.0/moler/observer_thread_wrapper.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.423968 moler-3.5.0/moler/parser/
+-rw-r--r--   0 ute       (1000) ute       (1000)      141 2024-02-06 08:16:12.000000 moler-3.5.0/moler/parser/__init__.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18616 2024-04-15 07:32:05.000000 moler-3.5.0/moler/parser/table_text.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5503 2024-02-06 14:47:26.000000 moler-3.5.0/moler/publisher.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    37230 2024-03-06 09:47:05.000000 moler-3.5.0/moler/runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3910 2024-02-19 07:54:48.000000 moler-3.5.0/moler/runner_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20412 2024-02-19 07:54:48.000000 moler-3.5.0/moler/runner_single_thread.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     6890 2024-04-15 07:32:05.000000 moler-3.5.0/moler/scheduler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8824 2024-02-19 07:54:48.000000 moler-3.5.0/moler/threaded_moler_connection.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.471968 moler-3.5.0/moler/util/
+-rw-r--r--   0 ute       (1000) ute       (1000)      138 2024-02-06 08:16:12.000000 moler-3.5.0/moler/util/__init__.py
+-rwxr-xr-x   0 ute       (1000) ute       (1000)    13210 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/cmds_events_doc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2581 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/compressed_rotating_file_handler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1405 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/compressed_timed_rotating_file_handler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1255 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/connection_observer.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3436 2024-02-14 14:53:24.000000 moler-3.5.0/moler/util/connection_observer_life_status.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4520 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/converterhelper.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    12577 2024-04-15 07:32:05.000000 moler-3.5.0/moler/util/devices_SM.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2987 2024-02-06 14:47:26.000000 moler-3.5.0/moler/util/loghelper.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9386 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/moler_serial_proxy.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10038 2024-04-15 07:32:05.000000 moler-3.5.0/moler/util/moler_test.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     1973 2024-02-19 07:54:48.000000 moler-3.5.0/moler/util/tracked_thread.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.579968 moler-3.5.0/moler.egg-info/
+-rw-r--r--   0 ute       (1000) ute       (1000)    26591 2024-04-16 13:13:11.000000 moler-3.5.0/moler.egg-info/PKG-INFO
+-rw-r--r--   0 ute       (1000) ute       (1000)     8786 2024-04-16 13:13:12.000000 moler-3.5.0/moler.egg-info/SOURCES.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)        1 2024-04-16 13:13:11.000000 moler-3.5.0/moler.egg-info/dependency_links.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)      157 2024-04-16 13:13:11.000000 moler-3.5.0/moler.egg-info/requires.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)        6 2024-04-16 13:13:11.000000 moler-3.5.0/moler.egg-info/top_level.txt
+-rw-r--r--   0 ute       (1000) ute       (1000)      165 2024-04-16 13:13:13.599968 moler-3.5.0/setup.cfg
+-rw-r--r--   0 ute       (1000) ute       (1000)     1966 2024-04-15 07:32:05.000000 moler-3.5.0/setup.py
+drwxr-xr-x   0 ute       (1000) ute       (1000)        0 2024-04-16 13:13:13.575968 moler-3.5.0/test/
+-rw-r--r--   0 ute       (1000) ute       (1000)    10233 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_cmds_events_doc.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    10694 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_command.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    20821 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_connection.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8679 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_connection_configuration.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     5284 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_connection_factory.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    24667 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_connection_observer.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8313 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_event.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4828 2024-03-06 09:25:24.000000 moler-3.5.0/test/test_event_awaiter.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    13445 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_helpers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    15345 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_loggers.py
+-rw-r--r--   0 ute       (1000) ute       (1000)      474 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_moler_sleep.py
+-rw-r--r--   0 ute       (1000) ute       (1000)    18464 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_moler_test.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     9533 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_publisher.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     8171 2024-02-19 07:54:48.000000 moler-3.5.0/test/test_runner.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     3908 2024-03-01 08:45:11.000000 moler-3.5.0/test/test_scheduler.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     2845 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_table_read_parser.py
+-rw-r--r--   0 ute       (1000) ute       (1000)     4260 2024-02-06 08:16:12.000000 moler-3.5.0/test/test_util_loghelper.py
```

### Comparing `moler-3.4.0/LICENSE` & `moler-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/PKG-INFO` & `moler-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moler
-Version: 3.4.0
+Version: 3.5.0
 Summary: Moler is a library for working with terminals, mainly for automated tests
 Home-page: https://github.com/nokia/moler
 Author: Nokia
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/nokia/moler/issues
 Project-URL: Source, https://github.com/nokia/moler
 Keywords: testing development
@@ -38,15 +38,15 @@
 Requires-Dist: psutil
 Requires-Dist: python-dateutil
 Requires-Dist: pyserial
 Requires-Dist: cryptography
 Requires-Dist: paramiko
 Requires-Dist: importlib-metadata
 
-[![image](https://img.shields.io/badge/pypi-v3.4.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v3.5.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://github.com/nokia/moler/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/nokia/moler/actions)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
 
 # Table of Contents
 1. [Changelog](#changelog)
 2. [Moler info](#moler)
```

### Comparing `moler-3.4.0/README.md` & `moler-3.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![image](https://img.shields.io/badge/pypi-v3.4.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v3.5.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://github.com/nokia/moler/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/nokia/moler/actions)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
 
 # Table of Contents
 1. [Changelog](#changelog)
 2. [Moler info](#moler)
```

### Comparing `moler-3.4.0/moler/abstract_moler_connection.py` & `moler-3.5.0/moler/abstract_moler_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/asyncio_runner.py` & `moler-3.5.0/moler/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/__init__.py` & `moler-3.5.0/moler/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/adb/adb_shell.py` & `moler-3.5.0/moler/cmd/adb/adb_shell.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/at.py` & `moler-3.5.0/moler/cmd/at/at.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/attach.py` & `moler-3.5.0/moler/cmd/at/attach.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/create_pdu_session.py` & `moler-3.5.0/moler/cmd/at/create_pdu_session.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/cu.py` & `moler-3.5.0/moler/cmd/at/cu.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/detach.py` & `moler-3.5.0/moler/cmd/at/detach.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/enable_echo.py` & `moler-3.5.0/moler/cmd/at/enable_echo.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/exit_serial_proxy.py` & `moler-3.5.0/moler/cmd/at/exit_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/genericat.py` & `moler-3.5.0/moler/cmd/at/genericat.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_apns.py` & `moler-3.5.0/moler/cmd/at/get_apns.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_attach_state.py` & `moler-3.5.0/moler/cmd/at/get_attach_state.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_cell_id.py` & `moler-3.5.0/moler/cmd/at/get_cell_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_cell_id_gprs.py` & `moler-3.5.0/moler/cmd/at/get_cell_id_gprs.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_cell_id_lte.py` & `moler-3.5.0/moler/cmd/at/get_cell_id_lte.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_cell_id_nr.py` & `moler-3.5.0/moler/cmd/at/get_cell_id_nr.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_functionality_level.py` & `moler-3.5.0/moler/cmd/at/get_functionality_level.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_imei.py` & `moler-3.5.0/moler/cmd/at/get_imei.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_imsi.py` & `moler-3.5.0/moler/cmd/at/get_imsi.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_ip.py` & `moler-3.5.0/moler/cmd/at/get_ip.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_manufacturer_id.py` & `moler-3.5.0/moler/cmd/at/get_manufacturer_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_product_info.py` & `moler-3.5.0/moler/cmd/at/get_product_info.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/get_revision_id.py` & `moler-3.5.0/moler/cmd/at/get_revision_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/plink_serial.py` & `moler-3.5.0/moler/cmd/at/plink_serial.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/quectel_lock_nr_earfcn.py` & `moler-3.5.0/moler/cmd/at/quectel_lock_nr_earfcn.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/quectel_network_preferences.py` & `moler-3.5.0/moler/cmd/at/quectel_network_preferences.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/release_pdu_session.py` & `moler-3.5.0/moler/cmd/at/release_pdu_session.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/run_script.py` & `moler-3.5.0/moler/cmd/at/run_script.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_apn.py` & `moler-3.5.0/moler/cmd/at/set_apn.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_cell_id.py` & `moler-3.5.0/moler/cmd/at/set_cell_id.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_cell_id_gprs.py` & `moler-3.5.0/moler/cmd/at/set_cell_id_gprs.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_cell_id_lte.py` & `moler-3.5.0/moler/cmd/at/set_cell_id_lte.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_cell_id_nr.py` & `moler-3.5.0/moler/cmd/at/set_cell_id_nr.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_functionality_level.py` & `moler-3.5.0/moler/cmd/at/set_functionality_level.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/at/set_mode.py` & `moler-3.5.0/moler/cmd/at/set_mode.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/commandchangingprompt.py` & `moler-3.5.0/moler/cmd/commandchangingprompt.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/commandtextualgeneric.py` & `moler-3.5.0/moler/cmd/commandtextualgeneric.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/juniper/cli/configure.py` & `moler-3.5.0/moler/cmd/juniper/cli/configure.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/juniper/configure/exit_configure.py` & `moler-3.5.0/moler/cmd/juniper/configure/exit_configure.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/juniper/genericjuniper.py` & `moler-3.5.0/moler/cmd/juniper/genericjuniper.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/pdu_aten/generic_pdu_aten.py` & `moler-3.5.0/moler/cmd/pdu_aten/generic_pdu_aten.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/pdu_aten/pdu/generic_pdu.py` & `moler-3.5.0/moler/cmd/pdu_aten/pdu/generic_pdu.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/pdu_aten/pdu/quit.py` & `moler-3.5.0/moler/cmd/pdu_aten/pdu/quit.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/pdu_aten/pdu/read_meter.py` & `moler-3.5.0/moler/cmd/pdu_aten/pdu/read_meter.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/pdu_aten/pdu/read_status.py` & `moler-3.5.0/moler/cmd/pdu_aten/pdu/read_status.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/pdu_aten/pdu/sw.py` & `moler-3.5.0/moler/cmd/pdu_aten/pdu/sw.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/scpi/scpi/genericscpistate.py` & `moler-3.5.0/moler/cmd/scpi/scpi/genericscpistate.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/scpi/scpi/idn.py` & `moler-3.5.0/moler/cmd/scpi/scpi/idn.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/scpi/scpi/read.py` & `moler-3.5.0/moler/cmd/scpi/scpi/read.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/scpi/scpi/run_command.py` & `moler-3.5.0/moler/cmd/scpi/scpi/run_command.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/adb_devices.py` & `moler-3.5.0/moler/cmd/unix/adb_devices.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/adb_forward.py` & `moler-3.5.0/moler/cmd/unix/adb_forward.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/adb_root.py` & `moler-3.5.0/moler/cmd/unix/adb_root.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/bash.py` & `moler-3.5.0/moler/cmd/unix/bash.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/cat.py` & `moler-3.5.0/moler/cmd/unix/cat.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/cd.py` & `moler-3.5.0/moler/cmd/unix/cd.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/chgrp.py` & `moler-3.5.0/moler/cmd/unix/chgrp.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/chmod.py` & `moler-3.5.0/moler/cmd/unix/chmod.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/chown.py` & `moler-3.5.0/moler/cmd/unix/chown.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/cp.py` & `moler-3.5.0/moler/cmd/unix/cp.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ctrl_c.py` & `moler-3.5.0/moler/cmd/unix/ctrl_c.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ctrl_z.py` & `moler-3.5.0/moler/cmd/unix/ctrl_z.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/cut.py` & `moler-3.5.0/moler/cmd/unix/cut.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/date.py` & `moler-3.5.0/moler/cmd/unix/date.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/devmem.py` & `moler-3.5.0/moler/cmd/unix/devmem.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/df.py` & `moler-3.5.0/moler/cmd/unix/df.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/dmesg.py` & `moler-3.5.0/moler/cmd/unix/dmesg.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/du.py` & `moler-3.5.0/moler/cmd/unix/du.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/echo.py` & `moler-3.5.0/moler/cmd/unix/echo.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/enter.py` & `moler-3.5.0/moler/cmd/unix/enter.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/env.py` & `moler-3.5.0/moler/cmd/unix/env.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ethtool.py` & `moler-3.5.0/moler/cmd/unix/ethtool.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/exit.py` & `moler-3.5.0/moler/cmd/unix/exit.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/exit_telnet.py` & `moler-3.5.0/moler/cmd/unix/exit_telnet.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/export.py` & `moler-3.5.0/moler/cmd/unix/export.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/find.py` & `moler-3.5.0/moler/cmd/unix/find.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/generictelnetssh.py` & `moler-3.5.0/moler/cmd/unix/generictelnetssh.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/genericunix.py` & `moler-3.5.0/moler/cmd/unix/genericunix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Generic Unix/Linux module
 """
 
-__author__ = 'Marcin Usielski'
+__author__ = 'Marcin Usielski', 'Jakub Kochaniak'
 __copyright__ = 'Copyright (C) 2018-2024, Nokia'
-__email__ = 'marcin.usielski@nokia.com'
+__email__ = 'marcin.usielski@nokia.com', 'jakub.kochaniak@nokia.com'
 
 import re
 import abc
 from typing import Optional, Union, Pattern, Sequence
 import six
 from moler.abstract_moler_connection import AbstractMolerConnection
 from moler.runner import ConnectionObserverRunner
@@ -44,14 +44,15 @@
         super(GenericUnixCommand, self).__init__(connection=connection, prompt=prompt, newline_chars=newline_chars,
                                                  runner=runner)
         self.remove_all_known_special_chars_from_terminal_output = True
         self.re_fail = re.compile(r_cmd_failure_cause_alternatives, re.IGNORECASE)
 
         self._ctrl_z_sent = False
         self._kill_ctrl_z_sent = False
+        self._kill_ctrl_z_job_done = False
         self._instance_timeout_action = None
 
     def _decode_line(self, line: str) -> str:
         """
         Method to delete new line chars and other chars we don not need to parse in on_new_line (color escape character)
 
         :param line: Line with special chars, raw string from device
@@ -122,26 +123,40 @@
     def is_end_of_cmd_output(self, line: str) -> bool:
         """
         Checks if end of command is reached.
 
         :param line: Line from device.
         :return: True if end of command is reached, False otherwise.
         """
-        if not self._kill_ctrl_z_sent and self._ctrl_z_sent:
+        if not self._kill_ctrl_z_job_done and self._ctrl_z_sent:
             return False
         return super(GenericUnixCommand, self).is_end_of_cmd_output(line=line)
 
     # [2]+  Stopped
     _re_ctrl_z_stopped = re.compile(r"\[(?P<JOB_ID>\d+)\]\+\s+Stopped")
 
+    # [2]+  Done
+    _re_kill_done = re.compile(r"\[?\d+\]\+\s+Done")
+
+    # -bash: wait: %2: no such job
+    _re_kill_no_job = re.compile(r"\:\s+\%\d+\s?\:\s+no such job")
+
     def _parse_control_z(self, line: str) -> None:
         """
         Parse line that is control+z.
 
         :param line: Line from device.
         :return: None.
         """
-        if self._ctrl_z_sent and not self._kill_ctrl_z_sent and self._regex_helper.search_compiled(GenericUnixCommand._re_ctrl_z_stopped, line):
+        if self._ctrl_z_sent and not self._kill_ctrl_z_job_done and self._regex_helper.search_compiled(
+            GenericUnixCommand._re_ctrl_z_stopped, line
+        ):
             job_id = self._regex_helper.group("JOB_ID")
-            self.connection.sendline(f"kill %{job_id}")
+            self.connection.sendline(f"kill %{job_id}; wait %{job_id}")
             self._kill_ctrl_z_sent = True
             raise ParsingDone()
+
+        if self._kill_ctrl_z_sent and (
+            self._regex_helper.search_compiled(GenericUnixCommand._re_kill_done, line) or self._regex_helper.search_compiled(GenericUnixCommand._re_kill_no_job, line)
+        ):
+            self._kill_ctrl_z_job_done = True
+            raise ParsingDone()
```

### Comparing `moler-3.4.0/moler/cmd/unix/grep.py` & `moler-3.5.0/moler/cmd/unix/grep.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/gunzip.py` & `moler-3.5.0/moler/cmd/unix/gunzip.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/gzip.py` & `moler-3.5.0/moler/cmd/unix/gzip.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/hciconfig.py` & `moler-3.5.0/moler/cmd/unix/hciconfig.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/head.py` & `moler-3.5.0/moler/cmd/unix/head.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/hexdump.py` & `moler-3.5.0/moler/cmd/unix/hexdump.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/history.py` & `moler-3.5.0/moler/cmd/unix/history.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/hostname.py` & `moler-3.5.0/moler/cmd/unix/hostname.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/id.py` & `moler-3.5.0/moler/cmd/unix/id.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ifconfig.py` & `moler-3.5.0/moler/cmd/unix/ifconfig.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ip_addr.py` & `moler-3.5.0/moler/cmd/unix/ip_addr.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ip_link.py` & `moler-3.5.0/moler/cmd/unix/ip_link.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ip_neigh.py` & `moler-3.5.0/moler/cmd/unix/ip_neigh.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ip_route.py` & `moler-3.5.0/moler/cmd/unix/ip_route.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/iperf.py` & `moler-3.5.0/moler/cmd/unix/iperf.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/iperf2.py` & `moler-3.5.0/moler/cmd/unix/iperf2.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/iperf3.py` & `moler-3.5.0/moler/cmd/unix/iperf3.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 Iperf3 command module.
 
 It is refactored Iperf2 module adapted to iperf ver. 3.9.
 The changes align with the iperf3 documentation available at https://iperf.fr/iperf-doc.php.
 
 Important changes (in comparison to Iperf2) to note:
+
 - Certain options such as -u, -t, and -P are no longer applicable on the server side.
   Although these options are included on the client side,
 - Removed dual tests,
 - Added several new stats: Retr and Cwnd for TCP; Total Datagrams for UDP.
 """
 
 __author__ = "Kacper Kozik"
```

### Comparing `moler-3.4.0/moler/cmd/unix/ipsec.py` & `moler-3.5.0/moler/cmd/unix/ipsec.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/iptables.py` & `moler-3.5.0/moler/cmd/unix/iptables.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/kill.py` & `moler-3.5.0/moler/cmd/unix/kill.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/killall.py` & `moler-3.5.0/moler/cmd/unix/killall.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ln.py` & `moler-3.5.0/moler/cmd/unix/ln.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ls.py` & `moler-3.5.0/moler/cmd/unix/ls.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/lsof.py` & `moler-3.5.0/moler/cmd/unix/lsof.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/lxc_attach.py` & `moler-3.5.0/moler/cmd/unix/lxc_attach.py`

 * *Files 17% similar despite different names*

```diff
@@ -89,70 +89,67 @@
     "name": "0x2015",
     "options": "--quiet"
 }
 
 COMMAND_RESULT_2 = {}
 
 
-"""
-=================================================HELP=MESSAGE===========================================================
-root@0xe000:~ >lxc-attach --help
-Usage: lxc-attach --name=NAME [-- COMMAND]
-
-Execute the specified COMMAND - enter the container NAME
-
-Options :
-  -n, --name=NAME   NAME of the container
-  -e, --elevated-privileges=PRIVILEGES
-                    Use elevated privileges instead of those of the
-                    container. If you don't specify privileges to be
-                    elevated as OR'd list: CAP, CGROUP and LSM (capabilities,
-                    cgroup and restrictions, respectively) then all of them
-                    will be elevated.
-                    WARNING: This may leak privileges into the container.
-                    Use with care.
-  -a, --arch=ARCH   Use ARCH for program instead of container's own
-                    architecture.
-  -s, --namespaces=FLAGS
-                    Don't attach to all the namespaces of the container
-                    but just to the following OR'd list of flags:
-                    MOUNT, PID, UTSNAME, IPC, USER or NETWORK.
-                    WARNING: Using -s implies -e with all privileges
-                    elevated, it may therefore leak privileges into the
-                    container. Use with care.
-  -R, --remount-sys-proc
-                    Remount /sys and /proc if not attaching to the
-                    mount namespace when using -s in order to properly
-                    reflect the correct namespace context. See the
-                    lxc-attach(1) manual page for details.
-      --clear-env   Clear all environment variables before attaching.
-                    The attached shell/program will start with only
-                    container=lxc set.
-      --keep-env    Keep all current environment variables. This
-                    is the current default behaviour, but is likely to
-                    change in the future.
-  -L, --pty-log=FILE
-                    Log pty output to FILE
-  -v, --set-var     Set an additional variable that is seen by the
-                    attached program in the container. May be specified
-                    multiple times.
-      --keep-var    Keep an additional environment variable. Only
-                    applicable if --clear-env is specified. May be used
-                    multiple times.
-  -f, --rcfile=FILE
-                    Load configuration file FILE
-
-Common options :
-  -o, --logfile=FILE               Output log to FILE instead of stderr
-  -l, --logpriority=LEVEL          Set log priority to LEVEL
-  -q, --quiet                      Don't produce any output
-  -P, --lxcpath=PATH               Use specified container path
-  -?, --help                       Give this help list
-      --usage                      Give a short usage message
-      --version                    Print the version number
+# =================================================HELP=MESSAGE===========================================================
+# root@0xe000:~ >lxc-attach --help
+# Usage: lxc-attach --name=NAME [-- COMMAND]
+
+# Execute the specified COMMAND - enter the container NAME
+
+# Options :
+#   -n, --name=NAME   NAME of the container
+#   -e, --elevated-privileges=PRIVILEGES
+#                     Use elevated privileges instead of those of the
+#                     container. If you don't specify privileges to be
+#                     elevated as OR'd list: CAP, CGROUP and LSM (capabilities,
+#                     cgroup and restrictions, respectively) then all of them
+#                     will be elevated.
+#                     WARNING: This may leak privileges into the container.
+#                     Use with care.
+#   -a, --arch=ARCH   Use ARCH for program instead of container's own
+#                     architecture.
+#   -s, --namespaces=FLAGS
+#                     Don't attach to all the namespaces of the container
+#                     but just to the following OR'd list of flags:
+#                     MOUNT, PID, UTSNAME, IPC, USER or NETWORK.
+#                     WARNING: Using -s implies -e with all privileges
+#                     elevated, it may therefore leak privileges into the
+#                     container. Use with care.
+#   -R,--remount-sys-proc
+#                     Remount /sys and /proc if not attaching to the
+#                     mount namespace when using -s in order to properly
+#                     reflect the correct namespace context. See the
+#                     lxc-attach(1) manual page for details.
+#       --clear-env   Clear all environment variables before attaching.
+#                     The attached shell/program will start with only
+#                     container=lxc set.
+#       --keep-env    Keep all current environment variables. This
+#                     is the current default behaviour, but is likely to
+#                     change in the future.
+#   -L, --pty-log=FILE
+#                     Log pty output to FILE
+#   -v, --set-var     Set an additional variable that is seen by the
+#                     attached program in the container. May be specified
+#                     multiple times.
+#       --keep-var    Keep an additional environment variable. Only
+#                     applicable if --clear-env is specified. May be used
+#                     multiple times.
+#   -f, --rcfile=FILE
+#                     Load configuration file FILE
+
+# Common options :
+#   -o, --logfile=FILE               Output log to FILE instead of stderr
+#   -l, --logpriority=LEVEL          Set log priority to LEVEL
+#   -q, --quiet                      Don't produce any output
+#   -P, --lxcpath=PATH               Use specified container path
+#   -?, --help                       Give this help list
+#       --usage                      Give a short usage message
+#       --version                    Print the version number
 
-Mandatory or optional arguments to long options are also mandatory or optional
-for any corresponding short options.
+# Mandatory or optional arguments to long options are also mandatory or optional
+# for any corresponding short options.
 
-See the lxc-attach man page for further information.
-
-"""
+# See the lxc-attach man page for further information.
```

### Comparing `moler-3.4.0/moler/cmd/unix/lxc_info.py` & `moler-3.5.0/moler/cmd/unix/lxc_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,39 +194,37 @@
 State:          RUNNING
 root@fserver >"""
 
 COMMAND_KWARGS_2 = {"name": "0xe019", "options": "-s"}
 
 COMMAND_RESULT_2 = {"RESULT": {"State": "RUNNING"}}
 
-"""
-=================================================HELP=MESSAGE===========================================================
-root@server~ >lxc-info --help
-Usage: lxc-info --name=NAME
-
-lxc-info display some information about a container with the identifier NAME
-
-Options :
-  -n, --name=NAME       NAME of the container
-  -c, --config=KEY      show configuration variable KEY from running container
-  -i, --ips             shows the IP addresses
-  -p, --pid             shows the process id of the init container
-  -S, --stats           shows usage stats
-  -H, --no-humanize     shows stats as raw numbers, not humanized
-  -s, --state           shows the state of the container
-  --rcfile=FILE         Load configuration file FILE
-
-Common options :
-  -o, --logfile=FILE               Output log to FILE instead of stderr
-  -l, --logpriority=LEVEL          Set log priority to LEVEL
-  -q, --quiet                      Don't produce any output
-  -P, --lxcpath=PATH               Use specified container path
-  -?, --help                       Give this help list
-      --usage                      Give a short usage message
-      --version                    Print the version number
 
-Mandatory or optional arguments to long options are also mandatory or optional
-for any corresponding short options.
+# =================================================HELP=MESSAGE===========================================================
+# root@server~ >lxc-info --help
+# Usage: lxc-info --name=NAME
+
+# lxc-info display some information about a container with the identifier NAME
+
+# Options :
+#   -n, --name=NAME       NAME of the container
+#   -c, --config=KEY      show configuration variable KEY from running container
+#   -i, --ips             shows the IP addresses
+#   -p, --pid             shows the process id of the init container
+#   -S, --stats           shows usage stats
+#   -H, --no-humanize     shows stats as raw numbers, not humanized
+#   -s, --state           shows the state of the container
+#   --rcfile=FILE         Load configuration file FILE
+
+# Common options :
+#   -o, --logfile=FILE               Output log to FILE instead of stderr
+#   -l, --logpriority=LEVEL          Set log priority to LEVEL
+#   -q, --quiet                      Don't produce any output
+#   -P, --lxcpath=PATH               Use specified container path
+#   -?, --help                       Give this help list
+#       --usage                      Give a short usage message
+#       --version                    Print the version number
 
-See the lxc-info man page for further information.
+# Mandatory or optional arguments to long options are also mandatory or optional
+# for any corresponding short options.
 
-"""
+# See the lxc-info man page for further information.
```

### Comparing `moler-3.4.0/moler/cmd/unix/lxc_ls.py` & `moler-3.5.0/moler/cmd/unix/lxc_ls.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,48 +347,47 @@
             "0xe019/0xe00c",
             "0xe019/0xe00d",
             "0xe019/0xe019",
         ],
     ]
 }
 
-"""
-==================================================HELP=MESSAGE==========================================================
-root@0xe000:~ >lxc-ls --help
-Usage: lxc-ls
-[-P lxcpath] [--active] [--running] [--frozen] [--stopped] [--nesting] [-g groups] [--filter regex]
-[-1] [-P lxcpath] [--active] [--running] [--frozen] [--stopped] [--nesting] [-g groups] [--filter regex]
-[-f] [-P lxcpath] [--active] [--running] [--frozen] [--stopped] [--nesting] [-g groups] [--filter regex]
-
-lxc-ls list containers
-
-Options :
-  -1, --line         show one entry per line
-  -f, --fancy        use a fancy, column-based output
-  -F, --fancy-format comma separated list of columns to show in the fancy output
-                     valid columns are: NAME, STATE, PID, RAM, SWAP, AUTOSTART,
-                     GROUPS, INTERFACE, IPV4 and IPV6
-  --active           list only active containers
-  --running          list only running containers
-  --frozen           list only frozen containers
-  --stopped          list only stopped containers
-  --defined          list only defined containers
-  --nesting=NUM      list nested containers up to NUM (default is 5) levels of nesting
-  --filter=REGEX     filter container names by regular expression
-  -g --groups        comma separated list of groups a container must have to be displayed
-
-Common options :
-  -o, --logfile=FILE               Output log to FILE instead of stderr
-  -l, --logpriority=LEVEL          Set log priority to LEVEL
-  -q, --quiet                      Don't produce any output
-  -P, --lxcpath=PATH               Use specified container path
-  -?, --help                       Give this help list
-      --usage                      Give a short usage message
-      --version                    Print the version number
 
-Mandatory or optional arguments to long options are also mandatory or optional
-for any corresponding short options.
+# ==================================================HELP=MESSAGE==========================================================
+# root@0xe000:~ >lxc-ls --help
+# Usage: lxc-ls
+# [-P lxcpath] [--active] [--running] [--frozen] [--stopped] [--nesting] [-g groups] [--filter regex]
+# [-1] [-P lxcpath] [--active] [--running] [--frozen] [--stopped] [--nesting] [-g groups] [--filter regex]
+# [-f] [-P lxcpath] [--active] [--running] [--frozen] [--stopped] [--nesting] [-g groups] [--filter regex]
+
+# lxc-ls list containers
+
+# Options :
+#   -1, --line         show one entry per line
+#   -f, --fancy        use a fancy, column-based output
+#   -F, --fancy-format comma separated list of columns to show in the fancy output
+#                      valid columns are: NAME, STATE, PID, RAM, SWAP, AUTOSTART,
+#                      GROUPS, INTERFACE, IPV4 and IPV6
+#   --active           list only active containers
+#   --running          list only running containers
+#   --frozen           list only frozen containers
+#   --stopped          list only stopped containers
+#   --defined          list only defined containers
+#   --nesting=NUM      list nested containers up to NUM (default is 5) levels of nesting
+#   --filter=REGEX     filter container names by regular expression
+#   -g --groups        comma separated list of groups a container must have to be displayed
+
+# Common options :
+#   -o, --logfile=FILE               Output log to FILE instead of stderr
+#   -l, --logpriority=LEVEL          Set log priority to LEVEL
+#   -q, --quiet                      Don't produce any output
+#   -P, --lxcpath=PATH               Use specified container path
+#   -?, --help                       Give this help list
+#       --usage                      Give a short usage message
+#       --version                    Print the version number
 
-See the lxc-ls man page for further information.
+# Mandatory or optional arguments to long options are also mandatory or optional
+# for any corresponding short options.
 
-root@0xe000:~ >
-"""
+# See the lxc-ls man page for further information.
+
+# root@0xe000:~ >
```

### Comparing `moler-3.4.0/moler/cmd/unix/md5sum.py` & `moler-3.5.0/moler/cmd/unix/md5sum.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/mkdir.py` & `moler-3.5.0/moler/cmd/unix/mkdir.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/mount.py` & `moler-3.5.0/moler/cmd/unix/mount.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/mpstat.py` & `moler-3.5.0/moler/cmd/unix/mpstat.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/mv.py` & `moler-3.5.0/moler/cmd/unix/mv.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/netstat.py` & `moler-3.5.0/moler/cmd/unix/netstat.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/nft.py` & `moler-3.5.0/moler/cmd/unix/nft.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/nmap.py` & `moler-3.5.0/moler/cmd/unix/nmap.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/nping.py` & `moler-3.5.0/moler/cmd/unix/nping.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ntpq.py` & `moler-3.5.0/moler/cmd/unix/ntpq.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/openssl_s_client.py` & `moler-3.5.0/moler/cmd/unix/openssl_s_client.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/openssl_x509_text_in.py` & `moler-3.5.0/moler/cmd/unix/openssl_x509_text_in.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/passwd.py` & `moler-3.5.0/moler/cmd/unix/passwd.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ping.py` & `moler-3.5.0/moler/cmd/unix/ping.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/pkill.py` & `moler-3.5.0/moler/cmd/unix/pkill.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ps.py` & `moler-3.5.0/moler/cmd/unix/ps.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/pwd.py` & `moler-3.5.0/moler/cmd/unix/pwd.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/reboot.py` & `moler-3.5.0/moler/cmd/unix/reboot.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/rm.py` & `moler-3.5.0/moler/cmd/unix/rm.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/route.py` & `moler-3.5.0/moler/cmd/unix/route.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/run_script.py` & `moler-3.5.0/moler/cmd/unix/run_script.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/run_serial_proxy.py` & `moler-3.5.0/moler/cmd/unix/run_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/scp.py` & `moler-3.5.0/moler/cmd/unix/scp.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/sed.py` & `moler-3.5.0/moler/cmd/unix/sed.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/service.py` & `moler-3.5.0/moler/cmd/unix/service.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/sftp.py` & `moler-3.5.0/moler/cmd/unix/sftp.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/shasum.py` & `moler-3.5.0/moler/cmd/unix/shasum.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/socat.py` & `moler-3.5.0/moler/cmd/unix/socat.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ss.py` & `moler-3.5.0/moler/cmd/unix/ss.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/ssh.py` & `moler-3.5.0/moler/cmd/unix/ssh.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/sshkeygen.py` & `moler-3.5.0/moler/cmd/unix/sshkeygen.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/su.py` & `moler-3.5.0/moler/cmd/unix/su.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/sudo.py` & `moler-3.5.0/moler/cmd/unix/sudo.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/sync.py` & `moler-3.5.0/moler/cmd/unix/sync.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/sysctl.py` & `moler-3.5.0/moler/cmd/unix/sysctl.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/systemctl.py` & `moler-3.5.0/moler/cmd/unix/systemctl.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/tail.py` & `moler-3.5.0/moler/cmd/unix/tail.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/tail_latest_file.py` & `moler-3.5.0/moler/cmd/unix/tail_latest_file.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/tar.py` & `moler-3.5.0/moler/cmd/unix/tar.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/tcpdump.py` & `moler-3.5.0/moler/cmd/unix/tcpdump.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/tee.py` & `moler-3.5.0/moler/cmd/unix/tee.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/telnet.py` & `moler-3.5.0/moler/cmd/unix/telnet.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/top.py` & `moler-3.5.0/moler/cmd/unix/top.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/touch.py` & `moler-3.5.0/moler/cmd/unix/touch.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/traceroute.py` & `moler-3.5.0/moler/cmd/unix/traceroute.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/tshark.py` & `moler-3.5.0/moler/cmd/unix/tshark.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/uname.py` & `moler-3.5.0/moler/cmd/unix/uname.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/unxz.py` & `moler-3.5.0/moler/cmd/unix/unxz.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/unzip.py` & `moler-3.5.0/moler/cmd/unix/unzip.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/uptime.py` & `moler-3.5.0/moler/cmd/unix/uptime.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/useradd.py` & `moler-3.5.0/moler/cmd/unix/useradd.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/userdel.py` & `moler-3.5.0/moler/cmd/unix/userdel.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/w.py` & `moler-3.5.0/moler/cmd/unix/w.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/wget.py` & `moler-3.5.0/moler/cmd/unix/wget.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/which.py` & `moler-3.5.0/moler/cmd/unix/which.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/whoami.py` & `moler-3.5.0/moler/cmd/unix/whoami.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/cmd/unix/zip.py` & `moler-3.5.0/moler/cmd/unix/zip.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/command.py` & `moler-3.5.0/moler/command.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/command_scheduler.py` & `moler-3.5.0/moler/command_scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/config/__init__.py` & `moler-3.5.0/moler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/config/connections.py` & `moler-3.5.0/moler/config/connections.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/config/devices.py` & `moler-3.5.0/moler/config/devices.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/config/loggers.py` & `moler-3.5.0/moler/config/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,16 @@
 
     return f"{version} cloned from git repository"
 
 
 def set_backup_count(backup_count):
     """
     Set maximum number of files of logs to rotate for rotating logging. If parameter is not an int number then the
-     function does not change any value.
+    function does not change any value.
+
     :param backup_count: int number of how many files to keep to rotate logs.
     :return: None
     """
     global _backup_count  # pylint: disable=global-statement
     try:
         _backup_count = int(backup_count)
     except ValueError:
@@ -524,20 +525,21 @@
     name,
     log_file=None,
     log_level=TRACE,
     log_format="%(asctime)s %(levelname)-10s: |%(message)s",
     datefmt=None,
 ):
     """
-    Creates Logger with (optional) file writer
+    Create Logger with (optional) file writer.
+
     :param name: Logger name
-    :param log_file: Path to logfile. Final logfile location is logging_path + log_file
-    :param log_level: only log records with equal and greater level will be accepted for storage in log
-    :param log_format: layout of log file, default is "%(asctime)s %(levelname)-10s: |%(message)s"
-    :param datefmt: format the creation time of the log record
+    :param log_file: Path to logfile. Final logfile location is logging_path + log_file.
+    :param log_level: only log records with equal and greater level will be accepted for storage in log.
+    :param log_format: layout of log file.".
+    :param datefmt: format the creation time of the log record.
     :return: None
     """
     logger = logging.getLogger(name)
     if name not in active_loggers:
         logger.setLevel(log_level)
         if log_file:  # if present means: "please add this file as logs storage for my logger"
             _add_new_file_handler(
@@ -804,44 +806,58 @@
         raw_formatter = RawDataFormatter()
         self.setFormatter(raw_formatter)
         self.setLevel(RAW_DATA)
         raw_records_only_filter = SpecificLevelFilter(RAW_DATA)
         self.addFilter(raw_records_only_filter)
 
     def emit(self, record):
-        """
+        r"""
         Emit a record.
-        We don't want base class implementation since we don't want to do:
-        stream.write(self.terminator)
-        We are not adding any \n to bytes-message from record.
+
+
+        ::
+
+
+            We don't want the base class implementation since we don't want to include
+            stream.write(self.terminator)
+            We are not adding any newline character (\n) to the bytes message
+            from the record.
+
+
         """
         if self.stream is None:
             self.stream = self._open()
         try:
             msg = self.format(record)
             stream = self.stream
             stream.write(msg)
             self.flush()
         except Exception:
             self.handleError(record)
 
 
 class MultilineWithDirectionFormatter(logging.Formatter):
     """
-    We want logs to have non-overlapping areas
-    timestamp area TTTTTTTTTTT
-    transfer direction area >  (shows send '>' or receive '<')
-    log message area MMMMMMMMMM
-    It should look like:
-    TTTTTTTTTTTTTTT D MMMMMMMMMMMMMMM
-    01 00:36:09.581 >|cat my_file.txt
-    01 00:36:09.585 <|This is
-                     |multiline
-                     |content
-    This formatter allows to use %(transfer_direction)s inside format
+    We want logs to have non-overlapping areas.
+
+
+    ::
+
+
+        Timestamp area TTTTTTTTTTT
+        transfer direction area >  (shows send '>' or receive '<')
+        log message area MMMMMMMMMM
+        It should look like:
+
+        TTTTTTTTTTTTTTT D MMMMMMMMMMMMMMM
+        01 00:36:09.581 >|cat my_file.txt
+        01 00:36:09.585 <|This is
+                        |multiline
+                        |content
+        This formatter allows to use %(transfer_direction)s inside format.
     """
 
     def __init__(self, fmt=None, datefmt=None):
         if fmt is None:
             fmt = "%(asctime)s.%(msecs)03d %(transfer_direction)s|%(message)s"
         else:  # message should be last part of format
             assert fmt.endswith("|%(message)s")
```

### Comparing `moler-3.4.0/moler/config/runners.py` & `moler-3.5.0/moler/config/runners.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/connection.py` & `moler-3.5.0/moler/connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/connection_factory.py` & `moler-3.5.0/moler/connection_factory.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/connection_observer.py` & `moler-3.5.0/moler/connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/device/abstract_device.py` & `moler-3.5.0/moler/device/abstract_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         :param state: name of state to go.
         :param timeout: Time in seconds when break transitions if still not success.
         :param rerun: How many times try to rerun command(s) when device is still not in requested state.
         :param send_enter_after_changed_state: Set True to send enter after enters proper state.
         :param log_stacktrace_on_fail: Set True to log exceptions if command to enter state failed.
         :param keep_state: if True and state is changed without goto_state then device tries to change state to state
-        defined by goto_state.
+         defined by goto_state.
         :return: None
         """
 
     @abc.abstractmethod
     def establish_connection(self):
         """
         Establishes connection to real device.
```

### Comparing `moler-3.4.0/moler/device/adbremote.py` & `moler-3.5.0/moler/device/adbremote.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,36 +20,40 @@
 
 
 @call_base_class_method_with_same_name
 class AdbRemote(UnixRemote):
     r"""
     AdbRemote device class.
 
-    Example of device in yaml configuration file:
-    -without PROXY_PC:
-      ADB_1:
-       DEVICE_CLASS: moler.device.adbremote.AdbRemote
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-      UNIX_REMOTE:
-        ADB_SHELL:
-          execute_command: adb_shell # default value; default command is:  adb shell
-          command_params:
-            serial_number: 'f57e6b7d'  #  to create:  adb -s f57e6b7d shell
-            expected_prompt: 'shell@adbhost: $'
-      ADB_SHELL:
-        UNIX_REMOTE:
-          execute_command: exit # default value
+
+    ::
+
+
+        Example of device in yaml configuration file:
+        -without PROXY_PC:
+            ADB_1:
+            DEVICE_CLASS: moler.device.adbremote.AdbRemote
+            CONNECTION_HOPS:
+                UNIX_LOCAL:
+                UNIX_REMOTE:
+                    execute_command: ssh # default value
+                    command_params:
+                    expected_prompt: unix_remote_prompt
+                    host: host_ip
+                    login: login
+                    password: password
+            UNIX_REMOTE:
+            ADB_SHELL:
+                execute_command: adb_shell # default value; default command is:  adb shell
+                command_params:
+                serial_number: 'f57e6b7d'  #  to create:  adb -s f57e6b7d shell
+                expected_prompt: 'shell@adbhost: $'
+            ADB_SHELL:
+            UNIX_REMOTE:
+                execute_command: exit # default value
     """
 
     adb_shell = "ADB_SHELL"
     adb_shell_root = "ADB_SHELL_ROOT"
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
```

### Comparing `moler-3.4.0/moler/device/adbremote2.py` & `moler-3.5.0/moler/device/adbremote2.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,97 +29,101 @@
 
 
 @call_base_class_method_with_same_name
 class AdbRemote2(UnixRemote2):
     r"""
     AdbRemote device class.
 
-    Example of device in yaml configuration file:
 
-    - with PROXY_PC and io "terminal":
-      ADB_1:
-       DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           PROXY_PC:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: proxy_pc_prompt
-               host: host_ip
-               login: login
-               password: password
-         PROXY_PC:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-         UNIX_REMOTE:
-           ADB_SHELL:
-             execute_command: adb_shell # default value
-             command_params:
-               serial_number: 'f57e6b7d'
-
-    - with PROXY_PC and remote-access-io like "sshshell":
-      ADB_1:
-       DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
-       CONNECTION_DESC:
-         io_type: sshshell
-         host: host_ip
-         login: login
-         password: password
-       CONNECTION_HOPS:
-         PROXY_PC:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-         UNIX_REMOTE:
-           ADB_SHELL:
-             execute_command: adb_shell # default value
-             command_params:
-               serial_number: 'f57e6b7d'
-
-    -without PROXY_PC and io "terminal":
-      ADB_1:
-       DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-         UNIX_REMOTE:
-           ADB_SHELL:
-             execute_command: adb_shell # default value
-             command_params:
-               serial_number: 'f57e6b7d'
-
-    -without PROXY_PC and remote-access-io like "sshshell":
-      ADB_1:
-       DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
-       CONNECTION_DESC:
-         io_type: sshshell
-         host: host_ip
-         login: login
-         password: password
-       CONNECTION_HOPS:
-         UNIX_REMOTE:
-           ADB_SHELL:
-             execute_command: adb_shell # default value
-             command_params:
-               serial_number: 'f57e6b7d'
+    ::
+
+
+        Example of device in yaml configuration file:
+
+        - with PROXY_PC and io "terminal":
+        ADB_1:
+        DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
+        CONNECTION_HOPS:
+            UNIX_LOCAL:
+            PROXY_PC:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: proxy_pc_prompt
+                host: host_ip
+                login: login
+                password: password
+            PROXY_PC:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
+            UNIX_REMOTE:
+            ADB_SHELL:
+                execute_command: adb_shell # default value
+                command_params:
+                serial_number: 'f57e6b7d'
+
+        - with PROXY_PC and remote-access-io like "sshshell":
+        ADB_1:
+        DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
+        CONNECTION_DESC:
+            io_type: sshshell
+            host: host_ip
+            login: login
+            password: password
+        CONNECTION_HOPS:
+            PROXY_PC:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
+            UNIX_REMOTE:
+            ADB_SHELL:
+                execute_command: adb_shell # default value
+                command_params:
+                serial_number: 'f57e6b7d'
+
+        -without PROXY_PC and io "terminal":
+        ADB_1:
+        DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
+        CONNECTION_HOPS:
+            UNIX_LOCAL:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
+            UNIX_REMOTE:
+            ADB_SHELL:
+                execute_command: adb_shell # default value
+                command_params:
+                serial_number: 'f57e6b7d'
+
+        -without PROXY_PC and remote-access-io like "sshshell":
+        ADB_1:
+        DEVICE_CLASS: moler.device.adbremote2.AdbRemote2
+        CONNECTION_DESC:
+            io_type: sshshell
+            host: host_ip
+            login: login
+            password: password
+        CONNECTION_HOPS:
+            UNIX_REMOTE:
+            ADB_SHELL:
+                execute_command: adb_shell # default value
+                command_params:
+                serial_number: 'f57e6b7d'
     """
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
         """
         Create ADB device communicating over io_connection
         :param sm_params: dict with parameters of state machine for device
```

### Comparing `moler-3.4.0/moler/device/atremote.py` & `moler-3.5.0/moler/device/atremote.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,35 +18,39 @@
 
 
 @call_base_class_method_with_same_name
 class AtRemote(UnixRemote):
     r"""
     AtRemote device class.
 
-    Example of device in yaml configuration file:
-    -without PROXY_PC:
-      AT_1:
-       DEVICE_CLASS: moler.device.atremote.AtRemote
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-      UNIX_REMOTE:
-        AT_REMOTE:
-          execute_command: plink_serial # default value
-          command_params:
-            serial_devname: 'COM5'
-      AT_REMOTE:
+
+    ::
+
+
+        Example of device in yaml configuration file:
+        -without PROXY_PC:
+        AT_1:
+        DEVICE_CLASS: moler.device.atremote.AtRemote
+        CONNECTION_HOPS:
+            UNIX_LOCAL:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
         UNIX_REMOTE:
-          execute_command: ctrl_c # default value
+            AT_REMOTE:
+            execute_command: plink_serial # default value
+            command_params:
+                serial_devname: 'COM5'
+        AT_REMOTE:
+            UNIX_REMOTE:
+            execute_command: ctrl_c # default value
     """
 
     at_remote = "AT_REMOTE"
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
         """
```

### Comparing `moler-3.4.0/moler/device/device.py` & `moler-3.5.0/moler/device/device.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/device/juniper_ex.py` & `moler-3.5.0/moler/device/juniper_ex.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,44 +12,48 @@
 
 
 @call_base_class_method_with_same_name
 class JuniperEX(JuniperGeneric):
     r"""
     Juniperex device class.
 
-    Example of device in yaml configuration file:
-    - with PROXY_PC:
-      JUNIPER_EX_PROXY_PC:
-        DEVICE_CLASS: moler.device.juniper_ex.JuniperEX
-        CONNECTION_HOPS:
-          PROXY_PC:
-            CLI:
-              execute_command: ssh
-              command_params:
-                host: cli_host
-                login: cli_login
-                password: password
-          UNIX_LOCAL:
-            PROXY_PC:
-              execute_command: ssh
-              command_params:
-                expected_prompt: "proxy_pc#"
-                host: proxy_pc_host
-                login: proxy_pc_login
-                password: password
-          CLI:
+
+    ::
+
+
+      Example of device in yaml configuration file:
+      - with PROXY_PC:
+        JUNIPER_EX_PROXY_PC:
+          DEVICE_CLASS: moler.device.juniper_ex.JuniperEX
+          CONNECTION_HOPS:
             PROXY_PC:
-              execute_command: exit
-              command_params:
-                expected_prompt: "proxy_pc#"
-    - without PROXY_PC:
-      JUNIPER_EX:
-        DEVICE_CLASS: moler.device.juniper_ex.JuniperEX
-        CONNECTION_HOPS:
-          UNIX_LOCAL:
+              CLI:
+                execute_command: ssh
+                command_params:
+                  host: cli_host
+                  login: cli_login
+                  password: password
+            UNIX_LOCAL:
+              PROXY_PC:
+                execute_command: ssh
+                command_params:
+                  expected_prompt: "proxy_pc#"
+                  host: proxy_pc_host
+                  login: proxy_pc_login
+                  password: password
             CLI:
-              execute_command: ssh # default value
-              command_params:
-                host: cli_host
-                login: cli_login
-                password: password
+              PROXY_PC:
+                execute_command: exit
+                command_params:
+                  expected_prompt: "proxy_pc#"
+      - without PROXY_PC:
+        JUNIPER_EX:
+          DEVICE_CLASS: moler.device.juniper_ex.JuniperEX
+          CONNECTION_HOPS:
+            UNIX_LOCAL:
+              CLI:
+                execute_command: ssh # default value
+                command_params:
+                  host: cli_host
+                  login: cli_login
+                  password: password
     """
```

### Comparing `moler-3.4.0/moler/device/junipergeneric.py` & `moler-3.5.0/moler/device/junipergeneric.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/device/pdu_aten.py` & `moler-3.5.0/moler/device/pdu_aten.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,46 +14,50 @@
 
 
 @call_base_class_method_with_same_name
 class PduAten(ProxyPc):
     r"""
     PDU Aten device class.
 
-    Example of device in yaml configuration file:
-    - with PROXY_PC:
-      PDU_1:
-        DEVICE_CLASS: moler.device.pdu_aten.PduAten
-        CONNECTION_HOPS:
-          PROXY_PC:
-            PDU:
-              execute_command: telnet # default value
-              command_params:
-                host: 10.0.0.1
-          PDU:
-            PROXY_PC:
-              execute_command: exit_telnet # default value
-              command_params:
-                expected_prompt: proxy_pc.*>
-          UNIX_LOCAL:
-            PROXY_PC:
-              execute_command: ssh # default value
-              command_params:
-                expected_prompt: proxy_pc.*>
-                host: 10.0.0.2
-                login: user
-                password: password
-    -without PROXY_PC:
+
+    ::
+
+
+        Example of device in yaml configuration file:
+        - with PROXY_PC:
         PDU_1:
             DEVICE_CLASS: moler.device.pdu_aten.PduAten
             CONNECTION_HOPS:
-              UNIX_LOCAL:
+            PROXY_PC:
                 PDU:
-                  execute_command: telnet # default value
-                  command_params:
+                execute_command: telnet # default value
+                command_params:
                     host: 10.0.0.1
+            PDU:
+                PROXY_PC:
+                execute_command: exit_telnet # default value
+                command_params:
+                    expected_prompt: proxy_pc.*>
+            UNIX_LOCAL:
+                PROXY_PC:
+                execute_command: ssh # default value
+                command_params:
+                    expected_prompt: proxy_pc.*>
+                    host: 10.0.0.2
+                    login: user
+                    password: password
+        -without PROXY_PC:
+            PDU_1:
+                DEVICE_CLASS: moler.device.pdu_aten.PduAten
+                CONNECTION_HOPS:
+                UNIX_LOCAL:
+                    PDU:
+                    execute_command: telnet # default value
+                    command_params:
+                        host: 10.0.0.1
     """
 
     pdu = "PDU"
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
         """
```

### Comparing `moler-3.4.0/moler/device/proxy_pc.py` & `moler-3.5.0/moler/device/proxy_pc.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/device/proxy_pc2.py` & `moler-3.5.0/moler/device/proxy_pc2.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 
 @six.add_metaclass(abc.ABCMeta)
 class ProxyPc2(UnixLocal):
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
         """
-        Create Unix device communicating over io_connection
+        Create Unix device communicating over io_connection.
+
         :param sm_params: dict with parameters of state machine for device
         :param name: name of device
         :param io_connection: External-IO connection having embedded moler-connection
         :param io_type: type of connection - tcp, udp, ssh, telnet, ...
         :param variant: connection implementation variant, ex. 'threaded', 'twisted', 'asyncio', ...
                         (if not given then default one is taken)
         :param io_constructor_kwargs: additional parameter into constructor of selected connection type
@@ -432,14 +433,15 @@
                 return available[observer]
 
         return available
 
     def get_cmd(self, cmd_name, cmd_params=None, check_state=True, for_state=None):
         """
         Returns instance of command connected with the device.
+
         :param cmd_name: name of commands, name of class (without package), for example "cd".
         :param cmd_params: dict with command parameters.
         :param check_state: if True then before execute of command the state of device will be check if the same
          as when command was created. If False the device state is not checked.
         :param for_state: if None then command object for current state is returned, otherwise object for for_state is
          returned.
         :return: Instance of command
```

### Comparing `moler-3.4.0/moler/device/scpi.py` & `moler-3.5.0/moler/device/scpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,50 +14,54 @@
 
 
 @call_base_class_method_with_same_name
 class Scpi(ProxyPc):
     r"""
     Scpi device class.
 
-    Example of device in yaml configuration file:
-    - with PROXY_PC:
-        SCPI_1:
-        DEVICE_CLASS: moler.device.scpi.Scpi
-        CONNECTION_HOPS:
-          PROXY_PC:
-            SCPI:
-              execute_command: telnet # default value
-              command_params:
-                expected_prompt: SCPI>
-                host: 10.0.0.1
-                port: 99999
-          SCPI:
-            PROXY_PC:
-              execute_command: exit_telnet # default value
-              command_params:
-                expected_prompt: proxy_pc.*>
-          UNIX_LOCAL:
-            PROXY_PC:
-              execute_command: ssh # default value
-              command_params:
-                expected_prompt: proxy_pc.*>
-                host: 10.0.0.2
-                login: user
-                password: password
-    -without PROXY_PC:
-        SCPI_1:
+
+    ::
+
+
+        Example of device in yaml configuration file:
+        - with PROXY_PC:
+            SCPI_1:
             DEVICE_CLASS: moler.device.scpi.Scpi
             CONNECTION_HOPS:
-              UNIX_LOCAL:
+            PROXY_PC:
                 SCPI:
-                  execute_command: telnet # default value
-                  command_params:
+                execute_command: telnet # default value
+                command_params:
                     expected_prompt: SCPI>
                     host: 10.0.0.1
                     port: 99999
+            SCPI:
+                PROXY_PC:
+                execute_command: exit_telnet # default value
+                command_params:
+                    expected_prompt: proxy_pc.*>
+            UNIX_LOCAL:
+                PROXY_PC:
+                execute_command: ssh # default value
+                command_params:
+                    expected_prompt: proxy_pc.*>
+                    host: 10.0.0.2
+                    login: user
+                    password: password
+        -without PROXY_PC:
+            SCPI_1:
+                DEVICE_CLASS: moler.device.scpi.Scpi
+                CONNECTION_HOPS:
+                UNIX_LOCAL:
+                    SCPI:
+                    execute_command: telnet # default value
+                    command_params:
+                        expected_prompt: SCPI>
+                        host: 10.0.0.1
+                        port: 99999
     """
 
     scpi = "SCPI"
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None,
                  io_constructor_kwargs=None, initial_state=None, lazy_cmds_events=False):
         """
```

### Comparing `moler-3.4.0/moler/device/state_machine.py` & `moler-3.5.0/moler/device/state_machine.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/device/textualdevice.py` & `moler-3.5.0/moler/device/textualdevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,23 +432,23 @@
         rerun=0,
         send_enter_after_changed_state=False,
         log_stacktrace_on_fail=True,
         keep_state=False,
         timeout_multiply=1.0,
     ):
         """
-        Goes to specific state.
+        Go to specific state.
 
         :param state: Name to state to change on the device.
         :param timeout: Timeout for changing state, if negative then timeout from commands are taken.
         :param rerun: How many times rerun the procedure before it fails.
         :param send_enter_after_changed_state: If True then enter is sent after state is changed. False nothing is sent.
         :param log_stacktrace_on_fail: Set True to have stacktrace in logs when failed, otherwise False.
         :param keep_state: if True and state is changed without goto_state then device tries to change state to state
-        defined by goto_state.
+         defined by goto_state.
         :param timeout_multiply: how many times multiply passed timeout to get final timeout.
         :return: None
         :raise: DeviceChangeStateFailure if cannot change the state of device.
         """
         self._kept_state = None
         if not self.has_established_connection():
             self.establish_connection()
@@ -873,15 +873,16 @@
                     raise exc
 
             observer._validate_start = validate_device_state_before_observer_start  # pylint: disable=protected-access
         return observer
 
     def get_cmd(self, cmd_name, cmd_params=None, check_state=True, for_state=None):
         """
-        Returns instance of command connected with the device.
+        Return instance of command connected with the device.
+
         :param cmd_name: name of commands, name of class (without package), for example "cd".
         :param cmd_params: dict with command parameters.
         :param check_state: if True then before execute of command the state of device will be check if the same
          as when command was created. If False the device state is not checked.
         :param for_state: if None then command object for current state is returned, otherwise object for for_state is
          returned.
         :return: Instance of command
@@ -902,14 +903,15 @@
         return cmd
 
     def get_event(
         self, event_name, event_params=None, check_state=True, for_state=None
     ):
         """
         Return instance of event connected with the device.
+
         :param event_name: name of event, name of class (without package).
         :param event_params: dict with event parameters.
         :param check_state: if True then before execute of event the state of device will be check if the same
          as when event was created. If False the device state is not checked.
         :param for_state: if None then event object for current state is returned, otherwise object for for_state is
          returned.
         :return: Event object
```

### Comparing `moler-3.4.0/moler/device/unixlocal.py` & `moler-3.5.0/moler/device/unixlocal.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 
 
 # TODO: name, logger/logger_name as param
 class UnixLocal(TextualDevice):
     r"""
     UnixLocal device class.
 
-    Example of device in yaml configuration file:
-    UNIX_1:
-        DEVICE_CLASS: moler.device.unixlocal.UnixLocal
-
-    UNIX_2:
-        DEVICE_CLASS: moler.device.unixlocal.UnixLocal
-        'CONNECTION_HOPS': {
-                    'UNIX_LOCAL': {
-                        'UNIX_LOCAL_ROOT': {
-                            "command_params": {
-                                "password": "root_password",
-                                "expected_prompt": r'local_root_prompt',
+
+    ::
+
+
+        Example of device in yaml configuration file:
+        UNIX_1:
+            DEVICE_CLASS: moler.device.unixlocal.UnixLocal
+
+        UNIX_2:
+            DEVICE_CLASS: moler.device.unixlocal.UnixLocal
+            'CONNECTION_HOPS': {
+                        'UNIX_LOCAL': {
+                            'UNIX_LOCAL_ROOT': {
+                                "command_params": {
+                                    "password": "root_password",
+                                    "expected_prompt": r'local_root_prompt',
+                                }
                             }
                         }
                     }
-                }
+
 
     """
 
     unix_local = "UNIX_LOCAL"
     unix_local_root = "UNIX_LOCAL_ROOT"
 
     def __init__(
```

### Comparing `moler-3.4.0/moler/device/unixremote.py` & `moler-3.5.0/moler/device/unixremote.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,52 +14,58 @@
 
 
 @call_base_class_method_with_same_name
 class UnixRemote(ProxyPc):
     r"""
     UnixRemote device class.
 
-    Example of device in yaml configuration file:
-    - with PROXY_PC:
-      UNIX_1:
-       DEVICE_CLASS: moler.device.unixremote.UnixRemote
-       CONNECTION_HOPS:
-         PROXY_PC:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-         UNIX_REMOTE:
-           PROXY_PC:
-             execute_command: exit # default value
-             command_params:
-               expected_prompt: proxy_pc_prompt
-         UNIX_LOCAL:
-           PROXY_PC:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: proxy_pc_prompt
-               host: host_ip
-               login: login
-               password: password
-    -without PROXY_PC:
-      UNIX_1:
-       DEVICE_CLASS: moler.device.unixremote.UnixRemote
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
+
+    ::
+
+
+            Example of device in yaml configuration file:
+            - with PROXY_PC:
+            UNIX_1:
+            DEVICE_CLASS: moler.device.unixremote.UnixRemote
+            CONNECTION_HOPS:
+                PROXY_PC:
+                UNIX_REMOTE:
+                    execute_command: ssh # default value
+                    command_params:
+                    expected_prompt: unix_remote_prompt
+                    host: host_ip
+                    login: login
+                    password: password
+                UNIX_REMOTE:
+                PROXY_PC:
+                    execute_command: exit # default value
+                    command_params:
+                    expected_prompt: proxy_pc_prompt
+                UNIX_LOCAL:
+                PROXY_PC:
+                    execute_command: ssh # default value
+                    command_params:
+                    expected_prompt: proxy_pc_prompt
+                    host: host_ip
+                    login: login
+                    password: password
+            -without PROXY_PC:
+            UNIX_1:
+            DEVICE_CLASS: moler.device.unixremote.UnixRemote
+            CONNECTION_HOPS:
+                UNIX_LOCAL:
+                UNIX_REMOTE:
+                    execute_command: ssh # default value
+                    command_params:
+                    expected_prompt: unix_remote_prompt
+                    host: host_ip
+                    login: login
+                    password: password
+
+
     """
 
     unix_remote = "UNIX_REMOTE"
     unix_remote_root = "UNIX_REMOTE_ROOT"
 
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
```

### Comparing `moler-3.4.0/moler/device/unixremote2.py` & `moler-3.5.0/moler/device/unixremote2.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,75 +28,82 @@
 
 @call_base_class_method_with_same_name
 class UnixRemote2(ProxyPc2):
     r"""
     UnixRemote2 device class.
 
     Example of device in yaml configuration file:
-    - with PROXY_PC and io "terminal":
-      UNIX_1:
-       DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           PROXY_PC:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: proxy_pc_prompt
-               host: host_ip
-               login: login
-               password: password
-         PROXY_PC:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-
-    - with PROXY_PC and remote-access-io like "sshshell":
-      UNIX_1:
-       DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
-       CONNECTION_DESC:
-         io_type: sshshell
-         host: host_ip
-         login: login
-         password: password
-       CONNECTION_HOPS:
-         PROXY_PC:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-
-    -without PROXY_PC and io "terminal":
-      UNIX_1:
-       DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
-       CONNECTION_HOPS:
-         UNIX_LOCAL:
-           UNIX_REMOTE:
-             execute_command: ssh # default value
-             command_params:
-               expected_prompt: unix_remote_prompt
-               host: host_ip
-               login: login
-               password: password
-
-    -without PROXY_PC and remote-access-io like "sshshell":
-      UNIX_1:
-       DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
-       CONNECTION_DESC:
-         io_type: sshshell
-         host: host_ip
-         login: login
-         password: password
-       (no need for CONNECTION_HOPS since we jump directly from NOT_CONNECTED to UNIX_REMOTE using sshshell)
+
+
+    ::
+
+
+        - with PROXY_PC and io "terminal":
+        UNIX_1:
+        DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
+        CONNECTION_HOPS:
+            UNIX_LOCAL:
+            PROXY_PC:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: proxy_pc_prompt
+                host: host_ip
+                login: login
+                password: password
+            PROXY_PC:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
+
+        - with PROXY_PC and remote-access-io like "sshshell":
+        UNIX_1:
+        DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
+        CONNECTION_DESC:
+            io_type: sshshell
+            host: host_ip
+            login: login
+            password: password
+        CONNECTION_HOPS:
+            PROXY_PC:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
+
+        -without PROXY_PC and io "terminal":
+        UNIX_1:
+        DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
+        CONNECTION_HOPS:
+            UNIX_LOCAL:
+            UNIX_REMOTE:
+                execute_command: ssh # default value
+                command_params:
+                expected_prompt: unix_remote_prompt
+                host: host_ip
+                login: login
+                password: password
+
+        -without PROXY_PC and remote-access-io like "sshshell":
+        UNIX_1:
+        DEVICE_CLASS: moler.device.unixremote2.UnixRemote2
+        CONNECTION_DESC:
+            io_type: sshshell
+            host: host_ip
+            login: login
+            password: password
+        (no need for CONNECTION_HOPS since we jump directly from NOT_CONNECTED to UNIX_REMOTE using sshshell)
+
+
     """
     def __init__(self, sm_params, name=None, io_connection=None, io_type=None, variant=None, io_constructor_kwargs=None,
                  initial_state=None, lazy_cmds_events=False):
         """
         Create Unix device communicating over io_connection
         :param sm_params: dict with parameters of state machine for device
         :param name: name of device
```

### Comparing `moler-3.4.0/moler/event.py` & `moler-3.5.0/moler/event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 
 __author__ = "Michal Ernst, Marcin Usielski"
-__copyright__ = "Copyright (C) 2018-2020, Nokia"
+__copyright__ = "Copyright (C) 2018-2024, Nokia"
 __email__ = "michal.ernst@nokia.com, marcin.usielski@nokia.com"
 
 import abc
 import functools
 import logging
-
+from typing import Optional
 import six
 
+from moler.abstract_moler_connection import AbstractMolerConnection
+from moler.runner import ConnectionObserverRunner
 from moler.connection_observer import ConnectionObserver
 from moler.exceptions import MolerException, ResultAlreadySet
 from moler.helpers import instance_id
 
 
 @six.add_metaclass(abc.ABCMeta)
 class Event(ConnectionObserver):
-    def __init__(self, connection=None, till_occurs_times=-1, runner=None):
+    def __init__(self, connection: Optional[AbstractMolerConnection] = None, till_occurs_times: int = -1, runner: Optional[ConnectionObserverRunner] = None):
         """
 
         :param connection: connection to observe.
         :param till_occurs_times: If -1 then infinite. If positive value match the number of times.
         :param runner: runner to run event.
         """
         super(Event, self).__init__(connection=connection, runner=runner)
@@ -40,15 +42,15 @@
         Returns description of event object.
 
         :return: String representation of event.
         """
         return f"{self.__class__.__name__}(id:{instance_id(self)})"
 
     # pylint: disable=keyword-arg-before-vararg
-    def start(self, timeout=None, *args, **kwargs):
+    def start(self, timeout: float = None, *args, **kwargs):
         """Start background execution of command."""
         self._validate_start(*args, **kwargs)
         ret = super(Event, self).start(timeout, *args, **kwargs)
         self.life_status._is_running = True  # pylint: disable=protected-access
         return ret
 
     def add_event_occurred_callback(self, callback, callback_params=None):
@@ -58,77 +60,85 @@
             partial_callback = functools.partial(callback, **callback_params)
             self.callback = partial_callback
         else:
             raise MolerException(
                 f"Cannot assign a callback '{callback}' to event '{self}' when another callback '{self.callback}' is already assigned"
             )
 
-    def enable_log_occurrence(self):
+    def enable_log_occurrence(self) -> None:
         """
         Enables to log every occurrence of the event.
 
         :return: None
         """
         self._log_every_occurrence = True
 
-    def disable_log_occurrence(self):
+    def disable_log_occurrence(self) -> None:
         """
         Disables to log every occurrence of the event.
 
         :return: None
         """
         self._log_every_occurrence = False
 
-    def remove_event_occurred_callback(self):
+    def remove_event_occurred_callback(self) -> None:
         """
         Removes callback from the event.
 
         :return: None
         """
         self.callback = None
 
-    def notify(self):
+    def notify(self) -> None:
         """
         Notifies (call callback).
 
         :return: None
         """
         self._log_occurred()
         if self.callback:
             self.callback()
 
-    def event_occurred(self, event_data):
+    def event_occurred(self, event_data) -> None:
         """
         Sets event_data as new item of occurrence ret.
         :param event_data: data to set as value of occurrence.
         :return: None
         """
         # Should be used to set final result of event.
         if self.done():
             raise ResultAlreadySet(self)
-        if self._occurred is None:
-            self._occurred = []
+        self._prepare_result_from_occurred()
         self._occurred.append(event_data)
         if self.till_occurs_times > 0:
             if len(self._occurred) >= self.till_occurs_times:
-                self.set_result(self._occurred)
+                self.break_event()
         self.notify()
 
-    def _get_module_class(self):
+    def _prepare_result_from_occurred(self) -> None:
+        """
+        Prepare result from occurred.
+
+        :return: None.
+        """
+        if self._occurred is None:
+            self._occurred = []
+
+    def _get_module_class(self) -> str:
         return f"{self.__class__.__module__}.{self}"
 
-    def get_long_desc(self):
+    def get_long_desc(self) -> str:
         """
         Returns string with description of event.
 
         :return: String with description.
         """
         return f"Event '{self._get_module_class()}'"
 
-    def get_short_desc(self):
+    def get_short_desc(self) -> str:
         """
         Returns string with description of event.
 
         :return: String with description.
         """
         return self.get_long_desc()
 
@@ -139,15 +149,29 @@
         :return: ret value form last occurrence or None if there is no occurrence.
         """
         if self._occurred:
             return self._occurred[-1]
         else:
             return None
 
-    def _log_occurred(self):
+    def break_event(self, force=False) -> None:
+        """
+        Break event. Do not process anymore. Clean up all resources. Prepare result.
+
+        :param force: If False then check if no of occurred is as expected Force, True to not check.
+        :return: None.
+        """
+        if not self.done():
+            self._prepare_result_from_occurred()
+            if not force and len(self._occurred) < self.till_occurs_times:
+                self.set_exception(MolerException(f"Expected {self.till_occurs_times} occurrences but got {len(self._occurred)}."))
+            else:
+                self.set_result(self._occurred)
+
+    def _log_occurred(self) -> None:
         """
         Logs info about notify when callback is not defined.
 
         :return: None
         """
         msg = f"Notify for event:  '{self.__class__.__module__}.{self}'"
         if self._log_every_occurrence:
@@ -155,21 +179,21 @@
         if self.callback:
             msg = f"{msg} with callback '{self.callback}'."
         else:
             msg = f"{msg} without callback."
         self._log(lvl=logging.DEBUG, msg=msg)
 
     @abc.abstractmethod
-    def pause(self):
+    def pause(self) -> None:
         """
         Pauses the event. Do not process till resume.
 
         :return: None.
         """
 
     @abc.abstractmethod
-    def resume(self):
+    def resume(self) -> None:
         """
         Resumes processing output from connection by the event.
 
         :return: None.
         """
```

### Comparing `moler-3.4.0/moler/event_awaiter.py` & `moler-3.5.0/moler/event_awaiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         Example 1:
             cmds = [cmd1, cmd2, cmd3]
             events = [event1, (event2, event3), event4]
 
         Example 2:
             cmds = [(cmd1, cmd2), cmd3, cmd4]
             events = [event1, event2]
+
         :param cmds: A list of commands to start.
         :param events: A list of events to start. If None, then the next command is started immediately.
         :param event_timeout: Timeout for each event.
         :param sleep_after_event: Time to sleep after every event.
         :return: None
         """
         events_cp = copy_list(events, deep_copy=False)
```

### Comparing `moler-3.4.0/moler/events/juniper/genericshared_lineevent.py` & `moler-3.5.0/moler/events/juniper/genericshared_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py` & `moler-3.5.0/moler/events/juniper_ex/genericjuniper_ex_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/lineevent.py` & `moler-3.5.0/moler/events/lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/scpi/genericscpi_lineevent.py` & `moler-3.5.0/moler/events/scpi/genericscpi_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/shared/genericshared_lineevent.py` & `moler-3.5.0/moler/events/shared/genericshared_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/shared/genericshared_textualevent.py` & `moler-3.5.0/moler/events/shared/genericshared_textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/shared/password_prompt.py` & `moler-3.5.0/moler/events/shared/password_prompt.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/shared/wait4.py` & `moler-3.5.0/moler/events/shared/wait4.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/textualevent.py` & `moler-3.5.0/moler/events/textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/advise_to_change_your_password.py` & `moler-3.5.0/moler/events/unix/advise_to_change_your_password.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/failed_login_counter.py` & `moler-3.5.0/moler/events/unix/failed_login_counter.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/genericunix_lineevent.py` & `moler-3.5.0/moler/events/unix/genericunix_lineevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/genericunix_textualevent.py` & `moler-3.5.0/moler/events/unix/genericunix_textualevent.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/last_failed_login.py` & `moler-3.5.0/moler/events/unix/last_failed_login.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/last_login.py` & `moler-3.5.0/moler/events/unix/last_login.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/ping_no_response.py` & `moler-3.5.0/moler/events/unix/ping_no_response.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/ping_response.py` & `moler-3.5.0/moler/events/unix/ping_response.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/private_system.py` & `moler-3.5.0/moler/events/unix/private_system.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/shutdown.py` & `moler-3.5.0/moler/events/unix/shutdown.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/u_boot_crtm.py` & `moler-3.5.0/moler/events/unix/u_boot_crtm.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 from moler.events.unix.genericunix_textualevent import GenericUnixTextualEvent
 from moler.exceptions import ParsingDone
 
 
 class UBootCrtm(GenericUnixTextualEvent):
     def __init__(self, connection, till_occurs_times=-1, runner=None):
         """
-        Event for 'Site is resetting due to Fault'
+        Event for 'Site is resetting due to Fault'.
+
         :param connection: moler connection to device, terminal when command is executed
         :param till_occurs_times: number of event occurrence
         :param runner: Runner to run event
         """
         super(UBootCrtm, self).__init__(
             connection=connection, runner=runner, till_occurs_times=till_occurs_times
         )
         self.current_ret = {}
 
     def on_new_line(self, line, is_full_line):
         """
-         Put your parsing code here.
+        Put your parsing code here.
+
         :param line: Line to process, can be only part of line. New line chars are removed from line.
         :param is_full_line: True if line had new line chars, False otherwise
         :return: None
         """
         if is_full_line:
             try:
                 self._parse_u_boot_crtm(line)
```

### Comparing `moler-3.4.0/moler/events/unix/wait4prompt.py` & `moler-3.5.0/moler/events/unix/wait4prompt.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/wait4prompts.py` & `moler-3.5.0/moler/events/unix/wait4prompts.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/events/unix/warning_default_password.py` & `moler-3.5.0/moler/events/unix/warning_default_password.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/exceptions.py` & `moler-3.5.0/moler/exceptions.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/helpers.py` & `moler-3.5.0/moler/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,17 @@
     return line
 
 
 # ESC [ ? 12 h   Start the cursor blinking
 # ESC [ ? 12 l   Stop blinking the cursor
 # ESC [ ? 25 h   Show the cursor
 # ESC [ ? 25 l   Show the cursor
-_re_cursor_visibility_codes = re.compile(r"\x1B\[\?(12|25)[hl]")
+# ESC [ ? 2004 l Control sequence odd character
+# ESC [ ? 2004 h Control sequence odd character
+_re_cursor_visibility_codes = re.compile(r"\x1B\[\?(12|25|2004)[hl]")
 
 
 def remove_cursor_visibility_codes(multiline):
     """
     :param multiline: string from terminal holding single or multiple lines
     :return: line(s) without terminal escape codes related to cursor visibility
     """
```

### Comparing `moler-3.4.0/moler/instance_loader.py` & `moler-3.5.0/moler/instance_loader.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/asyncio/__init__.py` & `moler-3.5.0/moler/io/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/asyncio/tcp.py` & `moler-3.5.0/moler/io/asyncio/tcp.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/asyncio/terminal.py` & `moler-3.5.0/moler/io/asyncio/terminal.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/io_connection.py` & `moler-3.5.0/moler/io/io_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/io_exceptions.py` & `moler-3.5.0/moler/io/io_exceptions.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/__init__.py` & `moler-3.5.0/moler/io/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/memory.py` & `moler-3.5.0/moler/io/raw/memory.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/sshshell.py` & `moler-3.5.0/moler/io/raw/sshshell.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/subprocess.py` & `moler-3.5.0/moler/io/raw/subprocess.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/tcp.py` & `moler-3.5.0/moler/io/raw/tcp.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/tcpserverpiped.py` & `moler-3.5.0/moler/io/raw/tcpserverpiped.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/io/raw/terminal.py` & `moler-3.5.0/moler/io/raw/terminal.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/moler_connection_for_single_thread_runner.py` & `moler-3.5.0/moler/moler_connection_for_single_thread_runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/observable_connection.py` & `moler-3.5.0/moler/observable_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/observer_thread_wrapper.py` & `moler-3.5.0/moler/observer_thread_wrapper.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/parser/table_text.py` & `moler-3.5.0/moler/parser/table_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Last modification: adding support for EPC tables and partially empty tables changes till 23.05.2018
-                   added adjustements for project requirements
-Commad TableText is parsing Linux Command to according to headers and columns (adjusted)
+                   added adjustments for project requirements.
+
+Command TableText is parsing Linux Command to according to headers and columns (adjusted)
 For initialization it is getting 4 parameters (2 required 2 optional)
 Required parameters:
 _header_regexps --> regexp array for finding headers
 _header_keys --> array of keys assigned for found columns
 Optional parameters:
 _skip --> regexp for skipping line
 _finish --> regexp for finishing parsing (next parse execution will not give any line)
```

### Comparing `moler-3.4.0/moler/publisher.py` & `moler-3.5.0/moler/publisher.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/runner.py` & `moler-3.5.0/moler/runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/runner_factory.py` & `moler-3.5.0/moler/runner_factory.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/runner_single_thread.py` & `moler-3.5.0/moler/runner_single_thread.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/scheduler.py` & `moler-3.5.0/moler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 
 class Scheduler:
 
     @staticmethod
     def get_job(callback, interval, callback_params=None, cancel_on_exception=False, misfire_grace_time=0):
         """
-        Static method to create job.
+        Static method to create a job.
+
         :param callback: Reference to callable object (i.e. function, method)
         :param interval: time in float seconds when fun is called. If time of one execution is longer than interval then
-         some callbacks are missed. For example: interval is 2s and time of execution is 3s then callback will be called
-         when job ios created after 2s,  after 4s will not be executed because still the first excection is running,
-         then after 6s of is called.
+                         some callbacks are missed. For example: interval is 2s and time of execution is 3s then callback will be called
+                         when job ios created after 2s,  after 4s will not be executed because still the first exception is running,
+                         then after 6s of is called.
         :param callback_params: dict of params of fun
         :param cancel_on_exception: set True if you want to break next execution of this callback if previous raises an
-         exception
+                                    exception
         :param int misfire_grace_time: seconds after the designated runtime that the job is still allowed to be run
         :return: Instance of Job.
         """
         instance = Scheduler._get_instance()
         decorated = DecoratedCallable(callback, cancel_on_exception)
 
         if misfire_grace_time != 0:
@@ -44,18 +45,19 @@
         job = Job(job_internal)
         decorated.job = job
         return job
 
     @staticmethod
     def change_kind(scheduler_type=None):
         """
-        Static method to change type of scheduler
+        Static method to change type of scheduler.
+
         :param scheduler_type: type of new scheduler. Allowed thread (default) or asyncio. If None then default multi
-            threading model will be used.
-        :return: None. If scheduler_type is not supported then it raises object of type moler.exceptions.WrongUsage
+                               threading model will be used.
+        :return: None. If scheduler_type is not supported then it raises object of type moler.exceptions.WrongUsage.
         """
         instance = Scheduler._get_instance()
         instance._swap_scheduler(scheduler_type)  # pylint: disable=protected-access
 
     @staticmethod
     def _get_instance():
         """
```

### Comparing `moler-3.4.0/moler/threaded_moler_connection.py` & `moler-3.5.0/moler/threaded_moler_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/cmds_events_doc.py` & `moler-3.5.0/moler/util/cmds_events_doc.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/compressed_rotating_file_handler.py` & `moler-3.5.0/moler/util/compressed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/compressed_timed_rotating_file_handler.py` & `moler-3.5.0/moler/util/compressed_timed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/connection_observer.py` & `moler-3.5.0/moler/util/connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/connection_observer_life_status.py` & `moler-3.5.0/moler/util/connection_observer_life_status.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/converterhelper.py` & `moler-3.5.0/moler/util/converterhelper.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/devices_SM.py` & `moler-3.5.0/moler/util/devices_SM.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     tests_per_device=300,
     max_no_of_threads=11,
     rerun=0,
     timeout_multiply=3.0,
 ):
     """
     Check all states in device under test.
+
     :param device: device
     :param max_time: maximum time of check. None for infinity. If execution time is greater then max_time then test is
      interrupted.
     :param tests_per_device: how many tests should be performed in one thread.
     :param max_no_of_threads: maximum number of threads that can be started.
     :param rerun: rerun for goto_state
     :param timeout_multiply: timeout_multiply for goto_state
```

### Comparing `moler-3.4.0/moler/util/loghelper.py` & `moler-3.5.0/moler/util/loghelper.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/moler_serial_proxy.py` & `moler-3.5.0/moler/util/moler_serial_proxy.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler/util/moler_test.py` & `moler-3.5.0/moler/util/moler_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,69 +24,75 @@
 
 
 class MolerTest:
     @classmethod
     def steps_end(cls):
         """
         You should call this function at the end of your test code with Moler.
+
         :return: None
         """
         cls._was_steps_end = True
 
     @classmethod
     def error(cls, msg, raise_exception=False, dump=None):
         """
         Makes an error (fail the test) and (optional) continue the test flow.
+
         :param msg: Message to show.
         :param raise_exception: If True then raise an exception (if not in try except block then test will be
          terminated), if False then only show msg and mark error in logs.
         :param dump: If defined then dump object.
         :return: None.
         """
         cls._list_of_errors.append(msg)
         cls._error(msg, raise_exception, dump)
 
     @classmethod
     def info(cls, msg, dump=None):
         """
-        Shows the message
+        Shows the message.
+
         :param msg: Message to show.
         :param dump: If defined then dump object.
         :return: None.
         """
         msg = cls._get_string_message(msg, dump, None)
         cls._logger.info(msg)
 
     @classmethod
     def warning(cls, msg, dump=None):
         """
         Shows the message as warning.
+
         :param msg: Message to show.
         :param dump: If defined then dump object.
         :return: None
         """
         msg = cls._get_string_message(msg, dump, None)
         cls._logger.warning(msg)
 
     @classmethod
     def stop_python(cls, force=False):
         """
         Stops current Python.
+
         :return: None
         """
         cls.info("Python will be closed by user request.")
         pid = os.getpid()
         if force:
             os.kill(pid, signal.SIGKILL)
         os.kill(pid, signal.SIGINT)
 
     @classmethod
     def _dump(cls, obj):
         """
         Dumping objet to moler log.
+
         :param obj: Object to dump.
         :return: Dumped object as string
         """
         msg_str = pprint.pformat(obj, indent=1)
         return msg_str
 
     @classmethod
@@ -98,28 +104,30 @@
             msg = f"{msg}\n{caller_msg}"
 
         return msg
 
     @classmethod
     def sleep(cls, seconds, quiet=False):
         """
-        Add sleep functionality
+        Add sleep functionality.
+
         TODO: add support to asyncio when runner ready
         :param seconds: Time to sleep (in seconds)
         :param quiet: If True then no info to log about sleeping, if False then sleep info will be logged
         :return:
         """
         if not quiet:
             cls.info(f"Sleep for {seconds:.2f} seconds.")
         time.sleep(seconds)
 
     @classmethod
     def raise_background_exceptions(cls, decorated="function", check_steps_end=False):
         """
         Decorates the function, method or class.
+
         :param decorated: Function, method or class to decorate.
         :param check_steps_end: If True then check if steps_end was called before return the method, if False then do
          not check
         :return: Decorated callable
         """
         if callable(decorated):
             # direct decoration
```

### Comparing `moler-3.4.0/moler/util/tracked_thread.py` & `moler-3.5.0/moler/util/tracked_thread.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/moler.egg-info/PKG-INFO` & `moler-3.5.0/moler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moler
-Version: 3.4.0
+Version: 3.5.0
 Summary: Moler is a library for working with terminals, mainly for automated tests
 Home-page: https://github.com/nokia/moler
 Author: Nokia
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/nokia/moler/issues
 Project-URL: Source, https://github.com/nokia/moler
 Keywords: testing development
@@ -38,15 +38,15 @@
 Requires-Dist: psutil
 Requires-Dist: python-dateutil
 Requires-Dist: pyserial
 Requires-Dist: cryptography
 Requires-Dist: paramiko
 Requires-Dist: importlib-metadata
 
-[![image](https://img.shields.io/badge/pypi-v3.4.0-blue.svg)](https://pypi.org/project/moler/)
+[![image](https://img.shields.io/badge/pypi-v3.5.0-blue.svg)](https://pypi.org/project/moler/)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/moler/)
 [![Build Status](https://github.com/nokia/moler/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/nokia/moler/actions)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](./LICENSE)
 
 # Table of Contents
 1. [Changelog](#changelog)
 2. [Moler info](#moler)
```

### Comparing `moler-3.4.0/moler.egg-info/SOURCES.txt` & `moler-3.5.0/moler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/setup.py` & `moler-3.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import io
+from os import getcwd
 from os.path import abspath, dirname, join
 from setuptools import setup, find_packages
 
 here = abspath(dirname(__file__))
 with io.open(join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-with io.open(join(here, 'requirements.txt'), encoding='utf-8') as f:
+with io.open(join(getcwd(), 'requirements', 'base.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='moler',
-    version='3.4.0',
+    version='3.5.0',
     description='Moler is a library for working with terminals, mainly for automated tests',  # Required
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nokia/moler',
     author='Nokia',
     license='BSD 3-Clause',
     classifiers=[
```

### Comparing `moler-3.4.0/test/test_cmds_events_doc.py` & `moler-3.5.0/test/test_cmds_events_doc.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_command.py` & `moler-3.5.0/test/test_command.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_connection.py` & `moler-3.5.0/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_connection_configuration.py` & `moler-3.5.0/test/test_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_connection_factory.py` & `moler-3.5.0/test/test_connection_factory.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_connection_observer.py` & `moler-3.5.0/test/test_connection_observer.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_event.py` & `moler-3.5.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_event_awaiter.py` & `moler-3.5.0/test/test_event_awaiter.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_helpers.py` & `moler-3.5.0/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_loggers.py` & `moler-3.5.0/test/test_loggers.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_moler_test.py` & `moler-3.5.0/test/test_moler_test.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_publisher.py` & `moler-3.5.0/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_runner.py` & `moler-3.5.0/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_scheduler.py` & `moler-3.5.0/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_table_read_parser.py` & `moler-3.5.0/test/test_table_read_parser.py`

 * *Files identical despite different names*

### Comparing `moler-3.4.0/test/test_util_loghelper.py` & `moler-3.5.0/test/test_util_loghelper.py`

 * *Files identical despite different names*

