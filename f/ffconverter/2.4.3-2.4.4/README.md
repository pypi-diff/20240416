# Comparing `tmp/ffconverter-2.4.3.tar.gz` & `tmp/ffconverter-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffconverter-2.4.3.tar", last modified: Mon Apr  8 20:07:22 2024, max compression
+gzip compressed data, was "ffconverter-2.4.4.tar", last modified: Tue Apr 16 19:41:08 2024, max compression
```

## Comparing `ffconverter-2.4.3.tar` & `ffconverter-2.4.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/
--rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.3/AUTHORS
--rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.3/COPYING
--rw-r--r--   0 luna      (1000) luna      (1000)     6895 2024-04-08 19:51:36.000000 ffconverter-2.4.3/ChangeLog
--rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.3/MANIFEST.in
--rw-r--r--   0 luna      (1000) luna      (1000)     2639 2024-04-08 20:07:22.700591 ffconverter-2.4.3/PKG-INFO
--rw-r--r--   0 luna      (1000) luna      (1000)     4765 2024-04-08 19:17:41.000000 ffconverter-2.4.3/README.md
--rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.3/TRANSLATORS
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.693924 ffconverter-2.4.3/bin/
--rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.3/bin/ffconverter
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.697257 ffconverter-2.4.3/ffconverter/
--rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-08 19:21:32.000000 ffconverter-2.4.3/ffconverter/__init__.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/about_dlg.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/audiovideotab.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/config.py
--rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.3/ffconverter/dynamictab.py
--rw-r--r--   0 luna      (1000) luna      (1000)    29489 2024-04-08 19:33:48.000000 ffconverter-2.4.3/ffconverter/ffconverter.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/imagetab.py
--rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/preferences_dlg.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/presets_dlgs.py
--rw-r--r--   0 luna      (1000) luna      (1000)    27485 2024-04-08 19:49:28.000000 ffconverter-2.4.3/ffconverter/progress.py
--rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/qrc_resources.py
--rw-r--r--   0 luna      (1000) luna      (1000)    27485 2024-04-08 19:41:28.000000 ffconverter-2.4.3/ffconverter/utils.py
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/ffconverter.egg-info/
--rw-r--r--   0 luna      (1000) luna      (1000)     2639 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/PKG-INFO
--rw-r--r--   0 luna      (1000) luna      (1000)     1296 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/SOURCES.txt
--rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/dependency_links.txt
--rw-r--r--   0 luna      (1000) luna      (1000)       30 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/requires.txt
--rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/top_level.txt
--rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.3/launcher
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.697257 ffconverter-2.4.3/locale/
--rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter.pro
--rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_bg.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ca.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_cs.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_de_DE.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_el.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_en.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_es.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_fr.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_gl.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_gl_ES.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_hu.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_it.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ms_MY.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_pl_PL.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_pt.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_pt_BR.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ro_RO.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ru.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_tr.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_vi.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_zh_CN.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_zh_TW.ts
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/man/
--rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.3/man/ffconverter.1.gz
--rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.3/resources.qrc
--rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-08 20:07:22.700591 ffconverter-2.4.3/setup.cfg
--rwxr-xr-x   0 luna      (1000) luna      (1000)     3652 2024-04-08 19:20:09.000000 ffconverter-2.4.3/setup.py
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/share/
--rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-08 19:21:37.000000 ffconverter-2.4.3/share/ffconverter.desktop
--rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.3/share/ffconverter.png
--rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.3/share/presets.xml
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/test/
--rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.3/test/test_dialogs.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.203520 ffconverter-2.4.4/
+-rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.4/AUTHORS
+-rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.4/COPYING
+-rw-r--r--   0 luna      (1000) luna      (1000)     6975 2024-04-16 19:40:32.000000 ffconverter-2.4.4/ChangeLog
+-rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.4/MANIFEST.in
+-rw-r--r--   0 luna      (1000) luna      (1000)     2639 2024-04-16 19:41:08.203520 ffconverter-2.4.4/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     4691 2024-04-08 20:23:16.000000 ffconverter-2.4.4/README.md
+-rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.4/TRANSLATORS
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.190187 ffconverter-2.4.4/bin/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.4/bin/ffconverter
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.190187 ffconverter-2.4.4/ffconverter/
+-rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-16 19:40:43.000000 ffconverter-2.4.4/ffconverter/__init__.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/about_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/audiovideotab.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/config.py
+-rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.4/ffconverter/dynamictab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    29489 2024-04-08 19:33:48.000000 ffconverter-2.4.4/ffconverter/ffconverter.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/imagetab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/preferences_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/presets_dlgs.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    27485 2024-04-08 19:49:28.000000 ffconverter-2.4.4/ffconverter/progress.py
+-rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.4/ffconverter/qrc_resources.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    27313 2024-04-16 19:38:53.000000 ffconverter-2.4.4/ffconverter/utils.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.203520 ffconverter-2.4.4/ffconverter.egg-info/
+-rw-r--r--   0 luna      (1000) luna      (1000)     2639 2024-04-16 19:41:08.000000 ffconverter-2.4.4/ffconverter.egg-info/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     1296 2024-04-16 19:41:08.000000 ffconverter-2.4.4/ffconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-16 19:41:08.000000 ffconverter-2.4.4/ffconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)       30 2024-04-16 19:41:08.000000 ffconverter-2.4.4/ffconverter.egg-info/requires.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-16 19:41:08.000000 ffconverter-2.4.4/ffconverter.egg-info/top_level.txt
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.4/launcher
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.203520 ffconverter-2.4.4/locale/
+-rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter.pro
+-rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_bg.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_ca.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_cs.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_de_DE.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_el.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_en.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_es.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_fr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_gl.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_gl_ES.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_hu.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_it.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_ms_MY.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_pl_PL.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_pt.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_pt_BR.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_ro_RO.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_ru.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_tr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_vi.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_zh_CN.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.4/locale/ffconverter_zh_TW.ts
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.203520 ffconverter-2.4.4/man/
+-rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.4/man/ffconverter.1.gz
+-rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.4/resources.qrc
+-rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-16 19:41:08.203520 ffconverter-2.4.4/setup.cfg
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3652 2024-04-08 19:20:09.000000 ffconverter-2.4.4/setup.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.203520 ffconverter-2.4.4/share/
+-rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-16 19:40:39.000000 ffconverter-2.4.4/share/ffconverter.desktop
+-rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.4/share/ffconverter.png
+-rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.4/share/presets.xml
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-16 19:41:08.203520 ffconverter-2.4.4/test/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.4/test/test_dialogs.py
```

### Comparing `ffconverter-2.4.3/COPYING` & `ffconverter-2.4.4/COPYING`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ChangeLog` & `ffconverter-2.4.4/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Version 2.4.4
+-------------
+
+* Fix imagemagick detection of supported formats
+
+
 Version 2.4.3
 -------------
 
 * Move trimesh/gmsh to optional dependencies
 
 * Add missing 3D Formats
```

