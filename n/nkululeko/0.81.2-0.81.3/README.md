# Comparing `tmp/nkululeko-0.81.2.tar.gz` & `tmp/nkululeko-0.81.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.81.2.tar", last modified: Mon Apr 15 11:56:11 2024, max compression
+gzip compressed data, was "nkululeko-0.81.3.tar", last modified: Tue Apr 16 14:07:48 2024, max compression
```

## Comparing `nkululeko-0.81.2.tar` & `nkululeko-0.81.3.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16443 2024-04-15 11:35:17.000000 nkululeko-0.81.2/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.2/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34523 2024-04-15 11:56:11.319774 nkululeko-0.81.2/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.2/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.2/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.2/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.2/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.2/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.2/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.2/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/crema-d/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3281 2023-06-13 12:24:10.000000 nkululeko-0.81.2/data/crema-d/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.2/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.2/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.2/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.2/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.2/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.2/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3327 2023-08-31 07:30:49.000000 nkululeko-0.81.2/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.2/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.2/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.2/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3072 2024-03-13 09:14:20.000000 nkululeko-0.81.2/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.2/meta/demos/demo_best_model.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/meta/demos/multiple_exeriments/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.2/meta/demos/multiple_exeriments/do_experiments.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.2/meta/demos/multiple_exeriments/parse_nkulu.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.2/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.2/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.2/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.2/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.2/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.2/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.2/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.2/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.2/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.2/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.2/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4818 2023-09-26 13:42:48.000000 nkululeko-0.81.2/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.2/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-15 11:55:58.000000 nkululeko-0.81.2/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.2/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27265 2024-03-27 10:33:18.000000 nkululeko-0.81.2/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.2/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2500 2024-03-14 10:49:21.000000 nkululeko-0.81.2/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.2/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4733 2024-04-15 11:33:44.000000 nkululeko-0.81.2/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29575 2024-03-18 15:37:11.000000 nkululeko-0.81.2/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2250 2024-02-29 11:07:16.000000 nkululeko-0.81.2/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.2/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3192 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3278 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3108 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3078 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-03-11 08:25:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4149 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3039 2023-12-15 13:29:14.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2771 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4521 2024-02-20 12:42:26.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21287 2024-04-15 11:30:05.000000 nkululeko-0.81.2/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7281 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.2/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.2/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.2/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.2/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9337 2024-02-26 18:28:01.000000 nkululeko-0.81.2/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.2/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11638 2024-03-21 10:35:30.000000 nkululeko-0.81.2/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.2/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9716 2024-02-13 14:17:48.000000 nkululeko-0.81.2/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.2/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.2/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.2/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.2/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9097 2024-03-12 12:49:32.000000 nkululeko-0.81.2/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10054 2024-03-21 10:35:22.000000 nkululeko-0.81.2/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      867 2024-03-21 10:56:45.000000 nkululeko-0.81.2/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.2/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.2/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.2/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.2/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.2/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5732 2024-03-11 14:48:46.000000 nkululeko-0.81.2/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.2/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.2/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1876 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/predict.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11497 2024-02-13 13:56:24.000000 nkululeko-0.81.2/nkululeko/reporter.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.2/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.2/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.2/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.2/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2233 2024-03-14 15:08:12.000000 nkululeko-0.81.2/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      574 2024-02-13 13:17:42.000000 nkululeko-0.81.2/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7451 2024-02-26 18:30:48.000000 nkululeko-0.81.2/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.2/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.2/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.2/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.2/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.2/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1486 2024-03-18 15:18:33.000000 nkululeko-0.81.2/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2695 2024-03-18 15:40:15.000000 nkululeko-0.81.2/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.2/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.2/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2788 2023-12-19 11:26:19.000000 nkululeko-0.81.2/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.2/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34523 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5124 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.2/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      968 2024-04-15 11:56:11.319774 nkululeko-0.81.2/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.2/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.2/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16523 2024-04-16 12:34:42.000000 nkululeko-0.81.3/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.3/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34664 2024-04-16 14:07:48.790954 nkululeko-0.81.3/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.3/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.3/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.3/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.3/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.3/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.3/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.3/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/crema-d/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3281 2023-06-13 12:24:10.000000 nkululeko-0.81.3/data/crema-d/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.3/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.3/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.3/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.3/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.3/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.3/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.3/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.3/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3327 2023-08-31 07:30:49.000000 nkululeko-0.81.3/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.3/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.3/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.3/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.3/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.3/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3072 2024-03-13 09:14:20.000000 nkululeko-0.81.3/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.3/meta/demos/demo_best_model.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.782954 nkululeko-0.81.3/meta/demos/multiple_exeriments/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.3/meta/demos/multiple_exeriments/do_experiments.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.3/meta/demos/multiple_exeriments/parse_nkulu.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.3/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.3/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.3/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.3/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.3/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.3/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.3/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.3/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.3/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.3/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.3/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4818 2023-09-26 13:42:48.000000 nkululeko-0.81.3/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.3/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-16 12:34:59.000000 nkululeko-0.81.3/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.3/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27265 2024-03-27 10:33:18.000000 nkululeko-0.81.3/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.3/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2500 2024-03-14 10:49:21.000000 nkululeko-0.81.3/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.3/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4733 2024-04-15 11:33:44.000000 nkululeko-0.81.3/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29575 2024-03-18 15:37:11.000000 nkululeko-0.81.3/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2250 2024-02-29 11:07:16.000000 nkululeko-0.81.3/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.3/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3192 2024-03-12 12:44:04.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3108 2024-03-12 12:44:04.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3078 2024-03-12 12:44:04.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-03-11 08:25:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4149 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3039 2023-12-15 13:29:14.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2771 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4521 2024-02-20 12:42:26.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.3/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.81.3/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7281 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.3/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.786954 nkululeko-0.81.3/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.3/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.3/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.3/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9337 2024-02-26 18:28:01.000000 nkululeko-0.81.3/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.3/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11648 2024-04-16 11:54:27.000000 nkululeko-0.81.3/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.3/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.81.3/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.3/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.3/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.3/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.3/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.81.3/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.81.3/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      867 2024-03-21 10:56:45.000000 nkululeko-0.81.3/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.3/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.3/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.3/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.3/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.3/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5732 2024-03-11 14:48:46.000000 nkululeko-0.81.3/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.3/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.3/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1876 2023-12-19 11:16:14.000000 nkululeko-0.81.3/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.3/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.3/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.3/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.3/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.3/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12670 2024-04-16 13:43:47.000000 nkululeko-0.81.3/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.81.3/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2233 2024-03-14 15:08:12.000000 nkululeko-0.81.3/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7461 2024-04-16 11:54:24.000000 nkululeko-0.81.3/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.3/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.3/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.3/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.3/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.3/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.3/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1486 2024-03-18 15:18:33.000000 nkululeko-0.81.3/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2695 2024-03-18 15:40:15.000000 nkululeko-0.81.3/nkululeko/test_predictor.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.3/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.3/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2788 2023-12-19 11:26:19.000000 nkululeko-0.81.3/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.3/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34664 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5144 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-16 14:07:48.000000 nkululeko-0.81.3/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.3/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-16 14:07:48.790954 nkululeko-0.81.3/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.3/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.778954 nkululeko-0.81.3/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-16 14:07:48.790954 nkululeko-0.81.3/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.3/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.81.2/CHANGELOG.md` & `nkululeko-0.81.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.81.3
+--------------
+* added confidence intervals to result reporting
+
 Version 0.81.2
 --------------
 * added a parselmouth.Praat error if pitch out of range
 * changed file path for demo_predictor
 
 Version 0.81.1
 --------------
