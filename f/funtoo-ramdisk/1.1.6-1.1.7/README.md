# Comparing `tmp/funtoo_ramdisk-1.1.6.tar.gz` & `tmp/funtoo_ramdisk-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo_ramdisk-1.1.6.tar", last modified: Mon Apr 15 03:23:13 2024, max compression
+gzip compressed data, was "funtoo_ramdisk-1.1.7.tar", last modified: Mon Apr 15 16:55:19 2024, max compression
```

## Comparing `funtoo_ramdisk-1.1.6.tar` & `funtoo_ramdisk-1.1.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.463770 funtoo_ramdisk-1.1.6/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8429 2024-04-15 03:22:39.000000 funtoo_ramdisk-1.1.6/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      111 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/MANIFEST.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16081 2024-04-15 03:23:13.463770 funtoo_ramdisk-1.1.6/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-04-15 03:15:29.000000 funtoo_ramdisk-1.1.6/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1901 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/bin/ramdisk
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/doc/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7107 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/doc/manpage.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7113 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/doc/manpage.rst.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7642 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/doc/ramdisk.8
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6309 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/args.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2041 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/config_files.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/const.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12096 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/initramfs.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1602 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/kernel.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1252 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/log.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    15949 2024-04-15 03:11:58.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/modules.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1167 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugin_base.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      361 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/btrfs.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      359 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      782 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/lvm.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      319 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/initrd.defaults
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6059 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/initrd.scripts
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      645 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      117 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/udev.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/initramfs.cpio
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2174 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/linuxrc
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2091 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.autoload
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1349 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.copy
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1375 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/utilities.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/version.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16081 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1374 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        5 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       15 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      721 2024-04-15 03:17:25.000000 funtoo_ramdisk-1.1.6/make.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-04-15 03:23:13.463770 funtoo_ramdisk-1.1.6/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      944 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      950 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/setup.py.in
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8638 2024-04-15 16:55:07.000000 funtoo_ramdisk-1.1.7/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      111 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/MANIFEST.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16290 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-04-15 16:54:11.000000 funtoo_ramdisk-1.1.7/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.028974 funtoo_ramdisk-1.1.7/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1901 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/bin/ramdisk
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.028974 funtoo_ramdisk-1.1.7/doc/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7107 2024-04-15 16:55:15.000000 funtoo_ramdisk-1.1.7/doc/manpage.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7113 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/doc/manpage.rst.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7642 2024-04-15 16:55:15.000000 funtoo_ramdisk-1.1.7/doc/ramdisk.8
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.028974 funtoo_ramdisk-1.1.7/funtoo_ramdisk/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6309 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/args.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2041 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/config_files.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/const.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12203 2024-04-15 16:53:26.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/initramfs.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1602 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/kernel.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1252 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/log.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    15949 2024-04-15 03:11:58.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/modules.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1167 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugin_base.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugins/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugins/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      361 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugins/btrfs.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      359 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugins/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      782 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugins/lvm.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      319 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/initrd.defaults
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6059 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/initrd.scripts
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/scan_mode/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/scan_mode/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      645 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      117 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/scan_mode/udev.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/initramfs.cpio
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2174 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/linuxrc
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/full/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/full/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2091 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/full/modules.autoload
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1349 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/full/modules.copy
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1375 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/utilities.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-04-15 16:55:15.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk/version.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16290 2024-04-15 16:55:18.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1374 2024-04-15 16:55:18.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-04-15 16:55:18.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        5 2024-04-15 16:55:18.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       15 2024-04-15 16:55:18.000000 funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      721 2024-04-15 03:17:25.000000 funtoo_ramdisk-1.1.7/make.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-04-15 16:55:19.038973 funtoo_ramdisk-1.1.7/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      944 2024-04-15 16:55:15.000000 funtoo_ramdisk-1.1.7/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      950 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.7/setup.py.in
```

### Comparing `funtoo_ramdisk-1.1.6/ChangeLog.rst` & `funtoo_ramdisk-1.1.7/ChangeLog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+funtoo-ramdisk 1.1.7
+--------------------
+
+Released on April 15, 2024.
+
+This is a minor bug release.
+
+* Fix a possible issue where ``__pycache__`` directories can mess
+  up copying of files to the initramfs.
+
 funtoo-ramdisk 1.1.6
 --------------------
 
 Released on April 14, 2024.
 
 This is a maintenance and minor features release.
```

### Comparing `funtoo_ramdisk-1.1.6/PKG-INFO` & `funtoo_ramdisk-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-ramdisk
-Version: 1.1.6
+Version: 1.1.7
 Summary: Funtoo framework for creating initial ramdisks.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse
 Author: Daniel Robbins, Funtoo Solutions Inc.
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -21,15 +21,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.6
+:Version: 1.1.7
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -168,14 +168,24 @@
 
 
 
 
 ChangeLog
 =========
 
