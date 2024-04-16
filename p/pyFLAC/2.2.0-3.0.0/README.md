# Comparing `tmp/pyFLAC-2.2.0.tar.gz` & `tmp/pyFLAC-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFLAC-2.2.0.tar", last modified: Tue Aug  1 09:01:34 2023, max compression
+gzip compressed data, was "pyFLAC-3.0.0.tar", last modified: Tue Apr 16 14:20:55 2024, max compression
```

## Comparing `pyFLAC-2.2.0.tar` & `pyFLAC-3.0.0.tar`

### file list

```diff
@@ -1,95 +1,68 @@
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.923354 pyFLAC-2.2.0/
--rw-r--r--   0 joe.todd   (502) staff       (20)      407 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/.coveragerc
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.795972 pyFLAC-2.2.0/.github/
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.829201 pyFLAC-2.2.0/.github/workflows/
--rw-r--r--   0 joe.todd   (502) staff       (20)     2664 2023-07-29 14:35:20.000000 pyFLAC-2.2.0/.github/workflows/build.yml
--rw-r--r--   0 joe.todd   (502) staff       (20)      333 2023-07-27 19:46:44.000000 pyFLAC-2.2.0/.github/workflows/lint.yml
--rw-r--r--   0 joe.todd   (502) staff       (20)     1781 2023-07-28 07:19:52.000000 pyFLAC-2.2.0/.github/workflows/test.yml
--rw-r--r--   0 joe.todd   (502) staff       (20)     1928 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/.gitignore
--rw-r--r--   0 joe.todd   (502) staff       (20)      485 2023-07-27 19:49:35.000000 pyFLAC-2.2.0/.readthedocs.yml
--rw-r--r--   0 joe.todd   (502) staff       (20)     1053 2023-07-29 12:00:20.000000 pyFLAC-2.2.0/CHANGELOG.rst
--rw-r--r--   0 joe.todd   (502) staff       (20)     1062 2023-07-29 12:04:01.000000 pyFLAC-2.2.0/CONTRIBUTING.rst
--rw-r--r--   0 joe.todd   (502) staff       (20)    11341 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/LICENSE.txt
--rw-r--r--   0 joe.todd   (502) staff       (20)      788 2022-10-26 13:28:49.000000 pyFLAC-2.2.0/MANIFEST.in
--rw-r--r--   0 joe.todd   (502) staff       (20)     3271 2023-08-01 09:01:34.922826 pyFLAC-2.2.0/PKG-INFO
--rw-r--r--   0 joe.todd   (502) staff       (20)     2472 2023-07-27 19:50:48.000000 pyFLAC-2.2.0/README.rst
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.845533 pyFLAC-2.2.0/assets/
--rw-r--r--   0 joe.todd   (502) staff       (20)   138802 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/assets/icon-black.png
--rw-r--r--   0 joe.todd   (502) staff       (20)   130824 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/assets/icon-white.png
--rw-r--r--   0 joe.todd   (502) staff       (20)   270219 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/assets/logo-black.png
--rw-r--r--   0 joe.todd   (502) staff       (20)   154889 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/assets/logo-white-background.jpg
--rw-r--r--   0 joe.todd   (502) staff       (20)   301930 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/assets/logo-white-wide.jpg
--rw-r--r--   0 joe.todd   (502) staff       (20)   332847 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/assets/logo-white.png
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.853351 pyFLAC-2.2.0/docs/
--rw-r--r--   0 joe.todd   (502) staff       (20)      634 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/docs/Makefile
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.854618 pyFLAC-2.2.0/docs/_static/
--rw-r--r--   0 joe.todd   (502) staff       (20)       52 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/docs/_static/custom.css
--rw-r--r--   0 joe.todd   (502) staff       (20)     3159 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/docs/conf.py
--rw-r--r--   0 joe.todd   (502) staff       (20)     2458 2023-07-29 11:53:54.000000 pyFLAC-2.2.0/docs/index.rst
--rw-r--r--   0 joe.todd   (502) staff       (20)      795 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/docs/make.bat
--rw-r--r--   0 joe.todd   (502) staff       (20)       28 2021-07-21 07:22:54.000000 pyFLAC-2.2.0/docs/requirements.txt
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.856789 pyFLAC-2.2.0/examples/
--rwxr-xr-x   0 joe.todd   (502) staff       (20)     2870 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/examples/passthrough.py
--rwxr-xr-x   0 joe.todd   (502) staff       (20)     3843 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/examples/stream.py
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.861950 pyFLAC-2.2.0/pyFLAC.egg-info/
--rw-r--r--   0 joe.todd   (502) staff       (20)     3271 2023-08-01 09:01:34.000000 pyFLAC-2.2.0/pyFLAC.egg-info/PKG-INFO
--rw-r--r--   0 joe.todd   (502) staff       (20)     1781 2023-08-01 09:01:34.000000 pyFLAC-2.2.0/pyFLAC.egg-info/SOURCES.txt
--rw-r--r--   0 joe.todd   (502) staff       (20)        1 2023-08-01 09:01:34.000000 pyFLAC-2.2.0/pyFLAC.egg-info/dependency_links.txt
--rw-r--r--   0 joe.todd   (502) staff       (20)       48 2023-08-01 09:01:34.000000 pyFLAC-2.2.0/pyFLAC.egg-info/entry_points.txt
--rw-r--r--   0 joe.todd   (502) staff       (20)       40 2023-08-01 09:01:34.000000 pyFLAC-2.2.0/pyFLAC.egg-info/requires.txt
--rw-r--r--   0 joe.todd   (502) staff       (20)        7 2023-08-01 09:01:34.000000 pyFLAC-2.2.0/pyFLAC.egg-info/top_level.txt
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.865561 pyFLAC-2.2.0/pyflac/
--rw-r--r--   0 joe.todd   (502) staff       (20)     1592 2023-08-01 08:58:20.000000 pyFLAC-2.2.0/pyflac/__init__.py
--rw-r--r--   0 joe.todd   (502) staff       (20)     2236 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/pyflac/__main__.py
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.868268 pyFLAC-2.2.0/pyflac/builder/
--rw-r--r--   0 joe.todd   (502) staff       (20)     2201 2023-08-01 09:00:45.000000 pyFLAC-2.2.0/pyflac/builder/build_args.py
--rw-r--r--   0 joe.todd   (502) staff       (20)    18601 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/pyflac/builder/decoder.py
--rw-r--r--   0 joe.todd   (502) staff       (20)    16004 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/pyflac/builder/encoder.py
--rw-r--r--   0 joe.todd   (502) staff       (20)    14866 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/pyflac/decoder.py
--rw-r--r--   0 joe.todd   (502) staff       (20)    17957 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/pyflac/encoder.py
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.800291 pyFLAC-2.2.0/pyflac/include/
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.872980 pyFLAC-2.2.0/pyflac/include/FLAC/
--rw-r--r--   0 joe.todd   (502) staff       (20)     4102 2023-07-29 12:06:46.000000 pyFLAC-2.2.0/pyflac/include/FLAC/export.h
--rw-r--r--   0 joe.todd   (502) staff       (20)    41367 2023-07-29 12:06:46.000000 pyFLAC-2.2.0/pyflac/include/FLAC/format.h
--rw-r--r--   0 joe.todd   (502) staff       (20)     2081 2023-07-29 12:06:46.000000 pyFLAC-2.2.0/pyflac/include/FLAC/ordinals.h
--rw-r--r--   0 joe.todd   (502) staff       (20)    70056 2023-07-29 12:06:46.000000 pyFLAC-2.2.0/pyflac/include/FLAC/stream_decoder.h
--rw-r--r--   0 joe.todd   (502) staff       (20)    84581 2023-07-29 12:06:46.000000 pyFLAC-2.2.0/pyflac/include/FLAC/stream_encoder.h
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.874094 pyFLAC-2.2.0/pyflac/libraries/
--rw-r--r--   0 joe.todd   (502) staff       (20)     1509 2023-07-29 12:05:42.000000 pyFLAC-2.2.0/pyflac/libraries/LICENSE
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.875263 pyFLAC-2.2.0/pyflac/libraries/darwin-arm64/
--rw-r--r--   0 joe.todd   (502) staff       (20)   241792 2023-07-29 12:24:02.000000 pyFLAC-2.2.0/pyflac/libraries/darwin-arm64/libFLAC.12.dylib
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.878367 pyFLAC-2.2.0/pyflac/libraries/darwin-x86_64/
--rw-r--r--   0 joe.todd   (502) staff       (20)   297496 2023-07-29 12:24:18.000000 pyFLAC-2.2.0/pyflac/libraries/darwin-x86_64/libFLAC.12.dylib
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.881527 pyFLAC-2.2.0/pyflac/libraries/linux-arm64/
--rwxr-xr-x   0 joe.todd   (502) staff       (20)   410392 2023-07-28 17:46:03.000000 pyFLAC-2.2.0/pyflac/libraries/linux-arm64/libFLAC-12.1.0.so
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.884734 pyFLAC-2.2.0/pyflac/libraries/linux-x86_64/
--rwxr-xr-x   0 joe.todd   (502) staff       (20)   330216 2023-07-28 17:17:24.000000 pyFLAC-2.2.0/pyflac/libraries/linux-x86_64/libFLAC-12.1.0.so
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.887932 pyFLAC-2.2.0/pyflac/libraries/raspbian-armv6z/
--rwxr-xr-x   0 joe.todd   (502) staff       (20)   354068 2023-07-29 14:48:01.000000 pyFLAC-2.2.0/pyflac/libraries/raspbian-armv6z/libFLAC-12.1.0.so
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.891145 pyFLAC-2.2.0/pyflac/libraries/raspbian-armv7a/
--rwxr-xr-x   0 joe.todd   (502) staff       (20)   348896 2023-07-28 17:15:37.000000 pyFLAC-2.2.0/pyflac/libraries/raspbian-armv7a/libFLAC-12.1.0.so
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.895818 pyFLAC-2.2.0/pyflac/libraries/windows-i686/
--rw-r--r--   0 joe.todd   (502) staff       (20)   229388 2023-08-01 08:57:47.000000 pyFLAC-2.2.0/pyflac/libraries/windows-i686/FLAC-12.lib
--rw-r--r--   0 joe.todd   (502) staff       (20)   512014 2023-08-01 08:58:20.000000 pyFLAC-2.2.0/pyflac/libraries/windows-i686/libFLAC.dll
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.899690 pyFLAC-2.2.0/pyflac/libraries/windows-x86_64/
--rw-r--r--   0 joe.todd   (502) staff       (20)   226594 2023-08-01 08:57:47.000000 pyFLAC-2.2.0/pyflac/libraries/windows-x86_64/FLAC-12.lib
--rw-r--r--   0 joe.todd   (502) staff       (20)   446976 2023-08-01 08:58:20.000000 pyFLAC-2.2.0/pyflac/libraries/windows-x86_64/libFLAC.dll
--rw-r--r--   0 joe.todd   (502) staff       (20)     1343 2023-07-29 12:05:13.000000 pyFLAC-2.2.0/pyproject.toml
--rw-r--r--   0 joe.todd   (502) staff       (20)       38 2023-08-01 09:01:34.923521 pyFLAC-2.2.0/setup.cfg
--rw-r--r--   0 joe.todd   (502) staff       (20)      568 2023-07-29 12:53:19.000000 pyFLAC-2.2.0/setup.py
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.903616 pyFLAC-2.2.0/tests/
--rw-r--r--   0 joe.todd   (502) staff       (20)        0 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/__init__.py
-drwxr-xr-x   0 joe.todd   (502) staff       (20)        0 2023-08-01 09:01:34.920246 pyFLAC-2.2.0/tests/data/
--rw-r--r--   0 joe.todd   (502) staff       (20)    21727 2023-07-28 09:51:23.000000 pyFLAC-2.2.0/tests/data/32bit.flac
--rw-r--r--   0 joe.todd   (502) staff       (20)   176480 2023-07-28 09:51:23.000000 pyFLAC-2.2.0/tests/data/32bit.wav
--rw-r--r--   0 joe.todd   (502) staff       (20)    15832 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/8bit.flac
--rw-r--r--   0 joe.todd   (502) staff       (20)       84 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/LICENSE
--rw-r--r--   0 joe.todd   (502) staff       (20)    20964 2023-07-30 11:17:52.000000 pyFLAC-2.2.0/tests/data/mono.flac
--rw-r--r--   0 joe.todd   (502) staff       (20)    88324 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/mono.wav
--rw-r--r--   0 joe.todd   (502) staff       (20)    73681 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/stereo.flac
--rw-r--r--   0 joe.todd   (502) staff       (20)   264644 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/stereo.wav
--rw-r--r--   0 joe.todd   (502) staff       (20)    65653 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/surround.flac
--rw-r--r--   0 joe.todd   (502) staff       (20)   329980 2021-04-22 16:21:37.000000 pyFLAC-2.2.0/tests/data/surround.wav
--rw-r--r--   0 joe.todd   (502) staff       (20)     5538 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/tests/test_decoder.py
--rw-r--r--   0 joe.todd   (502) staff       (20)    12430 2023-07-29 12:05:43.000000 pyFLAC-2.2.0/tests/test_encoder.py
--rw-r--r--   0 joe.todd   (502) staff       (20)      175 2023-07-27 21:05:28.000000 pyFLAC-2.2.0/tox.ini
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.456264 pyFLAC-3.0.0/
+-rw-r--r--   0 joe.todd   (503) staff       (20)     1419 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 joe.todd   (503) staff       (20)     1062 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 joe.todd   (503) staff       (20)    11341 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/LICENSE.txt
+-rw-r--r--   0 joe.todd   (503) staff       (20)      788 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/MANIFEST.in
+-rw-r--r--   0 joe.todd   (503) staff       (20)     3253 2024-04-16 14:20:55.455918 pyFLAC-3.0.0/PKG-INFO
+-rw-r--r--   0 joe.todd   (503) staff       (20)     2318 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/README.rst
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.427500 pyFLAC-3.0.0/examples/
+-rwxr-xr-x   0 joe.todd   (503) staff       (20)     3166 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/examples/passthrough.py
+-rwxr-xr-x   0 joe.todd   (503) staff       (20)     3843 2024-03-31 10:43:40.000000 pyFLAC-3.0.0/examples/stream.py
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.455438 pyFLAC-3.0.0/pyFLAC.egg-info/
+-rw-r--r--   0 joe.todd   (503) staff       (20)     3253 2024-04-16 14:20:55.000000 pyFLAC-3.0.0/pyFLAC.egg-info/PKG-INFO
+-rw-r--r--   0 joe.todd   (503) staff       (20)     1331 2024-04-16 14:20:55.000000 pyFLAC-3.0.0/pyFLAC.egg-info/SOURCES.txt
+-rw-r--r--   0 joe.todd   (503) staff       (20)        1 2024-04-16 14:20:55.000000 pyFLAC-3.0.0/pyFLAC.egg-info/dependency_links.txt
+-rw-r--r--   0 joe.todd   (503) staff       (20)       48 2024-04-16 14:20:55.000000 pyFLAC-3.0.0/pyFLAC.egg-info/entry_points.txt
+-rw-r--r--   0 joe.todd   (503) staff       (20)       40 2024-04-16 14:20:55.000000 pyFLAC-3.0.0/pyFLAC.egg-info/requires.txt
+-rw-r--r--   0 joe.todd   (503) staff       (20)        7 2024-04-16 14:20:55.000000 pyFLAC-3.0.0/pyFLAC.egg-info/top_level.txt
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.431290 pyFLAC-3.0.0/pyflac/
+-rw-r--r--   0 joe.todd   (503) staff       (20)     1634 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/pyflac/__init__.py
+-rw-r--r--   0 joe.todd   (503) staff       (20)     2101 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/pyflac/__main__.py
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.432593 pyFLAC-3.0.0/pyflac/builder/
+-rw-r--r--   0 joe.todd   (503) staff       (20)     2201 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/builder/build_args.py
+-rw-r--r--   0 joe.todd   (503) staff       (20)    18601 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/builder/decoder.py
+-rw-r--r--   0 joe.todd   (503) staff       (20)    16004 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/builder/encoder.py
+-rw-r--r--   0 joe.todd   (503) staff       (20)    18408 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/pyflac/decoder.py
+-rw-r--r--   0 joe.todd   (503) staff       (20)    18029 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/pyflac/encoder.py
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.423114 pyFLAC-3.0.0/pyflac/include/
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.434571 pyFLAC-3.0.0/pyflac/include/FLAC/
+-rw-r--r--   0 joe.todd   (503) staff       (20)     4102 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/include/FLAC/export.h
+-rw-r--r--   0 joe.todd   (503) staff       (20)    41367 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/include/FLAC/format.h
+-rw-r--r--   0 joe.todd   (503) staff       (20)     2081 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/include/FLAC/ordinals.h
+-rw-r--r--   0 joe.todd   (503) staff       (20)    70056 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/include/FLAC/stream_decoder.h
+-rw-r--r--   0 joe.todd   (503) staff       (20)    84581 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/include/FLAC/stream_encoder.h
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.435121 pyFLAC-3.0.0/pyflac/libraries/
+-rw-r--r--   0 joe.todd   (503) staff       (20)     1509 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/LICENSE
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.435585 pyFLAC-3.0.0/pyflac/libraries/darwin-arm64/
+-rw-r--r--   0 joe.todd   (503) staff       (20)   241792 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/darwin-arm64/libFLAC.12.dylib
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.436605 pyFLAC-3.0.0/pyflac/libraries/darwin-x86_64/
+-rw-r--r--   0 joe.todd   (503) staff       (20)   297496 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/darwin-x86_64/libFLAC.12.dylib
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.437714 pyFLAC-3.0.0/pyflac/libraries/linux-arm64/
+-rwxr-xr-x   0 joe.todd   (503) staff       (20)   410392 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/linux-arm64/libFLAC-12.1.0.so
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.438648 pyFLAC-3.0.0/pyflac/libraries/linux-x86_64/
+-rwxr-xr-x   0 joe.todd   (503) staff       (20)   330216 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/linux-x86_64/libFLAC-12.1.0.so
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.439714 pyFLAC-3.0.0/pyflac/libraries/raspbian-armv7a/
+-rwxr-xr-x   0 joe.todd   (503) staff       (20)   348896 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/raspbian-armv7a/libFLAC-12.1.0.so
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.441756 pyFLAC-3.0.0/pyflac/libraries/windows-i686/
+-rw-r--r--   0 joe.todd   (503) staff       (20)   229388 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/windows-i686/FLAC-12.lib
+-rw-r--r--   0 joe.todd   (503) staff       (20)   512014 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/windows-i686/libFLAC.dll
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.443938 pyFLAC-3.0.0/pyflac/libraries/windows-x86_64/
+-rw-r--r--   0 joe.todd   (503) staff       (20)   226594 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/windows-x86_64/FLAC-12.lib
+-rw-r--r--   0 joe.todd   (503) staff       (20)   446976 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/pyflac/libraries/windows-x86_64/libFLAC.dll
+-rw-r--r--   0 joe.todd   (503) staff       (20)     1389 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/pyproject.toml
+-rw-r--r--   0 joe.todd   (503) staff       (20)       38 2024-04-16 14:20:55.456325 pyFLAC-3.0.0/setup.cfg
+-rw-r--r--   0 joe.todd   (503) staff       (20)      568 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/setup.py
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.445917 pyFLAC-3.0.0/tests/
+-rw-r--r--   0 joe.todd   (503) staff       (20)        0 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/__init__.py
+drwxr-xr-x   0 joe.todd   (503) staff       (20)        0 2024-04-16 14:20:55.452989 pyFLAC-3.0.0/tests/data/
+-rw-r--r--   0 joe.todd   (503) staff       (20)    21727 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/32bit.flac
+-rw-r--r--   0 joe.todd   (503) staff       (20)   176480 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/32bit.wav
+-rw-r--r--   0 joe.todd   (503) staff       (20)    15832 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/8bit.flac
+-rw-r--r--   0 joe.todd   (503) staff       (20)    20964 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/mono.flac
+-rw-r--r--   0 joe.todd   (503) staff       (20)    88324 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/mono.wav
+-rw-r--r--   0 joe.todd   (503) staff       (20)    73681 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/stereo.flac
+-rw-r--r--   0 joe.todd   (503) staff       (20)   264644 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/stereo.wav
+-rw-r--r--   0 joe.todd   (503) staff       (20)    65653 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/surround.flac
+-rw-r--r--   0 joe.todd   (503) staff       (20)   329980 2024-03-29 13:52:25.000000 pyFLAC-3.0.0/tests/data/surround.wav
+-rw-r--r--   0 joe.todd   (503) staff       (20)     6515 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/tests/test_decoder.py
+-rw-r--r--   0 joe.todd   (503) staff       (20)    12058 2024-04-16 13:51:03.000000 pyFLAC-3.0.0/tests/test_encoder.py
```

### Comparing `pyFLAC-2.2.0/CHANGELOG.rst` & `pyFLAC-3.0.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 pyFLAC Changelog
 ----------------
 