### Comparing `ffconverter-2.4.3/PKG-INFO` & `ffconverter-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.4.3
+Version: 2.4.4
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
```

### Comparing `ffconverter-2.4.3/README.md` & `ffconverter-2.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,27 @@
 On Windows, use [python.org](https://python.org) to get python (the version  
 in the Microsoft Store is [worse in some regards](https://docs.python.org/3/using/windows.html#known-issues)), then use  
 `python -m pip install PyQt5` to get PyQt5.  
 
 #### Optional dependencies:
 Without these some conversions will not work.  
 
+Python packages:  
+
+* trimesh (python package, used for 3D Models)  
+* gmsh (python package, requires trimesh, used for more 3D Models)  
+
 System Packages:  
 
 * ffmpeg (Audio and Video)  
 * imagemagick (Images)  
 * unoconv (Office formats)  
 * pandoc (Markdown)  
 * squashfs-tools, zip, unzip, binutils, tar, gzip, bzip2 (Compressed files)  
 
-Python packages:  
-
-* trimesh _AND_ gmsh (python packages, used for 3D Models)  
-
-These should be installed automatically when using pip/pipx,  
-but if you don't need to convert 3D Models you can remove these.  
-
 On Linux, use your distributions Package manager to install the System  
 packages. On Windows, either get .exe files and place them on the $PATH,  
 use [scoop](https://scoop.sh), or (for everything but ffmpeg) install the  
 dependencies in WSL. You could also try other third-party package managers  
 or even the Microsoft Store, the program only needs the command  
 (e.g. `unoconv`) to be available on the CMD.
```

### Comparing `ffconverter-2.4.3/TRANSLATORS` & `ffconverter-2.4.4/TRANSLATORS`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/__init__.py` & `ffconverter-2.4.4/ffconverter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 GUI File Format Converter
 """
 
 # version
 __major__ = 2
 __minor__ = 4
-__patch__ = 3
+__patch__ = 4
 __prerelease__ = "" # alpha, beta, rc etc.
 
 # package information
 __name__ = "ffconverter"
 __version__ = "{0}.{1}.{2}".format(__major__, __minor__, __patch__)
 __version__ += __prerelease__
 __description__ = "File Format Converter with Qt GUI"
```

### Comparing `ffconverter-2.4.3/ffconverter/about_dlg.py` & `ffconverter-2.4.4/ffconverter/about_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/audiovideotab.py` & `ffconverter-2.4.4/ffconverter/audiovideotab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/config.py` & `ffconverter-2.4.4/ffconverter/config.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/dynamictab.py` & `ffconverter-2.4.4/ffconverter/dynamictab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/ffconverter.py` & `ffconverter-2.4.4/ffconverter/ffconverter.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/imagetab.py` & `ffconverter-2.4.4/ffconverter/imagetab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/preferences_dlg.py` & `ffconverter-2.4.4/ffconverter/preferences_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/presets_dlgs.py` & `ffconverter-2.4.4/ffconverter/presets_dlgs.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/progress.py` & `ffconverter-2.4.4/ffconverter/progress.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/qrc_resources.py` & `ffconverter-2.4.4/ffconverter/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/ffconverter/utils.py` & `ffconverter-2.4.4/ffconverter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,36 +223,31 @@
         magick_format_list = magick_formats.split('\n')
         in_formats = []
         out_formats = []
         for line in magick_format_list:
             line_args = line.split()
             # if the line is empty or does not start with all-caps (EXTENSION)
             uppercase_chars = string.ascii_uppercase + '*-'
-            if len(line_args) < 3 or set(line_args[0]) <= set(uppercase_chars):
+            if len(line_args) < 3 or set(line_args[0]) > set(uppercase_chars):
                 continue
-            file_format, module, rw_status = line_args[:3]
+            file_format, module, rw_status = line_args[:3] # yayyyy the silly :33
             file_format = file_format.lower().replace('*', '')
             if module in ['BRAILLE', 'TXT']:
                 continue
-            if "r" in rw_status:
+            if "r" in rw_status and file_format not in list('rw+') and module != 'PDF':
                 # the program will break trying to read some PDFs
-                if module not in ['PDF']:
-                    in_formats.append(file_format)
-            if "w" in rw_status:
+                in_formats.append(file_format)
+            if "w" in rw_status and file_format not in list('rw+'):
                 out_formats.append(file_format)
-        # for formats like PNG, the output will be PNG00 .. PNG64.
-        if 'png00' in in_formats and 'png' not in in_formats:
-            in_formats.append('png')
-        if 'png00' in out_formats and 'png' not in out_formats:
-            out_formats.append('png')
         magick_conversions = [in_formats + extraformats_image,
                               out_formats + extraformats_image]
         supported_tmp.append(magick_conversions)
     else:
         magick_conversions = [[], []]
+    print(magick_conversions)
 
     # libreoffice exts
     # cant actually get those right now, so have some predefined lists instead
     if 'unoconv' not in missing:
         extraformats_document = (settings.value('extraformats_document') or [])
         calc  = [['csv', 'xls', 'xml', 'xlsx', 'ods', 'sdc'] + extraformats_document,
                 ['csv', 'html', 'xls', 'xml', 'ods', 'sdc', 'xhtml'] + extraformats_document]
```

### Comparing `ffconverter-2.4.3/ffconverter.egg-info/PKG-INFO` & `ffconverter-2.4.4/ffconverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.4.3
+Version: 2.4.4
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
```

### Comparing `ffconverter-2.4.3/ffconverter.egg-info/SOURCES.txt` & `ffconverter-2.4.4/ffconverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter.pro` & `ffconverter-2.4.4/locale/ffconverter.pro`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_bg.ts` & `ffconverter-2.4.4/locale/ffconverter_bg.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_ca.ts` & `ffconverter-2.4.4/locale/ffconverter_ca.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_cs.ts` & `ffconverter-2.4.4/locale/ffconverter_cs.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_de_DE.ts` & `ffconverter-2.4.4/locale/ffconverter_de_DE.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_el.ts` & `ffconverter-2.4.4/locale/ffconverter_el.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_en.ts` & `ffconverter-2.4.4/locale/ffconverter_en.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_es.ts` & `ffconverter-2.4.4/locale/ffconverter_es.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_fr.ts` & `ffconverter-2.4.4/locale/ffconverter_fr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_gl.ts` & `ffconverter-2.4.4/locale/ffconverter_gl.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_gl_ES.ts` & `ffconverter-2.4.4/locale/ffconverter_gl_ES.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_hu.ts` & `ffconverter-2.4.4/locale/ffconverter_hu.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_it.ts` & `ffconverter-2.4.4/locale/ffconverter_it.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_ms_MY.ts` & `ffconverter-2.4.4/locale/ffconverter_ms_MY.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_pl_PL.ts` & `ffconverter-2.4.4/locale/ffconverter_pl_PL.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_pt.ts` & `ffconverter-2.4.4/locale/ffconverter_pt.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_pt_BR.ts` & `ffconverter-2.4.4/locale/ffconverter_pt_BR.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_ro_RO.ts` & `ffconverter-2.4.4/locale/ffconverter_ro_RO.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_ru.ts` & `ffconverter-2.4.4/locale/ffconverter_ru.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_tr.ts` & `ffconverter-2.4.4/locale/ffconverter_tr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_vi.ts` & `ffconverter-2.4.4/locale/ffconverter_vi.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_zh_CN.ts` & `ffconverter-2.4.4/locale/ffconverter_zh_CN.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/locale/ffconverter_zh_TW.ts` & `ffconverter-2.4.4/locale/ffconverter_zh_TW.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/man/ffconverter.1.gz` & `ffconverter-2.4.4/man/ffconverter.1.gz`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/resources.qrc` & `ffconverter-2.4.4/resources.qrc`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/setup.py` & `ffconverter-2.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/share/ffconverter.png` & `ffconverter-2.4.4/share/ffconverter.png`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/share/presets.xml` & `ffconverter-2.4.4/share/presets.xml`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.3/test/test_dialogs.py` & `ffconverter-2.4.4/test/test_dialogs.py`

 * *Files identical despite different names*

