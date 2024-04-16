# Comparing `tmp/astro-p3-1.2.8.tar.gz` & `tmp/astro-p3-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-p3-1.2.8.tar", last modified: Fri Nov 10 14:01:55 2023, max compression
+gzip compressed data, was "astro-p3-1.2.9.tar", last modified: Sat Dec  2 17:52:57 2023, max compression
```

## Comparing `astro-p3-1.2.8.tar` & `astro-p3-1.2.9.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.972900 astro-p3-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.860898 astro-p3-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.868898 astro-p3-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-10 14:01:32.000000 astro-p3-1.2.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-10 14:01:32.000000 astro-p3-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-11-10 14:01:32.000000 astro-p3-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-10 14:01:32.000000 astro-p3-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-11-10 14:01:55.972900 astro-p3-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-11-10 14:01:32.000000 astro-p3-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.868898 astro-p3-1.2.8/astro_p3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-11-10 14:01:55.000000 astro-p3-1.2.8/astro_p3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2023-11-10 14:01:55.000000 astro-p3-1.2.8/astro_p3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 14:01:55.000000 astro-p3-1.2.8/astro_p3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 14:01:55.000000 astro-p3-1.2.8/astro_p3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-10 14:01:55.000000 astro-p3-1.2.8/astro_p3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.868898 astro-p3-1.2.8/p3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-10 14:01:55.000000 astro-p3-1.2.8/p3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.872898 astro-p3-1.2.8/p3/aoSystem/
--rw-r--r--   0 runner    (1001) docker     (127)    39904 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/FourierUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.872898 astro-p3-1.2.8/p3/aoSystem/_txtFile/
--rw-r--r--   0 runner    (1001) docker     (127)    39085 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/_txtFile/ELT_segmentVertices.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/_txtFile/Keck_segmentVertices.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/anisoplanatismModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    36805 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/aoSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/createSegmentedModes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.868898 astro-p3-1.2.8/p3/aoSystem/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.880898 astro-p3-1.2.8/p3/aoSystem/data/ELT_CALIBRATION/
--rw-r--r--   0 runner    (1001) docker     (127)  4331520 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits
--rw-r--r--   0 runner    (1001) docker     (127)   938880 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.880898 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.880898 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidActuatorMap.txt
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidSubapMap.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.928899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/
--rw-r--r--   0 runner    (1001) docker     (127) 11522880 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits
--rw-r--r--   0 runner    (1001) docker     (127)  2882880 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits
--rw-r--r--   0 runner    (1001) docker     (127) 11522880 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits
--rw-r--r--   0 runner    (1001) docker     (127) 11845440 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits
--rw-r--r--   0 runner    (1001) docker     (127)   325440 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.868898 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.932899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.932899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat
--rw-r--r--   0 runner    (1001) docker     (127)    26149 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.932899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat
--rw-r--r--   0 runner    (1001) docker     (127)    25122 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.932899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat
--rw-r--r--   0 runner    (1001) docker     (127)    24174 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.932899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat
--rw-r--r--   0 runner    (1001) docker     (127)    27413 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat
--rw-r--r--   0 runner    (1001) docker     (127)    24174 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.940899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/
--rw-r--r--   0 runner    (1001) docker     (127)    45636 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat
--rw-r--r--   0 runner    (1001) docker     (127)    31637 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat
--rw-r--r--   0 runner    (1001) docker     (127)    51146 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat
--rw-r--r--   0 runner    (1001) docker     (127)    42642 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat
--rw-r--r--   0 runner    (1001) docker     (127)    45125 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat
--rw-r--r--   0 runner    (1001) docker     (127)    60065 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat
--rw-r--r--   0 runner    (1001) docker     (127)    54054 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat
--rw-r--r--   0 runner    (1001) docker     (127)    60374 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    58102 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat
--rw-r--r--   0 runner    (1001) docker     (127)    61576 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat
--rw-r--r--   0 runner    (1001) docker     (127)    41888 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat
--rw-r--r--   0 runner    (1001) docker     (127)  2079744 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls
--rw-r--r--   0 runner    (1001) docker     (127)   128912 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.940899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/
--rw-r--r--   0 runner    (1001) docker     (127)    77760 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits
--rw-r--r--   0 runner    (1001) docker     (127)   463680 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits
--rw-r--r--   0 runner    (1001) docker     (127)   463680 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.944899 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1330560 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.868898 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.948900 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/
--rw-r--r--   0 runner    (1001) docker     (127)   152640 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits
--rw-r--r--   0 runner    (1001) docker     (127)   593280 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits
--rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits
--rw-r--r--   0 runner    (1001) docker     (127)   429120 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits
--rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits
--rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits
--rw-r--r--   0 runner    (1001) docker     (127)   429120 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits
--rw-r--r--   0 runner    (1001) docker     (127)    60480 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits
--rw-r--r--   0 runner    (1001) docker     (127)  2102400 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.952900 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/
--rw-r--r--   0 runner    (1001) docker     (127)  9835200 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/defineAoSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/deformableMirror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    58621 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/fourierModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/frequencyDomain.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/optics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.964900 astro-p3-1.2.8/p3/aoSystem/parFiles/
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/HarmoniLTAO.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/HarmoniSCAO.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/MavisMCAO.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/MosaicGLAO.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/eris.ini
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/irdis.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/nirc2.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/nirc2_monochromatic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/parFiles/template.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21580 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/pupil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/rtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/spiders.py
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.964900 astro-p3-1.2.8/p3/aoSystem/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/testing/tests_aoSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/testing/tests_tiptop_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/aoSystem/zernike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.968900 astro-p3-1.2.8/p3/deepLoop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/dataBaseVerification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10414 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/dataGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/dataGeneratorBatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    24969 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/deepLoopPerformance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/deepLoopPerformanceBatch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      628 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/jobGenerate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      828 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/jobPerformance.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/deepLoop/recover_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.968900 astro-p3-1.2.8/p3/psfFitting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfFitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfFitting/confidenceInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)    30451 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfFitting/fittingUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfFitting/imageModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10944 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfFitting/psfFitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.968900 astro-p3-1.2.8/p3/psfao21/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfao21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfao21/psfao21.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.968900 astro-p3-1.2.8/p3/psfr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14707 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfr/psfR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/psfr/psfrUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.968900 astro-p3-1.2.8/p3/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/configFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/keckUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/massdimm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8108 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/sphereUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21961 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/systemDiagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/telemetryKASP.py
--rw-r--r--   0 runner    (1001) docker     (127)    19117 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/telemetry/telemetryKeck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:55.968900 astro-p3-1.2.8/p3/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2023-11-10 14:01:32.000000 astro-p3-1.2.8/p3/testing/tests_p3.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-11-10 14:01:32.000000 astro-p3-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 14:01:55.972900 astro-p3-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.752545 astro-p3-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.648545 astro-p3-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.652545 astro-p3-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-02 17:52:44.000000 astro-p3-1.2.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-02 17:52:44.000000 astro-p3-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-12-02 17:52:44.000000 astro-p3-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-02 17:52:44.000000 astro-p3-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-12-02 17:52:57.752545 astro-p3-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-02 17:52:44.000000 astro-p3-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/astro_p3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-12-02 17:52:57.000000 astro-p3-1.2.9/astro_p3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2023-12-02 17:52:57.000000 astro-p3-1.2.9/astro_p3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 17:52:57.000000 astro-p3-1.2.9/astro_p3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 17:52:57.000000 astro-p3-1.2.9/astro_p3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-02 17:52:57.000000 astro-p3-1.2.9/astro_p3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.652545 astro-p3-1.2.9/p3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-02 17:52:57.000000 astro-p3-1.2.9/p3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.656545 astro-p3-1.2.9/p3/aoSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)    39905 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/FourierUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.656545 astro-p3-1.2.9/p3/aoSystem/_txtFile/
+-rw-r--r--   0 runner    (1001) docker     (127)    39085 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/_txtFile/ELT_segmentVertices.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/_txtFile/Keck_segmentVertices.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/anisoplanatismModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36832 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/aoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/createSegmentedModes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.648545 astro-p3-1.2.9/p3/aoSystem/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.660545 astro-p3-1.2.9/p3/aoSystem/data/ELT_CALIBRATION/
+-rw-r--r--   0 runner    (1001) docker     (127)  4331520 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   938880 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.664545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.664545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidActuatorMap.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECKAO/keckValidSubapMap.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.712545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/
+-rw-r--r--   0 runner    (1001) docker     (127) 11522880 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  2882880 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits
+-rw-r--r--   0 runner    (1001) docker     (127) 11522880 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits
+-rw-r--r--   0 runner    (1001) docker     (127) 11845440 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   325440 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.648545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.712545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.712545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    26149 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.712545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    25122 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.712545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24174 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.712545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    27413 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24174 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.720545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/
+-rw-r--r--   0 runner    (1001) docker     (127)    45636 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    31637 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    51146 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    42642 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    45125 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    60065 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    54054 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    60374 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    58102 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    61576 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    41888 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  2079744 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls
+-rw-r--r--   0 runner    (1001) docker     (127)   128912 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.720545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/
+-rw-r--r--   0 runner    (1001) docker     (127)    77760 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   463680 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   463680 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.724545 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1330560 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.648545 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.728546 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/
+-rw-r--r--   0 runner    (1001) docker     (127)   152640 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   593280 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   429120 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   429120 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    60480 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  2102400 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.732545 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/
+-rw-r--r--   0 runner    (1001) docker     (127)  9835200 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/defineAoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/deformableMirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58455 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/fourierModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/frequencyDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/optics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.744546 astro-p3-1.2.9/p3/aoSystem/parFiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/HarmoniLTAO.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/HarmoniSCAO.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/MavisMCAO.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/MosaicGLAO.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/eris.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/irdis.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/nirc2.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/nirc2_monochromatic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/parFiles/template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21580 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/pupil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/rtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/spiders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.744546 astro-p3-1.2.9/p3/aoSystem/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/testing/tests_aoSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/testing/tests_tiptop_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/aoSystem/zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/p3/deepLoop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/dataBaseVerification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/dataGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/dataGeneratorBatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24969 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/deepLoopPerformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/deepLoopPerformanceBatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      628 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/jobGenerate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      828 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/jobPerformance.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/deepLoop/recover_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/p3/psfFitting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfFitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfFitting/confidenceInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30451 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfFitting/fittingUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfFitting/imageModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfFitting/psfFitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/p3/psfao21/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfao21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfao21/psfao21.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/p3/psfr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14707 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfr/psfR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/psfr/psfrUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/p3/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/configFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/keckUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13812 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/massdimm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/sphereUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21961 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/systemDiagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/telemetryKASP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19117 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/telemetry/telemetryKeck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:57.748546 astro-p3-1.2.9/p3/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15103 2023-12-02 17:52:44.000000 astro-p3-1.2.9/p3/testing/tests_p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-02 17:52:44.000000 astro-p3-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 17:52:57.752545 astro-p3-1.2.9/setup.cfg
```

### Comparing `astro-p3-1.2.8/.github/workflows/publish.yml` & `astro-p3-1.2.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/LICENSE` & `astro-p3-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/PKG-INFO` & `astro-p3-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-p3
-Version: 1.2.8
+Version: 1.2.9
 Author: Olivier Beltramo-Martin
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/astro-tiptop/P3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy
```

### Comparing `astro-p3-1.2.8/README.md` & `astro-p3-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/astro_p3.egg-info/PKG-INFO` & `astro-p3-1.2.9/astro_p3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-p3
-Version: 1.2.8
+Version: 1.2.9
 Author: Olivier Beltramo-Martin
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/astro-tiptop/P3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy
```

### Comparing `astro-p3-1.2.8/astro_p3.egg-info/SOURCES.txt` & `astro-p3-1.2.9/astro_p3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/FourierUtils.py` & `astro-p3-1.2.9/p3/aoSystem/FourierUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1065,15 +1065,15 @@
         psfDL   = telescopePsf(pupil,samp)
         psfDL   = interpolateSupport(psfDL,nnp.array(psfDL.shape))
         psf[psf<0]  =0 
         SR      = psf.max()/psfDL.max() * psfDL.sum()/psf.sum()
     else:
         raise ValueError("Method must be 'otf' or 'max'")
         
