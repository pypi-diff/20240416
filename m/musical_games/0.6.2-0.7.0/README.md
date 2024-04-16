# Comparing `tmp/musical_games-0.6.2.tar.gz` & `tmp/musical_games-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.6.2.tar` & `musical_games-0.7.0.tar`

### file list

```diff
@@ -1,91 +1,99 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.6.2/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.6.2/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.6.2/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.6.2/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.6.2/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.6.2/.travis.yml
--rw-r--r--   0        0        0      941 2024-04-13 18:22:27.832740 musical_games-0.6.2/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.6.2/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.6.2/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.6.2/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.6.2/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.6.2/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.6.2/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.6.2/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.6.2/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.6.2/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.6.2/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.6.2/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.6.2/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     5346 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.6.2/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    34442 2024-04-13 18:22:02.752740 musical_games-0.6.2/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.6.2/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    13161 2024-04-13 13:40:32.743692 musical_games-0.6.2/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/external/images.py
--rw-r--r--   0        0        0     3459 2024-04-10 16:29:16.694716 musical_games-0.6.2/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.6.2/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.6.2/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.6.2/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4695 2024-04-09 10:54:53.546529 musical_games-0.6.2/musical_games/utils.py
--rw-r--r--   0        0        0     1114 2024-04-13 18:22:18.384740 musical_games-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.6.2/scripts/__init__.py
--rw-r--r--   0        0        0     1649 2024-04-13 13:01:09.427755 musical_games-0.6.2/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     1652 2024-04-13 13:54:11.547670 musical_games-0.6.2/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1761 2024-04-13 14:21:32.579626 musical_games-0.6.2/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1519 2024-04-13 14:35:38.727603 musical_games-0.6.2/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     1664 2024-04-13 13:01:48.155754 musical_games-0.6.2/scripts/demo_stadler_meneut_trio.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.6.2/tox.ini
--rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 musical_games-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.7.0/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.7.0/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.7.0/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.7.0/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.7.0/.travis.yml
+-rw-r--r--   0        0        0     1032 2024-04-16 05:06:34.950851 musical_games-0.7.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.7.0/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.7.0/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.7.0/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.7.0/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.7.0/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.7.0/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.7.0/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1830 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2798 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3767 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.7.0/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    34442 2024-04-13 18:22:02.752740 musical_games-0.7.0/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.7.0/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    15391 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.7.0/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.7.0/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.7.0/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4695 2024-04-09 10:54:53.546529 musical_games-0.7.0/musical_games/utils.py
+-rw-r--r--   0        0        0     1114 2024-04-16 05:06:24.374851 musical_games-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.7.0/scripts/__init__.py
+-rw-r--r--   0        0        0     9431 2024-04-16 05:05:56.478852 musical_games-0.7.0/scripts/copy_bars.py
+-rw-r--r--   0        0        0     1649 2024-04-13 13:01:09.427755 musical_games-0.7.0/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     1652 2024-04-13 13:54:11.547670 musical_games-0.7.0/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1761 2024-04-13 14:21:32.579626 musical_games-0.7.0/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1556 2024-04-16 05:05:56.478852 musical_games-0.7.0/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1519 2024-04-13 14:35:38.727603 musical_games-0.7.0/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     1664 2024-04-13 13:01:48.155754 musical_games-0.7.0/scripts/demo_stadler_meneut_trio.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.7.0/tox.ini
+-rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 musical_games-0.7.0/PKG-INFO
```

### Comparing `musical_games-0.6.2/.gitchangelog.rc` & `musical_games-0.7.0/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/.gitignore` & `musical_games-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/CHANGELOG.rst` & `musical_games-0.7.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 *********
 Changelog
 *********
 
+v0.7.0 (2024-04-16)
+===================
+
+Added
+-----
+- Adds the contredanse from Mozart.
+
+
 v0.6.2 (2024-04-13)
 ===================
 
 Added
 -----
 - Adds pip release to makefile.