```

### Comparing `nkululeko-0.81.2/LICENSE` & `nkululeko-0.81.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/PKG-INFO` & `nkululeko-0.81.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.2
+Version: 0.81.3
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audeer
 Requires-Dist: audformat
 Requires-Dist: audinterface
 Requires-Dist: audiofile
 Requires-Dist: audiomentations
+Requires-Dist: audmetric
 Requires-Dist: audonnx
+Requires-Dist: confidence_intervals
 Requires-Dist: datasets
 Requires-Dist: imageio
 Requires-Dist: laion-clap
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: opensmile
 Requires-Dist: pandas
@@ -317,14 +319,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.3
+--------------
+* added confidence intervals to result reporting
+
 Version 0.81.2
 --------------
 * added a parselmouth.Praat error if pitch out of range
 * changed file path for demo_predictor
 
 Version 0.81.1
 --------------
```

### Comparing `nkululeko-0.81.2/README.md` & `nkululeko-0.81.3/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/aesdd/process_database.py` & `nkululeko-0.81.3/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/androids/process_database.py` & `nkululeko-0.81.3/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/androids_orig/process_database.py` & `nkululeko-0.81.3/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/androids_test/process_database.py` & `nkululeko-0.81.3/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/ased/process_database.py` & `nkululeko-0.81.3/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/asvp-esd/process_database.py` & `nkululeko-0.81.3/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/baved/process_database.py` & `nkululeko-0.81.3/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/cafe/process_database.py` & `nkululeko-0.81.3/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/clac/process_database.py` & `nkululeko-0.81.3/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/cmu-mosei/process_database.py` & `nkululeko-0.81.3/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/crema-d/process_database.py` & `nkululeko-0.81.3/data/crema-d/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/demos/process_database.py` & `nkululeko-0.81.3/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/ekorpus/process_database.py` & `nkululeko-0.81.3/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emns/process_database.py` & `nkululeko-0.81.3/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emofilm/convert_to_16k.py` & `nkululeko-0.81.3/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emofilm/process_database.py` & `nkululeko-0.81.3/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emorynlp/process_database.py` & `nkululeko-0.81.3/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emov-db/process_database.py` & `nkululeko-0.81.3/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emovo/process_database.py` & `nkululeko-0.81.3/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/emozionalmente/create.py` & `nkululeko-0.81.3/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/enterface/process_database.py` & `nkululeko-0.81.3/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/esd/process_database.py` & `nkululeko-0.81.3/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/gerparas/process_database.py` & `nkululeko-0.81.3/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/iemocap/process_database.py` & `nkululeko-0.81.3/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/jl/process_database.py` & `nkululeko-0.81.3/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/jtes/process_database.py` & `nkululeko-0.81.3/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/meld/process_database.py` & `nkululeko-0.81.3/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/mesd/process_database.py` & `nkululeko-0.81.3/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/mess/process_database.py` & `nkululeko-0.81.3/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/mlendsnd/process_database.py` & `nkululeko-0.81.3/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/msp-improv/process_database2.py` & `nkululeko-0.81.3/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/msp-podcast/process_database.py` & `nkululeko-0.81.3/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/oreau2/process_database.py` & `nkululeko-0.81.3/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/portuguese/process_database.py` & `nkululeko-0.81.3/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/ravdess/process_database.py` & `nkululeko-0.81.3/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/ravdess/process_database_speaker.py` & `nkululeko-0.81.3/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/savee/process_database.py` & `nkululeko-0.81.3/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/shemo/process_database.py` & `nkululeko-0.81.3/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/subesco/process_database.py` & `nkululeko-0.81.3/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/tess/process_database.py` & `nkululeko-0.81.3/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/thorsten-emotional/process_database.py` & `nkululeko-0.81.3/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/urdu/process_database.py` & `nkululeko-0.81.3/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/data/vivae/process_database.py` & `nkululeko-0.81.3/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/docs/source/conf.py` & `nkululeko-0.81.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/meta/demos/demo_best_model.py` & `nkululeko-0.81.3/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/meta/demos/multiple_exeriments/do_experiments.py` & `nkululeko-0.81.3/meta/demos/multiple_exeriments/do_experiments.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/meta/demos/multiple_exeriments/parse_nkulu.py` & `nkululeko-0.81.3/meta/demos/multiple_exeriments/parse_nkulu.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/meta/demos/my_experiment.py` & `nkululeko-0.81.3/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/meta/demos/my_experiment_local.py` & `nkululeko-0.81.3/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/meta/demos/plot_faster_anim.py` & `nkululeko-0.81.3/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/aug_train.py` & `nkululeko-0.81.3/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/augment.py` & `nkululeko-0.81.3/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/augmenting/augmenter.py` & `nkululeko-0.81.3/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.81.3/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.81.3/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/augmenting/resampler.py` & `nkululeko-0.81.3/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_age.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.81.3/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.81.3/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/cacheddataset.py` & `nkululeko-0.81.3/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/data/dataset.py` & `nkululeko-0.81.3/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/data/dataset_csv.py` & `nkululeko-0.81.3/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/demo.py` & `nkululeko-0.81.3/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/demo_feats.py` & `nkululeko-0.81.3/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/demo_predictor.py` & `nkululeko-0.81.3/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/experiment.py` & `nkululeko-0.81.3/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/explore.py` & `nkululeko-0.81.3/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/export.py` & `nkululeko-0.81.3/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,19 @@
         if not os.path.isdir(model_root):
             cache_root = audeer.mkdir("cache")
             model_root = audeer.mkdir(model_root)
             archive_path = audeer.download_url(model_url, cache_root, verbose=True)
             audeer.extract_archive(archive_path, model_root)
         device = self.util.config_val("MODEL", "device", "cpu")
         self.model = audonnx.load(model_root, device=device)
