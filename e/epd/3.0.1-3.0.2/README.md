# Comparing `tmp/epd-3.0.1.tar.gz` & `tmp/epd-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epd-3.0.1.tar", last modified: Wed Apr  3 12:32:34 2024, max compression
+gzip compressed data, was "epd-3.0.2.tar", last modified: Tue Apr 16 09:38:38 2024, max compression
```

## Comparing `epd-3.0.1.tar` & `epd-3.0.2.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.636923 epd-3.0.1/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       78 2024-04-02 12:30:14.000000 epd-3.0.1/MANIFEST.in
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     6774 2024-04-03 12:32:34.636923 epd-3.0.1/PKG-INFO
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     6450 2024-04-03 12:30:36.000000 epd-3.0.1/README.md
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.624923 epd-3.0.1/c_kaleido/
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.624923 epd-3.0.1/c_kaleido/src/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2486 2024-04-02 13:38:59.000000 epd-3.0.1/c_kaleido/src/1bpp.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     3429 2024-04-02 13:38:59.000000 epd-3.0.1/c_kaleido/src/2bpp.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     8521 2024-04-02 13:38:59.000000 epd-3.0.1/c_kaleido/src/4bpp.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     3237 2024-04-02 13:38:59.000000 epd-3.0.1/c_kaleido/src/c_kaleido.c
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.628923 epd-3.0.1/epd/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)        0 2018-09-25 13:20:41.000000 epd-3.0.1/epd/__init__.py
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.628923 epd-3.0.1/epd/convert/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       23 2024-02-28 10:02:02.000000 epd-3.0.1/epd/convert/__init__.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      530 2018-10-02 11:28:36.000000 epd-3.0.1/epd/image.py
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.632923 epd-3.0.1/epd/tcm/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2323 2018-09-25 12:41:53.000000 epd-3.0.1/epd/tcm/TCGen1.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2874 2019-07-16 06:35:22.000000 epd-3.0.1/epd/tcm/TCGen2.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     8000 2024-04-02 10:54:37.000000 epd-3.0.1/epd/tcm/TCGen3.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     3148 2023-08-21 06:51:46.000000 epd-3.0.1/epd/tcm/__init__.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1908 2022-03-16 19:58:34.000000 epd-3.0.1/epd/tcm/tcm102.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1693 2022-03-16 19:58:34.000000 epd-3.0.1/epd/tcm/tcm113.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1506 2022-03-16 19:58:34.000000 epd-3.0.1/epd/tcm/tcm133.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1134 2022-12-31 20:07:26.000000 epd-3.0.1/epd/tcm/tcm27.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      802 2023-08-18 14:16:10.000000 epd-3.0.1/epd/tcm/tcm280.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2088 2022-03-16 20:49:45.000000 epd-3.0.1/epd/tcm/tcm312.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      906 2022-03-16 19:58:34.000000 epd-3.0.1/epd/tcm/tcm74.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1528 2022-03-16 19:58:34.000000 epd-3.0.1/epd/tcm/tcm97.py
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1933 2024-03-26 12:43:31.000000 epd-3.0.1/epd/tcm3_usb.py
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.628923 epd-3.0.1/epd.egg-info/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     6774 2024-04-03 12:32:34.000000 epd-3.0.1/epd.egg-info/PKG-INFO
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      997 2024-04-03 12:32:34.000000 epd-3.0.1/epd.egg-info/SOURCES.txt
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)        1 2024-04-03 12:32:34.000000 epd-3.0.1/epd.egg-info/dependency_links.txt
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       14 2024-04-03 12:32:34.000000 epd-3.0.1/epd.egg-info/top_level.txt
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.624923 epd-3.0.1/epdconvert/
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.632923 epd-3.0.1/epdconvert/include/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      115 2019-05-28 13:20:34.000000 epd-3.0.1/epdconvert/include/Chunks.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      194 2018-10-02 11:53:39.000000 epd-3.0.1/epdconvert/include/Compression.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      109 2019-05-28 11:28:27.000000 epd-3.0.1/epdconvert/include/Flip.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      106 2018-10-10 21:16:37.000000 epd-3.0.1/epdconvert/include/Invert.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      198 2018-09-24 08:34:59.000000 epd-3.0.1/epdconvert/include/Type0.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      117 2018-09-24 09:14:04.000000 epd-3.0.1/epdconvert/include/Type2.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      117 2019-03-06 11:23:51.000000 epd-3.0.1/epdconvert/include/Type7.h
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      103 2023-08-18 12:56:23.000000 epd-3.0.1/epdconvert/include/crc32.h
--rw-r--r--   0 musialpa  (1000) musialpa  (1000)     1907 2006-07-23 01:36:48.000000 epd-3.0.1/epdconvert/include/lz.h
-drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-03 12:32:34.636923 epd-3.0.1/epdconvert/src/
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1372 2020-02-24 13:20:05.000000 epd-3.0.1/epdconvert/src/Chunks.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1835 2019-05-17 11:51:49.000000 epd-3.0.1/epdconvert/src/Compression.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1191 2019-05-28 11:30:42.000000 epd-3.0.1/epdconvert/src/Flip.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      721 2018-10-11 06:27:36.000000 epd-3.0.1/epdconvert/src/Invert.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2136 2019-05-17 09:44:17.000000 epd-3.0.1/epdconvert/src/Type0.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1184 2018-12-19 09:55:49.000000 epd-3.0.1/epdconvert/src/Type2.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1675 2022-03-16 19:51:59.000000 epd-3.0.1/epdconvert/src/Type7.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1080 2023-08-18 13:00:12.000000 epd-3.0.1/epdconvert/src/crc32.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2372 2023-08-18 13:21:02.000000 epd-3.0.1/epdconvert/src/epdconvert.c
--rw-r--r--   0 musialpa  (1000) musialpa  (1000)    17692 2018-09-24 09:18:42.000000 epd-3.0.1/epdconvert/src/lz.c
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       38 2024-04-03 12:32:34.636923 epd-3.0.1/setup.cfg
--rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2132 2024-04-03 12:31:51.000000 epd-3.0.1/setup.py
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.444307 epd-3.0.2/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       78 2024-04-16 09:30:21.000000 epd-3.0.2/MANIFEST.in
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     6774 2024-04-16 09:38:38.444307 epd-3.0.2/PKG-INFO
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     6450 2024-04-03 12:30:36.000000 epd-3.0.2/README.md
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.436307 epd-3.0.2/c_kaleido/
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.436307 epd-3.0.2/c_kaleido/include/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      143 2024-04-02 13:38:59.000000 epd-3.0.2/c_kaleido/include/1bpp.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      143 2024-04-02 13:38:59.000000 epd-3.0.2/c_kaleido/include/2bpp.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      143 2024-04-02 13:38:59.000000 epd-3.0.2/c_kaleido/include/4bpp.h
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.440307 epd-3.0.2/c_kaleido/src/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2487 2024-04-16 09:34:14.000000 epd-3.0.2/c_kaleido/src/1bpp.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     3429 2024-04-02 13:38:59.000000 epd-3.0.2/c_kaleido/src/2bpp.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     8521 2024-04-02 13:38:59.000000 epd-3.0.2/c_kaleido/src/4bpp.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     3219 2024-04-16 09:34:14.000000 epd-3.0.2/c_kaleido/src/c_kaleido.c
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.440307 epd-3.0.2/epd/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)        0 2018-09-25 13:20:41.000000 epd-3.0.2/epd/__init__.py
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.440307 epd-3.0.2/epd/convert/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       23 2024-02-28 10:02:02.000000 epd-3.0.2/epd/convert/__init__.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      530 2018-10-02 11:28:36.000000 epd-3.0.2/epd/image.py
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.440307 epd-3.0.2/epd/tcm/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2323 2018-09-25 12:41:53.000000 epd-3.0.2/epd/tcm/TCGen1.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2874 2019-07-16 06:35:22.000000 epd-3.0.2/epd/tcm/TCGen2.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     8000 2024-04-02 10:54:37.000000 epd-3.0.2/epd/tcm/TCGen3.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     3148 2023-08-21 06:51:46.000000 epd-3.0.2/epd/tcm/__init__.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1908 2022-03-16 19:58:34.000000 epd-3.0.2/epd/tcm/tcm102.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1693 2022-03-16 19:58:34.000000 epd-3.0.2/epd/tcm/tcm113.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1506 2022-03-16 19:58:34.000000 epd-3.0.2/epd/tcm/tcm133.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1134 2022-12-31 20:07:26.000000 epd-3.0.2/epd/tcm/tcm27.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      802 2023-08-18 14:16:10.000000 epd-3.0.2/epd/tcm/tcm280.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2088 2022-03-16 20:49:45.000000 epd-3.0.2/epd/tcm/tcm312.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      906 2022-03-16 19:58:34.000000 epd-3.0.2/epd/tcm/tcm74.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1528 2022-03-16 19:58:34.000000 epd-3.0.2/epd/tcm/tcm97.py
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1933 2024-03-26 12:43:31.000000 epd-3.0.2/epd/tcm3_usb.py
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.440307 epd-3.0.2/epd.egg-info/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     6774 2024-04-16 09:38:38.000000 epd-3.0.2/epd.egg-info/PKG-INFO
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1072 2024-04-16 09:38:38.000000 epd-3.0.2/epd.egg-info/SOURCES.txt
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)        1 2024-04-16 09:38:38.000000 epd-3.0.2/epd.egg-info/dependency_links.txt
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       14 2024-04-16 09:38:38.000000 epd-3.0.2/epd.egg-info/top_level.txt
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.436307 epd-3.0.2/epdconvert/
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.444307 epd-3.0.2/epdconvert/include/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      115 2019-05-28 13:20:34.000000 epd-3.0.2/epdconvert/include/Chunks.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      194 2018-10-02 11:53:39.000000 epd-3.0.2/epdconvert/include/Compression.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      109 2019-05-28 11:28:27.000000 epd-3.0.2/epdconvert/include/Flip.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      106 2018-10-10 21:16:37.000000 epd-3.0.2/epdconvert/include/Invert.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      198 2018-09-24 08:34:59.000000 epd-3.0.2/epdconvert/include/Type0.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      117 2018-09-24 09:14:04.000000 epd-3.0.2/epdconvert/include/Type2.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      117 2019-03-06 11:23:51.000000 epd-3.0.2/epdconvert/include/Type7.h
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      103 2023-08-18 12:56:23.000000 epd-3.0.2/epdconvert/include/crc32.h
+-rw-r--r--   0 musialpa  (1000) musialpa  (1000)     1907 2006-07-23 01:36:48.000000 epd-3.0.2/epdconvert/include/lz.h
+drwxrwxr-x   0 musialpa  (1000) musialpa  (1000)        0 2024-04-16 09:38:38.444307 epd-3.0.2/epdconvert/src/
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1372 2020-02-24 13:20:05.000000 epd-3.0.2/epdconvert/src/Chunks.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1835 2019-05-17 11:51:49.000000 epd-3.0.2/epdconvert/src/Compression.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1191 2019-05-28 11:30:42.000000 epd-3.0.2/epdconvert/src/Flip.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)      721 2018-10-11 06:27:36.000000 epd-3.0.2/epdconvert/src/Invert.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2136 2019-05-17 09:44:17.000000 epd-3.0.2/epdconvert/src/Type0.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1184 2018-12-19 09:55:49.000000 epd-3.0.2/epdconvert/src/Type2.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1675 2022-03-16 19:51:59.000000 epd-3.0.2/epdconvert/src/Type7.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     1080 2023-08-18 13:00:12.000000 epd-3.0.2/epdconvert/src/crc32.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2372 2023-08-18 13:21:02.000000 epd-3.0.2/epdconvert/src/epdconvert.c
+-rw-r--r--   0 musialpa  (1000) musialpa  (1000)    17692 2018-09-24 09:18:42.000000 epd-3.0.2/epdconvert/src/lz.c
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)       38 2024-04-16 09:38:38.444307 epd-3.0.2/setup.cfg
+-rw-rw-r--   0 musialpa  (1000) musialpa  (1000)     2132 2024-04-16 09:30:21.000000 epd-3.0.2/setup.py
```

### Comparing `epd-3.0.1/PKG-INFO` & `epd-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epd
-Version: 3.0.1
+Version: 3.0.2
 Summary: EPD library for MpicoSys Timing Controllers (TC/TCM), including color conversion
 Home-page: https://www.mpicosys.com/
 Author: Paweł Musiał, MpicoSys
 Author-email: pawel.musial@mpicosys.com
 Requires: Pillow
 Requires: hashlib
 Description-Content-Type: text/markdown