+**v3.0.0**
+
+* Fixed bug in the shutdown behaviour of the `StreamDecoder` (see #22 and #23).
+* Automatically detect bit depth of input data in the `FileEncoder`, and
+  raise an error if not 16-bit or 32-bit PCM (see #24).
+* Added a new `OneShotDecoder` to decode a buffer of FLAC data in a single
+  blocking operation, without the use of threads. Courtesy of @GOAE.
+
 **v2.2.0**
 
 * Updated FLAC library to v1.4.3.
     See `FLAC Changelog <https://xiph.org/flac/changelog.html>`_.
 * Added support for `int32` data
 * Added `limit_min_bitrate` property.
 * Removed support for Python 3.7
```

### Comparing `pyFLAC-2.2.0/CONTRIBUTING.rst` & `pyFLAC-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/LICENSE.txt` & `pyFLAC-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/MANIFEST.in` & `pyFLAC-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/PKG-INFO` & `pyFLAC-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: pyFLAC
-Version: 2.2.0
+Version: 3.0.0
 Summary: A Python wrapper for libFLAC
 Author-email: Joe Todd <joe.todd@sonos.com>
 License: Apache-2.0
 Keywords: lossless,compression,flac,bindings,audio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: cffi>=1.4.0
+Requires-Dist: numpy>=1.22
+Requires-Dist: SoundFile>=0.11
 
 .. image:: https://raw.githubusercontent.com/sonos/pyFLAC/develop/assets/logo-white-background.jpg
     :target: https://pyflac.readthedocs.io
 
 .. image:: https://github.com/sonos/pyFLAC/actions/workflows/lint.yml/badge.svg
     :target: https://github.com/sonos/pyFLAC/actions/workflows/lint.yml
 .. image:: https://github.com/sonos/pyFLAC/actions/workflows/test.yml/badge.svg
     :target: https://github.com/sonos/pyFLAC/actions/workflows/test.yml
-.. image:: https://github.com/sonos/pyFLAC/actions/workflows/build.yml/badge.svg
-    :target: https://github.com/sonos/pyFLAC/actions/workflows/build.yml
 .. image:: https://coveralls.io/repos/github/sonos/pyFLAC/badge.svg
     :target: https://coveralls.io/github/sonos/pyFLAC
 .. image:: https://readthedocs.org/projects/pyflac/badge
     :target: https://pyflac.readthedocs.io/en/latest/
 .. image:: https://badge.fury.io/py/pyFLAC.svg
     :target: https://badge.fury.io/py/pyFLAC
 .. image:: https://img.shields.io/pypi/pyversions/pyFLAC
```

### Comparing `pyFLAC-2.2.0/README.rst` & `pyFLAC-3.0.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 .. image:: https://raw.githubusercontent.com/sonos/pyFLAC/develop/assets/logo-white-background.jpg
     :target: https://pyflac.readthedocs.io
 
 .. image:: https://github.com/sonos/pyFLAC/actions/workflows/lint.yml/badge.svg
     :target: https://github.com/sonos/pyFLAC/actions/workflows/lint.yml
 .. image:: https://github.com/sonos/pyFLAC/actions/workflows/test.yml/badge.svg
     :target: https://github.com/sonos/pyFLAC/actions/workflows/test.yml
-.. image:: https://github.com/sonos/pyFLAC/actions/workflows/build.yml/badge.svg
-    :target: https://github.com/sonos/pyFLAC/actions/workflows/build.yml
 .. image:: https://coveralls.io/repos/github/sonos/pyFLAC/badge.svg
     :target: https://coveralls.io/github/sonos/pyFLAC
 .. image:: https://readthedocs.org/projects/pyflac/badge
     :target: https://pyflac.readthedocs.io/en/latest/
 .. image:: https://badge.fury.io/py/pyFLAC.svg
     :target: https://badge.fury.io/py/pyFLAC
 .. image:: https://img.shields.io/pypi/pyversions/pyFLAC
```

### Comparing `pyFLAC-2.2.0/examples/passthrough.py` & `pyFLAC-3.0.0/examples/passthrough.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,15 +25,24 @@
 
 class Passthrough:
 
     def __init__(self, args):
         self.idx = 0
         self.total_bytes = 0
         self.queue = queue.SimpleQueue()
-        self.data, self.sr = sf.read(args.input_file, dtype='int16', always_2d=True)
+
+        info = sf.info(str(args.input_file))
+        if info.subtype == 'PCM_16':
+            dtype = 'int16'
+        elif info.subtype == 'PCM_32':
+            dtype = 'int32'
+        else:
+            raise ValueError(f'WAV input data type must be either PCM_16 or PCM_32: Got {info.subtype}')
+
+        self.data, self.sr = sf.read(args.input_file, dtype=dtype, always_2d=True)
 
         self.encoder = pyflac.StreamEncoder(
             write_callback=self.encoder_callback,
             sample_rate=self.sr,
             blocksize=args.block_size,
         )
```

### Comparing `pyFLAC-2.2.0/examples/stream.py` & `pyFLAC-3.0.0/examples/stream.py`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyFLAC.egg-info/PKG-INFO` & `pyFLAC-3.0.0/pyFLAC.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: pyFLAC
-Version: 2.2.0
+Version: 3.0.0
 Summary: A Python wrapper for libFLAC
 Author-email: Joe Todd <joe.todd@sonos.com>
 License: Apache-2.0
 Keywords: lossless,compression,flac,bindings,audio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: cffi>=1.4.0
+Requires-Dist: numpy>=1.22
+Requires-Dist: SoundFile>=0.11
 
 .. image:: https://raw.githubusercontent.com/sonos/pyFLAC/develop/assets/logo-white-background.jpg
     :target: https://pyflac.readthedocs.io
 
 .. image:: https://github.com/sonos/pyFLAC/actions/workflows/lint.yml/badge.svg
     :target: https://github.com/sonos/pyFLAC/actions/workflows/lint.yml
 .. image:: https://github.com/sonos/pyFLAC/actions/workflows/test.yml/badge.svg
     :target: https://github.com/sonos/pyFLAC/actions/workflows/test.yml
-.. image:: https://github.com/sonos/pyFLAC/actions/workflows/build.yml/badge.svg
-    :target: https://github.com/sonos/pyFLAC/actions/workflows/build.yml
 .. image:: https://coveralls.io/repos/github/sonos/pyFLAC/badge.svg
     :target: https://coveralls.io/github/sonos/pyFLAC
 .. image:: https://readthedocs.org/projects/pyflac/badge
     :target: https://pyflac.readthedocs.io/en/latest/
 .. image:: https://badge.fury.io/py/pyFLAC.svg
     :target: https://badge.fury.io/py/pyFLAC
 .. image:: https://img.shields.io/pypi/pyversions/pyFLAC
```

### Comparing `pyFLAC-2.2.0/pyflac/__init__.py` & `pyFLAC-3.0.0/pyflac/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 
 # ------------------------------------------------------------------------------
 #
 #  pyFLAC
 #
-#  Copyright (c) 2020-2021, Sonos, Inc.
+#  Copyright (c) 2020-2024, Sonos, Inc.
 #  All rights reserved.
 #
 # ------------------------------------------------------------------------------
 
 __title__ = 'pyFLAC'
-__version__ = '2.2.0'
+__version__ = '3.0.0'
 __all__ = [
     'StreamEncoder',
     'FileEncoder',
     'EncoderState',
     'EncoderInitException',
     'EncoderProcessException',
     'StreamDecoder',
     'FileDecoder',
+    'OneShotDecoder',
     'DecoderState',
     'DecoderInitException',
     'DecoderProcessException'
 ]
 
 import os
 import platform
@@ -51,11 +52,12 @@
     EncoderState,
     EncoderInitException,
     EncoderProcessException
 )
 from .decoder import (
     StreamDecoder,
     FileDecoder,
+    OneShotDecoder,
     DecoderState,
     DecoderInitException,
     DecoderProcessException
 )
```

### Comparing `pyFLAC-2.2.0/pyflac/__main__.py` & `pyFLAC-3.0.0/pyflac/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         epilog='Convert WAV files to FLAC and vice versa'
     )
     parser.add_argument('input_file', type=Path, help='Input file to encode/decode')
     parser.add_argument('-o', '--output-file', type=Path, help='Output file')
     parser.add_argument('-c', '--compression-level', type=int, choices=range(0, 9), default=5,
                         help='0 is the fastest compression, 5 is the default, 8 is the highest compression')
     parser.add_argument('-b', '--block-size', type=int, default=0, help='The block size')