-        pytorch_total_params = sum(p.numel() for p in self.model.parameters())
-        self.util.debug(
-            f"initialized agender model with {pytorch_total_params} parameters in total"
-        )
+        #        pytorch_total_params = sum(p.numel() for p in self.model.parameters())
+        # self.util.debug(
+        #     f"initialized agender model with {pytorch_total_params} parameters in total"
+        # )
+        self.util.debug("initialized agender model")
         self.model_loaded = True
 
     def extract(self):
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path("store")
         store_format = self.util.config_val("FEATS", "store_format", "pkl")
         storage = f"{store}{self.name}.{store_format}"
```

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel_dim.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/featureset.py` & `nkululeko-0.81.3/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.81.3/nkululeko/feat_extract/feinberg_praat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,146 +1,145 @@
-"""
-This is a copy of David R. Feinberg's Praat scripts
+"""This is a copy of David R. Feinberg's Praat scripts.
 https://github.com/drfeinberg/PraatScripts
-taken June 23rd 2022
+taken June 23rd 2022.
 """
 
 #!/usr/bin/env python3
+import math
+import statistics
+
 import numpy as np
 import pandas as pd
-import math
-from tqdm import tqdm
 import parselmouth
-import statistics
-from nkululeko.utils.util import Util
-import audiofile
 from parselmouth.praat import call
 from scipy.stats.mstats import zscore
 from sklearn.decomposition import PCA
-from sklearn.preprocessing import StandardScaler
+from tqdm import tqdm
+
+import audiofile
 
 
 # This is the function to measure source acoustics using default male parameters.
 
 
-def measurePitch(voiceID, f0min, f0max, unit):
-    sound = parselmouth.Sound(voiceID)  # read the sound
+def measure_pitch(voice_id, f0min, f0max, unit):
+    sound = parselmouth.Sound(voice_id)  # read the sound
     duration = call(sound, "Get total duration")  # duration
     pitch = call(sound, "To Pitch", 0.0, f0min, f0max)  # create a praat pitch object
-    meanF0 = call(pitch, "Get mean", 0, 0, unit)  # get mean pitch
-    stdevF0 = call(
+    mean_f0 = call(pitch, "Get mean", 0, 0, unit)  # get mean pitch
+    stdev_f0 = call(
         pitch, "Get standard deviation", 0, 0, unit
     )  # get standard deviation
     harmonicity = call(sound, "To Harmonicity (cc)", 0.01, f0min, 0.1, 1.0)
     hnr = call(harmonicity, "Get mean", 0, 0)
-    pointProcess = call(sound, "To PointProcess (periodic, cc)", f0min, f0max)
-    localJitter = call(pointProcess, "Get jitter (local)", 0, 0, 0.0001, 0.02, 1.3)
-    localabsoluteJitter = call(
-        pointProcess, "Get jitter (local, absolute)", 0, 0, 0.0001, 0.02, 1.3
-    )
-    rapJitter = call(pointProcess, "Get jitter (rap)", 0, 0, 0.0001, 0.02, 1.3)
-    ppq5Jitter = call(pointProcess, "Get jitter (ppq5)", 0, 0, 0.0001, 0.02, 1.3)
-    ddpJitter = call(pointProcess, "Get jitter (ddp)", 0, 0, 0.0001, 0.02, 1.3)
-    localShimmer = call(
-        [sound, pointProcess],
+    point_process = call(sound, "To PointProcess (periodic, cc)", f0min, f0max)
+    local_jitter = call(point_process, "Get jitter (local)", 0, 0, 0.0001, 0.02, 1.3)
+    localabsolute_jitter = call(
+        point_process, "Get jitter (local, absolute)", 0, 0, 0.0001, 0.02, 1.3
+    )
+    rap_jitter = call(point_process, "Get jitter (rap)", 0, 0, 0.0001, 0.02, 1.3)
+    ppq5_jitter = call(point_process, "Get jitter (ppq5)", 0, 0, 0.0001, 0.02, 1.3)
+    ddp_jitter = call(point_process, "Get jitter (ddp)", 0, 0, 0.0001, 0.02, 1.3)
+    local_shimmer = call(
+        [sound, point_process],
         "Get shimmer (local)",
         0,
         0,
         0.0001,
         0.02,
         1.3,
         1.6,
     )
-    localdbShimmer = call(
-        [sound, pointProcess],
+    localdb_shimmer = call(
+        [sound, point_process],
         "Get shimmer (local_dB)",
         0,
         0,
         0.0001,
         0.02,
         1.3,
         1.6,
     )
-    apq3Shimmer = call(
-        [sound, pointProcess],
+    apq3_shimmer = call(
+        [sound, point_process],
         "Get shimmer (apq3)",
         0,
         0,
         0.0001,
         0.02,
         1.3,
         1.6,
     )
-    aqpq5Shimmer = call(
-        [sound, pointProcess],
+    aqpq5_shimmer = call(
+        [sound, point_process],
         "Get shimmer (apq5)",
         0,
         0,
         0.0001,
         0.02,
         1.3,
         1.6,
     )
-    apq11Shimmer = call(
-        [sound, pointProcess],
+    apq11_shimmer = call(
+        [sound, point_process],
         "Get shimmer (apq11)",
         0,
         0,
         0.0001,
         0.02,
         1.3,
         1.6,
     )
-    ddaShimmer = call(
-        [sound, pointProcess], "Get shimmer (dda)", 0, 0, 0.0001, 0.02, 1.3, 1.6
+    dda_shimmer = call(
+        [sound, point_process], "Get shimmer (dda)", 0, 0, 0.0001, 0.02, 1.3, 1.6
     )
 
     return (
         duration,
-        meanF0,
-        stdevF0,
+        mean_f0,
+        stdev_f0,
         hnr,
-        localJitter,
-        localabsoluteJitter,
-        rapJitter,
-        ppq5Jitter,
-        ddpJitter,
-        localShimmer,
-        localdbShimmer,
-        apq3Shimmer,
-        aqpq5Shimmer,
-        apq11Shimmer,
-        ddaShimmer,
+        local_jitter,
+        localabsolute_jitter,
+        rap_jitter,
+        ppq5_jitter,
+        ddp_jitter,
+        local_shimmer,
+        localdb_shimmer,
+        apq3_shimmer,
+        aqpq5_shimmer,
+        apq11_shimmer,
+        dda_shimmer,
     )
 
 
 # ## This function measures formants at each glottal pulse
 #
 # Puts, D. A., Apicella, C. L., & Cárdenas, R. A. (2012). Masculine voices signal men's threat potential in forager and industrial societies. Proceedings of the Royal Society of London B: Biological Sciences, 279(1728), 601-609.
 #
 # Adapted from: DOI 10.17605/OSF.IO/K2BHS
 # This function measures formants using Formant Position formula
 # def measureFormants(sound, wave_file, f0min,f0max):
-def measureFormants(sound, f0min, f0max):
+def measure_formants(sound, f0min, f0max):
     sound = parselmouth.Sound(sound)  # read the sound
     #    pitch = call(sound, "To Pitch (cc)", 0, f0min, 15, 'no', 0.03, 0.45, 0.01, 0.35, 0.14, f0max)
-    pointProcess = call(sound, "To PointProcess (periodic, cc)", f0min, f0max)
+    point_process = call(sound, "To PointProcess (periodic, cc)", f0min, f0max)
 
     formants = call(sound, "To Formant (burg)", 0.0025, 5, 5000, 0.025, 50)
-    numPoints = call(pointProcess, "Get number of points")
+    num_points = call(point_process, "Get number of points")
 
     f1_list = []
     f2_list = []
     f3_list = []
     f4_list = []
 
     # Measure formants only at glottal pulses
-    for point in range(0, numPoints):
+    for point in range(0, num_points):
         point += 1
-        t = call(pointProcess, "Get time from index", point)
+        t = call(point_process, "Get time from index", point)
         f1 = call(formants, "Get value at time", 1, t, "Hertz", "Linear")
         f2 = call(formants, "Get value at time", 2, t, "Hertz", "Linear")
         f3 = call(formants, "Get value at time", 3, t, "Hertz", "Linear")
         f4 = call(formants, "Get value at time", 4, t, "Hertz", "Linear")
         f1_list.append(f1)
         f2_list.append(f2)
         f3_list.append(f3)
@@ -175,15 +174,15 @@
         f4_median,
     )
 
 
 # ## This function runs a 2-factor Principle Components Analysis (PCA) on Jitter and Shimmer
 
 
-def runPCA(df):
+def run_pca(df):
     # z-score the Jitter and Shimmer measurements
     measures = [
         "localJitter",
         "localabsoluteJitter",
         "rapJitter",
         "ppq5Jitter",
         "ddpJitter",
@@ -207,50 +206,49 @@
         x[np.isnan(x)] = 0
     # if np.any(np.isfinite(x[0])):
     #     print(f"Warning: {np.count_nonzero(np.isfinite(x))} finite in x")
 
     # PCA
     pca = PCA(n_components=2)
     try:
-        principalComponents = pca.fit_transform(x)
-        if np.any(np.isnan(principalComponents)):
+        principal_components = pca.fit_transform(x)
+        if np.any(np.isnan(principal_components)):
             print("pc is nan")
-            print(f"count: {np.count_nonzero(np.isnan(principalComponents))}")
-            print(principalComponents)
-            principalComponents = np.nan_to_num(principalComponents)
+            print(f"count: {np.count_nonzero(np.isnan(principal_components))}")
+            print(principal_components)
+            principal_components = np.nan_to_num(principal_components)
     except ValueError:
         print("need more than one file for pca")
-        principalComponents = [[0, 0]]
-    principalDf = pd.DataFrame(
-        data=principalComponents, columns=["JitterPCA", "ShimmerPCA"]
+        principal_components = [[0, 0]]
+    principal_df = pd.DataFrame(
+        data=principal_components, columns=["JitterPCA", "ShimmerPCA"]
     )
-    return principalDf
+    return principal_df
 
 
 # ## This block of code runs the above functions on all of the '.wav' files in the /audio folder
 
 
 def compute_features(file_index):
     # create lists to put the results
-    file_list = []
     duration_list = []
-    mean_F0_list = []
-    sd_F0_list = []
+    mean_f0_list = []
+    sd_f0_list = []
     hnr_list = []
-    localJitter_list = []
-    localabsoluteJitter_list = []
-    rapJitter_list = []
-    ppq5Jitter_list = []
-    ddpJitter_list = []
-    localShimmer_list = []
-    localdbShimmer_list = []
-    apq3Shimmer_list = []
-    aqpq5Shimmer_list = []
-    apq11Shimmer_list = []
-    ddaShimmer_list = []
+    local_jitter_list = []
+    localabsolute_jitter_list = []
+    rap_jitter_list = []
+    ppq5_jitter_list = []
+    ddp_jitter_list = []
+    local_shimmer_list = []
+    localdb_shimmer_list = []
+    apq3_shimmer_list = []
+    aqpq5_shimmer_list = []
+    apq11_shimmer_list = []
+    dda_shimmer_list = []
     f1_mean_list = []
     f2_mean_list = []
     f3_mean_list = []
     f4_mean_list = []
     f1_median_list = []
     f2_median_list = []
     f3_median_list = []
@@ -264,60 +262,60 @@
             duration=(end - start).total_seconds(),
             always_2d=True,
         )
         try:
             sound = parselmouth.Sound(values=signal, sampling_frequency=sampling_rate)
             (
                 duration,
-                meanF0,
-                stdevF0,
+                mean_f0,
+                stdev_f0,
                 hnr,
-                localJitter,
-                localabsoluteJitter,
-                rapJitter,
-                ppq5Jitter,
-                ddpJitter,
-                localShimmer,
-                localdbShimmer,
-                apq3Shimmer,
-                aqpq5Shimmer,
-                apq11Shimmer,
-                ddaShimmer,
-            ) = measurePitch(sound, 75, 300, "Hertz")
+                local_jitter,
+                localabsolute_jitter,
+                rap_jitter,
+                ppq5_jitter,
+                ddp_jitter,
+                local_shimmer,
+                localdb_shimmer,
+                apq3_shimmer,
+                aqpq5_shimmer,
+                apq11_shimmer,
+                dda_shimmer,
+            ) = measure_pitch(sound, 75, 300, "Hertz")
             (
                 f1_mean,
                 f2_mean,
                 f3_mean,
                 f4_mean,
                 f1_median,
                 f2_median,
                 f3_median,
                 f4_median,
-            ) = measureFormants(sound, 75, 300)
+            ) = measure_formants(sound, 75, 300)
             #        file_list.append(wave_file) # make an ID list
         except (statistics.StatisticsError, parselmouth.PraatError) as errors:
             print(f"error on file {wave_file}: {errors}")
 
         duration_list.append(duration)  # make duration list
-        mean_F0_list.append(meanF0)  # make a mean F0 list
-        sd_F0_list.append(stdevF0)  # make a sd F0 list
+        mean_f0_list.append(mean_f0)  # make a mean F0 list
+        sd_f0_list.append(stdev_f0)  # make a sd F0 list
         hnr_list.append(hnr)  # add HNR data
 
         # add raw jitter and shimmer measures
-        localJitter_list.append(localJitter)
-        localabsoluteJitter_list.append(localabsoluteJitter)
-        rapJitter_list.append(rapJitter)
-        ppq5Jitter_list.append(ppq5Jitter)
-        ddpJitter_list.append(ddpJitter)
-        localShimmer_list.append(localShimmer)
-        localdbShimmer_list.append(localdbShimmer)
-        apq3Shimmer_list.append(apq3Shimmer)
-        aqpq5Shimmer_list.append(aqpq5Shimmer)
-        apq11Shimmer_list.append(apq11Shimmer)
-        ddaShimmer_list.append(ddaShimmer)
+        local_jitter_list.append(local_jitter)
+        localabsolute_jitter_list.append(localabsolute_jitter)
+        rap_jitter_list.append(rap_jitter)
+        ppq5_jitter_list.append(ppq5_jitter)
+        ddp_jitter_list.append(ddp_jitter)
+        local_shimmer_list.append(local_shimmer)
+        localdb_shimmer_list.append(localdb_shimmer)
+        apq3_shimmer_list.append(apq3_shimmer)
+        aqpq5_shimmer_list.append(aqpq5_shimmer)
+        apq11_shimmer_list.append(apq11_shimmer)
+        dda_shimmer_list.append(dda_shimmer)
 
         # add the formant data
         f1_mean_list.append(f1_mean)
         f2_mean_list.append(f2_mean)
         f3_mean_list.append(f3_mean)
         f4_mean_list.append(f4_mean)
         f1_median_list.append(f1_median)
@@ -326,28 +324,28 @@
         f4_median_list.append(f4_median)
     # ## This block of code adds all of that data we just generated to a Pandas data frame
     # Add the data to Pandas
     df = pd.DataFrame(
         np.column_stack(
             [
                 duration_list,
-                mean_F0_list,
-                sd_F0_list,
+                mean_f0_list,
+                sd_f0_list,
                 hnr_list,
-                localJitter_list,
-                localabsoluteJitter_list,
-                rapJitter_list,
-                ppq5Jitter_list,
-                ddpJitter_list,
-                localShimmer_list,
-                localdbShimmer_list,
-                apq3Shimmer_list,
-                aqpq5Shimmer_list,
-                apq11Shimmer_list,
-                ddaShimmer_list,
+                local_jitter_list,
+                localabsolute_jitter_list,
+                rap_jitter_list,
+                ppq5_jitter_list,
+                ddp_jitter_list,
+                local_shimmer_list,
+                localdb_shimmer_list,
+                apq3_shimmer_list,
+                aqpq5_shimmer_list,
+                apq11_shimmer_list,
+                dda_shimmer_list,
                 f1_mean_list,
                 f2_mean_list,
                 f3_mean_list,
                 f4_mean_list,
                 f1_median_list,
                 f2_median_list,
                 f3_median_list,
@@ -378,15 +376,15 @@
             "f2_median",
             "f3_median",
             "f4_median",
         ],
     )
 
     # add pca data
-    pcaData = runPCA(df)  # Run jitter and shimmer PCA
+    pcaData = run_pca(df)  # Run jitter and shimmer PCA
     df = pd.concat([df, pcaData], axis=1)  # Add PCA data
     # reload the data so it's all numbers
     df.to_csv("processed_results.csv", index=False)
     df = pd.read_csv("processed_results.csv", header=0)
     #    df.sort_values('voiceID').head(20)
     # ## Next we calculate the vocal-tract length estimates
```

