# Comparing `tmp/ships-1.2.6.tar.gz` & `tmp/ships-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ships-1.2.6.tar", last modified: Sun Apr  7 02:51:13 2024, max compression
+gzip compressed data, was "ships-1.2.7.tar", last modified: Tue Apr 16 02:28:14 2024, max compression
```

## Comparing `ships-1.2.6.tar` & `ships-1.2.7.tar`

### file list

```diff
@@ -1,273 +1,274 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/
--rw-r--r--   0 root         (0) root         (0)     1341 2024-04-07 02:51:13.902528 ships-1.2.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.870529 ships-1.2.6/fields/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.870529 ships-1.2.6/fields/gardens/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/AMLI/
--rw-rw-r--   0 root         (0) root         (0)      104 2024-03-30 17:23:39.000000 ships-1.2.6/fields/gardens/ships/AMLI/AMLI.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/AMLI/LLM/
--rw-rw-r--   0 root         (0) root         (0)       61 2024-02-15 19:38:33.000000 ships-1.2.6/fields/gardens/ships/AMLI/LLM/LLM.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/Search/
--rw-rw-r--   0 root         (0) root         (0)       44 2024-02-15 19:38:43.000000 ships-1.2.6/fields/gardens/ships/Search/Search.s.HTML
--rw-r--r--   0 root         (0) root         (0)     1008 2024-02-15 04:11:24.000000 ships-1.2.6/fields/gardens/ships/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/_clique/
--rw-rw-r--   0 root         (0) root         (0)      547 2024-02-15 04:21:26.000000 ships-1.2.6/fields/gardens/ships/_clique/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/_license/
--rw-r--r--   0 root         (0) root         (0)      173 2023-12-16 19:52:14.000000 ships-1.2.6/fields/gardens/ships/_license/license.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/_status/
--rw-r--r--   0 root         (0) root         (0)      198 2024-01-23 03:57:34.000000 ships-1.2.6/fields/gardens/ships/_status/ports.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-02-04 21:57:31.000000 ships-1.2.6/fields/gardens/ships/_status/status.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/business/
--rw-r--r--   0 root         (0) root         (0)       77 2023-11-22 19:02:46.000000 ships-1.2.6/fields/gardens/ships/business/business.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/business/decorators/
--rw-r--r--   0 root         (0) root         (0)       65 2023-11-22 19:10:51.000000 ships-1.2.6/fields/gardens/ships/business/decorators/decorators.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/business/decorators/examples/
--rw-r--r--   0 root         (0) root         (0)      747 2023-11-22 19:15:14.000000 ships-1.2.6/fields/gardens/ships/business/decorators/examples/example_1.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-11-22 19:09:40.000000 ships-1.2.6/fields/gardens/ships/business/decorators/examples/multiple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.874529 ships-1.2.6/fields/gardens/ships/cadence/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cadence/UTC/
--rw-rw-r--   0 root         (0) root         (0)        5 2023-08-24 19:13:50.000000 ships-1.2.6/fields/gardens/ships/cadence/UTC/UTC.r.HTML
--rw-rw-r--   0 root         (0) root         (0)      958 2023-12-19 05:34:09.000000 ships-1.2.6/fields/gardens/ships/cadence/UTC/current.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cadence/UTC/leap/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-24 19:08:54.000000 ships-1.2.6/fields/gardens/ships/cadence/UTC/leap/seconds.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-24 19:08:50.000000 ships-1.2.6/fields/gardens/ships/cadence/UTC/leap/years.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cadence/UTC/month/
--rw-rw-r--   0 root         (0) root         (0)      440 2023-12-19 05:34:09.000000 ships-1.2.6/fields/gardens/ships/cadence/UTC/month/strings.py
--rw-rw-r--   0 root         (0) root         (0)      604 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cadence/UTC/status_current.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cadence/filter/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-12-19 05:34:09.000000 ships-1.2.6/fields/gardens/ships/cadence/filter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cadence/filter/_status/
--rw-r--r--   0 root         (0) root         (0)      533 2023-12-19 05:34:09.000000 ships-1.2.6/fields/gardens/ships/cadence/filter/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-12-19 05:34:09.000000 ships-1.2.6/fields/gardens/ships/cadence/filter/_status/status_2.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-12-19 05:34:09.000000 ships-1.2.6/fields/gardens/ships/cadence/filter/_status/status_3.py
--rw-r--r--   0 root         (0) root         (0)        2 2023-11-27 01:22:43.000000 ships-1.2.6/fields/gardens/ships/clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/coms/
--rw-r--r--   0 root         (0) root         (0)      117 2023-12-01 16:30:53.000000 ships-1.2.6/fields/gardens/ships/coms/coms.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.874529 ships-1.2.6/fields/gardens/ships/coms/protocols/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/coms/protocols/SSH/
--rw-r--r--   0 root         (0) root         (0)      525 2023-12-01 14:37:22.000000 ships-1.2.6/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/coms/protocols/SSL/
--rw-r--r--   0 root         (0) root         (0)      186 2023-12-01 21:53:45.000000 ships-1.2.6/fields/gardens/ships/coms/protocols/SSL/SSL.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/coms/wall/
--rw-r--r--   0 root         (0) root         (0)        2 2023-12-01 16:29:57.000000 ships-1.2.6/fields/gardens/ships/coms/wall/wall.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cycle/
--rw-r--r--   0 root         (0) root         (0)      184 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cycle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cycle/loops/
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-06 04:02:30.000000 ships-1.2.6/fields/gardens/ships/cycle/loops/__init__.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-11-12 17:53:20.000000 ships-1.2.6/fields/gardens/ships/cycle/loops/loops.s.HTML
--rw-r--r--   0 root         (0) root         (0)      711 2023-12-19 05:47:03.000000 ships-1.2.6/fields/gardens/ships/cycle/loops/status_2.py
--rw-r--r--   0 root         (0) root         (0)      622 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cycle/loops/status_3.py
--rw-r--r--   0 root         (0) root         (0)      716 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cycle/loops/status_4.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.886528 ships-1.2.6/fields/gardens/ships/cycle/params/
--rw-r--r--   0 root         (0) root         (0)      658 2023-11-12 18:07:23.000000 ships-1.2.6/fields/gardens/ships/cycle/params/__init__.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cycle/params/status_1.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cycle/params/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/cycle/params_2/
--rw-r--r--   0 root         (0) root         (0)      940 2024-01-06 04:12:45.000000 ships-1.2.6/fields/gardens/ships/cycle/params_2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-12-28 20:22:31.000000 ships-1.2.6/fields/gardens/ships/cycle/params_2/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/cycle/presents/
--rw-r--r--   0 root         (0) root         (0)      313 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/cycle/presents/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/flow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/flow/demux_mux/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/flow/demux_mux/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/flow/demux_mux/_status/
--rw-r--r--   0 root         (0) root         (0)     1056 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/flow/demux_mux/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/flow/demux_mux2/
--rw-r--r--   0 root         (0) root         (0)      830 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/flow/demux_mux2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/flow/demux_mux2/_status/
--rw-r--r--   0 root         (0) root         (0)      515 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/flow/demux_mux2/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-11-08 16:55:45.000000 ships-1.2.6/fields/gardens/ships/flow/flow.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/flow/simultaneous/
--rw-rw-r--   0 root         (0) root         (0)     1402 2024-03-17 03:19:08.000000 ships-1.2.6/fields/gardens/ships/flow/simultaneous/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.874529 ships-1.2.6/fields/gardens/ships/formats/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/formats/ISO/
--rw-r--r--   0 root         (0) root         (0)      919 2024-01-19 20:43:25.000000 ships-1.2.6/fields/gardens/ships/formats/ISO/ISO.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.874529 ships-1.2.6/fields/gardens/ships/glamour/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/glamour/UTF8/
--rw-r--r--   0 root         (0) root         (0)     6927 2023-11-18 21:15:34.000000 ships-1.2.6/fields/gardens/ships/glamour/UTF8/one.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/insure/
--rw-r--r--   0 root         (0) root         (0)      690 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/insure/equalities.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/insure/equality.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/insure/status_equalitites_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.874529 ships-1.2.6/fields/gardens/ships/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/exceptions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/exceptions/custom/
--rw-r--r--   0 root         (0) root         (0)      221 2023-11-29 22:52:11.000000 ships-1.2.6/fields/gardens/ships/modules/exceptions/custom/__init__.py
--rw-r--r--   0 root         (0) root         (0)      445 2024-03-10 22:49:28.000000 ships-1.2.6/fields/gardens/ships/modules/exceptions/parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/fasten/
--rw-r--r--   0 root         (0) root         (0)      845 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/modules/fasten/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/fasten/_status/
--rw-r--r--   0 root         (0) root         (0)       46 2023-10-31 18:06:14.000000 ships-1.2.6/fields/gardens/ships/modules/fasten/_status/example.py
--rw-r--r--   0 root         (0) root         (0)      121 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/modules/fasten/_status/example_caller.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/modules/fasten/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/import/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/import/examples/
--rw-r--r--   0 root         (0) root         (0)      364 2023-11-28 05:02:32.000000 ships-1.2.6/fields/gardens/ships/modules/import/examples/example_1.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 04:57:58.000000 ships-1.2.6/fields/gardens/ships/modules/import/examples/example_1_module.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-11-30 01:01:28.000000 ships-1.2.6/fields/gardens/ships/modules/import/import.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/print/
--rw-r--r--   0 root         (0) root         (0)      679 2023-11-27 01:32:02.000000 ships-1.2.6/fields/gardens/ships/modules/print/print.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/string/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/string/NLP/
--rw-r--r--   0 root         (0) root         (0)       59 2023-12-17 22:23:07.000000 ships-1.2.6/fields/gardens/ships/modules/string/NLP/NLP.s.HTML
--rw-r--r--   0 root         (0) root         (0)      265 2023-11-12 18:56:01.000000 ships-1.2.6/fields/gardens/ships/modules/string/end_of_string_is.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/modules/string/sayings/
--rw-r--r--   0 root         (0) root         (0)       93 2023-12-17 22:25:39.000000 ships-1.2.6/fields/gardens/ships/modules/string/sayings/sayings.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.890528 ships-1.2.6/fields/gardens/ships/paths/
--rw-r--r--   0 root         (0) root         (0)      223 2023-12-01 04:01:32.000000 ships-1.2.6/fields/gardens/ships/paths/caller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/
--rw-r--r--   0 root         (0) root         (0)     3453 2024-02-15 05:14:15.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:01:19.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_1/1.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:01:24.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_2/1.HTML
--rw-r--r--   0 root         (0) root         (0)      587 2024-02-15 05:03:56.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:12:57.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1/1.HTML
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:12:39.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:13:01.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/1/2.HTML
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:12:42.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/2.HTML
--rw-r--r--   0 root         (0) root         (0)      682 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py
--rw-rw-r--   0 root         (0) root         (0)        3 2024-02-15 04:09:56.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/
--rw-r--r--   0 root         (0) root         (0)      702 2023-12-03 23:10:11.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-12-03 23:10:11.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py
--rw-r--r--   0 root         (0) root         (0)      291 2023-12-03 23:10:11.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/get_directories.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-12-03 23:10:11.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/get_same_directories.py
--rw-r--r--   0 root         (0) root         (0)       70 2023-12-03 21:57:50.000000 ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/is_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/deallocate/
--rw-r--r--   0 root         (0) root         (0)      165 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/deallocate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/
--rw-r--r--   0 root         (0) root         (0)     2162 2024-04-07 02:50:44.000000 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/1/start/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/1/start/1/
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/1/start/1/1.py
--rw-r--r--   0 root         (0) root         (0)     1387 2024-03-30 03:49:06.000000 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/2/start/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/2/start/1/
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/2/start/1/1.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-10-13 23:54:40.000000 ships-1.2.6/fields/gardens/ships/paths/directory/equalize/equalize.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string/
--rw-r--r--   0 root         (0) root         (0)     1581 2024-03-30 17:45:42.000000 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py
--rw-r--r--   0 root         (0) root         (0)      196 2024-03-30 04:06:11.000000 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string/field.S.HTML
--rw-r--r--   0 root         (0) root         (0)      115 2023-10-21 23:43:14.000000 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string/in_path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string_v2/
--rw-r--r--   0 root         (0) root         (0)     3622 2024-03-30 19:17:21.000000 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      196 2024-03-30 04:06:11.000000 ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string_v2/field.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.894528 ships-1.2.6/fields/gardens/ships/paths/directory/for_each_path/
--rw-r--r--   0 root         (0) root         (0)      781 2023-10-21 23:50:37.000000 ships-1.2.6/fields/gardens/ships/paths/directory/for_each_path/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/rsync/
--rw-r--r--   0 root         (0) root         (0)     1797 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/rsync/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/
--rw-rw-r--   0 root         (0) root         (0)      974 2024-03-30 18:50:21.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/DFS.py
--rw-rw-r--   0 root         (0) root         (0)     2200 2024-03-30 18:22:06.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2032 2024-03-30 18:03:59.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1/
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1/1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_1/
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_1/1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_symlink_to_1/
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_symlink_to_1/1.py
--rw-rw-r--   0 root         (0) root         (0)     3629 2024-03-30 19:04:59.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/2/
--rw-rw-r--   0 root         (0) root         (0)     1020 2024-03-30 19:04:22.000000 ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/sense/
--rw-r--r--   0 root         (0) root         (0)     1212 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/sense/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/sense/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/sense/_status/1/
--rw-r--r--   0 root         (0) root         (0)      826 2024-03-30 05:18:51.000000 ships-1.2.6/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/size/
--rw-r--r--   0 root         (0) root         (0)      763 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/size/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.878528 ships-1.2.6/fields/gardens/ships/paths/directory/size/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/size/_status/1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/directory/size/_status/1/cryo/
--rw-r--r--   0 root         (0) root         (0)       34 2023-12-03 23:22:28.000000 ships-1.2.6/fields/gardens/ships/paths/directory/size/_status/1/cryo/hyper.HTML
--rw-r--r--   0 root         (0) root         (0)      623 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/directory/size/_status/1/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/paths/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/paths/files/scan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/files/scan/JSON/
--rw-r--r--   0 root         (0) root         (0)      544 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/files/scan/JSON/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/files/scan/JSON/status/
--rw-r--r--   0 root         (0) root         (0)      534 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/path/
--rw-r--r--   0 root         (0) root         (0)      327 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/paths/path/relative.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.898528 ships-1.2.6/fields/gardens/ships/paths/variety/
--rw-rw-r--   0 root         (0) root         (0)      396 2024-03-30 18:12:33.000000 ships-1.2.6/fields/gardens/ships/paths/variety/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/
--rw-r--r--   0 root         (0) root         (0)    12177 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py
--rw-r--r--   0 root         (0) root         (0)    13419 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py
--rw-r--r--   0 root         (0) root         (0)     4089 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/_async.py
--rw-r--r--   0 root         (0) root         (0)     3465 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py
--rw-r--r--   0 root         (0) root         (0)     3802 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13827 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/expect.py
--rw-r--r--   0 root         (0) root         (0)     5991 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py
--rw-r--r--   0 root         (0) root         (0)     6159 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py
--rw-r--r--   0 root         (0) root         (0)    37382 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py
--rw-r--r--   0 root         (0) root         (0)    24445 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py
--rw-r--r--   0 root         (0) root         (0)     6629 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/run.py
--rw-r--r--   0 root         (0) root         (0)    13704 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/screen.py
--rw-r--r--   0 root         (0) root         (0)     4814 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py
--rw-r--r--   0 root         (0) root         (0)    21685 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py
--rw-r--r--   0 root         (0) root         (0)     6019 2024-01-23 00:01:37.000000 ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/ports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/ports/_status/
--rw-r--r--   0 root         (0) root         (0)      507 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/ports/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/ports/available.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/ports/claimed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/ports/find_multiple/
--rw-r--r--   0 root         (0) root         (0)      631 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/ports/find_multiple/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/ports/find_multiple/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.882528 ships-1.2.6/fields/gardens/ships/process/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/multi/
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-23 00:49:41.000000 ships-1.2.6/fields/gardens/ships/process/multi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/multi/_status/
--rw-r--r--   0 root         (0) root         (0)      851 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/process/multi/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-01-23 03:58:21.000000 ships-1.2.6/fields/gardens/ships/process/multi/_status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/multi_2/
--rw-r--r--   0 root         (0) root         (0)     3733 2024-01-23 04:02:43.000000 ships-1.2.6/fields/gardens/ships/process/multi_2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/multi_2/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/multi_2/_status/2/
--rw-r--r--   0 root         (0) root         (0)      180 2024-01-22 23:55:08.000000 ships-1.2.6/fields/gardens/ships/process/multi_2/_status/2/script.py
--rw-r--r--   0 root         (0) root         (0)     1429 2024-01-23 04:15:28.000000 ships-1.2.6/fields/gardens/ships/process/multi_2/_status/2/status_2.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-01-23 03:59:33.000000 ships-1.2.6/fields/gardens/ships/process/multi_2/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/start/
--rw-r--r--   0 root         (0) root         (0)     1605 2024-01-23 04:06:55.000000 ships-1.2.6/fields/gardens/ships/process/start/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/start/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/start/_status/2/
--rw-r--r--   0 root         (0) root         (0)      160 2024-01-23 01:46:12.000000 ships-1.2.6/fields/gardens/ships/process/start/_status/2/script.py
--rw-r--r--   0 root         (0) root         (0)     1495 2024-01-23 04:15:44.000000 ships-1.2.6/fields/gardens/ships/process/start/_status/2/status_2.py
--rw-r--r--   0 root         (0) root         (0)     1169 2024-01-23 04:07:00.000000 ships-1.2.6/fields/gardens/ships/process/start/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships/process/start/parts/
--rw-r--r--   0 root         (0) root         (0)      916 2024-01-23 03:03:06.000000 ships-1.2.6/fields/gardens/ships/process/start/parts/awareness.py
--rw-r--r--   0 root         (0) root         (0)      486 2024-01-23 04:06:27.000000 ships-1.2.6/fields/gardens/ships/process/start/parts/returns.py
--rw-r--r--   0 root         (0) root         (0)       69 2023-12-19 05:34:10.000000 ships-1.2.6/fields/gardens/ships/revenue.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-12-19 05:32:53.000000 ships-1.2.6/fields/gardens/ships/ships.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 02:51:13.902528 ships-1.2.6/fields/gardens/ships.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1341 2024-04-07 02:51:13.000000 ships-1.2.6/fields/gardens/ships.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8517 2024-04-07 02:51:13.000000 ships-1.2.6/fields/gardens/ships.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 02:51:13.000000 ships-1.2.6/fields/gardens/ships.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       39 2024-04-07 02:51:13.000000 ships-1.2.6/fields/gardens/ships.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-07 02:51:13.000000 ships-1.2.6/fields/gardens/ships.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-07 02:51:13.000000 ships-1.2.6/fields/gardens/ships.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      714 2024-04-07 02:51:08.000000 ships-1.2.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1108 2024-03-30 19:19:57.000000 ships-1.2.6/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 02:51:13.902528 ships-1.2.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-04-16 02:28:14.389786 ships-1.2.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.321787 ships-1.2.7/fields/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.321787 ships-1.2.7/fields/gardens/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.333787 ships-1.2.7/fields/gardens/ships/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.333787 ships-1.2.7/fields/gardens/ships/AMLI/
+-rw-rw-r--   0 root         (0) root         (0)      104 2024-03-30 17:23:39.000000 ships-1.2.7/fields/gardens/ships/AMLI/AMLI.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.333787 ships-1.2.7/fields/gardens/ships/AMLI/LLM/
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-02-15 19:38:33.000000 ships-1.2.7/fields/gardens/ships/AMLI/LLM/LLM.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/Search/
+-rw-rw-r--   0 root         (0) root         (0)       44 2024-02-15 19:38:43.000000 ships-1.2.7/fields/gardens/ships/Search/Search.s.HTML
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-02-15 04:11:24.000000 ships-1.2.7/fields/gardens/ships/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/_clique/
+-rw-rw-r--   0 root         (0) root         (0)      547 2024-02-15 04:21:26.000000 ships-1.2.7/fields/gardens/ships/_clique/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/_license/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-12-16 19:52:14.000000 ships-1.2.7/fields/gardens/ships/_license/license.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/_status/
+-rw-r--r--   0 root         (0) root         (0)      198 2024-01-23 03:57:34.000000 ships-1.2.7/fields/gardens/ships/_status/ports.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-02-04 21:57:31.000000 ships-1.2.7/fields/gardens/ships/_status/status.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/business/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-11-22 19:02:46.000000 ships-1.2.7/fields/gardens/ships/business/business.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/business/decorators/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-11-22 19:10:51.000000 ships-1.2.7/fields/gardens/ships/business/decorators/decorators.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.337787 ships-1.2.7/fields/gardens/ships/business/decorators/examples/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-11-22 19:15:14.000000 ships-1.2.7/fields/gardens/ships/business/decorators/examples/example_1.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-11-22 19:09:40.000000 ships-1.2.7/fields/gardens/ships/business/decorators/examples/multiple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.321787 ships-1.2.7/fields/gardens/ships/cadence/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.341786 ships-1.2.7/fields/gardens/ships/cadence/UTC/
+-rw-rw-r--   0 root         (0) root         (0)        5 2023-08-24 19:13:50.000000 ships-1.2.7/fields/gardens/ships/cadence/UTC/UTC.r.HTML
+-rw-rw-r--   0 root         (0) root         (0)      958 2023-12-19 05:34:09.000000 ships-1.2.7/fields/gardens/ships/cadence/UTC/current.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.341786 ships-1.2.7/fields/gardens/ships/cadence/UTC/leap/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-24 19:08:54.000000 ships-1.2.7/fields/gardens/ships/cadence/UTC/leap/seconds.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-24 19:08:50.000000 ships-1.2.7/fields/gardens/ships/cadence/UTC/leap/years.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.341786 ships-1.2.7/fields/gardens/ships/cadence/UTC/month/
+-rw-rw-r--   0 root         (0) root         (0)      440 2023-12-19 05:34:09.000000 ships-1.2.7/fields/gardens/ships/cadence/UTC/month/strings.py
+-rw-rw-r--   0 root         (0) root         (0)      604 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cadence/UTC/status_current.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.341786 ships-1.2.7/fields/gardens/ships/cadence/filter/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-12-19 05:34:09.000000 ships-1.2.7/fields/gardens/ships/cadence/filter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.341786 ships-1.2.7/fields/gardens/ships/cadence/filter/_status/
+-rw-r--r--   0 root         (0) root         (0)      533 2023-12-19 05:34:09.000000 ships-1.2.7/fields/gardens/ships/cadence/filter/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-12-19 05:34:09.000000 ships-1.2.7/fields/gardens/ships/cadence/filter/_status/status_2.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-12-19 05:34:09.000000 ships-1.2.7/fields/gardens/ships/cadence/filter/_status/status_3.py
+-rw-r--r--   0 root         (0) root         (0)        2 2023-11-27 01:22:43.000000 ships-1.2.7/fields/gardens/ships/clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.341786 ships-1.2.7/fields/gardens/ships/coms/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-12-01 16:30:53.000000 ships-1.2.7/fields/gardens/ships/coms/coms.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.321787 ships-1.2.7/fields/gardens/ships/coms/protocols/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.345786 ships-1.2.7/fields/gardens/ships/coms/protocols/SSH/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-12-01 14:37:22.000000 ships-1.2.7/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.345786 ships-1.2.7/fields/gardens/ships/coms/protocols/SSL/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-12-01 21:53:45.000000 ships-1.2.7/fields/gardens/ships/coms/protocols/SSL/SSL.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.345786 ships-1.2.7/fields/gardens/ships/coms/wall/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-12-01 16:29:57.000000 ships-1.2.7/fields/gardens/ships/coms/wall/wall.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.345786 ships-1.2.7/fields/gardens/ships/cycle/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cycle/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      610 2024-04-09 19:03:39.000000 ships-1.2.7/fields/gardens/ships/cycle/cycle.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.345786 ships-1.2.7/fields/gardens/ships/cycle/loops/
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-04-09 18:50:19.000000 ships-1.2.7/fields/gardens/ships/cycle/loops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-11-12 17:53:20.000000 ships-1.2.7/fields/gardens/ships/cycle/loops/loops.s.HTML
+-rw-r--r--   0 root         (0) root         (0)      711 2023-12-19 05:47:03.000000 ships-1.2.7/fields/gardens/ships/cycle/loops/status_2.py
+-rw-r--r--   0 root         (0) root         (0)      622 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cycle/loops/status_3.py
+-rw-r--r--   0 root         (0) root         (0)      716 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cycle/loops/status_4.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/cycle/params/
+-rw-r--r--   0 root         (0) root         (0)      658 2023-11-12 18:07:23.000000 ships-1.2.7/fields/gardens/ships/cycle/params/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cycle/params/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cycle/params/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/cycle/params_2/
+-rw-r--r--   0 root         (0) root         (0)      940 2024-01-06 04:12:45.000000 ships-1.2.7/fields/gardens/ships/cycle/params_2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-12-28 20:22:31.000000 ships-1.2.7/fields/gardens/ships/cycle/params_2/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/cycle/presents/
+-rw-r--r--   0 root         (0) root         (0)      313 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/cycle/presents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/flow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/flow/demux_mux/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/flow/demux_mux/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/flow/demux_mux/_status/
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/flow/demux_mux/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/flow/demux_mux2/
+-rw-r--r--   0 root         (0) root         (0)      830 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/flow/demux_mux2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/flow/demux_mux2/_status/
+-rw-r--r--   0 root         (0) root         (0)      515 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/flow/demux_mux2/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-11-08 16:55:45.000000 ships-1.2.7/fields/gardens/ships/flow/flow.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/flow/simultaneous/
+-rw-rw-r--   0 root         (0) root         (0)     1402 2024-03-17 03:19:08.000000 ships-1.2.7/fields/gardens/ships/flow/simultaneous/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.325787 ships-1.2.7/fields/gardens/ships/formats/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/formats/ISO/
+-rw-r--r--   0 root         (0) root         (0)      919 2024-01-19 20:43:25.000000 ships-1.2.7/fields/gardens/ships/formats/ISO/ISO.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.325787 ships-1.2.7/fields/gardens/ships/glamour/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.349786 ships-1.2.7/fields/gardens/ships/glamour/UTF8/
+-rw-r--r--   0 root         (0) root         (0)     6927 2023-11-18 21:15:34.000000 ships-1.2.7/fields/gardens/ships/glamour/UTF8/one.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.353786 ships-1.2.7/fields/gardens/ships/insure/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/insure/equalities.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/insure/equality.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/insure/status_equalitites_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.325787 ships-1.2.7/fields/gardens/ships/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.353786 ships-1.2.7/fields/gardens/ships/modules/exceptions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.353786 ships-1.2.7/fields/gardens/ships/modules/exceptions/custom/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-11-29 22:52:11.000000 ships-1.2.7/fields/gardens/ships/modules/exceptions/custom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      445 2024-03-10 22:49:28.000000 ships-1.2.7/fields/gardens/ships/modules/exceptions/parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.353786 ships-1.2.7/fields/gardens/ships/modules/fasten/
+-rw-r--r--   0 root         (0) root         (0)      845 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/modules/fasten/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.353786 ships-1.2.7/fields/gardens/ships/modules/fasten/_status/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-10-31 18:06:14.000000 ships-1.2.7/fields/gardens/ships/modules/fasten/_status/example.py
+-rw-r--r--   0 root         (0) root         (0)      121 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/modules/fasten/_status/example_caller.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/modules/fasten/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.353786 ships-1.2.7/fields/gardens/ships/modules/import/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/modules/import/examples/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-11-28 05:02:32.000000 ships-1.2.7/fields/gardens/ships/modules/import/examples/example_1.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 04:57:58.000000 ships-1.2.7/fields/gardens/ships/modules/import/examples/example_1_module.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-11-30 01:01:28.000000 ships-1.2.7/fields/gardens/ships/modules/import/import.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/modules/print/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-11-27 01:32:02.000000 ships-1.2.7/fields/gardens/ships/modules/print/print.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/modules/string/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/modules/string/NLP/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-12-17 22:23:07.000000 ships-1.2.7/fields/gardens/ships/modules/string/NLP/NLP.s.HTML
+-rw-r--r--   0 root         (0) root         (0)      265 2023-11-12 18:56:01.000000 ships-1.2.7/fields/gardens/ships/modules/string/end_of_string_is.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/modules/string/sayings/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-12-17 22:25:39.000000 ships-1.2.7/fields/gardens/ships/modules/string/sayings/sayings.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/paths/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-12-01 04:01:32.000000 ships-1.2.7/fields/gardens/ships/paths/caller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/
+-rw-r--r--   0 root         (0) root         (0)     3453 2024-02-15 05:14:15.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.325787 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.325787 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.357786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:01:19.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_1/1.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:01:24.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_2/1.HTML
+-rw-r--r--   0 root         (0) root         (0)      587 2024-02-15 05:03:56.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.325787 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:12:57.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1/1.HTML
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:12:39.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:13:01.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/1/2.HTML
+-rw-r--r--   0 root         (0) root         (0)        0 2023-09-26 17:12:42.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/2.HTML
+-rw-r--r--   0 root         (0) root         (0)      682 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py
+-rw-rw-r--   0 root         (0) root         (0)        3 2024-02-15 04:09:56.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-12-03 23:10:11.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-12-03 23:10:11.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-12-03 23:10:11.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/get_directories.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-12-03 23:10:11.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/get_same_directories.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-12-03 21:57:50.000000 ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/is_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/deallocate/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/deallocate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.361786 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-04-07 02:50:44.000000 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/1/start/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/1/start/1/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/1/start/1/1.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-03-30 03:49:06.000000 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/2/start/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/2/start/1/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/2/start/1/1.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-10-13 23:54:40.000000 ships-1.2.7/fields/gardens/ships/paths/directory/equalize/equalize.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-04-12 21:58:19.000000 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-03-30 04:06:11.000000 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string/field.S.HTML
+-rw-r--r--   0 root         (0) root         (0)      115 2023-10-21 23:43:14.000000 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string/in_path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string_v2/
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-04-16 02:26:41.000000 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-03-30 04:06:11.000000 ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string_v2/field.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/for_each_path/
+-rw-r--r--   0 root         (0) root         (0)      781 2023-10-21 23:50:37.000000 ships-1.2.7/fields/gardens/ships/paths/directory/for_each_path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/rsync/
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/rsync/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.365786 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/
+-rw-rw-r--   0 root         (0) root         (0)      974 2024-03-30 18:50:21.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/DFS.py
+-rw-rw-r--   0 root         (0) root         (0)     2200 2024-03-30 18:22:06.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2032 2024-03-30 18:03:59.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1/1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_1/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_1/1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_symlink_to_1/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-14 00:40:16.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/symlink_to_symlink_to_1/1.py
+-rw-rw-r--   0 root         (0) root         (0)     3629 2024-03-30 19:04:59.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/2/
+-rw-rw-r--   0 root         (0) root         (0)     1020 2024-03-30 19:04:22.000000 ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/sense/
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/sense/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/sense/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/sense/_status/1/
+-rw-r--r--   0 root         (0) root         (0)      826 2024-03-30 05:18:51.000000 ships-1.2.7/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/size/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/size/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/directory/size/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/size/_status/1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/directory/size/_status/1/cryo/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-12-03 23:22:28.000000 ships-1.2.7/fields/gardens/ships/paths/directory/size/_status/1/cryo/hyper.HTML
+-rw-r--r--   0 root         (0) root         (0)      623 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/directory/size/_status/1/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/paths/files/scan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/files/scan/JSON/
+-rw-r--r--   0 root         (0) root         (0)      544 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/files/scan/JSON/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/files/scan/JSON/status/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/path/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/paths/path/relative.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.369786 ships-1.2.7/fields/gardens/ships/paths/variety/
+-rw-rw-r--   0 root         (0) root         (0)      396 2024-03-30 18:12:33.000000 ships-1.2.7/fields/gardens/ships/paths/variety/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/
+-rw-r--r--   0 root         (0) root         (0)    12177 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py
+-rw-r--r--   0 root         (0) root         (0)    13419 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/_async.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py
+-rw-r--r--   0 root         (0) root         (0)     3802 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13827 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/expect.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py
+-rw-r--r--   0 root         (0) root         (0)     6159 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py
+-rw-r--r--   0 root         (0) root         (0)    37382 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py
+-rw-r--r--   0 root         (0) root         (0)    24445 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py
+-rw-r--r--   0 root         (0) root         (0)     6629 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/run.py
+-rw-r--r--   0 root         (0) root         (0)    13704 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/screen.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py
+-rw-r--r--   0 root         (0) root         (0)    21685 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2024-01-23 00:01:37.000000 ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/ports/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/ports/_status/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/ports/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/ports/available.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/ports/claimed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/ports/find_multiple/
+-rw-r--r--   0 root         (0) root         (0)      631 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/ports/find_multiple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/ports/find_multiple/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.329787 ships-1.2.7/fields/gardens/ships/process/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/process/multi/
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-01-23 00:49:41.000000 ships-1.2.7/fields/gardens/ships/process/multi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/process/multi/_status/
+-rw-r--r--   0 root         (0) root         (0)      851 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/process/multi/_status/status_1.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-01-23 03:58:21.000000 ships-1.2.7/fields/gardens/ships/process/multi/_status/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.385786 ships-1.2.7/fields/gardens/ships/process/multi_2/
+-rw-r--r--   0 root         (0) root         (0)     3733 2024-01-23 04:02:43.000000 ships-1.2.7/fields/gardens/ships/process/multi_2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships/process/multi_2/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships/process/multi_2/_status/2/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-01-22 23:55:08.000000 ships-1.2.7/fields/gardens/ships/process/multi_2/_status/2/script.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2024-01-23 04:15:28.000000 ships-1.2.7/fields/gardens/ships/process/multi_2/_status/2/status_2.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-01-23 03:59:33.000000 ships-1.2.7/fields/gardens/ships/process/multi_2/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships/process/start/
+-rw-r--r--   0 root         (0) root         (0)     1605 2024-01-23 04:06:55.000000 ships-1.2.7/fields/gardens/ships/process/start/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships/process/start/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships/process/start/_status/2/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-01-23 01:46:12.000000 ships-1.2.7/fields/gardens/ships/process/start/_status/2/script.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-01-23 04:15:44.000000 ships-1.2.7/fields/gardens/ships/process/start/_status/2/status_2.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-01-23 04:07:00.000000 ships-1.2.7/fields/gardens/ships/process/start/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships/process/start/parts/
+-rw-r--r--   0 root         (0) root         (0)      916 2024-01-23 03:03:06.000000 ships-1.2.7/fields/gardens/ships/process/start/parts/awareness.py
+-rw-r--r--   0 root         (0) root         (0)      486 2024-01-23 04:06:27.000000 ships-1.2.7/fields/gardens/ships/process/start/parts/returns.py
+-rw-r--r--   0 root         (0) root         (0)       69 2023-12-19 05:34:10.000000 ships-1.2.7/fields/gardens/ships/revenue.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-12-19 05:32:53.000000 ships-1.2.7/fields/gardens/ships/ships.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 02:28:14.389786 ships-1.2.7/fields/gardens/ships.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-04-16 02:28:14.000000 ships-1.2.7/fields/gardens/ships.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8557 2024-04-16 02:28:14.000000 ships-1.2.7/fields/gardens/ships.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 02:28:14.000000 ships-1.2.7/fields/gardens/ships.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       39 2024-04-16 02:28:14.000000 ships-1.2.7/fields/gardens/ships.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-16 02:28:14.000000 ships-1.2.7/fields/gardens/ships.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 02:28:14.000000 ships-1.2.7/fields/gardens/ships.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      714 2024-04-16 02:28:00.000000 ships-1.2.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-03-30 19:19:57.000000 ships-1.2.7/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 02:28:14.389786 ships-1.2.7/setup.cfg
```

### Comparing `ships-1.2.6/PKG-INFO` & `ships-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ships
-Version: 1.2.6
+Version: 1.2.7
 Summary: Various calculator tools
 License: GPL 3.0
 Description-Content-Type: text/markdown
 Requires-Dist: bracelet
 Requires-Dist: rich
 Requires-Dist: psutil
 Requires-Dist: pyinotify
