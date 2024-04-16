# Comparing `tmp/herschelhelp-0.0.tar.gz` & `tmp/herschelhelp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herschelhelp-0.0.tar", last modified: Thu Apr 11 16:43:05 2024, max compression
+gzip compressed data, was "herschelhelp-1.0.1.tar", last modified: Tue Apr 16 12:15:56 2024, max compression
```

## Comparing `herschelhelp-0.0.tar` & `herschelhelp-1.0.1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:05.639887 herschelhelp-0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-11 16:42:30.000000 herschelhelp-0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 16:42:30.000000 herschelhelp-0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 16:43:05.639887 herschelhelp-0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-11 16:42:30.000000 herschelhelp-0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:05.587886 herschelhelp-0.0/database_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:05.591886 herschelhelp-0.0/database_builder/coverages/
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/AKARI-NEP_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/AKARI-SEP_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/Bootes_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/CDFS-SWIRE_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/COSMOS_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/EGS_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/ELAIS-N1_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/ELAIS-N2_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/ELAIS-S1_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/GAMA-09_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/GAMA-12_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/GAMA-15_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/HATLAS-NGP_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)   106560 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/HATLAS-SGP_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/HDF-N_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)   123840 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/Herschel-Stripe-82_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/Lockman-SWIRE_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/SA13_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/SPIRE-NEP_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/SSDF_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/XMM-13hr_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/XMM-LSS_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/coverages/xFLS_MOC.fits
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/fields.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:05.635887 herschelhelp-0.0/database_builder/filters/
--rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/90prime_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/90prime_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    40850 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/90prime_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)   239593 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/acs_f435w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   342146 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/acs_f606w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   277376 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/acs_f775w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   348537 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/acs_f814w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   299477 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/acs_f850lp.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/bessell_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/bessell_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/bessell_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/bessell_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/bessell_v.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/cfht12k_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17583 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/cfht12k_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/cfht12k_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/decam_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/decam_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/decam_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/decam_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25687 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/decam_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    49382 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/galex_fuv.xml
--rw-r--r--   0 runner    (1001) docker     (127)   128431 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/galex_nuv.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/gpc1_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/gpc1_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19210 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/gpc1_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/gpc1_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17917 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/gpc1_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    27915 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/hawki_k.xml
--rw-r--r--   0 runner    (1001) docker     (127)    34326 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/irac_i1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    35159 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/irac_i2.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28456 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/irac_i3.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/irac_i4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    88624 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/isaac_k.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/lbc_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    51954 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/lbc_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/megacam_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/megacam_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/megacam_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/megacam_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/megacam_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/megacam_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44477 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mips_160.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mips_24.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mips_70.xml
--rw-r--r--   0 runner    (1001) docker     (127)    41596 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mmt_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    49778 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mmt_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    43612 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mmt_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mmt_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    59738 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mmt_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)   260715 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/moircs_k.xml
--rw-r--r--   0 runner    (1001) docker     (127)    80175 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/moircs_ks.xml
--rw-r--r--   0 runner    (1001) docker     (127)    67792 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mosaic_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    38350 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mosaic_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)   117383 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mosaic_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    75564 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mosaic_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    99723 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/mosaic_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    82160 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_h.xml
--rw-r--r--   0 runner    (1001) docker     (127)    82160 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_h1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    82160 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_h2.xml
--rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_j.xml
--rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_j1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_j2.xml
--rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_j3.xml
--rw-r--r--   0 runner    (1001) docker     (127)    97551 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/newfirm_k.xml
--rw-r--r--   0 runner    (1001) docker     (127)   719906 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/nicmos_f110w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   607355 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/nicmos_f160w.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omega2000_j.xml
--rw-r--r--   0 runner    (1001) docker     (127)    77132 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omega2000_ks.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19571 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omegacam_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omegacam_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16627 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omegacam_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omegacam_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/omegacam_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    45366 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/pacs_blue.xml
--rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/pacs_green.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28540 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/pacs_red.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15943 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/quirc_hk.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/sdss_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/sdss_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/sdss_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/sdss_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18785 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/sdss_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/spire_250.xml
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/spire_350.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23919 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/spire_500.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20489 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    67582 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ia484.xml
--rw-r--r--   0 runner    (1001) docker     (127)    76834 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ia527.xml
--rw-r--r--   0 runner    (1001) docker     (127)    94554 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ia624.xml
--rw-r--r--   0 runner    (1001) docker     (127)   115827 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ia679.xml
--rw-r--r--   0 runner    (1001) docker     (127)    95444 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ia738.xml
--rw-r--r--   0 runner    (1001) docker     (127)    49537 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ia767.xml
--rw-r--r--   0 runner    (1001) docker     (127)    57111 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ib427.xml
--rw-r--r--   0 runner    (1001) docker     (127)    59665 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ib464.xml
--rw-r--r--   0 runner    (1001) docker     (127)    71919 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ib505.xml
--rw-r--r--   0 runner    (1001) docker     (127)    96609 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ib574.xml
--rw-r--r--   0 runner    (1001) docker     (127)    94360 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ib709.xml
--rw-r--r--   0 runner    (1001) docker     (127)    87982 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ib827.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_ip.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_n816.xml
--rw-r--r--   0 runner    (1001) docker     (127)    72894 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_n921.xml
--rw-r--r--   0 runner    (1001) docker     (127)    52422 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_nb711.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53922 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_nb816.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_rc.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23659 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_rp.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20166 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_v.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    87982 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_zp.xml
--rw-r--r--   0 runner    (1001) docker     (127)    22952 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/suprime_zpp.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/tifkam_ks.xml
--rw-r--r--   0 runner    (1001) docker     (127)    76369 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/ukidss_h.xml
--rw-r--r--   0 runner    (1001) docker     (127)    33869 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/ukidss_j.xml
--rw-r--r--   0 runner    (1001) docker     (127)    69435 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/ukidss_k.xml
--rw-r--r--   0 runner    (1001) docker     (127)    32215 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/ukidss_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    49521 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/vista_h.xml
--rw-r--r--   0 runner    (1001) docker     (127)    33655 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/vista_j.xml
--rw-r--r--   0 runner    (1001) docker     (127)    55986 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/vista_ks.xml
--rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/vista_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21037 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/vista_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)   261186 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc3_f098m.xml
--rw-r--r--   0 runner    (1001) docker     (127)   382066 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc3_f105w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   340247 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc3_f125w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   388750 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc3_f140w.xml
--rw-r--r--   0 runner    (1001) docker     (127)   264721 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc3_f160w.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28020 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc_g.xml
--rw-r--r--   0 runner    (1001) docker     (127)    33201 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfc_z.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_416nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_461nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_485nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_518nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_571nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_604nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_646nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_696nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_753nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_815nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_856nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16571 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_914nm.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    41320 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_b123.xml
--rw-r--r--   0 runner    (1001) docker     (127)    26806 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_i.xml
--rw-r--r--   0 runner    (1001) docker     (127)    34351 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_r.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_u.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18886 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wfi_v.xml
--rw-r--r--   0 runner    (1001) docker     (127)    75882 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wircam_h.xml
--rw-r--r--   0 runner    (1001) docker     (127)   106895 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wircam_j.xml
--rw-r--r--   0 runner    (1001) docker     (127)    80023 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wircam_ks.xml
--rw-r--r--   0 runner    (1001) docker     (127)    87590 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wircam_y.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wircs_j.xml
--rw-r--r--   0 runner    (1001) docker     (127)    83392 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wircs_k.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wise_w1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wise_w2.xml
--rw-r--r--   0 runner    (1001) docker     (127)   112642 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wise_w3.xml
--rw-r--r--   0 runner    (1001) docker     (127)    91547 2024-04-11 16:42:30.000000 herschelhelp-0.0/database_builder/filters/wise_w4.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:05.639887 herschelhelp-0.0/herschelhelp/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    61205 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/cutouts_dl.py
--rw-r--r--   0 runner    (1001) docker     (127)    84304 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/cutouts_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/depth_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/image_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-11 16:42:30.000000 herschelhelp-0.0/herschelhelp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:05.639887 herschelhelp-0.0/herschelhelp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 16:43:05.000000 herschelhelp-0.0/herschelhelp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-04-11 16:43:05.000000 herschelhelp-0.0/herschelhelp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:43:05.000000 herschelhelp-0.0/herschelhelp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 16:43:05.000000 herschelhelp-0.0/herschelhelp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 16:43:05.000000 herschelhelp-0.0/herschelhelp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 16:43:05.000000 herschelhelp-0.0/herschelhelp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:43:05.639887 herschelhelp-0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-11 16:42:30.000000 herschelhelp-0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:15:56.384104 herschelhelp-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-16 12:15:56.384104 herschelhelp-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:15:56.332103 herschelhelp-1.0.1/database_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:15:56.336103 herschelhelp-1.0.1/database_builder/coverages/
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/AKARI-NEP_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/AKARI-SEP_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/Bootes_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/CDFS-SWIRE_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/COSMOS_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/EGS_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/ELAIS-N1_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/ELAIS-N2_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/ELAIS-S1_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/GAMA-09_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/GAMA-12_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/GAMA-15_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/HATLAS-NGP_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   106560 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/HATLAS-SGP_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/HDF-N_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   123840 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/Herschel-Stripe-82_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/Lockman-SWIRE_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/SA13_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/SPIRE-NEP_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/SSDF_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/XMM-13hr_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/XMM-LSS_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/coverages/xFLS_MOC.fits
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/fields.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:15:56.380104 herschelhelp-1.0.1/database_builder/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/90prime_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/90prime_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    40850 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/90prime_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   239593 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/acs_f435w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   342146 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/acs_f606w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   277376 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/acs_f775w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   348537 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/acs_f814w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   299477 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/acs_f850lp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/bessell_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/bessell_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/bessell_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/bessell_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/bessell_v.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/cfht12k_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17583 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/cfht12k_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/cfht12k_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/decam_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/decam_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/decam_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/decam_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25687 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/decam_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    49382 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/galex_fuv.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   128431 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/galex_nuv.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/gpc1_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/gpc1_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19210 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/gpc1_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/gpc1_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17917 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/gpc1_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27915 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/hawki_k.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    34326 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/irac_i1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35159 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/irac_i2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28456 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/irac_i3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/irac_i4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    88624 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/isaac_k.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/lbc_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    51954 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/lbc_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/megacam_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/megacam_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/megacam_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/megacam_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/megacam_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/megacam_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44477 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mips_160.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mips_24.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mips_70.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    41596 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mmt_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    49778 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mmt_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    43612 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mmt_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mmt_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    59738 2024-04-16 12:15:18.000000 herschelhelp-1.0.1/database_builder/filters/mmt_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   260715 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/moircs_k.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    80175 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/moircs_ks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    67792 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/mosaic_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    38350 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/mosaic_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   117383 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/mosaic_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    75564 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/mosaic_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    99723 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/mosaic_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    82160 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_h.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    82160 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_h1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    82160 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_h2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_j1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_j2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   280436 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_j3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    97551 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/newfirm_k.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   719906 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/nicmos_f110w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   607355 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/nicmos_f160w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omega2000_j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    77132 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omega2000_ks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19571 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omegacam_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omegacam_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16627 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omegacam_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omegacam_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/omegacam_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    45366 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/pacs_blue.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/pacs_green.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28540 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/pacs_red.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15943 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/quirc_hk.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/sdss_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/sdss_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/sdss_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/sdss_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18785 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/sdss_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/spire_250.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/spire_350.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23919 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/spire_500.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20489 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    67582 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ia484.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    76834 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ia527.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    94554 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ia624.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   115827 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ia679.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    95444 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ia738.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    49537 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ia767.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    57111 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ib427.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    59665 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ib464.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71919 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ib505.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    96609 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ib574.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    94360 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ib709.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    87982 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ib827.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_ip.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_n816.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    72894 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_n921.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    52422 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_nb711.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53922 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_nb816.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_rc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23659 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_rp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20166 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_v.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    87982 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_zp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22952 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/suprime_zpp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/tifkam_ks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    76369 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/ukidss_h.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    33869 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/ukidss_j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    69435 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/ukidss_k.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    32215 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/ukidss_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    49521 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/vista_h.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    33655 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/vista_j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    55986 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/vista_ks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/vista_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21037 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/vista_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   261186 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc3_f098m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   382066 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc3_f105w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   340247 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc3_f125w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   388750 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc3_f140w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   264721 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc3_f160w.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28020 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc_g.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    33201 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfc_z.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_416nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_461nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_485nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_518nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_571nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_604nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_646nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_696nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_753nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_815nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_856nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16571 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_914nm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    41320 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_b123.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    26806 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_i.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    34351 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_r.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_u.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18886 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wfi_v.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    75882 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wircam_h.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   106895 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wircam_j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    80023 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wircam_ks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    87590 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wircam_y.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wircs_j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    83392 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wircs_k.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wise_w1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wise_w2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   112642 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wise_w3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    91547 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/database_builder/filters/wise_w4.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:15:56.384104 herschelhelp-1.0.1/herschelhelp/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61205 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/cutouts_dl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84304 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/cutouts_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/depth_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/image_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/herschelhelp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:15:56.384104 herschelhelp-1.0.1/herschelhelp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-16 12:15:56.000000 herschelhelp-1.0.1/herschelhelp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-04-16 12:15:56.000000 herschelhelp-1.0.1/herschelhelp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:15:56.000000 herschelhelp-1.0.1/herschelhelp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 12:15:56.000000 herschelhelp-1.0.1/herschelhelp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 12:15:56.000000 herschelhelp-1.0.1/herschelhelp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 12:15:56.000000 herschelhelp-1.0.1/herschelhelp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:15:56.384104 herschelhelp-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-16 12:15:19.000000 herschelhelp-1.0.1/setup.py
```

### Comparing `herschelhelp-0.0/LICENSE` & `herschelhelp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/PKG-INFO` & `herschelhelp-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herschelhelp
-Version: 0.0
+Version: 1.0.1
 Summary: HELP project module
 Author: Yannick Roehlly
 Author-email: yannick.roehlly@lam.fr
 License: MIT
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: astropy
```

### Comparing `herschelhelp-0.0/README.md` & `herschelhelp-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/__init__.py` & `herschelhelp-1.0.1/database_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/AKARI-NEP_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/AKARI-NEP_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/AKARI-SEP_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/AKARI-SEP_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/Bootes_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/Bootes_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/CDFS-SWIRE_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/CDFS-SWIRE_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/COSMOS_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/COSMOS_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/EGS_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/EGS_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/ELAIS-N1_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/ELAIS-N1_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/ELAIS-N2_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/ELAIS-N2_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/ELAIS-S1_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/ELAIS-S1_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/GAMA-09_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/GAMA-09_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/GAMA-12_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/GAMA-12_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/GAMA-15_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/GAMA-15_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/HATLAS-NGP_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/HATLAS-NGP_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/HATLAS-SGP_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/HATLAS-SGP_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/HDF-N_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/HDF-N_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/Herschel-Stripe-82_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/Herschel-Stripe-82_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/Lockman-SWIRE_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/Lockman-SWIRE_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/SA13_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/SA13_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/SPIRE-NEP_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/SPIRE-NEP_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/SSDF_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/SSDF_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/XMM-13hr_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/XMM-13hr_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/XMM-LSS_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/XMM-LSS_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/coverages/xFLS_MOC.fits` & `herschelhelp-1.0.1/database_builder/coverages/xFLS_MOC.fits`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/90prime_g.xml` & `herschelhelp-1.0.1/database_builder/filters/90prime_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/90prime_r.xml` & `herschelhelp-1.0.1/database_builder/filters/90prime_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/90prime_z.xml` & `herschelhelp-1.0.1/database_builder/filters/90prime_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/acs_f435w.xml` & `herschelhelp-1.0.1/database_builder/filters/acs_f435w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/acs_f606w.xml` & `herschelhelp-1.0.1/database_builder/filters/acs_f606w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/acs_f775w.xml` & `herschelhelp-1.0.1/database_builder/filters/acs_f775w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/acs_f814w.xml` & `herschelhelp-1.0.1/database_builder/filters/acs_f814w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/acs_f850lp.xml` & `herschelhelp-1.0.1/database_builder/filters/acs_f850lp.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/bessell_b.xml` & `herschelhelp-1.0.1/database_builder/filters/bessell_b.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/bessell_i.xml` & `herschelhelp-1.0.1/database_builder/filters/bessell_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/bessell_r.xml` & `herschelhelp-1.0.1/database_builder/filters/bessell_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/bessell_u.xml` & `herschelhelp-1.0.1/database_builder/filters/bessell_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/bessell_v.xml` & `herschelhelp-1.0.1/database_builder/filters/bessell_v.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/cfht12k_b.xml` & `herschelhelp-1.0.1/database_builder/filters/cfht12k_b.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/cfht12k_i.xml` & `herschelhelp-1.0.1/database_builder/filters/cfht12k_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/cfht12k_r.xml` & `herschelhelp-1.0.1/database_builder/filters/cfht12k_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/decam_g.xml` & `herschelhelp-1.0.1/database_builder/filters/decam_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/decam_i.xml` & `herschelhelp-1.0.1/database_builder/filters/decam_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/decam_r.xml` & `herschelhelp-1.0.1/database_builder/filters/decam_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/decam_y.xml` & `herschelhelp-1.0.1/database_builder/filters/decam_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/decam_z.xml` & `herschelhelp-1.0.1/database_builder/filters/decam_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/galex_fuv.xml` & `herschelhelp-1.0.1/database_builder/filters/galex_fuv.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/galex_nuv.xml` & `herschelhelp-1.0.1/database_builder/filters/galex_nuv.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/gpc1_g.xml` & `herschelhelp-1.0.1/database_builder/filters/gpc1_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/gpc1_i.xml` & `herschelhelp-1.0.1/database_builder/filters/gpc1_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/gpc1_r.xml` & `herschelhelp-1.0.1/database_builder/filters/gpc1_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/gpc1_y.xml` & `herschelhelp-1.0.1/database_builder/filters/gpc1_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/gpc1_z.xml` & `herschelhelp-1.0.1/database_builder/filters/gpc1_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/hawki_k.xml` & `herschelhelp-1.0.1/database_builder/filters/hawki_k.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/irac_i1.xml` & `herschelhelp-1.0.1/database_builder/filters/irac_i1.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/irac_i2.xml` & `herschelhelp-1.0.1/database_builder/filters/irac_i2.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/irac_i3.xml` & `herschelhelp-1.0.1/database_builder/filters/irac_i3.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/irac_i4.xml` & `herschelhelp-1.0.1/database_builder/filters/irac_i4.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/isaac_k.xml` & `herschelhelp-1.0.1/database_builder/filters/isaac_k.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/lbc_u.xml` & `herschelhelp-1.0.1/database_builder/filters/lbc_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/lbc_y.xml` & `herschelhelp-1.0.1/database_builder/filters/lbc_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/megacam_g.xml` & `herschelhelp-1.0.1/database_builder/filters/megacam_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/megacam_i.xml` & `herschelhelp-1.0.1/database_builder/filters/megacam_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/megacam_r.xml` & `herschelhelp-1.0.1/database_builder/filters/megacam_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/megacam_u.xml` & `herschelhelp-1.0.1/database_builder/filters/megacam_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/megacam_y.xml` & `herschelhelp-1.0.1/database_builder/filters/megacam_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/megacam_z.xml` & `herschelhelp-1.0.1/database_builder/filters/megacam_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mips_160.xml` & `herschelhelp-1.0.1/database_builder/filters/mips_160.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mips_24.xml` & `herschelhelp-1.0.1/database_builder/filters/mips_24.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mips_70.xml` & `herschelhelp-1.0.1/database_builder/filters/mips_70.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mmt_g.xml` & `herschelhelp-1.0.1/database_builder/filters/mmt_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mmt_i.xml` & `herschelhelp-1.0.1/database_builder/filters/mmt_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mmt_r.xml` & `herschelhelp-1.0.1/database_builder/filters/mmt_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mmt_u.xml` & `herschelhelp-1.0.1/database_builder/filters/mmt_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mmt_z.xml` & `herschelhelp-1.0.1/database_builder/filters/mmt_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/moircs_k.xml` & `herschelhelp-1.0.1/database_builder/filters/moircs_k.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/moircs_ks.xml` & `herschelhelp-1.0.1/database_builder/filters/moircs_ks.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mosaic_b.xml` & `herschelhelp-1.0.1/database_builder/filters/mosaic_b.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mosaic_i.xml` & `herschelhelp-1.0.1/database_builder/filters/mosaic_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mosaic_r.xml` & `herschelhelp-1.0.1/database_builder/filters/mosaic_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mosaic_u.xml` & `herschelhelp-1.0.1/database_builder/filters/mosaic_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/mosaic_z.xml` & `herschelhelp-1.0.1/database_builder/filters/mosaic_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_h.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_h.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_h1.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_h1.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_h2.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_h2.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_j.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_j.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_j1.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_j1.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_j2.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_j2.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_j3.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_j3.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/newfirm_k.xml` & `herschelhelp-1.0.1/database_builder/filters/newfirm_k.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/nicmos_f110w.xml` & `herschelhelp-1.0.1/database_builder/filters/nicmos_f110w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/nicmos_f160w.xml` & `herschelhelp-1.0.1/database_builder/filters/nicmos_f160w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omega2000_j.xml` & `herschelhelp-1.0.1/database_builder/filters/omega2000_j.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omega2000_ks.xml` & `herschelhelp-1.0.1/database_builder/filters/omega2000_ks.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omegacam_g.xml` & `herschelhelp-1.0.1/database_builder/filters/omegacam_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omegacam_i.xml` & `herschelhelp-1.0.1/database_builder/filters/omegacam_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omegacam_r.xml` & `herschelhelp-1.0.1/database_builder/filters/omegacam_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omegacam_u.xml` & `herschelhelp-1.0.1/database_builder/filters/omegacam_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/omegacam_z.xml` & `herschelhelp-1.0.1/database_builder/filters/omegacam_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/pacs_blue.xml` & `herschelhelp-1.0.1/database_builder/filters/pacs_blue.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/pacs_green.xml` & `herschelhelp-1.0.1/database_builder/filters/pacs_green.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/pacs_red.xml` & `herschelhelp-1.0.1/database_builder/filters/pacs_red.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/quirc_hk.xml` & `herschelhelp-1.0.1/database_builder/filters/quirc_hk.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/sdss_g.xml` & `herschelhelp-1.0.1/database_builder/filters/sdss_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/sdss_i.xml` & `herschelhelp-1.0.1/database_builder/filters/sdss_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/sdss_r.xml` & `herschelhelp-1.0.1/database_builder/filters/sdss_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/sdss_u.xml` & `herschelhelp-1.0.1/database_builder/filters/sdss_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/sdss_z.xml` & `herschelhelp-1.0.1/database_builder/filters/sdss_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/spire_250.xml` & `herschelhelp-1.0.1/database_builder/filters/spire_250.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/spire_350.xml` & `herschelhelp-1.0.1/database_builder/filters/spire_350.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/spire_500.xml` & `herschelhelp-1.0.1/database_builder/filters/spire_500.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_b.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_b.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_g.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_i.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ia484.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ia484.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ia527.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ia527.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ia624.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ia624.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ia679.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ia679.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ia738.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ia738.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ia767.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ia767.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ib427.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ib427.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ib464.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ib464.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ib505.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ib505.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ib574.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ib574.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ib709.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ib709.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ib827.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ib827.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_ip.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_ip.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_n816.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_n816.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_n921.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_n921.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_nb711.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_nb711.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_nb816.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_nb816.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_r.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_rc.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_rc.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_rp.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_rp.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_v.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_v.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_y.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_z.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_zp.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_zp.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/suprime_zpp.xml` & `herschelhelp-1.0.1/database_builder/filters/suprime_zpp.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/tifkam_ks.xml` & `herschelhelp-1.0.1/database_builder/filters/tifkam_ks.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/ukidss_h.xml` & `herschelhelp-1.0.1/database_builder/filters/ukidss_h.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/ukidss_j.xml` & `herschelhelp-1.0.1/database_builder/filters/ukidss_j.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/ukidss_k.xml` & `herschelhelp-1.0.1/database_builder/filters/ukidss_k.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/ukidss_y.xml` & `herschelhelp-1.0.1/database_builder/filters/ukidss_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/vista_h.xml` & `herschelhelp-1.0.1/database_builder/filters/vista_h.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/vista_j.xml` & `herschelhelp-1.0.1/database_builder/filters/vista_j.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/vista_ks.xml` & `herschelhelp-1.0.1/database_builder/filters/vista_ks.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/vista_y.xml` & `herschelhelp-1.0.1/database_builder/filters/vista_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/vista_z.xml` & `herschelhelp-1.0.1/database_builder/filters/vista_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc3_f098m.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc3_f098m.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc3_f105w.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc3_f105w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc3_f125w.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc3_f125w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc3_f140w.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc3_f140w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc3_f160w.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc3_f160w.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc_g.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc_g.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc_i.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc_r.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc_u.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfc_z.xml` & `herschelhelp-1.0.1/database_builder/filters/wfc_z.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_416nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_416nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_461nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_461nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_485nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_485nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_518nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_518nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_571nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_571nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_604nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_604nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_646nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_646nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_696nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_696nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_753nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_753nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_815nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_815nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_856nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_856nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_914nm.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_914nm.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_b.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_b.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_b123.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_b123.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_i.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_i.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_r.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_r.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_u.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_u.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wfi_v.xml` & `herschelhelp-1.0.1/database_builder/filters/wfi_v.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wircam_h.xml` & `herschelhelp-1.0.1/database_builder/filters/wircam_h.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wircam_j.xml` & `herschelhelp-1.0.1/database_builder/filters/wircam_j.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wircam_ks.xml` & `herschelhelp-1.0.1/database_builder/filters/wircam_ks.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wircam_y.xml` & `herschelhelp-1.0.1/database_builder/filters/wircam_y.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wircs_j.xml` & `herschelhelp-1.0.1/database_builder/filters/wircs_j.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wircs_k.xml` & `herschelhelp-1.0.1/database_builder/filters/wircs_k.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wise_w1.xml` & `herschelhelp-1.0.1/database_builder/filters/wise_w1.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wise_w2.xml` & `herschelhelp-1.0.1/database_builder/filters/wise_w2.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wise_w3.xml` & `herschelhelp-1.0.1/database_builder/filters/wise_w3.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/database_builder/filters/wise_w4.xml` & `herschelhelp-1.0.1/database_builder/filters/wise_w4.xml`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/commands.py` & `herschelhelp-1.0.1/herschelhelp/commands.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/cutouts_dl.py` & `herschelhelp-1.0.1/herschelhelp/cutouts_dl.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/cutouts_server.py` & `herschelhelp-1.0.1/herschelhelp/cutouts_server.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/database.py` & `herschelhelp-1.0.1/herschelhelp/database.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/depth_coverage.py` & `herschelhelp-1.0.1/herschelhelp/depth_coverage.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/external.py` & `herschelhelp-1.0.1/herschelhelp/external.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/filters.py` & `herschelhelp-1.0.1/herschelhelp/filters.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/footprints.py` & `herschelhelp-1.0.1/herschelhelp/footprints.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/image_plotting.py` & `herschelhelp-1.0.1/herschelhelp/image_plotting.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp/utils.py` & `herschelhelp-1.0.1/herschelhelp/utils.py`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/herschelhelp.egg-info/PKG-INFO` & `herschelhelp-1.0.1/herschelhelp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herschelhelp
-Version: 0.0
+Version: 1.0.1
 Summary: HELP project module
 Author: Yannick Roehlly
 Author-email: yannick.roehlly@lam.fr
 License: MIT
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: astropy
```

### Comparing `herschelhelp-0.0/herschelhelp.egg-info/SOURCES.txt` & `herschelhelp-1.0.1/herschelhelp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `herschelhelp-0.0/setup.py` & `herschelhelp-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         import database_builder
         database_builder.build_base()
         # Process with the standard build
         build_py.run(self)
 
 setup(
     name="herschelhelp",
-    version="0.0",
+    version="1.0.1",
     description="HELP project module",
     long_description=README,
     author="Yannick Roehlly",
     author_email="yannick.roehlly@lam.fr",
     license='MIT',
     setup_requires=REQUIREMENTS,
     install_requires=REQUIREMENTS,
```