### Comparing `nkululeko-0.81.2/nkululeko/feature_extractor.py` & `nkululeko-0.81.3/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/file_checker.py` & `nkululeko-0.81.3/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/filter_data.py` & `nkululeko-0.81.3/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/losses/loss_ccc.py` & `nkululeko-0.81.3/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.81.3/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/modelrunner.py` & `nkululeko-0.81.3/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/models/model.py` & `nkululeko-0.81.3/nkululeko/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # model.py
 from nkululeko.utils.util import Util
 import pandas as pd
 import numpy as np
 import nkululeko.glob_conf as glob_conf
 import sklearn.utils
-from nkululeko.reporter import Reporter
+from nkululeko.reporting.reporter import Reporter
 import ast
 from sklearn.model_selection import GridSearchCV
 import pickle
 import random
 from sklearn.model_selection import LeaveOneGroupOut
 from sklearn.model_selection import StratifiedKFold
```

### Comparing `nkululeko-0.81.2/nkululeko/models/model_cnn.py` & `nkululeko-0.81.3/nkululeko/models/model_cnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from sklearn.metrics import recall_score
 from collections import OrderedDict
 from PIL import Image
 
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 from nkululeko.models.model import Model
-from nkululeko.reporter import Reporter
+from nkululeko.reporting.reporter import Reporter
 from nkululeko.losses.loss_softf1loss import SoftF1Loss
 
 
 class CNN_model(Model):
     """CNN = convolutional neural net"""
 
     is_classifier = True