+funtoo-ramdisk 1.1.7
+--------------------
+
+Released on April 15, 2024.
+
+This is a minor bug release.
+
+* Fix a possible issue where ``__pycache__`` directories can mess
+  up copying of files to the initramfs.
+
 funtoo-ramdisk 1.1.6
 --------------------
 
 Released on April 14, 2024.
 
 This is a maintenance and minor features release.
```

### Comparing `funtoo_ramdisk-1.1.6/README.rst` & `funtoo_ramdisk-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/bin/ramdisk` & `funtoo_ramdisk-1.1.7/bin/ramdisk`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/doc/manpage.rst` & `funtoo_ramdisk-1.1.7/doc/manpage.rst.in`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.6
+:Version: ##VERSION##
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
```

### Comparing `funtoo_ramdisk-1.1.6/doc/manpage.rst.in` & `funtoo_ramdisk-1.1.7/doc/manpage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: ##VERSION##
+:Version: 1.1.7
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
```

### Comparing `funtoo_ramdisk-1.1.6/doc/ramdisk.8` & `funtoo_ramdisk-1.1.7/doc/ramdisk.8`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "RAMDISK" "8" "" "1.1.6" "Funtoo Linux"
+.TH "RAMDISK" "8" "" "1.1.7" "Funtoo Linux"
 .SH NAME
 ramdisk \- create a bootable initial ramdisk
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 \fBramdisk\fP [build] [\fIOPTION...\fP] \fBinitramfs_outfile\fP
 .sp
```

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/args.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/args.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/config_files.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/config_files.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/const.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/const.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/initramfs.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/initramfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,19 @@
 			src = os.path.join(self.support_root, "etc", file)
 			if os.path.isfile(src):
 				shutil.copy(src, os.path.join(self.initramfs_root, "etc"))
 		for x in ["init", "etc/initrd.scripts", "etc/initrd.defaults"]:
 			os.chmod(os.path.join(self.initramfs_root, x), 0o755)
 		os.makedirs(os.path.join(self.initramfs_root, "etc/plugins/scan_mode"), exist_ok=True)
 		for file in os.listdir(os.path.join(self.support_root, "etc/plugins/scan_mode")):
-			shutil.copy(os.path.join(self.support_root, "etc/plugins/scan_mode", file), os.path.join(self.initramfs_root, "etc/plugins/scan_mode"))
+			src_path = os.path.join(self.support_root, "etc/plugins/scan_mode", file)
+			if os.path.isdir(file):
+				# Likely a __pycache__ directory:
+				continue
+			shutil.copy(src_path, os.path.join(self.initramfs_root, "etc/plugins/scan_mode", file))
 
 	def setup_busybox(self):
 		self.copy_binary("/bin/busybox")
 		self.copy_binary("/sbin/modprobe")
 		# Make sure these applets exist even before we tell busybox to create all the applets on initramfs:
 		for applet in [
 			"ash",
```

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/kernel.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/kernel.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/log.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/log.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/modules.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/modules.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugin_base.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugin_base.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/lvm.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/plugins/lvm.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/initrd.scripts` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/initrd.scripts`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/initramfs.cpio` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/initramfs.cpio`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/linuxrc` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/linuxrc`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.autoload` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/full/modules.autoload`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.copy` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/support/module_configs/full/modules.copy`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk/utilities.py` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk/utilities.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/PKG-INFO` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-ramdisk
-Version: 1.1.6
+Version: 1.1.7
 Summary: Funtoo framework for creating initial ramdisks.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse
 Author: Daniel Robbins, Funtoo Solutions Inc.
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -21,15 +21,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.6
+:Version: 1.1.7
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -168,14 +168,24 @@
 
 
 
 
 ChangeLog
 =========
 
+funtoo-ramdisk 1.1.7
+--------------------
+
+Released on April 15, 2024.
+
+This is a minor bug release.
+
+* Fix a possible issue where ``__pycache__`` directories can mess
+  up copying of files to the initramfs.
+
 funtoo-ramdisk 1.1.6
 --------------------
 
 Released on April 14, 2024.
 
 This is a maintenance and minor features release.
```

### Comparing `funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/SOURCES.txt` & `funtoo_ramdisk-1.1.7/funtoo_ramdisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/make.sh` & `funtoo_ramdisk-1.1.7/make.sh`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.6/setup.py` & `funtoo_ramdisk-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open("ChangeLog.rst", "r") as fh:
 	long_description += fh.read()
 
 print(long_description)
 
 setuptools.setup(
 	name="funtoo-ramdisk",
-	version="1.1.6",
+	version="1.1.7",
 	author="Daniel Robbins, Funtoo Solutions Inc.",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for creating initial ramdisks.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse",
 	scripts=["bin/ramdisk"],
```

### Comparing `funtoo_ramdisk-1.1.6/setup.py.in` & `funtoo_ramdisk-1.1.7/setup.py.in`

 * *Files identical despite different names*

