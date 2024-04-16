# Comparing `tmp/pysus-0.9.3.tar.gz` & `tmp/pysus-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysus-0.9.3.tar", max compression
+gzip compressed data, was "pysus-0.9.4.tar", max compression
```

## Comparing `pysus-0.9.3.tar` & `pysus-0.9.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    35149 2023-06-06 14:48:28.955027 pysus-0.9.3/LICENSE
--rw-r--r--   0        0        0     1372 2023-06-06 14:50:33.538730 pysus-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     8421 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/Analyzing SIH.ipynb
--rw-r--r--   0        0        0    15450 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/Analyzing SIM.ipynb
--rw-r--r--   0        0        0    14877 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/Analyzing SINASC Data.ipynb
--rw-r--r--   0        0        0    47374 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/Getting_CNES_Data.ipynb
--rw-r--r--   0        0        0     3057 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/Processing SIM with municipality.ipynb
--rw-r--r--   0        0        0    27870 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/Processing SIM.ipynb
--rw-r--r--   0        0        0    59869 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/Notebooks/SINAN.ipynb
--rw-r--r--   0        0        0      422 2023-06-06 14:50:33.538730 pysus-0.9.3/pysus/__init__.py
--rw-r--r--   0        0        0   165526 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/dataset/geocode_by_cities.json
--rw-r--r--   0        0        0     3931 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/ANIM.tar.gz
--rw-r--r--   0        0        0     7064 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/BOTU.tar.gz
--rw-r--r--   0        0        0     5341 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/CHAG.tar.gz
--rw-r--r--   0        0        0     5439 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/CHIK.tar.gz
--rw-r--r--   0        0        0     5290 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/COLE.tar.gz
--rw-r--r--   0        0        0     4496 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/COQU.tar.gz
--rw-r--r--   0        0        0     5439 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/DENG.tar.gz
--rw-r--r--   0        0        0     5093 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/DIFT.tar.gz
--rw-r--r--   0        0        0     2953 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/ESQU.tar.gz
--rw-r--r--   0        0        0     5257 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/FAMA.tar.gz
--rw-r--r--   0        0        0     4638 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/FMAC.tar.gz
--rw-r--r--   0        0        0     6354 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/FTIF.tar.gz
--rw-r--r--   0        0        0     4247 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/HANS.tar.gz
--rw-r--r--   0        0        0     6202 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/HANT.tar.gz
--rw-r--r--   0        0        0     5603 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/HEPA.tar.gz
--rw-r--r--   0        0        0     4554 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/IEXO.tar.gz
--rw-r--r--   0        0        0     4214 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/LEIV.tar.gz
--rw-r--r--   0        0        0     4958 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/LEPT.tar.gz
--rw-r--r--   0        0        0     4293 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/LTAN.tar.gz
--rw-r--r--   0        0        0     3614 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/MALA.tar.gz
--rw-r--r--   0        0        0     5652 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/MENI.tar.gz
--rw-r--r--   0        0        0     3114 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/PEST.tar.gz
--rw-r--r--   0        0        0     5404 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/RAIV.tar.gz
--rw-r--r--   0        0        0     5439 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/SIFC.tar.gz
--rw-r--r--   0        0        0     1952 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/SIFG.tar.gz
--rw-r--r--   0        0        0     4189 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/TETA.tar.gz
--rw-r--r--   0        0        0     5518 2023-06-06 14:48:28.999027 pysus-0.9.3/pysus/metadata/SINAN/TETN.tar.gz
--rw-r--r--   0        0        0     5659 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/metadata/SINAN/TUBE.tar.gz
--rw-r--r--   0        0        0    35103 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/metadata/SINAN/typecast.py
--rw-r--r--   0        0        0      766 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/CIHA.py
--rw-r--r--   0        0        0     2277 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/CNES.py
--rw-r--r--   0        0        0     3078 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/ESUS.py
--rw-r--r--   0        0        0    13567 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/IBGE.py
--rw-r--r--   0        0        0     3170 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/Infodengue.py
--rw-r--r--   0        0        0      696 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/Infogripe.py
--rw-r--r--   0        0        0     1016 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/PNI.py
--rw-r--r--   0        0        0     2382 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/SIA.py
--rw-r--r--   0        0        0      953 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/SIH.py
--rw-r--r--   0        0        0     6675 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/SIM.py
--rw-r--r--   0        0        0     1688 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/SINAN.py
--rw-r--r--   0        0        0    24411 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/__init__.py
--rw-r--r--   0        0        0      790 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/sinasc.py
--rw-r--r--   0        0        0     3677 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/online_data/vaccine.py
--rw-r--r--   0        0        0     1922 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/preprocessing/ESUS.py
--rw-r--r--   0        0        0     6289 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/preprocessing/SIM.py
--rw-r--r--   0        0        0      128 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/preprocessing/__init__.py
--rw-r--r--   0        0        0    10109 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/preprocessing/decoders.py
--rw-r--r--   0        0        0     2402 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/preprocessing/geodata.py
--rw-r--r--   0        0        0     3878 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/preprocessing/sinan.py
--rw-r--r--   0        0        0      128 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/tests/__init__.py
--rw-r--r--   0        0        0      505 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/tests/test_SIA.py
--rw-r--r--   0        0        0      722 2023-06-06 14:48:29.003027 pysus-0.9.3/pysus/tests/test_cnes.py
--rw-r--r--   0        0        0  9175254 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/EPR-2016-06-01-2016.dbf
--rw-r--r--   0        0        0       66 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/__init__.py
--rw-r--r--   0        0        0     3126 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_Infodengue.py
--rw-r--r--   0        0        0      330 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_Infogripe.py
--rw-r--r--   0        0        0      640 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_PNI.py
--rw-r--r--   0        0        0      795 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_ciha.py
--rw-r--r--   0        0        0     2265 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_sia.py
--rw-r--r--   0        0        0      547 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_sih.py
--rw-r--r--   0        0        0     1249 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_sim.py
--rw-r--r--   0        0        0     4624 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_sinan.py
--rw-r--r--   0        0        0      785 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_sinasc.py
--rw-r--r--   0        0        0      419 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_data/test_vaccine.py
--rw-r--r--   0        0        0     6975 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_decoders.py
--rw-r--r--   0        0        0      304 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_esus.py
--rw-r--r--   0        0        0     1382 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_ibge.py
--rw-r--r--   0        0        0      741 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_init.py
--rw-r--r--   0        0        0      642 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_sih.py
--rw-r--r--   0        0        0     2123 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_sim.py
--rw-r--r--   0        0        0      758 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/tests/test_utilities.py
--rw-r--r--   0        0        0        0 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/utilities/__init__.py
--rw-r--r--   0        0        0     2766 2023-06-06 14:48:29.031027 pysus-0.9.3/pysus/utilities/readdbc.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 pysus-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-31 23:40:35.235189 pysus-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1333 2023-07-31 23:42:59.490255 pysus-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     8421 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/Analyzing SIH.ipynb
+-rw-r--r--   0        0        0    15450 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/Analyzing SIM.ipynb
+-rw-r--r--   0        0        0    14877 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/Analyzing SINASC Data.ipynb
+-rw-r--r--   0        0        0    47374 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/Getting_CNES_Data.ipynb
+-rw-r--r--   0        0        0     3057 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/Processing SIM with municipality.ipynb
+-rw-r--r--   0        0        0    27870 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/Processing SIM.ipynb
+-rw-r--r--   0        0        0    59869 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/Notebooks/SINAN.ipynb
+-rw-r--r--   0        0        0      422 2023-07-31 23:42:59.490255 pysus-0.9.4/pysus/__init__.py
+-rw-r--r--   0        0        0   165526 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/dataset/geocode_by_cities.json
+-rw-r--r--   0        0        0     3931 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/ANIM.tar.gz
+-rw-r--r--   0        0        0     7064 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/BOTU.tar.gz
+-rw-r--r--   0        0        0     5341 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/CHAG.tar.gz
+-rw-r--r--   0        0        0     5439 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/CHIK.tar.gz
+-rw-r--r--   0        0        0     5290 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/COLE.tar.gz
+-rw-r--r--   0        0        0     4496 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/COQU.tar.gz
+-rw-r--r--   0        0        0     5439 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/DENG.tar.gz
+-rw-r--r--   0        0        0     5093 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/DIFT.tar.gz
+-rw-r--r--   0        0        0     2953 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/ESQU.tar.gz
+-rw-r--r--   0        0        0     5257 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/FAMA.tar.gz
+-rw-r--r--   0        0        0     4638 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/FMAC.tar.gz
+-rw-r--r--   0        0        0     6354 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/FTIF.tar.gz
+-rw-r--r--   0        0        0     4247 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/HANS.tar.gz
+-rw-r--r--   0        0        0     6202 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/HANT.tar.gz
+-rw-r--r--   0        0        0     5603 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/HEPA.tar.gz
+-rw-r--r--   0        0        0     4554 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/IEXO.tar.gz
+-rw-r--r--   0        0        0     4214 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/LEIV.tar.gz
+-rw-r--r--   0        0        0     4958 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/LEPT.tar.gz
+-rw-r--r--   0        0        0     4293 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/LTAN.tar.gz
+-rw-r--r--   0        0        0     3614 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/MALA.tar.gz
+-rw-r--r--   0        0        0     5652 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/MENI.tar.gz
+-rw-r--r--   0        0        0     3114 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/PEST.tar.gz
+-rw-r--r--   0        0        0     5404 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/RAIV.tar.gz
+-rw-r--r--   0        0        0     5439 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/SIFC.tar.gz
+-rw-r--r--   0        0        0     1952 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/SIFG.tar.gz
+-rw-r--r--   0        0        0     4189 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/TETA.tar.gz
+-rw-r--r--   0        0        0     5518 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/TETN.tar.gz
+-rw-r--r--   0        0        0     5659 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/TUBE.tar.gz
+-rw-r--r--   0        0        0    35103 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/metadata/SINAN/typecast.py
+-rw-r--r--   0        0        0      766 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/CIHA.py
+-rw-r--r--   0        0        0     2277 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/CNES.py
+-rw-r--r--   0        0        0     3078 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/ESUS.py
+-rw-r--r--   0        0        0    13567 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/IBGE.py
+-rw-r--r--   0        0        0     3170 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/Infodengue.py
+-rw-r--r--   0        0        0      696 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/Infogripe.py
+-rw-r--r--   0        0        0     1016 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/PNI.py
+-rw-r--r--   0        0        0     2382 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/SIA.py
+-rw-r--r--   0        0        0      953 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/SIH.py
+-rw-r--r--   0        0        0     6675 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/SIM.py
+-rw-r--r--   0        0        0     1688 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/SINAN.py
+-rw-r--r--   0        0        0    24411 2023-07-31 23:40:35.283189 pysus-0.9.4/pysus/online_data/__init__.py
+-rw-r--r--   0        0        0      790 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/online_data/sinasc.py
+-rw-r--r--   0        0        0     3677 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/online_data/vaccine.py
+-rw-r--r--   0        0        0     1922 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/preprocessing/ESUS.py
+-rw-r--r--   0        0        0     6289 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/preprocessing/SIM.py
+-rw-r--r--   0        0        0      128 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/preprocessing/__init__.py
+-rw-r--r--   0        0        0    10109 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/preprocessing/decoders.py
+-rw-r--r--   0        0        0     2402 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/preprocessing/geodata.py
+-rw-r--r--   0        0        0     3878 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/preprocessing/sinan.py
+-rw-r--r--   0        0        0      128 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/tests/__init__.py
+-rw-r--r--   0        0        0      505 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/tests/test_SIA.py
+-rw-r--r--   0        0        0      722 2023-07-31 23:40:35.287189 pysus-0.9.4/pysus/tests/test_cnes.py
+-rw-r--r--   0        0        0  9175254 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/EPR-2016-06-01-2016.dbf
+-rw-r--r--   0        0        0       66 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     3126 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_Infodengue.py
+-rw-r--r--   0        0        0      330 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_Infogripe.py
+-rw-r--r--   0        0        0      640 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_PNI.py
+-rw-r--r--   0        0        0      795 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_ciha.py
+-rw-r--r--   0        0        0     2265 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_sia.py
+-rw-r--r--   0        0        0      547 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_sih.py
+-rw-r--r--   0        0        0     1249 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_sim.py
+-rw-r--r--   0        0        0     4624 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_sinan.py
+-rw-r--r--   0        0        0      785 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_sinasc.py
+-rw-r--r--   0        0        0      419 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_data/test_vaccine.py
+-rw-r--r--   0        0        0     6975 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_decoders.py
+-rw-r--r--   0        0        0      304 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_esus.py
+-rw-r--r--   0        0        0     1382 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_ibge.py
+-rw-r--r--   0        0        0      741 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_init.py
+-rw-r--r--   0        0        0      642 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_sih.py
+-rw-r--r--   0        0        0     2123 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_sim.py
+-rw-r--r--   0        0        0      758 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/tests/test_utilities.py
+-rw-r--r--   0        0        0        0 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/utilities/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-31 23:40:35.315189 pysus-0.9.4/pysus/utilities/readdbc.py
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 pysus-0.9.4/PKG-INFO
```

### Comparing `pysus-0.9.3/LICENSE` & `pysus-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pyproject.toml` & `pysus-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "pysus"
-version = "0.9.3"  # changed by semantic-release
+version = "0.9.4"  # changed by semantic-release
 description = "Tools for dealing with Brazil's Public health data"
 authors = ["Flavio Codeco Coelho <fccoelho@gmail.com>"]
 license = "GPL"
 
 packages = [{include='pysus'}]
 
 [tool.poetry.dependencies]
 cffi = "1.15.1"
 dbfread = "2.0.7"
 fastparquet = "^0.8.1"
 geocoder = "^1.38.1"
 jupyterlab = "^3.4.5"
 numpy = "1.23.2"