```

### Comparing `nkululeko-0.81.2/nkululeko/models/model_gmm.py` & `nkululeko-0.81.3/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/models/model_knn.py` & `nkululeko-0.81.3/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/models/model_knn_reg.py` & `nkululeko-0.81.3/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/models/model_mlp.py` & `nkululeko-0.81.3/nkululeko/models/model_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # model_mlp.py
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 from nkululeko.models.model import Model
-from nkululeko.reporter import Reporter
+from nkululeko.reporting.reporter import Reporter
 import torch
 import ast
 import numpy as np
 from sklearn.metrics import recall_score
 from collections import OrderedDict
 from nkululeko.losses.loss_softf1loss import SoftF1Loss
```

### Comparing `nkululeko-0.81.2/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.81.3/nkululeko/models/model_mlp_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # model_mlp.py
-from nkululeko.utils.util import Util
-import nkululeko.glob_conf as glob_conf
-from nkululeko.models.model import Model
-from nkululeko.reporter import Reporter
-import torch
 import ast
-import numpy as np
-from sklearn.metrics import mean_squared_error, mean_absolute_error
 from collections import OrderedDict
-from nkululeko.losses.loss_ccc import ConcordanceCorCoeff
 import os
 
+import numpy as np
+import torch
+
+from audmetric import concordance_cc
+from audmetric import mean_absolute_error
+from audmetric import mean_squared_error
+
+import nkululeko.glob_conf as glob_conf
+from nkululeko.losses.loss_ccc import ConcordanceCorCoeff
+from nkululeko.models.model import Model
+from nkululeko.reporting.reporter import Reporter
+
 
 class MLP_Reg_model(Model):
     """MLP = multi layer perceptron"""
 
     is_classifier = False
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
@@ -197,15 +201,15 @@
         predictions = logits
         measure = self.util.config_val("MODEL", "measure", "mse")
         if measure == "mse":
             result = mean_squared_error(targets.numpy(), predictions.numpy())
         elif measure == "mae":
             result = mean_absolute_error(targets.numpy(), predictions.numpy())
         elif measure == "ccc":