-    parser.add_argument('-d', '--dtype', default='int16', help='The encoded data type (int16 or int32)')
     parser.add_argument('-v', '--verify', action='store_false', default=True, help='Verify the compressed data')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = get_args()
@@ -41,15 +40,14 @@
     filename, extension = os.path.splitext(args.input_file)
     if header == 'RIFF':
         args.output_file = f'{filename}.flac' if args.output_file is None else args.output_file
         encoder = FileEncoder(
             input_file=args.input_file,
             output_file=args.output_file,
             blocksize=args.block_size,
-            dtype=args.dtype,
             compression_level=args.compression_level,
             verify=args.verify
         )
         encoder.process()
     elif header == 'FLAC':
         args.output_file = f'{filename}.wav' if args.output_file is None else args.output_file
         decoder = FileDecoder(args.input_file, args.output_file)
```

### Comparing `pyFLAC-2.2.0/pyflac/builder/build_args.py` & `pyFLAC-3.0.0/pyflac/builder/build_args.py`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/builder/decoder.py` & `pyFLAC-3.0.0/pyflac/builder/decoder.py`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/builder/encoder.py` & `pyFLAC-3.0.0/pyflac/builder/encoder.py`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/decoder.py` & `pyFLAC-3.0.0/pyflac/decoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # ------------------------------------------------------------------------------
 #
 #  pyFLAC decoder
 #
-#  Copyright (c) 2020-2021, Sonos, Inc.
+#  Copyright (c) 2020-2024, Sonos, Inc.
 #  All rights reserved.
 #
 # ------------------------------------------------------------------------------
 
 from collections import deque
 from enum import Enum
 import logging
@@ -89,15 +89,16 @@
     def finish(self):
         """
         Finish the decoding process.
 
         Flushes the decoding buffer, releases resources, resets the decoder
         settings to their defaults, and returns the decoder state to `DecoderState.UNINITIALIZED`.
 
-        A well behaved program should always call this at the end.
+        A well behaved program should always call this at the end, otherwise the processing
+        thread will be left running, awaiting more data.
         """
         _lib.FLAC__stream_decoder_finish(self._decoder)
 
     # -- State
 
     @property
     def state(self) -> DecoderState:
@@ -117,14 +118,17 @@
     A pyFLAC stream decoder converts a stream of FLAC encoded bytes
     back to raw audio data.
 
     The compressed data is passed in via the `process` method, and
     blocks of raw uncompressed audio is passed back to the user via
     the `callback`.
 
+    The `finish` method must be called at the end of the decoding process,
+    otherwise the processing thread will be left running.
+
     Args:
         write_callback (fn): Function to call when there is uncompressed
             audio data ready, see the example below for more information.
 
     Examples:
         An example callback which writes the audio data to file
         using SoundFile.
@@ -155,14 +159,16 @@
     """
     def __init__(self,
                  write_callback: Callable[[np.ndarray, int, int, int], None]):
         super().__init__()
 
         self._done = False
         self._buffer = deque()
+        self._event = threading.Event()
+        self._lock = threading.Lock()
         self.write_callback = write_callback
 
         rc = _lib.FLAC__stream_decoder_init_stream(
             self._decoder,
             _lib._read_callback,
             _ffi.NULL,
             _ffi.NULL,
@@ -196,15 +202,18 @@
 
         Note: This is a non-blocking function, data is processed in
         a background thread.
 
         Args:
             data (bytes): Bytes of FLAC data
         """
+        self._lock.acquire()
         self._buffer.append(data)
+        self._lock.release()
+        self._event.set()
 
     def finish(self):
         """
         Finish the decoding process.
 
         This must be called at the end of the decoding process.
 
@@ -221,16 +230,17 @@
         while self._thread.is_alive() and self._error is None and len(self._buffer) > 0:
             time.sleep(0.01)
 
         # --------------------------------------------------------------
         # Instruct the decoder to finish up and wait until it is done
         # --------------------------------------------------------------
         self._done = True
+        self._event.set()
+        self._thread.join()
         super().finish()
-        self._thread.join(timeout=3)
         if self._error:
             raise DecoderProcessException(self._error)
 
 
 class FileDecoder(_Decoder):
     """
     The pyFLAC file decoder reads the encoded audio data directly from a FLAC
@@ -299,25 +309,109 @@
             self.__output = sf.SoundFile(
                 self.__output_file, mode='w', channels=num_channels,
                 samplerate=sample_rate
             )
         self.__output.write(data)
 
 
+class OneShotDecoder(_Decoder):
+    """
+    A pyFLAC one-shot decoder converts a buffer of FLAC encoded
+    bytes back to raw audio data. Unlike the `StreamDecoder` class,
+    the one-shot decoder operates on a single block of data, and
+    runs in a blocking manner, as opposed to in a background thread.
+
+    The compressed data is passed in via the constructor, and
+    blocks of raw uncompressed audio is passed back to the user via
+    the `callback`.
+
+    Args:
+        write_callback (fn): Function to call when there is uncompressed
+            audio data ready, see the example below for more information.
+        buffer (bytes): The FLAC encoded audio data
+
+    Examples:
+        An example callback which writes the audio data to file
+        using SoundFile.
+
+        .. code-block:: python
+            :linenos:
+
+            import soundfile as sf
+
+            def callback(self,
+                         audio: np.ndarray,
+                         sample_rate: int,
+                         num_channels: int,
+                         num_samples: int):
+
+                # ------------------------------------------------------
+                # Note: num_samples is the number of samples per channel
+                # ------------------------------------------------------
+                if self.output is None:
+                    self.output = sf.SoundFile(
+                        'output.wav', mode='w', channels=num_channels,
+                        samplerate=sample_rate
+                    )
+                self.output.write(audio)
+
+    Raises:
+        DecoderInitException: If initialisation of the decoder fails
+    """
+    def __init__(self,
+                 write_callback: Callable[[np.ndarray, int, int, int], None],
+                 buffer: bytes):
+        super().__init__()
+        self._done = False
+        self._buffer = deque()
+        self._buffer.append(buffer)
+        self._event = threading.Event()
+        self._event.set()
+        self._lock = threading.Lock()
+        self.write_callback = write_callback
+
+        rc = _lib.FLAC__stream_decoder_init_stream(
+            self._decoder,
+            _lib._read_callback,
+            _ffi.NULL,
+            _ffi.NULL,
+            _ffi.NULL,
+            _ffi.NULL,
+            _lib._write_callback,
+            _ffi.NULL,
+            _lib._error_callback,
+            self._decoder_handle
+        )
+        if rc != _lib.FLAC__STREAM_DECODER_INIT_STATUS_OK:
+            raise DecoderInitException(rc)
+
+        while len(self._buffer) > 0:
+            _lib.FLAC__stream_decoder_process_single(self._decoder)
+
+        self._done = True
+        super().finish()
+
+
 @_ffi.def_extern(error=_lib.FLAC__STREAM_DECODER_READ_STATUS_ABORT)
 def _read_callback(_decoder,
                    byte_buffer,
                    num_bytes,
                    client_data):
     """
     Called internally when the decoder needs more input data.
 
     If an exception is raised here, the abort status is returned.
     """
     decoder = _ffi.from_handle(client_data)
+
+    # ----------------------------------------------------------
+    # Wait until there is something in the buffer, or an error
+    # occurs, or the end of the stream is reached.
+    # ----------------------------------------------------------
+    decoder._event.wait()
     if decoder._error:
         # ----------------------------------------------------------
         # If an error has been issued via the error callback, then
         # abort the processing of the stream.
         # ----------------------------------------------------------
         return _lib.FLAC__STREAM_DECODER_READ_STATUS_ABORT
 
@@ -325,34 +419,37 @@
         # ----------------------------------------------------------
         # The end of the stream has been instructed by a call to
         # finish.
         # ----------------------------------------------------------
         num_bytes[0] = 0
         return _lib.FLAC__STREAM_DECODER_READ_STATUS_END_OF_STREAM
 
-    maximum_bytes = int(num_bytes[0])
-    while len(decoder._buffer) == 0:
-        # ----------------------------------------------------------
-        # Wait until there is something in the buffer
-        # ----------------------------------------------------------
-        time.sleep(0.01)
-
     # --------------------------------------------------------------
     # Ensure only the maximum bytes or less is taken from
     # the thread safe queue.
     # --------------------------------------------------------------
     data = bytes()
+    maximum_bytes = int(num_bytes[0])
+    decoder._lock.acquire()
     if len(decoder._buffer[0]) <= maximum_bytes:
         data = decoder._buffer.popleft()
         maximum_bytes -= len(data)
 
     if len(decoder._buffer) > 0 and len(decoder._buffer[0]) > maximum_bytes:
         data += decoder._buffer[0][0:maximum_bytes]
         decoder._buffer[0] = decoder._buffer[0][maximum_bytes:]
 
+    # --------------------------------------------------------------
+    # If there is no more data to process from the buffer, then
+    # clear the event, the thread will await more data to process.
+    # --------------------------------------------------------------
+    if len(decoder._buffer) == 0 or (len(decoder._buffer) > 0 and len(decoder._buffer[0]) == 0):
+        decoder._event.clear()
+    decoder._lock.release()
+
     actual_bytes = len(data)
     num_bytes[0] = actual_bytes
     _ffi.memmove(byte_buffer, data, actual_bytes)
     return _lib.FLAC__STREAM_DECODER_READ_STATUS_CONTINUE
 
 
 @_ffi.def_extern()
@@ -445,7 +542,8 @@
     Called whenever an error occurs during decoding.
     """
     decoder = _ffi.from_handle(client_data)
     message = _ffi.string(
         _lib.FLAC__StreamDecoderErrorStatusString[status]).decode()
     decoder.logger.error(f'Error in libFLAC decoder: {message}')
     decoder._error = message
+    decoder._event.set()
```

