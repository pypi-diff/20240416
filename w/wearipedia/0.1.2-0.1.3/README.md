# Comparing `tmp/wearipedia-0.1.2.tar.gz` & `tmp/wearipedia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wearipedia-0.1.2.tar", max compression
+gzip compressed data, was "wearipedia-0.1.3.tar", max compression
```

## Comparing `wearipedia-0.1.2.tar` & `wearipedia-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,89 @@
--rw-r--r--   0        0        0     1097 2023-02-15 01:13:22.238689 wearipedia-0.1.2/LICENSE
--rw-r--r--   0        0        0     5460 2023-02-15 01:13:22.238829 wearipedia-0.1.2/README.md
--rw-r--r--   0        0        0     3845 2023-02-15 01:13:36.298245 wearipedia-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5766 2023-02-15 01:13:22.294009 wearipedia-0.1.2/wearipedia/__init__.py
--rw-r--r--   0        0        0     1497 2023-02-15 01:13:22.294092 wearipedia-0.1.2/wearipedia/__main__.py
--rw-r--r--   0        0        0     5346 2023-02-15 01:13:22.294185 wearipedia-0.1.2/wearipedia/cl_parser.py
--rw-r--r--   0        0        0      189 2023-02-15 01:13:22.294251 wearipedia-0.1.2/wearipedia/constants.py
--rw-r--r--   0        0        0      152 2023-02-15 01:13:22.294342 wearipedia-0.1.2/wearipedia/devices/__init__.py
--rw-r--r--   0        0        0     7825 2023-02-15 01:13:22.294430 wearipedia-0.1.2/wearipedia/devices/device.py
--rw-r--r--   0        0        0       23 2023-02-15 01:13:22.294515 wearipedia-0.1.2/wearipedia/devices/dexcom/__init__.py
--rw-r--r--   0        0        0     3404 2023-02-15 01:13:22.294613 wearipedia-0.1.2/wearipedia/devices/dexcom/pro_cgm.py
--rw-r--r--   0        0        0     3343 2023-02-15 01:13:22.294678 wearipedia-0.1.2/wearipedia/devices/dexcom/pro_cgm_fetch.py
--rw-r--r--   0        0        0     2599 2023-02-15 01:13:22.294780 wearipedia-0.1.2/wearipedia/devices/dexcom/pro_cgm_gen.py
--rw-r--r--   0        0        0     6278 2023-02-15 01:13:22.294904 wearipedia-0.1.2/wearipedia/devices/dreem/dreem_fetch.py
--rw-r--r--   0        0        0        6 2023-02-15 01:13:22.294965 wearipedia-0.1.2/wearipedia/devices/dreem/dreem_gen.py
--rw-r--r--   0        0        0     2165 2023-02-15 01:13:22.295045 wearipedia-0.1.2/wearipedia/devices/dreem/headband_2.py
--rw-r--r--   0        0        0        0 2023-02-15 01:13:22.295113 wearipedia-0.1.2/wearipedia/devices/fitbit/__init__.py
--rw-r--r--   0        0        0       24 2023-02-15 01:13:22.295251 wearipedia-0.1.2/wearipedia/devices/garmin/__init__.py
--rw-r--r--   0        0        0     4103 2023-02-15 01:13:22.295342 wearipedia-0.1.2/wearipedia/devices/garmin/fenix_7s.py
--rw-r--r--   0        0        0     2665 2023-02-15 01:13:22.295452 wearipedia-0.1.2/wearipedia/devices/garmin/fenix_fetch.py
--rw-r--r--   0        0        0    16848 2023-02-15 01:13:22.295591 wearipedia-0.1.2/wearipedia/devices/garmin/fenix_gen.py
--rw-r--r--   0        0        0        0 2023-02-15 01:13:22.295672 wearipedia-0.1.2/wearipedia/devices/oura/ring_3.py
--rw-r--r--   0        0        0       28 2023-02-15 01:13:22.295760 wearipedia-0.1.2/wearipedia/devices/polar/__init__.py
--rw-r--r--   0        0        0     2181 2023-02-15 01:13:22.295850 wearipedia-0.1.2/wearipedia/devices/polar/verity_gen.py
--rw-r--r--   0        0        0     3324 2023-02-15 01:13:22.295941 wearipedia-0.1.2/wearipedia/devices/polar/verity_get.py
--rw-r--r--   0        0        0     2887 2023-02-15 01:13:22.296004 wearipedia-0.1.2/wearipedia/devices/polar/verity_sense.py
--rw-r--r--   0        0        0       23 2023-02-15 01:13:22.296087 wearipedia-0.1.2/wearipedia/devices/whoop/__init__.py
--rw-r--r--   0        0        0     5438 2023-02-15 01:13:22.296172 wearipedia-0.1.2/wearipedia/devices/whoop/whoop_4.py
--rw-r--r--   0        0        0     6376 2023-02-15 01:13:22.296276 wearipedia-0.1.2/wearipedia/devices/whoop/whoop_gen.py
--rw-r--r--   0        0        0     2718 2023-02-15 01:13:22.296357 wearipedia-0.1.2/wearipedia/devices/whoop/whoop_user.py
--rw-r--r--   0        0        0       73 2023-02-15 01:13:22.296440 wearipedia-0.1.2/wearipedia/devices/withings/__init__.py
--rw-r--r--   0        0        0     2858 2023-02-15 01:13:22.296499 wearipedia-0.1.2/wearipedia/devices/withings/bodyplus.py
--rw-r--r--   0        0        0     3572 2023-02-15 01:13:22.296581 wearipedia-0.1.2/wearipedia/devices/withings/scanwatch.py
--rw-r--r--   0        0        0     1943 2023-02-15 01:13:22.296640 wearipedia-0.1.2/wearipedia/devices/withings/sleepmat.py
--rw-r--r--   0        0        0     2807 2023-02-15 01:13:22.296701 wearipedia-0.1.2/wearipedia/devices/withings/withings_authenticate.py
--rw-r--r--   0        0        0     9067 2023-02-15 01:13:22.296786 wearipedia-0.1.2/wearipedia/devices/withings/withings_extract.py
--rw-r--r--   0        0        0     8254 2023-02-15 01:13:22.296900 wearipedia-0.1.2/wearipedia/devices/withings/withings_gen.py
--rw-r--r--   0        0        0     1875 2023-02-15 01:13:22.296970 wearipedia-0.1.2/wearipedia/utils.py
--rw-r--r--   0        0        0     6830 1970-01-01 00:00:00.000000 wearipedia-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-02-21 19:37:53.150098 wearipedia-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4129 2024-04-16 07:07:16.377993 wearipedia-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5565 2023-02-21 19:37:53.151098 wearipedia-0.1.3/README.md
+-rw-r--r--   0        0        0     7849 2024-04-16 03:21:46.463743 wearipedia-0.1.3/wearipedia/__init__.py
+-rw-r--r--   0        0        0     1564 2023-02-21 19:37:53.262103 wearipedia-0.1.3/wearipedia/__main__.py
+-rw-r--r--   0        0        0     5501 2023-02-21 19:37:53.262103 wearipedia-0.1.3/wearipedia/cl_parser.py
+-rw-r--r--   0        0        0      201 2023-02-21 19:37:53.263102 wearipedia-0.1.3/wearipedia/constants.py
+-rw-r--r--   0        0        0      330 2024-04-14 05:56:50.776076 wearipedia-0.1.3/wearipedia/devices/__init__.py
+-rw-r--r--   0        0        0       26 2023-10-16 06:28:41.698622 wearipedia-0.1.3/wearipedia/devices/apple/__init__.py
+-rw-r--r--   0        0        0     7888 2023-10-16 06:28:41.704620 wearipedia-0.1.3/wearipedia/devices/apple/apple_gen.py
+-rw-r--r--   0        0        0     2926 2023-10-16 06:28:41.717625 wearipedia-0.1.3/wearipedia/devices/apple/healthkit.py
+-rw-r--r--   0        0        0       20 2024-04-14 05:56:50.786576 wearipedia-0.1.3/wearipedia/devices/biostrap/__init__.py
+-rw-r--r--   0        0        0     5448 2024-04-14 05:56:50.800601 wearipedia-0.1.3/wearipedia/devices/biostrap/evo.py
+-rw-r--r--   0        0        0     8409 2024-04-14 05:56:50.813595 wearipedia-0.1.3/wearipedia/devices/biostrap/evo_fetch.py
+-rw-r--r--   0        0        0    11541 2024-04-14 05:56:50.826599 wearipedia-0.1.3/wearipedia/devices/biostrap/evo_gen.py
+-rw-r--r--   0        0        0       29 2024-01-16 00:17:28.123107 wearipedia-0.1.3/wearipedia/devices/coros/__init__.py
+-rw-r--r--   0        0        0     3714 2024-01-16 00:17:28.124105 wearipedia-0.1.3/wearipedia/devices/coros/coros_pace_2.py
+-rw-r--r--   0        0        0     3580 2024-01-16 00:17:28.125105 wearipedia-0.1.3/wearipedia/devices/coros/coros_pace_2_fetch.py
+-rw-r--r--   0        0        0    12367 2024-01-16 00:17:28.125105 wearipedia-0.1.3/wearipedia/devices/coros/coros_pace_2_gen.py
+-rw-r--r--   0        0        0       27 2023-10-16 06:28:41.795806 wearipedia-0.1.3/wearipedia/devices/cronometer/__init__.py
+-rw-r--r--   0        0        0     5099 2023-10-16 06:28:41.796808 wearipedia-0.1.3/wearipedia/devices/cronometer/cronometer.py
+-rw-r--r--   0        0        0     3774 2024-03-07 20:05:14.863862 wearipedia-0.1.3/wearipedia/devices/cronometer/cronometer_fetch.py
+-rw-r--r--   0        0        0     7794 2023-10-16 06:28:41.993471 wearipedia-0.1.3/wearipedia/devices/cronometer/cronometer_synthetic.py
+-rw-r--r--   0        0        0    20529 2023-10-16 06:28:41.995471 wearipedia-0.1.3/wearipedia/devices/cronometer/servings.csv
+-rw-r--r--   0        0        0     8023 2023-11-30 23:30:23.652399 wearipedia-0.1.3/wearipedia/devices/device.py
+-rw-r--r--   0        0        0       24 2023-02-21 19:37:53.264102 wearipedia-0.1.3/wearipedia/devices/dexcom/__init__.py
+-rw-r--r--   0        0        0     3509 2023-02-21 19:37:53.265103 wearipedia-0.1.3/wearipedia/devices/dexcom/pro_cgm.py
+-rw-r--r--   0        0        0     3449 2023-02-21 19:37:53.266104 wearipedia-0.1.3/wearipedia/devices/dexcom/pro_cgm_fetch.py
+-rw-r--r--   0        0        0     2687 2023-02-21 19:37:53.266104 wearipedia-0.1.3/wearipedia/devices/dexcom/pro_cgm_gen.py
+-rw-r--r--   0        0        0     6506 2023-02-21 19:37:53.267103 wearipedia-0.1.3/wearipedia/devices/dreem/dreem_fetch.py
+-rw-r--r--   0        0        0        7 2023-02-21 19:37:53.267103 wearipedia-0.1.3/wearipedia/devices/dreem/dreem_gen.py
+-rw-r--r--   0        0        0     2241 2023-02-21 19:37:53.268104 wearipedia-0.1.3/wearipedia/devices/dreem/headband_2.py
+-rw-r--r--   0        0        0       61 2024-01-16 00:17:28.127105 wearipedia-0.1.3/wearipedia/devices/fitbit/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-16 03:21:46.465739 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_authenticate.py
+-rw-r--r--   0        0        0     2356 2024-01-16 00:17:28.128610 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_charge4_fetch.py
+-rw-r--r--   0        0        0     4536 2024-04-16 03:21:46.475675 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_charge_4.py
+-rw-r--r--   0        0        0     8037 2024-04-16 03:21:46.486191 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_charge_4_gen.py
+-rw-r--r--   0        0        0     5125 2024-04-16 03:21:46.496037 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_sense.py
+-rw-r--r--   0        0        0     2782 2024-04-16 03:21:46.497039 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_sense_fetch.py
+-rw-r--r--   0        0        0    14326 2024-04-16 03:21:46.498554 wearipedia-0.1.3/wearipedia/devices/fitbit/fitbit_sense_gen.py
+-rw-r--r--   0        0        0       25 2023-02-21 19:37:53.269104 wearipedia-0.1.3/wearipedia/devices/garmin/__init__.py
+-rw-r--r--   0        0        0     4218 2024-04-14 05:56:50.828602 wearipedia-0.1.3/wearipedia/devices/garmin/fenix_7s.py
+-rw-r--r--   0        0        0     2754 2024-04-14 05:56:50.829595 wearipedia-0.1.3/wearipedia/devices/garmin/fenix_fetch.py
+-rw-r--r--   0        0        0    17268 2024-04-14 05:56:50.831596 wearipedia-0.1.3/wearipedia/devices/garmin/fenix_gen.py
+-rw-r--r--   0        0        0       26 2023-10-16 06:28:42.002465 wearipedia-0.1.3/wearipedia/devices/google/__init__.py
+-rw-r--r--   0        0        0     8314 2023-10-16 06:28:42.003467 wearipedia-0.1.3/wearipedia/devices/google/googlefit.py
+-rw-r--r--   0        0        0     4280 2023-10-16 06:28:42.011528 wearipedia-0.1.3/wearipedia/devices/google/googlefitness_fetch.py
+-rw-r--r--   0        0        0    27626 2023-10-16 06:28:42.015529 wearipedia-0.1.3/wearipedia/devices/google/googlefitness_synthetic.py
+-rw-r--r--   0        0        0       29 2024-03-07 20:05:14.894632 wearipedia-0.1.3/wearipedia/devices/myfitnesspal/__init__.py
+-rw-r--r--   0        0        0     4873 2024-03-07 20:05:14.895639 wearipedia-0.1.3/wearipedia/devices/myfitnesspal/myfitnesspal.py
+-rw-r--r--   0        0        0     6149 2024-03-07 20:05:14.903806 wearipedia-0.1.3/wearipedia/devices/myfitnesspal/myfitnesspal_fetch.py
+-rw-r--r--   0        0        0    35070 2024-03-07 20:05:14.904804 wearipedia-0.1.3/wearipedia/devices/myfitnesspal/myfitnesspal_syn_data.json
+-rw-r--r--   0        0        0     7747 2024-03-07 20:05:14.916859 wearipedia-0.1.3/wearipedia/devices/myfitnesspal/myfitnesspal_synthetic.py
+-rw-r--r--   0        0        0       20 2023-05-19 04:50:14.696181 wearipedia-0.1.3/wearipedia/devices/nutrisense/__init__.py
+-rw-r--r--   0        0        0     5301 2024-04-14 05:56:50.846628 wearipedia-0.1.3/wearipedia/devices/nutrisense/cgm.py
+-rw-r--r--   0        0        0     4840 2023-05-19 04:50:14.697181 wearipedia-0.1.3/wearipedia/devices/nutrisense/cgm_fetch.py
+-rw-r--r--   0        0        0     5951 2024-04-14 05:56:50.860603 wearipedia-0.1.3/wearipedia/devices/nutrisense/cgm_gen.py
+-rw-r--r--   0        0        0       27 2024-01-16 00:17:28.136619 wearipedia-0.1.3/wearipedia/devices/oura/__init__.py
+-rw-r--r--   0        0        0     3599 2024-04-16 03:21:46.500571 wearipedia-0.1.3/wearipedia/devices/oura/oura_ring3.py
+-rw-r--r--   0        0        0      470 2024-01-16 00:17:28.137620 wearipedia-0.1.3/wearipedia/devices/oura/oura_ring3_authenticate.py
+-rw-r--r--   0        0        0     4051 2024-03-07 19:28:21.732874 wearipedia-0.1.3/wearipedia/devices/oura/oura_ring3_fetch.py
+-rw-r--r--   0        0        0    14257 2024-04-16 03:21:46.502577 wearipedia-0.1.3/wearipedia/devices/oura/oura_ring3_gen.py
+-rw-r--r--   0        0        0       73 2023-12-12 04:47:18.835880 wearipedia-0.1.3/wearipedia/devices/polar/__init__.py
+-rw-r--r--   0        0        0     4406 2023-12-12 04:47:18.841892 wearipedia-0.1.3/wearipedia/devices/polar/h10.py
+-rw-r--r--   0        0        0     3519 2024-03-07 20:05:14.941007 wearipedia-0.1.3/wearipedia/devices/polar/h10_gen.py
+-rw-r--r--   0        0        0     6196 2023-12-12 04:47:18.857153 wearipedia-0.1.3/wearipedia/devices/polar/polar_get.py
+-rw-r--r--   0        0        0     5077 2023-10-16 06:28:42.059063 wearipedia-0.1.3/wearipedia/devices/polar/vantage.py
+-rw-r--r--   0        0        0     3620 2023-10-16 06:28:42.061061 wearipedia-0.1.3/wearipedia/devices/polar/vantage_fetch.py
+-rw-r--r--   0        0        0    10606 2023-10-16 06:28:42.074063 wearipedia-0.1.3/wearipedia/devices/polar/vantage_synthetic.py
+-rw-r--r--   0        0        0     2465 2024-03-07 20:05:14.948011 wearipedia-0.1.3/wearipedia/devices/polar/verity_gen.py
+-rw-r--r--   0        0        0     2975 2023-12-12 04:47:18.871187 wearipedia-0.1.3/wearipedia/devices/polar/verity_sense.py
+-rw-r--r--   0        0        0       23 2023-10-16 06:28:42.078061 wearipedia-0.1.3/wearipedia/devices/strava/__init__.py
+-rw-r--r--   0        0        0     8527 2024-03-07 20:05:14.956032 wearipedia-0.1.3/wearipedia/devices/strava/strava.py
+-rw-r--r--   0        0        0     3199 2024-03-07 20:05:14.964023 wearipedia-0.1.3/wearipedia/devices/strava/strava_fetch.py
+-rw-r--r--   0        0        0     6263 2024-03-07 20:05:14.971611 wearipedia-0.1.3/wearipedia/devices/strava/strava_syn_gen.py
+-rw-r--r--   0        0        0     1666 2024-03-07 20:05:14.978065 wearipedia-0.1.3/wearipedia/devices/strava/strava_syn_gen_streams.py
+-rw-r--r--   0        0        0       24 2023-02-21 19:37:53.274103 wearipedia-0.1.3/wearipedia/devices/whoop/__init__.py
+-rw-r--r--   0        0        0     5595 2024-04-14 05:56:50.862596 wearipedia-0.1.3/wearipedia/devices/whoop/whoop_4.py
+-rw-r--r--   0        0        0     6539 2024-04-14 05:56:50.863632 wearipedia-0.1.3/wearipedia/devices/whoop/whoop_gen.py
+-rw-r--r--   0        0        0     2808 2023-02-21 19:37:53.276104 wearipedia-0.1.3/wearipedia/devices/whoop/whoop_user.py
+-rw-r--r--   0        0        0       76 2023-02-21 19:37:53.276104 wearipedia-0.1.3/wearipedia/devices/withings/__init__.py
+-rw-r--r--   0        0        0     2945 2023-02-21 19:37:53.277099 wearipedia-0.1.3/wearipedia/devices/withings/bodyplus.py
+-rw-r--r--   0        0        0     3679 2023-02-21 19:37:53.278103 wearipedia-0.1.3/wearipedia/devices/withings/scanwatch.py
+-rw-r--r--   0        0        0     2011 2023-02-21 19:37:53.278103 wearipedia-0.1.3/wearipedia/devices/withings/sleepmat.py
+-rw-r--r--   0        0        0     2938 2023-02-28 23:06:39.529579 wearipedia-0.1.3/wearipedia/devices/withings/withings_authenticate.py
+-rw-r--r--   0        0        0     9337 2023-02-21 19:37:53.279103 wearipedia-0.1.3/wearipedia/devices/withings/withings_extract.py
+-rw-r--r--   0        0        0     8519 2023-02-21 19:37:53.280104 wearipedia-0.1.3/wearipedia/devices/withings/withings_gen.py
+-rw-r--r--   0        0        0     1949 2023-02-21 19:37:53.280104 wearipedia-0.1.3/wearipedia/utils.py
+-rw-r--r--   0        0        0     6938 1970-01-01 00:00:00.000000 wearipedia-0.1.3/PKG-INFO
```

### Comparing `wearipedia-0.1.2/LICENSE` & `wearipedia-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-Copyright (c) 2022 The Stanford Wearipedia Project
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
-OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+Copyright (c) 2022 The Stanford Wearipedia Project
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
+OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `wearipedia-0.1.2/README.md` & `wearipedia-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-# wearipedia
-
-<div align="center">
-
-[![Build status](https://github.com/Stanford-Health/wearipedia/workflows/build/badge.svg?branch=master&event=push)](https://github.com/Stanford-Health/wearipedia/actions?query=workflow%3Abuild)
-[![Python Version](https://img.shields.io/pypi/pyversions/wearipedia.svg)](https://pypi.org/project/wearipedia/)
-[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Stanford-Health/wearipedia/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Stanford-Health/wearipedia/blob/master/.pre-commit-config.yaml)
-[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Stanford-Health/wearipedia/releases)
-[![License](https://img.shields.io/github/license/Stanford-Health/wearipedia)](https://github.com/Stanford-Health/wearipedia/blob/master/LICENSE)
-![Coverage Report](assets/images/coverage.svg)
-
-</div>
-
-<h3 align="center">
-    <p>A one-stop shop for wearable device data extraction and simulation</p>
-</h3>
-
-Wearipedia provides a one-stop shop for accessing and extracting data from wearable devices.
-
-Data from these devices may be used for:
-
-* Clinical research
-* Personal health monitoring
-* Health coaching
-* Health product development
-* Wearable device development
-
-Wearipedia is developed and maintained by the [Snyder Lab](https://med.stanford.edu/snyderlab.html) at the Stanford University.
-
-## Accessing data from wearable devices
-
-The data from these devices is accessed using an easy-to-use API. In order to use this API, you will need to import the `wearipedia` module:
-
-```python
-import wearipedia
-```
-
-Once you have imported the `wearipedia` module, accessing data from any wearable device is as easy as:
-
-```python
-device = wearipedia.get_device("whoop/whoop_4")
-device.authenticate({"email": "joesmith@gmail.com", "password": "foobar"})
-
-# data is a DataFrame
-data = device.get_data("metrics")
-```
-
-If you don't have access to your device, or need to demo data from a device without revealing your sensitive data or getting a device yourself, you can generate synthetic data, as shown below:
-
-```python
-device = wearipedia.get_device("whoop/whoop_4")
-
-# data is an automatically generated DataFrame
-data = device.get_data("metrics")
-```
-
-and you're done!
-
-## Installing
-
-The easiest way to install wearipedia is to use pip:
-
-`pip install wearipedia`
-
-We currently support Python 3.7, 3.8, and 3.9.
-
-## Supported Devices
-
-Wearipedia supports the following devices:
-
-| Company | Model Name | Description | Example Notebook | Kinds of Data Available | Unique name |
-|---|---|---|---|---|---|
-| [Whoop](https://www.whoop.com/) | Whoop | The WHOOP 4.0 strap tracks sleep and activity data. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/whoop/Example%20Notebook.ipynb) | cycles, hr. | `whoop/whoop_4` |
-| [Garmin](https://www.garmin.com/en-US) | Fenix 7S | The Garmin Fenix 7S is a watch that activity data. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/garmin/Example%20Notebook.ipynb) |  dates, steps, hrs, brpms. | `garmin/fenix_7s` |
-| [Dexcom](https://www.dexcom.com/) | Pro CGM | The Dexcom Pro CGM wearable device tracks blood sugar levels. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/dexcom/Example%20Notebook.ipynb) |  dataframe. | `dexcom/pro_cgm` |
-| [Withings](https://www.withings.com) | Body+ | The Withings Body+ is a smart scale that tracks weight and other metrics (body fat %). | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/withings/Example%20Notebook.ipynb) | measurements. | `withings/bodyplus` |
-| [Withings](https://www.withings.com) | ScanWatch | The Withings ScanWatch wearable device tracks sleep and activity data. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/withings/Example%20Notebook.ipynb) | heart_rates, sleeps. | `withings/scanwatch` |
-
-## Documentation
-
-For more information on how to use wearipedia, please refer to our [documentation](https://wearipedia.readthedocs.io).
-
-## Citing
-
-A paper is in progress!
-
-## Disclaimer
-
-This project is currently in *alpha*. This means that test coverage is limited, and the codebase is still really a prototype. Moreover, the API is unstable, as we are still rapidly iterating on it. Expect for most things to work, but also small bugs, rough edges, and sparse documentation.
-
-## Contributing
-
-As Wearipedia is still at an early stage, we are not yet accepting contributions from the broader community. Once Wearipedia reaches its first stable release, we will begin accepting contributions.
-
-## License
-
-Wearipedia is released under the MIT license.
-
-## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
-
-This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
+# wearipedia
+
+<div align="center">
+
+[![Build status](https://github.com/Stanford-Health/wearipedia/workflows/build/badge.svg?branch=master&event=push)](https://github.com/Stanford-Health/wearipedia/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/wearipedia.svg)](https://pypi.org/project/wearipedia/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Stanford-Health/wearipedia/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Stanford-Health/wearipedia/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Stanford-Health/wearipedia/releases)
+[![License](https://img.shields.io/github/license/Stanford-Health/wearipedia)](https://github.com/Stanford-Health/wearipedia/blob/master/LICENSE)
+![Coverage Report](assets/images/coverage.svg)
+
+</div>
+
+<h3 align="center">
+    <p>A one-stop shop for wearable device data extraction and simulation</p>
+</h3>
+
+Wearipedia provides a one-stop shop for accessing and extracting data from wearable devices.
+
+Data from these devices may be used for:
+
+* Clinical research
+* Personal health monitoring
+* Health coaching
+* Health product development
+* Wearable device development
+
+Wearipedia is developed and maintained by the [Snyder Lab](https://med.stanford.edu/snyderlab.html) at the Stanford University.
+
+## Accessing data from wearable devices
+
+The data from these devices is accessed using an easy-to-use API. In order to use this API, you will need to import the `wearipedia` module:
+
+```python
+import wearipedia
+```
+
+Once you have imported the `wearipedia` module, accessing data from any wearable device is as easy as:
+
+```python
+device = wearipedia.get_device("whoop/whoop_4")
+device.authenticate({"email": "joesmith@gmail.com", "password": "foobar"})
+
+# data is a DataFrame
+data = device.get_data("metrics")
+```
+
+If you don't have access to your device, or need to demo data from a device without revealing your sensitive data or getting a device yourself, you can generate synthetic data, as shown below:
+
+```python
+device = wearipedia.get_device("whoop/whoop_4")
+
+# data is an automatically generated DataFrame
+data = device.get_data("metrics")
+```
+
+and you're done!
+
+## Installing
+
+The easiest way to install wearipedia is to use pip:
+
+`pip install wearipedia`
+
+We currently support Python 3.7, 3.8, and 3.9.
+
+## Supported Devices
+
+Wearipedia supports the following devices:
+
+| Company | Model Name | Description | Example Notebook | Kinds of Data Available | Unique name |
+|---|---|---|---|---|---|
+| [Whoop](https://www.whoop.com/) | Whoop | The WHOOP 4.0 strap tracks sleep and activity data. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/whoop/Example%20Notebook.ipynb) | cycles, hr. | `whoop/whoop_4` |
+| [Garmin](https://www.garmin.com/en-US) | Fenix 7S | The Garmin Fenix 7S is a watch that activity data. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/garmin/Example%20Notebook.ipynb) |  dates, steps, hrs, brpms. | `garmin/fenix_7s` |
+| [Dexcom](https://www.dexcom.com/) | Pro CGM | The Dexcom Pro CGM wearable device tracks blood sugar levels. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/dexcom/Example%20Notebook.ipynb) |  dataframe. | `dexcom/pro_cgm` |
+| [Withings](https://www.withings.com) | Body+ | The Withings Body+ is a smart scale that tracks weight and other metrics (body fat %). | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/withings/Example%20Notebook.ipynb) | measurements. | `withings/bodyplus` |
+| [Withings](https://www.withings.com) | ScanWatch | The Withings ScanWatch wearable device tracks sleep and activity data. | [Notebook](https://github.com/snyder-lab/wearipedia/blob/master/notebooks/withings/Example%20Notebook.ipynb) | heart_rates, sleeps. | `withings/scanwatch` |
+
+## Documentation
+
+For more information on how to use wearipedia, please refer to our [documentation](https://wearipedia.readthedocs.io).
+
+## Citing
+
+A paper is in progress!
+
+## Disclaimer
+
+This project is currently in *alpha*. This means that test coverage is limited, and the codebase is still really a prototype. Moreover, the API is unstable, as we are still rapidly iterating on it. Expect for most things to work, but also small bugs, rough edges, and sparse documentation.
+
+## Contributing
+
+As Wearipedia is still at an early stage, we are not yet accepting contributions from the broader community. Once Wearipedia reaches its first stable release, we will begin accepting contributions.
+
+## License
+
+Wearipedia is released under the MIT license.
+
+## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
+
+This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
```

