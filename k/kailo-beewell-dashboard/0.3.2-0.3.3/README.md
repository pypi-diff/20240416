# Comparing `tmp/kailo-beewell-dashboard-0.3.2.tar.gz` & `tmp/kailo-beewell-dashboard-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kailo-beewell-dashboard-0.3.2.tar", last modified: Fri Apr 12 14:53:47 2024, max compression
+gzip compressed data, was "kailo-beewell-dashboard-0.3.3.tar", last modified: Tue Apr 16 14:30:56 2024, max compression
```

## Comparing `kailo-beewell-dashboard-0.3.2.tar` & `kailo-beewell-dashboard-0.3.3.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/
--rw-rw-r--   0 amy       (1000) amy       (1000)     1070 2024-02-19 16:48:26.000000 kailo-beewell-dashboard-0.3.2/LICENSE
--rw-rw-r--   0 amy       (1000) amy       (1000)      158 2024-04-09 15:53:10.000000 kailo-beewell-dashboard-0.3.2/MANIFEST.in
--rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/PKG-INFO
--rw-rw-r--   0 amy       (1000) amy       (1000)     1590 2024-04-12 14:51:29.000000 kailo-beewell-dashboard-0.3.2/README.md
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.633476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/
--rw-rw-r--   0 amy       (1000) amy       (1000)      151 2024-04-12 14:50:52.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/__init__.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6619 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/about_page.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3939 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/authentication.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    15122 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6242 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts_text.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.637476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/
--rw-rw-r--   0 amy       (1000) amy       (1000)     1802 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/static_report_style.css
--rw-rw-r--   0 amy       (1000) amy       (1000)     3223 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/style.css
--rw-rw-r--   0 amy       (1000) amy       (1000)    25957 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/explore_results.py
--rw-rw-r--   0 amy       (1000) amy       (1000)      557 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/grammar.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.645476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/
--rw-rw-r--   0 amy       (1000) amy       (1000)    61702 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/beewell_map.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   185745 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/canva_people.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    48221 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/circle_divider.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    72751 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/dashboard_home_section.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    31928 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/devices.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   550917 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/discovery-looking-researching.jpg
--rw-rw-r--   0 amy       (1000) amy       (1000)   258283 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/home_image_3_transparent.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    92545 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    93979 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    88360 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_systems_adapted.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   564177 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/levelling-the-ground.jpg
--rw-rw-r--   0 amy       (1000) amy       (1000)    21040 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/northern_devon.png
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/
--rw-rw-r--   0 amy       (1000) amy       (1000)   180897 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   155419 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    23923 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choose_one.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   131754 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   106617 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   127520 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   102391 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   129719 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   104548 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   123168 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    98588 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    21352 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/happy.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   108174 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    82741 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   120585 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    95604 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   121744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    96996 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    16076 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/ok.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    19823 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/sad.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   121199 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    96276 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   156249 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   131030 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    85100 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/thinking.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   475730 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/young-person-journey.jpg
--rw-rw-r--   0 amy       (1000) amy       (1000)     1767 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     4418 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/import_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     1843 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/map.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2503 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/page_setup.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6853 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reshape_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14456 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/response_labels.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    13118 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reuse_text.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2723 2024-02-21 10:54:31.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/score_descriptions.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    13596 2024-04-12 14:37:13.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/static_report.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2297 2024-02-21 10:54:39.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/stylable_container.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    12744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/summary_rag.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     1077 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/switch_page_button.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14229 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_aggregate.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3553 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_demographic.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    19646 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_responses.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14885 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_scores.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3935 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/topic_labels.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     7968 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/who_took_part.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/
--rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 amy       (1000) amy       (1000)     3546 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)        1 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)      275 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/requires.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)      693 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/requirements.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)       38 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/setup.cfg
--rw-rw-r--   0 amy       (1000) amy       (1000)     1167 2024-04-09 15:51:48.000000 kailo-beewell-dashboard-0.3.2/setup.py
+drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.379128 kailo-beewell-dashboard-0.3.3/
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1070 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/LICENSE
+-rw-r--r--   0 ellengoddard   (501) staff       (20)      158 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/MANIFEST.in
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     2744 2024-04-16 14:30:56.378890 kailo-beewell-dashboard-0.3.3/PKG-INFO
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1631 2024-04-16 14:23:31.000000 kailo-beewell-dashboard-0.3.3/README.md
+drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.323499 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/
+-rw-r--r--   0 ellengoddard   (501) staff       (20)      169 2024-04-16 14:23:31.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/__init__.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     6521 2024-04-16 14:23:31.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/about_page.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     3939 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/authentication.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    15122 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     6242 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts_text.py
+drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.324589 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1802 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/static_report_style.css
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     3223 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/style.css
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    25957 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/explore_results.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)      557 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/grammar.py
+drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.341757 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    61702 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/beewell_map.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   185745 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/canva_people.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    48221 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/circle_divider.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    72751 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/dashboard_home_section.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    31928 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/devices.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   550917 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/discovery-looking-researching.jpg
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   258283 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/home_image_3_transparent.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    92545 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    93979 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    88360 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_systems_adapted.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   564177 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/levelling-the-ground.jpg
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    21040 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/northern_devon.png
+drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.377186 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   180897 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   155419 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    23923 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choose_one.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   131754 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   106617 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   127520 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   102391 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   129719 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   104548 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   123168 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    98588 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    21352 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/happy.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   108174 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    82741 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   120585 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    95604 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   121744 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    96996 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    16076 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/ok.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    19823 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/sad.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   121199 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    96276 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   156249 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   131030 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things_crop.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    85100 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/thinking.png
+-rw-r--r--   0 ellengoddard   (501) staff       (20)   475730 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/young-person-journey.jpg
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1767 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     4418 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/import_data.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1843 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/map.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     2503 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/page_setup.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     6853 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reshape_data.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    14456 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/response_labels.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    13118 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reuse_text.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     2723 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/score_descriptions.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    13596 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/static_report.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     2297 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/stylable_container.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    12744 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/summary_rag.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1077 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/switch_page_button.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    14229 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_aggregate.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     3553 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_demographic.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    19646 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_responses.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)    14885 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_scores.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     3935 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/topic_labels.py
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     7968 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/who_took_part.py
+drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.378570 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     2744 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     3561 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 ellengoddard   (501) staff       (20)        1 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 ellengoddard   (501) staff       (20)      308 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/requires.txt
+-rw-r--r--   0 ellengoddard   (501) staff       (20)       24 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 ellengoddard   (501) staff       (20)      675 2024-04-16 14:30:27.000000 kailo-beewell-dashboard-0.3.3/pyproject.toml
+-rw-r--r--   0 ellengoddard   (501) staff       (20)      728 2024-04-16 14:30:05.000000 kailo-beewell-dashboard-0.3.3/requirements.txt
+-rw-r--r--   0 ellengoddard   (501) staff       (20)       38 2024-04-16 14:30:56.379181 kailo-beewell-dashboard-0.3.3/setup.cfg
+-rw-r--r--   0 ellengoddard   (501) staff       (20)     1167 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/setup.py
```

### Comparing `kailo-beewell-dashboard-0.3.2/LICENSE` & `kailo-beewell-dashboard-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/PKG-INFO` & `kailo-beewell-dashboard-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kailo-beewell-dashboard
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tools to support creation of #BeeWell survey dashboards for Kailo
 Home-page: https://github.com/kailo-beewell/kailo_beewell_dashboard_package
 Author: Amy Heather
 Author-email: a.heather2@exeter.ac.uk
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,20 @@
 Requires-Dist: streamlit>=1.32.2
 Requires-Dist: twine==5.0.0
 Requires-Dist: sphinx==7.2.6
 Requires-Dist: sphinx-rtd-theme==2.0.0
 Requires-Dist: myst-parser==2.0.0
 Requires-Dist: sphinx-autoapi==3.0.0
 Requires-Dist: matplotlib==3.8.3