### Comparing `pyFLAC-2.2.0/pyflac/encoder.py` & `pyFLAC-3.0.0/pyflac/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # ------------------------------------------------------------------------------
 #
 #  pyFLAC encoder
 #
-#  Copyright (c) 2020-2021, Sonos, Inc.
+#  Copyright (c) 2020-2024, Sonos, Inc.
 #  All rights reserved.
 #
 # ------------------------------------------------------------------------------
 
 from enum import Enum
 import logging
 from pathlib import Path
@@ -331,26 +331,26 @@
 
 
 class FileEncoder(_Encoder):
     """
     The pyFLAC file encoder reads the raw audio data from the WAV file and
     writes the encoded audio data to a FLAC file.
 
+    Note that the input WAV file must be either PCM_16 or PCM_32.
+
     Args:
         input_file (pathlib.Path): Path to the input WAV file
         output_file (pathlib.Path): Path to the output FLAC file, a temporary
             file will be created if unspecified.
         compression_level (int): The compression level parameter that
             varies from 0 (fastest) to 8 (slowest). The default setting
             is 5, see https://en.wikipedia.org/wiki/FLAC for more details.
         blocksize (int): The size of the block to be returned in the
             callback. The default is 0 which allows libFLAC to determine
             the best block size.
-        dtype (str): The data type to use in the FLAC encoder, either int16 or int32,
-            defaults to int16.
         streamable_subset (bool): Whether to use the streamable subset for encoding.
             If true the encoder will check settings for compatibility. If false,
             the settings may take advantage of the full range that the format allows.
         verify (bool): If `True`, the encoder will verify it's own
             encoded output by feeding it through an internal decoder and
             comparing the original signal against the decoded signal.
             If a mismatch occurs, the `process` method will raise a
@@ -361,21 +361,25 @@
         ValueError: If any invalid values are passed in to the constructor.
     """
     def __init__(self,
                  input_file: Path,
                  output_file: Path = None,
                  compression_level: int = 5,
                  blocksize: int = 0,
-                 dtype: str = 'int16',
                  streamable_subset: bool = True,
                  verify: bool = False):
         super().__init__()
 
