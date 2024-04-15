# Comparing `tmp/sts_lib-0.23.0.tar.gz` & `tmp/sts_lib-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.23.0.tar", last modified: Sun Apr 14 08:56:06 2024, max compression
+gzip compressed data, was "sts_lib-0.24.0.tar", last modified: Mon Apr 15 17:16:41 2024, max compression
```

## Comparing `sts_lib-0.23.0.tar` & `sts_lib-0.24.0.tar`

### file list

```diff
@@ -1,55 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.574401 sts_lib-0.23.0/
--rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts_lib-0.23.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-08 13:49:48.000000 sts_lib-0.23.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7172 2024-04-14 08:56:06.574401 sts_lib-0.23.0/PKG-INFO
--rw-rw-rw-   0        0        0     5830 2024-04-14 08:53:14.000000 sts_lib-0.23.0/README.md
--rw-rw-rw-   0        0        0     1687 2024-04-14 08:56:06.575400 sts_lib-0.23.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-08 13:49:48.000000 sts_lib-0.23.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.522474 sts_lib-0.23.0/sts/
--rw-rw-rw-   0        0        0    41481 2024-04-14 08:53:14.000000 sts_lib-0.23.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-08 13:49:45.000000 sts_lib-0.23.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7754 2024-04-14 08:53:14.000000 sts_lib-0.23.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.524455 sts_lib-0.23.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.540436 sts_lib-0.23.0/sts/data/config/
--rw-rw-rw-   0        0        0      653 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      369 2020-08-12 18:29:24.000000 sts_lib-0.23.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      275 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      323 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      289 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      201 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      287 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      369 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      197 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      211 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      201 2020-07-16 15:29:01.000000 sts_lib-0.23.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      195 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      367 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      413 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      273 2020-07-12 06:22:39.000000 sts_lib-0.23.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.559417 sts_lib-0.23.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-14 07:55:14.000000 sts_lib-0.23.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2020-07-12 14:58:22.000000 sts_lib-0.23.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    21012 2024-04-14 08:53:14.000000 sts_lib-0.23.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.563415 sts_lib-0.23.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-14 08:48:53.000000 sts_lib-0.23.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2020-07-10 16:04:12.000000 sts_lib-0.23.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-14 08:56:06.571405 sts_lib-0.23.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     7172 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      170 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-14 08:56:06.000000 sts_lib-0.23.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.881226 sts_lib-0.24.0/
+-rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts_lib-0.24.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-08 13:49:48.000000 sts_lib-0.24.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7650 2024-04-15 17:16:41.881226 sts_lib-0.24.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6197 2024-04-15 14:44:56.000000 sts_lib-0.24.0/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-15 17:16:41.882239 sts_lib-0.24.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-08 13:49:48.000000 sts_lib-0.24.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.816144 sts_lib-0.24.0/sts/
+-rw-rw-rw-   0        0        0    43648 2024-04-15 14:45:47.000000 sts_lib-0.24.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-08 13:49:45.000000 sts_lib-0.24.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7803 2024-04-15 14:45:56.000000 sts_lib-0.24.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.817143 sts_lib-0.24.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.840678 sts_lib-0.24.0/sts/data/config/
+-rw-rw-rw-   0        0        0     1225 2024-04-15 14:45:58.000000 sts_lib-0.24.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      642 2024-04-15 14:45:59.000000 sts_lib-0.24.0/sts/data/config/_extend.json
+-rw-rw-rw-   0        0        0      383 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      458 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/config/hk2sp.json
+-rw-rw-rw-   0        0        0      518 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/config/hk2spx.json
+-rw-rw-rw-   0        0        0      446 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/hk2sx.json
+-rw-rw-rw-   0        0        0      289 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      368 2024-04-15 14:45:56.000000 sts_lib-0.24.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      334 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      376 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/config/s2hkp.json
+-rw-rw-rw-   0        0        0      244 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      332 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      413 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      211 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      374 2024-04-15 14:45:59.000000 sts_lib-0.24.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      435 2024-04-15 14:45:59.000000 sts_lib-0.24.0/sts/data/config/t2jpx.json
+-rw-rw-rw-   0        0        0      215 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      276 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/t2sx.json
+-rw-rw-rw-   0        0        0      209 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      381 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      455 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      516 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/config/tw2spx.json
+-rw-rw-rw-   0        0        0      444 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/config/tw2sx.json
+-rw-rw-rw-   0        0        0      287 2024-04-15 13:10:46.000000 sts_lib-0.24.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.864658 sts_lib-0.24.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0       32 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/dictionary/HKPhrases.txt
+-rw-rw-rw-   0        0        0       47 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/dictionary/HKPhrasesRev.txt
+-rw-rw-rw-   0        0        0      604 2024-04-15 14:45:53.000000 sts_lib-0.24.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2020-07-10 16:04:12.000000 sts_lib-0.24.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      243 2024-04-15 14:45:59.000000 sts_lib-0.24.0/sts/data/dictionary/JPKyujitaiCharacters.txt
+-rw-rw-rw-   0        0        0      193 2024-04-15 14:46:01.000000 sts_lib-0.24.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2020-07-10 16:04:12.000000 sts_lib-0.24.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3235 2024-04-15 14:46:04.000000 sts_lib-0.24.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0      969 2024-04-15 14:46:04.000000 sts_lib-0.24.0/sts/data/dictionary/JPVariantsEx.txt
+-rw-rw-rw-   0        0        0    26463 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0    37567 2024-04-15 14:45:52.000000 sts_lib-0.24.0/sts/data/dictionary/STCharactersEx.txt
+-rw-rw-rw-   0        0        0  1053396 2024-04-15 14:46:05.000000 sts_lib-0.24.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    34102 2024-04-15 14:45:55.000000 sts_lib-0.24.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0    37436 2024-04-15 14:45:52.000000 sts_lib-0.24.0/sts/data/dictionary/TSCharactersEx.txt
+-rw-rw-rw-   0        0        0     5642 2024-04-15 14:46:05.000000 sts_lib-0.24.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-15 14:46:06.000000 sts_lib-0.24.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2020-07-10 16:04:12.000000 sts_lib-0.24.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-15 14:46:03.000000 sts_lib-0.24.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      257 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/dictionary/TWPhrasesRev.txt
+-rw-rw-rw-   0        0        0      360 2024-04-15 14:45:53.000000 sts_lib-0.24.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2020-07-12 14:58:22.000000 sts_lib-0.24.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    21012 2024-04-14 08:53:14.000000 sts_lib-0.24.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.871269 sts_lib-0.24.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    22034 2024-04-15 14:45:54.000000 sts_lib-0.24.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0    60986 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/scheme/st_unihan13.txt
+-rw-rw-rw-   0        0        0     3957 2024-04-15 14:46:04.000000 sts_lib-0.24.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0    49876 2024-04-15 14:45:49.000000 sts_lib-0.24.0/sts/data/scheme/ts_tgh_convert.txt
+-rw-rw-rw-   0        0        0    81246 2024-04-15 14:45:49.000000 sts_lib-0.24.0/sts/data/scheme/ts_tgh_list.txt
+-rw-rw-rw-   0        0        0    61047 2024-04-15 14:45:50.000000 sts_lib-0.24.0/sts/data/scheme/ts_unihan13.txt
+-rw-rw-rw-   0        0        0     2108 2020-07-10 16:04:12.000000 sts_lib-0.24.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 17:16:41.879229 sts_lib-0.24.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     7650 2024-04-15 17:16:41.000000 sts_lib-0.24.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1970 2024-04-15 17:16:41.000000 sts_lib-0.24.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:16:41.000000 sts_lib-0.24.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-15 17:16:41.000000 sts_lib-0.24.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-15 17:16:41.000000 sts_lib-0.24.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-15 17:16:41.000000 sts_lib-0.24.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.23.0/LICENSE` & `sts_lib-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/PKG-INFO` & `sts_lib-0.24.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.23.0
+Version: 0.24.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: yaml
+Requires-Dist: pyyaml>=5.0; extra == "yaml"
 Provides-Extra: dev
+Requires-Dist: pyyaml>=5.0; extra == "dev"
 Requires-Dist: flake8>=4.0; extra == "dev"
 Requires-Dist: flake8-quotes>=3.4; extra == "dev"
 Requires-Dist: flake8-comprehensions>=3.7; extra == "dev"
 Requires-Dist: flake8-string-format>=0.3; extra == "dev"
 Requires-Dist: pep8-naming>=0.13.2; extra == "dev"
 Requires-Dist: flake8-bugbear>=22.0; extra == "dev"
 Requires-Dist: flake8-isort>=4.2; extra == "dev"
@@ -108,32 +111,37 @@
  *     directory of this config file, or the basename of a built-in config file
  *     (with or without ".json")
  * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
  */
 
 /**
  * @typedef {Object} dictScheme
- * @property {string} file - path of the dictionary file to generate. Each as
- *     an absolute path, or a path relative to the specified output directory
- *     (or the directory of this config file). Each should be a .tlist
- *     (compiled trie), .jlist (compiled table), or .list (plain text table).
+ * @property {string} file - path of the dictionary file to generate, as an
+ *     absolute path, or a path relative to the specified output directory
+ *     (or the directory of this config file). It should be a .tlist (compiled
+ *     trie), .jlist (compiled table), or .list (plain text table).
  * @property {string} mode - the mode to handle the loaded source files: "load"
  *     to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
  * @property {Array.<(string|string[])>} src - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
- *     or the basename of a built-in dictionary file. Each should be a .txt or
- *     .list dictionary file.
+ *     or the basename of a built-in dictionary file. Each should be a .txt,
+ *     .list, .json, .jlist, .yaml, or .yml dictionary file.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
  * @property {string} [include] - a regex filter that discards non-matched
  *     conversion values.
  * @property {string} [exclude] - a regex filter that discards matched
  *     conversion values.
+ * @property {boolean} [check] - true to raise an exception if the output
+ *     contains an invalid char which will be loaded incorrectly. Set this
+ *     when the output is a plain text table file and the source files contain
+ *     untrusted JSON or YAML data that may include a char like " ", "\t",
+ *     "\n", etc. in the dictionary.
  */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
```

### Comparing `sts_lib-0.23.0/README.md` & `sts_lib-0.24.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,32 +76,37 @@
  *     directory of this config file, or the basename of a built-in config file
  *     (with or without ".json")
  * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
  */
 
 /**
  * @typedef {Object} dictScheme
- * @property {string} file - path of the dictionary file to generate. Each as
- *     an absolute path, or a path relative to the specified output directory
- *     (or the directory of this config file). Each should be a .tlist
- *     (compiled trie), .jlist (compiled table), or .list (plain text table).
+ * @property {string} file - path of the dictionary file to generate, as an
+ *     absolute path, or a path relative to the specified output directory
+ *     (or the directory of this config file). It should be a .tlist (compiled
+ *     trie), .jlist (compiled table), or .list (plain text table).
  * @property {string} mode - the mode to handle the loaded source files: "load"
  *     to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
  * @property {Array.<(string|string[])>} src - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
- *     or the basename of a built-in dictionary file. Each should be a .txt or
- *     .list dictionary file.
+ *     or the basename of a built-in dictionary file. Each should be a .txt,
+ *     .list, .json, .jlist, .yaml, or .yml dictionary file.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
  * @property {string} [include] - a regex filter that discards non-matched
  *     conversion values.
  * @property {string} [exclude] - a regex filter that discards matched
  *     conversion values.
+ * @property {boolean} [check] - true to raise an exception if the output
+ *     contains an invalid char which will be loaded incorrectly. Set this
+ *     when the output is a plain text table file and the source files contain
+ *     untrusted JSON or YAML data that may include a char like " ", "\t",
+ *     "\n", etc. in the dictionary.
  */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
```

### Comparing `sts_lib-0.23.0/setup.cfg` & `sts_lib-0.24.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -47,60 +47,62 @@
 000002e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
 00000300: 203a 3a20 332e 3132 0d0a 0d0a 5b6f 7074   :: 3.12....[opt
 00000310: 696f 6e73 5d0d 0a70 7974 686f 6e5f 7265  ions]..python_re
 00000320: 7175 6972 6573 203d 207e 3d33 2e37 0d0a  quires = ~=3.7..
 00000330: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
 00000340: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