```

### Comparing `musical_games-0.6.2/LICENSE` & `musical_games-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/Makefile` & `musical_games-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/README.rst` & `musical_games-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/Makefile` & `musical_games-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/conf.py` & `musical_games-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/contributing.rst` & `musical_games-0.7.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/index.rst` & `musical_games-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/make.bat` & `musical_games-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/musical_games.converters.rst` & `musical_games-0.7.0/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.7.0/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/musical_games.dice_games.rst` & `musical_games-0.7.0/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/docs/musical_games.rst` & `musical_games-0.7.0/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/__version__.py` & `musical_games-0.7.0/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 "12","g''8. [b''16] dis''8. [fis''16] e''4","e4 b,4 e,4"
 "13","\tuplet 3/2 {fis''8 [g''8 a''8]} fis''4 \tuplet 3/2 {cis''8 [d''8 e''8]}","d'4 a4 g4"
 "14","fis''8 [e''8] e''4 fis''4","d4. a8 fis8 [d8]"
 "15","g''8 [a'8] r8 cis''8 e''8 [g''8]","cis4 a,4 cis4"
 "16","d'2.","d4 a,4 d,4"
 "17","\tuplet 3/2 {b'8 [a'8 g'8]} b'4 b'4","r4 g4 g4"
 "18","\tuplet 3/2 {fis''8 [e''8 d''8]} fis''4 fis''4","r4 d4 d4"
-"19","fis''8 [d'8] r8 a''8 cis''8 ([d''8)]","d4 e4 fis4"
+"19","fis''8 [d'8] r8 a''8 cis''8 ([d''8])","d4 e4 fis4"
 "20","g'8 [e''8] e'8 [g'8] fis'4","e4 cis4 d4"
 "21","r8 a'8 [b'8 a'8] e''8 [g''8]","cis2."
 "22","a'8 [d''8] g''8 [fis''8] e''8 [d''8]","r4 d4 d4"
 "23","a'8 [d''8] fis''4 e''4","d4 d'4 a4"
 "24","d'2.","d4 a,4 d,4"
 "25","b'8 [g'8] fis'8 [g'8] b'8 [d''8]","g4 g4 g4"
 "26","d''8 [d'8] fis'4 e'4 ^\trill","fis8 [g8] a4 a,4"
```

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/dice_games/base.py` & `musical_games-0.7.0/musical_games/dice_games/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/dice_games/data_csv.py` & `musical_games-0.7.0/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/dice_games/dice_games.py` & `musical_games-0.7.0/musical_games/dice_games/dice_games.py`

 * *Files 11% similar despite different names*

```diff
@@ -184,18 +184,56 @@
             {'waltz': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'waltz': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Mozart', 'Waltz', dice_tables, bar_collections,
                          jinja2_environment, midi_settings)
 
 
+class MozartContredanse(SimpleDiceGame):
+
+    def __init__(self):
+        """Implementation of a Contredanse dice game by Mozart."""
+        dice_tables = {
+            'contredanse': SimpleDiceTable(np.array([
+                [70, 14, 164, 122, 25, 153, 18, 167, 155, 3, 162, 170, 13, 166, 95, 5],
+                [10, 64, 100, 12, 149, 30, 161, 11, 148, 28, 135, 173, 169, 174, 2, 20],
+                [33, 1, 160, 163, 77, 156, 168, 172, 22, 176, 62, 126, 31, 24, 159, 41],
+                [36, 114, 8, 35, 111, 39, 137, 44, 4, 157, 38, 9, 151, 32, 17, 171],
+                [105, 150, 57, 71, 117, 52, 132, 130, 136, 91, 138, 19, 134, 101, 154, 146],
+                [165, 152, 112, 15, 147, 27, 73, 102, 144, 104, 87, 107, 128, 48, 109, 74],
+                [7, 81, 131, 37, 21, 125, 49, 115, 116, 133, 72, 141, 94, 80, 129, 65],
+                [142, 106, 40, 69, 43, 140, 23, 89, 66, 124, 26, 84, 75, 103, 96, 127],
+                [99, 68, 86, 139, 120, 92, 143, 83, 93, 55, 29, 51, 42, 110, 108, 98],
+                [85, 45, 90, 158, 82, 123, 78, 58, 61, 34, 119, 46, 59, 54, 60, 47],
+                [145, 97, 6, 121, 56, 67, 63, 16, 50, 79, 175, 76, 113, 88, 53, 118]]))
+        }
+
+        csv_reader = SimpleBarCollectionCSVReader()
+        bar_collections = {'contredanse': csv_reader.read_csv(resources.files('musical_games') /
+                                                        'data/dice_games/mozart_contredanse/contredanse_bars.csv')}
+
+        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/mozart_contredanse/lilypond')
+        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
+        jinja2_environment = jinja2.Environment(**env_options)
+
+        midi_settings = SimpleMidiSettings(
+            {'contredanse': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
+            {'contredanse': {'piano_right_hand': 0, 'piano_left_hand': 0}},
+            {'contredanse': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
+
+        super().__init__('Mozart', 'Contredanse', dice_tables, bar_collections,
+                         jinja2_environment, midi_settings)
+
+
 class StadlerMenuetTrio(SimpleDiceGame):
 
     def __init__(self):
-        """Implementation of a Menuet and Trio dice game by Kirnberger.
+        """Implementation of a Menuet and Trio dice game by Stadler.
+
+        A similar dice game has been made by Haydn.
 
         In this dice game, there is a dice table for the menuet and one for the trio.
         """
         dice_tables = {
             'menuet': SimpleDiceTable(np.array([
                 [96, 22, 141, 41, 105, 122, 11, 30, 70, 121, 26, 9, 112, 49, 109, 14],
                 [32, 6, 128, 63, 146, 46, 134, 81, 117, 39, 126, 56, 174, 18, 116, 83],
```