-        if dtype not in ('int16', 'int32'):
-            raise ValueError('FLAC encoding data type must be either int16 or int32')
+        info = sf.info(str(input_file))
+        if info.subtype == 'PCM_16':
+            dtype = 'int16'
+        elif info.subtype == 'PCM_32':
+            dtype = 'int32'
+        else:
+            raise ValueError(f'WAV input data type must be either PCM_16 or PCM_32: Got {info.subtype}')
 
         self.__raw_audio, sample_rate = sf.read(str(input_file), dtype=dtype)
         if output_file:
             self.__output_file = output_file
         else:
             output_file = tempfile.NamedTemporaryFile(suffix='.flac')
             self.__output_file = Path(output_file.name)
```

### Comparing `pyFLAC-2.2.0/pyflac/include/FLAC/export.h` & `pyFLAC-3.0.0/pyflac/include/FLAC/export.h`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/include/FLAC/format.h` & `pyFLAC-3.0.0/pyflac/include/FLAC/format.h`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/include/FLAC/ordinals.h` & `pyFLAC-3.0.0/pyflac/include/FLAC/ordinals.h`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/include/FLAC/stream_decoder.h` & `pyFLAC-3.0.0/pyflac/include/FLAC/stream_decoder.h`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/include/FLAC/stream_encoder.h` & `pyFLAC-3.0.0/pyflac/include/FLAC/stream_encoder.h`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/LICENSE` & `pyFLAC-3.0.0/pyflac/libraries/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/darwin-arm64/libFLAC.12.dylib` & `pyFLAC-3.0.0/pyflac/libraries/darwin-arm64/libFLAC.12.dylib`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/darwin-x86_64/libFLAC.12.dylib` & `pyFLAC-3.0.0/pyflac/libraries/darwin-x86_64/libFLAC.12.dylib`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/linux-arm64/libFLAC-12.1.0.so` & `pyFLAC-3.0.0/pyflac/libraries/linux-arm64/libFLAC-12.1.0.so`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/linux-x86_64/libFLAC-12.1.0.so` & `pyFLAC-3.0.0/pyflac/libraries/linux-x86_64/libFLAC-12.1.0.so`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/raspbian-armv7a/libFLAC-12.1.0.so` & `pyFLAC-3.0.0/pyflac/libraries/raspbian-armv7a/libFLAC-12.1.0.so`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/windows-i686/FLAC-12.lib` & `pyFLAC-3.0.0/pyflac/libraries/windows-i686/FLAC-12.lib`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/windows-i686/libFLAC.dll` & `pyFLAC-3.0.0/pyflac/libraries/windows-i686/libFLAC.dll`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/windows-x86_64/FLAC-12.lib` & `pyFLAC-3.0.0/pyflac/libraries/windows-x86_64/FLAC-12.lib`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyflac/libraries/windows-x86_64/libFLAC.dll` & `pyFLAC-3.0.0/pyflac/libraries/windows-x86_64/libFLAC.dll`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/pyproject.toml` & `pyFLAC-3.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # ------------------------------------------------------------------------------
 #
 #  pyFLAC
 #