-00000350: 7261 735f 7265 7175 6972 655d 0d0a 6465  ras_require]..de
-00000360: 7620 3d20 0d0a 0966 6c61 6b65 3820 3e3d  v = ...flake8 >=
-00000370: 2034 2e30 0d0a 0966 6c61 6b65 382d 7175   4.0...flake8-qu
-00000380: 6f74 6573 203e 3d20 332e 340d 0a09 666c  otes >= 3.4...fl
-00000390: 616b 6538 2d63 6f6d 7072 6568 656e 7369  ake8-comprehensi
-000003a0: 6f6e 7320 3e3d 2033 2e37 0d0a 0966 6c61  ons >= 3.7...fla
-000003b0: 6b65 382d 7374 7269 6e67 2d66 6f72 6d61  ke8-string-forma
-000003c0: 7420 3e3d 2030 2e33 0d0a 0970 6570 382d  t >= 0.3...pep8-
-000003d0: 6e61 6d69 6e67 203e 3d20 302e 3133 2e32  naming >= 0.13.2
-000003e0: 0d0a 0966 6c61 6b65 382d 6275 6762 6561  ...flake8-bugbea
-000003f0: 7220 3e3d 2032 322e 300d 0a09 666c 616b  r >= 22.0...flak
-00000400: 6538 2d69 736f 7274 203e 3d20 342e 320d  e8-isort >= 4.2.
-00000410: 0a09 6973 6f72 7420 3e3d 2035 2e35 0d0a  ..isort >= 5.5..
-00000420: 0974 6f78 203e 3d20 342e 300d 0a0d 0a5b  .tox >= 4.0....[
-00000430: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000440: 2e66 696e 645d 0d0a 6578 636c 7564 6520  .find]..exclude 
-00000450: 3d20 7465 7374 730d 0a0d 0a5b 6f70 7469  = tests....[opti
-00000460: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000470: 5d0d 0a73 7473 203d 200d 0a09 6461 7461  ]..sts = ...data
-00000480: 2f2a 2e68 746d 6c0d 0a09 6461 7461 2f63  /*.html...data/c
-00000490: 6f6e 6669 672f 2a2e 6a73 6f6e 0d0a 0964  onfig/*.json...d
-000004a0: 6174 612f 6469 6374 696f 6e61 7279 2f2a  ata/dictionary/*
-000004b0: 2e74 7874 0d0a 0964 6174 612f 7363 6865  .txt...data/sche
-000004c0: 6d65 2f2a 2e74 7874 0d0a 0d0a 5b6f 7074  me/*.txt....[opt
-000004d0: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
-000004e0: 735d 0d0a 636f 6e73 6f6c 655f 7363 7269  s]..console_scri
-000004f0: 7074 7320 3d20 0d0a 0973 7473 203d 2073  pts = ...sts = s
-00000500: 7473 2e63 6c69 3a6d 6169 6e0d 0a0d 0a5b  ts.cli:main....[
-00000510: 666c 616b 6538 5d0d 0a65 7863 6c75 6465  flake8]..exclude
-00000520: 203d 2062 7569 6c64 2c20 2e67 6974 0d0a   = build, .git..
-00000530: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
-00000540: 3d20 3136 300d 0a65 7874 656e 642d 7365  = 160..extend-se
-00000550: 6c65 6374 203d 200d 0a09 4531 3233 0d0a  lect = ...E123..
-00000560: 6967 6e6f 7265 203d 200d 0a09 5735 3033  ignore = ...W503
-00000570: 0d0a 6967 6e6f 7265 2d6e 616d 6573 203d  ..ignore-names =
-00000580: 200d 0a09 7365 7455 700d 0a09 7465 6172   ...setUp...tear
-00000590: 446f 776e 0d0a 0973 6574 5570 436c 6173  Down...setUpClas
-000005a0: 730d 0a09 7465 6172 446f 776e 436c 6173  s...tearDownClas
-000005b0: 730d 0a09 7365 7455 704d 6f64 756c 650d  s...setUpModule.
-000005c0: 0a09 7465 6172 446f 776e 4d6f 6475 6c65  ..tearDownModule
-000005d0: 0d0a 0961 7379 6e63 5365 7455 700d 0a09  ...asyncSetUp...
-000005e0: 6173 796e 6354 6561 7244 6f77 6e0d 0a09  asyncTearDown...
-000005f0: 7365 7455 7054 6573 7444 6174 610d 0a09  setUpTestData...
-00000600: 6661 696c 7572 6545 7863 6570 7469 6f6e  failureException
-00000610: 0d0a 096c 6f6e 674d 6573 7361 6765 0d0a  ...longMessage..
-00000620: 096d 6178 4469 6666 0d0a 0d0a 5b69 736f  .maxDiff....[iso
-00000630: 7274 5d0d 0a6d 756c 7469 5f6c 696e 655f  rt]..multi_line_
-00000640: 6f75 7470 7574 203d 2033 0d0a 696e 636c  output = 3..incl
-00000650: 7564 655f 7472 6169 6c69 6e67 5f63 6f6d  ude_trailing_com
-00000660: 6d61 203d 2074 7275 650d 0a0d 0a5b 6567  ma = true....[eg
-00000670: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000680: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000690: 3d20 300d 0a0d 0a                        = 0....
+00000350: 7261 735f 7265 7175 6972 655d 0d0a 7961  ras_require]..ya
+00000360: 6d6c 203d 200d 0a09 7079 7961 6d6c 203e  ml = ...pyyaml >
+00000370: 3d20 352e 300d 0a64 6576 203d 200d 0a09  = 5.0..dev = ...
+00000380: 7079 7961 6d6c 203e 3d20 352e 300d 0a09  pyyaml >= 5.0...
+00000390: 666c 616b 6538 203e 3d20 342e 300d 0a09  flake8 >= 4.0...
+000003a0: 666c 616b 6538 2d71 756f 7465 7320 3e3d  flake8-quotes >=
+000003b0: 2033 2e34 0d0a 0966 6c61 6b65 382d 636f   3.4...flake8-co
+000003c0: 6d70 7265 6865 6e73 696f 6e73 203e 3d20  mprehensions >= 
+000003d0: 332e 370d 0a09 666c 616b 6538 2d73 7472  3.7...flake8-str
+000003e0: 696e 672d 666f 726d 6174 203e 3d20 302e  ing-format >= 0.
+000003f0: 330d 0a09 7065 7038 2d6e 616d 696e 6720  3...pep8-naming 
+00000400: 3e3d 2030 2e31 332e 320d 0a09 666c 616b  >= 0.13.2...flak
+00000410: 6538 2d62 7567 6265 6172 203e 3d20 3232  e8-bugbear >= 22
+00000420: 2e30 0d0a 0966 6c61 6b65 382d 6973 6f72  .0...flake8-isor
+00000430: 7420 3e3d 2034 2e32 0d0a 0969 736f 7274  t >= 4.2...isort
+00000440: 203e 3d20 352e 350d 0a09 746f 7820 3e3d   >= 5.5...tox >=
+00000450: 2034 2e30 0d0a 0d0a 5b6f 7074 696f 6e73   4.0....[options
+00000460: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000470: 0a65 7863 6c75 6465 203d 2074 6573 7473  .exclude = tests
+00000480: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000490: 6b61 6765 5f64 6174 615d 0d0a 7374 7320  kage_data]..sts 
+000004a0: 3d20 0d0a 0964 6174 612f 2a2e 6874 6d6c  = ...data/*.html
+000004b0: 0d0a 0964 6174 612f 636f 6e66 6967 2f2a  ...data/config/*
+000004c0: 2e6a 736f 6e0d 0a09 6461 7461 2f64 6963  .json...data/dic
+000004d0: 7469 6f6e 6172 792f 2a2e 7478 740d 0a09  tionary/*.txt...
+000004e0: 6461 7461 2f73 6368 656d 652f 2a2e 7478  data/scheme/*.tx
+000004f0: 740d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  t....[options.en
+00000500: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+00000510: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+00000520: 0a09 7374 7320 3d20 7374 732e 636c 693a  ..sts = sts.cli:
+00000530: 6d61 696e 0d0a 0d0a 5b66 6c61 6b65 385d  main....[flake8]
+00000540: 0d0a 6578 636c 7564 6520 3d20 6275 696c  ..exclude = buil
+00000550: 642c 202e 6769 740d 0a6d 6178 2d6c 696e  d, .git..max-lin
+00000560: 652d 6c65 6e67 7468 203d 2031 3630 0d0a  e-length = 160..
+00000570: 6578 7465 6e64 2d73 656c 6563 7420 3d20  extend-select = 
+00000580: 0d0a 0945 3132 330d 0a69 676e 6f72 6520  ...E123..ignore 
+00000590: 3d20 0d0a 0957 3530 330d 0a69 676e 6f72  = ...W503..ignor
+000005a0: 652d 6e61 6d65 7320 3d20 0d0a 0973 6574  e-names = ...set
+000005b0: 5570 0d0a 0974 6561 7244 6f77 6e0d 0a09  Up...tearDown...
+000005c0: 7365 7455 7043 6c61 7373 0d0a 0974 6561  setUpClass...tea
+000005d0: 7244 6f77 6e43 6c61 7373 0d0a 0973 6574  rDownClass...set
+000005e0: 5570 4d6f 6475 6c65 0d0a 0974 6561 7244  UpModule...tearD
+000005f0: 6f77 6e4d 6f64 756c 650d 0a09 6173 796e  ownModule...asyn
+00000600: 6353 6574 5570 0d0a 0961 7379 6e63 5465  cSetUp...asyncTe
+00000610: 6172 446f 776e 0d0a 0973 6574 5570 5465  arDown...setUpTe
+00000620: 7374 4461 7461 0d0a 0966 6169 6c75 7265  stData...failure
+00000630: 4578 6365 7074 696f 6e0d 0a09 6c6f 6e67  Exception...long
+00000640: 4d65 7373 6167 650d 0a09 6d61 7844 6966  Message...maxDif
+00000650: 660d 0a0d 0a5b 6973 6f72 745d 0d0a 6d75  f....[isort]..mu
+00000660: 6c74 695f 6c69 6e65 5f6f 7574 7075 7420  lti_line_output 
+00000670: 3d20 330d 0a69 6e63 6c75 6465 5f74 7261  = 3..include_tra
+00000680: 696c 696e 675f 636f 6d6d 6120 3d20 7472  iling_comma = tr
+00000690: 7565 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ue....[egg_info]
+000006a0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000006b0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `sts_lib-0.23.0/sts/__init__.py` & `sts_lib-0.24.0/sts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 """An open library for flexible simplified-traditional Chinese text conversion.
 """
 import html
+import itertools
 import json
 import math
 import os
 import re
 import sys
 from collections import namedtuple
 from contextlib import nullcontext
@@ -43,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.23.0'
+__version__ = '0.24.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -288,44 +289,85 @@
         Args:
             skip_check: True to skip checking duplicated values.
         """
         for key, values in stsdict.items():
             self.add(key, values, skip_check=skip_check)
         return self
 
-    def load(self, *files):
-        """Add all key-values pairs from plain-dict file(s).
+    def load(self, *files, type=None):
+        """Add all key-values pairs from dict file(s).
         """
         for file in files:
-            with open(file, 'r', encoding='UTF-8') as fh:
-                for line in fh:
-                    try:
-                        key, values, *_ = line.rstrip('\n').split('\t')
-                    except ValueError:
-                        pass
-                    else:
-                        self.add(key, values.split(' '))
+            t = os.path.splitext(file)[1][1:].lower() if type is None else type
+            if t in ('json', 'jlist'):
+                self._load_json(file)
+            elif t in ('yaml', 'yml'):
+                self._load_yaml(file)
+            else:
+                self._load_plain(file)
         return self
 
-    def dump(self, file=None, sort=False):
+    def _load_plain(self, file):
+        with open(file, 'r', encoding='UTF-8') as fh:
+            for line in fh:
+                try:
+                    key, values, *_ = line.rstrip('\n').split('\t')
+                except ValueError:
+                    pass
+                else:
+                    self.add(key, values.split(' '))
+
+    def _load_json(self, file):
+        with open(file, 'r', encoding='UTF-8') as fh:
+            data = json.load(fh)
+            if not isinstance(data, dict):
+                data = dict(data)
+            for key, values in data.items():
+                self.add(key, values)
+
+    def _load_yaml(self, file):
+        try:
+            import yaml
+        except ModuleNotFoundError:
+            raise RuntimeError('install PyYAML module to support loading .yaml files')
+
+        with open(file, 'r', encoding='UTF-8') as fh:
+            data = yaml.safe_load(fh)
+            if not isinstance(data, dict):
+                data = dict(data)
+            for key, values in data.items():
+                self.add(key, values)
+
+    def dump(self, file=None, sort=False, check=False):
         """Dump key-values pairs to a plain-dict file.
 
         Args:
             file: path of file to save. Use stdout if None.
             sort: True to sort the output.
         """
-        iterator = self.items()
+        it = self.items()
         if sort:
-            iterator = sorted(iterator)
+            it = sorted(it)
         with (
             open(file, 'w', encoding='UTF-8', newline='')
             if file
             else nullcontext(sys.stdout)
         ) as fh:
-            for key, values in iterator:
+            for key, values in it:
+                if check:
+                    for badchar in '\t\n\r':
+                        if badchar in key:
+                            raise ValueError(
+                                f'{repr(key)} => {repr(values)} contains invalid {repr(badchar)}'
+                            )
+                    for badchar in ' \t\n\r':
+                        if any(badchar in v for v in values):
+                            raise ValueError(
+                                f'{repr(key)} => {repr(values)} contains invalid {repr(badchar)}'
+                            )
                 fh.write(f'{key}\t{" ".join(values)}\n')
 
     def loadjson(self, file):
         """Load from a JSON file.
 
         NOTE: The input data format may vary across subclasses.
 
@@ -360,18 +402,18 @@
 
     def print(self, sort=False):
         """Print key-values pairs.
 
         Args:
             sort: True to sort the output.
         """
-        iterator = self.items()
+        it = self.items()
         if sort:
-            iterator = sorted(iterator)
-        for key, values in iterator:
+            it = sorted(it)
+        for key, values in it:
             print(f'{key} => {" ".join(values)}')
 
     def find(self, keyword, from_keys=True, from_values=True, exact=False):
         """Search for keyword from the dictionary.
 
         Args:
             from_keys: True to search from keys.
@@ -532,26 +574,26 @@
         if isinstance(parts, str):
             return Unicode.split(parts)
         elif isinstance(parts, list):
             return parts
         else:
             return list(parts)
 
-    def match(self, parts, pos, maxlen=math.inf):
+    def match(self, parts, pos, maxpos=math.inf):
         """Match a unicode composite at pos.
 
         Args:
             parts: a string or iterable parts to be matched.
 
         Returns:
             an StsDictMatch or None if no match.
         """
         parts = self._split(parts)
         i = max(len(Unicode.split(key)) for key in self._dict)
-        i = min(i, min(len(parts), maxlen) - pos)
+        i = min(i, min(len(parts), maxpos) - pos)
         while i >= 1:
             end = pos + i
             current_parts = parts[pos:end]
             current = ''.join(current_parts)
             try:
                 conv = StsDictConv(current_parts, self._dict[current])
             except KeyError:
@@ -635,31 +677,31 @@
     def _apply_enum_sub(self, stack, data, include_short=False, include_self=False):
         """Helper function of apply_enum
         """
         (parts, matched, index) = data
         has_atomic_match = False
         i = math.inf
         while i > index:
-            match = self.match(parts, index, maxlen=i)
+            match = self.match(parts, index, i)
 
             if match is None:
                 break
 
             if match.end - index == 1:
                 has_atomic_match = True
 
-            for value in match.conv.values:
-                result = parts[:index] + [value] + parts[match.end:]
-                stack.append((result, matched + 1, index + 1))
-
+            values = match.conv.values
             if include_self:
                 value = ''.join(match.conv.key)
-                if value not in match.conv.values:
-                    result = parts[:index] + [value] + parts[match.end:]
-                    stack.append((result, matched + 1, index + 1))
+                if value not in values:
+                    values = itertools.chain(values, (value,))
+
+            for value in values:
+                result = parts[:index] + [value] + parts[match.end:]
+                stack.append((result, matched + 1, index + 1))
 
             if not include_short:
                 return
 
             i = match.end - 1
 
         # add atomic stepping (length = 1) case if none
@@ -686,50 +728,61 @@
     The internal data format is same as base StsDict.
 
     NOTE: The cache will not update after generated, and therefore the
     dictionary should not be modified after performing a text matching or
     conversion (match, apply, apply_enum, etc.) to avoid an unexpected
     behavior.
     """
-    @cached_property
-    def key_maxlen(self):
-        """Get the maximal length of the keys.
-        """
-        return max(len(Unicode.split(key)) for key in self._dict)
+    key_head_length = 2
 
     @cached_property
-    def key_headchars(self):
-        """Get a set of the first char of the keys.
-        """
-        return {key[0] for key in self._dict}
+    def key_map(self):
+        """Get a dict of the first N parts to max length."""
+        dict_ = {}
+        for key in self._dict:
+            parts = Unicode.split(key)
+            length = len(parts)
+            if length < self.key_head_length:
+                continue
+            head = ''.join(parts[:self.key_head_length])
+            try:
+                length_last = dict_[head]
+            except KeyError:
+                dict_[head] = length
+            else:
+                if length > length_last:
+                    dict_[head] = length
+        return dict_
 
-    def match(self, parts, pos, maxlen=math.inf):
+    def match(self, parts, pos, maxpos=math.inf):
         """Match a unicode composite at pos.
 
         Args:
             parts: a string or iterable parts to be matched.
 
         Returns:
             an StsDictMatch or None if no match.
         """
         parts = self._split(parts)
-        if parts[pos][0] in self.key_headchars:
-            i = self.key_maxlen
-            i = min(i, min(len(parts), maxlen) - pos)
-            while i >= 1:
-                end = pos + i
-                current_parts = parts[pos:end]
-                current = ''.join(current_parts)
-                try:
-                    conv = StsDictConv(current_parts, self._dict[current])
-                except KeyError:
-                    pass
-                else:
-                    return StsDictMatch(conv, pos, end)
-                i -= 1
+        try:
+            i = self.key_map[''.join(parts[pos:pos + self.key_head_length])]
+        except KeyError:
+            i = self.key_head_length - 1
+        i = min(i, min(len(parts), maxpos) - pos)
+        while i >= 1:
+            end = pos + i
+            current_parts = parts[pos:end]
+            current = ''.join(current_parts)
+            try:
+                conv = StsDictConv(current_parts, self._dict[current])
+            except KeyError:
+                pass
+            else:
+                return StsDictMatch(conv, pos, end)
+            i -= 1
         return None
 
 
 class Trie(StsDict):
     """An STS dictionary with trie (prefix tree) format.
 
     Compared with hash, trie is faster for applying conversion,
@@ -832,27 +885,27 @@
         for composite in Unicode.split(key):
             current = current.setdefault(composite, {})
 
         list_ = current.setdefault('', [])
         list_ += values if skip_check else [x for x in values if x not in list_]
         return self
 
-    def match(self, parts, pos, maxlen=math.inf):
+    def match(self, parts, pos, maxpos=math.inf):
         """Match a unicode composite at pos.
 
         Args:
             parts: a string or iterable parts to be matched.
 
         Returns:
             an StsDictMatch or None if no match.
         """
         parts = self._split(parts)
         trie = self._dict
         i = pos
-        total = min(len(parts), maxlen)
+        total = min(len(parts), maxpos)
         match = None
         match_end = None
         while i < total:
             try:
                 trie = trie[parts[i]]
             except KeyError:
                 break
@@ -868,14 +921,17 @@
             return StsDictMatch(conv, pos, match_end)
         return None
 
 
 class StsMaker():
     """A class for making dictionary file(s).
     """
+    config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
+    dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
+
     def make(self, config_name, base_dir=None, output_dir=None,
              skip_check=False, skip_requires=False, quiet=False):
         """Make dictionary file(s) according to a config.
 
         scheme of config (.json):
             {
                 "name": "...",
@@ -884,18 +940,21 @@
                 ],
                 "dicts": [  // dictionaries to generate
                     {
                         "file": "...",  // path of the generated dictionary
                                         // file, relative to output_dir
                         "mode": "...",  // mode to handle the loaded sources:
                                         // load, swap, join
-                        "sort": true,   // truthy to sort the keys of the
-                                        // generated dictionary
                         "src": ["...", ...]  // list of the source file paths,
                                              // should be .txt or .list files
+                        "sort": true,   // truthy to sort the keys of the
+                                        // generated dictionary
+                        "include": "...",  // regex filter for output values
+                        "exclude": "...",  // regex filter for output values
+                        "check": true,  // check for invalid output
                     },
                     ...
                 ]
             }
 
         Args:
             config_name: a str for the config file or name
@@ -931,14 +990,15 @@
             files = [self.get_stsdict_file(f, base_dir=config_dir)
                      if isinstance(f, str)
                      else [self.get_stsdict_file(i, base_dir=config_dir) for i in f]
                      for f in dict_['src']]
             sort = dict_.get('sort', False)
             include = dict_.get('include', None)
             exclude = dict_.get('exclude', None)
+            check = dict_.get('check', False)
 
             if include is not None:
                 try:
                     include = re.compile(include)
                 except re.error as exc:
                     raise ValueError(f'regex syntax error of the include filter: {exc}')
 
@@ -978,15 +1038,15 @@
             os.makedirs(os.path.dirname(dest), exist_ok=True)
 
             if format == 'tlist':
                 Trie(table).dumpjson(dest, sort=sort)
             elif format == 'jlist':
                 table.dumpjson(dest, sort=sort)
             else:  # default: list
-                table.dump(dest, sort=sort)
+                table.dump(dest, sort=sort, check=check)
 
         return dest
 
     def get_config_file(self, config, base_dir=None):
         """Calculate the path of a config file.
 
         1. Use it if it's an absolute path.
@@ -1045,21 +1105,22 @@
                 files = [files]
             for file in files:
                 if os.path.getmtime(file) > os.path.getmtime(output):
                     return True
 
         return False
 
-    config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
-    dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
-
 
 class StsConverter():
     """Convert a text using an stsdict.
     """
+    exclude_return_group_pattern = re.compile(r'^return\d*$')
+    template_placeholder_pattern = re.compile(r'%(\w*)%')
+    htmlpage_template = os.path.join(os.path.dirname(__file__), 'data', 'htmlpage.tpl.html')
+
     def __init__(self, stsdict):
         """Initialize a converter.
 
         Args:
             stsdict: an StsDict or a str, bytes or os.PathLike object for a
                 dictionary file
         """
@@ -1221,11 +1282,7 @@
         with (
             open(output, 'w', encoding=output_encoding, newline='')
             if output
             else nullcontext(sys.stdout)
         ) as fh:
             for part in conv:
                 fh.write(part)
-
-    exclude_return_group_pattern = re.compile(r'^return\d*$')
-    template_placeholder_pattern = re.compile(r'%(\w*)%')
-    htmlpage_template = os.path.join(os.path.dirname(__file__), 'data', 'htmlpage.tpl.html')
```

### Comparing `sts_lib-0.23.0/sts/cli.py` & `sts_lib-0.24.0/sts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     # subcommand: convert
     parser_convert = subparsers.add_parser('convert',
                                            help=convert.__doc__, description=convert.__doc__)
     parser_convert.add_argument('file', nargs='*',
                                 help="""file(s) to convert (default: STDIN)""")
     parser_convert.add_argument('-c', '--config', default='s2t',
                                 help="""the config to use, either a built-in config name or a path to a custom JSON file
-(built-in configs: s2t|t2s|s2tw|tw2s|s2twp|tw2sp|s2hk|hk2s|t2tw|tw2t|t2hk|hk2t|t2jp|jp2t)
+(built-in configs: s2t|t2s|t2sx|s2tw|tw2s|tw2sx|s2twp|tw2sp|tw2spx|s2hk|hk2s|hk2sx|s2hkp|hk2sp|hk2spx|t2tw|tw2t|t2hk|hk2t|t2jp|t2jpx|jp2t)
 (default: %(default)s)""")
     parser_convert.add_argument('-f', '--format', default='txt',
                                 choices=['txt', 'txtm', 'html', 'htmlpage', 'json'], metavar='FORMAT',
                                 help="""output format (txt|txtm|html|htmlpage|json) (default: %(default)s)""")
     parser_convert.add_argument('--exclude', type=regex,
                                 help="""exclude text matching given regex from conversion, and replace it with the
 "return" (or "return1", "return2", etc.) subgroup value if exists""")
```

### Comparing `sts_lib-0.23.0/sts/data/config/_default.json` & `sts_lib-0.24.0/sts/data/config/tw2spx.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.35000000000000003%*

 * *Differences: {"'dicts'": "{0: {'file': '../dictionary/tw2spx.tlist', 'mode': 'join', 'src': "*

 * *            "[['TWPhrasesRev.txt', 'TWPhrasesRev.list', 'TWVariantsRevPhrases.txt', "*

 * *            "'TWVariantsRev.list'], ['TSPhrases.txt', 'TSCharacters.txt', 'TSCharactersEx.txt']]}, "*

 * *            'delete: [3, 2, 1, 0]}',*

 * * "'name'": "'Traditional Chinese (Taiwan standard) to Simplified Chinese (with phrases and "*

 * *           "extended simplification)'",*

 * * "'requires'": "['_default']"}*

```diff
@@ -1,42 +1,25 @@
 {
     "dicts": [
         {
-            "file": "TWPhrases.list",
-            "mode": "load",
+            "file": "../dictionary/tw2spx.tlist",
+            "mode": "join",
             "src": [
-                "TWPhrasesIT.txt",
-                "TWPhrasesName.txt",
-                "TWPhrasesOther.txt"
-            ]
-        },
-        {
-            "file": "TWPhrasesRev.list",
-            "mode": "swap",
-            "src": [
-                "TWPhrases.list"
-            ]
-        },
-        {
-            "file": "TWVariantsRev.list",
-            "mode": "swap",
-            "src": [
-                "TWVariants.txt"
-            ]
-        },
-        {
-            "file": "HKVariantsRev.list",
-            "mode": "swap",
-            "src": [
-                "HKVariants.txt"
-            ]
-        },
-        {
-            "file": "JPVariantsRev.list",
-            "mode": "swap",
-            "src": [
-                "JPVariants.txt"
+                [
+                    "TWPhrasesRev.txt",
+                    "TWPhrasesRev.list",
+                    "TWVariantsRevPhrases.txt",
+                    "TWVariantsRev.list"
+                ],
+                [
+                    "TSPhrases.txt",
+                    "TSCharacters.txt",
+                    "TSCharactersEx.txt"
+                ]
             ]
         }
     ],
-    "name": "Built-in dictionaries"
+    "name": "Traditional Chinese (Taiwan standard) to Simplified Chinese (with phrases and extended simplification)",
+    "requires": [
+        "_default"
+    ]
 }
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.24.0/sts/data/dictionary/HKVariants.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 僞	偽
 兌	兑
+冢	塚
 叄	叁
 只	只 衹
 啓	啓 啟
 喫	吃
 囪	囱
 妝	妝 粧
 媼	媪
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.24.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.24.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.24.0/sts/data/dictionary/JPVariants.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 乘	乗
 亂	乱
 亙	亘
 亞	亜
 佛	仏
 來	来
+俁	俣
 假	仮
 傳	伝
 僞	偽
 價	価
 儉	倹
 兒	児
+兔	兎
 內	内
 兩	両
+冢	塚
 剎	刹
 剩	剰
 劍	剣
 劑	剤
 勞	労
 勳	勲
 勵	励
@@ -23,37 +26,38 @@
 勻	匀
 區	区
 卷	巻
 卻	却
 參	参
 吳	呉
 咒	呪
-啞	唖
 單	単
+喻	喩
 噓	嘘
-嚙	噛
 嚴	厳
 囑	嘱
 圈	圏
 國	国
 圍	囲
 圓	円
 圖	図
 團	団
+堯	尭
 增	増
 墮	堕
 壓	圧
 壘	塁
 壞	壊
 壤	壌
 壯	壮
 壹	壱
 壽	寿
 奧	奥
 奬	奨
+妍	姸
 妝	粧
 孃	嬢
 學	学
 寢	寝
 實	実
 寫	写
 寬	寛
@@ -66,20 +70,20 @@
 峯	峰
 峽	峡
 嶽	岳
 巖	巌
 巢	巣
 帶	帯
 廁	厠
+廄	厩
 廢	廃
 廣	広
 廳	庁
 彈	弾
 彌	弥
-彎	弯
 彥	彦
 徑	径
 從	従
 徵	徴
 德	徳
 恆	恒
 悅	悦
@@ -96,52 +100,50 @@
 戾	戻
 拂	払
 拔	抜
 拜	拝
 挾	挟
 插	挿
 揭	掲
-搔	掻
 搖	揺
 搜	捜
-摑	掴
 擇	択
 擊	撃
 擔	担
 據	拠
 擴	拡
 攝	摂
-攪	撹
 收	収
 效	効
 敕	勅
 敘	叙
 數	数
 斷	断
 晉	晋
 晚	晩
 晝	昼
 暨	曁
 曆	暦
 曉	暁
 曾	曽
 會	会
-枡	桝
 查	査
 條	条
 棧	桟
 棱	稜 棱
 榆	楡
 榮	栄
 樂	楽
 樓	楼
 樞	枢
 樣	様
 橫	横
+檜	桧
 檢	検
+櫸	欅
 櫻	桜
 權	権
 歐	欧
 歡	歓
 步	歩
 歲	歳
 歷	歴
@@ -150,35 +152,33 @@
 殼	殻
 毆	殴
 每	毎
 氣	気
 污	汚
 沒	没
 涉	渉
+淒	凄
 淚	涙
 淨	浄
 淺	浅
 渴	渇
-潑	溌
 溪	渓
 溫	温
 溼	湿
 滯	滞
 滿	満
 潛	潜
 澀	渋
 澤	沢
 濟	済
 濤	涛
 濱	浜
-濾	沪
 瀧	滝
 瀨	瀬
 灣	湾
-焰	焔
 燈	灯
 燒	焼
 營	営
 爐	炉
 爭	争
 爲	為
 牀	床
@@ -190,65 +190,62 @@
 獸	獣
 獻	献
 瓣	弁
 產	産
 畫	画
 當	当
 疊	畳
-疎	疏
 痹	痺
 瘦	痩
 癡	痴
+癢	痒
 發	発
 皋	皐
 盜	盗
 盡	尽
 碎	砕
 祕	秘
 祿	禄
 禦	御
 禪	禅
 禮	礼
-禱	祷
+禰	祢
 稅	税
 稱	称
 稻	稲
-穎	頴
 穗	穂
 穩	穏
 穰	穣
-竈	竃
 竊	窃
 粹	粋
 糉	粽
 絕	絶
 絲	糸
 經	経
 綠	緑
 緖	緒
 緣	縁
 縣	県
 縱	縦
 總	総
-繫	繋
-繡	繍
 繩	縄
 繪	絵
 繼	継
 續	続
 纔	才
 纖	繊
 缺	欠
 罐	缶
 羣	群
 聯	連
 聰	聡
 聲	声
 聽	聴
 肅	粛
+脅	脇
 脣	唇
 脫	脱
 腦	脳
 腳	脚
 膽	胆
 臟	臓
 臺	台
@@ -258,67 +255,65 @@
 舍	舎
 荔	茘
 莊	荘
 莖	茎
 菸	煙
 萊	莱
 萬	万
-蔣	蒋
 蔥	葱
 薰	薫
 藏	蔵
 藝	芸
 藥	薬
-蘆	芦
 處	処
 虛	虚
 號	号
 螢	蛍
 蟲	虫
-蠟	蝋
 蠶	蚕
 蠻	蛮
 裝	装
 覺	覚
 覽	覧
 觀	観
 觸	触
 說	説
 謠	謡
 證	証
 譯	訳
 譽	誉
 讀	読
 變	変
+讎	讐
 讓	譲
+讚	讃
+豎	竪
 豐	豊
+豔	艶
 豫	予
 貓	猫
 貳	弐
 賣	売
 賴	頼
 贊	賛
 贗	贋
 踐	践
 輕	軽
 輛	輌
 轉	転
 辨	弁
 辭	辞
 辯	弁
+遙	遥
 遞	逓
-遥	遙
 遲	遅
 邊	辺
 鄉	郷
-酢	醋
 醉	酔
-醱	醗
 醫	医
-醬	醤
 釀	醸
 釋	釈
 鋪	舗
 錄	録
 錢	銭
 鍊	錬
 鐵	鉄
@@ -344,20 +339,17 @@
 驗	験
 驛	駅
 髓	髄
 體	体
 髮	髪
 鬥	闘
 鱉	鼈
-鷗	鴎
-鹼	鹸
 鹽	塩
 麥	麦
 麪	麺
-麴	麹
 黃	黄
 黑	黒
 默	黙
 點	点
 黨	党
 齊	斉
 齋	斎
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.24.0/sts/data/dictionary/STCharacters.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,29 @@
-㐷	傌
-㐹	㑶 㐹
-㐽	偑
 㑇	㑳
-㑈	倲
-㑔	㑯
-㑩	儸
-㓆	𠗣
-㓥	劏
-㓰	劃
-㔉	劚
-㖊	噚
-㖞	喎
 㘎	㘚
-㚯	㜄
-㛀	媰
-㛟	𡞵
-㛠	𡢃
-㛣	㜏
-㛤	孋
-㛿	𡠹
-㟆	㠏
-㟜	𡾱
-㟥	嵾
-㡎	幓
 㤘	㥮
-㤽	懤
-㥪	慺
-㧏	掆
 㧐	㩳
 㧑	撝
 㧟	擓
-㧰	擽
-㨫	㩜
 㭎	棡
-㭏	椲
-㭣	𣙎
-㭤	樢
-㭴	樫
-㱩	殰
-㱮	殨
-㲿	瀇
-㳔	濧
-㳕	灡
-㳠	澾
-㳡	濄
-㳢	𣾷
-㳽	瀰
-㴋	潚
-㶉	鸂
-㶶	燶
-㶽	煱
-㺍	獱
-㻅	璯
-㻏	𤫩
-㻘	𤪺
-䀥	䁻
 䁖	瞜
-䂵	碽
 䃅	磾
-䅉	稏
 䅟	穇
-䅪	𥢢
-䇲	筴
-䉤	籔
-䌶	䊷
-䌷	紬
-䌸	縳
 䌹	絅
-䌺	䋙
-䌻	䋚
-䌼	綐
-䌽	綵
-䌾	䋻
-䌿	䋹
-䍀	繿
-䍁	繸
-䍠	䍦
-䎬	䎱
 䏝	膞
-䑽	𦪙
-䓓	薵
-䓕	薳
 䓖	藭
 䓨	罃
 䗖	螮
-䘛	𧝞
-䘞	𧜗
-䙊	𧜵
-䙌	䙡
-䙓	襬
 䜣	訢
-䜤	鿁
-䜥	𧩙
-䜧	䜀
-䜩	讌
 䝙	貙
-䞌	𧵳
-䞍	䝼
-䞎	𧶧
-䞐	賰
-䟢	躎
-䢀	𨊰
-䢁	𨊸
-䢂	𨋢
-䥺	釾
 䥽	鏺
-䥾	䥱
-䥿	𨯅
-䦀	𨦫
-䦁	𨧜
-䦂	䥇
 䦃	鐯
-䦅	鐥
-䦆	钁
-䦶	䦛
-䦷	䦟
-䩄	靦
-䭪	𩞯
-䯃	𩣑
-䯄	騧
-䯅	䯀
-䲝	䱽
-䲞	𩶘
 䲟	鮣
 䲠	鰆
-䲡	鰌
 䲢	鰧
-䲣	䱷
 䴓	鳾
 䴔	鵁
 䴕	鴷
 䴖	鶄
 䴗	鶪
 䴘	鷉
 䴙	鸊
@@ -190,37 +83,36 @@
 优	優
 伙	夥 伙
 会	會
 伛	傴
 伞	傘
 伟	偉
 传	傳
-伡	俥
 伣	俔
 伤	傷
 伥	倀
 伦	倫
 伧	傖
 伪	僞
 伫	佇
 体	體
 余	餘 余
 佛	佛 彿
+你	你 妳
 佣	傭 佣
 佥	僉
 侠	俠
 侣	侶
 侥	僥
 侦	偵
 侧	側
 侨	僑
 侩	儈
 侪	儕
 侬	儂
-侭	儘
 俊	俊 儁
 俣	俁
 俦	儔
 俨	儼
 俩	倆
 俪	儷
 俫	倈
@@ -229,15 +121,14 @@
 借	借 藉
 债	債
 倾	傾
 偬	傯
 偻	僂
 偾	僨
 偿	償
-傤	儎
 傥	儻
 傧	儐
 储	儲
 傩	儺
 僵	僵 殭
 儿	兒
 克	克 剋
@@ -253,14 +144,15 @@
 冁	囅
 内	內
 冈	岡
 册	冊
 写	寫
 军	軍
 农	農
+冢	冢 塚
 冬	冬 鼕
 冯	馮
 冲	衝 沖
 决	決
 况	況
 冻	凍
 净	淨
@@ -290,15 +182,14 @@
 别	別 彆
 刬	剗
 刭	剄
 刮	刮 颳
 制	制 製
 刹	剎
 刽	劊
-刾	㓨
 刿	劌
 剀	剴
 剂	劑
 剐	剮
 剑	劍
 剥	剝
 剧	劇
@@ -336,15 +227,14 @@
 厂	廠 厂
 厅	廳
 历	歷 曆
 厉	厲
 压	壓
 厌	厭
 厍	厙
-厐	龎
 厕	廁
 厘	釐 厘
 厢	廂
 厣	厴
 厦	廈
 厨	廚
 厩	廄
@@ -403,29 +293,26 @@
 哑	啞
 哒	噠
 哓	嘵
 哔	嗶
 哕	噦
 哗	譁 嘩
 哙	噲
-哜	嚌
 哝	噥
 哟	喲
 唇	脣 唇
 唛	嘜
 唝	嗊
 唠	嘮
-唡	啢
 唢	嗩
 唤	喚
 啧	嘖
 啬	嗇
 啭	囀
 啮	齧 嚙
-啯	嘓
 啰	囉
 啴	嘽
 啸	嘯
 喂	喂 餵
 喷	噴
 喽	嘍
 喾	嚳
@@ -456,15 +343,14 @@
 坛	壇 罈
 坜	壢
 坝	壩 垻
 坞	塢
 坟	墳
 坠	墜
 垄	壟
-垅	壠
 垆	壚
 垒	壘
 垦	墾
 垩	堊
 垫	墊
 垭	埡
 垯	墶
@@ -629,24 +515,22 @@
 开	開
 异	異
 弃	棄
 弑	弒
 张	張
 弥	彌 瀰
 弦	弦 絃
-弪	弳
 弯	彎
 弹	彈
 强	強
 归	歸
 当	當 噹
 录	錄 彔
 彟	彠
 彦	彥
-彨	彲
 彩	彩 綵
 彻	徹
 征	徵 征
 径	徑
 徕	徠
 御	御 禦
 忆	憶
@@ -677,15 +561,14 @@
 恻	惻
 恼	惱
 恽	惲
 悦	悅
 悫	愨
 悬	懸
 悭	慳
-悮	悞
 悯	憫
 惊	驚
 惧	懼
 惨	慘
 惩	懲
 惫	憊
 惬	愜
@@ -705,15 +588,14 @@
 戆	戇
 戋	戔
 戏	戲
 戗	戧
 战	戰
 戚	戚 慼
 戬	戩
-戯	戱
 户	戶
 才	才 纔
 扎	扎 紮
 扑	撲
 托	託 托
 扣	扣 釦
 执	執
@@ -741,47 +623,42 @@
 拦	攔
 拧	擰
 拨	撥
 择	擇
 挂	掛 挂
 挚	摯
 挛	攣
-挜	掗
 挝	撾
 挞	撻
 挟	挾
 挠	撓
 挡	擋
-挢	撟
 挣	掙
 挤	擠
 挥	揮
 挦	撏
 挨	挨 捱
 挽	挽 輓
-捝	挩
 捞	撈
 损	損
 捡	撿
 换	換
 捣	搗
 据	據 据
 掳	擄
 掴	摑
 掷	擲
 掸	撣
 掺	摻
 掼	摜
 揽	攬
-揾	搵
 揿	撳
 搀	攙
 搁	擱
 搂	摟
-搄	揯
 搅	攪
 搜	搜 蒐
 携	攜
 摄	攝
 摅	攄
 摆	擺 襬
 摇	搖
@@ -789,19 +666,17 @@
 摊	攤
 撄	攖
 撑	撐
 撵	攆
 撷	擷
 撸	擼
 撺	攛
-擜	㩵
 擞	擻
 攒	攢
 敌	敵
-敚	敓
 敛	斂
 敩	斆
 数	數
 斋	齋
 斓	斕
 斗	鬥 斗
 斩	斬
@@ -882,39 +757,33 @@
 档	檔
 桤	榿
 桥	橋
 桦	樺
 桧	檜
 桨	槳
 桩	樁
-桪	樳
 梁	梁 樑
 梦	夢
 梼	檮
 梾	棶
 梿	槤
 检	檢
 棁	梲
 棂	欞
 椁	槨
-椝	槼
 椟	櫝
 椠	槧
-椢	槶
 椤	欏
-椫	樿
 椭	橢
-椮	槮
 楼	樓
 榄	欖
 榅	榲
 榇	櫬
 榈	櫚
 榉	櫸
-榝	樧
 槚	檟
 槛	檻
 槟	檳
 槠	櫧
 横	橫
 樯	檣
 樱	櫻
@@ -938,15 +807,14 @@
 殴	毆
 毁	毀 燬 譭
 毂	轂
 毕	畢
 毙	斃
 毡	氈
 毵	毿
-毶	𣯶
 氇	氌
 气	氣
 氢	氫
 氩	氬
 氲	氳
 汇	匯 彙
 汉	漢
@@ -961,19 +829,19 @@
 沥	瀝
 沦	淪
 沧	滄
 沨	渢
 沩	潙
 沪	滬
 沾	沾 霑
+泄	泄 洩
 泛	泛 氾 汎
 泞	濘
 注	注 註
 泪	淚
-泶	澩
 泷	瀧
 泸	瀘
 泺	濼
 泻	瀉
 泼	潑
 泽	澤
 泾	涇
@@ -995,15 +863,14 @@
 浑	渾
 浒	滸
 浓	濃
 浔	潯
 浕	濜
 涂	塗 涂
 涌	湧 涌
-涚	涗
 涛	濤
 涝	澇
 涞	淶
 涟	漣
 涠	潿
 涡	渦
 涢	溳
@@ -1017,15 +884,14 @@
 渊	淵
 渌	淥
 渍	漬
 渎	瀆
 渐	漸
 渑	澠
 渔	漁
-渖	瀋
 渗	滲
 温	溫
 游	遊 游
 湾	灣
 湿	溼
 溁	濚
 溃	潰
@@ -1134,15 +1000,14 @@
 珲	琿
 琎	璡
 琏	璉
 琐	瑣
 琼	瓊
 瑶	瑤
 瑷	璦
-瑸	璸
 璇	璇 璿
 璎	瓔
 瓒	瓚
 瓮	甕
 瓯	甌
 电	電
 画	畫
@@ -1159,15 +1024,14 @@
 疯	瘋
 疱	皰
 疴	痾
 症	症 癥
 痈	癰
 痉	痙
 痒	癢
-痖	瘂
 痨	癆
 痪	瘓
 痫	癇
 痴	癡
 瘅	癉
 瘆	瘮
 瘗	瘞
@@ -1191,15 +1055,14 @@
 盘	盤
 眍	瞘
 眦	眥
 眬	矓
 睁	睜
 睐	睞
 睑	瞼
-瞆	瞶
 瞒	瞞
 瞩	矚
 矩	矩 榘
 矫	矯
 矶	磯
 矾	礬
 矿	礦
@@ -1216,16 +1079,15 @@
 硁	硜
 硕	碩
 硖	硤
 硗	磽
 硙	磑
 硚	礄
 确	確 确
-硵	磠
-硷	礆
+硷	鹼 礆
 碍	礙
 碛	磧
 碜	磣
 碱	鹼
 礼	禮
 祃	禡
 祎	禕
@@ -1248,15 +1110,14 @@
 秽	穢
 秾	穠
 稆	穭
 税	稅
 稣	穌
 稳	穩
 穑	穡
-穞	穭
 穷	窮
 窃	竊
 窍	竅
 窎	窵
 窑	窯
 窜	竄
 窝	窩
@@ -1276,15 +1137,14 @@
 筚	篳
 筛	篩
 筜	簹
 筝	箏
 筹	籌
 筼	篔
 签	籤 簽
-筿	篠
 简	簡
 箓	籙
 箦	簀
 箧	篋
 箨	籜
 箩	籮
 箪	簞
@@ -1307,17 +1167,14 @@
 粽	糉
 糁	糝
 糇	餱
 糍	餈
 系	系 係 繫
 紧	緊
 絷	縶
-緼	縕
-縆	緪
-纟	糹
 纠	糾
 纡	紆
 红	紅
 纣	紂
 纤	纖 縴
 纥	紇
 约	約
@@ -1386,15 +1243,14 @@
 绥	綏
 绦	絛
 继	繼
 绨	綈
 绩	績
 绪	緒
 绫	綾
-绬	緓
 续	續
 绮	綺
 绯	緋
 绰	綽
 绱	鞝 緔
 绲	緄
 绳	繩
@@ -1417,19 +1273,16 @@
 缄	緘
 缅	緬
 缆	纜
 缇	緹
 缈	緲
 缉	緝
 缊	縕
-缋	繢
 缌	緦
-缍	綞
 缎	緞
-缏	緶
 缐	線
 缑	緱
 缒	縋
 缓	緩
 缔	締
 缕	縷
 编	編
@@ -1565,15 +1418,14 @@
 茧	繭
 荆	荊
 荐	薦 荐
 荙	薘
 荚	莢
 荛	蕘
 荜	蓽
-荝	萴
 荞	蕎
 荟	薈
 荠	薺
 荡	蕩 盪
 荣	榮
 荤	葷
 荥	滎
@@ -1602,54 +1454,49 @@
 萝	蘿
 萤	螢
 营	營
 萦	縈
 萧	蕭
 萨	薩
 葱	蔥
-蒀	蒕
 蒇	蕆
 蒉	蕢
 蒋	蔣
 蒌	蔞
-蒏	醟
 蒙	蒙 矇 濛 懞
 蓝	藍
 蓟	薊
 蓠	蘺
 蓣	蕷
 蓥	鎣
 蓦	驀
-蔂	虆
 蔑	蔑 衊
 蔷	薔
 蔹	蘞
 蔺	藺
 蔼	藹
 蕰	薀
 蕲	蘄
 蕴	蘊
 薮	藪
 藓	蘚
-藴	蘊
 蘖	櫱
 虏	虜
 虑	慮
 虚	虛
 虫	蟲 虫
 虬	虯
 虮	蟣
 虱	蝨
 虽	雖
 虾	蝦
 虿	蠆
 蚀	蝕
 蚁	蟻
 蚂	螞
-蚃	蠁
 蚕	蠶
 蚝	蠔 蚝
 蚬	蜆
 蛊	蠱
 蛎	蠣
 蛏	蟶
 蛮	蠻
@@ -1663,15 +1510,14 @@
 蜡	蠟 蜡
 蝇	蠅
 蝈	蟈
 蝉	蟬
 蝎	蠍 蝎
 蝼	螻
 蝾	蠑
-螀	螿
 螨	蟎
 蟏	蠨
 衅	釁
 衔	銜
 补	補
 表	表 錶
 衬	襯
@@ -1700,39 +1546,36 @@
 视	視
 觇	覘
 览	覽
 觉	覺
 觊	覬
 觋	覡
 觌	覿
-觍	覥
 觎	覦
 觏	覯
 觐	覲
 觑	覷
 觞	觴
 触	觸
 觯	觶
 訚	誾
 詟	讋
 誉	譽
 誊	謄
-讠	訁
 计	計
 订	訂
 讣	訃
 认	認
 讥	譏
 讦	訐
 讧	訌
 讨	討
 让	讓
 讪	訕
 讫	訖
-讬	託
 训	訓
 议	議
 讯	訊
 记	記
 讱	訒
 讲	講
 讳	諱
@@ -1786,27 +1629,25 @@
 诣	詣
 诤	諍
 该	該
 详	詳
 诧	詫
 诨	諢
 诩	詡
-诪	譸
 诫	誡
 诬	誣
 语	語
 诮	誚
 误	誤
 诰	誥
 诱	誘
 诲	誨
 诳	誑
 说	說
 诵	誦
-诶	誒
 请	請
 诸	諸
 诹	諏
 诺	諾
 读	讀
 诼	諑
 诽	誹
@@ -1817,30 +1658,28 @@
 谂	諗
 调	調
 谄	諂
 谅	諒
 谆	諄
 谇	誶
 谈	談
-谉	讅
 谊	誼
 谋	謀
 谌	諶
 谍	諜
 谎	謊
 谏	諫
 谐	諧
 谑	謔
 谒	謁
 谓	謂
 谔	諤
 谕	諭
 谖	諼
 谗	讒
-谘	諮
 谙	諳
 谚	諺
 谛	諦
 谜	謎
 谝	諞
 谞	諝
 谟	謨
@@ -1868,15 +1707,14 @@
 谵	譫
 谶	讖
 谷	谷 穀
 豮	豶
 贝	貝
 贞	貞
 负	負
-贠	貟
 贡	貢
 财	財
 责	責
 贤	賢
 败	敗
 账	賬
 货	貨
@@ -1963,15 +1801,14 @@
 蹑	躡
 蹒	蹣
 蹰	躕
 蹿	躥
 躏	躪
 躜	躦
 躯	軀
-輼	轀
 车	車
 轧	軋
 轨	軌
 轩	軒
 轪	軑
 轫	軔
 转	轉
@@ -2069,34 +1906,31 @@
 酝	醞
 酦	醱
 酱	醬
 酸	酸 痠
 酽	釅
 酾	釃
 酿	釀
-醖	醞
 采	採 采 寀
 释	釋
 里	裏 里
 鉴	鑑 鑒
 銮	鑾
 錾	鏨
-钅	釒
 钆	釓
 钇	釔
 针	針 鍼
 钉	釘
 钊	釗
 钋	釙
 钌	釕
 钍	釷
 钎	釺
 钏	釧
 钐	釤
-钑	鈒
 钒	釩
 钓	釣
 钔	鍆
 钕	釹
 钖	鍚
 钗	釵
 钘	鈃
@@ -2125,45 +1959,40 @@
 钯	鈀
 钰	鈺
 钱	錢
 钲	鉦
 钳	鉗
 钴	鈷
 钵	鉢
-钶	鈳
 钷	鉕
-钸	鈽
 钹	鈸
 钺	鉞
 钻	鑽 鉆
 钼	鉬
 钽	鉭
 钾	鉀
 钿	鈿
 铀	鈾
 铁	鐵
 铂	鉑
 铃	鈴
 铄	鑠
 铅	鉛
 铆	鉚
-铇	鉋
 铈	鈰
 铉	鉉
 铊	鉈
 铋	鉍
 铌	鈮
 铍	鈹
 铎	鐸
 铏	鉶
 铐	銬
 铑	銠
 铒	鉺
-铓	鋩
-铔	錏
 铕	銪
 铖	鋮
 铗	鋏
 铘	鋣
 铙	鐃
 铚	銍
 铛	鐺
@@ -2173,15 +2002,14 @@
 铟	銦
 铠	鎧
 铡	鍘
 铢	銖
 铣	銑
 铤	鋌
 铥	銩
-铦	銛
 铧	鏵
 铨	銓
 铩	鎩
 铪	鉿
 铫	銚
 铬	鉻
 铭	銘
@@ -2231,15 +2059,14 @@
 错	錯
 锚	錨
 锛	錛
 锜	錡
 锝	鍀
 锞	錁
 锟	錕
-锠	錩
 锡	錫
 锢	錮
 锣	鑼
 锤	錘
 锥	錐
 锦	錦
 锧	鑕
@@ -2288,21 +2115,19 @@
 镒	鎰
 镓	鎵
 镔	鑌
 镕	鎔
 镖	鏢
 镗	鏜
 镘	鏝
-镙	鏍
 镚	鏰
 镛	鏞
 镜	鏡
 镝	鏑
 镞	鏃
-镟	鏇
 镠	鏐
 镡	鐔
 镢	钁 鐝
 镣	鐐
 镤	鏷
 镥	鑥
 镦	鐓
@@ -2323,15 +2148,14 @@
 镵	鑱
 镶	鑲
 长	長
 门	門
 闩	閂
 闪	閃
 闫	閆
-闬	閈
 闭	閉
 问	問
 闯	闖
 闰	閏
 闱	闈
 闲	閒 閑
 闳	閎
@@ -2362,55 +2186,50 @@
 阌	閿
 阍	閽
 阎	閻
 阏	閼
 阐	闡
 阑	闌
 阒	闃
-阓	闠
 阔	闊
 阕	闋
 阖	闔
 阗	闐
 阘	闒
 阙	闕
 阚	闞
-阛	闤
 队	隊
 阳	陽
 阴	陰
 阵	陣
 阶	階
 际	際
 陆	陸
 陇	隴
 陈	陳
 陉	陘
 陕	陝
-陦	隯
 陧	隉
 陨	隕
 险	險
 随	隨
 隐	隱
 隶	隸
 隽	雋
 难	難
 雇	僱
 雏	雛
-雕	雕 鵰
+雕	雕 彫 鵰 琱
 雠	讎
 雳	靂
 雾	霧
 霁	霽
 霉	黴
-霡	霢
 霭	靄
 靓	靚
-靔	靝
 静	靜
 面	面 麪
 靥	靨
 鞑	韃
 鞒	鞽
 鞯	韉
 鞲	韝
@@ -2447,56 +2266,48 @@
 颋	頲
 颌	頜
 颍	潁
 颎	熲
 颏	頦
 颐	頤
 频	頻
-颒	頮
 颓	頹
 颔	頷
-颕	頴
 颖	穎
 颗	顆
 题	題
 颙	顒
 颚	顎
 颛	顓
 颜	顏
 额	額
 颞	顳
 颟	顢
 颠	顛
 颡	顙
 颢	顥
-颣	纇
 颤	顫
 颥	顬
 颦	顰
 颧	顴
 风	風
 飏	颺
 飐	颭
 飑	颮
 飒	颯
 飓	颶
 飔	颸
 飕	颼
-飖	颻
 飗	飀
 飘	飄
 飙	飆
-飚	飈
 飞	飛
 飨	饗
 餍	饜
-饣	飠
-饤	飣
 饥	飢 饑
-饦	飥
 饧	餳
 饨	飩
 饩	餼
 饪	飪
 饫	飫
 饬	飭
 饭	飯
@@ -2512,31 +2323,27 @@
 饷	餉
 饸	餄
 饹	餎
 饺	餃
 饻	餏
 饼	餅
 饽	餑
-饾	餖
 饿	餓
-馀	餘
 馁	餒
-馂	餕
 馃	餜
 馄	餛
 馅	餡
 馆	館
 馇	餷
 馈	饋
 馉	餶
 馊	餿
 馋	饞
 馌	饁
 馍	饃
-馎	餺
 馏	餾
 馐	饈
 馑	饉
 馒	饅
 馓	饊
 馔	饌
 馕	饢
@@ -2576,15 +2383,14 @@
 骍	騂
 骎	駸
 骏	駿
 骐	騏
 骑	騎
 骒	騍
 骓	騅
-骔	騌
 骕	驌
 骖	驂
 骗	騙
 骘	騭
 骙	騤
 骚	騷
 骛	騖
@@ -2611,30 +2417,28 @@
 鱽	魛
 鱾	魢
 鱿	魷
 鲀	魨
 鲁	魯
 鲂	魴
 鲃	䰾
-鲄	魺
 鲅	鮁
 鲆	鮃
 鲇	鮎
 鲈	鱸
 鲉	鮋
 鲊	鮓
 鲋	鮒
 鲌	鮊
 鲍	鮑
 鲎	鱟
 鲏	鮍
 鲐	鮐
 鲑	鮭
 鲒	鮚
-鲓	鮳
 鲔	鮪
 鲕	鮞
 鲖	鮦
 鲗	鰂
 鲘	鮜
 鲙	鱠
 鲚	鱭
@@ -2661,15 +2465,14 @@
 鲯	鯕
 鲰	鯫
 鲱	鯡
 鲲	鯤
 鲳	鯧
 鲴	鯝
 鲵	鯢
-鲶	鯰
 鲷	鯛
 鲸	鯨
 鲹	鰺
 鲺	鯴
 鲻	鯔
 鲼	鱝
 鲽	鰈
@@ -2677,20 +2480,18 @@
 鲿	鱨
 鳀	鯷
 鳁	鰮
 鳂	鰃
 鳃	鰓
 鳄	鱷
 鳅	鰍
-鳆	鰒
 鳇	鰉
 鳈	鰁
 鳉	鱂
 鳊	鯿
-鳋	鰠
 鳌	鰲
 鳍	鰭
 鳎	鰨
 鳏	鰥
 鳐	鰩
 鳑	鰟
 鳒	鰜
@@ -2729,15 +2530,14 @@
 鸭	鴨
 鸮	鴞
 鸯	鴦
 鸰	鴒
 鸱	鴟
 鸲	鴝
 鸳	鴛
-鸴	鷽
 鸵	鴕
 鸶	鷥
 鸷	鷙
 鸸	鴯
 鸹	鴰
 鸺	鵂
 鸻	鴴
@@ -2760,15 +2560,14 @@
 鹌	鵪
 鹍	鵾
 鹎	鵯
 鹏	鵬
 鹐	鵮
 鹑	鶉
 鹒	鶊
-鹓	鵷
 鹔	鷫
 鹕	鶘
 鹖	鶡
 鹗	鶚
 鹘	鶻
 鹙	鶖
 鹚	鷀
@@ -2778,15 +2577,14 @@
 鹞	鷂
 鹟	鶲
 鹠	鶹
 鹡	鶺
 鹢	鷁
 鹣	鶼
 鹤	鶴
-鹥	鷖
 鹦	鸚
 鹧	鷓
 鹨	鷚
 鹩	鷯
 鹪	鷦
 鹫	鷲
 鹬	鷸
@@ -2798,24 +2596,22 @@
 鹲	鸏
 鹳	鸛
 鹴	鸘
 鹾	鹺
 麦	麥
 麸	麩
 麹	麴
-麺	麪
 麽	麼
 黄	黃
 黉	黌
 黡	黶
 黩	黷
 黪	黲
 黾	黽
 鼋	黿
-鼌	鼂
 鼍	鼉
 鼹	鼴
 齐	齊
 齑	齏
 齿	齒
 龀	齔
 龁	齕
@@ -2832,1044 +2628,81 @@
 龌	齷
 龙	龍
 龚	龔
 龛	龕
 龟	龜
 鿎	䃮
 鿏	䥑
-鿒	鿓
-鿔	鎶
-𠀾	𠁞
-𠆲	儣
-𠆿	𠌥
-𠇹	俓
-𠉂	㒓
-𠉗	𠏢
-𠋆	儭
-𠚳	𠠎
-𠛅	剾
-𠛆	𠞆
-𠛾	𪟖
-𠡠	勑
-𠮶	嗰
-𠯟	哯
-𠯠	噅
-𠰱	㘉
-𠰷	嚧
-𠱞	囃
-𠲥	𡅏
-𠴛	𡃕
-𠴢	𡄔
-𠵸	𡄣
-𠵾	㗲
-𡋀	𡓾
-𡋗	𡑭
-𡋤	壗
-𡍣	𡔖
-𡒄	壈
-𡝠	㜷
-𡞋	㜗
-𡞱	㜢
-𡠟	孎
-𡥧	孻
-𡭜	𡮉
-𡭬	𡮣
-𡳃	𡳳
-𡳒	𦘧
-𡶴	嵼
-𡸃	𡽗
-𡺃	嶈
-𡺄	嶘
-𢋈	㢝
-𢗓	㦛
-𢘙	𢤱
-𢘝	𢣚
-𢘞	𢣭
-𢙏	愻
-𢙐	憹
-𢙑	𢠼
-𢙒	憢
-𢙓	懀
-𢛯	㦎
-𢠁	懎
-𢢐	𤢻
-𢧐	戰
-𢫊	𢷮
-𢫞	𢶫
-𢫬	摋
-𢬍	擫
-𢬦	𢹿
-𢭏	擣
-𢽾	斅
-𣃁	斸
-𣆐	曥
-𣈣	𣋋
-𣍨	𦢈
-𣍯	腪
-𣍰	脥
-𣎑	臗
-𣏢	槫
-𣐕	桱
-𣐤	欍
-𣑶	𣠲
-𣒌	楇
-𣓿	橯
-𣔌	樤
-𣗊	樠
 𣗋	欓
-𣗙	㰙
-𣘐	㯤
-𣘓	𣞻
-𣘴	檭
-𣘷	𣝕
-𣚚	欘
-𣞎	𣠩
-𣨼	殢
-𣭤	𣯴
-𣯣	𣯩
-𣱝	氭
 𣲗	湋
 𣲘	潕
-𣳆	㵗
-𣶩	澅
-𣶫	𣿉
-𣶭	𪷓
-𣷷	𤅶
 𣸣	濆
-𣺼	灙
-𣺽	𤁣
-𣽷	瀃
-𤆡	熓
-𤆢	㷍
-𤇃	爄
-𤇄	熌
-𤇭	爖
-𤇹	熚
-𤈶	熉
-𤈷	㷿
-𤊀	𤒎
-𤊰	𤓩
-𤋏	熡
-𤎺	𤓎
-𤎻	𤑳
-𤙯	𤛮
-𤝢	𤢟
-𤞃	獩
-𤞤	玁
-𤠋	㺏
-𤦀	瓕
 𤩽	瓛
-𤳄	𤳸
-𤶊	癐
-𤶧	𤸫
-𤻊	㿗
-𤽯	㿧
-𤾀	皟
-𤿲	麬
-𥁢	䀉
-𥅘	𥌃
-𥅴	䀹
-𥅿	𥊝
-𥆧	瞤
-𥇢	䁪
-𥎝	䂎
-𥐟	礒
-𥐯	𥖅
-𥐰	𥕥
-𥐻	碙
-𥞦	𥞵
-𥧂	𥨐
-𥩟	竚
-𥩺	𥪂
-𥫣	籅
-𥬀	䉙
-𥬞	籋
-𥬠	篘
-𥭉	𥵊
-𥮋	𥸠
-𥮜	䉲
-𥮾	篸
-𥱔	𥵃
-𥹥	𥼽
-𥺅	䊭
-𥺇	𥽖
-𦈈	𥿊
-𦈉	緷
-𦈋	綇
-𦈌	綀
-𦈎	繟
-𦈏	緍
-𦈐	縺
-𦈑	緸
-𦈒	𦂅
-𦈓	䋿
-𦈔	縎
-𦈕	緰
-𦈖	䌈
-𦈗	𦃄
-𦈘	䌋
-𦈙	䌰
-𦈚	縬
-𦈛	繓
-𦈜	䌖
-𦈝	繏
-𦈞	䌟
-𦈟	䌝
-𦈠	䌥
 𦈡	繻
-𦍠	䍽
-𦛨	朥
 𦝼	膢
-𦟗	𦣎
-𦨩	𦪽
-𦰏	蓧
-𦰴	䕳
-𦶟	爇
-𦶻	𦾟
-𦻕	蘟
-𧉐	𧕟
-𧉞	䗿
-𧌥	𧎈
-𧏖	蠙
-𧏗	蠀
-𧑏	蠾
-𧒭	𧔥
-𧜭	䙱
-𧝝	襰
-𧝧	𧟀
-𧮪	詀
-𧳕	𧳟
-𧹑	䞈
-𧹒	買
-𧹓	𧶔
-𧹔	賬
-𧹕	䝻
-𧹖	賟
-𧹗	贃
-𧿈	𨇁
-𨀁	躘
-𨀱	𨄣
-𨁴	𨅍
-𨂺	𨈊
-𨄄	𨈌
-𨅛	䠱
-𨅫	𨇞
-𨅬	躝
-𨉗	軉
-𨐅	軗
-𨐆	𨊻
-𨐇	𨏠
 𨐈	輄
-𨐉	𨎮
-𨐊	𨏥
-𨑹	䢨
-𨟳	𨣞
-𨠨	𨣧
-𨡙	𨢿
-𨡺	𨣈
-𨤰	𨤻
-𨰾	鎷
-𨰿	釳
-𨱀	𨥛
-𨱁	鈠
-𨱂	鈋
-𨱃	鈲
-𨱄	鈯
-𨱅	鉁
-𨱆	龯
 𨱇	銶
-𨱈	鋉
-𨱉	鍄
-𨱊	𨧱
-𨱋	錂
-𨱌	鏆
-𨱍	鎯
-𨱎	鍮
 𨱏	鎝
-𨱐	𨫒
 𨱑	鐄
-𨱒	鏉
-𨱓	鐎
 𨱔	鐏
-𨱕	𨮂
-𨱖	䥩
-𨷿	䦳
-𨸀	𨳕
-𨸁	𨳑
-𨸂	閍
-𨸃	閐
-𨸄	䦘
-𨸅	𨴗
-𨸆	𨵩
-𨸇	𨵸
-𨸉	𨶀
-𨸊	𨶏
-𨸋	𨶲
-𨸌	𨶮
-𨸎	𨷲
-𨸘	𨽏
-𨸟	䧢
-𩏼	䪏
-𩏽	𩏪
-𩏾	𩎢
-𩏿	䪘
-𩐀	䪗
-𩓋	顂
-𩖕	𩓣
-𩖖	顃
-𩖗	䫴
-𩙥	颰
-𩙦	𩗀
-𩙧	䬞
-𩙨	𩘹
-𩙩	𩘀
-𩙪	颷
-𩙫	颾
-𩙬	𩘺
-𩙭	𩘝
-𩙮	䬘
-𩙯	䬝
-𩙰	𩙈
-𩟿	𩚛
-𩠀	𩚥
-𩠁	𩚵
-𩠂	𩛆
-𩠃	𩛩
-𩠅	𩟐
-𩠆	𩜦
-𩠇	䭀
-𩠈	䭃
-𩠉	𩜇
-𩠊	𩜵
-𩠋	𩝔
-𩠌	餸
-𩠎	𩞄
-𩠏	𩞦
-𩠠	𩠴
-𩡖	𩡣
-𩧦	𩡺
-𩧨	駎
-𩧩	𩤊
-𩧪	䮾
-𩧫	駚
-𩧬	𩢡
-𩧭	䭿
-𩧮	𩢾
-𩧯	驋
-𩧰	䮝
-𩧱	𩥉
-𩧲	駧
-𩧳	𩢸
-𩧴	駩
-𩧵	𩢴
-𩧶	𩣏
-𩧸	𩣫
-𩧺	駶
-𩧻	𩣵
-𩧼	𩣺
-𩧿	䮠
-𩨀	騔
-𩨁	䮞
-𩨂	驄
-𩨃	騝
-𩨄	騪
-𩨅	𩤸
-𩨆	𩤙
-𩨇	䮫
-𩨈	騟
-𩨉	𩤲
-𩨊	騚
-𩨋	𩥄
-𩨌	𩥑
-𩨍	𩥇
-𩨎	龭
-𩨏	䮳
-𩨐	𩧆
-𩩈	䯤
-𩬣	𩭙
-𩬤	𩰀
-𩭹	鬖
-𩯒	𩯳
-𩰰	𩰹
-𩲒	𩳤
-𩴌	𩴵
-𩽹	魥
-𩽺	𩵩
-𩽻	𩵹
-𩽼	鯶
-𩽽	𩶱
 𩽾	鮟
-𩽿	𩶰
-𩾁	鯄
-𩾂	䲖
 𩾃	鮸
-𩾄	𩷰
-𩾅	𩸃
-𩾆	𩸦
-𩾇	鯱
-𩾈	䱙
-𩾊	䱬
-𩾋	䱰
 𩾌	鱇
-𩾎	𩽇
-𪉂	䲰
-𪉃	鳼
-𪉄	𩿪
-𪉅	𪀦
-𪉆	鴲
-𪉈	鴜
-𪉉	𪁈
-𪉊	鷨
-𪉋	𪀾
-𪉌	𪁖
-𪉍	鵚
-𪉎	𪂆
-𪉏	𪃏
-𪉐	𪃍
-𪉑	鷔
-𪉒	𪄕
-𪉔	𪄆
-𪉕	𪇳
-𪎈	䴬
-𪎉	麲
-𪎊	麨
-𪎋	䴴
-𪎌	麳
-𪑅	䵳
-𪔭	𪔵
-𪚏	𪘀
-𪚐	𪘯
-𪜎	𠿕
-𪞝	凙
-𪟎	㔋
 𪟝	勣
-𪠀	𧷎
-𪠟	㓄
-𪠡	𠬙
-𪠳	唓
-𪠵	㖮
-𪠸	嚛
-𪠺	𠽃
-𪠽	噹
-𪡀	嘺
-𪡃	嘪
-𪡋	噞
-𪡏	嗹
-𪡛	㗿
-𪡞	嘳
-𪡺	𡃄
-𪢌	㘓
-𪢐	𡃤
-𪢒	𡂡
-𪢕	嚽
-𪢖	𡅯
-𪢠	囒
-𪢮	圞
-𪢸	墲
-𪣆	埬
-𪣒	堚
 𪣻	塿
-𪤄	𡓁
-𪤚	壣
-𪥠	𧹈
-𪥫	孇
-𪥰	嬣
-𪥿	嬻
-𪧀	孾
-𪧘	寠
-𪨊	㞞
-𪨗	屩
-𪨧	崙
-𪨩	𡸗
 𪨶	輋
-𪨷	巗
-𪨹	𡹬
-𪩇	㟺
-𪩎	巊
 𪩘	巘
-𪩛	𡿖
-𪩷	幝
-𪩸	幩
-𪪏	廬
-𪪑	㢗
-𪪞	廧
-𪪴	𢍰
-𪪼	彃
-𪫌	徿
-𪫡	𢤩
-𪫷	㦞
-𪫺	憸
-𪬚	𢣐
-𪬯	𢤿
-𪭝	𢯷
-𪭢	摐
-𪭧	擟
-𪭯	𢶒
-𪭵	掚
-𪭾	撊
-𪮃	㨻
-𪮋	㩋
-𪮖	撧
-𪮳	𢺳
-𪮶	攋
-𪯋	㪎
-𪰶	曊
-𪱥	膹
-𪱷	梖
-𪲎	櫅
-𪲔	欐
-𪲛	檵
-𪲮	櫠
-𪳍	欇
-𪳗	𣜬
-𪴙	欑
-𪵑	毊
-𪵣	霼
-𪵱	濿
-𪶄	溡
-𪶒	𤄷
-𪶮	𣽏
-𪷍	㵾
-𪷽	灒
-𪸕	熂
-𪸩	煇
-𪹀	𤑹
-𪹠	𤓌
-𪹳	爥
-𪹹	𤒻
-𪺣	𤘀
-𪺪	𤜆
-𪺭	犞
-𪺷	獊
-𪺸	𤠮
-𪺻	㺜
-𪺽	猌
-𪻐	瑽
-𪻨	瓄
-𪻲	瑻
-𪻺	璝
-𪼋	㻶
-𪼴	𤬅
-𪽈	畼
-𪽝	𤳷
-𪽪	痮
-𪽭	𤷃
-𪽮	㿖
-𪽴	𤺔
-𪽷	瘱
-𪾔	盨
 𪾢	睍
-𪾣	眝
-𪾦	矑
-𪾸	矉
-𪿊	𥏝
-𪿞	𥖲
-𪿫	礮
-𪿵	𥗇
-𫀌	𥜰
-𫀓	𥜐
-𫀨	䅐
-𫀬	䅳
-𫀮	𥢷
-𫁂	䆉
-𫁟	竱
-𫁡	鴗
-𫁱	𥶽
-𫁲	䉑
-𫁳	𥯤
-𫁷	䉶
-𫁺	𥴼
-𫂃	簢
-𫂆	簂
-𫂈	䉬
-𫂖	𥴨
-𫂿	𥻦
-𫃗	𩏷
-𫄙	糺
-𫄚	䊺
-𫄛	紟
-𫄜	䋃
-𫄝	𥾯
-𫄞	䋔
-𫄟	絁
-𫄠	絙
-𫄡	絧
-𫄢	絥
-𫄣	繷
-𫄤	繨
-𫄥	纚
-𫄦	𦀖
 𫄧	綖
 𫄨	絺
-𫄩	䋦
-𫄪	𦅇
-𫄫	綟
-𫄬	緤
-𫄭	緮
-𫄮	䋼
-𫄯	𦃩
-𫄰	縍
-𫄱	繬
-𫄲	縸
-𫄳	縰
-𫄴	繂
-𫄵	𦅈
-𫄶	繈
 𫄷	繶
 𫄸	纁
-𫄹	纗
-𫅅	䍤
-𫅗	羵
-𫅥	𦒀
-𫅭	䎙
-𫅼	𦔖
-𫆏	聻
-𫆝	𦟼
-𫆫	𦡝
-𫇘	𦧺
-𫇛	艣
-𫇪	𦱌
 𫇭	蔿
-𫇴	蒭
-𫇽	蕽
-𫈉	蕳
-𫈎	葝
-𫈟	蔯
-𫈵	蕝
-𫉁	薆
-𫉄	藷
-𫊪	䗅
-𫊮	蠦
-𫊸	蟜
-𫊹	𧒯
-𫊻	蟳
-𫋇	蟂
-𫋌	蟘
-𫋲	䙔
-𫋷	襗
-𫋹	襓
-𫋻	襘
 𫌀	襀
-𫌇	襵
-𫌋	𧞫
-𫌨	覼
-𫌪	覛
-𫌫	𧡴
-𫌬	𧢄
-𫌭	覹
-𫌯	䚩
-𫍐	𧭹
-𫍙	訑
-𫍚	訞
-𫍛	訜
-𫍜	詓
-𫍝	諫
-𫍞	𧦝
-𫍟	𧦧
-𫍠	䛄
-𫍡	詑
-𫍢	譊
 𫍣	詷
-𫍤	譑
-𫍥	誂
-𫍦	譨
-𫍧	誺
-𫍨	誫
-𫍩	諣
-𫍪	誋
-𫍫	䛳
-𫍬	誷
-𫍭	𧩕
-𫍮	誳
 𫍯	諴
-𫍰	諰
-𫍱	諯
 𫍲	謏
-𫍳	諥
-𫍴	謱
-𫍵	謸
-𫍶	𧩼
-𫍷	謉
-𫍸	謆
-𫍹	謯
-𫍺	𧫝
-𫍻	譆
-𫍼	𧬤
 𫍽	譞
-𫍾	𧭈
-𫍿	譾
-𫎆	豵
-𫎌	貗
-𫎦	贚
-𫎧	䝭
-𫎨	𧸘
-𫎩	賝
-𫎪	䞋
-𫎫	贉
-𫎬	贑
-𫎭	䞓
-𫎱	䟐
-𫎳	䟆
-𫎸	𧽯
-𫎺	䟃
-𫏃	䠆
-𫏆	蹳
-𫏋	蹻
-𫏌	𨂐
-𫏐	蹔
-𫏑	𨇽
-𫏕	𨆪
-𫏞	𨇰
-𫏨	𨇤
 𫐄	軏
-𫐅	軕
-𫐆	轣
-𫐇	軜
-𫐈	軷
-𫐉	軨
-𫐊	軬
-𫐋	𨎌
-𫐌	軿
-𫐍	𨌈
-𫐎	輢
-𫐏	輖
 𫐐	輗
-𫐑	輨
-𫐒	輷
 𫐓	輮
-𫐔	𨍰
-𫐕	轊
-𫐖	轇
-𫐗	轐
-𫐘	轗
-𫐙	轠
-𫐷	遱
-𫑘	鄟
 𫑡	鄳
-𫑷	醶
-𫓥	釟
-𫓦	釨
 𫓧	鈇
-𫓨	鈛
-𫓩	鏦
-𫓪	鈆
-𫓫	𨥟
-𫓬	鉔
-𫓭	鉠
-𫓮	𨪕
 𫓯	銈
-𫓰	銊
-𫓱	鐈
-𫓲	銁
-𫓳	𨰋
-𫓴	鉾
-𫓵	鋠
 𫓶	鋗
-𫓷	𫒡
-𫓸	錽
 𫓹	錤
-𫓺	鐪
-𫓻	錜
-𫓼	𨨛
-𫓽	錝
-𫓾	錥
-𫓿	𨨢
-𫔀	鍊
-𫔁	鐼
-𫔂	鍉
-𫔃	𨰲
-𫔄	鍒
-𫔅	鎍
-𫔆	䥯
-𫔇	鎞
-𫔈	鎙
-𫔉	𨰃
-𫔊	鏥
-𫔋	䥗
-𫔌	鏾
 𫔍	鐇
 𫔎	鐍
-𫔏	𨬖
-𫔐	𨭸
-𫔑	𨭖
-𫔒	𨮳
-𫔓	𨯟
-𫔔	鑴
-𫔕	𨰥
-𫔖	𨲳
-𫔭	開
-𫔮	閒
-𫔯	閗
-𫔰	閞
-𫔲	𨴹
-𫔴	閵
-𫔵	䦯
 𫔶	闑
-𫔽	𨼳
-𫕚	𩀨
-𫕥	霣
-𫕨	𩅙
-𫖃	靧
-𫖅	䪊
-𫖇	鞾
-𫖑	𩎖
-𫖒	韠
-𫖓	𩏂
-𫖔	韛
-𫖕	韝
-𫖖	𩏠
-𫖪	𩑔
-𫖫	䪴
-𫖬	䪾
-𫖭	𩒎
 𫖮	顗
 𫖯	頫
-𫖰	䫂
-𫖱	䫀
-𫖲	䫟
 𫖳	頵
-𫖴	𩔳
-𫖵	𩓥
-𫖶	顅
-𫖷	𩔑
-𫖸	願
-𫖹	顣
-𫖺	䫶
-𫗇	䫻
-𫗈	𩗓
-𫗉	𩗴
-𫗊	䬓
-𫗋	飋
-𫗚	𩟗
-𫗞	飦
-𫗟	䬧
-𫗠	餦
-𫗡	𩚩
-𫗢	飵
-𫗣	飶
-𫗤	𩛌
-𫗥	餫
-𫗦	餔
 𫗧	餗
-𫗨	𩛡
-𫗩	饠
-𫗪	餧
-𫗫	餬
-𫗬	餪
-𫗭	餵
-𫗮	餭
-𫗯	餱
-𫗰	䭔
-𫗱	䭑
-𫗳	𩝽
 𫗴	饘
-𫗵	饟
-𫘛	馯
 𫘜	馼
 𫘝	駃
-𫘞	駞
-𫘟	駊
-𫘠	駤
-𫘡	駫
-𫘣	駻
-𫘤	騃
-𫘥	騉
 𫘦	騊
 𫘧	騄
 𫘨	騠
-𫘩	騜
 𫘪	騵
-𫘫	騴
 𫘬	騱
-𫘭	騻
-𫘮	䮰
-𫘯	驓
-𫘰	驙
-𫘱	驨
-𫘽	鬠
-𫙂	𩯁
-𫚈	鱮
-𫚉	魟
-𫚊	鰑
-𫚋	鱄
-𫚌	魦
-𫚍	魵
-𫚎	𩶁
-𫚏	䱁
-𫚐	䱀
-𫚑	鮅
-𫚒	鮄
-𫚓	鮤
-𫚔	鮰
 𫚕	鰤
 𫚖	鮆
-𫚗	鮯
-𫚘	𩻮
-𫚙	鯆
-𫚚	鮿
-𫚛	鮵
-𫚜	䲅
-𫚝	𩸄
-𫚞	鯬
-𫚟	𩸡
-𫚠	䱧
-𫚡	鯞
-𫚢	鰋
-𫚣	鯾
-𫚤	鰦
-𫚥	鰕
-𫚦	鰫
-𫚧	鰽
-𫚨	𩻗
-𫚩	𩻬
-𫚪	鱊
-𫚫	鱢
-𫚬	𩼶
 𫚭	鱲
-𫛚	鳽
-𫛛	鳷
-𫛜	鴀
-𫛝	鴅
-𫛞	鴃
-𫛟	鸗
-𫛠	𩿤
-𫛡	鴔
-𫛢	鸋
-𫛣	鴥
-𫛤	鴐
-𫛥	鵊
-𫛦	鴮
-𫛧	𪀖
-𫛨	鵧
-𫛩	鴳
-𫛪	鴽
-𫛫	鶰
-𫛬	䳜
 𫛭	鵟
-𫛮	䳤
-𫛯	鶭
-𫛰	䳢
-𫛱	鵫
-𫛲	鵰
-𫛳	鵩
-𫛴	鷤
-𫛵	鶌
-𫛶	鶒
-𫛷	鶦
-𫛸	鶗
-𫛹	𪃧
-𫛺	䳧
-𫛻	𪃒
-𫛼	䳫
-𫛽	鷅
-𫛾	𪆷
-𫜀	鷐
-𫜁	鷩
-𫜂	𪅂
-𫜃	鷣
-𫜄	鷷
-𫜅	䴋
-𫜊	𪉸
-𫜑	麷
-𫜒	䴱
-𫜓	𪌭
-𫜔	䴽
-𫜕	𪍠
-𫜙	䵴
-𫜟	𪓰
-𫜨	䶕
-𫜩	齧
-𫜪	齩
-𫜫	𫜦
-𫜬	齰
-𫜭	齭
-𫜮	齴
-𫜯	𪙏
-𫜰	齾
-𫜲	龓
-𫜳	䶲
-𫝈	㑮
-𫝋	𠐊
-𫝦	㛝
-𫝧	㜐
-𫝨	媈
-𫝩	嬦
-𫝪	𡟫
-𫝫	婡
-𫝬	嬇
-𫝭	孆
-𫝮	孄
-𫝵	嶹
-𫞅	𦠅
-𫞗	潣
-𫞚	澬
-𫞛	㶆
-𫞝	灍
-𫞠	爧
-𫞡	爃
-𫞢	𤛱
-𫞣	㹽
-𫞥	珼
-𫞦	璾
-𫞧	𤩂
-𫞨	璼
 𫞩	璊
-𫞷	𥢶
-𫟃	絍
-𫟄	綋
 𫟅	綡
-𫟆	緟
-𫟇	𦆲
-𫟑	䖅
-𫟕	䕤
-𫟞	訨
-𫟟	詊
-𫟠	譂
-𫟡	誴
-𫟢	䜖
-𫟤	䡐
-𫟥	䡩
 𫟦	䡵
-𫟫	𨞺
-𫟬	𨟊
-𫟲	釚
-𫟳	釲
-𫟴	鈖
-𫟵	鈗
-𫟶	銏
-𫟷	鉝
-𫟸	鉽
 𫟹	鉷
-𫟺	䤤
-𫟻	銂
 𫟼	鐽
-𫟽	𨧰
-𫟾	𨩰
-𫟿	鎈
-𫠀	䥄
-𫠁	鑉
-𫠂	閝
-𫠅	韚
 𫠆	頍
-𫠇	𩖰
-𫠈	䫾
 𫠊	䮄
-𫠋	騼
-𫠌	𩦠
-𫠏	𩵦
-𫠐	魽
-𫠑	䱸
-𫠒	鱆
-𫠖	𩿅
 𫠜	齯
 𫢸	僤
-𫧃	𣍐
-𫧮	𪋿
 𫫇	噁
-𫬐	㘔
 𫭟	塸
 𫭢	埨
 𫭼	𡑍
 𫮃	墠
 𫰛	娙
 𫵷	㠣
 𫶇	嵽
@@ -3930,15 +2763,14 @@
 𬭊	𨧀
 𬭎	鋐
 𬭚	錞
 𬭛	𨨏
 𬭤	鍭
 𬭩	鎓
 𬭬	鏏
-𬭭	鏚
 𬭯	䥕
 𬭳	𨭎
 𬭶	𨭆
 𬭸	鏻
 𬭼	鐩
 𬮱	闉
 𬮿	隑
@@ -3964,17 +2796,10 @@
 𬶮	鱚
 𬷕	鵏
 𬸘	鶠
 𬸚	鸑
 𬸣	鶱
 𬸦	鷟
 𬸪	鷭
-𬸯	鷿
 𬹼	齘
 𬺈	齮
 𬺓	齼
-𰬸	繐
-𰰨	菕
-𰶎	譅
-𰾄	鋂
-𰾭	鑀
-𱊜	𪈼
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.24.0/sts/data/dictionary/STPhrases.txt`

 * *Files 0% similar despite different names*

```diff
@@ -47092,15 +47092,15 @@
 雇用	僱用
 雌核	雌核
 雌雄同体	雌雄同體
 雌雄同体人	雌雄同體人
 雌雄同株	雌雄同株
 雍容闲雅	雍容閒雅
 雕丧	雕喪
-雕丽	雕麗
+雕丽	琱麗
 雕云	雕雲
 雕像	雕像
 雕具座	鵰具座
 雕出	雕出
 雕凿	雕鑿
 雕刻	雕刻
 雕刻出	雕刻出
@@ -47113,21 +47113,23 @@
 雕刻画	雕刻畫
 雕励	雕勵
 雕啄	雕啄
 雕塑	雕塑
 雕塑品	雕塑品
 雕塑家	雕塑家
 雕墙	雕牆
+雕履	琱履
 雕工	雕工
-雕弓	雕弓
+雕弓	琱弓
 雕心雁爪	鵰心雁爪
 雕悍	鵰悍
-雕戈	雕戈
+雕戈	琱戈
 雕成	雕成
 雕敝	雕敝
+雕文	琱文
 雕板	雕板
 雕栏	雕欄
 雕梁	雕樑
 雕梁画柱	雕樑畫柱
 雕梁画栋	雕樑畫棟
 雕楹碧槛	雕楹碧檻
 雕残	雕殘
@@ -47144,14 +47146,15 @@
 雕绘	雕繪
 雕翎	鵰翎
 雕翎扇	鵰翎扇
 雕肝琢肾	雕肝琢腎
 雕肝琢膂	雕肝琢膂
 雕肝镂肾	雕肝鏤腎
 雕胡米	雕胡米
+雕舆	琱輿
 雕色	雕色
 雕花	雕花
 雕花漆彩	雕花漆彩
 雕虫	雕蟲
 雕虫小技	雕蟲小技
 雕虫小艺	雕蟲小藝
 雕虫篆	雕蟲篆
@@ -47160,15 +47163,15 @@
 雕谢	雕謝
 雕镂	雕鏤
 雕镌	雕鐫
 雕零	雕零
 雕青	雕青
 雕题	雕題
 雕飕	雕颼
-雕饰	雕飾
+雕饰	琱飾
 雕饰品	雕飾品
 雕骚	雕騷
 雕鹗	鵰鶚
 雕龙	雕龍
 雨云	雨雲
 雨余芳草斜阳	雨餘芳草斜陽
 雨刮	雨刮
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.24.0/sts/data/dictionary/TSCharacters.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,1112 +1,1123 @@
-㑮	𫝈
-㑯	㑔
 㑳	㑇
-㑶	㐹
-㒓	𠉂
-㓄	𪠟
-㓨	刾
-㔋	𪟎
-㖮	𪠵
-㗲	𠵾
-㗿	𪡛
-㘉	𠰱
-㘓	𪢌
-㘔	𫬐
+㑺	俊
+㒺	罔
+㕁	却
+㕑	厨
+㕘	参
+㕥	以
 㘚	㘎
-㛝	𫝦
-㜄	㚯
-㜏	㛣
-㜐	𫝧
-㜗	𡞋
-㜢	𡞱
-㜷	𡝠
-㞞	𪨊
-㟺	𪩇
-㠏	㟆
+㘭	坳
+㝛	宿
+㝠	冥
+㝡	最
+㟁	岸
+㠀	岛
 㠣	𫵷
-㢗	𪪑
-㢝	𢋈
+㠯	以
+㠶	帆
+㡌	帽
+㢘	廉
+㤙	恩
+㥦	惬
+㥫	惇
 㥮	㤘
-㦎	𢛯
-㦛	𢗓
-㦞	𪫷
-㨻	𪮃
-㩋	𪮋
-㩜	㨫
+㧱	拿
+㨗	捷
+㨪	晃
+㨿	据
+㩗	携
+㩦	携
 㩳	㧐
-㩵	擜
-㪎	𪯋
-㯤	𣘐
-㰙	𣗙
-㵗	𣳆
-㵾	𪷍
-㶆	𫞛
-㷍	𤆢
-㷿	𤈷
-㸇	𤎺
-㹽	𫞣
-㺏	𤠋
-㺜	𪺻
-㻶	𪼋
-㿖	𪽮
-㿗	𤻊
-㿧	𤽯
-䀉	𥁢
-䀹	𥅴
-䁪	𥇢
-䁻	䀥
-䂎	𥎝
+㪚	散
+㪟	敦
+㬉	暖
+㬪	叠
+㮣	概
+㯭	橹
+㱃	饮
+㳄	涎
+㳒	法
+㴱	深
+㼝	碗
+㽞	留
+㿜	瘪
 䃮	鿎
-䅐	𫀨
-䅳	𫀬
-䆉	𫁂
-䉑	𫁲
-䉙	𥬀
-䉬	𫂈
-䉲	𥮜
-䉶	𫁷
-䊭	𥺅
-䊷	䌶
-䊺	𫄚
-䋃	𫄜
-䋔	𫄞
-䋙	䌺
-䋚	䌻
-䋦	𫄩
-䋹	䌿
-䋻	䌾
-䋼	𫄮
-䋿	𦈓
-䌈	𦈖
-䌋	𦈘
-䌖	𦈜
-䌝	𦈟
-䌟	𦈞
-䌥	𦈠
-䌰	𦈙
-䍤	𫅅
-䍦	䍠
-䍽	𦍠
-䎙	𫅭
-䎱	䎬
+䈰	筲
+䊀	糊
 䓣	𬜯
-䕤	𫟕
-䕳	𦰴
-䖅	𫟑
-䗅	𫊪
-䗿	𧉞
-䙔	𫋲
-䙡	䙌
-䙱	𧜭
-䚩	𫌯
-䛄	𫍠
-䛳	𫍫
-䜀	䜧
-䜖	𫟢
-䝭	𫎧
-䝻	𧹕
-䝼	䞍
-䞈	𧹑
-䞋	𫎪
-䞓	𫎭
-䟃	𫎺
-䟆	𫎳
-䟐	𫎱
-䠆	𫏃
-䠱	𨅛
-䡐	𫟤
-䡩	𫟥
+䗬	蜂
+䘏	恤
+䘑	脉
+䘚	卒
+䛐	词
+䛡	话
+䝔	獾
+䠀	蹚
+䠶	射
 䡵	𫟦
-䢨	𨑹
-䤤	𫟺
-䥄	𫠀
-䥇	䦂
 䥑	鿏
 䥕	𬭯
-䥗	𫔋
-䥩	𨱖
-䥯	𫔆
-䥱	䥾
-䦘	𨸄
-䦛	䦶
-䦟	䦷
-䦯	𫔵
-䦳	𨷿
-䧢	𨸟
-䪊	𫖅
-䪏	𩏼
-䪗	𩐀
-䪘	𩏿
-䪴	𫖫
-䪾	𫖬
-䫀	𫖱
-䫂	𫖰
-䫟	𫖲
-䫴	𩖗
-䫶	𫖺
-䫻	𫗇
-䫾	𫠈
-䬓	𫗊
-䬘	𩙮
-䬝	𩙯
-䬞	𩙧
-䬧	𫗟
-䭀	𩠇
-䭃	𩠈
-䭑	𫗱
-䭔	𫗰
-䭿	𩧭
+䥥	镰
+䬃	飒
+䭾	驮
 䮄	𫠊
-䮝	𩧰
-䮞	𩨁
-䮠	𩧿
-䮫	𩨇
-䮰	𫘮
-䮳	𩨏
-䮾	𩧪
-䯀	䯅
-䯤	𩩈
+䰟	魂
 䰾	鲃
-䱀	𫚐
-䱁	𫚏
-䱙	𩾈
-䱧	𫚠
-䱬	𩾊
-䱰	𩾋
-䱷	䲣
-䱸	𫠑
-䱽	䲝
 䲁	鳚
-䲅	𫚜
-䲖	𩾂
 䲘	鳤
-䲰	𪉂
-䳜	𫛬
-䳢	𫛰
-䳤	𫛮
-䳧	𫛺
-䳫	𫛼
+䳘	鹅
 䴉	鹮
-䴋	𫜅
-䴬	𪎈
-䴱	𫜒
-䴴	𪎋
-䴽	𫜔
-䵳	𪑅
-䵴	𫜙
-䶕	𫜨
-䶲	𫜳
+䴸	麸
+䶊	衄
 丟	丢
 並	并
+乗	乘
+乹	干
 乾	干 乾
+亁	干
 亂	乱
 亙	亘
+亝	斋
 亞	亚
+亯	享
+亱	夜
+亷	廉
+亾	亡
+仝	仝 同
+佀	似
 佇	伫
 佈	布
 佔	占
 併	并
 來	来
 侖	仑
 侶	侣
 侷	局
 俁	俣
 係	系
-俓	𠇹
 俔	伣
+俛	俯
 俠	侠
-俥	伡
 俬	私
+俻	备
 倀	伥
+倃	咱
 倆	俩
 倈	俫
 倉	仓
 個	个
+倐	倏
 們	们
 倖	幸
+倣	仿
 倫	伦
-倲	㑈
+倸	睬
 偉	伟
-偑	㐽
+偘	侃
+偪	逼
 側	侧
 偵	侦
+偺	咱
 偽	伪
-傌	㐷
+傌	骂
 傑	杰
 傖	伧
 傘	伞
 備	备
+傚	效
 傢	家
 傭	佣
 傯	偬
 傳	传
 傴	伛
 債	债
 傷	伤
 傾	倾
 僂	偻
 僅	仅
 僉	佥
+僊	仙
+働	动
 僑	侨
 僕	仆
 僞	伪
 僤	𫢸
 僥	侥
 僨	偾
 僱	雇
 價	价
 儀	仪
 儁	俊
 儂	侬
 億	亿
 儈	侩
 儉	俭
-儎	傤
+儌	侥
 儐	傧
 儔	俦
 儕	侪
-儘	尽 侭
+儗	拟
+儘	尽
 償	偿
-儣	𠆲
 優	优
-儭	𠋆
 儲	储
+儵	倏
 儷	俪
-儸	㑩
 儺	傩
 儻	傥
 儼	俨
 兇	凶
 兌	兑
+兎	兔
 兒	儿
 兗	兖
+兠	兜
 內	内
 兩	两
+冄	冉
 冊	册
+冐	冒
 冑	胄
+冣	最
 冪	幂
+冺	泯
 凈	净
 凍	冻
-凙	𪞝
 凜	凛
+凢	凡
 凱	凯
+凴	凭
 別	别
+刦	劫
+刧	劫
 刪	删
+刼	劫
 剄	刭
 則	则
+剉	锉
 剋	克 剋
 剎	刹
+剏	创
 剗	刬
+剙	创
 剛	刚
 剝	剥
 剮	剐
+剳	札
 剴	剀
 創	创
 剷	铲
-剾	𠛅
-劃	划 㓰
+剹	戮
+劃	划
+劄	札 劄
 劇	剧
 劉	刘
 劊	刽
 劌	刿
 劍	剑
-劏	㓥
 劑	剂
-劚	㔉
+劒	剑
+劵	券
+効	效
 勁	劲
-勑	𠡠
+勅	敕
+勌	倦
+勑	敕
 動	动
+勗	勖
 務	务
 勛	勋
 勝	胜
 勞	劳
 勢	势
-勣	𪟝
+勣	𪟝 绩
+勦	剿
 勩	勚
 勱	劢
 勳	勋
 勵	励
 勸	劝
 勻	匀
+匃	丐
+匄	丐
+匟	炕
 匭	匦
 匯	汇
 匱	匮
+匲	奁
+匳	奁
 區	区
 協	协
 卹	恤
 卻	却
 卽	即
+厀	膝
 厙	厍
 厠	厕
 厤	历
 厭	厌
 厲	厉
 厴	厣
 參	参
 叄	叁
+叚	叚 假
+叡	睿
 叢	丛
-吒	咤
+吒	吒 咤
+吚	咿
 吳	吴
 吶	呐
 呂	吕
+呌	叫
+呪	咒
+咊	和
+咲	笑
 咼	呙
 員	员
-哯	𠯟
+哶	咩
 唄	呗
-唓	𪠳
+唕	唣
+唘	启
+唫	吟
 唸	念
+啎	忤
 問	问
+啑	喋
 啓	启
+啗	啖
 啞	哑
 啟	启
-啢	唡
-喎	㖞
+啣	衔
+喆	喆 哲
+喒	咱
 喚	唤
 喪	丧
 喫	吃
 喬	乔
 單	单
 喲	哟
+嗁	啼
 嗆	呛
 嗇	啬
 嗊	唝
 嗎	吗
 嗚	呜
 嗩	唢
-嗰	𠮶
 嗶	哔
-嗹	𪡏
+嘅	慨
 嘆	叹
 嘍	喽
-嘓	啯
+嘑	呼
 嘔	呕
 嘖	啧
 嘗	尝
 嘜	唛
+嘠	嘎
 嘩	哗
-嘪	𪡃
 嘮	唠
 嘯	啸
 嘰	叽
-嘳	𪡞
 嘵	哓
+嘷	嗥
 嘸	呒
-嘺	𪡀
 嘽	啴
 噁	恶 𫫇
-噅	𠯠
+噉	啖
 噓	嘘
-噚	㖊
 噝	咝
-噞	𪡋
 噠	哒
 噥	哝
 噦	哕
 噯	嗳
 噲	哙
 噴	喷
 噸	吨
-噹	当 𪠽
+噹	当
 嚀	咛
 嚇	吓
-嚌	哜
 嚐	尝
 嚕	噜
 嚙	啮
-嚛	𪠸
 嚥	咽
 嚦	呖
-嚧	𠰷
 嚨	咙
 嚮	向
 嚲	亸
 嚳	喾
 嚴	严
 嚶	嘤
-嚽	𪢕
 囀	啭
 囁	嗫
 囂	嚣
-囃	𠱞
 囅	冁
 囈	呓
 囉	啰
 囌	苏
 囑	嘱
-囒	𪢠
+囓	啮
+囙	因
 囪	囱
+圅	函
 圇	囵
 國	国
 圍	围
 園	园
 圓	圆
 圖	图
 團	团
-圞	𪢮
+坵	丘
+坿	附
+垜	垛
 垻	坝
+埜	野
 埡	垭
 埨	𫭢
-埬	𪣆
 埰	采
+埳	坎
 執	执
+堃	堃 坤
 堅	坚
 堊	垩
 堖	垴
-堚	𪣒
+堘	塍
 堝	埚
+堦	阶
 堯	尧
 報	报
 場	场
+堿	碱
 塊	块
 塋	茔
 塏	垲
 塒	埘
 塗	涂
 塚	冢
+塟	葬
 塢	坞
 塤	埙
+塲	场
 塵	尘
 塸	𫭟
 塹	堑
+塼	砖
 塿	𪣻
 墊	垫
+墖	塔
 墜	坠
 墠	𫮃
+墪	墩
 墮	堕
 墰	坛
-墲	𪢸
 墳	坟
 墶	垯
 墻	墙
 墾	垦
 壇	坛
-壈	𡒄
 壋	垱
 壎	埙
 壓	压
-壗	𡋤
 壘	垒
 壙	圹
 壚	垆
 壜	坛
 壞	坏
 壟	垄
-壠	垅
 壢	坜
-壣	𪤚
 壩	坝
 壪	塆
 壯	壮
 壺	壶
+壻	婿
 壼	壸
 壽	寿
+夘	卯
 夠	够
 夢	梦
 夥	伙 夥
 夾	夹
 奐	奂
 奧	奥
 奩	奁
 奪	夺
 奬	奖
 奮	奋
 奼	姹
 妝	妆
+妬	妒
+妳	你 奶
+妷	侄
+姉	姊
 姍	姗
+姙	妊
 姦	奸
+姪	侄
 娙	𫰛
 娛	娱
+娿	婀
 婁	娄
-婡	𫝫
+婣	姻
 婦	妇
+婬	淫
 婭	娅
-媈	𫝨
+媍	妇
 媧	娲
+媮	偷
 媯	妫
-媰	㛀
 媼	媪
 媽	妈
+媿	愧
 嫋	袅
 嫗	妪
+嫰	嫩
 嫵	妩
 嫺	娴
 嫻	娴
 嫿	婳
 嬀	妫
 嬃	媭
-嬇	𫝬
 嬈	娆
 嬋	婵
 嬌	娇
 嬙	嫱
+嬝	袅
 嬡	嫒
-嬣	𪥰
 嬤	嬷
-嬦	𫝩
 嬪	嫔
+嬭	奶
 嬰	婴
 嬸	婶
-嬻	𪥿
+嬾	懒
 孃	娘
-孄	𫝮
-孆	𫝭
-孇	𪥫
-孋	㛤
 孌	娈
-孎	𡠟
 孫	孙
 學	学
-孻	𡥧
-孾	𪧀
+孼	孽
 孿	孪
+宂	冗 穴
 宮	宫
 寀	采
-寠	𪧘
+寃	冤
+寑	寝
+寔	实
+寕	宁
+寘	置
 寢	寝
 實	实
 寧	宁
 審	审
 寫	写
 寬	宽
+寳	宝
 寵	宠
 寶	宝
+尅	克 剋
 將	将
 專	专
 尋	寻
 對	对
 導	导
+尒	尔
+尟	鲜
+尠	鲜
 尷	尴
 屆	届
 屍	尸
 屓	屃
 屜	屉
 屢	屡
 層	层
 屨	屦
-屩	𪨗
 屬	属
+岅	坂
 岡	冈
+峝	峒
+峩	峨
 峯	峰
 峴	岘
 島	岛
 峽	峡
 崍	崃
+崐	昆
 崑	昆
 崗	岗
-崙	仑 𪨧
+崘	仑
+崙	仑
 崢	峥
 崬	岽
 嵐	岚
+嵒	岩
 嵗	岁
-嵼	𡶴
 嵽	𫶇
-嵾	㟥
 嶁	嵝
+嶃	崭
 嶄	崭
 嶇	岖
-嶈	𡺃
 嶔	嵚
 嶗	崂
-嶘	𡺄
 嶠	峤
 嶢	峣
 嶧	峄
 嶨	峃
 嶮	崄
 嶸	嵘
-嶹	𫝵
 嶺	岭
 嶼	屿
 嶽	岳
-巊	𪩎
 巋	岿
 巒	峦
 巔	巅
 巖	岩
-巗	𪨷
+巗	岩
 巘	𪩘
 巰	巯
+巵	卮
 巹	卺
+帀	匝
+帋	纸
 帥	帅
 師	师
+帬	裙
 帳	帐
 帶	带
 幀	帧
 幃	帏
-幓	㡎
+幇	帮
+幑	徽
 幗	帼
 幘	帻
-幝	𪩷
+幙	幕
+幚	帮
 幟	帜
 幣	币
-幩	𪩸
 幫	帮
 幬	帱
 幹	干
 幾	几
 庫	库
+庻	庶
+庽	寓
 廁	厕
 廂	厢
 廄	厩
 廈	厦
 廎	庼
+廐	厩
 廕	荫
 廚	厨
 廝	厮
 廞	𫷷
 廟	庙
 廠	厂
 廡	庑
 廢	废
 廣	广
-廧	𪪞
 廩	廪
-廬	庐 𪪏
+廬	庐
 廳	厅
+廵	巡
+廹	迫
+廻	回
+廼	乃
 弒	弑
 弔	吊
-弳	弪
 張	张
 強	强
-彃	𪪼
 彄	𫸩
 彆	别
 彈	弹
+彊	强
 彌	弥
 彎	弯
 彔	录
 彙	汇
 彠	彟
 彥	彦
 彫	雕
-彲	彨
 彷	彷 仿
 彿	佛
+徃	往
 後	后
 徑	径
 從	从
 徠	徕
+徧	遍
 復	复
 徵	征 徵
 徹	彻
-徿	𪫌
+怱	匆
+怳	恍
 恆	恒
+恠	怪
+恡	吝
 恥	耻
 悅	悦
-悞	悮
+悤	匆
 悵	怅
 悶	闷
 悽	凄
+惏	婪
 惡	恶
+惥	恿
+惪	德
 惱	恼
 惲	恽
+惷	蠢
 惻	恻
 愛	爱
 愜	惬
 愨	悫
+愬	诉
 愴	怆
 愷	恺
-愻	𢙏
+愽	博
 愾	忾
+慂	恿
 慄	栗
+慇	殷
 態	态
 慍	愠
 慘	惨
+慙	惭
 慚	惭
 慟	恸
 慣	惯
 慤	悫
 慪	怄
 慫	怂
 慮	虑
 慳	悭
+慴	慑
 慶	庆
-慺	㥪
 慼	戚
+慽	戚
 慾	欲
 憂	忧
+憇	憩
 憊	惫
 憐	怜
 憑	凭
 憒	愦
 憖	慭
 憚	惮
-憢	𢙒
 憤	愤
 憫	悯
 憮	怃
 憲	宪
 憶	忆
-憸	𪫺
-憹	𢙐
-懀	𢙓
+懃	勤
 懇	恳
 應	应
 懌	怿
 懍	懔
-懎	𢠁
 懞	蒙
 懟	怼
 懣	懑
-懤	㤽
 懨	恹
 懲	惩
 懶	懒
 懷	怀
 懸	悬
 懺	忏
 懼	惧
+懽	欢
 懾	慑
 戀	恋
 戇	戆
 戔	戋
+戞	戛
 戧	戗
 戩	戬
-戰	战 𢧐
-戱	戯
+戯	戏
+戰	战
 戲	戏
 戶	户
+戹	厄
+戼	卯
+扞	捍 扞
+抝	拗
 拋	抛
-挩	捝
+拏	拿
+拕	拖
+挐	拿
 挱	挲
+挵	弄
 挾	挟
+捄	救
 捨	舍
 捫	扪
 捱	挨
 捲	卷
 掃	扫
 掄	抡
-掆	㧏
-掗	挜
 掙	挣
-掚	𪭵
 掛	挂
 採	采
+掽	碰
 揀	拣
+揑	捏
 揚	扬
 換	换
+揫	揪
 揮	挥
-揯	搄
+揷	插
+揹	背
+搆	构
+搇	揿
+搉	榷
 損	损
 搖	摇
 搗	捣
-搵	揾
+搤	扼
+搥	捶
+搨	拓
+搯	掏
 搶	抢
-摋	𢫬
-摐	𪭢
+搾	榨
+摃	扛
 摑	掴
 摜	掼
 摟	搂
 摯	挚
 摳	抠
 摶	抟
 摺	折
 摻	掺
 撈	捞
-撊	𪭾
 撏	挦
 撐	撑
 撓	挠
 撝	㧑
-撟	挢
 撣	掸
 撥	拨
-撧	𪮖
+撦	扯
 撫	抚
 撲	扑
 撳	揿
 撻	挞
 撾	挝
 撿	捡
 擁	拥
 擄	掳
 擇	择
 擊	击
 擋	挡
 擓	㧟
 擔	担
+擕	携
 據	据
-擟	𪭧
 擠	挤
-擣	捣 𢭏
-擫	𢬍
+擣	捣
+擧	举
 擬	拟
 擯	摈
 擰	拧
 擱	搁
 擲	掷
 擴	扩
 擷	撷
 擺	摆
 擻	擞
 擼	撸
-擽	㧰
 擾	扰
 攄	摅
 攆	撵
-攋	𪮶
 攏	拢
 攔	拦
 攖	撄
 攙	搀
 攛	撺
 攜	携
 攝	摄
 攢	攒
 攣	挛
 攤	摊
+攩	挡
 攪	搅
 攬	揽
+攷	考
+敂	叩
+敍	叙
 敎	教
-敓	敚
 敗	败
 敘	叙
+敭	扬
 敵	敌
 數	数
+敺	驱
 斂	敛
 斃	毙
-斅	𢽾
 斆	敩
 斕	斓
 斬	斩
+斮	斫
+斲	斫
+斵	斫
 斷	断
-斸	𣃁
 於	于 於
 旂	旗
 旣	既
-昇	升
+旤	祸
+旹	时
+旾	春
+昇	升 昇
+昚	慎
+昬	昏
+昰	是
 時	时
 晉	晋
 晛	𬀪
 晝	昼
+晳	晰
+晻	暗
 暈	晕
 暉	晖
+暎	映
 暐	𬀩
 暘	旸
+暠	皓
 暢	畅
 暫	暂
+暱	昵
 曄	晔
 曆	历
 曇	昙
 曉	晓
-曊	𪰶
 曏	向
 曖	暧
 曠	旷
-曥	𣆐
+曡	叠
 曨	昽
 曬	晒
 書	书
 會	会
-朥	𦛨
+朞	期
+朢	望
 朧	胧
 朮	术
+朶	朵
 東	东
+枏	楠
+枒	丫
 枴	拐
+柟	楠
 柵	栅
+柹	柿
 柺	拐
 査	查
-桱	𣐕
+栁	柳
+栞	刊
+栢	柏
+栰	筏
+桒	桑
+桮	杯
+桺	柳
 桿	杆
 梔	栀
-梖	𪱷
 梘	枧
 梜	𬂩
 條	条
 梟	枭
 梲	棁
+棃	梨
 棄	弃
 棊	棋
 棖	枨
 棗	枣
 棟	栋
 棡	㭎
 棧	栈
 棲	栖
 棶	梾
-椏	桠
-椲	㭏
-楇	𣒌
+椀	椀 碗
+椉	乘
+椏	桠 丫
+椗	碇
+椶	棕
+椷	缄
+椾	笺
 楊	杨
 楓	枫
+楥	楦
 楨	桢
 業	业
+楳	梅
 極	极
 榘	矩
 榦	干
 榪	杩
 榮	荣
 榲	榅
 榿	桤
+槀	槁
 構	构
 槍	枪
+槑	梅
 槓	杠
+槕	桌
 槤	梿
 槧	椠
 槨	椁
-槫	𣏢
-槮	椮
 槳	桨
-槶	椢
-槼	椝
+槼	规
 樁	桩
 樂	乐
 樅	枞
+樐	橹
 樑	梁
 樓	楼
 標	标
 樞	枢
-樠	𣗊
-樢	㭤
 樣	样
-樤	𣔌
-樧	榝
-樫	㭴
-樳	桪
 樸	朴
 樹	树
 樺	桦
-樿	椫
 橈	桡
 橋	桥
+橜	橛
 機	机
 橢	椭
+橤	蕊
 橫	横
-橯	𣓿
 檁	檩
 檉	柽
 檔	档
 檜	桧
+檝	楫
 檟	槚
 檢	检
 檣	樯
-檭	𣘴
 檮	梼
 檯	台
 檳	槟
-檵	𪲛
 檸	柠
 檻	槛
+櫂	棹
 櫃	柜
-櫅	𪲎
+櫈	凳
 櫍	𬃊
 櫓	橹
 櫚	榈
 櫛	栉
 櫝	椟
 櫞	橼
 櫟	栎
-櫠	𪲮
 櫥	橱
 櫧	槠
 櫨	栌
 櫪	枥
 櫫	橥
 櫬	榇
 櫱	蘖
 櫳	栊
 櫸	榉
 櫻	樱
 欄	栏
 欅	榉
-欇	𪳍
 權	权
-欍	𣐤
 欏	椤
-欐	𪲔
-欑	𪴙
 欒	栾
 欓	𣗋
 欖	榄
-欘	𣚚
+欝	郁
 欞	棂
+欬	咳
+欵	款
 欽	钦
 歎	叹
 歐	欧
+歛	敛
 歟	欤
 歡	欢
 歲	岁
+歴	历
 歷	历
 歸	归
 歿	殁
+殀	夭
 殘	残
 殞	殒
-殢	𣨼
 殤	殇
-殨	㱮
 殫	殚
 殭	僵
 殮	殓
 殯	殡
-殰	㱩
 殲	歼
 殺	杀
 殻	壳
 殼	壳
+殽	淆
 毀	毁
 毆	殴
-毊	𪵑
+毘	毗
+毧	绒
+毬	球
 毿	毵
 氂	牦
 氈	毡
+氊	毡
 氌	氇
 氣	气
 氫	氢
 氬	氩
-氭	𣱝
 氳	氲
-氾	泛
+氷	冰
+氾	泛 氾
 汎	泛
 汙	污
+汚	污
 決	决
 沒	没
 沖	冲
 況	况
 泝	溯
 洩	泄
 洶	汹
 浹	浃
 浿	𬇙
 涇	泾
-涗	涚
+涖	莅
 涼	凉
 淒	凄
 淚	泪
+淛	浙
 淥	渌
 淨	净
 淩	凌
 淪	沦
 淵	渊
 淶	涞
 淺	浅
+淼	淼 渺
 渙	涣
 減	减
 渢	沨
 渦	涡
 測	测
 渾	浑
 湊	凑
 湋	𣲗
 湞	浈
 湧	涌
 湯	汤
+湻	淳
+湼	涅
 溈	沩
 準	准
 溝	沟
-溡	𪶄
 溫	温
 溮	浉
 溳	涢
 溼	湿
 滄	沧
 滅	灭
 滌	涤
 滎	荥
 滙	汇
+滛	淫
 滬	沪
 滯	滞
 滲	渗
 滷	卤
 滸	浒
 滻	浐
 滾	滚
@@ -1119,264 +1130,281 @@
 漣	涟
 漬	渍
 漲	涨
 漵	溆
 漸	渐
 漿	浆
 潁	颍
+潄	漱
 潑	泼
 潔	洁
 潕	𣲘
 潙	沩
-潚	㴋
 潛	潜
-潣	𫞗
 潤	润
 潯	浔
 潰	溃
 潷	滗
 潿	涠
 澀	涩
-澅	𣶩
+澁	涩
+澂	澂 澄
 澆	浇
 澇	涝
 澐	沄
 澗	涧
 澠	渑
+澣	浣
 澤	泽
 澦	滪
-澩	泶
 澫	𬇕
-澬	𫞚
 澮	浍
 澱	淀
-澾	㳠
 濁	浊
 濃	浓
-濄	㳡
 濆	𣸣
+濇	涩
 濕	湿
 濘	泞
 濚	溁
 濛	蒙
 濜	浕
 濟	济
 濤	涛
-濧	㳔
 濫	滥
+濬	浚
 濰	潍
 濱	滨
+濶	阔
 濺	溅
 濼	泺
 濾	滤
-濿	𪵱
 瀂	澛
-瀃	𣽷
 瀅	滢
 瀆	渎
-瀇	㲿
 瀉	泻
-瀋	沈 渖
+瀋	沈
 瀏	浏
 瀕	濒
 瀘	泸
 瀝	沥
 瀟	潇
 瀠	潆
 瀦	潴
 瀧	泷
 瀨	濑
-瀰	弥 㳽
+瀰	弥
 瀲	潋
 瀾	澜
 灃	沣
 灄	滠
-灍	𫞝
+灋	法
 灑	洒
-灒	𪷽
 灕	漓
 灘	滩
-灙	𣺼
 灝	灏
-灡	㳕
 灣	湾
 灤	滦
 灧	滟
+灨	赣
 灩	滟
 災	灾
+炤	照
 為	为
 烏	乌
+烖	灾
+烱	炯
 烴	烃
 無	无
-煇	𪸩
+煇	辉
 煉	炼
+煑	煮
 煒	炜
+煖	暖
+煗	暖
 煙	烟
 煢	茕
 煥	焕
 煩	烦
 煬	炀
-煱	㶽
-熂	𪸕
 熅	煴
-熉	𤈶
-熌	𤇄
+熈	熙
 熒	荧
-熓	𤆡
 熗	炝
-熚	𤇹
-熡	𤋏
 熰	𬉼
 熱	热
 熲	颎
 熾	炽
 燀	𬊤
 燁	烨
+燄	焰
 燈	灯
 燉	炖
+燐	磷
 燒	烧
 燖	𬊈
 燙	烫
 燜	焖
 營	营
 燦	灿
 燬	毁
 燭	烛
 燴	烩
-燶	㶶
 燻	熏
 燼	烬
 燾	焘
-爃	𫞡
-爄	𤇃
-爇	𦶟
+燿	耀
 爍	烁
 爐	炉
-爖	𤇭
+爕	燮
+爗	烨
 爛	烂
-爥	𪹳
-爧	𫞠
 爭	争
 爲	为
 爺	爷
 爾	尔
 牀	床
 牆	墙
+牋	笺
+牎	窗
+牐	闸
+牓	榜
+牕	窗
 牘	牍
-牴	牴 抵
+牠	它
+牴	抵
 牽	牵
+犂	犁
+犇	犇 奔
 犖	荦
 犛	牦
-犞	𪺭
 犢	犊
 犧	牺
 狀	状
+狥	徇
 狹	狭
 狽	狈
-猌	𪺽
+猂	悍
 猙	狰
+猨	猿
 猶	犹
 猻	狲
 獁	犸
 獃	呆
 獄	狱
 獅	狮
-獊	𪺷
+獋	嗥
 獎	奖
+獘	毙
+獧	狷
 獨	独
-獩	𤞃
 獪	狯
 獫	猃
 獮	狝
 獰	狞
-獱	㺍
 獲	获
 獵	猎
 獷	犷
 獸	兽
 獺	獭
 獻	献
 獼	猕
 玀	猡
-玁	𤞤
-珼	𫞥
+玅	妙
+珎	珍
 現	现
+琍	璃
+琖	盏
 琱	雕
+琹	琴
 琺	珐
 琿	珲
+瑇	玳
 瑋	玮
 瑒	玚
+瑠	琉
 瑣	琐
 瑤	瑶
 瑩	莹
 瑪	玛
+瑯	琅
 瑲	玱
-瑻	𪻲
-瑽	𪻐
 璉	琏
 璊	𫞩
 璕	𬍤
 璗	𬍡
-璝	𪻺
 璡	琎
+璢	琉
 璣	玑
 璦	瑷
 璫	珰
-璯	㻅
 環	环
 璵	玙
-璸	瑸
-璼	𫞨
 璽	玺
-璾	𫞦
 璿	璇
-瓄	𪻨
 瓅	𬍛
+瓈	璃
 瓊	琼
+瓌	瑰
 瓏	珑
 瓔	璎
-瓕	𤦀
 瓚	瓒
 瓛	𤩽
 甌	瓯
+甎	砖
 甕	瓮
+甖	罂
+甞	尝
 產	产
 産	产
-甦	苏
-甯	宁
+甦	苏 甦
+甯	甯 宁
+畂	亩
+畆	亩
+畊	耕
 畝	亩
 畢	毕
+畧	略
 畫	画 划
+畮	亩
 異	异
+畱	留
 畵	画
 當	当
-畼	𪽈
 疇	畴
 疊	叠
+疋	匹
+疎	疏
+疘	肛
+疿	痱
+痐	蛔
 痙	痉
 痠	酸
-痮	𪽪
+痳	淋
+痺	痹
 痾	疴
-瘂	痖
+瘉	愈
 瘋	疯
 瘍	疡
 瘓	痪
+瘖	喑
 瘞	瘗
 瘡	疮
 瘧	疟
 瘮	瘆
-瘱	𪽷
 瘲	疭
 瘺	瘘
 瘻	瘘
 療	疗
+癄	憔
+癅	瘤
 癆	痨
 癇	痫
+癈	废
 癉	瘅
-癐	𤶊
 癒	愈
 癘	疠
 癟	瘪
 癡	痴
 癢	痒
 癤	疖
 癥	症
@@ -1386,188 +1414,222 @@
 癭	瘿
 癮	瘾
 癰	痈
 癱	瘫
 癲	癫
 發	发
 皁	皂
+皐	皋
 皚	皑
-皟	𤾀
+皜	皓
 皰	疱
+皷	鼓
 皸	皲
 皺	皱
 盃	杯
+盇	盍
+盋	钵
+盌	碗
 盜	盗
 盞	盏
 盡	尽
 監	监
 盤	盘
 盧	卢
-盨	𪾔
 盪	荡
-眝	𪾣
+眎	视
 眞	真
+眡	视
 眥	眦
 眾	众
 睍	𪾢
 睏	困
 睜	睁
 睞	睐
+睠	眷
+瞇	眯
+瞖	翳
 瞘	眍
 瞜	䁖
 瞞	瞒
-瞤	𥆧
 瞭	瞭 了
-瞶	瞆
 瞼	睑
+矁	瞅
 矇	蒙
-矉	𪾸
-矑	𪾦
 矓	眬
+矙	瞰
 矚	瞩
 矯	矫
+矴	碇
+砦	寨
+砲	炮
 硃	朱
 硜	硁
 硤	硖
 硨	砗
 硯	砚
+碁	棋
 碕	埼
-碙	𥐻
 碩	硕
+碪	砧
 碭	砀
 碸	砜
 確	确
 碼	码
-碽	䂵
 磑	硙
 磚	砖
-磠	硵
+磟	碌
 磣	碜
 磧	碛
 磯	矶
 磽	硗
 磾	䃅
 礄	硚
-礆	硷
 礎	础
 礐	𬒈
-礒	𥐟
 礙	碍
 礦	矿
 礪	砺
 礫	砾
 礬	矾
-礮	𪿫
+礮	炮
 礱	砻
 祇	祇 只
-祕	秘
+祕	秘 祕
 祿	禄
 禍	祸
 禎	祯
 禕	祎
 禡	祃
 禦	御
+禩	祀
 禪	禅
 禮	礼
 禰	祢
 禱	祷
 禿	秃
 秈	籼
+秊	年
+秌	秋
+秔	粳
+秖	只
 稅	税
 稈	秆
-稏	䅉
+稉	粳
 稜	棱
 稟	禀
+稬	糯
+稭	秸
 種	种
 稱	称
+稺	稚
+稾	稿
 穀	谷
+穅	糠
 穇	䅟
+穉	稚
 穌	稣
 積	积
 穎	颖
 穠	秾
 穡	穑
 穢	秽
+穤	糯
+穨	颓
 穩	稳
 穫	获
-穭	穞
+穽	阱
+窓	窗
 窩	窝
 窪	洼
 窮	穷
 窯	窑
+窰	窑
 窵	窎
 窶	窭
 窺	窥
+窻	窗
 竄	窜
 竅	窍
 竇	窦
 竈	灶
 竊	窃
-竚	𥩟
+竚	伫
+竝	并
+竢	俟
 竪	竖
-竱	𫁟
 競	竞
 筆	笔
 筍	笋
+筞	策
+筦	筦 管
 筧	笕
-筴	䇲
+筩	筒
+筯	箸
+筴	策
 箇	个
 箋	笺
 箏	筝
+箒	帚
+箠	棰
 節	节
 範	范
 築	筑
 篋	箧
 篔	筼
-篘	𥬠
-篠	筿
+篛	箬
 篢	𬕂
 篤	笃
 篩	筛
 篳	筚
-篸	𥮾
 簀	箦
-簂	𫂆
 簍	篓
 簑	蓑
+簒	篡
 簞	箪
 簡	简
-簢	𫂃
 簣	篑
 簫	箫
+簮	簪
+簷	檐
 簹	筜
 簽	签
 簾	帘
 籃	篮
-籅	𥫣
-籋	𥬞
 籌	筹
-籔	䉤
+籐	藤
+籑	馔
 籙	箓
 籛	篯
 籜	箨
 籟	籁
 籠	笼
 籤	签
+籨	奁
 籩	笾
 籪	簖
 籬	篱
 籮	箩
 籲	吁
+粃	秕
+粇	糠 粳
+粦	磷
+粧	妆
+粰	麸
 粵	粤
+粺	稗
 糉	粽
 糝	糁
 糞	粪
 糧	粮
 糰	团
 糲	粝
 糴	籴
 糶	粜
-糹	纟
-糺	𫄙
+糺	纠
 糾	纠
 紀	纪
 紂	纣
 紃	𬘓
 約	约
 紅	红
 紆	纡
@@ -1585,76 +1647,67 @@
 紘	纮
 紙	纸
 級	级
 紛	纷
 紜	纭
 紝	纴
 紞	𬘘
-紟	𫄛
 紡	纺
-紬	䌷
+紥	扎
+紬	绸
 紮	扎
 細	细
 紱	绂
 紲	绁
 紳	绅
 紵	纻
 紹	绍
 紺	绀
 紼	绋
 紿	绐
 絀	绌
-絁	𫄟
 終	终
 絃	弦
 組	组
 絅	䌹
 絆	绊
-絍	𫟃
 絎	绗
+絏	绁
 結	结
 絕	绝
-絙	𫄠
 絛	绦
+絜	絜 洁
 絝	绔
 絞	绞
 絡	络
 絢	绚
-絥	𫄢
 給	给
-絧	𫄡
 絨	绒
 絪	𬘡
 絰	绖
 統	统
 絲	丝
 絳	绛
 絶	绝
 絹	绢
 絺	𫄨
-綀	𦈌
 綁	绑
 綃	绡
 綄	𬘫
 綆	绠
-綇	𦈋
 綈	绨
 綉	绣
-綋	𫟄
 綌	绤
 綎	𬘩
 綏	绥
-綐	䌼
 綑	捆
 經	经
 綖	𫄧
 綜	综
 綝	𬘭
-綞	缍
-綟	𫄫
 綠	绿
 綡	𫟅
 綢	绸
 綣	绻
 綧	𬘯
 綪	𬘬
 綫	线
@@ -1662,592 +1715,607 @@
 維	维
 綯	绹
 綰	绾
 綱	纲
 網	网
 綳	绷
 綴	缀
-綵	彩 䌽
+綵	彩
 綸	纶
 綹	绺
 綺	绮
 綻	绽
 綽	绰
 綾	绫
 綿	绵
 緄	绲
 緇	缁
 緊	紧
 緋	绯
-緍	𦈏
+緐	繁
 緑	绿
 緒	绪
-緓	绬
 緔	绱
 緗	缃
 緘	缄
 緙	缂
 線	线 缐
+緜	绵
 緝	缉
 緞	缎
-緟	𫟆
 締	缔
 緡	缗
 緣	缘
-緤	𫄬
+緥	褓
 緦	缌
 編	编
 緩	缓
 緬	缅
-緮	𫄭
 緯	纬
-緰	𦈕
 緱	缑
 緲	缈
 練	练
-緶	缏
-緷	𦈉
-緸	𦈑
 緹	缇
 緻	致
 緼	缊
 縈	萦
 縉	缙
 縊	缢
 縋	缒
-縍	𫄰
-縎	𦈔
 縐	绉
 縑	缣
 縕	缊
 縗	缞
+縚	绦
 縛	缚
 縝	缜
 縞	缟
 縟	缛
 縣	县
 縧	绦
 縫	缝
-縬	𦈚
 縭	缡
 縮	缩
 縯	𬙂
-縰	𫄳
 縱	纵
 縲	缧
-縳	䌸
 縴	纤
 縵	缦
 縶	絷
 縷	缕
-縸	𫄲
 縹	缥
-縺	𦈐
 總	总
 績	绩
-繂	𫄴
 繃	绷
 繅	缫
 繆	缪
-繈	𫄶
-繏	𦈝
-繐	𰬸
 繒	缯
-繓	𦈛
 織	织
 繕	缮
+繖	伞
+繙	翻
 繚	缭
 繞	绕
-繟	𦈎
 繡	绣
-繢	缋
-繨	𫄤
+繦	襁
 繩	绳
 繪	绘
 繫	系
-繬	𫄱
 繭	茧
 繮	缰
 繯	缳
 繰	缲
 繳	缴
 繶	𫄷
-繷	𫄣
-繸	䍁
 繹	绎
 繻	𦈡
 繼	继
 繽	缤
 繾	缱
-繿	䍀
 纁	𫄸
 纆	𬙊
-纇	颣
 纈	缬
 纊	纩
 續	续
 纍	累
 纏	缠
 纓	缨
 纔	才
 纕	𬙋
 纖	纤
-纗	𫄹
 纘	缵
-纚	𫄥
 纜	缆
 缽	钵
+缾	瓶
 罃	䓨
+罇	樽
 罈	坛
+罋	瓮
 罌	罂
 罎	坛
 罰	罚
 罵	骂
 罷	罢
+罸	罚
 羅	罗
 羆	罴
 羈	羁
 羋	芈
+羗	羌
+羢	绒
 羣	群
 羥	羟
 羨	羡
 義	义
-羵	𫅗
+羴	膻
 羶	膻
+翄	翅
 習	习
 翫	玩
 翬	翚
 翹	翘
+翺	翱
 翽	翙
+耑	耑 专
+耡	锄
 耬	耧
 耮	耢
 聖	圣
 聞	闻
 聯	联
 聰	聪
 聲	声
 聳	耸
 聵	聩
 聶	聂
 職	职
 聹	聍
-聻	𫆏
 聽	听
 聾	聋
 肅	肃
+肎	肯
+肐	胳
+肧	胚
+胷	胸
+脃	脆
 脅	胁
+脇	胁
 脈	脉
+脗	吻
 脛	胫
 脣	唇
-脥	𣍰
-脩	修
+脩	修 脩
 脫	脱
 脹	胀
 腎	肾
 腖	胨
 腡	脶
 腦	脑
-腪	𣍯
 腫	肿
 腳	脚
 腸	肠
 膃	腽
+膓	肠
 膕	腘
 膚	肤
 膞	䏝
 膠	胶
 膢	𦝼
 膩	腻
-膹	𪱥
 膽	胆
 膾	脍
 膿	脓
+臈	腊
 臉	脸
+臋	臀
 臍	脐
 臏	膑
-臗	𣎑
+臕	膘
 臘	腊
+臙	胭
 臚	胪
+臝	裸
 臟	脏
 臠	脔
 臢	臜
 臥	卧
 臨	临
+臯	皋
 臺	台
 與	与
 興	兴
 舉	举
 舊	旧
+舖	铺
 舘	馆
+舩	船
 艙	舱
-艣	𫇛
+艢	樯
+艣	橹
 艤	舣
 艦	舰
+艪	橹
 艫	舻
 艱	艰
 艷	艳
+艸	草
+芲	花
 芻	刍
 苧	苎
+茘	荔
 茲	兹
 荊	荆
+荍	荞
+荳	豆
 莊	庄
 莖	茎
 莢	荚
 莧	苋
-菕	𰰨
+菉	菉 绿
+菑	灾
+菓	果
 華	华
 菴	庵
 菸	烟
 萇	苌
 萊	莱
 萬	万
-萴	荝
+萲	萱
 萵	莴
 葉	叶
 葒	荭
-葝	𫈎
+葠	参
 葤	荮
 葦	苇
 葯	药
 葷	荤
 蒍	𫇭
-蒐	搜
+蒐	搜 蒐
 蒓	莼
 蒔	莳
-蒕	蒀
 蒞	莅
-蒭	𫇴
 蒼	苍
 蓀	荪
 蓆	席
 蓋	盖
-蓧	𦰏
+蓡	参
 蓮	莲
 蓯	苁
 蓴	莼
 蓽	荜
 蔄	𬜬
+蔆	菱
 蔔	卜
+蔕	蒂
 蔘	参
 蔞	蒌
 蔣	蒋
 蔥	葱
 蔦	茑
 蔭	荫
-蔯	𫈟
+蔴	麻
+蔾	藜
 蔿	𫇭
 蕁	荨
 蕆	蒇
+蕋	蕊
 蕎	荞
 蕒	荬
 蕓	芸
 蕕	莸
 蕘	荛
-蕝	𫈵
+蕚	萼
 蕢	蒉
 蕩	荡
 蕪	芜
 蕭	萧
-蕳	𫈉
 蕷	蓣
-蕽	𫇽
+蕿	萱
 薀	蕰
-薆	𫉁
 薈	荟
 薊	蓟
 薌	芗
 薑	姜
 薔	蔷
 薘	荙
+薙	剃
 薟	莶
 薦	荐
 薩	萨
-薳	䓕
 薴	苧
-薵	䓓
 薹	苔 薹
 薺	荠
 藉	藉 借
 藍	蓝
 藎	荩
 藝	艺
 藥	药
 藪	薮
 藭	䓖
 藴	蕴
 藶	苈
-藷	𫉄
+藷	薯
 藹	蔼
 藺	蔺
+藼	萱
 蘀	萚
+蘂	蕊
 蘄	蕲
 蘆	芦
 蘇	苏
 蘊	蕴
 蘋	苹 𬞟
+蘐	萱
+蘓	苏
 蘚	藓
 蘞	蔹
-蘟	𦻕
 蘢	茏
+蘤	花
 蘭	兰
 蘺	蓠
 蘿	萝
-虆	蔂
 虉	𬟁
 處	处
+虖	呼
 虛	虚
 虜	虏
 號	号
 虧	亏
 虯	虬
+虵	蛇
+蚘	蛔
+蛕	蛔
 蛺	蛱
 蛻	蜕
 蜆	蚬
+蜋	螂
+蜖	蛔
+蜨	蝶
+蜺	霓
 蝀	𬟽
 蝕	蚀
 蝟	猬
+蝡	蠕
 蝦	虾
 蝨	虱
+蝯	猿
+蝱	虻
 蝸	蜗
 螄	蛳
+螎	融
 螞	蚂
+螡	蚊
 螢	萤
 螮	䗖
 螻	蝼
-螿	螀
-蟂	𫋇
+蟁	蚊
 蟄	蛰
+蟇	蟆
 蟈	蝈
 蟎	螨
-蟘	𫋌
-蟜	𫊸
 蟣	虮
 蟬	蝉
 蟯	蛲
 蟲	虫
-蟳	𫊻
 蟶	蛏
 蟻	蚁
-蠀	𧏗
-蠁	蚃
 蠅	蝇
 蠆	虿
 蠍	蝎
+蠏	蟹
 蠐	蛴
 蠑	蝾
+蠒	茧
 蠔	蚝
-蠙	𧏖
 蠟	蜡
 蠣	蛎
-蠦	𫊮
 蠨	蟏
+蠭	蜂
 蠱	蛊
 蠶	蚕
 蠻	蛮
-蠾	𧑏
+衂	衄
 衆	众
+衇	脉
 衊	蔑
 術	术
 衕	同
+衖	弄
+衘	衔
 衚	胡
 衛	卫
 衝	冲
-衹	衹 只
+衹	只
+衺	邪
 袞	衮
+袟	帙
+袠	帙
+袴	裤
+袵	衽
+袷	夹 袷
 裊	袅
+裌	夹
 裏	里
 補	补
 裝	装
+裠	裙
 裡	里
 製	制
 複	复
 褌	裈
 褘	袆
+褭	袅
 褲	裤
 褳	裢
 褸	褛
 褻	亵
 襀	𫌀
+襃	褒
 襇	裥
 襉	裥
+襍	杂
 襏	袯
-襓	𫋹
 襖	袄
-襗	𫋷
-襘	𫋻
 襝	裣
 襠	裆
+襢	袒
 襤	褴
 襪	袜
-襬	摆 䙓
+襬	摆
 襯	衬
-襰	𧝝
 襲	袭
 襴	襕
-襵	𫌇
 覆	覆 复
+覇	霸
 覈	核
+覊	羁
 見	见
 覎	觃
 規	规
 覓	觅
+覔	觅
 視	视
 覘	觇
-覛	𫌪
+覜	眺
 覡	觋
-覥	觍
 覦	觎
+覩	睹
 親	亲
 覬	觊
 覯	觏
 覲	觐
 覷	觑
-覹	𫌭
 覺	觉
-覼	𫌨
 覽	览
 覿	觌
 觀	观
+觔	斤
+觕	粗
+觝	抵
 觴	觞
 觶	觯
 觸	触
-訁	讠
 訂	订
 訃	讣
 計	计
 訊	讯
 訌	讧
 討	讨
 訏	𬣙
 訐	讦
-訑	𫍙
 訒	讱
 訓	训
 訕	讪
 訖	讫
-託	托 讬
+託	托
 記	记
 訛	讹
-訜	𫍛
 訝	讶
-訞	𫍚
 訟	讼
-訢	䜣
+訢	䜣 欣
 訣	诀
 訥	讷
-訨	𫟞
 訩	讻
 訪	访
 設	设
 許	许
 訴	诉
 訶	诃
 診	诊
 註	注
 証	证
-詀	𧮪
 詁	诂
 詆	诋
-詊	𫟟
 詎	讵
 詐	诈
-詑	𫍡
 詒	诒
-詓	𫍜
 詔	诏
 評	评
 詖	诐
 詗	诇
 詘	诎
 詛	诅
 詝	𬣞
 詞	词
 詠	咏
 詡	诩
 詢	询
 詣	诣
 試	试
+詧	察
 詩	诗
 詪	𬣳
 詫	诧
 詬	诟
 詭	诡
 詮	诠
 詰	诘
 話	话
 該	该
 詳	详
 詵	诜
+詶	酬
 詷	𫍣
 詼	诙
 詿	诖
-誂	𫍥
 誄	诔
 誅	诛
 誆	诓
 誇	夸
-誋	𫍪
 誌	志
 認	认
 誑	诳
-誒	诶
 誕	诞
+誖	悖
 誘	诱
 誚	诮
 語	语
 誠	诚
 誡	诫
 誣	诬
 誤	误
 誥	诰
 誦	诵
 誨	诲
 說	说
-誫	𫍨
 説	说
 誰	谁
 課	课
-誳	𫍮
-誴	𫟡
 誶	谇
-誷	𫍬
 誹	诽
-誺	𫍧
 誼	谊
 誾	訚
 調	调
 諂	谄
 諄	谆
 談	谈
 諉	诿
 請	请
 諍	诤
 諏	诹
+諐	愆
 諑	诼
 諒	谅
 諓	𬣡
 論	论
 諗	谂
 諛	谀
 諜	谍
 諝	谞
 諞	谝
 諟	𬤊
+諠	喧
 諡	谥
 諢	诨
-諣	𫍩
 諤	谔
-諥	𫍳
 諦	谛
 諧	谐
-諫	谏 𫍝
+諫	谏
 諭	谕
-諮	咨 谘
-諯	𫍱
-諰	𫍰
+諮	咨
 諱	讳
 諲	𬤇
 諳	谙
 諴	𫍯
 諶	谌
 諷	讽
 諸	诸
@@ -2255,750 +2323,694 @@
 諼	谖
 諾	诺
 謀	谋
 謁	谒
 謂	谓
 謄	誊
 謅	诌
-謆	𫍸
-謉	𫍷
 謊	谎
+謌	歌
 謎	谜
 謏	𫍲
 謐	谧
 謔	谑
 謖	谡
 謗	谤
 謙	谦
 謚	谥
 講	讲
 謝	谢
+謟	谄
 謠	谣
 謡	谣
 謨	谟
+謩	谟
 謫	谪
 謬	谬
 謭	谫
-謯	𫍹
-謱	𫍴
 謳	讴
-謸	𫍵
 謹	谨
+謼	呼
 謾	谩
 譁	哗
-譂	𫟠
-譅	𰶎
-譆	𫍻
+譆	嘻
 證	证
-譊	𫍢
+譌	讹
 譎	谲
 譏	讥
-譑	𫍤
 譓	𬤝
+譔	撰
 譖	谮
 識	识
 譙	谯
 譚	谭
 譜	谱
 譞	𫍽
 譟	噪
-譨	𫍦
 譫	谵
 譭	毁
 譯	译
 議	议
 譴	谴
 護	护
-譸	诪
 譽	誉
-譾	谫 𫍿
+譾	谫
 讀	读
-讅	谉
+讁	谪
 變	变
 讋	詟
-讌	䜩
-讎	雠
+讌	宴
+讎	仇 雠
+讐	仇 雠
 讒	谗
 讓	让
 讕	谰
 讖	谶
+讙	欢
 讚	赞
 讜	谠
 讞	谳
+谿	溪 谿
 豈	岂
 豎	竖
 豐	丰
+豓	艳
 豔	艳
 豬	猪
-豵	𫎆
 豶	豮
+貍	狸
 貓	猫
-貗	𫎌
 貙	䝙
+貛	獾
 貝	贝
 貞	贞
-貟	贠
 負	负
 財	财
 貢	贡
 貧	贫
 貨	货
 販	贩
 貪	贪
 貫	贯
 責	责
 貯	贮
 貰	贳
-貲	赀
+貲	赀 资
 貳	贰
 貴	贵
 貶	贬
-買	买 𧹒
+買	买
 貸	贷
 貺	贶
 費	费
 貼	贴
 貽	贻
 貿	贸
 賀	贺
 賁	贲
 賂	赂
 賃	赁
 賄	贿
 賅	赅
 資	资
 賈	贾
+賉	恤
 賊	贼
 賑	赈
 賒	赊
 賓	宾
 賕	赇
 賙	赒
 賚	赉
+賛	赞
 賜	赐
-賝	𫎩
 賞	赏
-賟	𧹖
 賠	赔
 賡	赓
 賢	贤
 賣	卖
 賤	贱
 賦	赋
 賧	赕
 質	质
 賫	赍
 賬	账
 賭	赌
-賰	䞐
 賴	赖
 賵	赗
+賷	赍
+賸	剩
 賺	赚
 賻	赙
 購	购
 賽	赛
 賾	赜
-贃	𧹗
 贄	贽
 贅	赘
 贇	赟
 贈	赠
-贉	𫎫
 贊	赞
 贋	赝
 贍	赡
 贏	赢
 贐	赆
-贑	𫎬
+贑	赣
 贓	赃
 贔	赑
 贖	赎
 贗	赝
-贚	𫎦
 贛	赣
 贜	赃
 赬	赪
+趂	趁
 趕	赶
 趙	赵
 趨	趋
 趲	趱
 跡	迹
+跥	跺
+跴	踩
+跼	局
+踁	胫
 踐	践
+踫	碰
 踰	逾
 踴	踊
 蹌	跄
-蹔	𫏐
+蹏	蹄
+蹔	暂
 蹕	跸
 蹟	迹
 蹠	跖
 蹣	蹒
 蹤	踪
-蹳	𫏆
+蹧	糟
+蹵	蹴
 蹺	跷
-蹻	𫏋
+蹻	跷
 躂	跶
 躉	趸
 躊	踌
 躋	跻
 躍	跃
-躎	䟢
 躑	踯
 躒	跞
 躓	踬
 躕	蹰
-躘	𨀁
 躚	跹
-躝	𨅬
 躡	蹑
 躥	蹿
 躦	躜
 躪	躏
+躭	耽
+躳	躬
+躶	裸
 軀	躯
-軉	𨉗
 車	车
 軋	轧
 軌	轨
 軍	军
 軏	𫐄
 軑	轪
 軒	轩
 軔	轫
-軕	𫐅
-軗	𨐅
 軛	轭
-軜	𫐇
 軝	𬨂
 軟	软
 軤	轷
-軨	𫐉
 軫	轸
-軬	𫐊
 軲	轱
-軷	𫐈
 軸	轴
 軹	轵
 軺	轺
 軻	轲
 軼	轶
 軾	轼
-軿	𫐌
 較	较
 輄	𨐈
 輅	辂
 輇	辁
 輈	辀
 載	载
 輊	轾
 輋	𪨶
 輒	辄
 輓	挽
 輔	辅
 輕	轻
-輖	𫐏
 輗	𫐐
+輙	辄
 輛	辆
 輜	辎
 輝	辉
 輞	辋
 輟	辍
-輢	𫐎
 輥	辊
 輦	辇
-輨	𫐑
 輩	辈
 輪	轮
 輬	辌
+輭	软
 輮	𫐓
 輯	辑
 輳	辏
 輶	𬨎
-輷	𫐒
 輸	输
 輻	辐
 輼	辒
 輾	辗
 輿	舆
 轀	辒
 轂	毂
 轄	辖
 轅	辕
 轆	辘
-轇	𫐖
 轉	转
-轊	𫐕
 轍	辙
 轎	轿
-轐	𫐗
 轔	辚
-轗	𫐘
 轟	轰
-轠	𫐙
 轡	辔
 轢	轹
-轣	𫐆
 轤	轳
+辠	罪
+辢	辣
+辤	辞
 辦	办
 辭	辞
 辮	辫
 辯	辩
 農	农
+辳	农
 迴	回
-逕	迳
+迺	迺 乃
+迻	移
+逈	迥
+逕	径 迳
 這	这
 連	连
+逥	回
+逩	奔
 週	周
 進	进
+遉	侦
 遊	游
 運	运
 過	过
 達	达
 違	违
 遙	遥
 遜	逊
 遞	递
 遠	远
 遡	溯
 適	适
-遱	𫐷
+遯	遁
 遲	迟
+遶	绕
 遷	迁
 選	选
 遺	遗
 遼	辽
 邁	迈
 還	还
 邇	迩
 邊	边
 邏	逻
 邐	逦
+邨	邨 村
 郟	郏
 郵	邮
 鄆	郓
 鄉	乡
 鄒	邹
 鄔	邬
 鄖	郧
-鄟	𫑘
 鄧	邓
 鄩	𬩽
 鄭	郑
 鄰	邻
 鄲	郸
 鄳	𫑡
 鄴	邺
 鄶	郐
 鄺	邝
 酇	酂
 酈	郦
+酖	鸩
+酧	酬
 醃	腌
+醆	盏
+醕	醇
 醖	酝
 醜	丑
 醞	酝
-醟	蒏
 醣	糖
 醫	医
 醬	酱
 醱	酦
 醲	𬪩
-醶	𫑷
+醻	酬
+醼	宴
 釀	酿
 釁	衅
 釃	酾
 釅	酽
 釋	释
-釐	厘
-釒	钅
+釐	厘 釐
 釓	钆
 釔	钇
 釕	钌
 釗	钊
 釘	钉
 釙	钋
-釚	𫟲
 針	针
-釟	𫓥
 釣	钓
 釤	钐
 釦	扣
 釧	钏
-釨	𫓦
 釩	钒
-釲	𫟳
-釳	𨰿
+釬	焊
 釴	𬬩
 釵	钗
 釷	钍
 釹	钕
 釺	钎
-釾	䥺
 釿	𬬱
 鈀	钯
 鈁	钫
 鈃	钘
 鈄	钭
 鈅	钥
-鈆	𫓪
+鈆	铅
 鈇	𫓧
 鈈	钚
 鈉	钠
-鈋	𨱂
 鈍	钝
 鈎	钩
 鈐	钤
 鈑	钣
-鈒	钑
 鈔	钞
 鈕	钮
-鈖	𫟴
-鈗	𫟵
-鈛	𫓨
 鈞	钧
-鈠	𨱁
 鈡	钟
 鈣	钙
 鈥	钬
 鈦	钛
 鈧	钪
 鈮	铌
-鈯	𨱄
 鈰	铈
-鈲	𨱃
-鈳	钶
 鈴	铃
 鈷	钴
 鈸	钹
 鈹	铍
 鈺	钰
-鈽	钸
 鈾	铀
 鈿	钿
 鉀	钾
-鉁	𨱅
 鉅	巨 钜
 鉆	钻
 鉈	铊
 鉉	铉
 鉊	𬬿
-鉋	铇
+鉋	刨
 鉍	铋
+鉏	锄
 鉑	铂
-鉔	𫓬
 鉕	钷
 鉗	钳
 鉚	铆
 鉛	铅
-鉝	𫟷
 鉞	钺
-鉠	𫓭
 鉢	钵
 鉤	钩
 鉥	𬬸
 鉦	钲
 鉧	𬭁
 鉬	钼
 鉭	钽
 鉮	𬬹
 鉳	锫
 鉶	铏
 鉷	𫟹
 鉸	铰
 鉺	铒
 鉻	铬
-鉽	𫟸
-鉾	𫓴
 鉿	铪
 銀	银
-銁	𫓲
-銂	𫟻
 銃	铳
 銅	铜
 銈	𫓯
-銊	𫓰
 銍	铚
-銏	𫟶
 銑	铣
 銓	铨
 銖	铢
 銘	铭
 銚	铫
-銛	铦
 銜	衔
 銠	铑
 銣	铷
 銥	铱
 銦	铟
 銨	铵
 銩	铥
 銪	铕
 銫	铯
 銬	铐
 銱	铞
+銲	焊
 銳	锐
 銶	𨱇
 銷	销
 銹	锈
 銻	锑
 銼	锉
 鋁	铝
-鋂	𰾄
 鋃	锒
 鋅	锌
 鋇	钡
-鋉	𨱈
 鋌	铤
 鋏	铗
 鋐	𬭎
 鋒	锋
 鋗	𫓶
 鋙	铻
 鋝	锊
 鋟	锓
-鋠	𫓵
 鋣	铘
 鋤	锄
 鋥	锃
 鋦	锔
 鋨	锇
-鋩	铓
 鋪	铺
 鋭	锐
 鋮	铖
 鋯	锆
 鋰	锂
 鋱	铽
 鋶	锍
 鋸	锯
 鋹	𬬮
 鋼	钢
 錀	𬬭
 錁	锞
-錂	𨱋
 錄	录
 錆	锖
 錇	锫
 錈	锩
-錏	铔
 錐	锥
 錒	锕
 錕	锟
 錘	锤
 錙	锱
 錚	铮
 錛	锛
-錜	𫓻
-錝	𫓽
 錞	𬭚
 錟	锬
 錠	锭
 錡	锜
 錢	钱
 錤	𫓹
-錥	𫓾
 錦	锦
 錨	锚
-錩	锠
 錫	锡
 錮	锢
 錯	错
 録	录
 錳	锰
 錶	表
 錸	铼
 錼	镎
-錽	𫓸
 鍀	锝
 鍁	锨
 鍃	锪
-鍄	𨱉
 鍅	钫
 鍆	钔
 鍇	锴
 鍈	锳
-鍉	𫔂
-鍊	炼 链 𫔀
+鍊	炼 链
 鍋	锅
 鍍	镀
-鍒	𫔄
 鍔	锷
 鍘	铡
 鍚	钖
 鍛	锻
 鍠	锽
 鍤	锸
 鍥	锲
 鍩	锘
+鍫	锹
 鍬	锹
 鍭	𬭤
-鍮	𨱎
 鍰	锾
+鍳	鉴
 鍵	键
 鍶	锶
 鍺	锗
 鍼	针
 鍾	钟 锺
 鎂	镁
 鎄	锿
 鎇	镅
-鎈	𫟿
 鎊	镑
 鎌	镰
-鎍	𫔅
 鎓	𬭩
 鎔	镕
 鎖	锁
+鎗	枪
 鎘	镉
-鎙	𫔈
 鎚	锤
 鎛	镈
 鎝	𨱏
-鎞	𫔇
 鎡	镃
 鎢	钨
 鎣	蓥
 鎦	镏
 鎧	铠
 鎩	铩
 鎪	锼
 鎬	镐
 鎭	镇
 鎮	镇
-鎯	𨱍
 鎰	镒
 鎲	镋
 鎳	镍
 鎵	镓
-鎶	鿔
-鎷	𨰾
 鎸	镌
+鎻	锁
 鎿	镎
 鏃	镞
-鏆	𨱌
-鏇	旋 镟
+鏇	旋
 鏈	链
-鏉	𨱒
 鏌	镆
-鏍	镙
 鏏	𬭬
 鏐	镠
 鏑	镝
 鏗	铿
 鏘	锵
-鏚	𬭭
 鏜	镗
 鏝	镘
 鏞	镛
 鏟	铲
 鏡	镜
 鏢	镖
 鏤	镂
-鏥	𫔊
-鏦	𫓩
 鏨	錾
 鏰	镚
 鏵	铧
 鏷	镤
 鏹	镪
 鏺	䥽
 鏻	𬭸
 鏽	锈
-鏾	𫔌
 鐃	铙
 鐄	𨱑
 鐇	𫔍
-鐈	𫓱
 鐋	铴
 鐍	𫔎
-鐎	𨱓
 鐏	𨱔
 鐐	镣
 鐒	铹
 鐓	镦
 鐔	镡
 鐘	钟
 鐙	镫
 鐝	镢
 鐠	镨
-鐥	䦅
 鐦	锎
 鐧	锏
 鐨	镄
 鐩	𬭼
-鐪	𫓺
 鐫	镌
 鐮	镰
 鐯	䦃
 鐲	镯
 鐳	镭
 鐵	铁
 鐶	镮
 鐸	铎
 鐺	铛
-鐼	𫔁
 鐽	𫟼
 鐿	镱
-鑀	𰾭
 鑄	铸
-鑉	𫠁
 鑊	镬
 鑌	镔
 鑑	鉴
 鑒	鉴
 鑔	镲
 鑕	锧
+鑚	钻
+鑛	矿
 鑞	镴
 鑠	铄
 鑣	镳
+鑤	刨
 鑥	镥
-鑪	𬬻
+鑪	𬬻 炉
 鑭	镧
 鑰	钥
 鑱	镵
 鑲	镶
-鑴	𫔔
+鑵	罐
 鑷	镊
 鑹	镩
 鑼	锣
 鑽	钻
 鑾	銮
 鑿	凿
-钁	镢 䦆
+钁	镢
 钂	镋
 長	长
 門	门
 閂	闩
 閃	闪
 閆	闫
-閈	闬
 閉	闭
-開	开 𫔭
+開	开
 閌	闶
-閍	𨸂
 閎	闳
 閏	闰
-閐	𨸃
 閑	闲
-閒	闲 𫔮
+閒	闲
 間	间
 閔	闵
-閗	𫔯
 閘	闸
-閝	𫠂
-閞	𫔰
+閙	闹
 閡	阂
 閣	阁
-閤	合
+閤	合 阁
 閥	阀
+閧	哄
 閨	闺
 閩	闽
 閫	阃
 閬	阆
 閭	闾
 閱	阅
 閲	阅
-閵	𫔴
 閶	阊
 閹	阉
 閻	阎
 閼	阏
 閽	阍
 閾	阈
 閿	阌
@@ -3014,92 +3026,102 @@
 闐	阗
 闑	𫔶
 闒	阘
 闓	闿
 闔	阖
 闕	阙
 闖	闯
+闚	窥
 關	关
 闞	阚
-闠	阓
 闡	阐
 闢	辟
-闤	阛
 闥	闼
+阨	厄
 阪	阪 坂
+阬	坑
+阯	址
+陗	峭
 陘	陉
 陝	陕
-陞	升
+陞	陞 升
 陣	阵
 陰	阴
 陳	陈
 陸	陆
+陻	堙
 陽	阳
+陿	狭
+隂	阴
+隄	堤
 隉	陧
 隊	队
 階	阶
 隑	𬮿
 隕	陨
+隖	坞
 際	际
+隣	邻
 隤	𬯎
 隨	随
 險	险
 隮	𬯀
-隯	陦
 隱	隐
 隴	陇
+隷	隶
 隸	隶
 隻	只
 雋	隽
 雖	虽
 雙	双
 雛	雏
 雜	杂
+雝	雍
 雞	鸡
 離	离
 難	难
+雰	氛
 雲	云
 電	电
 霑	沾
-霢	霡
-霣	𫕥
 霧	雾
-霼	𪵣
 霽	霁
 靂	雳
 靄	霭
 靆	叇
 靈	灵
 靉	叆
 靚	靓
 靜	静
-靝	靔
-靦	腼 䩄
-靧	𫖃
+靦	腼
 靨	靥
+靭	韧
+靱	韧
+鞌	鞍
 鞏	巩
 鞝	绱
 鞦	秋
+鞵	鞋
 鞽	鞒
-鞾	𫖇
+鞾	靴
 韁	缰
 韃	鞑
 韆	千
+韈	袜
 韉	鞯
 韋	韦
 韌	韧
 韍	韨
 韓	韩
 韙	韪
-韚	𫠅
-韛	𫖔
 韜	韬
-韝	鞲 𫖕
+韝	鞲
 韞	韫
-韠	𫖒
+韤	袜
+韮	韭
 韻	韵
 響	响
 頁	页
 頂	顶
 頃	顷
 項	项
 順	顺
@@ -3114,297 +3136,267 @@
 頑	顽
 頒	颁
 頓	顿
 頔	𬱖
 頗	颇
 領	领
 頜	颌
+頟	额
 頠	𬱟
 頡	颉
 頤	颐
 頦	颏
-頫	𫖯
+頫	𫖯 俯
 頭	头
-頮	颒
 頰	颊
 頲	颋
-頴	颕
+頴	颖
 頵	𫖳
 頷	颔
 頸	颈
 頹	颓
 頻	频
+頼	赖
 頽	颓
-顂	𩓋
-顃	𩖖
-顅	𫖶
 顆	颗
+顇	悴
+顋	腮
 題	题
 額	额
 顎	颚
 顏	颜
 顒	颙
 顓	颛
 顔	颜
 顗	𫖮
-願	愿 𫖸
+願	愿
 顙	颡
 顛	颠
 類	类
 顢	颟
-顣	𫖹
 顥	颢
+顦	憔
 顧	顾
 顫	颤
 顬	颥
 顯	显
 顰	颦
 顱	颅
 顳	颞
 顴	颧
 風	风
 颭	飐
 颮	飑
 颯	飒
-颰	𩙥
 颱	台
 颳	刮
 颶	飓
-颷	𩙪
 颸	飔
-颺	飏
-颻	飖
+颺	飏 扬
 颼	飕
-颾	𩙫
+颿	帆
 飀	飗
+飃	飘
 飄	飘
 飆	飙
-飈	飚
-飋	𫗋
 飛	飞
-飠	饣
+飜	翻
 飢	饥
-飣	饤
-飥	饦
-飦	𫗞
+飤	饲
 飩	饨
 飪	饪
 飫	饫
 飭	饬
 飯	饭
 飱	飧
 飲	饮
 飴	饴
-飵	𫗢
-飶	𫗣
 飼	饲
 飽	饱
 飾	饰
 飿	饳
+餁	饪
 餃	饺
 餄	饸
 餅	饼
 餈	糍
 餉	饷
 養	养
 餌	饵
 餎	饹
 餏	饻
 餑	饽
 餒	馁
 餓	饿
-餔	𫗦
-餕	馂
-餖	饾
 餗	𫗧
-餘	余 馀
+餘	余
 餚	肴
 餛	馄
 餜	馃
 餞	饯
 餡	馅
-餦	𫗠
-餧	𫗪
+餧	喂
 館	馆
-餪	𫗬
-餫	𫗥
-餬	糊 𫗫
-餭	𫗮
-餱	糇 𫗯
+餬	糊
+餱	糇
 餳	饧
-餵	喂 𫗭
+餵	喂
 餶	馉
 餷	馇
-餸	𩠌
-餺	馎
+餹	糖
+餻	糕
 餼	饩
+餽	馈
 餾	馏
 餿	馊
 饁	馌
 饃	馍
 饅	馒
 饈	馐
 饉	馑
 饊	馓
 饋	馈
 饌	馔
+饍	膳
 饑	饥
 饒	饶
 饗	飨
 饘	𫗴
 饜	餍
+饝	馍
 饞	馋
-饟	𫗵
-饠	𫗩
+饟	饷
 饢	馕
 馬	马
 馭	驭
 馮	冯
-馯	𫘛
 馱	驮
 馳	驰
 馴	驯
 馹	驲
 馼	𫘜
 駁	驳
 駃	𫘝
+駈	驱
 駉	𬳶
-駊	𫘟
-駎	𩧨
 駐	驻
 駑	驽
 駒	驹
 駓	𬳵
 駔	驵
 駕	驾
 駘	骀
 駙	驸
-駚	𩧫
 駛	驶
 駝	驼
-駞	𫘞
+駞	驼
 駟	驷
 駡	骂
 駢	骈
-駤	𫘠
-駧	𩧲
-駩	𩧴
 駪	𬳽
-駫	𫘡
 駭	骇
+駮	驳
 駰	骃
 駱	骆
-駶	𩧺
 駸	骎
-駻	𫘣
 駼	𬳿
 駿	骏
 騁	骋
 騂	骍
-騃	𫘤
 騄	𫘧
 騅	骓
-騉	𫘥
 騊	𫘦
-騌	骔
+騌	鬃
 騍	骒
 騎	骑
 騏	骐
+騐	验
 騑	𬴂
-騔	𩨀
 騖	骛
 騙	骗
-騚	𩨊
-騜	𫘩
-騝	𩨃
 騞	𬴃
-騟	𩨈
 騠	𫘨
+騣	鬃
 騤	骙
-騧	䯄
-騪	𩨄
 騫	骞
 騭	骘
 騮	骝
 騰	腾
 騱	𫘬
-騴	𫘫
 騵	𫘪
 騶	驺
 騷	骚
 騸	骟
-騻	𫘭
-騼	𫠋
 騾	骡
 驀	蓦
 驁	骜
 驂	骖
 驃	骠
-驄	骢 𩨂
+驄	骢
 驅	驱
 驊	骅
-驋	𩧯
 驌	骕
 驍	骁
 驎	𬴊
 驏	骣
-驓	𫘯
 驕	骄
 驗	验
-驙	𫘰
+驘	骡
 驚	惊
 驛	驿
 驟	骤
 驢	驴
 驤	骧
 驥	骥
 驦	骦
-驨	𫘱
+驩	欢
 驪	骊
 驫	骉
 骯	肮
+骽	腿
+骾	鲠
+髈	膀
 髏	髅
 髒	脏
 體	体
 髕	髌
 髖	髋
+髣	仿
+髥	髯
 髮	发
+髴	佛
+鬀	剃
 鬆	松
+鬉	鬃
 鬍	胡
-鬖	𩭹
 鬚	须
-鬠	𫘽
 鬢	鬓
 鬥	斗
+鬦	斗
 鬧	闹
 鬨	哄
 鬩	阋
+鬪	斗
+鬭	斗
 鬮	阄
+鬰	郁
 鬱	郁
 鬹	鬶
 魎	魉
 魘	魇
 魚	鱼
 魛	鱽
-魟	𫚉
 魢	鱾
-魥	𩽹
-魦	𫚌
 魨	鲀
 魯	鲁
 魴	鲂
-魵	𫚍
 魷	鱿
-魺	鲄
-魽	𫠐
 鮀	𬶍
 鮁	鲅
 鮃	鲆
-鮄	𫚒
-鮅	𫚑
 鮆	𫚖
 鮈	𬶋
 鮊	鲌
 鮋	鲉
 鮍	鲏
 鮎	鲇
 鮐	鲐
@@ -3415,307 +3407,247 @@
 鮜	鲘
 鮝	鲞
 鮞	鲕
 鮟	𩽾
 鮠	𬶏
 鮡	𬶐
 鮣	䲟
-鮤	𫚓
 鮦	鲖
 鮪	鲔
 鮫	鲛
 鮭	鲑
 鮮	鲜
-鮯	𫚗
-鮰	𫚔
-鮳	鲓
-鮵	𫚛
 鮶	鲪
 鮸	𩾃
 鮺	鲝
-鮿	𫚚
 鯀	鲧
 鯁	鲠
-鯄	𩾁
-鯆	𫚙
 鯇	鲩
 鯉	鲤
 鯊	鲨
 鯒	鲬
 鯔	鲻
 鯕	鲯
 鯖	鲭
 鯗	鲞
 鯛	鲷
 鯝	鲴
-鯞	𫚡
 鯡	鲱
 鯢	鲵
 鯤	鲲
 鯧	鲳
 鯨	鲸
 鯪	鲮
 鯫	鲰
-鯬	𫚞
-鯰	鲶
-鯱	𩾇
 鯴	鲺
-鯶	𩽼
 鯷	鳀
 鯻	𬶟
 鯽	鲫
-鯾	𫚣
 鯿	鳊
 鰁	鳈
 鰂	鲗
 鰃	鳂
 鰆	䲠
 鰈	鲽
 鰉	鳇
 鰊	𬶠
-鰋	𫚢
-鰌	䲡
+鰌	鳅
 鰍	鳅
 鰏	鲾
 鰐	鳄
-鰑	𫚊
-鰒	鳆
 鰓	鳃
-鰕	𫚥
 鰛	鳁
 鰜	鳒
 鰟	鳑
-鰠	鳋
 鰣	鲥
 鰤	𫚕
 鰥	鳏
-鰦	𫚤
 鰧	䲢
 鰨	鳎
 鰩	鳐
-鰫	𫚦
 鰭	鳍
 鰮	鳁
 鰱	鲢
 鰲	鳌
 鰳	鳓
 鰵	鳘
 鰶	𬶭
 鰷	鲦
 鰹	鲣
 鰺	鲹
 鰻	鳗
 鰼	鳛
-鰽	𫚧
 鰾	鳔
 鱀	𬶨
 鱂	鳉
-鱄	𫚋
 鱅	鳙
-鱆	𫠒
 鱇	𩾌
 鱈	鳕
 鱉	鳖
-鱊	𫚪
 鱒	鳟
+鱓	鳝
 鱔	鳝
 鱖	鳜
 鱗	鳞
 鱘	鲟
 鱚	𬶮
 鱝	鲼
 鱟	鲎
 鱠	鲙
-鱢	𫚫
 鱣	鳣
 鱤	鳡
 鱧	鳢
 鱨	鲿
 鱭	鲚
-鱮	𫚈
 鱯	鳠
 鱲	𫚭
 鱷	鳄
 鱸	鲈
 鱺	鲡
+鱻	鲜
 鳥	鸟
 鳧	凫
 鳩	鸠
 鳬	凫
 鳲	鸤
 鳳	凤
 鳴	鸣
 鳶	鸢
-鳷	𫛛
-鳼	𪉃
-鳽	𫛚
 鳾	䴓
-鴀	𫛜
-鴃	𫛞
-鴅	𫛝
 鴆	鸩
 鴇	鸨
+鴈	雁
 鴉	鸦
-鴐	𫛤
 鴒	鸰
-鴔	𫛡
 鴕	鸵
-鴗	𫁡
 鴛	鸳
-鴜	𪉈
 鴝	鸲
 鴞	鸮
 鴟	鸱
 鴣	鸪
-鴥	𫛣
 鴦	鸯
 鴨	鸭
-鴮	𫛦
 鴯	鸸
 鴰	鸹
-鴲	𪉆
-鴳	𫛩
 鴴	鸻
 鴷	䴕
 鴻	鸿
-鴽	𫛪
 鴿	鸽
 鵁	䴔
 鵂	鸺
 鵃	鸼
-鵊	𫛥
 鵏	𬷕
 鵐	鹀
 鵑	鹃
 鵒	鹆
 鵓	鹁
-鵚	𪉍
 鵜	鹈
 鵝	鹅
+鵞	鹅
 鵟	𫛭
 鵠	鹄
 鵡	鹉
-鵧	𫛨
-鵩	𫛳
 鵪	鹌
-鵫	𫛱
 鵬	鹏
 鵮	鹐
 鵯	鹎
-鵰	雕 𫛲
+鵰	雕
 鵲	鹊
-鵷	鹓
+鵶	鸦
 鵾	鹍
 鶄	䴖
 鶇	鸫
 鶉	鹑
 鶊	鹒
-鶌	𫛵
-鶒	𫛶
 鶓	鹋
 鶖	鹙
-鶗	𫛸
 鶘	鹕
 鶚	鹗
 鶠	𬸘
 鶡	鹖
 鶥	鹛
-鶦	𫛷
 鶩	鹜
 鶪	䴗
 鶬	鸧
-鶭	𫛯
 鶯	莺
-鶰	𫛫
 鶱	𬸣
 鶲	鹟
 鶴	鹤
 鶹	鹠
 鶺	鹡
 鶻	鹘
 鶼	鹣
 鶿	鹚
 鷀	鹚
 鷁	鹢
 鷂	鹞
 鷄	鸡
-鷅	𫛽
 鷉	䴘
 鷊	鹝
-鷐	𫜀
 鷓	鹧
-鷔	𪉑
-鷖	鹥
 鷗	鸥
 鷙	鸷
 鷚	鹨
 鷟	𬸦
-鷣	𫜃
-鷤	𫛴
 鷥	鸶
 鷦	鹪
-鷨	𪉊
-鷩	𫜁
 鷫	鹔
 鷭	𬸪
 鷯	鹩
+鷰	燕
 鷲	鹫
 鷳	鹇
 鷴	鹇
-鷷	𫜄
 鷸	鹬
 鷹	鹰
 鷺	鹭
-鷽	鸴
-鷿	𬸯
-鸂	㶉
 鸇	鹯
 鸊	䴙
-鸋	𫛢
 鸌	鹱
+鸎	莺
 鸏	鹲
 鸑	𬸚
 鸕	鸬
-鸗	𫛟
 鸘	鹴
 鸚	鹦
 鸛	鹳
 鸝	鹂
 鸞	鸾
 鹵	卤
 鹹	咸
 鹺	鹾
+鹻	碱
 鹼	碱
 鹽	盐
+麐	麟
 麗	丽
+麞	獐
+麤	粗
 麥	麦
-麨	𪎊
 麩	麸
-麪	面 麺
+麪	面
 麫	面
-麬	𤿲
 麯	曲
-麲	𪎉
-麳	𪎌
 麴	曲 麹
-麵	面 麺
-麷	𫜑
+麵	面
 麼	么 麽
 麽	么 麽
 黃	黄
 黌	黉
 點	点
 黨	党
 黲	黪
 黴	霉
 黶	黡
 黷	黩
 黽	黾
 黿	鼋
-鼂	鼌
+鼃	蛙
+鼇	鳌
+鼈	鳖
 鼉	鼍
 鼕	冬
 鼴	鼹
 齊	齐
 齋	斋
 齎	赍
 齏	齑
@@ -3727,387 +3659,77 @@
 齙	龅
 齜	龇
 齟	龃
 齠	龆
 齡	龄
 齣	出
 齦	龈
-齧	啮 𫜩
-齩	𫜪
+齧	啮
+齩	咬
 齪	龊
 齬	龉
-齭	𫜭
 齮	𬺈
 齯	𫠜
-齰	𫜬
 齲	龋
-齴	𫜮
 齶	腭
 齷	龌
 齼	𬺓
-齾	𫜰
 龍	龙
-龎	厐
 龐	庞
 龑	䶮
-龓	𫜲
 龔	龚
 龕	龛
 龜	龟
-龭	𩨎
-龯	𨱆
-鿁	䜤
-鿓	鿒
-𠁞	𠀾
-𠌥	𠆿
-𠏢	𠉗
-𠐊	𫝋
-𠗣	㓆
-𠞆	𠛆
-𠠎	𠚳
-𠬙	𪠡
-𠽃	𪠺
-𠿕	𪜎
-𡂡	𪢒
-𡃄	𪡺
-𡃕	𠴛
-𡃤	𪢐
-𡄔	𠴢
-𡄣	𠵸
-𡅏	𠲥
-𡅯	𪢖
+龢	龢 和
+虜	虏
+奔	奔
+𠇮	命
+𠌂	伞
+𠕂	再
+𠕅	再
+𠖇	冥
+𠞰	剿
+𠪱	历
+𠴟	咩
+𠴰	咱
+𠻳	嗽
+𡐨	野
 𡑍	𫭼
-𡑭	𡋗
-𡓁	𪤄
-𡓾	𡋀
-𡔖	𡍣
-𡞵	㛟
-𡟫	𫝪
-𡠹	㛿
-𡢃	㛠
-𡮉	𡭜
-𡮣	𡭬
-𡳳	𡳃
-𡸗	𪨩
-𡹬	𪨹
+𡚁	弊
+𡨘	冤
+𡨥	寇
+𡬶	寻
 𡻕	岁
-𡽗	𡸃
-𡾱	㟜
-𡿖	𪩛
-𢍰	𪪴
-𢠼	𢙑
-𢣐	𪬚
-𢣚	𢘝
-𢣭	𢘞
-𢤩	𪫡
-𢤱	𢘙
-𢤿	𪬯
-𢯷	𪭝
-𢶒	𪭯
-𢶫	𢫞
-𢷮	𢫊
-𢹿	𢬦
-𢺳	𪮳
+𢬸	括
+𢮥	操
+𢷬	捣
 𣈶	暅
-𣋋	𣈣
-𣍐	𫧃
-𣙎	㭣
-𣜬	𪳗
-𣝕	𣘷
-𣞻	𣘓
-𣠩	𣞎
-𣠲	𣑶
-𣯩	𣯣
-𣯴	𣭤
-𣯶	毶
-𣽏	𪶮
-𣾷	㳢
-𣿉	𣶫
-𤁣	𣺽
-𤄷	𪶒
-𤅶	𣷷
-𤑳	𤎻
-𤑹	𪹀
-𤒎	𤊀
-𤒻	𪹹
-𤓌	𪹠
-𤓎	𤎺
-𤓩	𤊰
-𤘀	𪺣
-𤛮	𤙯
-𤛱	𫞢
-𤜆	𪺪
-𤠮	𪺸
-𤢟	𤝢
-𤢻	𢢐
-𤩂	𫞧
-𤪺	㻘
-𤫩	㻏
-𤬅	𪼴
-𤳷	𪽝
-𤳸	𤳄
-𤷃	𪽭
-𤸫	𤶧
-𤺔	𪽴
-𥊝	𥅿
-𥌃	𥅘
-𥏝	𪿊
-𥕥	𥐰
-𥖅	𥐯
-𥖲	𪿞
-𥗇	𪿵
+𣙜	榷
+𣺌	渺
+𤋮	熙
+𤨏	琐
+𤰜	亩
+𤱈	亩
+𤱊	留
+𤺥	瘩
+𥄨	瞅
 𥗽	𬒗
-𥜐	𫀓
-𥜰	𫀌
-𥞵	𥞦
-𥢢	䅪
-𥢶	𫞷
-𥢷	𫀮
-𥨐	𥧂
-𥪂	𥩺
-𥯤	𫁳
-𥴨	𫂖
-𥴼	𫁺
-𥵃	𥱔
-𥵊	𥭉
-𥶽	𫁱
-𥸠	𥮋
-𥻦	𫂿
-𥼽	𥹥
-𥽖	𥺇
-𥾯	𫄝
-𥿊	𦈈
-𦀖	𫄦
-𦂅	𦈒
-𦃄	𦈗
-𦃩	𫄯
-𦅇	𫄪
-𦅈	𫄵
-𦆲	𫟇
-𦒀	𫅥
-𦔖	𫅼
-𦘧	𡳒
-𦟼	𫆝
-𦠅	𫞅
-𦡝	𫆫
-𦢈	𣍨
-𦣎	𦟗
-𦧺	𫇘
-𦪙	䑽
-𦪽	𦨩
-𦱌	𫇪
-𦾟	𦶻
-𧎈	𧌥
-𧒯	𫊹
-𧔥	𧒭
-𧕟	𧉐
-𧜗	䘞
-𧜵	䙊
-𧝞	䘛
-𧞫	𫌋
-𧟀	𧝧
-𧡴	𫌫
-𧢄	𫌬
-𧦝	𫍞
-𧦧	𫍟
-𧩕	𫍭
-𧩙	䜥
-𧩼	𫍶
-𧫝	𫍺
-𧬤	𫍼
-𧭈	𫍾
-𧭹	𫍐
-𧳟	𧳕
-𧵳	䞌
-𧶔	𧹓
-𧶧	䞎
-𧷎	𪠀
-𧸘	𫎨
-𧹈	𪥠
-𧽯	𫎸
-𨂐	𫏌
-𨄣	𨀱
-𨅍	𨁴
-𨆪	𫏕
-𨇁	𧿈
-𨇞	𨅫
-𨇤	𫏨
-𨇰	𫏞
-𨇽	𫏑
-𨈊	𨂺
-𨈌	𨄄
-𨊰	䢀
-𨊸	䢁
-𨊻	𨐆
-𨋢	䢂
-𨌈	𫐍
-𨍰	𫐔
-𨎌	𫐋
-𨎮	𨐉
-𨏠	𨐇
-𨏥	𨐊
-𨞺	𫟫
-𨟊	𫟬
-𨢿	𨡙
-𨣈	𨡺
-𨣞	𨟳
-𨣧	𨠨
-𨤻	𨤰
-𨥛	𨱀
-𨥟	𫓫
-𨦫	䦀
+𥤚	秋
+𥦗	窗
+𥲻	纂
+𦂳	紧
+𦃂	紧
+𦉆	碴
+𦊱	挂
+𦍑	羌
+𦕈	眇
+𦵏	葬
 𨧀	𬭊
-𨧜	䦁
-𨧰	𫟽
-𨧱	𨱊
 𨨏	𬭛
-𨨛	𫓼
-𨨢	𫓿
-𨩰	𫟾
-𨪕	𫓮
-𨫒	𨱐
-𨬖	𫔏
 𨭆	𬭶
 𨭎	𬭳
-𨭖	𫔑
-𨭸	𫔐
-𨮂	𨱕
-𨮳	𫔒
-𨯅	䥿
-𨯟	𫔓
-𨰃	𫔉
-𨰋	𫓳
-𨰥	𫔕
-𨰲	𫔃
-𨲳	𫔖
-𨳑	𨸁
-𨳕	𨸀
-𨴗	𨸅
-𨴹	𫔲
-𨵩	𨸆
-𨵸	𨸇
-𨶀	𨸉
-𨶏	𨸊
-𨶮	𨸌
-𨶲	𨸋
-𨷲	𨸎
-𨼳	𫔽
-𨽏	𨸘
-𩀨	𫕚
-𩅙	𫕨
-𩎖	𫖑
-𩎢	𩏾
-𩏂	𫖓
-𩏠	𫖖
-𩏪	𩏽
-𩏷	𫃗
-𩑔	𫖪
-𩒎	𫖭
-𩓣	𩖕
-𩓥	𫖵
-𩔑	𫖷
-𩔳	𫖴
-𩖰	𫠇
-𩗀	𩙦
-𩗓	𫗈
-𩗴	𫗉
-𩘀	𩙩
-𩘝	𩙭
-𩘹	𩙨
-𩘺	𩙬
-𩙈	𩙰
-𩚛	𩟿
-𩚥	𩠀
-𩚩	𫗡
-𩚵	𩠁
-𩛆	𩠂
-𩛌	𫗤
-𩛡	𫗨
-𩛩	𩠃
-𩜇	𩠉
-𩜦	𩠆
-𩜵	𩠊
-𩝔	𩠋
-𩝽	𫗳
-𩞄	𩠎
-𩞦	𩠏
-𩞯	䭪
-𩟐	𩠅
-𩟗	𫗚
-𩠴	𩠠
-𩡣	𩡖
-𩡺	𩧦
-𩢡	𩧬
-𩢴	𩧵
-𩢸	𩧳
-𩢾	𩧮
-𩣏	𩧶
-𩣑	䯃
-𩣫	𩧸
-𩣵	𩧻
-𩣺	𩧼
-𩤊	𩧩
-𩤙	𩨆
-𩤲	𩨉
-𩤸	𩨅
-𩥄	𩨋
-𩥇	𩨍
-𩥉	𩧱
-𩥑	𩨌
-𩦠	𫠌
-𩧆	𩨐
-𩭙	𩬣
-𩯁	𫙂
-𩯳	𩯒
-𩰀	𩬤
-𩰹	𩰰
-𩳤	𩲒
-𩴵	𩴌
-𩵦	𫠏
-𩵩	𩽺
-𩵹	𩽻
-𩶁	𫚎
-𩶘	䲞
-𩶰	𩽿
-𩶱	𩽽
-𩷰	𩾄
-𩸃	𩾅
-𩸄	𫚝
-𩸡	𫚟
-𩸦	𩾆
-𩻗	𫚨
-𩻬	𫚩
-𩻮	𫚘
-𩼶	𫚬
-𩽇	𩾎
-𩿅	𫠖
-𩿤	𫛠
-𩿪	𪉄
-𪀖	𫛧
-𪀦	𪉅
-𪀾	𪉋
-𪁈	𪉉
-𪁖	𪉌
-𪂆	𪉎
-𪃍	𪉐
-𪃏	𪉏
-𪃒	𫛻
-𪃧	𫛹
-𪄆	𪉔
-𪄕	𪉒
-𪅂	𫜂
-𪆷	𫛾
-𪇳	𪉕
-𪈼	𱊜
-𪉸	𫜊
-𪋿	𫧮
-𪌭	𫜓
-𪍠	𫜕
-𪓰	𫜟
-𪔵	𪔭
-𪘀	𪚏
-𪘯	𪚐
-𪙏	𫜯
-𪟖	𠛾
-𪷓	𣶭
-𫒡	𫓷
-𫜦	𫜫
+𨽻	隶
+𩓐	脖
+𩗗	飓
+𭁵	寇
+兔	兔
+軔	轫
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.24.0/sts/data/dictionary/TSPhrases.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 一目瞭然	一目了然
 上鍊	上链
+不可貲計	不可赀計
 不瞭解	不了解
 么麼	幺麽
 么麽	幺麽
 乾乾淨淨	干干净净
 乾乾脆脆	干干脆脆
 乾元	乾元
 乾卦	乾卦
@@ -26,14 +27,15 @@
 乾造	乾造
 乾道	乾道
 乾陵	乾陵
 乾隆	乾隆
 乾隆年間	乾隆年间
 乾隆皇帝	乾隆皇帝
 二噁英	二𫫇英
+仇讎	仇雠
 以免藉口	以免借口
 以功覆過	以功复过
 侔德覆載	侔德复载
 傢俱	家具
 傷亡枕藉	伤亡枕藉
 八濛山	八濛山
 凌藉	凌借
@@ -65,15 +67,17 @@
 徵羽摩柯	徵羽摩柯
 徵聲	徵声
 徵調	徵调
 徵音	徵音
 情有獨鍾	情有独钟 情有独锺
 憑藉	凭借
 憑藉着	凭借着
+所費不貲	所费不赀
 手鍊	手链
+扞格	扞格
 扭轉乾坤	扭转乾坤
 找藉口	找借口
 拉鍊	拉链
 拉鍊工程	拉链工程
 拜覆	拜复
 據瞭解	据了解
 文錦覆阱	文锦复阱
@@ -102,23 +106,27 @@
 於邑	於邑
 於陵子	於陵子
 旋乾轉坤	旋乾转坤
 旋轉乾坤	旋转乾坤
 旋轉乾坤之力	旋转乾坤之力
 明瞭	明了
 明覆	明复
+春蒐	春蒐
 書中自有千鍾粟	书中自有千锺粟
 有序	有序
 朝乾夕惕	朝乾夕惕
 木吒	木吒
 李乾德	李乾德
 李澤鉅	李泽钜
 李鍊福	李链福
 李鍾郁	李锺郁
+束脩	束脩
+校讎	校雠
 樊於期	樊於期
+橡椀	橡椀
 沈沒	沉没
 沈沒成本	沉没成本
 沈積	沉积
 沈船	沉船
 沈默	沉默
 流徵	流徵
 浪蕩乾坤	浪荡乾坤
@@ -128,14 +136,16 @@
 牴觸	抵触
 狐藉虎威	狐借虎威
 珍珠項鍊	珍珠项链
 甚鉅	甚钜
 申覆	申复
 畢昇	毕昇
 發覆	发复
+目劄	目劄
+瞭哨	瞭哨
 瞭如	了如
 瞭如指掌	了如指掌
 瞭望	瞭望
 瞭然	了然
 瞭然於心	了然于心
 瞭若指掌	了若指掌
 瞭解	了解
@@ -188,14 +198,15 @@
 藉詞	借词
 藉讀	借读
 藉資	借资
 衹得	只得
 衹見樹木	只见树木
 衹見樹木不見森林	只见树木不见森林
 袖裏乾坤	袖里乾坤
+袷袢	袷袢
 覆上	复上
 覆住	复住
 覆信	复信
 覆冒	复冒
 覆呈	复呈
 覆命	复命
 覆墓	复墓
@@ -225,14 +236,15 @@
 見覆	见复
 角徵	角徵
 角徵羽	角徵羽
 計畫	计划
 變徵	变徵
 變徵之聲	变徵之声
 變徵之音	变徵之音
+讎定	雠定
 貂覆額	貂复额
 買臣覆水	买臣复水
 踅門瞭戶	踅门了户
 躪藉	躏借
 郭子乾	郭子乾
 酒逢知己千鍾少	酒逢知己千锺少
 酒逢知己千鍾少話不投機半句多	酒逢知己千锺少话不投机半句多
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.24.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.24.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.24.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+借記卡	簽帳金融卡
 元音	母音
 冰棍	冰棒
 出租車	計程車
 咖喱	咖哩
 塑料	塑膠
 奔馳	賓士
 奶酪	乳酪
@@ -30,8 +31,7 @@
 鍀	鎝
 鎄	鑀
 鎇	鋂
 鎿	錼
 鐦	鉲
 鑥	鎦
 黃宏	黃宏
-借記卡	簽帳金融卡
```

### Comparing `sts_lib-0.23.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.24.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts/data/htmlpage.tpl.html` & `sts_lib-0.24.0/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.24.0/sts/data/scheme/st_multi.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 托	托 託	與「捧呈」、「承受」有關用「托」，與「寄」、「委任」有關用「託」。	襯托 槍托 寄託 託付 推託
 挨	挨 捱	表示「承受」、「拖延」、「抗拒」有關用「捱」，讀爲ai2，其餘用「挨」，讀爲ai1。	挨家挨戶 捱打
 挽	挽 輓	與「哀悼死者」有關用「輓」，其餘意義爲「挽」。	挽救 力挽狂瀾 輓聯 哀輓
 栗	慄 栗	表示「因恐懼而發抖」用「慄」，其餘意義用「栗」。	板栗 火中取栗 戰慄 不寒而慄
 炼	煉 鍊	專指「熔鍊金屬」時用「鍊」，一般意義用「煉」。	鍊鐵 淬鍊 煉乳 修煉
 链	鏈 鍊	「鏈」用作一般的「金屬繩狀物」，「鍊」專指首飾。	鎖鏈 鏈接 項鍊 金手鍊
 穗	穗 繐	「繐」用作「結紮成的裝飾物」，其餘用「穗」。	麥穗 帽繐
-雕	彫 鵰	「鵰」爲一種猛禽，與「彫刻」有關時用「彫」。	一箭雙鵰 彫刻 彫蟲小技
+雕	雕 彫 鵰 琱	猛禽名用「鵰」「雕」，「雕刻之技術或成品」用「彫」「雕」「琱」，玉器、彩飾等用「琱」「雕」。	一箭雙鵰 彫刻 彫蟲小技 琱弓 琱麗
 梁	樑 梁	與「橋樑」、「棟樑」有關用「樑」，其餘意義爲「梁」。	樑上君子 鼻樑 大梁城 梁朝 梁山
 升	升 昇	「昇」字帶有濃烈喜慶氣氛，其餘用「升」。	上升 一升水 旭日東昇 歌舞昇平
 摆	擺 襬	表示「衣服下緣的部分」用「襬」，其餘用「擺」。	搖擺 擺放 裙襬 下襬
 岩	巖 岩	「岩」只用於「岩石」相關意義，其餘用「巖」。	沉積岩 岩漿 巖壁 中空成巖
 娘	娘 孃	「孃」意義爲「母親」，其餘用「娘」。	老孃 爹孃 孃家 姑娘 娘子 婆娘 舞娘
 僵	僵 殭	「殭」意義爲「不腐朽的屍體」，其餘用「僵」。	殭屍 殭蠶 僵硬 僵局 李代桃僵 百足之蟲，死而不僵
 药	藥 葯	「葯」特指「花的雄蕊中貯藏花粉的部份」，其餘用「藥」。	醫藥 良藥 芍藥 藥到病除 花葯
@@ -198,10 +198,12 @@
 谥	諡 謚	「諡」用於「諡號」，「謚」見於古文。
 熏	熏 燻	「熏」可用於「煙燻」或「薰香」義。
 旋	旋 鏇	「旋」用於「旋轉」等。「鏇」用於「旋轉削切」等。
 沾	沾 霑	「雨水浸潤」、「受恩」等義用「霑」，「浸溼」等義通用，「接觸」「染上」「帶有」等義用「沾」。
 跖	跖 蹠	「腳掌」等以「蹠」為正字。「跖」可用於人名，如「盜跖」。
 玩	玩 翫	「鬆懈、輕忽」用「翫」，其餘「玩」「翫」通用。
 璇	璇 璿	星名用「璇」。「天文儀」、「美玉」義可互通。二字皆有用於人名。	天璇
+你	你 妳	「你」用於一般性第二人稱，或專指男性。「妳」用於女性第二人稱。
 它	它 牠	對動物的第三人稱用「牠」。
 蝎	蠍 蝎	「蝎」另兼正字義為「木中蠹蟲」。
 唇	脣 唇	「嘴脣」以「脣」為正字。「唇」另義為「驚駭」，讀作zhēn。
+硷	鹼 礆	《簡化字總表》把「鹼」簡化為「硷」，《通用規範漢字表》改以「碱」為標準字，「鹼」為異體字。「硷」另可作為「礆」的類推簡化字。
```

### Comparing `sts_lib-0.23.0/sts/data/scheme/variant.txt` & `sts_lib-0.24.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.23.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.24.0/sts_lib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.23.0
+Version: 0.24.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: yaml
+Requires-Dist: pyyaml>=5.0; extra == "yaml"
 Provides-Extra: dev
+Requires-Dist: pyyaml>=5.0; extra == "dev"
 Requires-Dist: flake8>=4.0; extra == "dev"
 Requires-Dist: flake8-quotes>=3.4; extra == "dev"
 Requires-Dist: flake8-comprehensions>=3.7; extra == "dev"
 Requires-Dist: flake8-string-format>=0.3; extra == "dev"
 Requires-Dist: pep8-naming>=0.13.2; extra == "dev"
 Requires-Dist: flake8-bugbear>=22.0; extra == "dev"
 Requires-Dist: flake8-isort>=4.2; extra == "dev"
@@ -108,32 +111,37 @@
  *     directory of this config file, or the basename of a built-in config file
  *     (with or without ".json")
  * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
  */
 
 /**
  * @typedef {Object} dictScheme
- * @property {string} file - path of the dictionary file to generate. Each as
- *     an absolute path, or a path relative to the specified output directory
- *     (or the directory of this config file). Each should be a .tlist
- *     (compiled trie), .jlist (compiled table), or .list (plain text table).
+ * @property {string} file - path of the dictionary file to generate, as an
+ *     absolute path, or a path relative to the specified output directory
+ *     (or the directory of this config file). It should be a .tlist (compiled
+ *     trie), .jlist (compiled table), or .list (plain text table).
  * @property {string} mode - the mode to handle the loaded source files: "load"
  *     to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
  * @property {Array.<(string|string[])>} src - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
- *     or the basename of a built-in dictionary file. Each should be a .txt or
- *     .list dictionary file.
+ *     or the basename of a built-in dictionary file. Each should be a .txt,
+ *     .list, .json, .jlist, .yaml, or .yml dictionary file.
  * @property {boolean} [sort] - true to sort the keys of the output dictionary.
  * @property {string} [include] - a regex filter that discards non-matched
  *     conversion values.
  * @property {string} [exclude] - a regex filter that discards matched
  *     conversion values.
+ * @property {boolean} [check] - true to raise an exception if the output
+ *     contains an invalid char which will be loaded incorrectly. Set this
+ *     when the output is a plain text table file and the source files contain
+ *     untrusted JSON or YAML data that may include a char like " ", "\t",
+ *     "\n", etc. in the dictionary.
  */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