### Comparing `musical_games-0.6.2/musical_games/external/base.py` & `musical_games-0.7.0/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/external/images.py` & `musical_games-0.7.0/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/external/lilypond.py` & `musical_games-0.7.0/musical_games/external/lilypond.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from pathlib import Path
 import os
 
 from musical_games.external.images import trim_image
 from musical_games.external.utils import run_command
 
 
-def typeset_lilypond(lilypond_in: Path, output_basename: Path, pdf: bool = True, png: bool = True, ps: bool = False):
+def typeset_lilypond(lilypond_in: Path, output_basename: Path, pdf: bool = True, png: bool = True, ps: bool = False,
+                     trim_png: bool = True):
     """Typeset a lilypond file and produce midi and/or a composition from the input file.
 
     This runs the shell command lilypond to on the inputs. Note that Midi output needs to be defined in the lilypond
     file and can not be set on the command line.
 
     Args:
         lilypond_in: the location of the lilypond file to convert.
         output_basename: the location for the output files, suffixes will be added.
         pdf: if we want pdf output
         png: if we want png output
         ps: if we want postscript output
+        trim_png: if we want to automatically trim the PNG images.
 
     Raises:
         RuntimeError: if the compilation of the lilypond file failed somehow.
 
     Returns:
         LilypondTypesetResults: the result set with the location of the output files.
     """
@@ -44,16 +46,17 @@
     run_command(command)
 
     pdf_list = [output_basename.with_suffix('.pdf')] if pdf else []
     png_list = _get_png_list(output_basename) if png else []
     ps_list = [output_basename.with_suffix('.ps')] if ps else []
     midi_list = _get_midi_list(output_basename)
 
-    for png in png_list:
-        trim_image(png)
+    if trim_png:
+        for png in png_list:
+            trim_image(png)
 
     return LilypondTypesetResults(pdf_list, png_list, ps_list, midi_list)
 
 
 @dataclass(frozen=True, slots=True)
 class LilypondTypesetResults:
     """Result set for the output of the lilypond function.
```

### Comparing `musical_games-0.6.2/musical_games/external/midi_converters.py` & `musical_games-0.7.0/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/external/utils.py` & `musical_games-0.7.0/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/external/wav_converters.py` & `musical_games-0.7.0/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/musical_games/utils.py` & `musical_games-0.7.0/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/pyproject.toml` & `musical_games-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.6.2"
+version = "0.7.0"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.6.2/scripts/demo_cpe_bach.py` & `musical_games-0.7.0/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.7.0/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.7.0/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/scripts/demo_mozart_waltz.py` & `musical_games-0.7.0/scripts/demo_mozart_waltz.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.7.0/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/tox.ini` & `musical_games-0.7.0/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.6.2/PKG-INFO` & `musical_games-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.6.2
+Version: 0.7.0
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