+Requires-Dist: setuptools==69.1.1
+Requires-Dist: wheel==0.42.0
 
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.2-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.2/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.3-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.3/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -50,19 +52,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.2). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. and Goddard, Ellen. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.3). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
 @software{kailo-beewell-dashboard,
-  author = {Heather, Amy},
+  author = {Heather, Amy. and Goddard, Ellen.},
   title = {kailo-beewell-dashboard},
-  date = {2024-04-12},
-  version = {0.3.2},
+  date = {2024-04-16},
+  version = {0.3.3},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.3.2/README.md` & `kailo-beewell-dashboard-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.2-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.2/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.3-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.3/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -19,19 +19,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.2). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. and Goddard, Ellen. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.3). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
 @software{kailo-beewell-dashboard,
-  author = {Heather, Amy},
+  author = {Heather, Amy. and Goddard, Ellen.},
   title = {kailo-beewell-dashboard},
-  date = {2024-04-12},
-  version = {0.3.2},
+  date = {2024-04-16},
+  version = {0.3.3},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/about_page.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/about_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,157 @@
-'''
+"""
 Helper functions to produce the About page for each version of the dashboard
-'''
+"""
+
 from kailo_beewell_dashboard.images import get_image_path
 from kailo_beewell_dashboard.reuse_text import reuse_text
 from kailo_beewell_dashboard.stylable_container import header_container
 import streamlit as st
 
 
 def symbol_content():
-    '''
+    """
     Descriptions content of symbol survey using combination of text and images
     (hence provided as function, rather than using reuse_text like all the
     other About page sections)
-    '''
-    st.markdown('''The survey contained ten questions which use the Widgit
-                symbol system. These were:''')
+    """
+    st.markdown("""The survey contained ten questions which use the Widgit
+                symbol system. These were:""")
     # Add the images (they are the same as those used for the survey, but
     # cropped to height of 340 to remove the 'choose one' from each)
-    st.image(get_image_path('symbol_survey/family_crop.png'))
-    st.image(get_image_path('symbol_survey/home_crop.png'))
-    st.image(get_image_path('symbol_survey/friends_crop.png'))
-    st.image(get_image_path('symbol_survey/choice_crop.png'))
-    st.image(get_image_path('symbol_survey/things_crop.png'))
-    st.image(get_image_path('symbol_survey/health_crop.png'))
-    st.image(get_image_path('symbol_survey/future_crop.png'))
-    st.image(get_image_path('symbol_survey/school_crop.png'))
-    st.image(get_image_path('symbol_survey/free_time_crop.png'))
-    st.image(get_image_path('symbol_survey/life_crop.png'))
-    st.markdown('For each questions, pupils had three response options:')
-    st.image(get_image_path('symbol_survey/choose_one.png'))
+    st.image(get_image_path("symbol_survey/family_crop.png"))
+    st.image(get_image_path("symbol_survey/home_crop.png"))
+    st.image(get_image_path("symbol_survey/friends_crop.png"))
+    st.image(get_image_path("symbol_survey/choice_crop.png"))
+    st.image(get_image_path("symbol_survey/things_crop.png"))
+    st.image(get_image_path("symbol_survey/health_crop.png"))
+    st.image(get_image_path("symbol_survey/future_crop.png"))
+    st.image(get_image_path("symbol_survey/school_crop.png"))
+    st.image(get_image_path("symbol_survey/free_time_crop.png"))
+    st.image(get_image_path("symbol_survey/life_crop.png"))
+    st.markdown("For each questions, pupils had three response options:")
+    st.image(get_image_path("symbol_survey/choose_one.png"))
     cols = st.columns(3)
     with cols[0]:
-        st.image(get_image_path('symbol_survey/happy.png'))
+        st.image(get_image_path("symbol_survey/happy.png"))
     with cols[1]:
-        st.image(get_image_path('symbol_survey/ok.png'))
+        st.image(get_image_path("symbol_survey/ok.png"))
     with cols[2]:
-        st.image(get_image_path('symbol_survey/sad.png'))
+        st.image(get_image_path("symbol_survey/sad.png"))
 
 
 def create_about_page(dashboard_type):
-    '''
+    """
     Creates the 'About' page on the streamlit dashboard
 
     Parameters
     ----------
     dashboard_type : string
         Specifies whether this is for 'standard' or 'symbol' school
         dashboard, or for the 'public' area-level dashboard
-    '''
+    """
     # Page title
-    st.title('About')
+    st.title("About")
+    st.markdown("Test Ellen")
 
     # Introduction
-    st.markdown(reuse_text['about_intro'])
+    st.markdown(reuse_text["about_intro"])
 
     # Expand toggle
-    expand = st.toggle('Toggle to expand all the boxes below', value=False)
+    expand = st.toggle("Toggle to expand all the boxes below", value=False)
 
     # FAQs about Kailo
-    header_container('green_container', '🌿 Kailo', '#D9ECCA')
+    header_container("green_container", "🌿 Kailo", "#D9ECCA")
 
     # Description of the Kailo project
-    with st.expander('What is Kailo?', expanded=expand):
-        st.markdown(reuse_text['kailo'])
-        st.image(get_image_path('kailo_systems_adapted.png'),
-                 use_column_width=True)
+    with st.expander("What is Kailo?", expanded=expand):
+        st.markdown(reuse_text["kailo"])
+        st.image(get_image_path("kailo_systems_adapted.png"), use_column_width=True)
 
     # FAQs about the #BeeWell survey
-    header_container('orange_container', '🐝 The #BeeWell survey', '#F7DCC8')
+    header_container("orange_container", "🐝 The #BeeWell survey", "#F7DCC8")
 
     # Survey sample
-    with st.expander('Who took part in the #BeeWell survey in Devon?',
-                     expanded=expand):
-        if dashboard_type == 'symbol':
-            st.markdown(reuse_text['sample_symbol'])
+    with st.expander("Who took part in the #BeeWell survey in Devon?", expanded=expand):
+        if dashboard_type == "symbol":
+            st.markdown(reuse_text["sample_symbol"])
         else:
-            st.markdown(reuse_text['sample'])
-        st.image(get_image_path('northern_devon.png'), use_column_width=True)
+            st.markdown(reuse_text["sample"])
+        st.image(get_image_path("northern_devon.png"), use_column_width=True)
 
     # Survey content, and design of the survey
-    if dashboard_type == 'public':
+    if dashboard_type == "public":
         # Public dashboard - survey content
-        with st.expander('What topics did the standard survey cover?',
-                         expanded=expand):
-            st.markdown(reuse_text['standard_content'])
-        with st.expander('What topics did the symbol survey cover?',
-                         expanded=expand):
+        with st.expander("What topics did the standard survey cover?", expanded=expand):
+            st.markdown(reuse_text["standard_content"])
+        with st.expander("What topics did the symbol survey cover?", expanded=expand):
             symbol_content()
         # Public dashboard - survey design
-        with st.expander('How was the standard survey designed?',
-                         expanded=expand):
-            st.markdown(reuse_text['standard_design'])
-            st.image(get_image_path('canva_people.png'), use_column_width=True)
-        with st.expander('How was the symbol survey designed?',
-                         expanded=expand):
-            st.markdown(reuse_text['symbol_design'])
+        with st.expander("How was the standard survey designed?", expanded=expand):
+            st.markdown(reuse_text["standard_design"])
+            st.image(get_image_path("canva_people.png"), use_column_width=True)
+        with st.expander("How was the symbol survey designed?", expanded=expand):
+            st.markdown(reuse_text["symbol_design"])
     else:
         # School dashboards - survey content
-        with st.expander('What topics did the survey cover?', expanded=expand):
-            if dashboard_type == 'standard':
-                st.markdown(reuse_text['standard_content'])
-            elif dashboard_type == 'symbol':
+        with st.expander("What topics did the survey cover?", expanded=expand):
+            if dashboard_type == "standard":
+                st.markdown(reuse_text["standard_content"])
+            elif dashboard_type == "symbol":
                 symbol_content()
         # School dashboards - survey design
-        with st.expander('How was the survey designed?', expanded=expand):
-            if dashboard_type == 'standard':
-                st.markdown(reuse_text['standard_design'])
-            elif dashboard_type == 'symbol':
-                st.markdown(reuse_text['symbol_design'])
-            st.image(get_image_path('canva_people.png'), use_column_width=True)
+        with st.expander("How was the survey designed?", expanded=expand):
+            if dashboard_type == "standard":
+                st.markdown(reuse_text["standard_design"])
+            elif dashboard_type == "symbol":
+                st.markdown(reuse_text["symbol_design"])
+            st.image(get_image_path("canva_people.png"), use_column_width=True)
 
     # Other #BeeWell sites
-    with st.expander('Where else have these surveys been completed?',
-                     expanded=expand):
-        st.markdown(reuse_text['other_beewell_sites'])
-        st.image(get_image_path('beewell_map.png'), use_column_width=True)
+    with st.expander("Where else have these surveys been completed?", expanded=expand):
+        st.markdown(reuse_text["other_beewell_sites"])
+        st.image(get_image_path("beewell_map.png"), use_column_width=True)
 
     # FAQs about the dashboard
-    header_container('blue_container', '📊 Dashboard', '#D0C9FF')
+    header_container("blue_container", "📊 Dashboard", "#D0C9FF")
 
     # Data used to create the dashboard
-    with st.expander('What data has been used in this dashboard?',
-                     expanded=expand):
-        if dashboard_type == 'standard':
-            st.markdown(reuse_text['standard_data'])
-        elif dashboard_type == 'symbol':
-            st.markdown(reuse_text['symbol_data'])
-        elif dashboard_type == 'public':
-            st.markdown(reuse_text['public_data'])
+    with st.expander("What data has been used in this dashboard?", expanded=expand):
+        if dashboard_type == "standard":
+            st.markdown(reuse_text["standard_data"])
+        elif dashboard_type == "symbol":
+            st.markdown(reuse_text["symbol_data"])
+        elif dashboard_type == "public":
+            st.markdown(reuse_text["public_data"])
 
     # How to use the results
-    with st.expander('How should we use these results?', expanded=expand):
-        st.markdown(reuse_text['how_to_use_results'])
-        st.image(get_image_path('thinking.png'), use_column_width=True)
+    with st.expander("How should we use these results?", expanded=expand):
+        st.markdown(reuse_text["how_to_use_results"])
+        st.image(get_image_path("thinking.png"), use_column_width=True)
 
     # Accessing the dashboard on different devices
-    with st.expander('Can I access this dashboard on different devices?',
-                     expanded=expand):
-        st.markdown(reuse_text['view_devices'])
-        st.image(get_image_path('devices.png'), use_column_width=True)
+    with st.expander(
+        "Can I access this dashboard on different devices?", expanded=expand
+    ):
+        st.markdown(reuse_text["view_devices"])
+        st.image(get_image_path("devices.png"), use_column_width=True)
 
     # Support with dashboards (for school dashboards only)
-    if dashboard_type != 'public':
-        with st.expander('''
+    if dashboard_type != "public":
+        with st.expander(
+            """
 Will there be support available for interpreting and actioning on the dashboard
-results?''', expanded=expand):
-            st.markdown(reuse_text['dashboard_support'])
+results?""",
+            expanded=expand,
+        ):
+            st.markdown(reuse_text["dashboard_support"])
 
     # FAQs about wellbeing
-    header_container('yellow_container', '😌 Wellbeing', '#FFF3B3')
+    header_container("yellow_container", "😌 Wellbeing", "#FFF3B3")
 
     # What do we already know?
-    with st.expander('''
-What do we already know about young people's wellbeing?''', expanded=expand):
-        st.markdown(reuse_text['wellbeing_context'], unsafe_allow_html=True)
+    with st.expander(
+        """
+What do we already know about young people's wellbeing?""",
+        expanded=expand,
+    ):
+        st.markdown(reuse_text["wellbeing_context"], unsafe_allow_html=True)
```

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/authentication.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/authentication.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts_text.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts_text.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/static_report_style.css` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/static_report_style.css`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/style.css` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/style.css`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/explore_results.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/explore_results.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/grammar.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/grammar.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/beewell_map.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/beewell_map.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/canva_people.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/canva_people.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/circle_divider.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/circle_divider.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/dashboard_home_section.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/dashboard_home_section.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/devices.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/devices.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/discovery-looking-researching.jpg` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/discovery-looking-researching.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/home_image_3_transparent.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/home_image_3_transparent.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_systems_adapted.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_systems_adapted.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/levelling-the-ground.jpg` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/levelling-the-ground.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/northern_devon.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/northern_devon.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choose_one.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choose_one.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/happy.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/happy.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/ok.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/ok.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/sad.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/sad.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things_crop.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/thinking.png` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/thinking.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/young-person-journey.jpg` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/young-person-journey.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/import_data.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/import_data.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/map.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/map.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/page_setup.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/page_setup.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reshape_data.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reshape_data.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/response_labels.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/response_labels.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reuse_text.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reuse_text.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/score_descriptions.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/score_descriptions.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/static_report.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/static_report.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/stylable_container.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/stylable_container.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/summary_rag.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/summary_rag.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/switch_page_button.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/switch_page_button.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_aggregate.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_aggregate.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_demographic.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_demographic.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_responses.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_responses.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_scores.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_scores.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/topic_labels.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/topic_labels.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/who_took_part.py` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/who_took_part.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/PKG-INFO` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kailo-beewell-dashboard
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tools to support creation of #BeeWell survey dashboards for Kailo
 Home-page: https://github.com/kailo-beewell/kailo_beewell_dashboard_package
 Author: Amy Heather
 Author-email: a.heather2@exeter.ac.uk
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,20 @@
 Requires-Dist: streamlit>=1.32.2
 Requires-Dist: twine==5.0.0
 Requires-Dist: sphinx==7.2.6
 Requires-Dist: sphinx-rtd-theme==2.0.0
 Requires-Dist: myst-parser==2.0.0
 Requires-Dist: sphinx-autoapi==3.0.0
 Requires-Dist: matplotlib==3.8.3
+Requires-Dist: setuptools==69.1.1
+Requires-Dist: wheel==0.42.0
 
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.2-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.2/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.3-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.3/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -50,19 +52,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.2). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. and Goddard, Ellen. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.3). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
 @software{kailo-beewell-dashboard,
-  author = {Heather, Amy},
+  author = {Heather, Amy. and Goddard, Ellen.},
   title = {kailo-beewell-dashboard},
-  date = {2024-04-12},
-  version = {0.3.2},
+  date = {2024-04-16},
+  version = {0.3.3},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/SOURCES.txt` & `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 kailo_beewell_dashboard/__init__.py
 kailo_beewell_dashboard/about_page.py
 kailo_beewell_dashboard/authentication.py
 kailo_beewell_dashboard/bar_charts.py
 kailo_beewell_dashboard/bar_charts_text.py
```

### Comparing `kailo-beewell-dashboard-0.3.2/requirements.txt` & `kailo-beewell-dashboard-0.3.3/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -35,8 +35,11 @@
 # To produce readthedocs
 sphinx==7.2.6
 sphinx-rtd-theme==2.0.0
 myst-parser==2.0.0
 sphinx-autoapi==3.0.0
 
 # To generate previews of figures in notebooks
-matplotlib==3.8.3
+matplotlib==3.8.3
+
+setuptools==69.1.1
+wheel==0.42.0
```

### Comparing `kailo-beewell-dashboard-0.3.2/setup.py` & `kailo-beewell-dashboard-0.3.3/setup.py`

 * *Files identical despite different names*