```

### Comparing `ships-1.2.6/fields/gardens/ships/__init__.py` & `ships-1.2.7/fields/gardens/ships/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/_clique/__init__.py` & `ships-1.2.7/fields/gardens/ships/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/_status/status.proc.py` & `ships-1.2.7/fields/gardens/ships/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/business/decorators/examples/example_1.py` & `ships-1.2.7/fields/gardens/ships/business/decorators/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cadence/UTC/current.py` & `ships-1.2.7/fields/gardens/ships/cadence/UTC/current.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cadence/UTC/status_current.py` & `ships-1.2.7/fields/gardens/ships/cadence/UTC/status_current.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cadence/filter/__init__.py` & `ships-1.2.7/fields/gardens/ships/cadence/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cadence/filter/_status/status_1.py` & `ships-1.2.7/fields/gardens/ships/cadence/filter/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cadence/filter/_status/status_2.py` & `ships-1.2.7/fields/gardens/ships/cadence/filter/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cadence/filter/_status/status_3.py` & `ships-1.2.7/fields/gardens/ships/cadence/filter/_status/status_3.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML` & `ships-1.2.7/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/loops/__init__.py` & `ships-1.2.7/fields/gardens/ships/cycle/loops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 			the "show" function doesn't raise an exception			
 
 
 	loop with the same parameters, each cycle
 '''
 
 '''