```

### Comparing `sts_lib-0.23.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.24.0/sts_lib.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,44 +4,64 @@
 setup.cfg
 setup.py
 sts/__init__.py
 sts/__main__.py
 sts/cli.py
 sts/data/htmlpage.tpl.html
 sts/data/config/_default.json
+sts/data/config/_extend.json
 sts/data/config/hk2s.json
+sts/data/config/hk2sp.json
+sts/data/config/hk2spx.json
+sts/data/config/hk2sx.json
 sts/data/config/hk2t.json
 sts/data/config/jp2t.json
 sts/data/config/s2hk.json
+sts/data/config/s2hkp.json
 sts/data/config/s2t.json
 sts/data/config/s2tw.json
 sts/data/config/s2twp.json
 sts/data/config/t2hk.json
 sts/data/config/t2jp.json
+sts/data/config/t2jpx.json
 sts/data/config/t2s.json
+sts/data/config/t2sx.json
 sts/data/config/t2tw.json
 sts/data/config/tw2s.json
 sts/data/config/tw2sp.json
+sts/data/config/tw2spx.json
+sts/data/config/tw2sx.json
 sts/data/config/tw2t.json
+sts/data/dictionary/HKPhrases.txt
+sts/data/dictionary/HKPhrasesRev.txt
 sts/data/dictionary/HKVariants.txt
 sts/data/dictionary/HKVariantsRevPhrases.txt