-#  Copyright (c) 2020-2023, Sonos, Inc.
+#  Copyright (c) 2020-2024, Sonos, Inc.
 #  All rights reserved.
 #
 # ------------------------------------------------------------------------------
 [build-system]
 requires = ["setuptools>=42", "cffi>=1.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyFLAC"
-version = "2.2.0"
+version = "3.0.0"
 description = "A Python wrapper for libFLAC"
 readme = "README.rst"
 authors = [{ name = "Joe Todd", email = "joe.todd@sonos.com" }]
 requires-python = ">=3.8"
 license = { text = "Apache-2.0" }
 keywords = ["lossless", "compression", "flac", "bindings", "audio"]
 classifiers = [
@@ -25,14 +25,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Multimedia :: Sound/Audio",
 ]
 dependencies = ["cffi>=1.4.0", "numpy>=1.22", "SoundFile>=0.11"]
 
 [project.scripts]
 pyflac = "pyflac.__main__:main"
```

### Comparing `pyFLAC-2.2.0/setup.py` & `pyFLAC-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/32bit.flac` & `pyFLAC-3.0.0/tests/data/32bit.flac`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/32bit.wav` & `pyFLAC-3.0.0/tests/data/32bit.wav`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/8bit.flac` & `pyFLAC-3.0.0/tests/data/8bit.flac`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/mono.flac` & `pyFLAC-3.0.0/tests/data/mono.flac`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/mono.wav` & `pyFLAC-3.0.0/tests/data/mono.wav`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/stereo.flac` & `pyFLAC-3.0.0/tests/data/stereo.flac`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/stereo.wav` & `pyFLAC-3.0.0/tests/data/stereo.wav`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/surround.flac` & `pyFLAC-3.0.0/tests/data/surround.flac`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/data/surround.wav` & `pyFLAC-3.0.0/tests/data/surround.wav`

 * *Files identical despite different names*

### Comparing `pyFLAC-2.2.0/tests/test_decoder.py` & `pyFLAC-3.0.0/tests/test_decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # ------------------------------------------------------------------------------
 #
 #  pyFLAC decoder test suite
 #
-#  Copyright (c) 2020-2021, Sonos, Inc.
+#  Copyright (c) 2020-2024, Sonos, Inc.
 #  All rights reserved.
 #
 # ------------------------------------------------------------------------------
 
 import os
 import pathlib
 import tempfile
@@ -16,14 +16,15 @@
 import unittest
 
 import numpy as np
 from pyflac.decoder import _Decoder
 from pyflac import (
     FileDecoder,
     StreamDecoder,
+    OneShotDecoder,
     DecoderState,
     DecoderInitException,
     DecoderProcessException
 )
 
 
 class TestDecoder(unittest.TestCase):
@@ -72,14 +73,15 @@
 
         self.decoder = StreamDecoder(write_callback=self._write_callback)
         time.sleep(0.05)
 
         self.decoder.process(test_data)
         self.decoder.finish()
         self.assertTrue(self.write_callback_called)
+        self.assertFalse(self.decoder._thread.is_alive())
 
     def test_process_blocks(self):
         """ Test that FLAC data can be decoded in blocks """
         blocksize = 1024
         test_path = self.tests_path / 'data/stereo.flac'
         with open(test_path, 'rb') as flac:
             test_data = flac.read()
@@ -145,9 +147,35 @@
         test_file = pathlib.Path(__file__).parent / 'data/32bit.flac'
         self.default_kwargs['input_file'] = test_file
         self.default_kwargs['output_file'] = pathlib.Path(self.temp_file.name)
         self.decoder = FileDecoder(**self.default_kwargs)
         self.assertIsNotNone(self.decoder.process())
 
 
+class TestOneShotDecoder(unittest.TestCase):
+    """
+    Test suite for the one-shot decoder class.
+    """
+    def setUp(self):
+        self.decoder = None
+        self.write_callback_called = False
+        self.tests_path = pathlib.Path(__file__).parent.absolute()
+
+    def _write_callback(self, data, rate, channels, samples):
+        assert isinstance(data, np.ndarray)
+        assert isinstance(rate, int)
+        assert isinstance(channels, int)
+        assert isinstance(samples, int)
+        self.write_callback_called = True
+
+    def test_process(self):
+        """ Test that FLAC data can be decoded """
+        test_path = self.tests_path / 'data/stereo.flac'
+        with open(test_path, 'rb') as flac:
+            test_data = flac.read()
+
+        self.decoder = OneShotDecoder(write_callback=self._write_callback, buffer=test_data)
+        self.assertTrue(self.write_callback_called)
+
+
 if __name__ == '__main__':
     unittest.main(failfast=True)
```

### Comparing `pyFLAC-2.2.0/tests/test_encoder.py` & `pyFLAC-3.0.0/tests/test_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # ------------------------------------------------------------------------------
 #
 #  pyFLAC encoder test suite
 #
-#  Copyright (c) 2020-2021, Sonos, Inc.
+#  Copyright (c) 2020-2024, Sonos, Inc.
 #  All rights reserved.
 #
 # ------------------------------------------------------------------------------
 
 import pathlib
 import tempfile
 import unittest
@@ -233,20 +233,14 @@
     def test_invalid_blocksize(self):
         """ Test than an exception is raised if given an invalid block size """
         self.default_kwargs['blocksize'] = 1000000
         self.encoder = FileEncoder(**self.default_kwargs)
         with self.assertRaisesRegex(EncoderInitException, 'FLAC__STREAM_ENCODER_INIT_STATUS_INVALID_BLOCK_SIZE'):
             self.encoder._init()
 
-    def test_invalid_dtype(self):
-        """ Test than an exception is raised if given an invalid dtype """
-        self.default_kwargs['dtype'] = 'int24'
-        with self.assertRaisesRegex(ValueError, 'FLAC encoding data type must be either int16 or int32'):
-            self.encoder = FileEncoder(**self.default_kwargs)
-
     def test_blocksize_streamable_subset(self):
         """ Test that an exception is raised if blocksize is outside the streamable subset """
         self.default_kwargs['blocksize'] = 65535
         self.encoder = FileEncoder(**self.default_kwargs)
         with self.assertRaisesRegex(EncoderInitException, 'FLAC__STREAM_ENCODER_INIT_STATUS_NOT_STREAMABLE'):
             self.encoder._init()
 
@@ -287,14 +281,13 @@
         self.encoder.process()
 
     def test_process_32_bit_file(self):
         """ Test that a 32 bit WAV file can be processed """
         test_path = pathlib.Path(__file__).parent.absolute() / 'data/32bit.wav'
         self.default_kwargs['input_file'] = test_path
         self.default_kwargs['output_file'] = pathlib.Path(self.temp_file.name)
-        self.default_kwargs['dtype'] = 'int32'
         self.encoder = FileEncoder(**self.default_kwargs)
         self.encoder.process()
 
 
 if __name__ == '__main__':
     unittest.main(failfast=True)
```