```

### Comparing `epd-3.0.1/README.md` & `epd-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/c_kaleido/src/1bpp.c` & `epd-3.0.2/c_kaleido/src/1bpp.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include <stdint.h>
 #include <string.h>
 // FIXME make it workable for all different display sizes (not only 13.3 1600x1200)
 
+
 #define W 1600
 #define H 1200
 #define STEP 3
 
 static uint8_t NO_RED[3] = {2,1,4};
 static uint8_t NO_GREEN[3] = {1,4,2};
 static uint8_t NO_BLUE[3] = {4,2,1};
```

### Comparing `epd-3.0.1/c_kaleido/src/2bpp.c` & `epd-3.0.2/c_kaleido/src/2bpp.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/c_kaleido/src/4bpp.c` & `epd-3.0.2/c_kaleido/src/4bpp.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/c_kaleido/src/c_kaleido.c` & `epd-3.0.2/c_kaleido/src/c_kaleido.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
-#include "1bpp.h"
 
 #if PY_MAJOR_VERSION >= 3
 #define PY3K
 #endif
 
 #include "1bpp.h"
 #include "2bpp.h"
```

### Comparing `epd-3.0.1/epd/image.py` & `epd-3.0.2/epd/image.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/TCGen1.py` & `epd-3.0.2/epd/tcm/TCGen1.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/TCGen2.py` & `epd-3.0.2/epd/tcm/TCGen2.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/TCGen3.py` & `epd-3.0.2/epd/tcm/TCGen3.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/__init__.py` & `epd-3.0.2/epd/tcm/__init__.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm102.py` & `epd-3.0.2/epd/tcm/tcm102.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm113.py` & `epd-3.0.2/epd/tcm/tcm113.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm133.py` & `epd-3.0.2/epd/tcm/tcm133.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm27.py` & `epd-3.0.2/epd/tcm/tcm27.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm280.py` & `epd-3.0.2/epd/tcm/tcm280.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm312.py` & `epd-3.0.2/epd/tcm/tcm312.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm74.py` & `epd-3.0.2/epd/tcm/tcm74.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm/tcm97.py` & `epd-3.0.2/epd/tcm/tcm97.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd/tcm3_usb.py` & `epd-3.0.2/epd/tcm3_usb.py`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epd.egg-info/PKG-INFO` & `epd-3.0.2/epd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epd
-Version: 3.0.1
+Version: 3.0.2
 Summary: EPD library for MpicoSys Timing Controllers (TC/TCM), including color conversion
 Home-page: https://www.mpicosys.com/
 Author: Paweł Musiał, MpicoSys
 Author-email: pawel.musial@mpicosys.com
 Requires: Pillow
 Requires: hashlib
 Description-Content-Type: text/markdown
```