-            result = Reporter.ccc(targets.numpy(), predictions.numpy())
+            result = concordance_cc(targets.numpy(), predictions.numpy())
         else:
             self.util.error(f"unknown measure: {measure}")
         return result, targets, predictions
 
     def store(self):
         torch.save(self.model.state_dict(), self.store_path)
```

### Comparing `nkululeko-0.81.2/nkululeko/models/model_svm.py` & `nkululeko-0.81.3/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/models/model_svr.py` & `nkululeko-0.81.3/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/multidb.py` & `nkululeko-0.81.3/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/nkululeko.py` & `nkululeko-0.81.3/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/plots.py` & `nkululeko-0.81.3/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/predict.py` & `nkululeko-0.81.3/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/reporter.py` & `nkululeko-0.81.3/nkululeko/reporting/reporter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import ast
 import glob
 import json
 import math
+
+from confidence_intervals import evaluate_with_conf_int
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.stats import pearsonr
-from sklearn.metrics import (
-    ConfusionMatrixDisplay,
-    accuracy_score,
-    classification_report,
-    confusion_matrix,
-    mean_squared_error,
-    mean_absolute_error,
-    r2_score,
-    recall_score,
-)
-from sklearn.utils import resample
+from sklearn.metrics import ConfusionMatrixDisplay
+from sklearn.metrics import classification_report
+from sklearn.metrics import confusion_matrix
+from sklearn.metrics import r2_score
+from torch import is_tensor
+
+from audmetric import accuracy
+from audmetric import concordance_cc
+from audmetric import mean_absolute_error
+from audmetric import mean_squared_error
+from audmetric import unweighted_average_recall
 
 import nkululeko.glob_conf as glob_conf
-from nkululeko.reporting.report_item import ReportItem
-from nkululeko.result import Result
 from nkululeko.reporting.defines import Header
+from nkululeko.reporting.report_item import ReportItem
+from nkululeko.reporting.result import Result
 from nkululeko.utils.util import Util
 
 
 class Reporter:
     def __set_measure(self):
         if self.util.exp_is_classification():
             self.MEASURE = "UAR"
@@ -40,50 +42,77 @@
                 self.MEASURE = "MAE"
                 self.result.measure = self.MEASURE
             elif self.measure == "ccc":
                 self.MEASURE = "CCC"
                 self.result.measure = self.MEASURE
 
     def __init__(self, truths, preds, run, epoch):
-        """Initialization with ground truth und predictions vector"""
+        """Initialization with ground truth und predictions vector."""
         self.util = Util("reporter")
         self.format = self.util.config_val("PLOT", "format", "png")
-        self.truths = truths
-        self.preds = preds
+        self.truths = np.asarray(truths)
+        self.preds = np.asarray(preds)
         self.result = Result(0, 0, 0, 0, "unknown")
         self.run = run
         self.epoch = epoch
         self.__set_measure()
         self.cont_to_cat = False
         if len(self.truths) > 0 and len(self.preds) > 0:
             if self.util.exp_is_classification():