### Comparing `wearipedia-0.1.2/pyproject.toml` & `wearipedia-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,157 +1,165 @@
-# Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
-[build-system]
-requires = ["poetry_core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry]
-name = "wearipedia"
-version = "0.1.2"
-description = "Wearable data for all"
-readme = "README.md"
-authors = ["The Stanford Wearipedia Project <arjo@stanford.edu>"]
-license = "MIT"
-repository = "https://github.com/Stanford-Health/wearipedia"
-homepage = "http://wearipedia.com"
-
-# Keywords description https://python-poetry.org/docs/pyproject/#keywords
-keywords = []  #! Update me
-
-# Pypi classifiers: https://pypi.org/classifiers/
-classifiers = [  #! Update me
-  "Development Status :: 3 - Alpha",
-  "Intended Audience :: Developers",
-  "Operating System :: OS Independent",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-  "License :: OSI Approved :: MIT License",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-]
-
-[tool.poetry.scripts]
-# Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
-"wearipedia" = "wearipedia.cl_parser:parse_CLI"
-
-[tool.poetry.dependencies]
-python = "^3.7"
-
-typer = {extras = ["all"], version = "^0.6.1"}
-rich = "^12.6.0"
-pandas = "^1.1"
-tqdm = "^4.64.1"
-garminconnect = "^0.1.48"
-scipy = "^1.6"
-wget = "^3.2"
-
-[tool.poetry.group.dev.dependencies]
-bandit = "^1.7.1"
-black = {version = "^22.10.0", allow-prereleases = true}
-darglint = "^1.8.1"
-insipid-sphinx-theme = "^0.3.6"
-isort = {extras = ["colors"], version = "^5.10.1"}
-mypy = "^0.982"
-mypy-extensions = "^0.4.3"
-pre-commit = "^2.15.0"
-pydocstyle = "^6.1.1"
-pytest = "^7.1.3"
-pylint = "^2.13"
-pyupgrade = "^3.1.0"
-safety = "^2.3.1"
-coverage = "^6.5.0"
-coverage-badge = "^1.1.0"
-pytest-html = "^3.1.1"
-pytest-cov = "^4.0.0"
-sphinx-reredirects = "^0.1.1"
-sphinx-copybutton = "^0.5.1"
-myst-parser = "^0.18.1"
-numpydoc = "^1.5.0"
-
-[tool.black]
-# https://github.com/psf/black
-target-version = ["py39"]
-line-length = 88
-color = true
-
-exclude = '''
-/(
-    \.git
-    | \.hg
-    | \.mypy_cache
-    | \.tox
-    | \.venv
-    | _build
-    | buck-out
-    | build
-    | dist
-    | env
-    | venv
-)/
-'''
-
-[tool.isort]
-# https://github.com/timothycrosley/isort/
-py_version = 39
-line_length = 88
-
-known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
-sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
-include_trailing_comma = true
-profile = "black"
-multi_line_output = 3
-indent = 4
-color_output = true
-
-[tool.mypy]
-# https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.9
-pretty = true
-show_traceback = true
-color_output = true
-
-allow_redefinition = false
-check_untyped_defs = true
-disallow_any_generics = true
-disallow_incomplete_defs = true
-ignore_missing_imports = true
-implicit_reexport = false
-no_implicit_optional = true
-show_column_numbers = true
-show_error_codes = true
-show_error_context = true
-strict_equality = true
-strict_optional = true
-warn_no_return = true
-warn_redundant_casts = true
-warn_return_any = true
-warn_unreachable = true
-warn_unused_configs = true
-warn_unused_ignores = true
-
-
-[tool.pytest.ini_options]
-# https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
-# Directories that are not visited by pytest collector:
-norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
-doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
-
-# Extra options:
-addopts = [
-  "--strict-markers",
-  "--tb=short",
-  "--doctest-modules",
-  "--doctest-continue-on-failure",
-]
-
-[tool.coverage.run]
-source = ["tests"]
-
-[coverage.paths]
-source = "wearipedia"
-
-[coverage.run]
-branch = true
-
-[coverage.report]
-fail_under = 50
-show_missing = true
+# Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
+[build-system]
+requires = ["poetry_core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
+name = "wearipedia"
+version = "0.1.3"
+description = "Wearable data for all"
+readme = "README.md"
+authors = ["The Stanford Wearipedia Project <arjo@stanford.edu>"]
+license = "MIT"
+repository = "https://github.com/Stanford-Health/wearipedia"
+homepage = "http://wearipedia.com"
+
+# Keywords description https://python-poetry.org/docs/pyproject/#keywords
+keywords = []  #! Update me
+
+# Pypi classifiers: https://pypi.org/classifiers/
+classifiers = [  #! Update me
+  "Development Status :: 3 - Alpha",
+  "Intended Audience :: Developers",
+  "Operating System :: OS Independent",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.9",
+]
+
+[tool.poetry.scripts]
+# Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
+"wearipedia" = "wearipedia.cl_parser:parse_CLI"
+
+[tool.poetry.dependencies]
+python = ">=3.9, <4.0"
+
+typer = {extras = ["all"], version = "^0.6.1"}
+rich = "^12.6.0"
+pandas = "1.5.3"
+tqdm = "^4.64.1"
+garminconnect = "^0.1.48"
+scipy = "^1.6"
+wget = "^3.2"
+fbm = "^0.3.0"
+beautifulsoup4 = "^4.12.2"
+myfitnesspal = "^2.0.1"
+polyline = "^2.0.0"
+jupyter = "^1.0.0"
+fastapi = "0.101"
+typing-extensions = "4.5.0"
+kaleido = "0.2.1"
+lida = "^0.0.11"
+
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.1"
+black = {version = "^22.10.0", allow-prereleases = true}
+darglint = "^1.8.1"
+insipid-sphinx-theme = "^0.3.6"
+isort = {extras = ["colors"], version = "^5.10.1"}
+mypy = "^0.982"
+mypy-extensions = "^0.4.3"
+pre-commit = "^2.15.0"
+pydocstyle = "^6.1.1"
+pytest = "^7.1.3"
+pylint = "^2.13"
+pyupgrade = "^3.1.0"
+safety = "^2.3.1"
+coverage = "^6.5.0"
+coverage-badge = "^1.1.0"
+pytest-html = "^3.1.1"
+pytest-cov = "^4.0.0"
+sphinx-reredirects = "^0.1.1"
+sphinx-copybutton = "^0.5.1"
+myst-parser = "^0.18.1"
+numpydoc = "^1.5.0"
+
+[tool.black]
+# https://github.com/psf/black
+target-version = ["py39"]
+line-length = 88
+color = true
+
+exclude = '''
+/(
+    \.git
+    | \.hg
+    | \.mypy_cache
+    | \.tox
+    | \.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+    | env
+    | venv
+    | docs
+)/
+'''
+
+[tool.isort]
+# https://github.com/timothycrosley/isort/
+py_version = 39
+line_length = 88
+
+known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
+sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+include_trailing_comma = true
+profile = "black"
+multi_line_output = 3
+indent = 4
+color_output = true
+
+[tool.mypy]
+# https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
+python_version = 3.9
+pretty = true
+show_traceback = true
+color_output = true
+
+allow_redefinition = false
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+ignore_missing_imports = true
+implicit_reexport = false
+no_implicit_optional = true
+show_column_numbers = true
+show_error_codes = true
+show_error_context = true
+strict_equality = true
+strict_optional = true
+warn_no_return = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unreachable = true
+warn_unused_configs = true
+warn_unused_ignores = true
+
+
+[tool.pytest.ini_options]
+# https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
+# Directories that are not visited by pytest collector:
+norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
+doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
+
+# Extra options:
+addopts = [
+  "--strict-markers",
+  "--tb=short",
+  "--doctest-modules",
+  "--doctest-continue-on-failure",
+]
+
+[tool.coverage.run]
+source = ["tests"]
+
+[coverage.paths]
+source = "wearipedia"
+
+[coverage.run]
+branch = true
+
+[coverage.report]
+fail_under = 50
+show_missing = true
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/device.py` & `wearipedia-0.1.3/wearipedia/devices/device.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-"""
-device.py
-====================================
-The core module for the wearipedia library.
-"""
-
-__all__ = ["BaseDevice"]
-
-
-class BaseDevice:
-    """This class is a base class for all devices. It should not be instantiated directly.
-    Instead, you should instantiate a child class of this class, which should be specific to
-    a particular device. For example, the Fenix7S class is a child class of this class, and
-    is specific to the Garmin Fenix7S device.
-
-    The child class should implement the following methods:
-
-    * __init__
-
-    * _get_real
-
-    * _filter_synthetic
-
-    * _gen_synthetic
-
-    * _default_params
-
-    * _authenticate
-
-    """
-
-    def __init__(self, **kwargs):
-        """Initializes the device. If you are implementing a child device, the overrided
-        __init__() should call _initialize_device_params().
-        """
-
-        default_init_params = {
-            "seed": 0,
-            "synthetic_start_date": "2022-03-01",
-            "synthetic_end_date": "2022-06-17",
-        }
-
-        params = default_init_params
-
-        self._initialize_device_params([], params, default_init_params)
-
-    def _initialize_device_params(self, valid_data_types, params, default_init_params):
-        """Initializes the device parameters. This is called by the __init__ method.
-        This method will set some member attributes and override the default_init_params
-        with the params provided by the user.
-
-        IF YOU ARE IMPLEMENTING A NEW DEVICE, YOU SHOULD NOT NEED TO OVERRIDE THIS METHOD.
-
-        :param valid_data_types: a list of valid data types for the device.
-        :type valid_data_types: List
-        :param params: a dictionary containing parameters for the device. These are specific
-            to each device, and should usually consist of parameters for synthetic data
-            generation (for example, the start and end dates, persona, or random seed).
-        :type params: Dict
-        :param default_init_params: a dictionary containing default parameters for the device.
-        :type default_init_params: Dict
-        """
-
-        self._authenticated = False
-        self.valid_data_types = valid_data_types
-        self._synthetic_has_been_generated = False
-        self.init_params = default_init_params
-
-        if params is None:
-            params = dict()
-
-        for key in self.init_params.keys():
-            if key in params:
-                self.init_params[key] = params[key]
-
-    def _get_real(self, data_type, params):
-        """Gets real data from the API according to the data_type and params.
-
-        :param data_type: a string describing the type of data to get.
-        :type data_type: str
-        :param params: dictionary containing parameters for API extraction
-        :type params: Dict
-        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
-            by child classes.
-        """
-        raise NotImplementedError
-
-    def _filter_synthetic(self, data, data_type, params):
-        """Filters synthetic data that was already generated by _gen_synthetic() according
-        to params in the same way that the real API would filter data.
-
-        :param data: the data to filter
-        :type data: List or DataFrame or Series or Dict
-        :param data_type: a string describing the type of data to get.
-        :type data_type: str
-        :param params: dictionary containing parameters for API extraction
-        :type params: Dict
-        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
-            by child classes.
-        """
-        raise NotImplementedError
-
-    def _gen_synthetic(self):
-        """Generates synthetic data for the device. This is automatically called by get_data()
-        exactly once, when the user calls get_data() without first calling authenticate().
-
-        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
-            by child classes.
-        """
-        raise NotImplementedError
-
-    def _default_params(self):
-        """Returns default parameters for API extraction.
-
-        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
-            by child classes.
-        """
-        raise NotImplementedError
-
-    def get_data(self, data_type, params=None):
-        """Gets data from the API according to the data_type and params.
-
-        Follows the procedure of first checking if the data_type is valid, then setting
-        default parameters if none are provided, then checking if the device is authenticated,
-        and finally calling the _get_real method if the device is authenticated (otherwise
-        fetching synthetic data).
-
-        Note that we explicitly enforce that the child class must set a separate piece of data
-        as a member attribute for each data type. This is because we want to ensure that
-        (unauthenticated) child objects are not generating data on the fly on each call to
-        get_data(), but instead are generating data once and storing it in a member attribute.
-
-        Generating data all at once for the entire time period is not very slow, and is
-        necessary for the synthetic data to be consistent across calls to get_data().
-
-        IF YOU ARE IMPLEMENTING A NEW DEVICE, YOU SHOULD NOT NEED TO OVERRIDE THIS METHOD.
-
-        :param data_type: a string describing the type of data to get.
-        :type data_type: str
-        :param params: dictionary containing parameters for API extraction, defaults to None
-        :type params: Dict, optional
-        :raises ValueError: if data_type is not in valid_data_types
-        :raises Exception: if the user has not called gen_synthetic() or authenticate() yet.
-        :return: returns the data from the API (or synthetic data if gen_synthetic() has been called)
-        :rtype: List or DataFrame or Series or Dict
-        """
-        if not data_type in self.valid_data_types:
-            raise ValueError(f"data_type must be in {list(self.valid_data_types)}")
-
-        if params is None:
-            params = self._default_params()
-
-        if self.authenticated:
-            return self._get_real(data_type, params)
-        else:
-            if self.synthetic_has_been_generated:
-                return self._filter_synthetic(
-                    getattr(self, data_type), data_type, params
-                )
-            else:
-                self._gen_synthetic()
-                self._synthetic_has_been_generated = True
-                return self._filter_synthetic(
-                    getattr(self, data_type), data_type, params
-                )
-
-    def _authenticate(self, auth_creds):
-        """Authenticates the device. This is called by the authenticate() method.
-
-        :param auth_creds: a dictionary containing authentication credentials for the device.
-        :type auth_creds: Dict
-        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
-            by child classes.
-        """
-
-        raise NotImplementedError
-
-    def authenticate(self, auth_creds):
-        """Authenticates the device against the API. For now, should be user-interactive, if
-        the authentication protocol requires a step in which you get a code by visiting their
-        website.
-
-        IF YOU ARE IMPLEMENTING A NEW DEVICE, YOU SHOULD NOT NEED TO OVERRIDE THIS METHOD.
-
-        :param auth_creds: a dictionary containing the authentication credentials.
-        :type auth_creds: Dict
-        """
-
-        self._authenticate(auth_creds)
-        self._authenticated = True
-
-    @property
-    def authenticated(self):
-        return self._authenticated
-
-    @property
-    def synthetic_has_been_generated(self):
-        return self._synthetic_has_been_generated
+"""
+device.py
+====================================
+The core module for the wearipedia library.
+"""
+
+__all__ = ["BaseDevice"]
+
+
+class BaseDevice:
+    """This class is a base class for all devices. It should not be instantiated directly.
+    Instead, you should instantiate a child class of this class, which should be specific to
+    a particular device. For example, the Fenix7S class is a child class of this class, and
+    is specific to the Garmin Fenix7S device.
+
+    The child class should implement the following methods:
+
+    * __init__
+
+    * _get_real
+
+    * _filter_synthetic
+
+    * _gen_synthetic
+
+    * _default_params
+
+    * _authenticate
+
+    """
+
+    def __init__(self, **kwargs):
+        """Initializes the device. If you are implementing a child device, the overrided
+        __init__() should call _initialize_device_params().
+        """
+
+        default_init_params = {
+            "seed": 0,
+            "synthetic_start_date": "2022-03-01",
+            "synthetic_end_date": "2022-06-17",
+        }
+
+        params = default_init_params
+
+        self._initialize_device_params([], params, default_init_params)
+
+    def _initialize_device_params(self, valid_data_types, params, default_init_params):
+        """Initializes the device parameters. This is called by the __init__ method.
+        This method will set some member attributes and override the default_init_params
+        with the params provided by the user.
+
+        IF YOU ARE IMPLEMENTING A NEW DEVICE, YOU SHOULD NOT NEED TO OVERRIDE THIS METHOD.
+
+        :param valid_data_types: a list of valid data types for the device.
+        :type valid_data_types: List
+        :param params: a dictionary containing parameters for the device. These are specific
+            to each device, and should usually consist of parameters for synthetic data
+            generation (for example, the start and end dates, persona, or random seed).
+        :type params: Dict
+        :param default_init_params: a dictionary containing default parameters for the device.
+        :type default_init_params: Dict
+        """
+
+        self._authenticated = False
+        self.valid_data_types = valid_data_types
+        self._synthetic_has_been_generated = False
+        self.init_params = default_init_params
+
+        if params is None:
+            params = dict()
+
+        for key in self.init_params.keys():
+            if key in params:
+                self.init_params[key] = params[key]
+
+    def _get_real(self, data_type, params):
+        """Gets real data from the API according to the data_type and params.
+
+        :param data_type: a string describing the type of data to get.
+        :type data_type: str
+        :param params: dictionary containing parameters for API extraction
+        :type params: Dict
+        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
+            by child classes.
+        """
+        raise NotImplementedError
+
+    def _filter_synthetic(self, data, data_type, params):
+        """Filters synthetic data that was already generated by _gen_synthetic() according
+        to params in the same way that the real API would filter data.
+
+        :param data: the data to filter
+        :type data: List or DataFrame or Series or Dict
+        :param data_type: a string describing the type of data to get.
+        :type data_type: str
+        :param params: dictionary containing parameters for API extraction
+        :type params: Dict
+        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
+            by child classes.
+        """
+        raise NotImplementedError
+
+    def _gen_synthetic(self):
+        """Generates synthetic data for the device. This is automatically called by get_data()
+        exactly once, when the user calls get_data() without first calling authenticate().
+
+        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
+            by child classes.
+        """
+        raise NotImplementedError
+
+    def _default_params(self):
+        """Returns default parameters for API extraction.
+
+        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
+            by child classes.
+        """
+        raise NotImplementedError
+
+    def get_data(self, data_type, params=None):
+        """Gets data from the API according to the data_type and params.
+
+        Follows the procedure of first checking if the data_type is valid, then setting
+        default parameters if none are provided, then checking if the device is authenticated,
+        and finally calling the _get_real method if the device is authenticated (otherwise
+        fetching synthetic data).
+
+        Note that we explicitly enforce that the child class must set a separate piece of data
+        as a member attribute for each data type. This is because we want to ensure that
+        (unauthenticated) child objects are not generating data on the fly on each call to
+        get_data(), but instead are generating data once and storing it in a member attribute.
+
+        Generating data all at once for the entire time period is not very slow, and is
+        necessary for the synthetic data to be consistent across calls to get_data().
+
+        IF YOU ARE IMPLEMENTING A NEW DEVICE, YOU SHOULD NOT NEED TO OVERRIDE THIS METHOD.
+
+        :param data_type: a string describing the type of data to get.
+        :type data_type: str
+        :param params: dictionary containing parameters for API extraction, defaults to None
+        :type params: Dict, optional
+        :raises ValueError: if data_type is not in valid_data_types
+        :raises Exception: if the user has not called gen_synthetic() or authenticate() yet.
+        :return: returns the data from the API (or synthetic data if gen_synthetic() has been called)
+        :rtype: List or DataFrame or Series or Dict
+        """
+        if not data_type in self.valid_data_types:
+            raise ValueError(f"data_type must be in {list(self.valid_data_types)}")
+
+        if params is None:
+            params = self._default_params()
+
+        if self.authenticated:
+            return self._get_real(data_type, params)
+        else:
+            if self.synthetic_has_been_generated:
+                return self._filter_synthetic(
+                    getattr(self, data_type), data_type, params
+                )
+            else:
+                self._gen_synthetic()
+                self._synthetic_has_been_generated = True
+                return self._filter_synthetic(
+                    getattr(self, data_type), data_type, params
+                )
+
+    def _authenticate(self, auth_creds):
+        """Authenticates the device. This is called by the authenticate() method.
+
+        :param auth_creds: a dictionary containing authentication credentials for the device.
+        :type auth_creds: Dict
+        :raises NotImplementedError: for now, raises NotImplementedError, but should be implemented
+            by child classes.
+        """
+
+        raise NotImplementedError
+
+    def authenticate(self, auth_creds):
+        """Authenticates the device against the API. For now, should be user-interactive, if
+        the authentication protocol requires a step in which you get a code by visiting their
+        website.
+
+        IF YOU ARE IMPLEMENTING A NEW DEVICE, YOU SHOULD NOT NEED TO OVERRIDE THIS METHOD.
+
+        :param auth_creds: a dictionary containing the authentication credentials.
+        :type auth_creds: Dict
+        """
+
+        self._authenticate(auth_creds)
+        self._authenticated = True
+
+    @property
+    def authenticated(self):
+        return self._authenticated
+
+    @property
+    def synthetic_has_been_generated(self):
+        return self._synthetic_has_been_generated
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/dexcom/pro_cgm.py` & `wearipedia-0.1.3/wearipedia/devices/dexcom/pro_cgm.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import http
-import json
-
-import numpy as np
-import pandas as pd
-
-from ...devices.device import BaseDevice
-from ...utils import bin_search, seed_everything
-from .pro_cgm_fetch import *
-from .pro_cgm_gen import *
-
-class_name = "DexcomProCGM"
-
-
-class DexcomProCGM(BaseDevice):
-    """This device allows you to work with data from the `Dexcom Pro CGM <https://provider.dexcom.com/products/dexcom-g6-pro>`_ device.
-    Available datatypes for this device are:
-
-    * `data`: contains all data in one dictionary
-
-    :param seed: random seed for synthetic data generation, defaults to 0
-    :type seed: int, optional
-    :param synthetic_start_date: start date for synthetic data generation, defaults to "2022-03-01"
-    :type synthetic_start_date: str, optional
-    :param synthetic_end_date: end date for synthetic data generation, defaults to "2022-06-17"
-    :type synthetic_end_date: str, optional
-    """
-
-    def __init__(
-        self, seed=0, synthetic_start_date="2022-02-16", synthetic_end_date="2022-05-15"
-    ):
-
-        params = {
-            "seed": seed,
-            "synthetic_start_date": synthetic_start_date,
-            "synthetic_end_date": synthetic_end_date,
-        }
-
-        self._initialize_device_params(
-            ["data"],
-            params,
-            {
-                "seed": 0,
-                "synthetic_start_date": "2022-02-16",
-                "synthetic_end_date": "2022-05-15",
-            },
-        )
-
-    def _default_params(self):
-        return {
-            "start_date": self.init_params["synthetic_start_date"],
-            "end_date": self.init_params["synthetic_end_date"],
-        }
-
-    def _get_real(self, data_type, params):
-        # there is really only one data type for this device,
-        # so we don't need to check the data_type
-
-        return fetch_data(
-            self.access_token,
-            start_date=params["start_date"],
-            end_date=params["end_date"],
-        )
-
-    def _filter_synthetic(self, data, data_type, params):
-        # there is really only one data type for this device,
-        # so we don't need to check the data_type
-
-        start_ts = pd.Timestamp(params["start_date"])
-        end_ts = pd.Timestamp(params["end_date"])
-
-        timestamps = [pd.Timestamp(x["systemTime"]) for x in self.data["egvs"]]
-
-        start_idx = bin_search(timestamps, start_ts)
-        end_idx = bin_search(timestamps, end_ts)
-
-        return {
-            "unit": "mg/dL",
-            "rateUnit": "mg/dL/min",
-            "egvs": self.data["egvs"][start_idx:end_idx],
-        }
-
-    def _gen_synthetic(self):
-        # generate random data according to seed
-        seed_everything(self.init_params["seed"])
-
-        self.data = create_synth(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-        )
-
-    def _authenticate(self, auth_creds, use_cache=True):
-        if use_cache and hasattr(self, "access_token"):
-            return
-
-        if "refresh_token" in auth_creds:
-            self.refresh_token, self.access_token = refresh_access_token(
-                auth_creds["refresh_token"],
-                auth_creds["client_id"],
-                auth_creds["client_secret"],
-            )
-        else:
-            self.refresh_token, self.access_token = dexcom_authenticate(
-                auth_creds["client_id"], auth_creds["client_secret"]
-            )
+import http
+import json
+
+import numpy as np
+import pandas as pd
+
+from ...devices.device import BaseDevice
+from ...utils import bin_search, seed_everything
+from .pro_cgm_fetch import *
+from .pro_cgm_gen import *
+
+class_name = "DexcomProCGM"
+
+
+class DexcomProCGM(BaseDevice):
+    """This device allows you to work with data from the `Dexcom Pro CGM <https://provider.dexcom.com/products/dexcom-g6-pro>`_ device.
+    Available datatypes for this device are:
+
+    * `data`: contains all data in one dictionary
+
+    :param seed: random seed for synthetic data generation, defaults to 0
+    :type seed: int, optional
+    :param synthetic_start_date: start date for synthetic data generation, defaults to "2022-03-01"
+    :type synthetic_start_date: str, optional
+    :param synthetic_end_date: end date for synthetic data generation, defaults to "2022-06-17"
+    :type synthetic_end_date: str, optional
+    """
+
+    def __init__(
+        self, seed=0, synthetic_start_date="2022-02-16", synthetic_end_date="2022-05-15"
+    ):
+
+        params = {
+            "seed": seed,
+            "synthetic_start_date": synthetic_start_date,
+            "synthetic_end_date": synthetic_end_date,
+        }
+
+        self._initialize_device_params(
+            ["data"],
+            params,
+            {
+                "seed": 0,
+                "synthetic_start_date": "2022-02-16",
+                "synthetic_end_date": "2022-05-15",
+            },
+        )
+
+    def _default_params(self):
+        return {
+            "start_date": self.init_params["synthetic_start_date"],
+            "end_date": self.init_params["synthetic_end_date"],
+        }
+
+    def _get_real(self, data_type, params):
+        # there is really only one data type for this device,
+        # so we don't need to check the data_type
+
+        return fetch_data(
+            self.access_token,
+            start_date=params["start_date"],
+            end_date=params["end_date"],
+        )
+
+    def _filter_synthetic(self, data, data_type, params):
+        # there is really only one data type for this device,
+        # so we don't need to check the data_type
+
+        start_ts = pd.Timestamp(params["start_date"])
+        end_ts = pd.Timestamp(params["end_date"])
+
+        timestamps = [pd.Timestamp(x["systemTime"]) for x in self.data["egvs"]]
+
+        start_idx = bin_search(timestamps, start_ts)
+        end_idx = bin_search(timestamps, end_ts)
+
+        return {
+            "unit": "mg/dL",
+            "rateUnit": "mg/dL/min",
+            "egvs": self.data["egvs"][start_idx:end_idx],
+        }
+
+    def _gen_synthetic(self):
+        # generate random data according to seed
+        seed_everything(self.init_params["seed"])
+
+        self.data = create_synth(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+        )
+
+    def _authenticate(self, auth_creds, use_cache=True):
+        if use_cache and hasattr(self, "access_token"):
+            return
+
+        if "refresh_token" in auth_creds:
+            self.refresh_token, self.access_token = refresh_access_token(
+                auth_creds["refresh_token"],
+                auth_creds["client_id"],
+                auth_creds["client_secret"],
+            )
+        else:
+            self.refresh_token, self.access_token = dexcom_authenticate(
+                auth_creds["client_id"], auth_creds["client_secret"]
+            )
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/dexcom/pro_cgm_fetch.py` & `wearipedia-0.1.3/wearipedia/devices/dexcom/pro_cgm_fetch.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import http
-import json
-import time
-import urllib
-from datetime import datetime
-
-import pandas as pd
-import requests
-
-__all__ = ["refresh_access_token", "dexcom_authenticate", "fetch_data"]
-
-
-def refresh_access_token(refresh_token, client_id, client_secret):
-    # gives us access token given the refresh token
-
-    params = {
-        "client_id": client_id,
-        "client_secret": client_secret,
-        "refresh_token": refresh_token,
-        "grant_type": "refresh_token",
-        "redirect_uri": "https://www.google.com",
-    }
-
-    out = requests.post("https://api.dexcom.com/v2/oauth2/token", data=params)
-
-    body = json.loads(out.text)
-
-    return body["refresh_token"], body["access_token"]
-
-
-def dexcom_authenticate(your_client_id, your_client_secret):
-    your_redirect_uri = "https://www.google.com"
-    your_state_value = "1234"
-
-    url = f"https://api.dexcom.com/v2/oauth2/login?client_id={your_client_id}&redirect_uri={your_redirect_uri}&response_type=code&scope=offline_access&state={your_state_value}"
-
-    print(url)
-
-    print("redirect url below:")
-    time.sleep(0.1)
-    redirect_url = input(">")
-
-    try:
-        your_authorization_code = urllib.parse.parse_qs(
-            urllib.parse.urlparse(redirect_url).query
-        )["code"][0]
-    except Exception as e:
-        exception_str = f"Caught error:\n{e}\n"
-        exception_str += "\nPlease copy and paste the entire URL (including https)"
-        raise Exception(exception_str)
-
-    conn = http.client.HTTPSConnection("api.dexcom.com")
-
-    payload = f"client_secret={your_client_secret}&client_id={your_client_id}&code={your_authorization_code}&grant_type=authorization_code&redirect_uri={your_redirect_uri}"
-
-    headers = {
-        "content-type": "application/x-www-form-urlencoded",
-        "cache-control": "no-cache",
-    }
-
-    conn.request("POST", "/v2/oauth2/token", payload, headers)
-
-    res = conn.getresponse()
-    data = res.read()
-
-    json_response = json.loads(data.decode("utf-8"))
-
-    if "error" in json_response.keys() and json_response["error"] == "invalid_grant":
-        exception_str = (
-            "The code you got has expired.\nAuthorize and enter the redirect URL again."
-        )
-        raise Exception(exception_str)
-    else:
-        body = json.loads(data.decode("utf-8"))
-        access_token = body["access_token"]
-        refresh_token = body["refresh_token"]
-
-        print(f'Entire response was {data.decode("utf-8")}')
-        print(f"Our access token is {access_token}")
-
-    return refresh_token, access_token
-
-
-def fetch_data(access_token, start_date="2022-02-16", end_date="2022-05-15"):
-    start_date = start_date + "T15:30:00"
-    end_date = end_date + "T15:45:00"
-
-    headers = {"authorization": f"Bearer {access_token}"}
-
-    endpoint = f"https://api.dexcom.com/v2/users/self/egvs?startDate={start_date}&endDate={end_date}"
-
-    out = json.loads(requests.get(endpoint, headers=headers).text)
-
-    if "errors" in out.keys():
-        exception_str = (
-            f'Got error(s) {out["errors"]}. Fix start and end dates and rerun.'
-        )
-        raise Exception(exception_str)
-    elif "fault" in out.keys():
-        exception_str = (
-            f'Got fault {out["fault"]}. You might need to request another access token.'
-        )
-        raise Exception(exception_str)
-    else:
-
-        return out
+import http
+import json
+import time
+import urllib
+from datetime import datetime
+
+import pandas as pd
+import requests
+
+__all__ = ["refresh_access_token", "dexcom_authenticate", "fetch_data"]
+
+
+def refresh_access_token(refresh_token, client_id, client_secret):
+    # gives us access token given the refresh token
+
+    params = {
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "refresh_token": refresh_token,
+        "grant_type": "refresh_token",
+        "redirect_uri": "https://www.google.com",
+    }
+
+    out = requests.post("https://api.dexcom.com/v2/oauth2/token", data=params)
+
+    body = json.loads(out.text)
+
+    return body["refresh_token"], body["access_token"]
+
+
+def dexcom_authenticate(your_client_id, your_client_secret):
+    your_redirect_uri = "https://www.google.com"
+    your_state_value = "1234"
+
+    url = f"https://api.dexcom.com/v2/oauth2/login?client_id={your_client_id}&redirect_uri={your_redirect_uri}&response_type=code&scope=offline_access&state={your_state_value}"
+
+    print(url)
+
+    print("redirect url below:")
+    time.sleep(0.1)
+    redirect_url = input(">")
+
+    try:
+        your_authorization_code = urllib.parse.parse_qs(
+            urllib.parse.urlparse(redirect_url).query
+        )["code"][0]
+    except Exception as e:
+        exception_str = f"Caught error:\n{e}\n"
+        exception_str += "\nPlease copy and paste the entire URL (including https)"
+        raise Exception(exception_str)
+
+    conn = http.client.HTTPSConnection("api.dexcom.com")
+
+    payload = f"client_secret={your_client_secret}&client_id={your_client_id}&code={your_authorization_code}&grant_type=authorization_code&redirect_uri={your_redirect_uri}"
+
+    headers = {
+        "content-type": "application/x-www-form-urlencoded",
+        "cache-control": "no-cache",
+    }
+
+    conn.request("POST", "/v2/oauth2/token", payload, headers)
+
+    res = conn.getresponse()
+    data = res.read()
+
+    json_response = json.loads(data.decode("utf-8"))
+
+    if "error" in json_response.keys() and json_response["error"] == "invalid_grant":
+        exception_str = (
+            "The code you got has expired.\nAuthorize and enter the redirect URL again."
+        )
+        raise Exception(exception_str)
+    else:
+        body = json.loads(data.decode("utf-8"))
+        access_token = body["access_token"]
+        refresh_token = body["refresh_token"]
+
+        print(f'Entire response was {data.decode("utf-8")}')
+        print(f"Our access token is {access_token}")
+
+    return refresh_token, access_token
+
+
+def fetch_data(access_token, start_date="2022-02-16", end_date="2022-05-15"):
+    start_date = start_date + "T15:30:00"
+    end_date = end_date + "T15:45:00"
+
+    headers = {"authorization": f"Bearer {access_token}"}
+
+    endpoint = f"https://api.dexcom.com/v2/users/self/egvs?startDate={start_date}&endDate={end_date}"
+
+    out = json.loads(requests.get(endpoint, headers=headers).text)
+
+    if "errors" in out.keys():
+        exception_str = (
+            f'Got error(s) {out["errors"]}. Fix start and end dates and rerun.'
+        )
+        raise Exception(exception_str)
+    elif "fault" in out.keys():
+        exception_str = (
+            f'Got fault {out["fault"]}. You might need to request another access token.'
+        )
+        raise Exception(exception_str)
+    else:
+
+        return out
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/dexcom/pro_cgm_gen.py` & `wearipedia-0.1.3/wearipedia/devices/dexcom/pro_cgm_gen.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from datetime import datetime, timedelta
-
-import numpy as np
-import pandas as pd
-from scipy.ndimage import gaussian_filter
-from tqdm import tqdm
-
-__all__ = ["create_synth"]
-
-
-def lerp(x1, x2, t):
-    return t * x2 + (1 - t) * x1
-
-
-base_keypoints = [100] * 4 + [120] * 4 + [130] * 8 + [120] * 4 + [100] * 4
-
-
-def create_synth(start_day_str, end_day_str):
-    """Create a synthetic dataframe of CGM data.
-
-    :param start_day_str: the start date represented as a string in the format "YYYY-MM-DD"
-    :type start_day_str: str
-    :param end_day_str: the end date represented as a string in the format "YYYY-MM-DD"
-    :type end_day_str: str
-    :return: the synthetic dataframe
-    :rtype: pd.DataFrame
-    """
-
-    start_day = datetime.strptime(start_day_str, "%Y-%m-%d")
-    end_day = datetime.strptime(end_day_str, "%Y-%m-%d")
-
-    num_days = (end_day - start_day).days
-
-    datetimes = []
-    glucoses = []
-
-    for day_offset in tqdm(range(num_days)):
-        if day_offset != 0:
-            overlap = keypoints[-1]
-        keypoints = list(np.random.randn(24) * 10 + np.array(base_keypoints))
-        if day_offset != 0:
-            keypoints[0] = overlap
-
-        keypoints = keypoints + [keypoints[0]]
-
-        for minute_offset in range(0, 24 * 60, 5):
-            minute = (
-                start_day
-                + timedelta(days=day_offset)
-                + timedelta(minutes=minute_offset)
-            )
-
-            scaled_offset = minute_offset / 60
-
-            k1 = keypoints[np.floor(scaled_offset).astype("int")]
-            k2 = keypoints[np.ceil(scaled_offset).astype("int")]
-
-            value = lerp(k1, k2, scaled_offset % 1)
-            if value > 130:
-                scaling = 30
-            else:
-                scaling = 15
-            value += np.random.randn() * scaling
-
-            datetimes.append(minute)
-            glucoses.append(value)
-
-    egvs = []
-    glucoses = gaussian_filter(glucoses, 2, mode="constant")
-
-    for dt_obj, glucose in zip(datetimes[::-1], glucoses[::-1]):
-        egvs.append(
-            {
-                "systemTime": dt_obj.strftime("%Y-%m-%dT%H:%M:%S"),
-                # this is supposed to be timezone shift
-                "displayTime": dt_obj.strftime("%Y-%m-%dT%H:%M:%S"),
-                "value": glucose,
-                "realtimeValue": glucose,
-                "smoothedValue": None,
-                "status": None,
-                "trend": "flat",
-                "trendRate": np.round(np.random.normal(), 2),
-            }
-        )
-
-    out = {"unit": "mg/dL", "rateUnit": "mg/dL/min", "egvs": egvs}
-
-    return out
+from datetime import datetime, timedelta
+
+import numpy as np
+import pandas as pd
+from scipy.ndimage import gaussian_filter
+from tqdm import tqdm
+
+__all__ = ["create_synth"]
+
+
+def lerp(x1, x2, t):
+    return t * x2 + (1 - t) * x1
+
+
+base_keypoints = [100] * 4 + [120] * 4 + [130] * 8 + [120] * 4 + [100] * 4
+
+
+def create_synth(start_day_str, end_day_str):
+    """Create a synthetic dataframe of CGM data.
+
+    :param start_day_str: the start date represented as a string in the format "YYYY-MM-DD"
+    :type start_day_str: str
+    :param end_day_str: the end date represented as a string in the format "YYYY-MM-DD"
+    :type end_day_str: str
+    :return: the synthetic dataframe
+    :rtype: pd.DataFrame
+    """
+
+    start_day = datetime.strptime(start_day_str, "%Y-%m-%d")
+    end_day = datetime.strptime(end_day_str, "%Y-%m-%d")
+
+    num_days = (end_day - start_day).days
+
+    datetimes = []
+    glucoses = []
+
+    for day_offset in tqdm(range(num_days)):
+        if day_offset != 0:
+            overlap = keypoints[-1]
+        keypoints = list(np.random.randn(24) * 10 + np.array(base_keypoints))
+        if day_offset != 0:
+            keypoints[0] = overlap
+
+        keypoints = keypoints + [keypoints[0]]
+
+        for minute_offset in range(0, 24 * 60, 5):
+            minute = (
+                start_day
+                + timedelta(days=day_offset)
+                + timedelta(minutes=minute_offset)
+            )
+
+            scaled_offset = minute_offset / 60
+
+            k1 = keypoints[np.floor(scaled_offset).astype("int")]
+            k2 = keypoints[np.ceil(scaled_offset).astype("int")]
+
+            value = lerp(k1, k2, scaled_offset % 1)
+            if value > 130:
+                scaling = 30
+            else:
+                scaling = 15
+            value += np.random.randn() * scaling
+
+            datetimes.append(minute)
+            glucoses.append(value)
+
+    egvs = []
+    glucoses = gaussian_filter(glucoses, 2, mode="constant")
+
+    for dt_obj, glucose in zip(datetimes[::-1], glucoses[::-1]):
+        egvs.append(
+            {
+                "systemTime": dt_obj.strftime("%Y-%m-%dT%H:%M:%S"),
+                # this is supposed to be timezone shift
+                "displayTime": dt_obj.strftime("%Y-%m-%dT%H:%M:%S"),
+                "value": glucose,
+                "realtimeValue": glucose,
+                "smoothedValue": None,
+                "status": None,
+                "trend": "flat",
+                "trendRate": np.round(np.random.normal(), 2),
+            }
+        )
+
+    out = {"unit": "mg/dL", "rateUnit": "mg/dL/min", "egvs": egvs}
+
+    return out
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/dreem/headband_2.py` & `wearipedia-0.1.3/wearipedia/devices/dreem/headband_2.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import base64
-import json
-import os
-from pathlib import Path
-
-import requests
-
-from ...devices.device import BaseDevice
-from ...utils import seed_everything
-from .dreem_fetch import *
-from .dreem_gen import *
-
-class_name = "DreemHeadband2"
-
-
-class DreemHeadband2(BaseDevice):
-    def __init__(
-        self, seed=0, synthetic_start_date="2022-03-01", synthetic_end_date="2022-06-17"
-    ):
-
-        params = {
-            "seed": seed,
-            "synthetic_start_date": synthetic_start_date,
-            "synthetic_end_date": synthetic_end_date,
-        }
-
-        self._initialize_device_params(
-            ["users", "records", "hypnogram", "eeg_file"],
-            params,
-            {
-                "seed": 0,
-                "synthetic_start_date": "2022-03-01",
-                "synthetic_end_date": "2022-06-17",
-            },
-        )
-
-    def _default_params(self):
-        # this is wrong, but it's just a placeholder
-        return dict()
-
-    def _get_real(self, data_type, params):
-        if data_type == "users":
-            return fetch_users(self.auth_dict)
-        elif data_type == "records":
-            return fetch_records(self.auth_dict, params["user"])
-        elif data_type == "hypnogram":
-            return fetch_hypnogram(self.auth_dict, params["record_ref"])
-        elif data_type == "eeg_file":
-            return fetch_eeg_file(self.auth_dict, params["record_ref"])
-
-    def _filter_synthetic(self, data, data_type, params):
-        return []
-
-    def _gen_synthetic(self):
-        # generate random data according to seed
-        seed_everything(self.init_params["seed"])
-
-        self.users = []
-        self.records = []
-        self.hypnogram = []
-        self.eeg_file = []
-
-    def _authenticate(self, auth_creds):
-        authorization_str = (
-            "Basic "
-            + base64.b64encode(
-                bytes(auth_creds["email"] + ":" + auth_creds["password"], "utf-8")
-            ).decode()
-        )
-
-        self.auth_dict = json.loads(
-            requests.post(
-                "https://login.rythm.co/token/",
-                headers={"Authorization": authorization_str},
-            ).text
-        )
+import base64
+import json
+import os
+from pathlib import Path
+
+import requests
+
+from ...devices.device import BaseDevice
+from ...utils import seed_everything
+from .dreem_fetch import *
+from .dreem_gen import *
+
+class_name = "DreemHeadband2"
+
+
+class DreemHeadband2(BaseDevice):
+    def __init__(
+        self, seed=0, synthetic_start_date="2022-03-01", synthetic_end_date="2022-06-17"
+    ):
+
+        params = {
+            "seed": seed,
+            "synthetic_start_date": synthetic_start_date,
+            "synthetic_end_date": synthetic_end_date,
+        }
+
+        self._initialize_device_params(
+            ["users", "records", "hypnogram", "eeg_file"],
+            params,
+            {
+                "seed": 0,
+                "synthetic_start_date": "2022-03-01",
+                "synthetic_end_date": "2022-06-17",
+            },
+        )
+
+    def _default_params(self):
+        # this is wrong, but it's just a placeholder
+        return dict()
+
+    def _get_real(self, data_type, params):
+        if data_type == "users":
+            return fetch_users(self.auth_dict)
+        elif data_type == "records":
+            return fetch_records(self.auth_dict, params["user"])
+        elif data_type == "hypnogram":
+            return fetch_hypnogram(self.auth_dict, params["record_ref"])
+        elif data_type == "eeg_file":
+            return fetch_eeg_file(self.auth_dict, params["record_ref"])
+
+    def _filter_synthetic(self, data, data_type, params):
+        return []
+
+    def _gen_synthetic(self):
+        # generate random data according to seed
+        seed_everything(self.init_params["seed"])
+
+        self.users = []
+        self.records = []
+        self.hypnogram = []
+        self.eeg_file = []
+
+    def _authenticate(self, auth_creds):
+        authorization_str = (
+            "Basic "
+            + base64.b64encode(
+                bytes(auth_creds["email"] + ":" + auth_creds["password"], "utf-8")
+            ).decode()
+        )
+
+        self.auth_dict = json.loads(
+            requests.post(
+                "https://login.rythm.co/token/",
+                headers={"Authorization": authorization_str},
+            ).text
+        )
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/garmin/fenix_fetch.py` & `wearipedia-0.1.3/wearipedia/devices/garmin/fenix_fetch.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import os
-from datetime import datetime, timedelta
-from threading import Lock, Thread
-
-from tqdm import tqdm
-
-__all__ = ["fetch_real_data"]
-
-
-def fetch_day_data(date, array, api_func, lock):
-    date_str = datetime.strftime(date, "%Y-%m-%d")
-
-    # this does not need to be in a critical section, since
-    # requests don't really share state
-    elem = api_func(date_str)
-
-    # critical section, ensuring each index in each array
-    # matches up. with the "lock" context manager,
-    # we ensure that only one thread can access the
-    # critical section (e.g. adding an element to the array)
-    # at a time
-    with lock:
-        array.append(elem)
-
-
-def fetch_real_data(start_date, end_date, data_type, api):
-    """Main function for fetching real data from the Garmin Connect API.
-    We parallelize this since making requests to the API is day-by-day,
-    and API requests are I/O bound.
-
-    :param start_date: the start date represented as a string in the format "YYYY-MM-DD"
-    :type start_date: str
-    :param end_date: the end date represented as a string in the format "YYYY-MM-DD"
-    :type end_date: str
-    :param data_type: the type of data to fetch, one of "dates", "steps", "hrs", "brpms"
-    :type data_type: str
-    :param api: the Garmin Connect API object
-    :type api: Garmin
-    :return: the data fetched from the API according to the inputs
-    :rtype: List
-    """
-
-    num_days = (
-        datetime.strptime(end_date, "%Y-%m-%d")
-        - datetime.strptime(start_date, "%Y-%m-%d")
-    ).days
-
-    lock = Lock()
-
-    if data_type == "steps":
-        api_func = api.get_steps_data
-    elif data_type == "hrs":
-        api_func = api.get_heart_rates
-    elif data_type == "brpms":
-        api_func = api.get_respiration_data
-    elif data_type == "dates":
-        # no API interaction here
-        return [
-            datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=i)
-            for i in tqdm(range(num_days))
-        ]
-
-    arr = []
-
-    # create a thread per each day, and assign it
-    # to fetch the data for that day
-    print("configuring threads...")
-    threads = []
-
-    for i in tqdm(range(num_days)):
-        new_date = datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=i)
-
-        new_thread = Thread(target=fetch_day_data, args=(new_date, arr, api_func, lock))
-
-        threads.append(new_thread)
-
-    # start threads
-    for thread in threads:
-        thread.start()
-
-    # wait for all threads to terminate
-    print("Main thread waiting for child threads...")
-    for thread in tqdm(threads):
-        thread.join()
-
-    # report the number of items in the list
-    print("\ndone")
-
-    return arr
+import os
+from datetime import datetime, timedelta
+from threading import Lock, Thread
+
+from tqdm import tqdm
+
+__all__ = ["fetch_real_data"]
+
+
+def fetch_day_data(date, array, api_func, lock):
+    date_str = datetime.strftime(date, "%Y-%m-%d")
+
+    # this does not need to be in a critical section, since
+    # requests don't really share state
+    elem = api_func(date_str)
+
+    # critical section, ensuring each index in each array
+    # matches up. with the "lock" context manager,
+    # we ensure that only one thread can access the
+    # critical section (e.g. adding an element to the array)
+    # at a time
+    with lock:
+        array.append(elem)
+
+
+def fetch_real_data(start_date, end_date, data_type, api):
+    """Main function for fetching real data from the Garmin Connect API.
+    We parallelize this since making requests to the API is day-by-day,
+    and API requests are I/O bound.
+
+    :param start_date: the start date represented as a string in the format "YYYY-MM-DD"
+    :type start_date: str
+    :param end_date: the end date represented as a string in the format "YYYY-MM-DD"
+    :type end_date: str
+    :param data_type: the type of data to fetch, one of "dates", "steps", "hrs", "brpms"
+    :type data_type: str
+    :param api: the Garmin Connect API object
+    :type api: Garmin
+    :return: the data fetched from the API according to the inputs
+    :rtype: List
+    """
+
+    num_days = (
+        datetime.strptime(end_date, "%Y-%m-%d")
+        - datetime.strptime(start_date, "%Y-%m-%d")
+    ).days
+
+    lock = Lock()
+
+    if data_type == "steps":
+        api_func = api.get_steps_data
+    elif data_type == "hrs":
+        api_func = api.get_heart_rates
+    elif data_type == "brpms":
+        api_func = api.get_respiration_data
+    elif data_type == "dates":
+        # no API interaction here
+        return [
+            datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=i)
+            for i in tqdm(range(num_days))
+        ]
+
+    arr = []
+
+    # create a thread per each day, and assign it
+    # to fetch the data for that day
+    print("configuring threads...")
+    threads = []
+
+    for i in tqdm(range(num_days)):
+        new_date = datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=i)
+
+        new_thread = Thread(target=fetch_day_data, args=(new_date, arr, api_func, lock))
+
+        threads.append(new_thread)
+
+    # start threads
+    for thread in threads:
+        thread.start()
+
+    # wait for all threads to terminate
+    print("Main thread waiting for child threads...")
+    for thread in tqdm(threads):
+        thread.join()
+
+    # report the number of items in the list
+    print("\ndone")
+
+    return arr
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/garmin/fenix_gen.py` & `wearipedia-0.1.3/wearipedia/devices/garmin/fenix_gen.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,420 +1,420 @@
-from datetime import datetime, timedelta
-
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-
-__all__ = ["create_syn_data"]
-
-
-################
-# some helpers #
-################
-
-
-def get_act_level(steps):
-    """Heuristically determine the activity level based on the number of steps.
-
-    :param steps: number of steps
-    :type steps: int
-    :return: activity level
-    :rtype: str
-    """
-    if steps < 100:
-        return "sedentary"
-    else:
-        return "active"
-
-
-def get_start_end(start_remove, remove_duration, mult):
-    """Only used in the code that randomly deletes data (for missing data simulation purposes).
-    This function computes the index of the first and last elements to remove.
-
-    :param start_remove: point in time to start removing data
-    :type start_remove: float
-    :param remove_duration: point in time to stop removing data
-    :type remove_duration: float
-    :param mult: multiplier, meaning the number of chunks per hour
-    :type mult: int
-    :return: tuple of start and end indices
-    :rtype: Tuple[int, int]
-    """
-    # we just multiply by `mult` and then round to the nearest integer
-    return int(start_remove * mult), int((start_remove + remove_duration) * mult)
-
-
-def get_steps(start_date, num_days):
-    """Generate steps data for a given number of days.
-
-    :return: steps data, a list of lists, where each list represents a single day, and each
-        list contains a many steps values throughout the day marked by timestamp.
-    :rtype: List[List]
-    """
-    steps_synth = []
-
-    # num_step_elems represents the number of 15-minute chunks in a day
-    num_step_elems = 96
-
-    for day_idx in range(num_days):
-
-        # sample the number of steps for this chunk for each
-        # activity level as Poisson
-        sedentary_poi = np.random.poisson(20, size=num_step_elems)
-        medium_poi = np.random.poisson(500, size=num_step_elems)
-        high_poi = np.random.poisson(1500, size=num_step_elems)
-
-        # the below code samples from a Markov chain with 3 states:
-        # 1. "sedentary"
-        # 2. "medium"
-        # 3. "high"
-        # the transition probabilities were heuristically determined
-
-        mask = []
-        cur_state = 0
-        for i in range(num_step_elems):
-            # draw from a uniform distribution
-            rand_draw = np.random.randn()
-
-            # now transition to the next state
-            if cur_state == 0:
-                if rand_draw < 0.9:
-                    cur_state = 0
-                elif rand_draw < 0.97:
-                    cur_state = 1
-                else:
-                    cur_state = 2
-            elif cur_state == 1:
-                if rand_draw < 0.6:
-                    cur_state = 1
-                elif rand_draw < 0.8:
-                    cur_state = 2
-                else:
-                    cur_state = 0
-            elif cur_state == 2:
-                if rand_draw < 0.4:
-                    cur_state = 2
-                elif rand_draw < 0.8:
-                    cur_state = 1
-                else:
-                    cur_state = 0
-
-            # record the state
-            mask.append(cur_state)
-
-        # just overwrite the values for the "sedentary" state
-        # and save this as synth_steps_day
-        medium_idxes = np.where(np.array(mask) == 1)[0]
-        high_idxes = np.where(np.array(mask) == 2)[0]
-
-        sedentary_poi[medium_idxes] = medium_poi[medium_idxes]
-        sedentary_poi[high_idxes] = high_poi[high_idxes]
-
-        # convert to regular int, no need for np.int64
-        synth_steps_day = [int(synth_step) for synth_step in sedentary_poi]
-
-        # compute the start and end timestamps for each 15-minute chunk
-        start_gmts = [
-            datetime.strptime(start_date, "%Y-%m-%d")
-            + timedelta(days=day_idx, hours=7, minutes=15 * i)
-            for i in range(num_step_elems)
-        ]
-
-        end_gmts = [start_gmt + timedelta(minutes=15) for start_gmt in start_gmts]
-
-        # just heuristically determine the activity level for each chunk
-        # based on the number of steps
-        primary_activity_levels = [
-            get_act_level(synth_step) for synth_step in synth_steps_day
-        ]
-
-        # just set everything to be true
-        activity_level_constants = [True] * num_step_elems
-
-        # put everything into a list of dictionaries
-        steps_arrdict_day = [
-            {
-                "startGMT": start_gmt,
-                "endGMT": end_gmt,
-                "steps": synth_step,
-                "primaryActivityLevel": primary_activity_level,
-                "activityLevelConstant": activity_level_constant,
-            }
-            for start_gmt, end_gmt, synth_step, primary_activity_level, activity_level_constant in zip(
-                start_gmts,
-                end_gmts,
-                synth_steps_day,
-                primary_activity_levels,
-                activity_level_constants,
-            )
-        ]
-
-        steps_synth.append(steps_arrdict_day)
-
-    return steps_synth
-
-
-def get_hrs(start_date, num_days, steps_synth):
-    """Get synthetic heart rate data for a given number of days, based on the steps data that
-    has already been generated.
-
-    :param steps_synth: step data outputted from get_steps()
-    :type steps_synth: List[List[Dict]]
-    :return: heart rate data, a list of dictionaries, where each dictionary represents a
-        single day, and each dictionary contains a list of heart rate values throughout the day
-        marked by timestamp.
-    :rtype: List[Dict]
-    """
-
-    synth_hrs = []
-
-    for day_idx in tqdm(range(num_days)):
-        # the heart rate values are represented by a list of 2-minute chunks,
-        # so here we compute the timestamps for all 2-minute chunks in a day
-
-        num_hr_elems = int(24 * (60 // 2))
-
-        hr_timestamps = [
-            datetime.strptime(start_date, "%Y-%m-%d")
-            + timedelta(days=day_idx, hours=7, minutes=2 * i)
-            for i in range(num_hr_elems)
-        ]
-
-        steps_arrdict_day = steps_synth[day_idx]
-
-        hr_vals = []
-
-        for hr_timestamp in hr_timestamps:
-            # first get the steps 15-minute chunk corresponding to this heart rate timestamp
-            step_timestamps = np.array(
-                [x["startGMT"].timestamp() for x in steps_arrdict_day]
-            )
-
-            step_idx = np.where(
-                np.logical_and(
-                    hr_timestamp.timestamp() >= step_timestamps,
-                    hr_timestamp.timestamp() <= step_timestamps + 15 * 60,
-                )
-            )[0][0]
-
-            step_val_avg = steps_arrdict_day[step_idx]["steps"]
-
-            # compute the heart rate as a linear function of the number of steps,
-            # then add a small amount of noise (coefficients heuristically determined)
-            hr_val = int(step_val_avg * 0.03 + 80 + np.random.randn() * 5)
-
-            # multiply by 1000 since the API outputs in milliseconds
-            hr_vals.append([int(hr_timestamp.timestamp()) * 1000, hr_val])
-
-        # get the current day as a string
-        date = datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=day_idx)
-        date_str = datetime.strftime(date, "%Y-%m-%d")
-
-        hr_day_dict = {
-            "userProfilePK": 104779225,  # this was just copied from the real data
-            "calendarDate": date_str,
-            # this is a bit of hardcoding because of California (7 hours behind GMT)
-            "startTimestampGMT": f"{date_str}T07:00:00.0",
-            # again, hardcoding (but offset by a day)
-            "endTimestampGMT": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T07:00:00.0',
-            # obviously no need to adjust here, it's just midnight
-            "startTimestampLocal": f"{date_str}T00:00:00.0",
-            # again, midnight (but offset by a day)
-            "endTimestampLocal": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T00:00:00.0',
-            # just manually computed from our heart rate values
-            "maxHeartRate": max([hr_val[1] for hr_val in hr_vals]),
-            "minHeartRate": min([hr_val[1] for hr_val in hr_vals]),
-            "restingHeartRate": 60,  # hard code
-            "lastSevenDaysAvgRestingHeartRate": 60,  # hard code
-            # copied from real API output
-            "heartRateValueDescriptors": [
-                {"key": "timestamp", "index": 0},
-                {"key": "heartrate", "index": 1},
-            ],
-            # just the values we obtained earlier
-            "heartRateValues": hr_vals,
-        }
-
-        synth_hrs.append(hr_day_dict)
-
-    return synth_hrs
-
-
-def get_brpms(start_date, num_days, synth_hrs):
-    """Generate synthetic breath rate per minute data.
-
-    This function is fairly straightforward.
-
-    :param synth_hrs: list of dicts, each dict is a day of heart rate data
-    :type synth_hrs: List[Dict]
-    :return: breath rate per minute data, a list of dictionaries, where each dictionary
-        represents a single day, and each dictionary contains a list of breath rate per
-        minute values throughout the day marked by timestamp.
-    :rtype: List[Dict]
-    """
-    synth_brpms = []
-
-    for day_idx in tqdm(range(num_days)):
-        # since the sample rate for breaths per minute is exactly the same
-        # as for heart rate, we can just copy the heart rate timestamps
-        # and generate breaths per minute values based on the heart rate values
-        # (with a linear function)
-        synth_hr_vals = synth_hrs[day_idx]["heartRateValues"]
-        synth_brpm_vals = [
-            [synth_hr_val[0], int(synth_hr_val[1] * 0.1 + 5)]
-            for synth_hr_val in synth_hr_vals
-        ]
-
-        # just get the date as a string
-        date = datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=day_idx)
-        date_str = datetime.strftime(date, "%Y-%m-%d")
-
-        brpm_dict = {
-            # copied from real API output
-            "userProfilePK": 104779225,
-            "calendarDate": date_str,
-            # this is a bit of hardcoding because of California (7 hours behind GMT)
-            "startTimestampGMT": f"{date_str}T07:00:00.0",
-            # again, hardcoding (but offset by a day)
-            "endTimestampGMT": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T07:00:00.0',
-            # obviously no need to adjust here, it's just midnight
-            "startTimestampLocal": f"{date_str}T00:00:00.0",
-            # again, midnight (but offset by a day)
-            "endTimestampLocal": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T00:00:00.0',
-            # all the stuff below is just copied from the real API output
-            "sleepStartTimestampGMT": None,
-            "sleepEndTimestampGMT": None,
-            "sleepStartTimestampLocal": None,
-            "sleepEndTimestampLocal": None,
-            "tomorrowSleepStartTimestampGMT": None,
-            "tomorrowSleepEndTimestampGMT": None,
-            "tomorrowSleepStartTimestampLocal": None,
-            "tomorrowSleepEndTimestampLocal": None,
-            "lowestRespirationValue": 12.0,
-            "highestRespirationValue": 23.0,
-            "avgWakingRespirationValue": 15.0,
-            "avgSleepRespirationValue": None,
-            "avgTomorrowSleepRespirationValue": None,
-            "respirationValueDescriptorsDTOList": [
-                {"key": "timestamp", "index": 0},
-                {"key": "respiration", "index": 1},
-            ],
-            # just the values we obtained earlier
-            "respirationValuesArray": synth_brpm_vals,
-        }
-
-        synth_brpms.append(brpm_dict)
-
-    return synth_brpms
-
-
-def delete_stuff(dates, steps, hrs, brpms):
-    """Delete stuff randomly, since we want to simulate missing data.
-
-    :param dates: List of dates (each date is a separate day represented as a string)
-    :type dates: List[str]
-    :param steps: List of step data (each element is a list of dictionaries, each dictionary
-        represents the step data for a 15-minute chunk of time in the day)
-    :type steps: List[List[Dict]]
-    :param hrs: List of heart rate data (each element is a dictionary)
-    :type hrs: List[Dict]
-    :param brpms: List of breathing rate data (each element is a dictionary)
-    :type brpms: List[Dict]
-    :return: List of dates, List of step data, List of heart rate data, List of breathing rate data
-    :rtype: Tuple[List[str], List[Dict], List[Dict], List[Dict]]
-    """
-
-    num_days = len(dates)  # we can just use the length of the dates list
-
-    for day_idx in tqdm(range(num_days)):
-        # the duration to remove (in hours) is sampled from an exponential distribution,
-        # except we truncate the undesirable long tails of the distribution
-        remove_duration = np.clip(np.random.exponential(3), 0, 16)
-
-        # we remove everything after a certain time, so compute the
-        # start of that
-        start_remove = np.random.uniform(0, 24 - remove_duration)
-
-        # compute the index of the first and last elements to remove,
-        # note that we provide 30 because heart rate and breath rate
-        # is sampled every 2 minutes, so there are 30 samples per hour
-        start_idx, end_idx = get_start_end(start_remove, remove_duration, 30)
-
-        # Just slice and replace the middle part with a filler element,
-        # which just contains None (this is what the API would return
-        # when there is missing data). We do this for all the data types.
-        filler = [hrs[day_idx]["heartRateValues"][start_idx][0], None]
-        hrs[day_idx]["heartRateValues"] = (
-            hrs[day_idx]["heartRateValues"][:start_idx]
-            + [filler]
-            + hrs[day_idx]["heartRateValues"][end_idx:]
-        )
-        filler = [brpms[day_idx]["respirationValuesArray"][start_idx][0], None]
-        brpms[day_idx]["respirationValuesArray"] = (
-            brpms[day_idx]["respirationValuesArray"][:start_idx]
-            + [filler]
-            + brpms[day_idx]["respirationValuesArray"][end_idx:]
-        )
-
-        # provide 4 because steps are sampled every 15 minutes,
-        # so there are 4 samples per hour
-        start_idx, end_idx = get_start_end(start_remove, remove_duration, 4)
-
-        steps[day_idx] = steps[day_idx][:start_idx] + steps[day_idx][end_idx:]
-
-    return dates, steps, hrs, brpms
-
-
-def create_syn_data(start_date, end_date):
-    """Returns a tuple of dates, steps, heart rates, and breath rates. The data
-    format is as follows. Each element in the tuple is a list of length num_days.
-    For each tuple:
-    - dates: List of dates (each date is a separate day represented as a string)
-    - steps: List of step data (each element is a list of dictionaries, each dictionary
-        represents the step data for a 15-minute chunk of time in the day)
-    - heart rates: List of heart rate data (each element is a dictionary)
-    - breath rates: List of breathing rate data (each element is a dictionary)
-
-    :param start_date: the start date (inclusive) as a string in the format "YYYY-MM-DD"
-    :type start_date: str
-    :param end_date: the end date (inclusive) as a string in the format "YYYY-MM-DD"
-    :type end_date: str
-    :return: A four-tuple of dates, steps, heart rates, and breath rates, each
-        of which is just a list where each element represents a particular day.
-    :rtype: Tuple[List[str], List[List[Dict]], List[Dict], List[Dict]]
-    """
-
-    num_days = (
-        datetime.strptime(end_date, "%Y-%m-%d")
-        - datetime.strptime(start_date, "%Y-%m-%d")
-    ).days
-
-    # first get the dates as datetime objects
-    synth_dates = [
-        datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=i)
-        for i in range(num_days)
-    ]
-
-    # process is to first get the steps, then the heart rate (since you can just compute
-    # the heart rate from the steps), then the breathing rate (since you can just compute
-    # the breathing rate from the heart rate)
-    synth_steps = get_steps(start_date, num_days)
-    synth_hrs = get_hrs(start_date, num_days, synth_steps)
-    synth_brpms = get_brpms(start_date, num_days, synth_hrs)
-
-    # finally, we just iterate over the steps and
-    # turn the start and end timestamps to strings
-    for i, synth_steps_day in enumerate(synth_steps):
-        for j in range(len(synth_steps_day)):
-            synth_steps[i][j]["startGMT"] = datetime.strftime(
-                synth_steps[i][j]["startGMT"], "%Y-%m-%dT%H:%M:%S"
-            )
-            synth_steps[i][j]["endGMT"] = datetime.strftime(
-                synth_steps[i][j]["endGMT"], "%Y-%m-%dT%H:%M:%S"
-            )
-
-    # randomly delete stuff (to simulate missing data)
-    synth_dates, synth_steps, synth_hrs, synth_brpms = delete_stuff(
-        synth_dates, synth_steps, synth_hrs, synth_brpms
-    )
-
-    return synth_dates, synth_steps, synth_hrs, synth_brpms
+from datetime import datetime, timedelta
+
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+
+__all__ = ["create_syn_data"]
+
+
+################
+# some helpers #
+################
+
+
+def get_act_level(steps):
+    """Heuristically determine the activity level based on the number of steps.
+
+    :param steps: number of steps
+    :type steps: int
+    :return: activity level
+    :rtype: str
+    """
+    if steps < 100:
+        return "sedentary"
+    else:
+        return "active"
+
+
+def get_start_end(start_remove, remove_duration, mult):
+    """Only used in the code that randomly deletes data (for missing data simulation purposes).
+    This function computes the index of the first and last elements to remove.
+
+    :param start_remove: point in time to start removing data
+    :type start_remove: float
+    :param remove_duration: point in time to stop removing data
+    :type remove_duration: float
+    :param mult: multiplier, meaning the number of chunks per hour
+    :type mult: int
+    :return: tuple of start and end indices
+    :rtype: Tuple[int, int]
+    """
+    # we just multiply by `mult` and then round to the nearest integer
+    return int(start_remove * mult), int((start_remove + remove_duration) * mult)
+
+
+def get_steps(start_date, num_days):
+    """Generate steps data for a given number of days.
+
+    :return: steps data, a list of lists, where each list represents a single day, and each
+        list contains a many steps values throughout the day marked by timestamp.
+    :rtype: List[List]
+    """
+    steps_synth = []
+
+    # num_step_elems represents the number of 15-minute chunks in a day
+    num_step_elems = 96
+
+    for day_idx in range(num_days):
+
+        # sample the number of steps for this chunk for each
+        # activity level as Poisson
+        sedentary_poi = np.random.poisson(20, size=num_step_elems)
+        medium_poi = np.random.poisson(500, size=num_step_elems)
+        high_poi = np.random.poisson(1500, size=num_step_elems)
+
+        # the below code samples from a Markov chain with 3 states:
+        # 1. "sedentary"
+        # 2. "medium"
+        # 3. "high"
+        # the transition probabilities were heuristically determined
+
+        mask = []
+        cur_state = 0
+        for i in range(num_step_elems):
+            # draw from a uniform distribution
+            rand_draw = np.random.randn()
+
+            # now transition to the next state
+            if cur_state == 0:
+                if rand_draw < 0.9:
+                    cur_state = 0
+                elif rand_draw < 0.97:
+                    cur_state = 1
+                else:
+                    cur_state = 2
+            elif cur_state == 1:
+                if rand_draw < 0.6:
+                    cur_state = 1
+                elif rand_draw < 0.8:
+                    cur_state = 2
+                else:
+                    cur_state = 0
+            elif cur_state == 2:
+                if rand_draw < 0.4:
+                    cur_state = 2
+                elif rand_draw < 0.8:
+                    cur_state = 1
+                else:
+                    cur_state = 0
+
+            # record the state
+            mask.append(cur_state)
+
+        # just overwrite the values for the "sedentary" state
+        # and save this as synth_steps_day
+        medium_idxes = np.where(np.array(mask) == 1)[0]
+        high_idxes = np.where(np.array(mask) == 2)[0]
+
+        sedentary_poi[medium_idxes] = medium_poi[medium_idxes]
+        sedentary_poi[high_idxes] = high_poi[high_idxes]
+
+        # convert to regular int, no need for np.int64
+        synth_steps_day = [int(synth_step) for synth_step in sedentary_poi]
+
+        # compute the start and end timestamps for each 15-minute chunk
+        start_gmts = [
+            datetime.strptime(start_date, "%Y-%m-%d")
+            + timedelta(days=day_idx, hours=7, minutes=15 * i)
+            for i in range(num_step_elems)
+        ]
+
+        end_gmts = [start_gmt + timedelta(minutes=15) for start_gmt in start_gmts]
+
+        # just heuristically determine the activity level for each chunk
+        # based on the number of steps
+        primary_activity_levels = [
+            get_act_level(synth_step) for synth_step in synth_steps_day
+        ]
+
+        # just set everything to be true
+        activity_level_constants = [True] * num_step_elems
+
+        # put everything into a list of dictionaries
+        steps_arrdict_day = [
+            {
+                "startGMT": start_gmt,
+                "endGMT": end_gmt,
+                "steps": synth_step,
+                "primaryActivityLevel": primary_activity_level,
+                "activityLevelConstant": activity_level_constant,
+            }
+            for start_gmt, end_gmt, synth_step, primary_activity_level, activity_level_constant in zip(
+                start_gmts,
+                end_gmts,
+                synth_steps_day,
+                primary_activity_levels,
+                activity_level_constants,
+            )
+        ]
+
+        steps_synth.append(steps_arrdict_day)
+
+    return steps_synth
+
+
+def get_hrs(start_date, num_days, steps_synth):
+    """Get synthetic heart rate data for a given number of days, based on the steps data that
+    has already been generated.
+
+    :param steps_synth: step data outputted from get_steps()
+    :type steps_synth: List[List[Dict]]
+    :return: heart rate data, a list of dictionaries, where each dictionary represents a
+        single day, and each dictionary contains a list of heart rate values throughout the day
+        marked by timestamp.
+    :rtype: List[Dict]
+    """
+
+    synth_hrs = []
+
+    for day_idx in tqdm(range(num_days)):
+        # the heart rate values are represented by a list of 2-minute chunks,
+        # so here we compute the timestamps for all 2-minute chunks in a day
+
+        num_hr_elems = int(24 * (60 // 2))
+
+        hr_timestamps = [
+            datetime.strptime(start_date, "%Y-%m-%d")
+            + timedelta(days=day_idx, hours=7, minutes=2 * i)
+            for i in range(num_hr_elems)
+        ]
+
+        steps_arrdict_day = steps_synth[day_idx]
+
+        hr_vals = []
+
+        for hr_timestamp in hr_timestamps:
+            # first get the steps 15-minute chunk corresponding to this heart rate timestamp
+            step_timestamps = np.array(
+                [x["startGMT"].timestamp() for x in steps_arrdict_day]
+            )
+
+            step_idx = np.where(
+                np.logical_and(
+                    hr_timestamp.timestamp() >= step_timestamps,
+                    hr_timestamp.timestamp() <= step_timestamps + 15 * 60,
+                )
+            )[0][0]
+
+            step_val_avg = steps_arrdict_day[step_idx]["steps"]
+
+            # compute the heart rate as a linear function of the number of steps,
+            # then add a small amount of noise (coefficients heuristically determined)
+            hr_val = int(step_val_avg * 0.03 + 80 + np.random.randn() * 5)
+
+            # multiply by 1000 since the API outputs in milliseconds
+            hr_vals.append([int(hr_timestamp.timestamp()) * 1000, hr_val])
+
+        # get the current day as a string
+        date = datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=day_idx)
+        date_str = datetime.strftime(date, "%Y-%m-%d")
+
+        hr_day_dict = {
+            "userProfilePK": 104779225,  # this was just copied from the real data
+            "calendarDate": date_str,
+            # this is a bit of hardcoding because of California (7 hours behind GMT)
+            "startTimestampGMT": f"{date_str}T07:00:00.0",
+            # again, hardcoding (but offset by a day)
+            "endTimestampGMT": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T07:00:00.0',
+            # obviously no need to adjust here, it's just midnight
+            "startTimestampLocal": f"{date_str}T00:00:00.0",
+            # again, midnight (but offset by a day)
+            "endTimestampLocal": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T00:00:00.0',
+            # just manually computed from our heart rate values
+            "maxHeartRate": max([hr_val[1] for hr_val in hr_vals]),
+            "minHeartRate": min([hr_val[1] for hr_val in hr_vals]),
+            "restingHeartRate": 60,  # hard code
+            "lastSevenDaysAvgRestingHeartRate": 60,  # hard code
+            # copied from real API output
+            "heartRateValueDescriptors": [
+                {"key": "timestamp", "index": 0},
+                {"key": "heartrate", "index": 1},
+            ],
+            # just the values we obtained earlier
+            "heartRateValues": hr_vals,
+        }
+
+        synth_hrs.append(hr_day_dict)
+
+    return synth_hrs
+
+
+def get_brpms(start_date, num_days, synth_hrs):
+    """Generate synthetic breath rate per minute data.
+
+    This function is fairly straightforward.
+
+    :param synth_hrs: list of dicts, each dict is a day of heart rate data
+    :type synth_hrs: List[Dict]
+    :return: breath rate per minute data, a list of dictionaries, where each dictionary
+        represents a single day, and each dictionary contains a list of breath rate per
+        minute values throughout the day marked by timestamp.
+    :rtype: List[Dict]
+    """
+    synth_brpms = []
+
+    for day_idx in tqdm(range(num_days)):
+        # since the sample rate for breaths per minute is exactly the same
+        # as for heart rate, we can just copy the heart rate timestamps
+        # and generate breaths per minute values based on the heart rate values
+        # (with a linear function)
+        synth_hr_vals = synth_hrs[day_idx]["heartRateValues"]
+        synth_brpm_vals = [
+            [synth_hr_val[0], int(synth_hr_val[1] * 0.1 + 5)]
+            for synth_hr_val in synth_hr_vals
+        ]
+
+        # just get the date as a string
+        date = datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=day_idx)
+        date_str = datetime.strftime(date, "%Y-%m-%d")
+
+        brpm_dict = {
+            # copied from real API output
+            "userProfilePK": 104779225,
+            "calendarDate": date_str,
+            # this is a bit of hardcoding because of California (7 hours behind GMT)
+            "startTimestampGMT": f"{date_str}T07:00:00.0",
+            # again, hardcoding (but offset by a day)
+            "endTimestampGMT": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T07:00:00.0',
+            # obviously no need to adjust here, it's just midnight
+            "startTimestampLocal": f"{date_str}T00:00:00.0",
+            # again, midnight (but offset by a day)
+            "endTimestampLocal": f'{datetime.strftime(date + timedelta(days=1), "%Y-%m-%d")}T00:00:00.0',
+            # all the stuff below is just copied from the real API output
+            "sleepStartTimestampGMT": None,
+            "sleepEndTimestampGMT": None,
+            "sleepStartTimestampLocal": None,
+            "sleepEndTimestampLocal": None,
+            "tomorrowSleepStartTimestampGMT": None,
+            "tomorrowSleepEndTimestampGMT": None,
+            "tomorrowSleepStartTimestampLocal": None,
+            "tomorrowSleepEndTimestampLocal": None,
+            "lowestRespirationValue": 12.0,
+            "highestRespirationValue": 23.0,
+            "avgWakingRespirationValue": 15.0,
+            "avgSleepRespirationValue": None,
+            "avgTomorrowSleepRespirationValue": None,
+            "respirationValueDescriptorsDTOList": [
+                {"key": "timestamp", "index": 0},
+                {"key": "respiration", "index": 1},
+            ],
+            # just the values we obtained earlier
+            "respirationValuesArray": synth_brpm_vals,
+        }
+
+        synth_brpms.append(brpm_dict)
+
+    return synth_brpms
+
+
+def delete_stuff(dates, steps, hrs, brpms):
+    """Delete stuff randomly, since we want to simulate missing data.
+
+    :param dates: List of dates (each date is a separate day represented as a string)
+    :type dates: List[str]
+    :param steps: List of step data (each element is a list of dictionaries, each dictionary
+        represents the step data for a 15-minute chunk of time in the day)
+    :type steps: List[List[Dict]]
+    :param hrs: List of heart rate data (each element is a dictionary)
+    :type hrs: List[Dict]
+    :param brpms: List of breathing rate data (each element is a dictionary)
+    :type brpms: List[Dict]
+    :return: List of dates, List of step data, List of heart rate data, List of breathing rate data
+    :rtype: Tuple[List[str], List[Dict], List[Dict], List[Dict]]
+    """
+
+    num_days = len(dates)  # we can just use the length of the dates list
+
+    for day_idx in tqdm(range(num_days)):
+        # the duration to remove (in hours) is sampled from an exponential distribution,
+        # except we truncate the undesirable long tails of the distribution
+        remove_duration = np.clip(np.random.exponential(3), 0, 16)
+
+        # we remove everything after a certain time, so compute the
+        # start of that
+        start_remove = np.random.uniform(0, 24 - remove_duration)
+
+        # compute the index of the first and last elements to remove,
+        # note that we provide 30 because heart rate and breath rate
+        # is sampled every 2 minutes, so there are 30 samples per hour
+        start_idx, end_idx = get_start_end(start_remove, remove_duration, 30)
+
+        # Just slice and replace the middle part with a filler element,
+        # which just contains None (this is what the API would return
+        # when there is missing data). We do this for all the data types.
+        filler = [hrs[day_idx]["heartRateValues"][start_idx][0], None]
+        hrs[day_idx]["heartRateValues"] = (
+            hrs[day_idx]["heartRateValues"][:start_idx]
+            + [filler]
+            + hrs[day_idx]["heartRateValues"][end_idx:]
+        )
+        filler = [brpms[day_idx]["respirationValuesArray"][start_idx][0], None]
+        brpms[day_idx]["respirationValuesArray"] = (
+            brpms[day_idx]["respirationValuesArray"][:start_idx]
+            + [filler]
+            + brpms[day_idx]["respirationValuesArray"][end_idx:]
+        )
+
+        # provide 4 because steps are sampled every 15 minutes,
+        # so there are 4 samples per hour
+        start_idx, end_idx = get_start_end(start_remove, remove_duration, 4)
+
+        steps[day_idx] = steps[day_idx][:start_idx] + steps[day_idx][end_idx:]
+
+    return dates, steps, hrs, brpms
+
+
+def create_syn_data(start_date, end_date):
+    """Returns a tuple of dates, steps, heart rates, and breath rates. The data
+    format is as follows. Each element in the tuple is a list of length num_days.
+    For each tuple:
+    - dates: List of dates (each date is a separate day represented as a string)
+    - steps: List of step data (each element is a list of dictionaries, each dictionary
+        represents the step data for a 15-minute chunk of time in the day)
+    - heart rates: List of heart rate data (each element is a dictionary)
+    - breath rates: List of breathing rate data (each element is a dictionary)
+
+    :param start_date: the start date (inclusive) as a string in the format "YYYY-MM-DD"
+    :type start_date: str
+    :param end_date: the end date (inclusive) as a string in the format "YYYY-MM-DD"
+    :type end_date: str
+    :return: A four-tuple of dates, steps, heart rates, and breath rates, each
+        of which is just a list where each element represents a particular day.
+    :rtype: Tuple[List[str], List[List[Dict]], List[Dict], List[Dict]]
+    """
+
+    num_days = (
+        datetime.strptime(end_date, "%Y-%m-%d")
+        - datetime.strptime(start_date, "%Y-%m-%d")
+    ).days
+
+    # first get the dates as datetime objects
+    synth_dates = [
+        datetime.strptime(start_date, "%Y-%m-%d") + timedelta(days=i)
+        for i in range(num_days)
+    ]
+
+    # process is to first get the steps, then the heart rate (since you can just compute
+    # the heart rate from the steps), then the breathing rate (since you can just compute
+    # the breathing rate from the heart rate)
+    synth_steps = get_steps(start_date, num_days)
+    synth_hrs = get_hrs(start_date, num_days, synth_steps)
+    synth_brpms = get_brpms(start_date, num_days, synth_hrs)
+
+    # finally, we just iterate over the steps and
+    # turn the start and end timestamps to strings
+    for i, synth_steps_day in enumerate(synth_steps):
+        for j in range(len(synth_steps_day)):
+            synth_steps[i][j]["startGMT"] = datetime.strftime(
+                synth_steps[i][j]["startGMT"], "%Y-%m-%dT%H:%M:%S"
+            )
+            synth_steps[i][j]["endGMT"] = datetime.strftime(
+                synth_steps[i][j]["endGMT"], "%Y-%m-%dT%H:%M:%S"
+            )
+
+    # randomly delete stuff (to simulate missing data)
+    synth_dates, synth_steps, synth_hrs, synth_brpms = delete_stuff(
+        synth_dates, synth_steps, synth_hrs, synth_brpms
+    )
+
+    return synth_dates, synth_steps, synth_hrs, synth_brpms
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/polar/verity_gen.py` & `wearipedia-0.1.3/wearipedia/devices/polar/verity_gen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-import copy
-from threading import Thread
-
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-
-
-def gen_data(seed, start_date, end_date):
-    """Main function for creating synthetic heart rate data for the Verity Sense.
-
-    :param start_date: the start date represented as a string in the format "YYYY-MM-DD"
-    :type start_date: str
-    :param end_date: the end date represented as a string in the format "YYYY-MM-DD"
-    :type end_date: str
-    :return: a dictionary with keys the training session dates and values a dictionary with keys heart_rates, calories, and minutes
-    :rtype: Dict[str: Dict[str: list, str: int, str: int]]
-    """
-    np.random.seed(seed)
-    sessions = np.datetime64(end_date) - np.datetime64(start_date)
-    durations = (45, 60)  # minutes
-
-    def gen_session(result, index):
-        # simulate skip day
-        if np.random.uniform(low=0, high=1, size=(1,))[0] > 0.8:
-            return
-
-        # day that you workout
-        day = np.datetime64(start_date) + np.timedelta64(index, "D")
-        duration = int(
-            np.random.uniform(low=durations[0], high=durations[1], size=(1,))[0]
-        )
-        hrate = []
-        start_rate = np.random.uniform(low=70, high=110, size=(1,))[0]
-        for _ in range(duration * 60):
-            hrate.append(start_rate)
-            added = np.random.normal(scale=1) + 0.01 * (160 / start_rate)
-            if start_rate < 50:
-                added = abs(added)
-            elif start_rate > 190:
-                added = -1 * abs(added)
-            start_rate += added
-        result[pd.to_datetime(day).strftime("%Y-%m-%d")] = {
-            "heart_rates": copy.deepcopy(hrate),
-            "calories": int(np.random.uniform(low=200, high=500, size=(1,))[0]),
-            "minutes": duration,
-        }
-
-    threads = []
-    result = {}
-    for i in tqdm(range(int(sessions / np.timedelta64(1, "D")))):
-        new_thread = Thread(target=gen_session, args=(result, i))
-        threads.append(new_thread)
-
-    # start threads
-    for thread in threads:
-        thread.start()
-
-    # wait for all threads to terminate
-    for thread in tqdm(threads):
-        thread.join()
-
-    return result
+import copy
+import datetime
+from collections import defaultdict
+from threading import Thread
+
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+
+
+def gen_data(seed, start_date, end_date):
+    """Main function for creating synthetic heart rate data for the Verity Sense.
+
+    :param start_date: the start date represented as a string in the format "YYYY-MM-DD"
+    :type start_date: str
+    :param end_date: the end date represented as a string in the format "YYYY-MM-DD"
+    :type end_date: str
+    :return: a dictionary with keys the training session dates and values a dictionary with keys heart_rates, calories, and minutes
+    :rtype: Dict[str: Dict[str: list, str: int, str: int]]
+    """
+    sessions = np.datetime64(end_date) - np.datetime64(start_date)
+    durations = (45, 60)  # minutes
+
+    def gen_session(result, index):
+        local_rng = np.random.RandomState(seed + index)
+
+        # simulate skip day
+        if local_rng.uniform(low=0, high=1, size=(1,))[0] > 0.8:
+            return
+
+        # day that you workout
+        day = np.datetime64(start_date) + np.timedelta64(index, "D")
+        duration = int(
+            local_rng.uniform(low=durations[0], high=durations[1], size=(1,))[0]
+        )
+        hrate = []
+        start_rate = local_rng.uniform(low=70, high=110, size=(1,))[0]
+
+        for _ in range(duration * 60):
+            hrate.append(start_rate)
+            added = local_rng.normal(scale=1) + 0.01 * (160 / start_rate)
+            if start_rate < 50:
+                added = abs(added)
+            elif start_rate > 190:
+                added = -1 * abs(added)
+            start_rate += added
+
+        result[pd.to_datetime(day).strftime("%Y-%m-%d")]["heart_rates"] = copy.deepcopy(
+            hrate
+        )
+        result[pd.to_datetime(day).strftime("%Y-%m-%d")]["calories"] = int(
+            local_rng.uniform(low=200, high=500, size=(1,))[0]
+        )
+        result[pd.to_datetime(day).strftime("%Y-%m-%d")]["minutes"] = duration
+
+    threads = []
+    result = defaultdict(dict)
+    for i in tqdm(range(int(sessions / np.timedelta64(1, "D")))):
+        new_thread = Thread(target=gen_session, args=(result, i))
+
+        threads.append(new_thread)
+
+    # start threads
+    for thread in threads:
+        thread.start()
+
+    # wait for all threads to terminate
+    for thread in tqdm(threads):
+        thread.join()
+
+    return result
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/polar/verity_sense.py` & `wearipedia-0.1.3/wearipedia/devices/polar/verity_sense.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import numpy as np
-import requests
-
-from ...devices.device import BaseDevice
-from .verity_gen import *
-from .verity_get import *
-
-class_name = "VeritySense"
-
-
-class VeritySense(BaseDevice):
-    """This device allows you to work with data from the `Polar Verity Sense <https://www.polar.com/us-en/products/accessories/polar-verity-sense>`_ device.
-    Available datatypes for this device are:
-
-    * `sessions`: contains data from all sessions in one
-
-    :param seed: random seed for synthetic data generation, defaults to 0
-    :type seed: int, optional
-    :param start_date: start date for synthetic data generation, defaults to "2022-03-01"
-    :type start_date: str, optional
-    :param end_date: end date for synthetic data generation, defaults to "2022-06-17"
-    :type end_date: str, optional
-    """
-
-    def __init__(self, seed=0, start_date="2022-03-01", end_date="2022-06-17"):
-
-        params = {
-            "seed": seed,
-            "start_date": start_date,
-            "end_date": end_date,
-        }
-
-        self._initialize_device_params(
-            ["sessions"],
-            params,
-            {
-                "seed": 0,
-                "start_date": "2022-03-01",
-                "end_date": "2022-06-17",
-            },
-        )
-
-    def _default_params(self):
-        return {
-            "start_date": self.init_params["start_date"],
-            "end_date": self.init_params["end_date"],
-        }
-
-    def _get_real(self, data_type, params):
-        return fetch_real_data(
-            params["start_date"],
-            params["end_date"],
-            data_type,
-            self.session,
-            self.post,
-        )
-
-    def _filter_synthetic(self, data, data_type, params):
-        # return data within range of start date and end date
-        result = {}
-        for key in data.keys():
-            if np.datetime64(key) - np.datetime64(params["end_date"]) > 0:
-                break
-            elif np.datetime64(key) - np.datetime64(params["start_date"]) < 0:
-                continue
-            else:
-                result[key] = data[key]
-        return result
-
-    def _gen_synthetic(self):
-        # generate heart rate data according to start and end dates
-        self.sessions = gen_data(
-            self.init_params["seed"],
-            self.init_params["start_date"],
-            self.init_params["end_date"],
-        )
-
-    def _authenticate(self, auth_creds):
-
-        # set credentials for device object to be accessed later if needed
-        self.email = auth_creds["email"]
-        self.password = auth_creds["password"]
-
-        # authenticate device in a python session and save it
-        auth = {"email": self.email, "password": self.password}
-        self.session = requests.Session()
-
-        # contains polar global variables we need later
-        self.post = self.session.post("https://flow.polar.com/login", data=auth)
+import numpy as np
+import requests
+
+from ...devices.device import BaseDevice
+from .polar_get import *
+from .verity_gen import *
+
+class_name = "VeritySense"
+
+
+class VeritySense(BaseDevice):
+    """This device allows you to work with data from the `Polar Verity Sense <https://www.polar.com/us-en/products/accessories/polar-verity-sense>`_ device.
+    Available datatypes for this device are:
+
+    * `sessions`: contains data from all sessions in one
+
+    :param seed: random seed for synthetic data generation, defaults to 0
+    :type seed: int, optional
+    :param start_date: start date for synthetic data generation, defaults to "2022-03-01"
+    :type start_date: str, optional
+    :param end_date: end date for synthetic data generation, defaults to "2022-06-17"
+    :type end_date: str, optional
+    """
+
+    def __init__(self, seed=0, start_date="2022-03-01", end_date="2022-06-17"):
+
+        params = {
+            "seed": seed,
+            "start_date": start_date,
+            "end_date": end_date,
+        }
+
+        self._initialize_device_params(
+            ["sessions"],
+            params,
+            {
+                "seed": 0,
+                "start_date": "2022-03-01",
+                "end_date": "2022-06-17",
+            },
+        )
+
+    def _default_params(self):
+        return {
+            "start_date": self.init_params["start_date"],
+            "end_date": self.init_params["end_date"],
+        }
+
+    def _get_real(self, data_type, params):
+        return fetch_real_data(
+            params["start_date"],
+            params["end_date"],
+            data_type,
+            self.session,
+            self.post,
+        )
+
+    def _filter_synthetic(self, data, data_type, params):
+        # return data within range of start date and end date
+        result = {}
+        for key in data.keys():
+            if np.datetime64(key) - np.datetime64(params["end_date"]) > 0:
+                break
+            elif np.datetime64(key) - np.datetime64(params["start_date"]) < 0:
+                continue
+            else:
+                result[key] = data[key]
+        return result
+
+    def _gen_synthetic(self):
+        # generate heart rate data according to start and end dates
+        self.sessions = gen_data(
+            self.init_params["seed"],
+            self.init_params["start_date"],
+            self.init_params["end_date"],
+        )
+
+    def _authenticate(self, auth_creds):
+
+        # set credentials for device object to be accessed later if needed
+        self.email = auth_creds["email"]
+        self.password = auth_creds["password"]
+
+        # authenticate device in a python session and save it
+        auth = {"email": self.email, "password": self.password}
+        self.session = requests.Session()
+
+        # contains polar global variables we need later
+        self.post = self.session.post("https://flow.polar.com/login", data=auth)
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/whoop/whoop_4.py` & `wearipedia-0.1.3/wearipedia/devices/whoop/whoop_4.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-from datetime import datetime
-
-import numpy as np
-import pandas as pd
-
-from ...devices.device import BaseDevice
-from ...utils import bin_search, seed_everything
-from .whoop_gen import *
-from .whoop_user import *
-
-class_name = "Whoop4"
-
-
-class Whoop4(BaseDevice):
-    """This device allows you to work with data from the `WHOOP 4.0 <https://shop.whoop.com/en-us/collections/whoop4-0/?order_by=featured>`_ device.
-    Available datatypes for this device are:
-
-    * `cycles`: a DataFrame of all cycles (days)
-
-    * `hr`: heart rate data
-
-    :param seed: random seed for synthetic data generation, defaults to 0
-    :type seed: int, optional
-    :param synthetic_start_date: start date for synthetic data generation, defaults to "2022-03-01"
-    :type synthetic_start_date: str, optional
-    :param synthetic_end_date: end date for synthetic data generation, defaults to "2022-06-17"
-    :type synthetic_end_date: str, optional
-    :param use_cache: decide whether to cache the credentials, defaults to True
-    :type use_cache: bool, optional
-    """
-
-    def __init__(
-        self, seed=0, synthetic_start_date="2022-03-01", synthetic_end_date="2022-06-17"
-    ):
-
-        params = {
-            "seed": seed,
-            "synthetic_start_date": synthetic_start_date,
-            "synthetic_end_date": synthetic_end_date,
-        }
-
-        self.data_types_methods_map = {
-            "cycles": "get_cycles_json",
-            "hr": "get_heart_rate_json",
-        }
-
-        self._initialize_device_params(
-            list(self.data_types_methods_map.keys()),
-            params,
-            {
-                "seed": 0,
-                "synthetic_start_date": "2022-03-01",
-                "synthetic_end_date": "2022-06-17",
-            },
-        )
-
-    def _default_params(self):
-        params = {
-            "start": "2022-04-24T00:00:00.000Z",
-            "end": "2022-04-28T00:00:00.000Z",
-        }
-
-        return params
-
-    def _get_real(self, data_type, params):
-        api_func = getattr(self.user, self.data_types_methods_map[data_type])
-        return api_func(params)
-
-    def _filter_synthetic(self, data, data_type, params):
-        # Here we just return the data we've already generated,
-        # but index into it based on the params. Specifically, we
-        # want to return the data between the start and end dates.
-
-        if data_type != "hr":
-            # synthetic data is generated day-by-day, so we can just
-            # index into it based on the start and end dates
-
-            date_str_to_obj = lambda x: datetime.strptime(x, "%Y-%m-%d")
-            datetime_str_to_obj = lambda x: datetime.strptime(
-                x, "%Y-%m-%dT%H:%M:%S.%fZ"
-            )
-
-            # get the indices by subtracting against the start of the synthetic data
-            synthetic_start = date_str_to_obj(self.init_params["synthetic_start_date"])
-
-            start_idx = (datetime_str_to_obj(params["start"]) - synthetic_start).days
-            end_idx = (datetime_str_to_obj(params["end"]) - synthetic_start).days
-
-            cycles = {
-                "total_count": end_idx - start_idx,
-                "offset": end_idx - start_idx,
-                "records": data["records"][start_idx:end_idx],
-            }
-
-            return cycles
-
-        else:
-            # hr data is generated in 7 second intervals, so we need to
-            # do a binary search to find the start and end indices
-            # and then return the data between those indices
-
-            start_ts = pd.Timestamp(params["start"]).timestamp()
-            end_ts = pd.Timestamp(params["end"]).timestamp()
-
-            vals = np.array([val["time"] for val in data["values"]])
-
-            start_idx = bin_search(vals, start_ts)
-            end_idx = bin_search(vals, end_ts)
-
-            return {
-                "name": "heart_rate",
-                "start": data["values"][start_idx]["time"],
-                "values": data["values"][start_idx:end_idx],
-            }
-
-    def _gen_synthetic(self):
-        # generate random data according to seed
-        seed_everything(self.init_params["seed"])
-
-        self.cycles = create_fake_cycles(
-            datetime.strptime(self.init_params["synthetic_start_date"], "%Y-%m-%d"),
-            datetime.strptime(self.init_params["synthetic_end_date"], "%Y-%m-%d"),
-        )
-
-        self.hr = create_fake_hr(
-            datetime.strptime(self.init_params["synthetic_start_date"], "%Y-%m-%d"),
-            datetime.strptime(self.init_params["synthetic_end_date"], "%Y-%m-%d"),
-        )
-
-        return
-
-        # and based on start and end dates
-        self.cycles = create_fake_cycles_df(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-        )
-
-        self.health_metrics = create_fake_metrics_df(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-        )
-
-        self.sleeps = create_fake_sleeps_df(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-        )
-
-        self.hr = create_fake_hr_df(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-            self.sleeps,
-        )
-
-    def _authenticate(self, auth_creds):
-        # authenticate this device against API
-
-        self.user = WhoopUser(auth_creds["email"], auth_creds["password"])
+from datetime import datetime
+
+import numpy as np
+import pandas as pd
+
+from ...devices.device import BaseDevice
+from ...utils import bin_search, seed_everything
+from .whoop_gen import *
+from .whoop_user import *
+
+class_name = "Whoop4"
+
+
+class Whoop4(BaseDevice):
+    """This device allows you to work with data from the `WHOOP 4.0 <https://shop.whoop.com/en-us/collections/whoop4-0/?order_by=featured>`_ device.
+    Available datatypes for this device are:
+
+    * `cycles`: a DataFrame of all cycles (days)
+
+    * `hr`: heart rate data
+
+    :param seed: random seed for synthetic data generation, defaults to 0
+    :type seed: int, optional
+    :param synthetic_start_date: start date for synthetic data generation, defaults to "2022-03-01"
+    :type synthetic_start_date: str, optional
+    :param synthetic_end_date: end date for synthetic data generation, defaults to "2022-06-17"
+    :type synthetic_end_date: str, optional
+    :param use_cache: decide whether to cache the credentials, defaults to True
+    :type use_cache: bool, optional
+    """
+
+    def __init__(
+        self, seed=0, synthetic_start_date="2022-03-01", synthetic_end_date="2022-06-17"
+    ):
+
+        params = {
+            "seed": seed,
+            "synthetic_start_date": synthetic_start_date,
+            "synthetic_end_date": synthetic_end_date,
+        }
+
+        self.data_types_methods_map = {
+            "cycles": "get_cycles_json",
+            "hr": "get_heart_rate_json",
+        }
+
+        self._initialize_device_params(
+            list(self.data_types_methods_map.keys()),
+            params,
+            {
+                "seed": 0,
+                "synthetic_start_date": "2022-03-01",
+                "synthetic_end_date": "2022-06-17",
+            },
+        )
+
+    def _default_params(self):
+        params = {
+            "start": "2022-04-24T00:00:00.000Z",
+            "end": "2022-04-28T00:00:00.000Z",
+        }
+
+        return params
+
+    def _get_real(self, data_type, params):
+        api_func = getattr(self.user, self.data_types_methods_map[data_type])
+        return api_func(params)
+
+    def _filter_synthetic(self, data, data_type, params):
+        # Here we just return the data we've already generated,
+        # but index into it based on the params. Specifically, we
+        # want to return the data between the start and end dates.
+
+        if data_type != "hr":
+            # synthetic data is generated day-by-day, so we can just
+            # index into it based on the start and end dates
+
+            date_str_to_obj = lambda x: datetime.strptime(x, "%Y-%m-%d")
+            datetime_str_to_obj = lambda x: datetime.strptime(
+                x, "%Y-%m-%dT%H:%M:%S.%fZ"
+            )
+
+            # get the indices by subtracting against the start of the synthetic data
+            synthetic_start = date_str_to_obj(self.init_params["synthetic_start_date"])
+
+            start_idx = (datetime_str_to_obj(params["start"]) - synthetic_start).days
+            end_idx = (datetime_str_to_obj(params["end"]) - synthetic_start).days
+
+            cycles = {
+                "total_count": end_idx - start_idx,
+                "offset": end_idx - start_idx,
+                "records": data["records"][start_idx:end_idx],
+            }
+
+            return cycles
+
+        else:
+            # hr data is generated in 7 second intervals, so we need to
+            # do a binary search to find the start and end indices
+            # and then return the data between those indices
+
+            start_ts = pd.Timestamp(params["start"]).timestamp()
+            end_ts = pd.Timestamp(params["end"]).timestamp()
+
+            vals = np.array([val["time"] for val in data["values"]])
+
+            start_idx = bin_search(vals, start_ts)
+            end_idx = bin_search(vals, end_ts)
+
+            return {
+                "name": "heart_rate",
+                "start": data["values"][start_idx]["time"],
+                "values": data["values"][start_idx:end_idx],
+            }
+
+    def _gen_synthetic(self):
+        # generate random data according to seed
+        seed_everything(self.init_params["seed"])
+
+        self.cycles = create_fake_cycles(
+            datetime.strptime(self.init_params["synthetic_start_date"], "%Y-%m-%d"),
+            datetime.strptime(self.init_params["synthetic_end_date"], "%Y-%m-%d"),
+        )
+
+        self.hr = create_fake_hr(
+            datetime.strptime(self.init_params["synthetic_start_date"], "%Y-%m-%d"),
+            datetime.strptime(self.init_params["synthetic_end_date"], "%Y-%m-%d"),
+        )
+
+        return
+
+        # and based on start and end dates
+        self.cycles = create_fake_cycles_df(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+        )
+
+        self.health_metrics = create_fake_metrics_df(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+        )
+
+        self.sleeps = create_fake_sleeps_df(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+        )
+
+        self.hr = create_fake_hr_df(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+            self.sleeps,
+        )
+
+    def _authenticate(self, auth_creds):
+        # authenticate this device against API
+
+        self.user = WhoopUser(auth_creds["email"], auth_creds["password"])
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/whoop/whoop_gen.py` & `wearipedia-0.1.3/wearipedia/devices/whoop/whoop_gen.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# utils for generating synthetic data
-
-from datetime import datetime, timedelta
-
-import numpy as np
-
-__all__ = [
-    "create_fake_cycles",
-    "create_fake_hr",
-]
-
-
-def create_fake_cycles(start_date, end_date):
-    num_cycles = (end_date - start_date).days
-
-    records = []
-
-    for i in range(num_cycles):
-        day = end_date - timedelta(days=i + 1)
-
-        cycle = {
-            "id": np.random.randint(0, 1000000000),
-            "created_at": "2022-04-27T16:28:30.523+0000",
-            "updated_at": "2022-08-19T17:10:29.456+0000",
-            "scaled_strain": np.clip(0, 30, np.random.normal() * 5 + 10),
-            "during": "['2022-04-27T11:42:16.060Z','2022-04-28T12:41:13.254Z')",
-            "user_id": 4005531,
-            "sleep_need": None,
-            "predicted_end": "2022-04-28T12:41:13.254+0000",
-            "timezone_offset": "-0700",
-            "days": f"['{datetime.strftime(day, '%Y-%m-%d')}','{datetime.strftime(day + timedelta(days=1), '%Y-%m-%d')}')",
-            "intensity_score": None,
-            "data_state": "complete",
-            "day_strain": np.clip(0, 0.01, np.random.normal() * 0.005 + 0.005),
-            "day_kilojoules": np.random.normal() * 2500 + 5000,
-            "day_avg_heart_rate": np.random.normal() * 10 + 75,
-            "day_max_heart_rate": np.random.normal() * 20 + 150,
-        }
-
-        # overly simplistic model for now
-        # TODO: change this so that it matches the
-        # notebook
-        num_sleeps = np.random.poisson(1)
-
-        sleeps = []
-
-        for _ in range(num_sleeps):
-            sleep = {
-                "cycle_id": np.random.randint(0, 1000000000),
-                "created_at": "2022-04-27T01:47:48.706+0000",
-                "updated_at": "2022-04-27T03:25:23.600+0000",
-                "activity_id": np.random.randint(0, 1000000000),
-                "score": int(np.random.uniform(0, 100)),
-                "quality_duration": int(
-                    np.clip(0, 50_000_000, np.random.normal() * 5_000_000 + 25_000_000)
-                ),
-                "latency": 0,
-                "max_heart_rate": None,
-                "average_heart_rate": None,
-                "debt_pre": np.random.normal() * 100_000 + 3_000_000.0,
-                "debt_post": np.random.normal() * 100_000 + 3_000_000.0,
-                "need_from_strain": np.random.normal() * 100_000 + 3_000_000.0,
-                "sleep_need": np.random.normal() * 100_000 + 3_000_000.0,
-                "habitual_sleep_need": np.random.normal() * 100_000 + 3_000_000.0,
-                "disturbances": 1,
-                "time_in_bed": np.random.normal() * 100_000 + 3_000_000.0,
-                "light_sleep_duration": np.random.normal() * 100_000 + 3_000_000,
-                "slow_wave_sleep_duration": int(
-                    np.random.normal() * 100_000 + 3_000_000
-                ),
-                "rem_sleep_duration": int(np.random.normal() * 100_000 + 3_000_000),
-                "cycles_count": 1,
-                "wake_duration": np.clip(
-                    0, 1_000_000, int(np.random.normal() * 100_000 + 100_000)
-                ),
-                "arousal_time": np.random.normal() * 50_000 + 100_000,
-                "no_data_duration": 0,
-                "in_sleep_efficiency": np.random.uniform(0, 1),
-                "credit_from_naps": 0.0,
-                "hr_baseline": None,
-                "respiratory_rate": np.random.normal() * 10 + 15.0,
-                "sleep_consistency": None,
-                "algo_version": "5.0.0",
-                "projected_score": np.random.uniform(0, 100),
-                "projected_sleep": 4281596.0,
-                "optimal_sleep_times": None,
-                "kilojoules": None,
-                "user_id": np.random.randint(0, 1000000000),
-                "during": "['2022-04-27T00:03:38.208Z','2022-04-27T01:20:41.151Z')",
-                "timezone_offset": "-0700",
-                "survey_response_id": None,
-                "percent_recorded": 1.0,
-                "auto_detected": True,
-                "state": "complete",
-                "responded": False,
-                "team_act_id": None,
-                "source": "auto+user",
-                "is_significant": False,
-                "is_normal": True,
-                "is_nap": True,
-            }
-
-            sleeps.append(sleep)
-
-        recovery = {
-            "during": "['2022-04-27T11:42:16.060Z','2022-04-27T18:17:23.904Z')",
-            "id": np.random.randint(0, 1000000000),
-            "created_at": "2022-04-27T16:28:30.523+0000",
-            "updated_at": "2022-04-27T18:49:22.756+0000",
-            "date": "2022-04-27T18:17:23.904+0000",
-            "user_id": np.random.randint(0, 1000000000),
-            "sleep_id": np.random.randint(0, 1000000000),
-            "survey_response_id": None,
-            "cycle_id": np.random.randint(0, 1000000000),
-            "responded": False,
-            "recovery_score": int(np.random.uniform(0, 100)),
-            "resting_heart_rate": int(np.random.uniform(45, 65)),
-            "hrv_rmssd": 0.071095094,
-            "state": "complete",
-            "calibrating": True,
-            "prob_covid": None,
-            "hr_baseline": 57.0,
-            "skin_temp_celsius": np.round(np.random.uniform(25, 40), 1),
-            "spo2": np.round(np.random.uniform(70, 100), 1),
-            "algo_version": "5.0.0",
-            "rhr_component": None,
-            "hrv_component": None,
-            "history_size": 2.0,
-            "from_sws": False,
-            "recovery_rate": np.clip(0, 10, np.random.normal() * 2 + 3.5),
-            "is_normal": None,
-        }
-
-        record = {
-            "cycle": cycle,
-            "sleeps": sleeps,
-            "recovery": recovery,
-            "workouts": [],
-            "v2_activities": [],
-        }
-
-        records.append(record)
-
-    return {"total_count": num_cycles, "offset": num_cycles, "records": records}
-
-
-def create_fake_hr(start_date, end_date):
-    # samples every minute now, for some reason
-
-    values = []
-
-    cur_timestamp = start_date
-
-    while True:
-        if cur_timestamp > end_date:
-            break
-
-        values.append(
-            {"data": np.random.normal() * 20 + 80, "time": cur_timestamp.timestamp()}
-        )
-        cur_timestamp += timedelta(seconds=60.563)
-
-    return {"name": "heart_rate", "start": start_date.timestamp(), "values": values}
+# utils for generating synthetic data
+
+from datetime import datetime, timedelta
+
+import numpy as np
+
+__all__ = [
+    "create_fake_cycles",
+    "create_fake_hr",
+]
+
+
+def create_fake_cycles(start_date, end_date):
+    num_cycles = (end_date - start_date).days
+
+    records = []
+
+    for i in range(num_cycles):
+        day = end_date - timedelta(days=i + 1)
+
+        cycle = {
+            "id": np.random.randint(0, 1000000000),
+            "created_at": "2022-04-27T16:28:30.523+0000",
+            "updated_at": "2022-08-19T17:10:29.456+0000",
+            "scaled_strain": np.clip(0, 30, np.random.normal() * 5 + 10),
+            "during": "['2022-04-27T11:42:16.060Z','2022-04-28T12:41:13.254Z')",
+            "user_id": 4005531,
+            "sleep_need": None,
+            "predicted_end": "2022-04-28T12:41:13.254+0000",
+            "timezone_offset": "-0700",
+            "days": f"['{datetime.strftime(day, '%Y-%m-%d')}','{datetime.strftime(day + timedelta(days=1), '%Y-%m-%d')}')",
+            "intensity_score": None,
+            "data_state": "complete",
+            "day_strain": np.clip(0, 0.01, np.random.normal() * 0.005 + 0.005),
+            "day_kilojoules": np.random.normal() * 2500 + 5000,
+            "day_avg_heart_rate": np.random.normal() * 10 + 75,
+            "day_max_heart_rate": np.random.normal() * 20 + 150,
+        }
+
+        # overly simplistic model for now
+        # TODO: change this so that it matches the
+        # notebook
+        num_sleeps = np.random.poisson(1)
+
+        sleeps = []
+
+        for _ in range(num_sleeps):
+            sleep = {
+                "cycle_id": np.random.randint(0, 1000000000),
+                "created_at": "2022-04-27T01:47:48.706+0000",
+                "updated_at": "2022-04-27T03:25:23.600+0000",
+                "activity_id": np.random.randint(0, 1000000000),
+                "score": int(np.random.uniform(0, 100)),
+                "quality_duration": int(
+                    np.clip(0, 50_000_000, np.random.normal() * 5_000_000 + 25_000_000)
+                ),
+                "latency": 0,
+                "max_heart_rate": None,
+                "average_heart_rate": None,
+                "debt_pre": np.random.normal() * 100_000 + 3_000_000.0,
+                "debt_post": np.random.normal() * 100_000 + 3_000_000.0,
+                "need_from_strain": np.random.normal() * 100_000 + 3_000_000.0,
+                "sleep_need": np.random.normal() * 100_000 + 3_000_000.0,
+                "habitual_sleep_need": np.random.normal() * 100_000 + 3_000_000.0,
+                "disturbances": 1,
+                "time_in_bed": np.random.normal() * 100_000 + 3_000_000.0,
+                "light_sleep_duration": np.random.normal() * 100_000 + 3_000_000,
+                "slow_wave_sleep_duration": int(
+                    np.random.normal() * 100_000 + 3_000_000
+                ),
+                "rem_sleep_duration": int(np.random.normal() * 100_000 + 3_000_000),
+                "cycles_count": 1,
+                "wake_duration": np.clip(
+                    0, 1_000_000, int(np.random.normal() * 100_000 + 100_000)
+                ),
+                "arousal_time": np.random.normal() * 50_000 + 100_000,
+                "no_data_duration": 0,
+                "in_sleep_efficiency": np.random.uniform(0, 1),
+                "credit_from_naps": 0.0,
+                "hr_baseline": None,
+                "respiratory_rate": np.random.normal() * 10 + 15.0,
+                "sleep_consistency": None,
+                "algo_version": "5.0.0",
+                "projected_score": np.random.uniform(0, 100),
+                "projected_sleep": 4281596.0,
+                "optimal_sleep_times": None,
+                "kilojoules": None,
+                "user_id": np.random.randint(0, 1000000000),
+                "during": "['2022-04-27T00:03:38.208Z','2022-04-27T01:20:41.151Z')",
+                "timezone_offset": "-0700",
+                "survey_response_id": None,
+                "percent_recorded": 1.0,
+                "auto_detected": True,
+                "state": "complete",
+                "responded": False,
+                "team_act_id": None,
+                "source": "auto+user",
+                "is_significant": False,
+                "is_normal": True,
+                "is_nap": True,
+            }
+
+            sleeps.append(sleep)
+
+        recovery = {
+            "during": "['2022-04-27T11:42:16.060Z','2022-04-27T18:17:23.904Z')",
+            "id": np.random.randint(0, 1000000000),
+            "created_at": "2022-04-27T16:28:30.523+0000",
+            "updated_at": "2022-04-27T18:49:22.756+0000",
+            "date": "2022-04-27T18:17:23.904+0000",
+            "user_id": np.random.randint(0, 1000000000),
+            "sleep_id": np.random.randint(0, 1000000000),
+            "survey_response_id": None,
+            "cycle_id": np.random.randint(0, 1000000000),
+            "responded": False,
+            "recovery_score": int(np.random.uniform(0, 100)),
+            "resting_heart_rate": int(np.random.uniform(45, 65)),
+            "hrv_rmssd": 0.071095094,
+            "state": "complete",
+            "calibrating": True,
+            "prob_covid": None,
+            "hr_baseline": 57.0,
+            "skin_temp_celsius": np.round(np.random.uniform(25, 40), 1),
+            "spo2": np.round(np.random.uniform(70, 100), 1),
+            "algo_version": "5.0.0",
+            "rhr_component": None,
+            "hrv_component": None,
+            "history_size": 2.0,
+            "from_sws": False,
+            "recovery_rate": np.clip(0, 10, np.random.normal() * 2 + 3.5),
+            "is_normal": None,
+        }
+
+        record = {
+            "cycle": cycle,
+            "sleeps": sleeps,
+            "recovery": recovery,
+            "workouts": [],
+            "v2_activities": [],
+        }
+
+        records.append(record)
+
+    return {"total_count": num_cycles, "offset": num_cycles, "records": records}
+
+
+def create_fake_hr(start_date, end_date):
+    # samples every minute now, for some reason
+
+    values = []
+
+    cur_timestamp = start_date
+
+    while True:
+        if cur_timestamp > end_date:
+            break
+
+        values.append(
+            {"data": np.random.normal() * 20 + 80, "time": cur_timestamp.timestamp()}
+        )
+        cur_timestamp += timedelta(seconds=60.563)
+
+    return {"name": "heart_rate", "start": start_date.timestamp(), "values": values}
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/withings/bodyplus.py` & `wearipedia-0.1.3/wearipedia/devices/withings/sleepmat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,68 @@
-import os
-from pathlib import Path
-
-import wget
-
-from ...devices.device import BaseDevice
-from ...utils import bin_search, seed_everything
-from .withings_authenticate import *
-from .withings_extract import *
-from .withings_gen import *
-
-class_name = "BodyPlus"
-
-
-class BodyPlus(BaseDevice):
-    """This device allows you to work with data from the `Withings Body+ <https://www.withings.com/us/en/body-plus>`_ device.
-    Available datatypes for this device are:
-
-    * `measurements`: contains all measurements made with the scale
-
-    :param seed: random seed for synthetic data generation, defaults to 0
-    :type seed: int, optional
-    :param synthetic_start_date: start date for synthetic data generation, defaults to "2021-06-01"
-    :type start_date: str, optional
-    """
-
-    def __init__(self, seed=0, synthetic_start_date="2021-06-01"):
-
-        params = {"seed": seed, "synthetic_start_date": synthetic_start_date}
-
-        self._initialize_device_params(
-            ["measurements"],
-            params,
-            {
-                "seed": 0,
-                "synthetic_start_date": "2021-06-01",
-            },
-        )
-
-    def _default_params(self):
-        return {
-            "start": self.init_params["synthetic_start_date"],
-            "end": datetime.strftime(
-                datetime.strptime(self.init_params["synthetic_start_date"], "%Y-%m-%d")
-                + timedelta(days=900),
-                "%Y-%m-%d",
-            ),
-        }
-
-    def _get_real(self, data_type, params):
-        start = datetime.strptime(params["start"], "%Y-%m-%d")
-        end = datetime.strptime(params["end"], "%Y-%m-%d")
-
-        return fetch_measurements(self.access_token, start, end)
-
-    def _filter_synthetic(self, data, data_type, params):
-        start_ts = pd.Timestamp(params["start"])
-        end_ts = pd.Timestamp(params["end"])
-
-        start_idx = bin_search(np.array(data.date), start_ts)
-        end_idx = bin_search(np.array(data.date), end_ts)
-
-        return data.iloc[start_idx:end_idx]
-
-    def _gen_synthetic(self):
-        # generate random data according to seed
-        seed_everything(self.init_params["seed"])
-
-        self.measurements = create_syn_bodyplus(
-            self.init_params["synthetic_start_date"]
-        )
-
-    def _authenticate(self, auth_creds):
-        if "access_token" in auth_creds:
-            self.access_token = auth_creds["access_token"]
-            return
-
-        if "refresh_token" in auth_creds:
-            self.refresh_token, self.access_token = refresh_access_token(
-                auth_creds["refresh_token"],
-                auth_creds["client_id"],
-                auth_creds["client_secret"],
-            )
-        else:
-            self.refresh_token, self.access_token = withings_authenticate(
-                auth_creds["client_id"], auth_creds["client_secret"]
-            )
+#### sleep gives us bad data, so need to figure this one out
+
+
+import os
+from pathlib import Path
+
+import wget
+
+from ...devices.device import BaseDevice
+from ...utils import seed_everything
+from .withings_authenticate import *
+from .withings_extract import *
+
+class_name = "SleepMat"
+
+
+class SleepMat(BaseDevice):
+    def __init__(self, seed=0):
+
+        params = {
+            "seed": seed,
+        }
+
+        self._initialize_device_params(
+            ["measurements"],
+            params,
+            {"seed": 0},
+        )
+
+    def _default_params(self):
+        return dict()
+
+    def _get_real(self, data_type, params):
+        return fetch_measurements(self.access_token)
+
+    def _filter_synthetic(self, data, data_type, params):
+        return self.measurements
+
+    def _gen_synthetic(self):
+        # generate random data according to seed
+        seed_everything(self.init_params["seed"])
+
+        self.measurements = [0, 1, 2, 3, 4, 5]
+
+        # load in the CSV that we've pre-generated
+        # wget.download(CSV_URL, out=CSV_LOCAL_PATH)
+
+        # self.measurements = pd.read_csv(CSV_LOCAL_PATH)
+        # fix dates, convert to datetime obj from string
+        # self.measurements["date"] = self.measurements.date.apply(
+        #    lambda x: datetime.strptime(x, "%Y-%m-%d %H:%M:%S.%f")
+        # )
+
+        # self.measurements = self.measurements[
+        #    [col for col in self.measurements.columns if "Unnamed: 0" not in col]
+        # ]
+
+    def _authenticate(self, auth_creds):
+        if "refresh_token" in auth_creds:
+            self.refresh_token, self.access_token = refresh_access_token(
+                auth_creds["refresh_token"],
+                auth_creds["client_id"],
+                auth_creds["customer_secret"],
+            )
+        else:
+            self.refresh_token, self.access_token = withings_authenticate(
+                auth_creds["client_id"], auth_creds["customer_secret"]
+            )
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/withings/scanwatch.py` & `wearipedia-0.1.3/wearipedia/devices/withings/scanwatch.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import time
-
-from ...devices.device import BaseDevice
-from ...utils import bin_search, seed_everything
-from .withings_authenticate import *
-from .withings_extract import *
-from .withings_gen import *
-
-class_name = "ScanWatch"
-
-
-class ScanWatch(BaseDevice):
-    """This device allows you to work with data from the `Withings ScanWatch <https://www.withings.com/us/en/scanwatch>`_ device.
-    Available datatypes for this device are:
-
-    * `heart_rates`: heart rate data
-
-    * `sleeps`: sleep data
-
-    :param seed: random seed for synthetic data generation, defaults to 0
-    :type seed: int, optional
-    :param synthetic_start_date: start date for synthetic data generation, defaults to "2022-03-01"
-    :type start_date: str, optional
-    :param synthetic_end_date: end date for synthetic data generation, defaults to "2022-06-17"
-    :type end_date: str, optional
-    """
-
-    def __init__(
-        self, seed=0, synthetic_start_date="2022-03-01", synthetic_end_date="2022-06-17"
-    ):
-
-        params = {
-            "seed": seed,
-            "synthetic_start_date": synthetic_start_date,
-            "synthetic_end_date": synthetic_end_date,
-        }
-
-        self._initialize_device_params(
-            ["heart_rates", "sleeps"],
-            params,
-            {
-                "seed": 0,
-                "synthetic_start_date": "2022-03-01",
-                "synthetic_end_date": "2022-06-17",
-            },
-        )
-
-    def _default_params(self):
-        return {
-            "start": self.init_params["synthetic_start_date"],
-            "end": self.init_params["synthetic_end_date"],
-        }
-
-    def _get_real(self, data_type, params):
-        if data_type == "heart_rates":
-            return fetch_all_heart_rate(
-                self.access_token, params["start"], params["end"]
-            )
-        elif data_type == "sleeps":
-            return fetch_all_sleeps(self.access_token, params["start"], params["end"])
-
-    def _filter_synthetic(self, data, data_type, params):
-
-        if data_type == "sleeps":
-            key = "date"
-            target_start = params["start"]
-            target_end = params["end"]
-        elif data_type == "heart_rates":
-            key = "datetime"
-            target_start = pd.Timestamp(params["start"])
-            target_end = pd.Timestamp(params["end"])
-
-        start_idx = bin_search(np.array(data[key]), target_start)
-        end_idx = bin_search(np.array(data[key]), target_end)
-
-        return data.iloc[start_idx:end_idx]
-
-    def _gen_synthetic(self):
-        # generate random data according to seed
-        seed_everything(self.init_params["seed"])
-
-        self.sleeps = create_synthetic_sleeps_df(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-        )
-
-        self.heart_rates = create_syn_hr(
-            self.init_params["synthetic_start_date"],
-            self.init_params["synthetic_end_date"],
-            self.sleeps,
-        )
-
-    def _authenticate(self, auth_creds):
-        if "access_token" in auth_creds:
-            self.access_token = auth_creds["access_token"]
-            return
-
-        if "refresh_token" in auth_creds:
-            self.refresh_token, self.access_token = refresh_access_token(
-                auth_creds["refresh_token"],
-                auth_creds["client_id"],
-                auth_creds["client_secret"],
-            )
-        else:
-            self.refresh_token, self.access_token = withings_authenticate(
-                auth_creds["client_id"], auth_creds["client_secret"]
-            )
+import time
+
+from ...devices.device import BaseDevice
+from ...utils import bin_search, seed_everything
+from .withings_authenticate import *
+from .withings_extract import *
+from .withings_gen import *
+
+class_name = "ScanWatch"
+
+
+class ScanWatch(BaseDevice):
+    """This device allows you to work with data from the `Withings ScanWatch <https://www.withings.com/us/en/scanwatch>`_ device.
+    Available datatypes for this device are:
+
+    * `heart_rates`: heart rate data
+
+    * `sleeps`: sleep data
+
+    :param seed: random seed for synthetic data generation, defaults to 0
+    :type seed: int, optional
+    :param synthetic_start_date: start date for synthetic data generation, defaults to "2022-03-01"
+    :type start_date: str, optional
+    :param synthetic_end_date: end date for synthetic data generation, defaults to "2022-06-17"
+    :type end_date: str, optional
+    """
+
+    def __init__(
+        self, seed=0, synthetic_start_date="2022-03-01", synthetic_end_date="2022-06-17"
+    ):
+
+        params = {
+            "seed": seed,
+            "synthetic_start_date": synthetic_start_date,
+            "synthetic_end_date": synthetic_end_date,
+        }
+
+        self._initialize_device_params(
+            ["heart_rates", "sleeps"],
+            params,
+            {
+                "seed": 0,
+                "synthetic_start_date": "2022-03-01",
+                "synthetic_end_date": "2022-06-17",
+            },
+        )
+
+    def _default_params(self):
+        return {
+            "start": self.init_params["synthetic_start_date"],
+            "end": self.init_params["synthetic_end_date"],
+        }
+
+    def _get_real(self, data_type, params):
+        if data_type == "heart_rates":
+            return fetch_all_heart_rate(
+                self.access_token, params["start"], params["end"]
+            )
+        elif data_type == "sleeps":
+            return fetch_all_sleeps(self.access_token, params["start"], params["end"])
+
+    def _filter_synthetic(self, data, data_type, params):
+
+        if data_type == "sleeps":
+            key = "date"
+            target_start = params["start"]
+            target_end = params["end"]
+        elif data_type == "heart_rates":
+            key = "datetime"
+            target_start = pd.Timestamp(params["start"])
+            target_end = pd.Timestamp(params["end"])
+
+        start_idx = bin_search(np.array(data[key]), target_start)
+        end_idx = bin_search(np.array(data[key]), target_end)
+
+        return data.iloc[start_idx:end_idx]
+
+    def _gen_synthetic(self):
+        # generate random data according to seed
+        seed_everything(self.init_params["seed"])
+
+        self.sleeps = create_synthetic_sleeps_df(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+        )
+
+        self.heart_rates = create_syn_hr(
+            self.init_params["synthetic_start_date"],
+            self.init_params["synthetic_end_date"],
+            self.sleeps,
+        )
+
+    def _authenticate(self, auth_creds):
+        if "access_token" in auth_creds:
+            self.access_token = auth_creds["access_token"]
+            return
+
+        if "refresh_token" in auth_creds:
+            self.refresh_token, self.access_token = refresh_access_token(
+                auth_creds["refresh_token"],
+                auth_creds["client_id"],
+                auth_creds["client_secret"],
+            )
+        else:
+            self.refresh_token, self.access_token = withings_authenticate(
+                auth_creds["client_id"], auth_creds["client_secret"]
+            )
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/withings/withings_authenticate.py` & `wearipedia-0.1.3/wearipedia/devices/withings/withings_authenticate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,94 @@
-import json
-import time
-import urllib
-
-import requests
-
-__all__ = ["refresh_access_token", "withings_authenticate"]
-
-STATE = "string"
-ACCOUNT_URL = "https://account.withings.com"
-CALLBACK_URI = "https://wbsapi.withings.net/v2/oauth2"
-
-
-def refresh_access_token(refresh_token, client_id, client_secret):
-    # gives us access token given the refresh token
-
-    params = {
-        "action": "requesttoken",
-        "grant_type": "refresh_token",
-        "client_id": client_id,
-        "client_secret": client_secret,
-        "refresh_token": refresh_token,
-    }
-
-    out = requests.post("https://wbsapi.withings.net/v2/oauth2", data=params)
-
-    try:
-        body = json.loads(out.text)["body"]
-        new_refresh_token, access_token = body["refresh_token"], body["access_token"]
-        print(f"Got new refresh token: {new_refresh_token}")
-    except KeyError as e:
-        exception_str = f"Got exception: {e}\n"
-        exception_str += f"The full returned payload is: {json.loads(out.text)}"
-        raise Exception(exception_str)
-
-    return new_refresh_token, access_token
-
-
-def withings_authenticate(client_id, client_secret):
-    # gives us access token given the auth_creds + going through the process, it's interactive
-
-    payload = {
-        "response_type": "code",  # imposed string by the api
-        "client_id": client_id,
-        "state": STATE,
-        "scope": "user.info,user.metrics,user.activity",  # see docs for enhanced scope
-        "redirect_uri": CALLBACK_URI,  # URL of this app
-        #'mode': 'demo'  # Use demo mode, DELETE THIS FOR REAL APP
-    }
-
-    url = f"{ACCOUNT_URL}/oauth2_user/authorize2?"
-
-    for key, value in payload.items():
-        url += f"{key}={value}&"
-
-    url = url[:-1]
-
-    print(url)
-    print("redirect url below:")
-    time.sleep(0.1)
-    redirect_url = input(">")
-
-    try:
-        code = urllib.parse.parse_qs(urllib.parse.urlparse(redirect_url).query)["code"][
-            0
-        ]
-    except Exception as e:
-        exception_str = f"Caught error:\n{e}\n"
-        exception_str += "Please copy and paste the entire URL (including https)"
-        raise Exception(exception_str)
-
-    params = {
-        "action": "requesttoken",
-        "grant_type": "authorization_code",
-        "client_id": client_id,
-        "client_secret": client_secret,
-        "code": code,
-        #'scope': 'user.info',
-        "redirect_uri": "https://wbsapi.withings.net/v2/oauth2",
-    }
-
-    out = requests.get("https://wbsapi.withings.net/v2/oauth2", data=params)
-
-    out = json.loads(out.text)
-
-    try:
-        refresh_token, access_token = out["body"]["refresh_token"], out["body"]["access_token"]
-    except KeyError as e:
-        raise Exception("Took too long to paste in redirect URL. Please repeat step 7.")
-
-    return refresh_token, access_token
+import json
+import time
+import urllib
+
+import requests
+
+__all__ = ["refresh_access_token", "withings_authenticate"]
+
+STATE = "string"
+ACCOUNT_URL = "https://account.withings.com"
+CALLBACK_URI = "https://wbsapi.withings.net/v2/oauth2"
+
+
+def refresh_access_token(refresh_token, client_id, client_secret):
+    # gives us access token given the refresh token
+
+    params = {
+        "action": "requesttoken",
+        "grant_type": "refresh_token",
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "refresh_token": refresh_token,
+    }
+
+    out = requests.post("https://wbsapi.withings.net/v2/oauth2", data=params)
+
+    try:
+        body = json.loads(out.text)["body"]
+        new_refresh_token, access_token = body["refresh_token"], body["access_token"]
+        print(f"Got new refresh token: {new_refresh_token}")
+    except KeyError as e:
+        exception_str = f"Got exception: {e}\n"
+        exception_str += f"The full returned payload is: {json.loads(out.text)}"
+        raise Exception(exception_str)
+
+    return new_refresh_token, access_token
+
+
+def withings_authenticate(client_id, client_secret):
+    # gives us access token given the auth_creds + going through the process, it's interactive
+
+    payload = {
+        "response_type": "code",  # imposed string by the api
+        "client_id": client_id,
+        "state": STATE,
+        "scope": "user.info,user.metrics,user.activity",  # see docs for enhanced scope
+        "redirect_uri": CALLBACK_URI,  # URL of this app
+        #'mode': 'demo'  # Use demo mode, DELETE THIS FOR REAL APP
+    }
+
+    url = f"{ACCOUNT_URL}/oauth2_user/authorize2?"
+
+    for key, value in payload.items():
+        url += f"{key}={value}&"
+
+    url = url[:-1]
+
+    print(url)
+    print("redirect url below:")
+    time.sleep(0.1)
+    redirect_url = input(">")
+
+    try:
+        code = urllib.parse.parse_qs(urllib.parse.urlparse(redirect_url).query)["code"][
+            0
+        ]
+    except Exception as e:
+        exception_str = f"Caught error:\n{e}\n"
+        exception_str += "Please copy and paste the entire URL (including https)"
+        raise Exception(exception_str)
+
+    params = {
+        "action": "requesttoken",
+        "grant_type": "authorization_code",
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "code": code,
+        #'scope': 'user.info',
+        "redirect_uri": "https://wbsapi.withings.net/v2/oauth2",
+    }
+
+    out = requests.get("https://wbsapi.withings.net/v2/oauth2", data=params)
+
+    out = json.loads(out.text)
+
+    try:
+        refresh_token, access_token = (
+            out["body"]["refresh_token"],
+            out["body"]["access_token"],
+        )
+    except KeyError as e:
+        raise Exception("Took too long to paste in redirect URL. Please repeat step 7.")
+
+    return refresh_token, access_token
```

### Comparing `wearipedia-0.1.2/wearipedia/devices/withings/withings_gen.py` & `wearipedia-0.1.3/wearipedia/devices/withings/withings_gen.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-import hashlib
-from datetime import datetime, timedelta
-
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-
-__all__ = ["create_synthetic_sleeps_df", "create_syn_hr", "create_syn_bodyplus"]
-
-#############
-# ScanWatch #
-#############
-
-
-def create_synthetic_sleeps_df(start_date, end_date):
-    """Create a synthetic dataframe of sleep data. This is for
-    the ScanWatch.
-
-    :param start_date: the start date of the synthetic data as a string formatted as YYYY-MM-DD
-    :type start_date: str
-    :param end_date: the end date of the synthetic data as a string formatted as YYYY-MM-DD
-    :type end_date: str
-    :return: the synthetic dataframe containing sleep data
-    :rtype: pd.DataFrame
-    """
-
-    start_day = datetime.strptime(start_date, "%Y-%m-%d")
-    end_day = datetime.strptime(end_date, "%Y-%m-%d")
-    num_days = (end_day - start_day).days
-
-    syn_sleeps = pd.DataFrame()
-
-    syn_sleeps["id"] = np.random.randint(0, 100000000, size=(num_days,))
-    syn_sleeps["timezone"] = "America/Los_Angeles"
-    syn_sleeps["model"] = 16
-    syn_sleeps["model_id"] = 93
-    syn_sleeps[
-        "hash_deviceid"
-    ] = "d41d8cd98f00b204e9800998ecf8427e"  # randomly generated
-    syn_sleeps["date"] = [
-        datetime.fromtimestamp(
-            datetime.strptime(start_date, "%Y-%m-%d").timestamp() + i * 24 * 3600
-        ).strftime("%Y-%m-%d")
-        for i in range(num_days)
-    ]
-
-    startdates = []
-    enddates = []
-
-    for date in syn_sleeps["date"]:
-        sleep_start = np.random.randint(20, 27)
-        sleep_time = np.random.randint(4, 9)
-
-        startdate = datetime.strptime(date, "%Y-%m-%d") + timedelta(
-            hours=sleep_start + 7
-        )
-
-        enddate = startdate + timedelta(hours=sleep_time)
-
-        startdate, enddate = int(startdate.timestamp()), int(enddate.timestamp())
-
-        startdates.append(startdate)
-        enddates.append(enddate)
-
-    all_data = []
-
-    for _ in range(num_days):
-
-        data = {
-            "wakeupduration": np.random.randint(0, 3000),
-            "wakeupcount": np.random.poisson(1),
-            "durationtosleep": np.random.randint(120, 180),
-            "durationtowakeup": np.random.randint(0, 700),
-            "total_timeinbed": np.random.randint(10000, 50000),
-            "total_sleep_time": np.random.randint(10000, 50000),
-            "sleep_efficiency": np.random.rand() * 0.1 + 0.9,
-            "sleep_latency": np.random.randint(120, 130),
-            "wakeup_latency": np.random.randint(0, 800),
-            "waso": np.random.randint(0, 4000),
-            "nb_rem_episodes": 0,
-            "out_of_bed_count": 0,
-            "lightsleepduration": np.random.randint(6000, 35000),
-            "deepsleepduration": np.random.randint(3000, 17000),
-            "hr_average": np.random.randint(55, 65),
-            "hr_min": np.random.randint(40, 60),
-            "hr_max": np.random.randint(70, 120),
-            "sleep_score": np.random.randint(30, 80),
-        }
-
-        all_data.append(data)
-
-    syn_sleeps["startdate"] = startdates
-    syn_sleeps["enddate"] = enddates
-
-    syn_sleeps["data"] = all_data
-
-    syn_sleeps["created"] = enddates
-    syn_sleeps["modified"] = enddates
-
-    return syn_sleeps
-
-
-def create_syn_hr(start_date, end_date, syn_sleeps):
-    """Create a synthetic dataframe of heart rate data. This is for
-    the ScanWatch.
-
-    :param syn_sleeps: the synthetic sleep dataframe
-    :type syn_sleeps: pd.DataFrame
-    :return: the synthetic dataframe containing heart rate data
-    :rtype: pd.DataFrame
-    """
-    start_day = datetime.strptime(start_date, "%Y-%m-%d")
-    end_day = datetime.strptime(end_date, "%Y-%m-%d")
-
-    num_days = (end_day - start_day).days
-
-    hour_usage = [0.8] * 3 + [0.9] * 7 + [1.0] * 10 + [0.9] * 4
-
-    datetimes = []
-
-    for day_offset in tqdm(range(num_days)):
-        for hour_offset in range(24):
-            for minute_offset in range(0, 60, 10):
-                day = start_day + timedelta(days=day_offset)
-                hour = day + timedelta(hours=hour_offset)
-                minute = hour + timedelta(minutes=minute_offset)
-
-                if np.random.uniform(0, 1) < hour_usage[hour_offset]:
-                    datetimes.append(minute)
-
-    hr_measurements = (np.random.randn(len(datetimes)) * 5 + 90).astype("int")
-
-    timestamps = np.array([dt.timestamp() for dt in datetimes])
-
-    for i, (startdate, enddate) in tqdm(
-        enumerate(zip(syn_sleeps.startdate, syn_sleeps.enddate))
-    ):
-        idxes = np.where(np.logical_and(timestamps > startdate, timestamps < enddate))[
-            0
-        ]
-        duration = (enddate - startdate) / 3600
-        avg_hr = -5 / 7 * duration + 64.1428571429
-
-        hr_measurements[idxes] = (np.random.randn(idxes.shape[0]) + avg_hr).astype(
-            "int"
-        )
-
-    syn_hr = pd.DataFrame()
-    syn_hr["datetime"] = datetimes
-    syn_hr["heart_rate"] = hr_measurements
-
-    syn_hr["model"] = "ScanWatch"
-    syn_hr["model_id"] = 93
-    syn_hr["deviceid"] = hashlib.md5().hexdigest()
-
-    num_garbage = 1000
-
-    timestamps_garbage = np.random.uniform(
-        (start_day - timedelta(days=100)).timestamp(),
-        start_day.timestamp(),
-        size=num_garbage,
-    )
-
-    garbage_df = pd.DataFrame()
-    garbage_df["datetime"] = [
-        datetime.fromtimestamp(int(ts)) for ts in timestamps_garbage
-    ]
-    garbage_df["heart_rate"] = (np.random.randn(num_garbage) * 5 + 90).astype("int")
-
-    garbage_df["model"] = None
-    garbage_df["model_id"] = 1059
-    garbage_df["deviceid"] = None
-
-    syn_hr = pd.concat((garbage_df, syn_hr), ignore_index=True)
-
-    return syn_hr
-
-
-#########
-# Body+ #
-#########
-
-
-def create_syn_bodyplus(start_date):
-    """Create a synthetic dataframe of body+ data. This is for
-    the Body+ scale. The reason why we don't have an end date is
-    because we wish to generate 2.5 years' worth of data to portray
-    a fictional scenario where the user has been using the scale
-    for a year and we see the impact of a fictional medication.
-
-    :param start_date: the start date as a string formatted as YYYY-MM-DD
-    :type start_date: str
-    :return: the synthetic dataframe containing body+ data
-    :rtype: pd.DataFrame
-    """
-
-    # captures before/after meal weight discrepancies, offset from mean weight
-    offsets = [0] * 7 + [
-        -1,
-        -1,
-        -0.5,
-        -0.5,
-        0.5,
-        0.5,
-        0.2,
-        0,
-        -0.2,
-        -0.5,
-        -0.1,
-        0.7,
-        0.8,
-        0.7,
-        0.6,
-        0.6,
-    ]
-
-    total_duration = 75168000  # 2.5 years in seconds
-    start_ts = int(datetime.strptime(start_date, "%Y-%m-%d").timestamp())
-
-    # generate times by the day, sample from 8am to 11:59pm
-    random_times = []
-    for dt in range(start_ts, start_ts + total_duration, 24 * 3600):
-        random_times += list(
-            np.random.uniform(
-                dt + 8 * 3600, dt + 24 * 3600, size=np.random.randint(0, 5)
-            )
-        )
-
-    # delete so we have 1400 elements in the end
-    to_delete = np.random.choice(
-        len(random_times), size=len(random_times) - 1400, replace=False
-    )
-    random_times = np.delete(random_times, to_delete)
-
-    weights = np.random.normal(60, 1, len(random_times)) + np.concatenate(
-        (np.linspace(8, 10, 200), np.linspace(10, 0, 1200))
-    )
-
-    random_times_hour = np.array(
-        [int(datetime.fromtimestamp(t).strftime("%H")) for t in random_times]
-    )
-
-    # now actually offset the weights
-    for i, offset in zip(range(24), offsets):
-        special_idxes = np.where(random_times_hour == i)[0]
-        weights[special_idxes] = weights[special_idxes] + np.random.normal(
-            offset, 1, len(special_idxes)
-        )
-
-    fat_percent = np.random.normal(3, 1, len(random_times)) + np.concatenate(
-        (np.linspace(25, 30, 200), np.linspace(30, 13, 1200))
-    )
-
-    df = pd.DataFrame(columns=["date", "Weight (kg)", "Fat Ratio (%)"])
-
-    df.date = [datetime.fromtimestamp(t) for t in random_times]
-    df["Weight (kg)"] = weights
-    df["Fat Ratio (%)"] = fat_percent
-
-    # user left out some data, went on vacation, etc.
-    df.drop(index=df.index[300:310], axis=0, inplace=True)
-
-    df.drop(index=df.index[400:410], axis=0, inplace=True)
-
-    return df
+import hashlib
+from datetime import datetime, timedelta
+
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+
+__all__ = ["create_synthetic_sleeps_df", "create_syn_hr", "create_syn_bodyplus"]
+
+#############
+# ScanWatch #
+#############
+
+
+def create_synthetic_sleeps_df(start_date, end_date):
+    """Create a synthetic dataframe of sleep data. This is for
+    the ScanWatch.
+
+    :param start_date: the start date of the synthetic data as a string formatted as YYYY-MM-DD
+    :type start_date: str
+    :param end_date: the end date of the synthetic data as a string formatted as YYYY-MM-DD
+    :type end_date: str
+    :return: the synthetic dataframe containing sleep data
+    :rtype: pd.DataFrame
+    """
+
+    start_day = datetime.strptime(start_date, "%Y-%m-%d")
+    end_day = datetime.strptime(end_date, "%Y-%m-%d")
+    num_days = (end_day - start_day).days
+
+    syn_sleeps = pd.DataFrame()
+
+    syn_sleeps["id"] = np.random.randint(0, 100000000, size=(num_days,))
+    syn_sleeps["timezone"] = "America/Los_Angeles"
+    syn_sleeps["model"] = 16
+    syn_sleeps["model_id"] = 93
+    syn_sleeps[
+        "hash_deviceid"
+    ] = "d41d8cd98f00b204e9800998ecf8427e"  # randomly generated
+    syn_sleeps["date"] = [
+        datetime.fromtimestamp(
+            datetime.strptime(start_date, "%Y-%m-%d").timestamp() + i * 24 * 3600
+        ).strftime("%Y-%m-%d")
+        for i in range(num_days)
+    ]
+
+    startdates = []
+    enddates = []
+
+    for date in syn_sleeps["date"]:
+        sleep_start = np.random.randint(20, 27)
+        sleep_time = np.random.randint(4, 9)
+
+        startdate = datetime.strptime(date, "%Y-%m-%d") + timedelta(
+            hours=sleep_start + 7
+        )
+
+        enddate = startdate + timedelta(hours=sleep_time)
+
+        startdate, enddate = int(startdate.timestamp()), int(enddate.timestamp())
+
+        startdates.append(startdate)
+        enddates.append(enddate)
+
+    all_data = []
+
+    for _ in range(num_days):
+
+        data = {
+            "wakeupduration": np.random.randint(0, 3000),
+            "wakeupcount": np.random.poisson(1),
+            "durationtosleep": np.random.randint(120, 180),
+            "durationtowakeup": np.random.randint(0, 700),
+            "total_timeinbed": np.random.randint(10000, 50000),
+            "total_sleep_time": np.random.randint(10000, 50000),
+            "sleep_efficiency": np.random.rand() * 0.1 + 0.9,
+            "sleep_latency": np.random.randint(120, 130),
+            "wakeup_latency": np.random.randint(0, 800),
+            "waso": np.random.randint(0, 4000),
+            "nb_rem_episodes": 0,
+            "out_of_bed_count": 0,
+            "lightsleepduration": np.random.randint(6000, 35000),
+            "deepsleepduration": np.random.randint(3000, 17000),
+            "hr_average": np.random.randint(55, 65),
+            "hr_min": np.random.randint(40, 60),
+            "hr_max": np.random.randint(70, 120),
+            "sleep_score": np.random.randint(30, 80),
+        }
+
+        all_data.append(data)
+
+    syn_sleeps["startdate"] = startdates
+    syn_sleeps["enddate"] = enddates
+
+    syn_sleeps["data"] = all_data
+
+    syn_sleeps["created"] = enddates
+    syn_sleeps["modified"] = enddates
+
+    return syn_sleeps
+
+
+def create_syn_hr(start_date, end_date, syn_sleeps):
+    """Create a synthetic dataframe of heart rate data. This is for
+    the ScanWatch.
+
+    :param syn_sleeps: the synthetic sleep dataframe
+    :type syn_sleeps: pd.DataFrame
+    :return: the synthetic dataframe containing heart rate data
+    :rtype: pd.DataFrame
+    """
+    start_day = datetime.strptime(start_date, "%Y-%m-%d")
+    end_day = datetime.strptime(end_date, "%Y-%m-%d")
+
+    num_days = (end_day - start_day).days
+
+    hour_usage = [0.8] * 3 + [0.9] * 7 + [1.0] * 10 + [0.9] * 4
+
+    datetimes = []
+
+    for day_offset in tqdm(range(num_days)):
+        for hour_offset in range(24):
+            for minute_offset in range(0, 60, 10):
+                day = start_day + timedelta(days=day_offset)
+                hour = day + timedelta(hours=hour_offset)
+                minute = hour + timedelta(minutes=minute_offset)
+
+                if np.random.uniform(0, 1) < hour_usage[hour_offset]:
+                    datetimes.append(minute)
+
+    hr_measurements = (np.random.randn(len(datetimes)) * 5 + 90).astype("int")
+
+    timestamps = np.array([dt.timestamp() for dt in datetimes])
+
+    for i, (startdate, enddate) in tqdm(
+        enumerate(zip(syn_sleeps.startdate, syn_sleeps.enddate))
+    ):
+        idxes = np.where(np.logical_and(timestamps > startdate, timestamps < enddate))[
+            0
+        ]
+        duration = (enddate - startdate) / 3600
+        avg_hr = -5 / 7 * duration + 64.1428571429
+
+        hr_measurements[idxes] = (np.random.randn(idxes.shape[0]) + avg_hr).astype(
+            "int"
+        )
+
+    syn_hr = pd.DataFrame()
+    syn_hr["datetime"] = datetimes
+    syn_hr["heart_rate"] = hr_measurements
+
+    syn_hr["model"] = "ScanWatch"
+    syn_hr["model_id"] = 93
+    syn_hr["deviceid"] = hashlib.md5().hexdigest()
+
+    num_garbage = 1000
+
+    timestamps_garbage = np.random.uniform(
+        (start_day - timedelta(days=100)).timestamp(),
+        start_day.timestamp(),
+        size=num_garbage,
+    )
+
+    garbage_df = pd.DataFrame()
+    garbage_df["datetime"] = [
+        datetime.fromtimestamp(int(ts)) for ts in timestamps_garbage
+    ]
+    garbage_df["heart_rate"] = (np.random.randn(num_garbage) * 5 + 90).astype("int")
+
+    garbage_df["model"] = None
+    garbage_df["model_id"] = 1059
+    garbage_df["deviceid"] = None
+
+    syn_hr = pd.concat((garbage_df, syn_hr), ignore_index=True)
+
+    return syn_hr
+
+
+#########
+# Body+ #
+#########
+
+
+def create_syn_bodyplus(start_date):
+    """Create a synthetic dataframe of body+ data. This is for
+    the Body+ scale. The reason why we don't have an end date is
+    because we wish to generate 2.5 years' worth of data to portray
+    a fictional scenario where the user has been using the scale
+    for a year and we see the impact of a fictional medication.
+
+    :param start_date: the start date as a string formatted as YYYY-MM-DD
+    :type start_date: str
+    :return: the synthetic dataframe containing body+ data
+    :rtype: pd.DataFrame
+    """
+
+    # captures before/after meal weight discrepancies, offset from mean weight
+    offsets = [0] * 7 + [
+        -1,
+        -1,
+        -0.5,
+        -0.5,
+        0.5,
+        0.5,
+        0.2,
+        0,
+        -0.2,
+        -0.5,
+        -0.1,
+        0.7,
+        0.8,
+        0.7,
+        0.6,
+        0.6,
+    ]
+
+    total_duration = 75168000  # 2.5 years in seconds
+    start_ts = int(datetime.strptime(start_date, "%Y-%m-%d").timestamp())
+
+    # generate times by the day, sample from 8am to 11:59pm
+    random_times = []
+    for dt in range(start_ts, start_ts + total_duration, 24 * 3600):
+        random_times += list(
+            np.random.uniform(
+                dt + 8 * 3600, dt + 24 * 3600, size=np.random.randint(0, 5)
+            )
+        )
+
+    # delete so we have 1400 elements in the end
+    to_delete = np.random.choice(
+        len(random_times), size=len(random_times) - 1400, replace=False
+    )
+    random_times = np.delete(random_times, to_delete)
+
+    weights = np.random.normal(60, 1, len(random_times)) + np.concatenate(
+        (np.linspace(8, 10, 200), np.linspace(10, 0, 1200))
+    )
+
+    random_times_hour = np.array(
+        [int(datetime.fromtimestamp(t).strftime("%H")) for t in random_times]
+    )
+
+    # now actually offset the weights
+    for i, offset in zip(range(24), offsets):
+        special_idxes = np.where(random_times_hour == i)[0]
+        weights[special_idxes] = weights[special_idxes] + np.random.normal(
+            offset, 1, len(special_idxes)
+        )
+
+    fat_percent = np.random.normal(3, 1, len(random_times)) + np.concatenate(
+        (np.linspace(25, 30, 200), np.linspace(30, 13, 1200))
+    )
+
+    df = pd.DataFrame(columns=["date", "Weight (kg)", "Fat Ratio (%)"])
+
+    df.date = [datetime.fromtimestamp(t) for t in random_times]
+    df["Weight (kg)"] = weights
+    df["Fat Ratio (%)"] = fat_percent
+
+    # user left out some data, went on vacation, etc.
+    df.drop(index=df.index[300:310], axis=0, inplace=True)
+
+    df.drop(index=df.index[400:410], axis=0, inplace=True)
+
+    return df
```

### Comparing `wearipedia-0.1.2/PKG-INFO` & `wearipedia-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: wearipedia
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wearable data for all
 Home-page: http://wearipedia.com
 License: MIT
 Author: The Stanford Wearipedia Project
 Author-email: arjo@stanford.edu
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: fastapi (==0.101)
+Requires-Dist: fbm (>=0.3.0,<0.4.0)
 Requires-Dist: garminconnect (>=0.1.48,<0.2.0)
-Requires-Dist: pandas (>=1.1,<2.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: lida (>=0.0.11,<0.0.12)
+Requires-Dist: myfitnesspal (>=2.0.1,<3.0.0)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: polyline (>=2.0.0,<3.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: scipy (>=1.6,<2.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/Stanford-Health/wearipedia
 Description-Content-Type: text/markdown
 
 # wearipedia
 
 <div align="center">
```