### Comparing `epd-3.0.1/epd.egg-info/SOURCES.txt` & `epd-3.0.2/epd.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 MANIFEST.in
 README.md
 setup.py
+c_kaleido/include/1bpp.h
+c_kaleido/include/2bpp.h
+c_kaleido/include/4bpp.h
 c_kaleido/src/1bpp.c
 c_kaleido/src/2bpp.c
 c_kaleido/src/4bpp.c
 c_kaleido/src/c_kaleido.c
 epd/__init__.py
 epd/image.py
 epd/tcm3_usb.py
```

### Comparing `epd-3.0.1/epdconvert/include/lz.h` & `epd-3.0.2/epdconvert/include/lz.h`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Chunks.c` & `epd-3.0.2/epdconvert/src/Chunks.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Compression.c` & `epd-3.0.2/epdconvert/src/Compression.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Flip.c` & `epd-3.0.2/epdconvert/src/Flip.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Invert.c` & `epd-3.0.2/epdconvert/src/Invert.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Type0.c` & `epd-3.0.2/epdconvert/src/Type0.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Type2.c` & `epd-3.0.2/epdconvert/src/Type2.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/Type7.c` & `epd-3.0.2/epdconvert/src/Type7.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/crc32.c` & `epd-3.0.2/epdconvert/src/crc32.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/epdconvert.c` & `epd-3.0.2/epdconvert/src/epdconvert.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/epdconvert/src/lz.c` & `epd-3.0.2/epdconvert/src/lz.c`

 * *Files identical despite different names*

### Comparing `epd-3.0.1/setup.py` & `epd-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup (name = 'epd',
-       version = '3.0.1',
+       version = '3.0.2',
        author="Paweł Musiał, MpicoSys",
        url="https://www.mpicosys.com/",
        author_email='pawel.musial@mpicosys.com',
        description = 'EPD library for MpicoSys Timing Controllers (TC/TCM), including color conversion',
        ext_modules = [c_convert,c_kaleido],
        packages = ['epd','epd.tcm','epd.convert',],
        requires = ['Pillow','hashlib'],
```