+sts/data/dictionary/JPKyujitaiCharacters.txt
 sts/data/dictionary/JPShinjitaiCharacters.txt
 sts/data/dictionary/JPShinjitaiPhrases.txt
 sts/data/dictionary/JPVariants.txt
+sts/data/dictionary/JPVariantsEx.txt
 sts/data/dictionary/STCharacters.txt
+sts/data/dictionary/STCharactersEx.txt
 sts/data/dictionary/STPhrases.txt
 sts/data/dictionary/TSCharacters.txt
+sts/data/dictionary/TSCharactersEx.txt
 sts/data/dictionary/TSPhrases.txt
 sts/data/dictionary/TWPhrasesIT.txt
 sts/data/dictionary/TWPhrasesName.txt
 sts/data/dictionary/TWPhrasesOther.txt
+sts/data/dictionary/TWPhrasesRev.txt
 sts/data/dictionary/TWVariants.txt
 sts/data/dictionary/TWVariantsRevPhrases.txt
 sts/data/scheme/st_multi.txt
+sts/data/scheme/st_unihan13.txt
 sts/data/scheme/ts_multi.txt
+sts/data/scheme/ts_tgh_convert.txt
+sts/data/scheme/ts_tgh_list.txt
+sts/data/scheme/ts_unihan13.txt
 sts/data/scheme/variant.txt
 sts_lib.egg-info/PKG-INFO
 sts_lib.egg-info/SOURCES.txt
 sts_lib.egg-info/dependency_links.txt
 sts_lib.egg-info/entry_points.txt
 sts_lib.egg-info/requires.txt
 sts_lib.egg-info/top_level.txt
```