-    return np.round(SR,nR)
+    return nnp.round(SR,nR)
 
 #%% Data treatment
     
 def eqLayers(Cn2, altitudes, nEqLayers, power=5/3):
     '''
              Cn2         ::  The input Cn2 profile (vector)
              altitudes   ::  The input altitudes (vector)
```

### Comparing `astro-p3-1.2.8/p3/aoSystem/_txtFile/ELT_segmentVertices.txt` & `astro-p3-1.2.9/p3/aoSystem/_txtFile/ELT_segmentVertices.txt`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/anisoplanatismModel.py` & `astro-p3-1.2.9/p3/aoSystem/anisoplanatismModel.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/aoSystem.py` & `astro-p3-1.2.9/p3/aoSystem/aoSystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,15 +905,15 @@
             
             self.wfe['TT Noise']     = rad2nm(np.mean(varNoise))
         else:
             self.wfe['TT Servo-lag'] = 0
             self.wfe['TT Noise'] = 0
         
         # Focal anisoplanatism
-        if self.lgs:
+        if self.lgs and self.lgs.height[0] > 0:
             self.wfe['Focal anisoplanatism'] = anisoplanatismModel.focal_anisoplanatism_variance(self.tel,self.atm,self.lgs)
         else:
             self.wfe['Focal anisoplanatism'] = 0
             
         # TO be added : angular anisoplanatisms
            
         self.wfe['Total'] = np.sqrt(self.wfe['DM fitting']**2 + self.wfe['WFS aliasing']**2\
```

### Comparing `astro-p3-1.2.8/p3/aoSystem/atmosphere.py` & `astro-p3-1.2.9/p3/aoSystem/atmosphere.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/createSegmentedModes.py` & `astro-p3-1.2.9/p3/aoSystem/createSegmentedModes.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits` & `astro-p3-1.2.9/p3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits` & `astro-p3-1.2.9/p3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_9modes_lr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_modes_200px_all_lr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_piston_waffle_modes_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/KECK_STAT/keck_waffle_200px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130203/20130203.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20130914/20130914.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170314/20170314.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20170315/2017031520170315.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM/20201202/20201202.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.dimm.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.mass.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/MASSDIMM20170315.masspro.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Brgamma.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/FeII.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/H.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Hcont.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/J.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/K.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kcont.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Kp.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ks.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Lp.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/Ms.dat`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/filter_passbands.xls`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_FILTERS/wfc3_ir_F125W.dat.html`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_largeHex_272px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open2_240px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_MASK/keck_pupil_open_240px.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_11March2020_PD3.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_14March2017_PD2.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD1.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_15March2017_PD2.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Aug_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Feb_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/NCPA_Keck_Sept_2013.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/phase_maps_corr.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits` & `astro-p3-1.2.9/p3/aoSystem/data/KECK_CALIBRATION/NIRC2_STAT/staticMapsInFov_2017_positions.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ALC2LyotStop_measured.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/APO1Apodizer_measured_All.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil160.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupil320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3160noLB.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/ut4pupilM3320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vlt_pup_240.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_PUPIL/vltpupil.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits` & `astro-p3-1.2.9/p3/aoSystem/data/VLT_CALIBRATION/VLT_STAT/LWEMODES_320.fits`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/defineAoSystem.py` & `astro-p3-1.2.9/p3/aoSystem/defineAoSystem.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/deformableMirror.py` & `astro-p3-1.2.9/p3/aoSystem/deformableMirror.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/detector.py` & `astro-p3-1.2.9/p3/aoSystem/detector.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/fourierModel.py` & `astro-p3-1.2.9/p3/aoSystem/fourierModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -864,21 +864,15 @@
         ratio = (h_laser-h)/h_laser
         nCn2 = len(h)
         freqs = self.freq.kx_[int(np.ceil(self.freq.nOtf/2)-1):,0]
         if freqs[0] < 0:
             freqs = freqs[1:]
         nf0 = len(freqs)
         coeff = np.zeros((nf0,nCn2))
-        
-        if self.verbose:
-            print('h_laser',h_laser)
-            print('h',h)
-            print('nf0',nf0)
-            print('ratio',ratio)
-        
+
         for j in range(nCn2):
             for i in range(nf0):
                 if freqs[i]*ratio[j] > self.freq.kc_:
                     coeff[i,j] = 0.0
                 else:
                     if freqs[i] < 1e-5:
                         coeff[i,j] = 0
```

### Comparing `astro-p3-1.2.8/p3/aoSystem/frequencyDomain.py` & `astro-p3-1.2.9/p3/aoSystem/frequencyDomain.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/optics.py` & `astro-p3-1.2.9/p3/aoSystem/optics.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/HarmoniLTAO.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/HarmoniLTAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/HarmoniSCAO.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/HarmoniSCAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/KECKII_NIRC2_20130801_12_00_19.254.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/MavisMCAO.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/MavisMCAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/MosaicGLAO.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/MosaicGLAO.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/eris.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/eris.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/irdis.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/irdis.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/nirc2.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/nirc2.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/nirc2_monochromatic.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/nirc2_monochromatic.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/parFiles/template.ini` & `astro-p3-1.2.9/p3/aoSystem/parFiles/template.ini`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/processing.py` & `astro-p3-1.2.9/p3/aoSystem/processing.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/pupil.py` & `astro-p3-1.2.9/p3/aoSystem/pupil.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/rtc.py` & `astro-p3-1.2.9/p3/aoSystem/rtc.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/segment.py` & `astro-p3-1.2.9/p3/aoSystem/segment.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/sensor.py` & `astro-p3-1.2.9/p3/aoSystem/sensor.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/source.py` & `astro-p3-1.2.9/p3/aoSystem/source.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/spiders.py` & `astro-p3-1.2.9/p3/aoSystem/spiders.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/telescope.py` & `astro-p3-1.2.9/p3/aoSystem/telescope.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/testing/tests_aoSystem.py` & `astro-p3-1.2.9/p3/aoSystem/testing/tests_aoSystem.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/testing/tests_tiptop_compatibility.py` & `astro-p3-1.2.9/p3/aoSystem/testing/tests_tiptop_compatibility.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/aoSystem/zernike.py` & `astro-p3-1.2.9/p3/aoSystem/zernike.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/dataBaseVerification.py` & `astro-p3-1.2.9/p3/deepLoop/dataBaseVerification.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/dataGenerator.py` & `astro-p3-1.2.9/p3/deepLoop/dataGenerator.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/dataGeneratorBatch.py` & `astro-p3-1.2.9/p3/deepLoop/dataGeneratorBatch.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/deepLoopPerformance.py` & `astro-p3-1.2.9/p3/deepLoop/deepLoopPerformance.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/deepLoopPerformanceBatch.py` & `astro-p3-1.2.9/p3/deepLoop/deepLoopPerformanceBatch.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/jobGenerate.sh` & `astro-p3-1.2.9/p3/deepLoop/jobGenerate.sh`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/jobPerformance.sh` & `astro-p3-1.2.9/p3/deepLoop/jobPerformance.sh`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/deepLoop/recover_list.py` & `astro-p3-1.2.9/p3/deepLoop/recover_list.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfFitting/confidenceInterval.py` & `astro-p3-1.2.9/p3/psfFitting/confidenceInterval.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfFitting/fittingUtils.py` & `astro-p3-1.2.9/p3/psfFitting/fittingUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfFitting/imageModel.py` & `astro-p3-1.2.9/p3/psfFitting/imageModel.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfFitting/psfFitting.py` & `astro-p3-1.2.9/p3/psfFitting/psfFitting.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfao21/psfao21.py` & `astro-p3-1.2.9/p3/psfao21/psfao21.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfr/psfR.py` & `astro-p3-1.2.9/p3/psfr/psfR.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/psfr/psfrUtils.py` & `astro-p3-1.2.9/p3/psfr/psfrUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/configFile.py` & `astro-p3-1.2.9/p3/telemetry/configFile.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/keckUtils.py` & `astro-p3-1.2.9/p3/telemetry/keckUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/massdimm.py` & `astro-p3-1.2.9/p3/telemetry/massdimm.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/sphereUtils.py` & `astro-p3-1.2.9/p3/telemetry/sphereUtils.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/systemDiagnosis.py` & `astro-p3-1.2.9/p3/telemetry/systemDiagnosis.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/telemetryKASP.py` & `astro-p3-1.2.9/p3/telemetry/telemetryKASP.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/telemetry/telemetryKeck.py` & `astro-p3-1.2.9/p3/telemetry/telemetryKeck.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/p3/testing/tests_p3.py` & `astro-p3-1.2.9/p3/testing/tests_p3.py`

 * *Files identical despite different names*

### Comparing `astro-p3-1.2.8/pyproject.toml` & `astro-p3-1.2.9/pyproject.toml`

 * *Files identical despite different names*

