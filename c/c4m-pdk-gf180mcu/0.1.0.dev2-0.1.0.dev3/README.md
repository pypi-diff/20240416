# Comparing `tmp/c4m_pdk_gf180mcu-0.1.0.dev2.tar.gz` & `tmp/c4m_pdk_gf180mcu-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_gf180mcu-0.1.0.dev2.tar", last modified: Sun Jun 25 21:46:37 2023, max compression
+gzip compressed data, was "c4m_pdk_gf180mcu-0.1.0.dev3.tar", last modified: Tue Aug  8 14:51:35 2023, max compression
```

## Comparing `c4m_pdk_gf180mcu-0.1.0.dev2.tar` & `c4m_pdk_gf180mcu-0.1.0.dev3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.960172 c4m_pdk_gf180mcu-0.1.0.dev2/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      144 2023-03-20 17:55:59.000000 c4m_pdk_gf180mcu-0.1.0.dev2/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1227 2023-06-25 21:45:07.000000 c4m_pdk_gf180mcu-0.1.0.dev2/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2022-11-15 12:23:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/COPYRIGHT.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.948172 c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2022-11-15 12:23:59.000000 c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2022-11-15 12:23:59.000000 c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2022-11-15 12:23:59.000000 c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/gpl-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      138 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev2/MANIFEST.in
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3299 2023-06-25 21:46:37.960172 c4m_pdk_gf180mcu-0.1.0.dev2/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2825 2023-06-25 21:45:07.000000 c4m_pdk_gf180mcu-0.1.0.dev2/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.952172 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      163 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.952172 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      163 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.952172 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      212 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.952172 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      281 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/all.spice
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3173 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/design.ngspice
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)  1303098 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/sm141064.ngspice
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8045 2023-06-25 21:45:35.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/pdkmaster.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1193 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2158 2023-06-25 21:45:35.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/stdcell.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.956172 c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3299 2023-06-25 21:46:37.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1371 2023-06-25 21:46:37.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-25 21:46:37.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       53 2023-06-25 21:46:37.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-06-25 21:46:37.000000 c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1108 2023-06-25 21:45:07.000000 c4m_pdk_gf180mcu-0.1.0.dev2/cell_list.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    39537 2023-06-25 21:45:07.000000 c4m_pdk_gf180mcu-0.1.0.dev2/dodo.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       53 2023-04-20 11:17:51.000000 c4m_pdk_gf180mcu-0.1.0.dev2/env.sh
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.944172 c4m_pdk_gf180mcu-0.1.0.dev2/override/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.944172 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.956172 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      952 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/decap_w0.v
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      989 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/one_x1.v
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      993 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/zero_x1.v
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1033 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/zeroone_x1.v
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.956172 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      556 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/decap_w0.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      575 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/one_x1.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      580 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/zero_x1.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      614 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/zeroone_x1.vhdl
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.948172 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.956172 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      952 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/decap_w0.v
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      989 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/one_x1.v
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      993 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/zero_x1.v
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1033 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/zeroone_x1.v
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 21:46:37.960172 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      556 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/decap_w0.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      575 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/one_x1.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      580 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/zero_x1.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      614 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/zeroone_x1.vhdl
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-25 21:46:37.960172 c4m_pdk_gf180mcu-0.1.0.dev2/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1506 2023-06-25 21:45:07.000000 c4m_pdk_gf180mcu-0.1.0.dev2/setup.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.506818 c4m_pdk_gf180mcu-0.1.0.dev3/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      144 2023-03-20 17:55:59.000000 c4m_pdk_gf180mcu-0.1.0.dev3/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1227 2023-07-21 14:01:22.000000 c4m_pdk_gf180mcu-0.1.0.dev3/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2022-11-15 12:23:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/COPYRIGHT.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.466817 c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2022-11-15 12:23:59.000000 c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2022-11-15 12:23:59.000000 c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2022-11-15 12:23:59.000000 c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/gpl-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      138 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev3/MANIFEST.in
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3299 2023-08-08 14:51:35.506818 c4m_pdk_gf180mcu-0.1.0.dev3/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2825 2023-07-21 14:01:22.000000 c4m_pdk_gf180mcu-0.1.0.dev3/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.470818 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      163 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.470818 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      163 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.470818 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      212 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.474818 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      281 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/all.spice
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3173 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/design.ngspice
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)  1303098 2023-06-25 13:13:51.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/sm141064.ngspice
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8045 2023-07-21 14:01:22.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/pdkmaster.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1193 2023-06-25 12:57:24.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2254 2023-07-27 12:20:14.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/stdcell.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.498818 c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3299 2023-08-08 14:51:35.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1371 2023-08-08 14:51:35.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-08-08 14:51:35.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       54 2023-08-08 14:51:35.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-08-08 14:51:35.000000 c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1164 2023-08-08 14:37:37.000000 c4m_pdk_gf180mcu-0.1.0.dev3/cell_list.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    39537 2023-07-21 14:01:22.000000 c4m_pdk_gf180mcu-0.1.0.dev3/dodo.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       53 2023-04-20 11:17:51.000000 c4m_pdk_gf180mcu-0.1.0.dev3/env.sh
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.426817 c4m_pdk_gf180mcu-0.1.0.dev3/override/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.422817 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.502818 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      952 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/decap_w0.v
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      989 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/one_x1.v
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      993 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/zero_x1.v
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1033 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/zeroone_x1.v
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.502818 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      556 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/decap_w0.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      575 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/one_x1.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      580 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/zero_x1.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      614 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/zeroone_x1.vhdl
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.426817 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.502818 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      952 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/decap_w0.v
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      989 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/one_x1.v
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      993 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/zero_x1.v
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1033 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/zeroone_x1.v
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 14:51:35.506818 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      556 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/decap_w0.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      575 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/one_x1.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      580 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/zero_x1.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      614 2023-03-20 14:12:34.000000 c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/zeroone_x1.vhdl
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-08-08 14:51:35.506818 c4m_pdk_gf180mcu-0.1.0.dev3/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1507 2023-08-08 14:37:55.000000 c4m_pdk_gf180mcu-0.1.0.dev3/setup.py
```

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/.gitlab-ci.yml` & `c4m_pdk_gf180mcu-0.1.0.dev3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/LICENSE.md` & `c4m_pdk_gf180mcu-0.1.0.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/agpl-3.0.txt` & `c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/apache-2.0.txt` & `c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/cern_ohl_s_v2.txt` & `c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/LICENSES/gpl-2.0.txt` & `c4m_pdk_gf180mcu-0.1.0.dev3/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/PKG-INFO` & `c4m_pdk_gf180mcu-0.1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m_pdk_gf180mcu
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: gf180mcu as PDKMaster based PDK
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-pdk-gf180mcu
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-pdk-gf180mcu/issues
 Requires-Python: ~=3.6
```

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/README.md` & `c4m_pdk_gf180mcu-0.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/design.ngspice` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/design.ngspice`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/models/sm141064.ngspice` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/models/sm141064.ngspice`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/pdkmaster.py` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/pdkmaster.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/pyspice.py` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/pyspice.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m/pdk/gf180mcu/stdcell.py` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m/pdk/gf180mcu/stdcell.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             lib=lib, cktfab=cktfab, layoutfab=layoutfab,
             name_prefix=name_prefix, name_suffix=name_suffix,
             canvas=stdcell3v3canvas,
         )
 
 
 stdcell3v3canvas = _fab.StdCellCanvas(
-    tech=tech, lambda_=0.07,
+    tech=tech, **_fab.StdCellCanvas.compute_dimensions_lambda(lambda_=0.07),
     nmos=cast(_prm.MOSFET, prims.nfet_03v3), pmos=cast(_prm.MOSFET, prims.pfet_03v3),
 )
 stdcell3v3lib = _lbry.RoutingGaugeLibrary(
     name="StdCell3V3Lib", tech=tech, routinggauge=stdcell3v3canvas.routinggauge,
 )
 StdCell3V3Factory(lib=stdcell3v3lib).add_default()
 merge(stdcell3v3lib)
@@ -47,15 +47,15 @@
             lib=lib, cktfab=cktfab, layoutfab=layoutfab,
             name_prefix=name_prefix, name_suffix=name_suffix,
             canvas=stdcell5v0canvas,
         )
 
 
 stdcell5v0canvas = _fab.StdCellCanvas(
-    tech=tech, lambda_=0.07,
+    tech=tech, **_fab.StdCellCanvas.compute_dimensions_lambda(lambda_=0.07),
     nmos=cast(_prm.MOSFET, prims.nfet_05v0), pmos=cast(_prm.MOSFET, prims.pfet_05v0),
     l=0.6,
     inside=(cast(_prm.Insulator, prims.Dualgate), cast(_prm.Marker, prims.V5_XTOR)),
     inside_enclosure=(_prp.Enclosure(0.4), _prp.Enclosure(0.005)),
 )
 stdcell5v0lib = _lbry.RoutingGaugeLibrary(
     name="StdCell5V0Lib", tech=tech, routinggauge=stdcell5v0canvas.routinggauge,
```

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/PKG-INFO` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-gf180mcu
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: gf180mcu as PDKMaster based PDK
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-pdk-gf180mcu
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-pdk-gf180mcu/issues
 Requires-Python: ~=3.6
```

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/c4m_pdk_gf180mcu.egg-info/SOURCES.txt` & `c4m_pdk_gf180mcu-0.1.0.dev3/c4m_pdk_gf180mcu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/cell_list.yml` & `c4m_pdk_gf180mcu-0.1.0.dev3/cell_list.yml`

 * *Files 18% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 - nor4_x0
 - nor4_x1
 - or2_x1
 - or3_x1
 - or4_x1
 - mux2_x1
 - and21nor_x0
+- and21nor_x1
 - or21nand_x0
+- or21nand_x1
 - xor2_x0
 - nexor2_x0
 - nsnrlatch_x0
 - nsnrlatch_x1
 - dff_x1
 - dffnr_x1
 StdCell5V0Lib:
@@ -91,14 +93,16 @@
 - nor4_x0
 - nor4_x1
 - or2_x1
 - or3_x1
 - or4_x1
 - mux2_x1
 - and21nor_x0
+- and21nor_x1
 - or21nand_x0
+- or21nand_x1
 - xor2_x0
 - nexor2_x0
 - nsnrlatch_x0
 - nsnrlatch_x1
 - dff_x1
 - dffnr_x1
```

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/dodo.py` & `c4m_pdk_gf180mcu-0.1.0.dev3/dodo.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/decap_w0.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/decap_w0.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/one_x1.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/one_x1.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/zero_x1.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/zero_x1.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/verilog/zeroone_x1.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/verilog/zeroone_x1.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/decap_w0.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/decap_w0.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/one_x1.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/one_x1.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/zero_x1.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/zero_x1.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell3V3Lib/vhdl/zeroone_x1.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell3V3Lib/vhdl/zeroone_x1.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/decap_w0.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/decap_w0.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/one_x1.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/one_x1.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/zero_x1.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/zero_x1.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/verilog/zeroone_x1.v` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/verilog/zeroone_x1.v`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/decap_w0.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/decap_w0.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/one_x1.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/one_x1.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/zero_x1.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/zero_x1.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/override/StdCell5V0Lib/vhdl/zeroone_x1.vhdl` & `c4m_pdk_gf180mcu-0.1.0.dev3/override/StdCell5V0Lib/vhdl/zeroone_x1.vhdl`

 * *Files identical despite different names*

### Comparing `c4m_pdk_gf180mcu-0.1.0.dev2/setup.py` & `c4m_pdk_gf180mcu-0.1.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     description="gf180mcu as PDKMaster based PDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+",
     python_requires="~=3.6",
     setup_requires=["setuptools_scm"],
     install_requires=[
-        "setuptools", "PDKMaster~=0.9.3", "c4m-flexcell~=0.4.0.dev0",
+        "setuptools", "PDKMaster~=0.9.3", "c4m-flexcell~=0.4.0.dev23",
     ],
     include_package_data=True,
     packages=_packages,
     project_urls={
         #"Documentation": "???",
         "Source Code": "https://gitlab.com/Chips4Makers/c4m-pdk-gf180mcu",
         "Bug Tracker": "https://gitlab.com/Chips4Makers/c4m-pdk-gf180mcu/issues",
```