-
 import ships.cycle.loops as cycle_loops
 
 def show (* positionals, ** keywords):
 	print (positionals)
 	print (keywords)
 
 	return 99
```

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/loops/status_2.py` & `ships-1.2.7/fields/gardens/ships/cycle/loops/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/loops/status_3.py` & `ships-1.2.7/fields/gardens/ships/cycle/loops/status_3.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/loops/status_4.py` & `ships-1.2.7/fields/gardens/ships/cycle/loops/status_4.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/params/__init__.py` & `ships-1.2.7/fields/gardens/ships/cycle/params/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/params/status_2.py` & `ships-1.2.7/fields/gardens/ships/cycle/params/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/params_2/__init__.py` & `ships-1.2.7/fields/gardens/ships/cycle/params_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/cycle/params_2/status_1.py` & `ships-1.2.7/fields/gardens/ships/cycle/params_2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/flow/demux_mux/__init__.py` & `ships-1.2.7/fields/gardens/ships/flow/demux_mux/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/flow/demux_mux/_status/status_1.py` & `ships-1.2.7/fields/gardens/ships/flow/demux_mux/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/flow/demux_mux2/__init__.py` & `ships-1.2.7/fields/gardens/ships/flow/demux_mux2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/flow/demux_mux2/_status/status_1.py` & `ships-1.2.7/fields/gardens/ships/flow/demux_mux2/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/flow/simultaneous/__init__.py` & `ships-1.2.7/fields/gardens/ships/flow/simultaneous/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/formats/ISO/ISO.s.HTML` & `ships-1.2.7/fields/gardens/ships/formats/ISO/ISO.s.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/glamour/UTF8/one.HTML` & `ships-1.2.7/fields/gardens/ships/glamour/UTF8/one.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/insure/equalities.py` & `ships-1.2.7/fields/gardens/ships/insure/equalities.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/modules/fasten/__init__.py` & `ships-1.2.7/fields/gardens/ships/modules/fasten/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/modules/print/print.s.HTML` & `ships-1.2.7/fields/gardens/ships/modules/print/print.s.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/equalize/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/equalize/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 
 '''
+	use v2
+'''
+
+'''
 	Description:
 		Maybe this finds and replaces strings in the contents
 		of "files" in the glob...?
 '''
 
 '''
 	import ships.paths.directory.find_and_replace_string as find_and_replace_string
```

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,20 @@
 	glob.glob ('./[0-9].*')
 '''
 
 import glob
 import os.path
 import os
 import shutil
+import json
 
 import rich
 
+
+
 import ships.paths.directory.scan_tree as scan_tree
 import ships.paths.directory.scan_tree.DFS as DFS
 	
 from ships.paths.variety import path_variety
 
 def retrieve_paths (the_path):
 	paths_found = []
```

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/for_each_path/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/for_each_path/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/rsync/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/rsync/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/DFS.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/DFS.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/sense/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/sense/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/size/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/size/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/directory/size/_status/1/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/directory/size/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/files/scan/JSON/__init__.py` & `ships-1.2.7/fields/gardens/ships/paths/files/scan/JSON/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py` & `ships-1.2.7/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/_async.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/_async.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/expect.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/expect.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/run.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/run.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/screen.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/screen.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/pexpect_4_9_0_copy/utils.py` & `ships-1.2.7/fields/gardens/ships/pexpect_4_9_0_copy/utils.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/ports/available.py` & `ships-1.2.7/fields/gardens/ships/ports/available.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/ports/find_multiple/__init__.py` & `ships-1.2.7/fields/gardens/ships/ports/find_multiple/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/multi/__init__.py` & `ships-1.2.7/fields/gardens/ships/process/multi/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/multi/_status/status_1.py` & `ships-1.2.7/fields/gardens/ships/process/multi/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/multi/_status/status_2.py` & `ships-1.2.7/fields/gardens/ships/process/multi/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/multi_2/__init__.py` & `ships-1.2.7/fields/gardens/ships/process/multi_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/multi_2/_status/2/status_2.py` & `ships-1.2.7/fields/gardens/ships/process/multi_2/_status/2/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/multi_2/_status/status_1.py` & `ships-1.2.7/fields/gardens/ships/process/multi_2/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/start/__init__.py` & `ships-1.2.7/fields/gardens/ships/process/start/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/start/_status/2/status_2.py` & `ships-1.2.7/fields/gardens/ships/process/start/_status/2/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/start/_status/status_1.py` & `ships-1.2.7/fields/gardens/ships/process/start/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships/process/start/parts/awareness.py` & `ships-1.2.7/fields/gardens/ships/process/start/parts/awareness.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.6/fields/gardens/ships.egg-info/PKG-INFO` & `ships-1.2.7/fields/gardens/ships.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ships
-Version: 1.2.6
+Version: 1.2.7
 Summary: Various calculator tools
 License: GPL 3.0
 Description-Content-Type: text/markdown
 Requires-Dist: bracelet
 Requires-Dist: rich
 Requires-Dist: psutil
 Requires-Dist: pyinotify
```

### Comparing `ships-1.2.6/fields/gardens/ships.egg-info/SOURCES.txt` & `ships-1.2.7/fields/gardens/ships.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 fields/gardens/ships/cadence/filter/_status/status_2.py
 fields/gardens/ships/cadence/filter/_status/status_3.py
 fields/gardens/ships/coms/coms.r.HTML
 fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML
 fields/gardens/ships/coms/protocols/SSL/SSL.r.HTML
 fields/gardens/ships/coms/wall/wall.r.HTML
 fields/gardens/ships/cycle/__init__.py
+fields/gardens/ships/cycle/cycle.S.HTML
 fields/gardens/ships/cycle/loops/__init__.py
 fields/gardens/ships/cycle/loops/loops.s.HTML
 fields/gardens/ships/cycle/loops/status_2.py
 fields/gardens/ships/cycle/loops/status_3.py
 fields/gardens/ships/cycle/loops/status_4.py
 fields/gardens/ships/cycle/params/__init__.py
 fields/gardens/ships/cycle/params/status_1.py
```

### Comparing `ships-1.2.6/pyproject.toml` & `ships-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ships"
-version = "1.2.6"
+version = "1.2.7"
 description = "Various calculator tools"
 
 license = { text = "GPL 3.0" }
 
 readme = "readme.md"
 dependencies = [
 	'bracelet',
```

### Comparing `ships-1.2.6/readme.md` & `ships-1.2.7/readme.md`

 * *Files identical despite different names*