-pandas = "1.4.3"
 pyarrow = ">=11.0.0"
 pycparser = "2.21"
 pyreaddbc = "1.0.0"
 python = "^3.9"
 python-dateutil = "2.8.2"
 pytz = "2022.2.1"
 six = "1.16.0"
 tqdm = "4.64.0"
 wget = "^3.2"
 loguru = "^0.6.0"
 Unidecode = "^1.3.6"
-sqlalchemy = "<2.0.0"
 elasticsearch = "7.16.2"
 ipykernel = "^6.22.0"
 geobr = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=6.1.0"
 black = "^22.6.0"
```

### Comparing `pysus-0.9.3/pysus/Notebooks/Analyzing SIH.ipynb` & `pysus-0.9.4/pysus/Notebooks/Analyzing SIH.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/Notebooks/Analyzing SIM.ipynb` & `pysus-0.9.4/pysus/Notebooks/Analyzing SIM.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/Notebooks/Analyzing SINASC Data.ipynb` & `pysus-0.9.4/pysus/Notebooks/Analyzing SINASC Data.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/Notebooks/Getting_CNES_Data.ipynb` & `pysus-0.9.4/pysus/Notebooks/Getting_CNES_Data.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/Notebooks/Processing SIM with municipality.ipynb` & `pysus-0.9.4/pysus/Notebooks/Processing SIM with municipality.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/Notebooks/Processing SIM.ipynb` & `pysus-0.9.4/pysus/Notebooks/Processing SIM.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/Notebooks/SINAN.ipynb` & `pysus-0.9.4/pysus/Notebooks/SINAN.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/dataset/geocode_by_cities.json` & `pysus-0.9.4/pysus/dataset/geocode_by_cities.json`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/ANIM.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/ANIM.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/BOTU.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/BOTU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/CHAG.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/CHAG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/CHIK.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/CHIK.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/COLE.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/COLE.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/COQU.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/COQU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/DENG.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/DENG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/DIFT.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/DIFT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/ESQU.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/ESQU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/FAMA.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/FAMA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/FMAC.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/FMAC.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/FTIF.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/FTIF.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/HANS.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/HANS.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/HANT.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/HANT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/HEPA.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/HEPA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/IEXO.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/IEXO.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/LEIV.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/LEIV.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/LEPT.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/LEPT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/LTAN.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/LTAN.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/MALA.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/MALA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/MENI.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/MENI.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/PEST.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/PEST.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/RAIV.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/RAIV.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/SIFC.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/SIFC.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/SIFG.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/SIFG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/TETA.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/TETA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/TETN.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/TETN.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/TUBE.tar.gz` & `pysus-0.9.4/pysus/metadata/SINAN/TUBE.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/metadata/SINAN/typecast.py` & `pysus-0.9.4/pysus/metadata/SINAN/typecast.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/CIHA.py` & `pysus-0.9.4/pysus/online_data/CIHA.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/CNES.py` & `pysus-0.9.4/pysus/online_data/CNES.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/ESUS.py` & `pysus-0.9.4/pysus/online_data/ESUS.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/IBGE.py` & `pysus-0.9.4/pysus/online_data/IBGE.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/Infodengue.py` & `pysus-0.9.4/pysus/online_data/Infodengue.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/Infogripe.py` & `pysus-0.9.4/pysus/online_data/Infogripe.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/PNI.py` & `pysus-0.9.4/pysus/online_data/PNI.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/SIA.py` & `pysus-0.9.4/pysus/online_data/SIA.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/SIH.py` & `pysus-0.9.4/pysus/online_data/SIH.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/SIM.py` & `pysus-0.9.4/pysus/online_data/SIM.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/SINAN.py` & `pysus-0.9.4/pysus/online_data/SINAN.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/__init__.py` & `pysus-0.9.4/pysus/online_data/__init__.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/sinasc.py` & `pysus-0.9.4/pysus/online_data/sinasc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/online_data/vaccine.py` & `pysus-0.9.4/pysus/online_data/vaccine.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/preprocessing/ESUS.py` & `pysus-0.9.4/pysus/preprocessing/ESUS.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/preprocessing/SIM.py` & `pysus-0.9.4/pysus/preprocessing/SIM.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/preprocessing/decoders.py` & `pysus-0.9.4/pysus/preprocessing/decoders.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/preprocessing/geodata.py` & `pysus-0.9.4/pysus/preprocessing/geodata.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/preprocessing/sinan.py` & `pysus-0.9.4/pysus/preprocessing/sinan.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_cnes.py` & `pysus-0.9.4/pysus/tests/test_cnes.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/EPR-2016-06-01-2016.dbf` & `pysus-0.9.4/pysus/tests/test_data/EPR-2016-06-01-2016.dbf`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_Infodengue.py` & `pysus-0.9.4/pysus/tests/test_data/test_Infodengue.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_PNI.py` & `pysus-0.9.4/pysus/tests/test_data/test_PNI.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_ciha.py` & `pysus-0.9.4/pysus/tests/test_data/test_ciha.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_sia.py` & `pysus-0.9.4/pysus/tests/test_data/test_sia.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_sih.py` & `pysus-0.9.4/pysus/tests/test_data/test_sih.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_sim.py` & `pysus-0.9.4/pysus/tests/test_data/test_sim.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_sinan.py` & `pysus-0.9.4/pysus/tests/test_data/test_sinan.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_data/test_sinasc.py` & `pysus-0.9.4/pysus/tests/test_data/test_sinasc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_decoders.py` & `pysus-0.9.4/pysus/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_ibge.py` & `pysus-0.9.4/pysus/tests/test_ibge.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_init.py` & `pysus-0.9.4/pysus/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_sih.py` & `pysus-0.9.4/pysus/tests/test_sih.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_sim.py` & `pysus-0.9.4/pysus/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/tests/test_utilities.py` & `pysus-0.9.4/pysus/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/pysus/utilities/readdbc.py` & `pysus-0.9.4/pysus/utilities/readdbc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.3/PKG-INFO` & `pysus-0.9.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysus
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tools for dealing with Brazil's Public health data
 License: GPL
 Author: Flavio Codeco Coelho
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -18,17 +18,15 @@
 Requires-Dist: fastparquet (>=0.8.1,<0.9.0)
 Requires-Dist: geobr (>=0.2.0,<0.3.0)
 Requires-Dist: geocoder (>=1.38.1,<2.0.0)
 Requires-Dist: ipykernel (>=6.22.0,<7.0.0)
 Requires-Dist: jupyterlab (>=3.4.5,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: numpy (==1.23.2)
-Requires-Dist: pandas (==1.4.3)
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pycparser (==2.21)
 Requires-Dist: pyreaddbc (==1.0.0)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: pytz (==2022.2.1)
 Requires-Dist: six (==1.16.0)
-Requires-Dist: sqlalchemy (<2.0.0)
 Requires-Dist: tqdm (==4.64.0)
 Requires-Dist: wget (>=3.2,<4.0)
```