-                self.result.test = recall_score(
-                    self.truths, self.preds, average="macro"
+                uar, (upper, lower) = evaluate_with_conf_int(
+                    self.preds,
+                    unweighted_average_recall,
+                    self.truths,
+                    num_bootstraps=1000,
+                    alpha=5,
                 )
-                self.result.loss = 1 - accuracy_score(self.truths, self.preds)
+                self.result.test = uar
+                self.result.set_upper_lower(upper, lower)
+                self.result.loss = 1 - accuracy(self.truths, self.preds)
             else:
                 # regression experiment
                 if self.measure == "mse":
-                    self.result.test = mean_squared_error(self.truths, self.preds)
+                    test_result, (upper, lower) = evaluate_with_conf_int(
+                        self.preds,
+                        mean_squared_error,
+                        self.truths,
+                        num_bootstraps=1000,
+                        alpha=5,
+                    )
                 elif self.measure == "mae":
-                    self.result.test = mean_absolute_error(self.truths, self.preds)
+                    test_result, (upper, lower) = evaluate_with_conf_int(
+                        self.preds,
+                        mean_absolute_error,
+                        self.truths,
+                        num_bootstraps=1000,
+                        alpha=5,
+                    )
                 elif self.measure == "ccc":
-                    self.result.test = self.ccc(self.truths, self.preds)
+                    test_result, (upper, lower) = evaluate_with_conf_int(
+                        self.preds,
+                        concordance_cc,
+                        self.truths,
+                        num_bootstraps=1000,
+                        alpha=5,
+                    )
+
                     if math.isnan(self.result.test):
                         self.util.debug(f"Truth: {self.truths}")
                         self.util.debug(f"Predict.: {self.preds}")
-                        self.util.debug(f"Result is NAN: setting to -1")
+                        self.util.debug("Result is NAN: setting to -1")
                         self.result.test = -1
                 else:
                     self.util.error(f"unknown measure: {self.measure}")
 
+                self.result.test = test_result
+                self.result.set_upper_lower(upper, lower)
                 # train and loss are being set by the model
 
     def set_id(self, run, epoch):
-        """Make the report identifiable with run and epoch index"""
+        """Make the report identifiable with run and epoch index."""
         self.run = run
         self.epoch = epoch
 
     def continuous_to_categorical(self):
         if self.cont_to_cat:
             return
         self.cont_to_cat = True
@@ -93,17 +122,20 @@
 
     def plot_confmatrix(self, plot_name, epoch):
         if not self.util.exp_is_classification():
             self.continuous_to_categorical()
         self._plot_confmat(self.truths, self.preds, plot_name, epoch)
 
     def plot_per_speaker(self, result_df, plot_name, function):
-        """Plot a confusion matrix with the mode category per speakers
+        """Plot a confusion matrix with the mode category per speakers.
+
         Args:
-            * result_df: a pandas dataframe with columns: preds, truths and speaker
+            result_df: a pandas dataframe with columns: preds, truths and speaker.
+            plot_name: name for the figure.
+            function: either mode or mean.
         """
         speakers = result_df.speaker.unique()
         pred = np.zeros(0)
         truth = np.zeros(0)
         for s in speakers:
             s_df = result_df[result_df.speaker == s]
             mode = s_df.pred.mode().iloc[-1]
@@ -124,42 +156,60 @@
 
     def _plot_confmat(self, truths, preds, plot_name, epoch):
         # print(truths)
         # print(preds)
         fig_dir = self.util.get_path("fig_dir")
         labels = glob_conf.labels
         fig = plt.figure()  # figsize=[5, 5]
-        uar = recall_score(truths, preds, average="macro")
-        acc = accuracy_score(truths, preds)
+        uar, (upper, lower) = evaluate_with_conf_int(
+            self.preds,
+            unweighted_average_recall,
+            self.truths,
+            num_bootstraps=1000,
+            alpha=5,
+        )
+        acc = accuracy(truths, preds)
         cm = confusion_matrix(
             truths, preds, normalize=None
         )  # normalize must be one of {'true', 'pred', 'all', None}
         if cm.shape[0] != len(labels):
             self.util.error(
                 f"mismatch between confmatrix dim ({cm.shape[0]}) and labels"
                 f" length ({len(labels)}: {labels})"
             )
+
         try:
             disp = ConfusionMatrixDisplay(
                 confusion_matrix=cm, display_labels=labels
             ).plot(cmap="Blues")
         except ValueError:
             disp = ConfusionMatrixDisplay(
                 confusion_matrix=cm,
                 display_labels=list(labels).remove("neutral"),
             ).plot(cmap="Blues")
 
         reg_res = ""
         if not self.is_classification:
-            reg_res = f", {self.MEASURE}: {self.result.test:.3f}"
+            reg_res = f"{self.result.test:.3f} {self.MEASURE}"
+
+        uar_str = str(int(uar * 1000) / 1000.0)[1:]
+        acc_str = str(int(acc * 1000) / 1000.0)[1:]
+        up_str = str(int(upper * 1000) / 1000.0)[1:]
+        low_str = str(int(lower * 1000) / 1000.0)[1:]
 
         if epoch != 0:
-            plt.title(f"Confusion Matrix, UAR: {uar:.3f}{reg_res}, Epoch: {epoch}")
+            plt.title(
+                f"Confusion Matrix, UAR: {uar_str} "
+                + f"(+-{up_str}/{low_str}), {reg_res}, Epoch: {epoch}"
+            )
         else:
-            plt.title(f"Confusion Matrix, UAR: {uar:.3f}{reg_res}")
+            plt.title(
+                f"Confusion Matrix, UAR: {uar_str} "
+                + f"(+-{up_str}/{low_str}) {reg_res}"
+            )
         img_path = f"{fig_dir}{plot_name}.{self.format}"
         plt.savefig(img_path)
         fig.clear()
         plt.close(fig)
         plt.savefig(img_path)
         plt.close(fig)
         glob_conf.report.add_item(
@@ -168,25 +218,26 @@
                 self.util.get_model_description(),
                 "Confusion matrix",
                 img_path,
             )
         )
 
         res_dir = self.util.get_path("res_dir")
-        uar = int(uar * 1000) / 1000.0
-        acc = int(acc * 1000) / 1000.0
-        rpt = f"epoch: {epoch}, UAR: {uar}, ACC: {acc}"
+        rpt = (
+            f"epoch: {epoch}, UAR: {uar_str}"
+            + f", (+-{up_str}/{low_str}), ACC: {acc_str}"
+        )
         # print(rpt)
         self.util.debug(rpt)
         file_name = f"{res_dir}{self.util.get_exp_name()}_conf.txt"
         with open(file_name, "w") as text_file:
             text_file.write(rpt)
 
     def print_results(self, epoch):
-        """Print all evaluation values to text file"""
+        """Print all evaluation values to text file."""
         res_dir = self.util.get_path("res_dir")
         file_name = f"{res_dir}{self.util.get_exp_name()}_{epoch}.txt"
         if self.util.exp_is_classification():
             labels = glob_conf.labels
             try:
                 rpt = classification_report(
                     self.truths,
@@ -275,23 +326,7 @@
         plt.plot(losses, "black", label="losses")
         plt.plot(losses_eval, "grey", label="losses_eval")
         plt.xlabel("epochs")
         plt.ylabel(f"{self.MEASURE}")
         plt.legend()
         plt.savefig(f"{fig_dir}{out_name}.{self.format}")
         plt.close()
-
-    @staticmethod
-    def ccc(ground_truth, prediction):
-        mean_gt = np.mean(ground_truth, 0)
-        mean_pred = np.mean(prediction, 0)
-        var_gt = np.var(ground_truth, 0)
-        var_pred = np.var(prediction, 0)
-        v_pred = prediction - mean_pred
-        v_gt = ground_truth - mean_gt
-        cor = sum(v_pred * v_gt) / (np.sqrt(sum(v_pred**2)) * np.sqrt(sum(v_gt**2)))
-        sd_gt = np.std(ground_truth)
-        sd_pred = np.std(prediction)
-        numerator = 2 * cor * sd_gt * sd_pred
-        denominator = var_gt + var_pred + (mean_gt - mean_pred) ** 2
-        ccc = numerator / denominator
-        return ccc
```

### Comparing `nkululeko-0.81.2/nkululeko/reporting/defines.py` & `nkululeko-0.81.3/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/reporting/latex_writer.py` & `nkululeko-0.81.3/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/reporting/report.py` & `nkululeko-0.81.3/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/reporting/report_item.py` & `nkululeko-0.81.3/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/resample.py` & `nkululeko-0.81.3/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/result.py` & `nkululeko-0.81.3/nkululeko/reporting/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,19 @@
         self.loss = loss
         self.loss_eval = loss_eval
         self.measure = measure
 
     def get_result(self):
         return self.test
 
+    def set_upper_lower(self, upper, lower):
+        """Set the upper and lower bound of confidence interval."""
+        self.upper = upper
+        self.lower = lower
+
     def get_test_result(self):
         return f"test: {self.test:.3f} {self.measure}"
 
     def to_string(self):
         return (
             f"test: {self.test} {self.measure}, train:"
             f" {self.train} {self.measure}, loss: {self.loss}, eval-loss: {self.loss_eval}"
```

### Comparing `nkululeko-0.81.2/nkululeko/runmanager.py` & `nkululeko-0.81.3/nkululeko/runmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # runmanager.py
 
-from nkululeko.reporter import Reporter
+from nkululeko.reporting.reporter import Reporter
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 from nkululeko.modelrunner import Modelrunner
 
 
 class Runmanager:
     """Class to manage the runs of the experiment (e.g. when results differ caused by random initialization)"""
```

### Comparing `nkululeko-0.81.2/nkululeko/scaler.py` & `nkululeko-0.81.3/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/segment.py` & `nkululeko-0.81.3/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.81.3/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.81.3/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/syllable_nuclei.py` & `nkululeko-0.81.3/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/test.py` & `nkululeko-0.81.3/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/test_predictor.py` & `nkululeko-0.81.3/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/utils/files.py` & `nkululeko-0.81.3/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/utils/stats.py` & `nkululeko-0.81.3/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko/utils/util.py` & `nkululeko-0.81.3/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.2/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.81.3/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.2
+Version: 0.81.3
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audeer
 Requires-Dist: audformat
 Requires-Dist: audinterface
 Requires-Dist: audiofile
 Requires-Dist: audiomentations
+Requires-Dist: audmetric
 Requires-Dist: audonnx
+Requires-Dist: confidence_intervals
 Requires-Dist: datasets
 Requires-Dist: imageio
 Requires-Dist: laion-clap
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: opensmile
 Requires-Dist: pandas
@@ -317,14 +319,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.3
+--------------
+* added confidence intervals to result reporting
+
 Version 0.81.2
 --------------
 * added a parselmouth.Praat error if pitch out of range
 * changed file path for demo_predictor
 
 Version 0.81.1
 --------------
```

### Comparing `nkululeko-0.81.2/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.81.3/nkululeko.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,17 +70,15 @@
 nkululeko/filter_data.py
 nkululeko/glob_conf.py
 nkululeko/modelrunner.py
 nkululeko/multidb.py
 nkululeko/nkululeko.py
 nkululeko/plots.py
 nkululeko/predict.py
-nkululeko/reporter.py
 nkululeko/resample.py
-nkululeko/result.py
 nkululeko/runmanager.py
 nkululeko/scaler.py
 nkululeko/segment.py
 nkululeko/syllable_nuclei.py
 nkululeko/test.py
 nkululeko/test_predictor.py
 nkululeko.egg-info/PKG-INFO
@@ -151,14 +149,16 @@
 nkululeko/models/model_xgb.py
 nkululeko/models/model_xgr.py
 nkululeko/reporting/__init__.py
 nkululeko/reporting/defines.py
 nkululeko/reporting/latex_writer.py
 nkululeko/reporting/report.py
 nkululeko/reporting/report_item.py
+nkululeko/reporting/reporter.py
+nkululeko/reporting/result.py
 nkululeko/segmenting/__init__.py
 nkululeko/segmenting/seg_inaspeechsegmenter.py
 nkululeko/segmenting/seg_silero.py
 nkululeko/utils/__init__.py
 nkululeko/utils/files.py
 nkululeko/utils/stats.py
 nkululeko/utils/util.py
```

### Comparing `nkululeko-0.81.2/setup.cfg` & `nkululeko-0.81.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 packages = find:
 install_requires = 
 	audeer
 	audformat
 	audinterface
 	audiofile
 	audiomentations
+	audmetric
 	audonnx
+	confidence_intervals
 	datasets
 	imageio
 	laion-clap
 	matplotlib
 	numpy
 	opensmile
 	pandas
```

### Comparing `nkululeko-0.81.2/venv/bin/activate_this.py` & `nkululeko-0.81.3/venv/bin/activate_this.py`

 * *Files identical despite different names*

