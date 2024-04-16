# Comparing `tmp/ipi-2.6.0.tar.gz` & `tmp/ipi-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipi-2.6.0.tar", last modified: Thu Nov 30 22:40:13 2023, max compression
+gzip compressed data, was "ipi-2.6.3.tar", last modified: Tue Apr 16 07:33:19 2024, max compression
```

## Comparing `ipi-2.6.0.tar` & `ipi-2.6.3.tar`

### file list

```diff
@@ -1,187 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.149612 ipi-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-11-30 22:40:13.149612 ipi-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2023-11-30 22:40:03.000000 ipi-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.129612 ipi-2.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4024 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi
--rwxr-xr-x   0 runner    (1001) docker     (127)    10880 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-committee-reweight
--rwxr-xr-x   0 runner    (1001) docker     (127)     5193 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-contract-trajectory
--rwxr-xr-x   0 runner    (1001) docker     (127)     7176 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-get_Ascp
--rwxr-xr-x   0 runner    (1001) docker     (127)     7707 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-getacf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1918 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-getproperty
--rwxr-xr-x   0 runner    (1001) docker     (127)    12989 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-gleacf
--rwxr-xr-x   0 runner    (1001) docker     (127)     3499 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-kinetic2tag
--rwxr-xr-x   0 runner    (1001) docker     (127)     1383 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-mergebeadspdb
--rwxr-xr-x   0 runner    (1001) docker     (127)     4972 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-mux-positions
--rwxr-xr-x   0 runner    (1001) docker     (127)     9166 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-paraweights
--rwxr-xr-x   0 runner    (1001) docker     (127)    20066 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-planetary
--rwxr-xr-x   0 runner    (1001) docker     (127)     4625 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-posforce2kinetic
--rwxr-xr-x   0 runner    (1001) docker     (127)     6785 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-py_driver
--rwxr-xr-x   0 runner    (1001) docker     (127)    10017 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-remdsort
--rwxr-xr-x   0 runner    (1001) docker     (127)     3674 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-style
--rwxr-xr-x   0 runner    (1001) docker     (127)     1912 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-tests
--rwxr-xr-x   0 runner    (1001) docker     (127)     9247 2023-11-30 22:40:03.000000 ipi-2.6.0/bin/i-pi-trimsim
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.121612 ipi-2.6.0/drivers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.129612 ipi-2.6.0/drivers/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:03.000000 ipi-2.6.0/drivers/py/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6785 2023-11-30 22:40:03.000000 ipi-2.6.0/drivers/py/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.129612 ipi-2.6.0/drivers/py/pes/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-30 22:40:03.000000 ipi-2.6.0/drivers/py/pes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-30 22:40:03.000000 ipi-2.6.0/drivers/py/pes/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-30 22:40:03.000000 ipi-2.6.0/drivers/py/pes/harmonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-11-30 22:40:03.000000 ipi-2.6.0/drivers/py/pes/rascal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.129612 ipi-2.6.0/ipi/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.133612 ipi-2.6.0/ipi/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    49463 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/barostats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/beads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/cell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8818 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (127)    65557 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/forcefields.py
--rw-r--r--   0 runner    (1001) docker     (127)    57364 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/forces.py
--rw-r--r--   0 runner    (1001) docker     (127)    24989 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.133612 ipi-2.6.0/ipi/engine/motion/
--rwxr-xr-x   0 runner    (1001) docker     (127)      733 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26776 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/al6xxx_kmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/atomswap.py
--rw-r--r--   0 runner    (1001) docker     (127)    19035 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/constrained_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    28884 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/dynamics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35597 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/geop.py
--rw-r--r--   0 runner    (1001) docker     (127)    55134 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/instanton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)    40613 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/planetary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    33675 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/scphonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    60832 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/stringmep.py
--rw-r--r--   0 runner    (1001) docker     (127)    56436 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/motion/vscf.py
--rw-r--r--   0 runner    (1001) docker     (127)    34781 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/normalmodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    22634 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   124982 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    14626 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.137612 ipi-2.6.0/ipi/engine/smotion/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/smotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/smotion/dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/smotion/metad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/smotion/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/smotion/remd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/smotion/smotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    47982 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/engine/thermostats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.137612 ipi-2.6.0/ipi/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.137612 ipi-2.6.0/ipi/external/importlib/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/external/importlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/external/importlib/bundledimportlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.137612 ipi-2.6.0/ipi/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/barostats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/beads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (127)    33115 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/forcefields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/forces.py
--rw-r--r--   0 runner    (1001) docker     (127)    19179 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.141612 ipi-2.6.0/ipi/inputs/motion/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/al6xxx_kmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/atomswap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/constrained_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/geop.py
--rw-r--r--   0 runner    (1001) docker     (127)    12940 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/instanton.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15876 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/planetary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/scphonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10304 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/stringmep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/motion/vscf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/normalmodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/prng.py
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.141612 ipi-2.6.0/ipi/inputs/smotion/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/smotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/smotion/dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/smotion/metad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/smotion/remd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/smotion/smotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/inputs/thermostats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.141612 ipi-2.6.0/ipi/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31683 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/interfaces/sockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.145612 ipi-2.6.0/ipi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19240 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/constrtools.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    30563 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/depend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/hesstools.py
--rw-r--r--   0 runner    (1001) docker     (127)    49600 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/inputvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/instools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.145612 ipi-2.6.0/ipi/utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.145612 ipi-2.6.0/ipi/utils/io/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/backends/io_ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/backends/io_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/backends/io_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/backends/io_pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/backends/io_xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.145612 ipi-2.6.0/ipi/utils/io/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/inputs/io_xml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3853 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/io/io_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    52292 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/mintools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17257 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/nmtransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/phonontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/softexit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9798 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.149612 ipi-2.6.0/ipi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-11-30 22:40:13.000000 ipi-2.6.0/ipi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2023-11-30 22:40:13.000000 ipi-2.6.0/ipi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 22:40:13.000000 ipi-2.6.0/ipi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-30 22:40:13.000000 ipi-2.6.0/ipi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-30 22:40:13.000000 ipi-2.6.0/ipi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.149612 ipi-2.6.0/ipi_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.149612 ipi-2.6.0/ipi_tests/regression_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/runstools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.121612 ipi-2.6.0/ipi_tests/regression_tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.121612 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.121612 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.149612 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/files_to_check.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/init.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/input.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.frc_c.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.mom_c.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.out
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.pos_c.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.vel_c.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/test_settings.dat
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2023-11-30 22:40:03.000000 ipi-2.6.0/ipi_tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 22:40:13.149612 ipi-2.6.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2023-11-30 22:40:03.000000 ipi-2.6.0/licenses/license_GPL.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-30 22:40:03.000000 ipi-2.6.0/licenses/license_MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-30 22:40:03.000000 ipi-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-11-30 22:40:13.149612 ipi-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-30 22:40:03.000000 ipi-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.304335 ipi-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-16 07:33:19.304335 ipi-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-16 07:33:13.000000 ipi-2.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.280335 ipi-2.6.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4025 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10880 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-committee-reweight
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5193 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-contract-trajectory
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7206 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-driver-py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7176 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-get_Ascp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7707 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-getacf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1918 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-getproperty
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12989 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-gleacf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3499 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-kinetic2tag
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1383 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-mergebeadspdb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4972 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-mux-positions
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9166 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-paraweights
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20065 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-planetary
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4625 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-posforce2kinetic
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7206 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-py_driver
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10017 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-remdsort
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3674 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-style
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1924 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-tests
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9247 2024-04-16 07:33:13.000000 ipi-2.6.3/bin/i-pi-trimsim
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.276335 ipi-2.6.3/drivers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.280335 ipi-2.6.3/drivers/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7206 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.284335 ipi-2.6.3/drivers/py/pes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/bath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/doubledoublewell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/doublewell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/doublewell_with_bath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/doublewell_with_friction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/metatensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/pet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/rascal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-16 07:33:13.000000 ipi-2.6.3/drivers/py/pes/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.284335 ipi-2.6.3/ipi/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.288335 ipi-2.6.3/ipi/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49450 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/barostats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12128 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/beads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/cell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9149 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66126 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/forcefields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60035 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24867 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.292335 ipi-2.6.3/ipi/engine/motion/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      733 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26769 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/al6xxx_kmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/atomswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/constrained_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28677 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/dynamics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35583 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/geop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70739 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/instanton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40613 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/planetary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33628 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/scphonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60817 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/stringmep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56470 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/motion/vscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38618 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/normalmodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129875 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.292335 ipi-2.6.3/ipi/engine/smotion/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/smotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/smotion/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/smotion/metad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/smotion/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/smotion/remd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/smotion/smotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48870 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/engine/thermostats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.292335 ipi-2.6.3/ipi/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.292335 ipi-2.6.3/ipi/external/importlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/external/importlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/external/importlib/bundledimportlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.296335 ipi-2.6.3/ipi/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/barostats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/beads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34834 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/forcefields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.296335 ipi-2.6.3/ipi/inputs/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/al6xxx_kmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/atomswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/constrained_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/geop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/instanton.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15874 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/planetary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/scphonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/stringmep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/motion/vscf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/normalmodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.296335 ipi-2.6.3/ipi/inputs/smotion/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/smotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/smotion/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/smotion/metad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/smotion/remd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/smotion/smotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/inputs/thermostats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.296335 ipi-2.6.3/ipi/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35372 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/interfaces/sockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.300335 ipi-2.6.3/ipi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/constrtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27762 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/depend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/hesstools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49594 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/inputvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/instools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.300335 ipi-2.6.3/ipi/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.304335 ipi-2.6.3/ipi/utils/io/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/backends/io_ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/backends/io_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/backends/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/backends/io_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/backends/io_xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.304335 ipi-2.6.3/ipi/utils/io/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/inputs/io_xml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3850 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/io/io_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52258 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/mintools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/nmtransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/phonontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/softexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-16 07:33:13.000000 ipi-2.6.3/ipi/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.304335 ipi-2.6.3/ipi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-16 07:33:19.000000 ipi-2.6.3/ipi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-16 07:33:19.000000 ipi-2.6.3/ipi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:33:19.000000 ipi-2.6.3/ipi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 07:33:19.000000 ipi-2.6.3/ipi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-16 07:33:19.000000 ipi-2.6.3/ipi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:33:19.304335 ipi-2.6.3/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-16 07:33:13.000000 ipi-2.6.3/licenses/license_GPL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-16 07:33:13.000000 ipi-2.6.3/licenses/license_MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 07:33:13.000000 ipi-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 07:33:19.304335 ipi-2.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-16 07:33:13.000000 ipi-2.6.3/setup.py
```

### Comparing `ipi-2.6.0/PKG-INFO` & `ipi-2.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipi
-Version: 2.6.0
+Version: 2.6.3
 Summary: A Python interface for ab initio path integral molecular dynamics simulations
 Home-page: http://ipi-code.org
 Author: The i-PI developers
 Author-email: ipi.managers@gmail.com
 Project-URL: Documentation, https://ipi-code.org/i-pi
 Project-URL: Repository, https://github.com/i-pi/i-pi
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,49 +25,45 @@
 License-File: licenses/license_GPL.txt
 License-File: licenses/license_MIT.txt
 Requires-Dist: numpy
 
 i-PI: a Universal Force Engine
 ==============================
 
-A Python interface for ab initio path integral molecular dynamics simulations.
-i-PI is composed of a Python server (i-pi itself, that does not need to be
-compiled but only requires a relatively recent version of Python and Numpy)
-that apply an algorithm that updates the positions of the nuclei, and of an external
-code that acts as a client and computes the electronic energy and forces.
+A Python interface for ab initio path integral molecular dynamics simulations (and more).
+i-PI is a Python server (that does not need to be compiled and only requires a relatively 
+recent version of Python and Numpy) that applies an algorithm to update the positions of 
+the nuclei. One of many compatible external codes acts as client, and computes the 
+electronic energy and forces.
 
 This is typically a patched version of an electronic structure code, but a
 simple self-contained Fortran driver that implements several simple interatomic
 potentials is included for test purposes.
 
 i-PI was originally developed to simulate the quantum mechanical nature of light
 nuclei by performing path integral molecular dynamics simulations,
 and it implements most of the state-of-the-art methods to accelerate this kind of 
 calculations. It has since grown to also provide all sorts of simulation 
 strategies, from replica exchange to geometry optimization. 
 
-Quick Setup and Test
---------------------
+Quick Setup
+-----------
 
-To use i-PI with an existing driver, install and update using Pip:
+To use i-PI with an existing driver, install and update using `pip`:
+
+Last version:
 
-Last version::
 ```bash
 python -m pip install git+https://github.com/i-pi/i-pi.git
 ```
 
-Last Release::
-```bash
-pip install -U i-PI
-```
+Last Release:
 
-Test with Pytest::
 ```bash
-pip install pytest
-pytest --pyargs ipi.tests
+pip install -U ipi
 ```
 
 Full installation
 -----------------
 
 To develop i-PI or test it with the self-contained driver, follow these
 instructions. It is assumed that i-PI will
@@ -82,20 +78,25 @@
 Source the environment settings file `env.sh` as `source env.sh` or `.
 env.sh`.  It is useful to put this in your `.bashrc` or other settings file if
 you always want to have i-PI available.
 
 
 ### Compile the driver code
 
+The built-in driver requires a FORTRAN compiler, and can be built as
+
 ```bash
 cd drivers/f90
 make
 cd ../..
 ```
 
+There is also a Python driver available in `drivers/py`, which however has limited
+functionalities. 
+
 ### Examples and demos
 
 The `examples` and `demos` folders contain inputs for many different types of
 calculations based on i-PI. Examples are typically minimal use-cases of specific
 features, while demos are more structured, tutorial-like examples that show how
 to realize more complex setups, and also provide a brief discussion of the 
 underlying algorithms.
@@ -113,25 +114,26 @@
 i-pi-driver -h localhost -p 31415 -m sg -o 15 &
 i-pi-driver -h localhost -p 31415 -m sg -o 15 &
 tail -f log
 ```
 
 The monitoring can be interrupted with CTRL+C when the run has finished (5000 steps).
 
-
 ### Run the automatic test suite
 
-The automatic test suite can be run by calling the i-pi-test script.
+The automatic test suite can be run by calling the i-pi-tests script.
 You need to have the `pytest` package installed
 
 ```
-i-pi-test
+i-pi-tests
 ```
 
-See more details in the README file inside the ipi_tests folder.
+You may also need to install some dependencies, listed in `requirements.txt`.
+
+See more details in the README file inside the `ipi_tests` folder.
 
 Contributing
 ------------
 
 If you have new features you want to implement into i-PI, your contributions are much welcome.
 See `CONTRIBUTING.md` for a brief set of style guidelines and best practices. Before embarking
 into a substantial project, it might be good to get in touch with the developers, e.g. by opening
```

### Comparing `ipi-2.6.0/README.md` & `ipi-2.6.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 i-PI: a Universal Force Engine
 ==============================
 
-A Python interface for ab initio path integral molecular dynamics simulations.
-i-PI is composed of a Python server (i-pi itself, that does not need to be
-compiled but only requires a relatively recent version of Python and Numpy)
-that apply an algorithm that updates the positions of the nuclei, and of an external
-code that acts as a client and computes the electronic energy and forces.
+A Python interface for ab initio path integral molecular dynamics simulations (and more).
+i-PI is a Python server (that does not need to be compiled and only requires a relatively 
+recent version of Python and Numpy) that applies an algorithm to update the positions of 
+the nuclei. One of many compatible external codes acts as client, and computes the 
+electronic energy and forces.
 
 This is typically a patched version of an electronic structure code, but a
 simple self-contained Fortran driver that implements several simple interatomic
 potentials is included for test purposes.
 
 i-PI was originally developed to simulate the quantum mechanical nature of light
 nuclei by performing path integral molecular dynamics simulations,
 and it implements most of the state-of-the-art methods to accelerate this kind of 
 calculations. It has since grown to also provide all sorts of simulation 
 strategies, from replica exchange to geometry optimization. 
 
-Quick Setup and Test
---------------------
+Quick Setup
+-----------
 
-To use i-PI with an existing driver, install and update using Pip:
+To use i-PI with an existing driver, install and update using `pip`:
+
+Last version:
 
-Last version::
 ```bash
 python -m pip install git+https://github.com/i-pi/i-pi.git
 ```
 
-Last Release::
-```bash
-pip install -U i-PI
-```
+Last Release:
 
-Test with Pytest::
 ```bash
-pip install pytest
-pytest --pyargs ipi.tests
+pip install -U ipi
 ```
 
 Full installation
 -----------------
 
 To develop i-PI or test it with the self-contained driver, follow these
 instructions. It is assumed that i-PI will
@@ -54,20 +50,25 @@
 Source the environment settings file `env.sh` as `source env.sh` or `.
 env.sh`.  It is useful to put this in your `.bashrc` or other settings file if
 you always want to have i-PI available.
 
 
 ### Compile the driver code
 
+The built-in driver requires a FORTRAN compiler, and can be built as
+
 ```bash
 cd drivers/f90
 make
 cd ../..
 ```
 
+There is also a Python driver available in `drivers/py`, which however has limited
+functionalities. 
+
 ### Examples and demos
 
 The `examples` and `demos` folders contain inputs for many different types of
 calculations based on i-PI. Examples are typically minimal use-cases of specific
 features, while demos are more structured, tutorial-like examples that show how
 to realize more complex setups, and also provide a brief discussion of the 
 underlying algorithms.
@@ -85,25 +86,26 @@
 i-pi-driver -h localhost -p 31415 -m sg -o 15 &
 i-pi-driver -h localhost -p 31415 -m sg -o 15 &
 tail -f log
 ```
 
 The monitoring can be interrupted with CTRL+C when the run has finished (5000 steps).
 
-
 ### Run the automatic test suite
 
-The automatic test suite can be run by calling the i-pi-test script.
+The automatic test suite can be run by calling the i-pi-tests script.
 You need to have the `pytest` package installed
 
 ```
-i-pi-test
+i-pi-tests
 ```
 
-See more details in the README file inside the ipi_tests folder.
+You may also need to install some dependencies, listed in `requirements.txt`.
+
+See more details in the README file inside the `ipi_tests` folder.
 
 Contributing
 ------------
 
 If you have new features you want to implement into i-PI, your contributions are much welcome.
 See `CONTRIBUTING.md` for a brief set of style guidelines and best practices. Before embarking
 into a substantial project, it might be good to get in touch with the developers, e.g. by opening
```

### Comparing `ipi-2.6.0/bin/i-pi` & `ipi-2.6.3/bin/i-pi`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from ipi.utils.softexit import softexit
 from ipi.engine.simulation import Simulation
 
 def profile_exit(prefix="profile"):
     # write out the outputs of the profiler
     import yappi            
     yappi.stop()
-    yappi.get_thread_stats().print_all()
+    #yappi.get_thread_stats().print_all()
     yfs = yappi.get_func_stats()
     yfs.save(prefix+".kgrind", type="callgrind")
     ypo = open(prefix+".yappi", "w")
     yfs.print_all(out=ypo)
     ypo.close()
```

### Comparing `ipi-2.6.0/bin/i-pi-committee-reweight` & `ipi-2.6.3/bin/i-pi-committee-reweight`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-contract-trajectory` & `ipi-2.6.3/bin/i-pi-contract-trajectory`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-get_Ascp` & `ipi-2.6.3/bin/i-pi-get_Ascp`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-getacf` & `ipi-2.6.3/bin/i-pi-getacf`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-getproperty` & `ipi-2.6.3/bin/i-pi-getproperty`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-gleacf` & `ipi-2.6.3/bin/i-pi-gleacf`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-kinetic2tag` & `ipi-2.6.3/bin/i-pi-kinetic2tag`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-mergebeadspdb` & `ipi-2.6.3/bin/i-pi-mergebeadspdb`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-mux-positions` & `ipi-2.6.3/bin/i-pi-mux-positions`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-paraweights` & `ipi-2.6.3/bin/i-pi-paraweights`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-planetary` & `ipi-2.6.3/bin/i-pi-planetary`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
     return tcf
 
 
 # *******************************#
 
 
 class Planets(object):
-
     """
     Stores relevant trajectory info for planetary model simulation, calculates
     planetary dynamics and evaluates estimators and TCFs.
     """
 
     def __init__(
         self, prefix, natoms, iseed, npl, npts, stride, dt, temperature, estimators
```

### Comparing `ipi-2.6.0/bin/i-pi-posforce2kinetic` & `ipi-2.6.3/bin/i-pi-posforce2kinetic`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-py_driver` & `ipi-2.6.3/bin/i-pi-driver-py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import socket
 import argparse
 import numpy as np
 
+
 try:
     from pes import *
 except ImportError:
     # when in an installed i-PI package
     from ipi._driver.pes import *
 
 description = """
@@ -53,41 +54,45 @@
 def Message(mystr):
     """Returns a header of standard length HDRLEN."""
 
     # convert to bytestream since we'll be sending this over a socket
     return str.ljust(str.upper(mystr), HDRLEN).encode()
 
 
-def run_driver(unix=False, address="", port=12345, driver=Dummy_driver()):
+def run_driver(
+    unix=False, address="", port=12345, driver=Dummy_driver(), f_verbose=False
+):
     """Minimal socket client for i-PI."""
 
     # Opens a socket to i-PI
     if unix:
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.connect("/tmp/ipi_" + address)
     else:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        # this reduces latency for the small messages passed by the i-PI protocol
+        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         sock.connect((address, port))
 
     f_init = False
     f_data = False
-    f_verbose = False
 
     # initializes structure arrays
     cell = np.zeros((3, 3), float)
     icell = np.zeros((3, 3), float)
     pos = np.zeros(0, float)
 
     # initializes return arrays
     pot = 0.0
     force = np.zeros(0, float)
     vir = np.zeros((3, 3), float)
     while True:  # ah the infinite loop!
         header = sock.recv(HDRLEN)
-
+        if f_verbose:
+            print("Received ", header)
         if header == Message("STATUS"):
             # responds to a status request
             if not f_init:
                 sock.sendall(Message("NEEDINIT"))
             elif f_data:
                 sock.sendall(Message("HAVEDATA"))
             else:
@@ -196,23 +201,31 @@
         "-o",
         "--param",
         type=str,
         default="",
         help="""Parameters required to run the driver. Comma-separated list of values
         """,
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        default=False,
+        help="Verbose output.",
+    )
 
     args = parser.parse_args()
 
     if args.mode in __drivers__:
-        d_f = __drivers__[args.mode](args.param)
+        d_f = __drivers__[args.mode](args.param, args.verbose)
     elif args.mode == "dummy":
-        d_f = Dummy_driver(args.param)
+        d_f = Dummy_driver(args.param, args.verbose)
     else:
         raise ValueError("Unsupported driver mode ", args.mode)
 
     run_driver(
         unix=args.unix,
         address=args.address,
         port=args.port,
         driver=d_f,
+        f_verbose=args.verbose,
     )
```

### Comparing `ipi-2.6.0/bin/i-pi-remdsort` & `ipi-2.6.3/bin/i-pi-remdsort`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-style` & `ipi-2.6.3/bin/i-pi-style`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/bin/i-pi-tests` & `ipi-2.6.3/bin/i-pi-tests`

 * *Files 8% similar despite different names*

```diff
@@ -18,49 +18,49 @@
 )
 if dir_root not in sys.path:
     sys.path.insert(0, dir_root)
 
 main_folder = Path(__file__).resolve().parents[2] / "ipi_tests"
 test_folder = {
     "all": main_folder,
-    "example": main_folder / "examples",
+    "examples": main_folder / "examples",
     "regtests": main_folder / "regression_tests",
     "unit": main_folder / "unit_tests",
 }
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         formatter_class=RawTextHelpFormatter,
         description=""
         "Script that runs the tests provided with the code. \n"
         "\n"
         "If you want to run all the tests, \n"
         "type: i-pi-tests \n"
         "\n"
         "for running only the tests that checks the integrity of the examples inputs \n"
-        "type: i-pi-style -t example  \n"
+        "type: i-pi-tests -t examples  \n"
         "\n"
         "for running the regression tests  \n"
-        "type: i-pi-style -t regtests \n"
+        "type: i-pi-tests -t regtests \n"
         "\n"
         "and for running the unitary tests  \n"
-        "type: i-pi-style -t unit \n",
+        "type: i-pi-tests -t unit \n",
     )
 
     parser.add_argument(
         "-t",
         "--tests",
         type=str,
         default="all",
-        choices=["all", "example", "regtests", "unit"],
+        choices=["all", "examples", "regtests", "unit"],
         help="Specifies which tests are going to be called.",
     )
 
     args = parser.parse_args()
     tests = args.tests
     print(test_folder[args.tests])
     exit_code = pytest.main(
-        ["--tb=line", "-ra", "-vv", "-s", str(test_folder[args.tests])]
+        ["--tb=line", "--capture=no", "-ra", "-v", str(test_folder[args.tests])]
     )
 
     if exit_code != 0:
         raise RuntimeError("pytest exit code is {}".format(exit_code))
```

### Comparing `ipi-2.6.0/bin/i-pi-trimsim` & `ipi-2.6.3/bin/i-pi-trimsim`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/drivers/py/driver.py` & `ipi-2.6.3/bin/i-pi-py_driver`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import socket
 import argparse
 import numpy as np
 
+
 try:
     from pes import *
 except ImportError:
     # when in an installed i-PI package
     from ipi._driver.pes import *
 
 description = """
@@ -53,41 +54,45 @@
 def Message(mystr):
     """Returns a header of standard length HDRLEN."""
 
     # convert to bytestream since we'll be sending this over a socket
     return str.ljust(str.upper(mystr), HDRLEN).encode()
 
 
-def run_driver(unix=False, address="", port=12345, driver=Dummy_driver()):
+def run_driver(
+    unix=False, address="", port=12345, driver=Dummy_driver(), f_verbose=False
+):
     """Minimal socket client for i-PI."""
 
     # Opens a socket to i-PI
     if unix:
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.connect("/tmp/ipi_" + address)
     else:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        # this reduces latency for the small messages passed by the i-PI protocol
+        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         sock.connect((address, port))
 
     f_init = False
     f_data = False
-    f_verbose = False
 
     # initializes structure arrays
     cell = np.zeros((3, 3), float)
     icell = np.zeros((3, 3), float)
     pos = np.zeros(0, float)
 
     # initializes return arrays
     pot = 0.0
     force = np.zeros(0, float)
     vir = np.zeros((3, 3), float)
     while True:  # ah the infinite loop!
         header = sock.recv(HDRLEN)
-
+        if f_verbose:
+            print("Received ", header)
         if header == Message("STATUS"):
             # responds to a status request
             if not f_init:
                 sock.sendall(Message("NEEDINIT"))
             elif f_data:
                 sock.sendall(Message("HAVEDATA"))
             else:
@@ -196,23 +201,31 @@
         "-o",
         "--param",
         type=str,
         default="",
         help="""Parameters required to run the driver. Comma-separated list of values
         """,
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        default=False,
+        help="Verbose output.",
+    )
 
     args = parser.parse_args()
 
     if args.mode in __drivers__:
-        d_f = __drivers__[args.mode](args.param)
+        d_f = __drivers__[args.mode](args.param, args.verbose)
     elif args.mode == "dummy":
-        d_f = Dummy_driver(args.param)
+        d_f = Dummy_driver(args.param, args.verbose)
     else:
         raise ValueError("Unsupported driver mode ", args.mode)
 
     run_driver(
         unix=args.unix,
         address=args.address,
         port=args.port,
         driver=d_f,
+        f_verbose=args.verbose,
     )
```

### Comparing `ipi-2.6.0/drivers/py/pes/dummy.py` & `ipi-2.6.3/drivers/py/pes/dummy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+# this is how the driver will be referred to in the input files
+__DRIVER_NAME__ = "dummy"
+__DRIVER_CLASS__ = "Dummy_driver"
+
+
 class Dummy_driver(object):
-    def __init__(self, args=None):
+    """Base class providing the structure of a PES for the python driver."""
+
+    def __init__(
+        self, args="", verbose=False, error_msg="Invalid arguments for the PES"
+    ):
         """Initialized dummy drivers"""
-        self.args = args
+        self.error_msg = error_msg
+        self.args = args.split(",")
+        self.verbose = verbose
         self.check_arguments()
 
     def check_arguments(self):
         """Dummy function that checks the arguments required to run the driver"""
         pass
 
     def __call__(self, cell, pos):
```

### Comparing `ipi-2.6.0/drivers/py/pes/rascal.py` & `ipi-2.6.3/drivers/py/pes/rascal.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,37 @@
 from ipi.utils.units import unit_to_internal, unit_to_user
 
 try:
     from rascal.models.genericmd import GenericMDCalculator as RascalCalc
 except:
     RascalCalc = None
 
+__DRIVER_NAME__ = "rascal"
+__DRIVER_CLASS__ = "Rascal_driver"
+
+ERROR_MSG = """
+Rascal driver requires specification of a .json model file fitted with librascal, 
+and a template file that describes the chemical makeup of the structure. 
+Example: python driver.py -m rascal -u -o model.json,template.xyz
+"""
 
-class Rascal_driver(Dummy_driver):
-    def __init__(self, args=None):
-        self.error_msg = """Rascal driver requires specification of a .json model file fitted with librascal, 
-                            and a template file that describes the chemical makeup of the structure. 
-                            Example: python driver.py -m rascal -u -o model.json,template.xyz"""
 
-        super().__init__(args)
+class Rascal_driver(Dummy_driver):
+    def __init__(self, args=None, verbose=False):
+        super().__init__(args, verbose, error_msg=ERROR_MSG)
 
         if RascalCalc is None:
             raise ImportError("Couldn't load librascal bindings")
 
     def check_arguments(self):
         """Check the arguments required to run the driver
 
         This loads the potential and atoms template in librascal
         """
-        try:
-            arglist = self.args.split(",")
-        except ValueError:
-            sys.exit(self.error_msg)
+        arglist = self.args
 
         if len(arglist) == 2:
             self.model = arglist[0]
             self.template = arglist[1]
         else:
             sys.exit(self.error_msg)
```

### Comparing `ipi-2.6.0/ipi/engine/atoms.py` & `ipi-2.6.3/ipi/engine/atoms.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 from ipi.utils.depend import *
 
 
 __all__ = ["Atoms", "Atom"]
 
 
-class Atom(dobject):
-
+class Atom:
     """Represent an atom, with position, velocity, mass and related properties.
 
     This is actually only an interface to the Atoms class, i.e. only stores
     views of the large arrays which contain all the coordinates.
 
     Attributes:
        kin: The kinetic energy of the atom.
@@ -42,21 +41,20 @@
         """Initialises Atom.
 
         Args:
            system: An Atoms object containing the required atom.
            index: An integer giving the index of the required atom in the atoms
               list. Note that indices start from 0.
         """
-        dself = dd(self)  # direct access
 
-        dself.p = system.p[3 * index : 3 * index + 3]
-        dself.q = system.q[3 * index : 3 * index + 3]
-        dself.m = system.m[index : index + 1]
-        dself.name = system.names[index : index + 1]
-        dself.m3 = system.m3[3 * index : 3 * index + 3]
+        self.p = system.p[3 * index : 3 * index + 3]
+        self.q = system.q[3 * index : 3 * index + 3]
+        self.m = system.m[index : index + 1]
+        self.name = system.names[index : index + 1]
+        self.m3 = system.m3[3 * index : 3 * index + 3]
 
     @property
     def kin(self):
         """Calculates the contribution of the atom to the kinetic energy."""
 
         return np.dot(self.p, self.p) / (2.0 * self.m)
 
@@ -70,16 +68,18 @@
         ks = np.zeros((3, 3), float)
         for i in range(3):
             for j in range(i, 3):
                 ks[i, j] = p[i] * p[j]
         return ks / self.m
 
 
-class Atoms(dobject):
+# dproperties(Atom, ["p", "q", "m", "m3", "name"])
+
 
+class Atoms:
     """Storage for the atoms' positions, masses and velocities.
 
     Everything is stored as 3*n sized contiguous arrays,
     and a convenience-access is provided through a list of Atom objects.
 
     Attributes:
        natoms: The number of atoms.
@@ -116,42 +116,40 @@
            _prebind: An optional tuple of four elements; a depend_array of length
               3*natoms for the positions, another for the momenta, a depend_array
               of length natoms for the masses and another for the names.
         """
 
         self.natoms = natoms
 
-        dself = dd(self)  # direct access
-
         if _prebind is None:
-            dself.q = depend_array(name="q", value=np.zeros(3 * natoms, float))
-            dself.p = depend_array(name="p", value=np.zeros(3 * natoms, float))
-            dself.m = depend_array(name="m", value=np.zeros(natoms, float))
-            dself.names = depend_array(
+            self._q = depend_array(name="q", value=np.zeros(3 * natoms, float))
+            self._p = depend_array(name="p", value=np.zeros(3 * natoms, float))
+            self._m = depend_array(name="m", value=np.zeros(natoms, float))
+            self._names = depend_array(
                 name="names", value=np.zeros(natoms, np.dtype("|U6"))
             )
         else:
-            dself.q = _prebind[0]
-            dself.p = _prebind[1]
-            dself.m = _prebind[2]
-            dself.names = _prebind[3]
+            self._q = _prebind[0]
+            self._p = _prebind[1]
+            self._m = _prebind[2]
+            self._names = _prebind[3]
 
-        dself.m3 = depend_array(
+        self._m3 = depend_array(
             name="m3",
             value=np.zeros(3 * natoms, float),
             func=self.mtom3,
-            dependencies=[dself.m],
+            dependencies=[self._m],
         )
 
-        dself.M = depend_value(name="M", func=self.get_msum, dependencies=[dself.m])
-        dself.kin = depend_value(
-            name="kin", func=self.get_kin, dependencies=[dself.p, dself.m3]
+        self._M = depend_value(name="M", func=self.get_msum, dependencies=[self._m])
+        self._kin = depend_value(
+            name="kin", func=self.get_kin, dependencies=[self._p, self._m3]
         )
-        dself.kstress = depend_value(
-            name="kstress", func=self.get_kstress, dependencies=[dself.p, dself.m]
+        self._kstress = depend_value(
+            name="kstress", func=self.get_kstress, dependencies=[self._p, self._m]
         )
 
     def copy(self):
         """Creates a new Atoms object.
 
         Returns:
            An Atoms object with the same q, p, m and names arrays as the original.
@@ -267,7 +265,10 @@
         ks[0, 0] = np.dot(px, px / m)
         ks[1, 1] = np.dot(py, py / m)
         ks[2, 2] = np.dot(pz, pz / m)
         ks[0, 1] = np.dot(px, py / m)
         ks[0, 2] = np.dot(px, pz / m)
         ks[1, 2] = np.dot(py, pz / m)
         return ks
+
+
+dproperties(Atoms, ["p", "q", "m", "m3", "names", "M", "kin", "kstress"])
```

### Comparing `ipi-2.6.0/ipi/engine/barostats.py` & `ipi-2.6.3/ipi/engine/barostats.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             for i in m2f[f]:
                 hmask[i] = 0
         else:
             hmask[m2f[f]] = 0
     return hmask
 
 
-class Barostat(dobject):
+class Barostat:
     """Base barostat class.
 
     Gives the standard methods and attributes needed in all the barostat classes.
 
     Used as barostat for mode "dummy".
 
     Attributes:
@@ -107,47 +107,46 @@
               Defaults to the simulation temp.
            tau: Optional float giving the time scale associated with the barostat.
            ebaro: Optional float giving the conserved quantity already stored
               in the barostat initially. Used on restart.
            thermostat: The thermostat connected to the barostat degree of freedom.
         """
 
-        dself = dd(self)
-        dself.dt = depend_value(name="dt")
+        self._dt = depend_value(name="dt")
         if dt is not None:
             self.dt = dt
         else:
             self.dt = 1.0
 
-        dself.temp = depend_value(name="temp")
+        self._temp = depend_value(name="temp")
         if temp is not None:
             self.temp = temp
         else:
             self.temp = 1.0
 
-        dself.tau = depend_value(name="tau")
+        self._tau = depend_value(name="tau")
         if tau is not None:
             self.tau = tau
         else:
             self.tau = 1.0
 
-        dself.ebaro = depend_value(name="ebaro")
+        self._ebaro = depend_value(name="ebaro")
         if ebaro is not None:
             self.ebaro = ebaro
         else:
             self.ebaro = 0.0
 
         if thermostat is None:
             thermostat = Thermostat()
         self.thermostat = thermostat
 
         # temperature to the thermostat
-        dpipe(dself.temp, dd(self.thermostat).temp)
-        dself.pext = depend_value(name="pext", value=-1.0)
-        dself.stressext = depend_array(name="stressext", value=-np.ones((3, 3), float))
+        dpipe(self._temp, self.thermostat._temp)
+        self._pext = depend_value(name="pext", value=-1.0)
+        self._stressext = depend_array(name="stressext", value=-np.ones((3, 3), float))
 
     def bind(self, beads, nm, cell, forces, bias=None, prng=None, fixdof=None, nmts=1):
         """Binds beads, cell and forces to the barostat.
 
         This takes a beads object, a cell object and a forcefield object and
         makes them members of the barostat. It also then creates the objects that
         will hold the data needed in the barostat algorithms and the dependency
@@ -165,67 +164,65 @@
 
         self.beads = beads
         self.cell = cell
         self.forces = forces
         self.bias = bias
         self.nm = nm
 
-        dself = dd(self)
-
-        dself.kstress = depend_value(
+        self._kstress = depend_value(
             name="kstress",
             func=self.get_kstress,
-            dependencies=[dd(beads).q, dd(beads).qc, dd(beads).pc, dd(forces).f],
+            dependencies=[beads._q, beads._qc, beads._pc, forces._f],
         )
-        dself.stress = depend_value(
+        self._stress = depend_value(
             name="stress",
             func=self.get_stress,
-            dependencies=[dself.kstress, dd(cell).V, dd(forces).vir],
+            dependencies=[self._kstress, cell._V, forces._vir],
         )
 
-        dself.pot = depend_value(name="pot", value=0.0)
+        self._pot = depend_value(name="pot", value=0.0)
 
-        dself.kin = depend_value(name="kin", value=0.0)
+        self._kin = depend_value(name="kin", value=0.0)
 
-        dself.cell_jacobian = depend_value(name="kin", value=0.0)
+        self._cell_jacobian = depend_value(name="kin", value=0.0)
 
         # Stress depend objects for Suzuki-Chin PIMD
-        dself.kstress_sc = depend_value(
+        self._kstress_sc = depend_value(
             name="kstress_sc",
             func=self.get_kstress_sc,
             dependencies=[
-                dd(beads).q,
-                dd(beads).qc,
-                dd(forces).fsc_part_2,
-                dd(forces).f,
+                beads._q,
+                beads._qc,
+                forces._fsc_part_2,
+                forces._f,
             ],
         )
 
-        dself.stress_sc = depend_value(
+        self._stress_sc = depend_value(
             name="stress_sc",
             func=self.get_stress_sc,
             dependencies=[
-                dself.kstress_sc,
-                dd(self.cell).V,
-                dd(forces).vir,
-                dd(forces).virssc_part_2,
+                self._kstress_sc,
+                self.cell._V,
+                forces._vir,
+                forces._virssc_part_2,
             ],
         )
 
         if fixdof is None:
             self.mdof = float(self.beads.natoms) * 3.0
         else:
             self.mdof = float(self.beads.natoms) * 3.0 - float(fixdof)
 
         # creates and connects timesteps for the different parts of the propagator
         self.nmtslevels = nmts
-        dself.qdt = depend_value(name="qdt", value=self.dt)
-        dself.pdt = depend_array(name="pdt", value=np.zeros(nmts, float))
-        dself.tdt = depend_value(name="tdt", value=self.dt)
-        dpipe(dself.tdt, dd(self.thermostat).dt)
+        self._qdt = depend_value(name="qdt", value=self.dt)
+        self._pdt = depend_array(name="pdt", value=np.zeros(nmts, float))
+        self._tdt = depend_value(name="tdt", value=self.dt)
+        dpipe(self._tdt, self.thermostat._dt)
 
     # THESE SHOULD NOT BE USED ANYMORE
     def get_kstress(self):
         """Calculates the quantum centroid virial kinetic stress tensor
         estimator.
         """
 
@@ -262,15 +259,17 @@
 
         kst = np.zeros((3, 3), float)
         q = dstrip(self.beads.q)
         qc = dstrip(self.beads.qc)
         pc = dstrip(self.beads.pc)
         m = dstrip(self.beads.m)
         na3 = 3 * self.beads.natoms
-        fall = dstrip(self.forces.forces_mts(level)) * (1 + self.forces.coeffsc_part_1)
+        fall = dstrip(self.forces.mts_forces[level].f) * (
+            1 + self.forces.coeffsc_part_1
+        )
         if self.bias is None or level != 0:
             ball = fall * 0.00
         else:
             ball = dstrip(self.bias.f)
 
         for b in range(self.beads.nbeads):
             for i in range(3):
@@ -286,50 +285,49 @@
         return kst
 
     def kstress_mts(self, level):
         """Calculates the quantum centroid virial kinetic stress tensor
         associated with the forces at a MTS level.
         """
 
-        kst = np.zeros((3, 3), float)
-        q = dstrip(self.beads.q)
-        qc = dstrip(self.beads.qc)
-        pc = dstrip(self.beads.pc)
-        m = dstrip(self.beads.m)
-        na3 = 3 * self.beads.natoms
-        fall = dstrip(self.forces.forces_mts(level))
-        if self.bias is None or level != 0:
-            ball = fall * 0.00
-        else:
-            ball = dstrip(self.bias.f)
-
-        for b in range(self.beads.nbeads):
-            for i in range(3):
-                for j in range(i, 3):
-                    kst[i, j] -= np.dot(
-                        q[b, i:na3:3] - qc[i:na3:3], fall[b, j:na3:3] + ball[b, j:na3:3]
-                    )
+        fall = dstrip(self.forces.mts_forces[level].f)
+        if level == 0 and self.bias is not None:
+            # adds the bias. NB: don't += we don't want to overwrite the force
+            fall = fall + dstrip(self.bias.f)
+
+        beads = self.beads
+        qqc = (dstrip(beads.q) - dstrip(beads.qc)).reshape(-1, 3)
+        fall = fall.reshape(-1, 3)
+
+        kst = -noddot(qqc.T, fall)
+        # kst = np.zeros((3,3))
+        # kst[0] = -noddot(qqc[:,0], fall)
+        # kst[1,1:] = -noddot(qqc[:,1], fall[:,1:])
+        # kst[2,2] = -noddot(qqc[:,2], fall[:,2])
 
         if level == self.nmtslevels - 1:
-            for i in range(3):
-                kst[i, i] += np.dot(pc[i:na3:3], pc[i:na3:3] / m) * self.beads.nbeads
+            pc = dstrip(beads.pc).reshape(-1, 3)
+            m = dstrip(beads.m)
+            nbeads = beads.nbeads
+
+            kst[0, 0] += noddot(pc[:, 0], pc[:, 0] / m) * nbeads
+            kst[1, 1] += noddot(pc[:, 1], pc[:, 1] / m) * nbeads
+            kst[2, 2] += noddot(pc[:, 2], pc[:, 2] / m) * nbeads
 
         return kst
 
     def get_kstress_sc(self):
         """Calculates the high order part of the Suzuki-Chin
         quantum centroid virial kinetic stress tensor
         associated with the forces at a MTS level.
         """
 
         kst = np.zeros((3, 3), float)
         q = dstrip(self.beads.q)
         qc = dstrip(self.beads.qc)
-        # pc = dstrip(self.beads.pc)
-        # m = dstrip(self.beads.m)
         na3 = 3 * self.beads.natoms
         fall = dstrip(self.forces.fsc_part_2)
 
         for b in range(self.beads.nbeads):
             for i in range(3):
                 for j in range(i, 3):
                     kst[i, j] -= np.dot(q[b, i:na3:3] - qc[i:na3:3], fall[b, j:na3:3])
@@ -358,15 +356,15 @@
         bvir = np.zeros((3, 3), float)
         if self.bias is not None and level == 0:
             bvir[:] = self.bias.vir
 
         return (
             self.kstress_mts_sc(level)
             + np.sum(
-                self.forces.virs_mts(level)
+                self.forces.mts_forces[level].virs
                 * (1 + self.forces.coeffsc_part_1).reshape((self.beads.nbeads, 1, 1)),
                 axis=0,
             )
             + bvir
         ) / self.cell.V
 
     def stress_mts(self, level):
@@ -375,28 +373,51 @@
         """
 
         bvir = np.zeros((3, 3), float)
         if self.bias is not None and level == 0:
             bvir[:] = self.bias.vir
 
         return (
-            self.kstress_mts(level) + self.forces.vir_mts(level) + bvir
+            self.kstress_mts(level) + self.forces.mts_forces[level].vir + bvir
         ) / self.cell.V
 
     def pstep(self, level=0):
         """Dummy momenta propagator step."""
 
         pass
 
     def qcstep(self, level=0):
         """Dummy centroid position propagator step."""
 
         pass
 
 
+dproperties(
+    Barostat,
+    [
+        "dt",
+        "temp",
+        "tau",
+        "ebaro",
+        "pext",
+        "stressext",
+        "kstress",
+        "stress",
+        "pot",
+        "kin",
+        "cell_jacobian",
+        "kstress_sc",
+        "stress_sc",
+        "qdt",
+        "pdt",
+        "tdt",
+    ],
+)
+
+
 class BaroBZP(Barostat):
     """Bussi-Zykova-Parrinello barostat class.
 
     Mode "isotropic" implements the Bussi-Zykova-Parrinello barostat.
 
     Isotropically scales the unit cell volume while sampling the
     isothermal isobaric ensemble.
@@ -438,16 +459,15 @@
               in the barostat initially. Used on restart.
            thermostat: The thermostat connected to the barostat degree of freedom.
            p: Optional initial volume conjugate momentum. Defaults to 0.
         """
 
         super(BaroBZP, self).__init__(dt, temp, tau, ebaro, thermostat)
 
-        dself = dd(self)  # direct access
-        dself.p = depend_array(name="p", value=np.atleast_1d(0.0))
+        self._p = depend_array(name="p", value=np.atleast_1d(0.0))
 
         if p is not None:
             self.p = np.asarray([p])
         else:
             self.p = 0.0
 
         if pext is not None:
@@ -470,60 +490,59 @@
            forces: The forcefield object from which the force and virial are
               taken.
            prng: The parent PRNG to bind the thermostat to
            fixdof: The number of blocked degrees of freedom.
         """
 
         super(BaroBZP, self).bind(beads, nm, cell, forces, bias, prng, fixdof, nmts)
-        dself = dd(self)
 
         # obtain the thermostat mass from the given time constant
         # note that the barostat temperature is nbeads times the physical T
-        dself.m = depend_array(
+        self._m = depend_array(
             name="m",
             value=np.atleast_1d(0.0),
             func=(
                 lambda: np.asarray(
                     [self.tau**2 * 3 * self.beads.natoms * Constants.kb * self.temp]
                 )
             ),
-            dependencies=[dself.tau, dself.temp],
+            dependencies=[self._tau, self._temp],
         )
 
         # binds the thermostat to the piston degrees of freedom
         self.thermostat.bind(pm=[self.p, self.m], prng=prng)
 
         # barostat elastic energy
-        dself.pot = depend_value(
-            name="pot", func=self.get_pot, dependencies=[dd(cell).V, dself.pext]
+        self._pot = depend_value(
+            name="pot", func=self.get_pot, dependencies=[cell._V, self._pext]
         )
 
-        dself.kin = depend_value(
+        self._kin = depend_value(
             name="kin",
             func=(lambda: 0.5 * self.p[0] ** 2 / self.m[0]),
-            dependencies=[dself.p, dself.m],
+            dependencies=[self._p, self._m],
         )
 
         # defines the term that accounts for the explicit dependence of the volume on the ensemble
-        dself.cell_jacobian = depend_value(
+        self._cell_jacobian = depend_value(
             name="cell_jacobian",
             func=self.get_cell_jacobian,
-            dependencies=[dd(self.cell).V, dself.temp],
+            dependencies=[self.cell._V, self._temp],
         )
 
         # the barostat energy must be computed from bits & pieces (overwrite the default)
-        dself.ebaro = depend_value(
+        self._ebaro = depend_value(
             name="ebaro",
             func=self.get_ebaro,
             dependencies=[
-                dself.kin,
-                dself.pot,
-                dd(self.cell).V,
-                dself.temp,
-                dd(self.thermostat).ethermo,
+                self._kin,
+                self._pot,
+                self.cell._V,
+                self._temp,
+                self.thermostat._ethermo,
             ],
         )
 
     def get_pot(self):
         """Calculates the elastic strain energy of the cell."""
 
         # NOTE: since there are nbeads replicas of the unit cell, the enthalpy contains a nbeads factor
@@ -542,64 +561,62 @@
     def pstep(self, level=0):
         """Propagates the momentum of the barostat."""
 
         # we are assuming then that p the coupling between p^2 and dp/dt only involves the fast force
         dt = self.pdt[
             level
         ]  # this is already set to be half a time step at the specified MTS depth
-        dt2 = dt**2
-        dt3 = dt**3 / 3.0
 
         # computes the pressure associated with the forces at each MTS level.
         press = np.trace(self.stress_mts(level)) / 3.0
         self.p += dt * 3.0 * (self.cell.V * press)
 
         # integerates the kinetic part of the pressure with the force at the inner-most level.
         if level == self.nmtslevels - 1:
+            nbeads = self.beads.nbeads
             press = 0
             self.p += (
-                dt
-                * 3.0
+                3.0
+                * dt
                 * (
-                    self.cell.V * (press - self.beads.nbeads * self.pext)
+                    self.cell.V * (press - nbeads * self.pext)
                     + Constants.kb * self.temp
                 )
             )
 
             pc = dstrip(self.beads.pc)
-            fc = (
-                np.sum(dstrip(self.forces.forces_mts(level)), axis=0)
-                / self.beads.nbeads
-            )
-            m = dstrip(self.beads.m3)[0]
+            fc = np.sum(dstrip(self.forces.mts_forces[level].f), axis=0) / nbeads
+            fc_m = fc / dstrip(self.beads.m3)[0]
 
-            self.p += (
-                dt2 * np.dot(pc, fc / m) + dt3 * np.dot(fc, fc / m)
-            ) * self.beads.nbeads
+            dt2 = dt * dt * self.beads.nbeads
+            dt3 = dt / 3.0
+            self.p += (noddot(pc, fc_m) + dt3 * noddot(fc, fc_m)) * dt2
 
     def qcstep(self):
         """Propagates the centroid position and momentum and the volume."""
 
         v = self.p[0] / self.m[0]
         halfdt = (
             self.qdt
         )  # this is set to half the inner loop in all integrators that use a barostat
         expq, expp = (np.exp(v * halfdt), np.exp(-v * halfdt))
 
         m = dstrip(self.beads.m3)[0]
 
-        self.nm.qnm[0, :] *= expq
-        self.nm.qnm[0, :] += ((expq - expp) / (2.0 * v)) * (
-            dstrip(self.nm.pnm)[0, :] / m
-        )
-        self.nm.pnm[0, :] *= expp
+        self.nm.qnm[0, :] = (dstrip(self.nm.qnm)[0, :] * expq) + (
+            (expq - expp) / (2.0 * v)
+        ) * (dstrip(self.nm.pnm)[0, :] / m)
+        self.nm.pnm[0, :] = expp * dstrip(self.nm.pnm)[0, :]
 
         self.cell.h *= expq
 
 
+dproperties(BaroBZP, ["p", "m"])
+
+
 class BaroSCBZP(Barostat):
     """The Suzuki Chin Bussi-Zykova-Parrinello barostat class.
 
     Mode "sc-isotropic" implements the Bussi-Zykova-Parrinello
     barostat for Suzuki-Chin path integral molecular dynamics.
 
     Isotropically scales the unit cell volume while sampling the
@@ -643,17 +660,16 @@
            ebaro: Optional float giving the conserved quantity already stored
               in the barostat initially. Used on restart.
            thermostat: The thermostat connected to the barostat degree of freedom.
            p: Optional initial volume conjugate momentum. Defaults to 0.
         """
 
         super(BaroSCBZP, self).__init__(dt, temp, tau, ebaro, thermostat)
-        dself = dd(self)
 
-        dself.p = depend_array(name="p", value=np.atleast_1d(0.0))
+        self._p = depend_array(name="p", value=np.atleast_1d(0.0))
 
         if p is not None:
             self.p = np.asarray([p])
         else:
             self.p = 0.0
 
         if pext is not None:
@@ -676,58 +692,57 @@
            forces: The forcefield object from which the force and virial are
               taken.
            prng: The parent PRNG to bind the thermostat to
            fixdof: The number of blocked degrees of freedom.
         """
 
         super(BaroSCBZP, self).bind(beads, nm, cell, forces, bias, prng, fixdof, nmts)
-        dself = dd(self)
 
         # obtain the thermostat mass from the given time constant
-        dself.m = depend_array(
+        self._m = depend_array(
             name="m",
             value=np.atleast_1d(0.0),
             func=(
                 lambda: np.asarray(
                     [self.tau**2 * 3 * self.beads.natoms * Constants.kb * self.temp]
                 )
             ),
-            dependencies=[dself.tau, dself.temp],
+            dependencies=[self._tau, self._temp],
         )
 
         # binds the thermostat to the piston degrees of freedom
         self.thermostat.bind(pm=[self.p, self.m], prng=prng)
 
         # barostat elastic energy
-        dself.pot = depend_value(
-            name="pot", func=self.get_pot, dependencies=[dd(cell).V, dself.pext]
+        self._pot = depend_value(
+            name="pot", func=self.get_pot, dependencies=[cell._V, self._pext]
         )
 
-        dself.kin = depend_value(
+        self._kin = depend_value(
             name="kin",
             func=(lambda: 0.5 * self.p[0] ** 2 / self.m[0]),
-            dependencies=[dself.p, dself.m],
+            dependencies=[self._p, self._m],
         )
 
         # defines the term that accounts for the explicit dependence of the ensemble probability on the volume
-        dself.cell_jacobian = depend_value(
+        self._cell_jacobian = depend_value(
             name="cell_jacobian",
             func=self.get_cell_jacobian,
-            dependencies=[dd(self.cell).V, dself.temp],
+            dependencies=[self.cell._V, self._temp],
         )
 
         # the barostat energy must be computed from bits & pieces (overwrite the default)
-        dself.ebaro = depend_value(
+        self._ebaro = depend_value(
             name="ebaro",
             func=self.get_ebaro,
             dependencies=[
-                dself.kin,
-                dself.pot,
-                dself.cell_jacobian,
-                dd(self.thermostat).ethermo,
+                self._kin,
+                self._pot,
+                self._cell_jacobian,
+                self.thermostat._ethermo,
             ],
         )
 
     def get_pot(self):
         """Calculates the elastic strain energy of the cell."""
 
         # NOTE: since there are nbeads replicas of the unit cell, the enthalpy contains a nbeads factor
@@ -750,16 +765,14 @@
         # integrates with respect to the "high order" part of the stress with a timestep of dt /2
         press = np.trace(self.stress_sc) / 3.0
         self.p += self.dt / 2 * 3.0 * (self.cell.V * press)
 
     def pstep(self, level=0):
         """Propagates the momentum of the barostat."""
 
-        # self.pscstep()
-
         # we are assuming then that p the coupling between p^2 and dp/dt only involves the fast force
         dt = self.pdt[
             level
         ]  # this is already set to be half a time step at the specified MTS depth
         dt2 = dt**2
         dt3 = dt**3 / 3.0
 
@@ -777,15 +790,15 @@
                     self.cell.V * (press - self.beads.nbeads * self.pext)
                     + Constants.kb * self.temp
                 )
             )
             pc = dstrip(self.beads.pc)
             fc = (
                 np.sum(
-                    dstrip(self.forces.forces_mts(level))
+                    dstrip(self.forces.mts_forces[level].f)
                     * (1 + self.forces.coeffsc_part_1),
                     axis=0,
                 )
                 / self.beads.nbeads
             )
             m = dstrip(self.beads.m3)[0]
 
@@ -809,14 +822,17 @@
             dstrip(self.nm.pnm)[0, :] / m
         )
         self.nm.pnm[0, :] *= expp
 
         self.cell.h *= expq
 
 
+dproperties(BaroSCBZP, ["p", "m"])
+
+
 class BaroRGB(Barostat):
     """Raiteri-Gale-Bussi constant stress barostat class.
 
     Mode "anisotropic" implements the Raiteri-Gale-Bussi barostat which enables
     cell fluctuations (lengths and angles) at constant external stress.
 
     It is suitable for simulating solids at given external (non-diagonal) stresses
@@ -868,24 +884,22 @@
         super(BaroRGB, self).__init__(dt, temp, tau, ebaro, thermostat)
 
         # non-zero elements of the cell momentum are only
         # pxx pyy pzz pxy pxz pyz, but we want to access it either as a
         # 6-vector or as a 3x3 upper triangular tensor.
         # we use a synchronizer to achieve that
 
-        dself = dd(self)
-
         sync_baro = synchronizer()
-        dself.p6 = depend_array(
+        self._p6 = depend_array(
             name="p6",
             value=np.zeros(6, float),
             synchro=sync_baro,
             func={"p": self.get_3x3to6},
         )
-        dself.p = depend_array(
+        self._p = depend_array(
             name="p",
             value=np.zeros((3, 3), float),
             synchro=sync_baro,
             func={"p6": self.get_6to3x3},
         )
 
         if p is not None:
@@ -901,15 +915,15 @@
         if hfix is None:
             hfix = []
         self.hfix = hfix
 
         hmask = mask_from_fix(self.hfix)
 
         # mask to zero out components of the cell velocity, to implement cell-boundary constraints
-        dself.hmask = depend_array(name="hmask", value=hmask)
+        self._hmask = depend_array(name="hmask", value=hmask)
         # number of ones in the UT part of the mask
         self.L = np.diag([hmask[0].sum(), hmask[1, 1:].sum(), hmask[2, 2:].sum()])
 
         if stressext is not None:
             self.stressext = stressext
         else:
             self.stressext[:] = -1.0
@@ -932,72 +946,71 @@
         fixdof: The number of blocked degrees of freedom.
         """
 
         super(BaroRGB, self).bind(beads, nm, cell, forces, bias, prng, fixdof, nmts)
 
         # obtain the thermostat mass from the given time constant (1/3 of what used for the corresponding NPT case)
         # note that the barostat temperature is nbeads times the physical T
-        dself = dd(self)
 
-        dself.m = depend_array(
+        self._m = depend_array(
             name="m",
             value=np.atleast_1d(0.0),
             func=(
                 lambda: np.asarray(
                     [self.tau**2 * self.beads.natoms * Constants.kb * self.temp]
                 )
             ),
-            dependencies=[dself.tau, dself.temp],
+            dependencies=[self._tau, self._temp],
         )
 
-        dself.m6 = depend_array(
+        self._m6 = depend_array(
             name="m6",
             value=np.zeros(6, float),
             func=(lambda: np.asarray([1, 1, 1, 1, 1, 1]) * self.m[0]),
-            dependencies=[dself.m],
+            dependencies=[self._m],
         )
 
         # overrides definition of pot to depend on the many things it depends on for anisotropic cell
-        dself.pot = depend_value(
+        self._pot = depend_value(
             name="pot",
             func=self.get_pot,
             dependencies=[
-                dd(self.cell).h,
-                dd(self.h0).h,
-                dd(self.h0).V,
-                dd(self.h0).ih,
-                dself.stressext,
+                self.cell._h,
+                self.h0._h,
+                self.h0._V,
+                self.h0._ih,
+                self._stressext,
             ],
         )
 
         # binds the thermostat to the piston degrees of freedom
         self.thermostat.bind(pm=[self.p6, self.m6], prng=prng)
 
-        dself.kin = depend_value(
+        self._kin = depend_value(
             name="kin",
             func=(lambda: 0.5 * np.trace(np.dot(self.p.T, self.p)) / self.m[0]),
-            dependencies=[dself.p, dself.m],
+            dependencies=[self._p, self._m],
         )
 
         # defines the term that accounts for the explicit dependence of the ensemble on the cell
-        dself.cell_jacobian = depend_value(
+        self._cell_jacobian = depend_value(
             name="cell_jacobian",
             func=self.get_cell_jacobian,
-            dependencies=[dd(self.cell).h, dself.temp],
+            dependencies=[self.cell._h, self._temp],
         )
 
         # the barostat energy must be computed from bits & pieces (overwrite the default)
-        dself.ebaro = depend_value(
+        self._ebaro = depend_value(
             name="ebaro",
             func=self.get_ebaro,
             dependencies=[
-                dself.kin,
-                dself.pot,
-                dself.cell_jacobian,
-                dd(self.thermostat).ethermo,
+                self._kin,
+                self._pot,
+                self._cell_jacobian,
+                self.thermostat._ethermo,
             ],
         )
 
     def get_3x3to6(self):
         rp = np.zeros(6, float)
         rp[0] = self.p[0, 0]
         rp[1] = self.p[1, 1]
@@ -1022,17 +1035,14 @@
 
         # NOTE: since there are nbeads replicas of the unit cell, the enthalpy contains a nbeads factor
         eps = np.dot(self.cell.h, self.h0.ih)
         eps = np.dot(eps.T, eps)
         eps = 0.5 * (eps - np.identity(3))
 
         return self.h0.V * np.trace(np.dot(self.stressext, eps)) * self.beads.nbeads
-        # p = np.trace(self.stressext)/3
-        # return (p*(self.cell.V-self.h0.V) +
-        #    self.h0.V * np.trace(np.dot(self.stressext-np.eye(3)*p, eps)) ) * self.beads.nbeads
 
     def get_cell_jacobian(self):
         """Calculates the energy term that accounts for the size of the box."""
 
         cj = np.sum([(3 - i) * np.log(self.cell.h[i][i]) for i in range(3)])
         return -1.0 * Constants.kb * self.temp * cj
 
@@ -1059,15 +1069,15 @@
             self.p += dt * (
                 self.cell.V * np.triu(-self.beads.nbeads * pi_ext)
                 + Constants.kb * self.temp * self.L
             )
 
             pc = dstrip(self.beads.pc).reshape(self.beads.natoms, 3)
             fc = (
-                np.sum(dstrip(self.forces.forces_mts(level)), axis=0).reshape(
+                np.sum(dstrip(self.forces.mts_forces[level].f), axis=0).reshape(
                     self.beads.natoms, 3
                 )
                 / self.beads.nbeads
             )
             fcTonm = (fc / dstrip(self.beads.m3)[0].reshape(self.beads.natoms, 3)).T
 
             self.p += (
@@ -1116,14 +1126,17 @@
 
         self.nm.qnm[0] = q.reshape((self.beads.natoms * 3))
         self.nm.pnm[0] = p.reshape((self.beads.natoms * 3))
 
         self.cell.h = np.dot(expq, self.cell.h)
 
 
+dproperties(BaroRGB, ["p", "m", "p6", "hmask", "m6"])
+
+
 class BaroMTK(Barostat):
     """Martyna-Tobias-Klein flexible cell, constant pressure barostat class.
 
     Mode "flexible" implements the path integral version of Martyna-Tuckerman-Tobias-Klein
     barostat, which incorporates full cell fluctuations (lengths and angles) while
     sampling the isothermal isobaric ensemble.
 
@@ -1172,24 +1185,22 @@
         super(BaroMTK, self).__init__(dt, temp, tau, ebaro, thermostat)
 
         # non-zero elements of the cell momentum are only
         # pxx pyy pzz pxy pxz pyz, but we want to access it either as a
         # 6-vector or as a 3x3 upper triangular tensor.
         # we use a synchronizer to achieve that
 
-        dself = dd(self)
-
         sync_baro = synchronizer()
-        dself.p6 = depend_array(
+        self._p6 = depend_array(
             name="p6",
             value=np.zeros(6, float),
             synchro=sync_baro,
             func={"p": self.get_3x3to6},
         )
-        dself.p = depend_array(
+        self._p = depend_array(
             name="p",
             value=np.zeros((3, 3), float),
             synchro=sync_baro,
             func={"p6": self.get_6to3x3},
         )
 
         if p is not None:
@@ -1199,15 +1210,15 @@
 
         if hfix is None:
             hfix = []
         self.hfix = hfix
         hmask = mask_from_fix(hfix)
 
         # mask to zero out components of the cell velocity, to implement cell-boundary constraints
-        dself.hmask = depend_array(name="hmask", value=hmask)
+        self._hmask = depend_array(name="hmask", value=hmask)
         # number of ones in the UT part of the mask
         self.L = np.diag([hmask[0].sum(), hmask[1, 1:].sum(), hmask[2, 2:].sum()])
 
         if pext is not None:
             self.pext = pext
         else:
             self.pext = -1.0
@@ -1230,64 +1241,63 @@
         fixdof: The number of blocked degrees of freedom.
         """
 
         super(BaroMTK, self).bind(beads, nm, cell, forces, bias, prng, fixdof, nmts)
 
         # obtain the thermostat mass from the given time constant (1/3 of what used for the corresponding NPT case)
         # note that the barostat temperature is nbeads times the physical T
-        dself = dd(self)
 
-        dself.m = depend_array(
+        self._m = depend_array(
             name="m",
             value=np.atleast_1d(0.0),
             func=(
                 lambda: np.asarray(
                     [self.tau**2 * self.beads.natoms * Constants.kb * self.temp]
                 )
             ),
-            dependencies=[dself.tau, dself.temp],
+            dependencies=[self._tau, self._temp],
         )
 
-        dself.m6 = depend_array(
+        self._m6 = depend_array(
             name="m6",
             value=np.zeros(6, float),
             func=(lambda: np.asarray([1, 1, 1, 1, 1, 1]) * self.m[0]),
-            dependencies=[dself.m],
+            dependencies=[self._m],
         )
 
         # overrides definition of pot to depend on the many things it depends on for anisotropic cell
-        dself.pot = depend_value(
-            name="pot", func=self.get_pot, dependencies=[dd(self.cell).h, dself.pext]
+        self._pot = depend_value(
+            name="pot", func=self.get_pot, dependencies=[self.cell._h, self._pext]
         )
 
         # binds the thermostat to the piston degrees of freedom
         self.thermostat.bind(pm=[self.p6, self.m6], prng=prng)
 
-        dself.kin = depend_value(
+        self._kin = depend_value(
             name="kin",
             func=(lambda: 0.5 * np.trace(np.dot(self.p.T, self.p)) / self.m[0]),
-            dependencies=[dself.p, dself.m],
+            dependencies=[self._p, self._m],
         )
 
         # defines the term that accounts for the explicit dependence of the ensemble on the cell
-        dself.cell_jacobian = depend_value(
+        self._cell_jacobian = depend_value(
             name="cell_jacobian",
             func=self.get_cell_jacobian,
-            dependencies=[dd(self.cell).h, dself.temp],
+            dependencies=[self.cell._h, self._temp],
         )
 
         # the barostat energy must be computed from bits & pieces (overwrite the default)
-        dself.ebaro = depend_value(
+        self._ebaro = depend_value(
             name="ebaro",
             func=self.get_ebaro,
             dependencies=[
-                dself.kin,
-                dself.pot,
-                dself.cell_jacobian,
-                dd(self.thermostat).ethermo,
+                self._kin,
+                self._pot,
+                self._cell_jacobian,
+                self.thermostat._ethermo,
             ],
         )
 
     def get_3x3to6(self):
         rp = np.zeros(6, float)
         rp[0] = self.p[0, 0]
         rp[1] = self.p[1, 1]
@@ -1347,15 +1357,15 @@
             self.p += dt * (
                 self.cell.V * np.triu(-self.beads.nbeads * pi_ext)
                 + Constants.kb * self.temp * self.L
             )
 
             pc = dstrip(self.beads.pc).reshape(self.beads.natoms, 3)
             fc = (
-                np.sum(dstrip(self.forces.forces_mts(level)), axis=0).reshape(
+                np.sum(dstrip(self.forces.mts_forces[level].f), axis=0).reshape(
                     self.beads.natoms, 3
                 )
                 / self.beads.nbeads
             )
             fcTonm = (fc / dstrip(self.beads.m3)[0].reshape(self.beads.natoms, 3)).T
 
             self.p += (
@@ -1402,7 +1412,10 @@
         self.p *= self.hmask
         self.thermostat.ethermo -= self.kin
 
         self.nm.qnm[0] = q.reshape((self.beads.natoms * 3))
         self.nm.pnm[0] = p.reshape((self.beads.natoms * 3))
 
         self.cell.h = np.dot(expq, self.cell.h)
+
+
+dproperties(BaroMTK, ["p", "m", "p6", "hmask", "m6"])
```

### Comparing `ipi-2.6.0/ipi/engine/beads.py` & `ipi-2.6.3/ipi/engine/beads.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 from ipi.utils.depend import *
 from ipi.engine.atoms import Atoms
 
 
 __all__ = ["Beads"]
 
 
-class Beads(dobject):
-
+class Beads:
     """Storage for the beads positions and velocities.
 
     Everything is stored as (nbeads,3*natoms) sized contiguous arrays,
     and a convenience-access to each replica of the system is provided through a
     list of Atoms objects. Contains arrays of both the normal mode representation
     and the position representation, and various sized arrays for the atom
     labels and masses. Also contains the potential and force between
@@ -85,92 +84,90 @@
            natoms: The number of atoms.
            nbeads: The number of beads.
         """
 
         self.natoms = natoms
         self.nbeads = nbeads
 
-        dself = dd(self)
-
-        dself.names = depend_array(
+        self._names = depend_array(
             name="names", value=np.zeros(natoms, np.dtype("|U6"))
         )
 
         # atom masses, and mass-related arrays
-        dself.m = depend_array(
+        self._m = depend_array(
             name="m", value=np.zeros(natoms, float)
         )  # this is the prototype mass array (just one independent of bead n)
-        dself.m3 = depend_array(
+        self._m3 = depend_array(
             name="m3",
             value=np.zeros(
                 (nbeads, 3 * natoms), float
             ),  # this is m conveniently replicated to be (nb,3*nat)
             func=self.mtom3,
-            dependencies=[dself.m],
+            dependencies=[self._m],
         )
-        dself.sm3 = depend_array(
+        self._sm3 = depend_array(
             name="sm3",
             value=np.zeros(
                 (nbeads, 3 * natoms), float
             ),  # this is just the square root of m3
             func=self.m3tosm3,
-            dependencies=[dself.m3],
+            dependencies=[self._m3],
         )
 
         # positions and momenta. bead representation, base storage used everywhere
-        dself.q = depend_array(name="q", value=np.zeros((nbeads, 3 * natoms), float))
-        dself.p = depend_array(name="p", value=np.zeros((nbeads, 3 * natoms), float))
+        self._q = depend_array(name="q", value=np.zeros((nbeads, 3 * natoms), float))
+        self._p = depend_array(name="p", value=np.zeros((nbeads, 3 * natoms), float))
 
         # position and momentum of the centroid
-        dself.qc = depend_array(
+        self._qc = depend_array(
             name="qc",
             value=np.zeros(3 * natoms, float),
             func=self.get_qc,
-            dependencies=[dself.q],
+            dependencies=[self._q],
         )
-        dself.pc = depend_array(
+        self._pc = depend_array(
             name="pc",
             value=np.zeros(3 * natoms, float),
             func=self.get_pc,
-            dependencies=[dself.p],
+            dependencies=[self._p],
         )
 
         # path springs potential and force
-        dself.vpath = depend_value(
-            name="vpath", func=self.get_vpath, dependencies=[dself.q, dself.m3]
+        self._vpath = depend_value(
+            name="vpath", func=self.get_vpath, dependencies=[self._q, self._m3]
         )
-        dself.fpath = depend_array(
+        self._fpath = depend_array(
             name="fpath",
             value=np.zeros((nbeads, 3 * natoms), float),
             func=self.get_fpath,
-            dependencies=[dself.q],
+            dependencies=[self._q],
         )
 
         # create proxies to access the individual beads as Atoms objects
         # TODO: ACTUALLY THIS IS ONLY USED HERE METHINK, SO PERHAPS WE COULD REMOVE IT TO DECLUTTER THE CODE.
         self._blist = [
             Atoms(natoms, _prebind=(self.q[i, :], self.p[i, :], self.m, self.names))
             for i in range(nbeads)
         ]
 
         # kinetic energies of thhe beads, and total (classical) kinetic stress tensor
-        dself.kins = depend_array(
+        self._kins = depend_array(
             name="kins",
             value=np.zeros(nbeads, float),
             func=self.kin_gather,
-            dependencies=[dd(b).kin for b in self._blist],
+            dependencies=[b._kin for b in self._blist],
         )
-        dself.kin = depend_value(
-            name="kin", func=self.get_kin, dependencies=[dself.kins]
+        self._kin = depend_value(
+            name="kin", func=self.get_kin, dependencies=[self._kins]
         )
-        dself.kstress = depend_array(
+        self._kstress = depend_array(
             name="kstress",
             value=np.zeros((3, 3), float),
             func=self.get_kstress,
-            dependencies=[dd(b).kstress for b in self._blist],
+            dependencies=[b._kstress for b in self._blist],
         )
 
     def copy(self, nbeads=-1):
         """Creates a new beads object with newP <= P beads from the original.
 
         Returns:
            A Beads object with the first newP q, p, m and names arrays as the original.
@@ -207,20 +204,22 @@
         m3[:, 1 : 3 * self.natoms : 3] = m3[:, 0 : 3 * self.natoms : 3]
         m3[:, 2 : 3 * self.natoms : 3] = m3[:, 0 : 3 * self.natoms : 3]
         return m3
 
     def get_qc(self):
         """Gets the centroid coordinates."""
 
-        return np.dot(np.ones(self.nbeads, float), dstrip(self.q)) / float(self.nbeads)
+        return np.sum(dstrip(self.q), axis=0) / self.nbeads
+        # return np.dot(np.ones(self.nbeads, float), dstrip(self.q)) / float(self.nbeads)
 
     def get_pc(self):
         """Gets the centroid momenta."""
 
-        return np.dot(np.ones(self.nbeads, float), dstrip(self.p)) / float(self.nbeads)
+        return np.sum(dstrip(self.p), axis=0) / self.nbeads
+        # return np.dot(np.ones(self.nbeads, float), dstrip(self.p)) / float(self.nbeads)
 
     def kin_gather(self):
         """Gets the kinetic energy for all the replicas.
 
         Returns:
            A list of the kinetic energy for each system.
         """
@@ -342,7 +341,26 @@
            value: The Atoms object that holds the new values.
         """
 
         self._blist[index].p[:] = value.p
         self._blist[index].q[:] = value.q
         self._blist[index].m[:] = value.m
         self._blist[index].names[:] = value.names
+
+
+dproperties(
+    Beads,
+    [
+        "p",
+        "q",
+        "pc",
+        "qc",
+        "m",
+        "m3",
+        "names",
+        "sm3",
+        "kin",
+        "kstress",
+        "vpath",
+        "fpath",
+    ],
+)
```

### Comparing `ipi-2.6.0/ipi/engine/cell.py` & `ipi-2.6.3/ipi/engine/cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 from ipi.utils.depend import *
 from ipi.utils.mathtools import *
 
 
 __all__ = ["Cell"]
 
 
-class Cell(dobject):
-
+class Cell:
     """Base class to represent the simulation cell in a periodic system.
 
     This class has the base attributes required for either flexible or
     isotropic cell dynamics. Uses an upper triangular lattice vector matrix to
     represent the cell.
 
     Depend objects:
@@ -39,24 +38,22 @@
               reference cell matrix is set equal to this. Must be an upper
               triangular 3*3 matrix. Defaults to a 3*3 zeroes matrix.
         """
 
         if h is None:
             h = np.zeros((3, 3), float)
 
-        dself = dd(self)  # gets a direct-access view to self
-
-        dself.h = depend_array(name="h", value=h)
-        dself.ih = depend_array(
+        self._h = depend_array(name="h", value=h)
+        self._ih = depend_array(
             name="ih",
             value=np.zeros((3, 3), float),
             func=self.get_ih,
-            dependencies=[dself.h],
+            dependencies=[self._h],
         )
-        dself.V = depend_value(name="V", func=self.get_volume, dependencies=[dself.h])
+        self._V = depend_value(name="V", func=self.get_volume, dependencies=[self._h])
 
     def copy(self):
         return Cell(dstrip(self.h).copy())
 
     def get_ih(self):
         """Inverts the lattice vector matrix."""
 
@@ -126,7 +123,10 @@
            atom1 and atom2 in the minimum image convention.
         """
 
         s = np.dot(self.ih, atom1.q - atom2.q)
         for i in range(3):
             s[i] -= round(s[i])
         return np.dot(self.h, s)
+
+
+dproperties(Cell, ["h", "ih", "V"])
```

### Comparing `ipi-2.6.0/ipi/engine/ensembles.py` & `ipi-2.6.3/ipi/engine/ensembles.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,15 @@
     if not np.array_equal(ens1.hweights, ens2.hweights):
         ens1.hweights, ens2.hweights = (
             dstrip(ens2.hweights).copy(),
             dstrip(ens1.hweights).copy(),
         )
 
 
-class Ensemble(dobject):
-
+class Ensemble:
     """Base ensemble class.
 
     Defines the thermodynamic state of the system.
 
     Depend objects:
         temp: The system's temperature.
         pext: The systems's pressure
@@ -87,35 +86,34 @@
         """Initialises Ensemble.
 
         Args:
             temp: The temperature.
             fixcom: An optional boolean which decides whether the centre of mass
                 motion will be constrained or not. Defaults to False.
         """
-        dself = dd(self)
 
-        dself.temp = depend_value(name="temp")
+        self._temp = depend_value(name="temp")
         if temp is not None:
             self.temp = temp
         else:
             self.temp = -1.0
 
-        dself.stressext = depend_array(name="stressext", value=np.zeros((3, 3), float))
+        self._stressext = depend_array(name="stressext", value=np.zeros((3, 3), float))
         if stressext is not None:
             self.stressext = np.reshape(np.asarray(stressext), (3, 3))
         else:
             self.stressext = -1.0
 
-        dself.pext = depend_value(name="pext")
+        self._pext = depend_value(name="pext")
         if pext is not None:
             self.pext = pext
         else:
             self.pext = -1.0
 
-        dself.eens = depend_value(name="eens")
+        self._eens = depend_value(name="eens")
         if eens is not None:
             self.eens = eens
         else:
             self.eens = 0.0
 
         # the bias force contains two bits: explicit biases (that are meant to represent non-physical external biasing potentials)
         # and hamiltonian weights (that will act by scaling different physical components of the force). Both are bound as components
@@ -127,23 +125,23 @@
         self.bcomp = bcomponents
         self.bias = Forces()
 
         # and their weights
         if bweights is None or len(bweights) == 0:
             bweights = np.ones(len(self.bcomp))
 
-        dself.bweights = depend_array(name="bweights", value=np.asarray(bweights))
+        self._bweights = depend_array(name="bweights", value=np.asarray(bweights))
 
         # weights of the Hamiltonian scaling
         if hweights is None:
             hweights = np.ones(0)
         self.hweights = np.asarray(hweights)
 
         # Internal time counter
-        dd(self).time = depend_value(name="time")
+        self._time = depend_value(name="time")
         self.time = time
 
     def copy(self):
         return Ensemble(
             eens=self.eens,
             econs=0.0,
             temp=self.temp,
@@ -167,91 +165,97 @@
         xlpot=[],
         xlkin=[],
     ):
         self.beads = beads
         self.cell = cell
         self.forces = bforce
         self.nm = nm
-        dself = dd(self)
         self.output_maker = output_maker
 
         # this binds just the explicit bias forces
         self.bias.bind(
             self.beads,
             self.cell,
             self.bcomp,
             fflist,
             open_paths=nm.open_paths,
             output_maker=self.output_maker,
         )
 
-        dself.econs = depend_value(name="econs", func=self.get_econs)
+        self._econs = depend_value(name="econs", func=self.get_econs)
         # dependencies of the conserved quantity
-        dself.econs.add_dependency(dd(self.nm).kin)
-        dself.econs.add_dependency(dd(self.forces).pot)
-        dself.econs.add_dependency(dd(self.bias).pot)
-        dself.econs.add_dependency(dd(self.nm).vspring)
-        dself.econs.add_dependency(dself.eens)
+        self._econs.add_dependency(self.nm._kin)
+        self._econs.add_dependency(self.forces._pot)
+        self._econs.add_dependency(self.bias._pot)
+        self._econs.add_dependency(self.nm._vspring)
+        self._econs.add_dependency(self._eens)
 
         # pipes the weights to the list of weight vectors
         i = 0
         for fc in self.bias.mforces:
             if fc.weight != 1:
                 warning(
                     "The weight given to forces used in an ensemble bias are given a weight determined by bias_weight"
                 )
-            dpipe(dself.bweights, dd(fc).weight, i)
+            dpipe(self._bweights, fc._weight, i)
             i += 1
 
         # add Hamiltonian REM bias components
         if len(self.hweights) == 0:
             self.hweights = np.ones(len(self.forces.mforces))
 
-        dself.hweights = depend_array(name="hweights", value=np.asarray(self.hweights))
+        self._hweights = depend_array(name="hweights", value=np.asarray(self.hweights))
+        self._has_bias = depend_value(
+            name="has_bias",
+            func=lambda: (
+                len(self.bcomp) > 0 and np.mean((self.hweights - 1) ** 2) < 1e-20
+            ),
+            dependencies=[self._hweights],
+        )
 
-        # we use ScaledForceComponents to replicate the physical forces without (hopefully) them being actually recomputed
+        # we use ScaledForceComponents to replicate the physical forces without them being actually recomputed
         for ic in range(len(self.forces.mforces)):
             sfc = ScaledForceComponent(self.forces.mforces[ic], 1.0)
             self.bias.add_component(self.forces.mbeads[ic], self.forces.mrpc[ic], sfc)
-            dd(sfc).scaling._func = lambda i=ic: self.hweights[i] - 1
-            dd(sfc).scaling.add_dependency(dself.hweights)
+            sfc._scaling._func = lambda i=ic: self.hweights[i] - 1
+            sfc._scaling.add_dependency(self._hweights)
 
         self._elist = []
 
         for e in elist:
             self.add_econs(e)
 
-        dself.lpens = depend_value(
-            name="lpens", func=self.get_lpens, dependencies=[dself.temp]
+        self._lpens = depend_value(
+            name="lpens", func=self.get_lpens, dependencies=[self._temp]
         )
-        dself.lpens.add_dependency(dd(self.nm).kin)
-        dself.lpens.add_dependency(dd(self.forces).pot)
-        dself.lpens.add_dependency(dd(self.bias).pot)
-        dself.lpens.add_dependency(dd(self.nm).vspring)
+        self._lpens.add_dependency(self.nm._kin)
+        self._lpens.add_dependency(self.forces._pot)
+        self._lpens.add_dependency(self.bias._pot)
+        self._lpens.add_dependency(self.nm._vspring)
 
         # extended Lagrangian terms for the ensemble
         self._xlpot = []
         for p in xlpot:
             self.add_xlpot(p)
 
         self._xlkin = []
         for k in xlkin:
             self.add_xlkin(k)
 
     def add_econs(self, e):
         self._elist.append(e)
-        dd(self).econs.add_dependency(e)
+        self._econs.add_dependency(e)
 
     def add_xlpot(self, p):
         self._xlpot.append(p)
-        dd(self).lpens.add_dependency(p)
+        self._lpens.add_dependency(p)
 
     def add_xlkin(self, k):
         self._xlkin.append(k)
-        dd(self).lpens.add_dependency(k)
+        self._lpens.add_dependency(k)
 
     def get_econs(self):
         """Calculates the conserved energy quantity for constant energy
         ensembles.
         """
 
         eham = self.nm.vspring + self.nm.kin + self.forces.pot
@@ -274,7 +278,23 @@
         for p in self._xlpot:
             lpens += p.get()
         for k in self._xlkin:
             lpens += k.get()
 
         lpens *= -1.0 / (Constants.kb * self.temp * self.beads.nbeads)
         return lpens
+
+
+dproperties(
+    Ensemble,
+    [
+        "temp",
+        "stressext",
+        "pext",
+        "eens",
+        "bweights",
+        "time",
+        "econs",
+        "has_bias",
+        "lpens",
+    ],
+)
```

### Comparing `ipi-2.6.0/ipi/engine/forcefields.py` & `ipi-2.6.3/ipi/engine/forcefields.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,90 +16,79 @@
 
 import numpy as np
 
 from ipi.utils.softexit import softexit
 from ipi.utils.messages import verbosity
 from ipi.utils.messages import info
 from ipi.interfaces.sockets import InterfaceSocket
-from ipi.utils.depend import dobject
 from ipi.utils.depend import dstrip
 from ipi.utils.io import read_file
-from ipi.utils.units import unit_to_internal, UnitMap
+from ipi.utils.units import unit_to_internal
 from ipi.utils.distance import vector_separation
 
 try:
     import plumed
 except ImportError:
     plumed = None
 
 
-class NumpyEncoder(json.JSONEncoder):
-    """Special json encoder for numpy types"""
-
-    def default(self, obj):
-        if isinstance(obj, np.integer):
-            return int(obj)
-        elif isinstance(obj, np.floating):
-            return float(obj)
-        elif isinstance(obj, np.ndarray):
-            return obj.tolist()
-        return json.JSONEncoder.default(self, obj)
-
-
 class ForceRequest(dict):
-
     """An extension of the standard Python dict class which only has a == b
     if a is b == True, rather than if the elements of a and b are identical.
 
     Standard dicts are checked for equality if elements have the same value.
     Here I only care if requests are instances of the very same object.
     This is useful for the `in` operator, which uses equality to test membership.
     """
 
     def __eq__(self, y):
         """Overwrites the standard equals function."""
         return self is y
 
 
-class ForceField(dobject):
-
+class ForceField:
     """Base forcefield class.
 
     Gives the standard methods and quantities needed in all the forcefield
     classes.
 
     Attributes:
         pars: A dictionary of the parameters needed to initialize the forcefield.
             Of the form {'name1': value1, 'name2': value2, ... }.
         name: The name of the forcefield.
         latency: A float giving the number of seconds the socket will wait
             before updating the client list.
+        offset: A float giving a constant value that is subtracted from the return
+            value of the forcefield
         requests: A list of all the jobs to be given to the client codes.
         dopbc: A boolean giving whether or not to apply the periodic boundary
             conditions before sending the positions to the client code.
         _thread: The thread on which the socket polling loop is being run.
         _doloop: A list of booleans. Used to decide when to stop running the
             polling loop.
         _threadlock: Python handle used to lock the thread held in _thread.
     """
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         pars=None,
         dopbc=True,
         active=np.array([-1]),
         threaded=False,
     ):
         """Initialises ForceField.
 
         Args:
             latency: The number of seconds the socket will wait before updating
                 the client list.
+            offset: A constant offset subtracted from the energy value given by the
+                client.
             name: The name of the forcefield.
             pars: A dictionary used to initialize the forcefield, if required.
                 Of the form {'name1': value1, 'name2': value2, ... }.
             dopbc: Decides whether or not to apply the periodic boundary conditions
                 before sending the positions to the client code.
             active: Indexes of active atoms in this forcefield
         """
@@ -107,14 +96,15 @@
         if pars is None:
             self.pars = {}
         else:
             self.pars = pars
 
         self.name = name
         self.latency = latency
+        self.offset = offset
         self.requests = []
         self.dopbc = dopbc
         self.active = active
         self.iactive = None
         self.threaded = threaded
         self._thread = None
         self._doloop = [False]
@@ -217,15 +207,15 @@
         """Polls the forcefield object to check if it has finished."""
 
         with self._threadlock:
             for r in self.requests:
                 if r["status"] == "Queued":
                     r["t_dispatched"] = time.time()
                     r["result"] = [
-                        0.0,
+                        0.0 - self.offset,
                         np.zeros(len(r["pos"]), float),
                         np.zeros((3, 3), float),
                         {"raw": ""},
                     ]
                     r["status"] = "Done"
                     r["t_finished"] = time.time()
 
@@ -301,29 +291,29 @@
         """Makes updates to the potential that only need to be triggered
         upon completion of a time step."""
 
         pass
 
 
 class FFSocket(ForceField):
-
     """Interface between the PIMD code and a socket for a single replica.
 
     Deals with an individual replica of the system, obtaining the potential
     force and virial appropriate to this system. Deals with the distribution of
     jobs to the interface.
 
     Attributes:
         socket: The interface object which contains the socket through which
             communication between the forcefield and the driver is done.
     """
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         pars=None,
         dopbc=True,
         active=np.array([-1]),
         threaded=True,
         interface=None,
     ):
@@ -338,20 +328,23 @@
            dopbc: Decides whether or not to apply the periodic boundary conditions
               before sending the positions to the client code.
            interface: The object used to create the socket used to interact
               with the client codes.
         """
 
         # a socket to the communication library is created or linked
-        super(FFSocket, self).__init__(latency, name, pars, dopbc, active, threaded)
+        super(FFSocket, self).__init__(
+            latency, offset, name, pars, dopbc, active, threaded
+        )
         if interface is None:
             self.socket = InterfaceSocket()
         else:
             self.socket = interface
         self.socket.requests = self.requests
+        self.socket.offset = self.offset
 
     def poll(self):
         """Function to check the status of the client calculations."""
 
         self.socket.poll()
 
     def start(self):
@@ -366,16 +359,44 @@
         super(FFSocket, self).stop()
         if self._thread is not None:
             # must wait until loop has ended before closing the socket
             self._thread.join()
         self.socket.close()
 
 
-class FFLennardJones(ForceField):
+class FFEval(ForceField):
+    """General class for models that provide a self.evaluate(request)
+    to compute the potential, force and virial.
+    """
+
+    def poll(self):
+        """Polls the forcefield checking if there are requests that should
+        be answered, and if necessary evaluates the associated forces and energy."""
 
+        # We have to be thread-safe, as in multi-system mode this might get
+        # called by many threads at once.
+        with self._threadlock:
+            for r in self.requests:
+                if r["status"] == "Queued":
+                    r["status"] = "Running"
+                    r["t_dispatched"] = time.time()
+                    self.evaluate(r)
+                    r["result"][0] -= self.offset  # subtract constant offset
+
+    def evaluate(self, request):
+        request["result"] = [
+            0.0,
+            np.zeros(len(request["pos"]), float),
+            np.zeros((3, 3), float),
+            {"raw": ""},
+        ]
+        request["status"] = "Done"
+
+
+class FFLennardJones(FFEval):
     """Basic fully pythonic force provider.
 
     Computes LJ interactions without minimum image convention, cutoffs or
     neighbour lists. Parallel evaluation with threads.
 
     Attributes:
         parameters: A dictionary of the parameters used by the driver. Of the
@@ -383,48 +404,43 @@
         requests: During the force calculation step this holds a dictionary
             containing the relevant data for determining the progress of the step.
             Of the form {'atoms': atoms, 'cell': cell, 'pars': parameters,
                          'status': status, 'result': result, 'id': bead id,
                          'start': starting time}.
     """
 
-    def __init__(self, latency=1.0e-3, name="", pars=None, dopbc=False, threaded=False):
+    def __init__(
+        self,
+        latency=1.0e-3,
+        offset=0.0,
+        name="",
+        pars=None,
+        dopbc=False,
+        threaded=False,
+    ):
         """Initialises FFLennardJones.
 
         Args:
            pars: Optional dictionary, giving the parameters needed by the driver.
         """
 
         # check input - PBCs are not implemented here
         if dopbc:
             raise ValueError(
                 "Periodic boundary conditions are not supported by FFLennardJones."
             )
 
         # a socket to the communication library is created or linked
         super(FFLennardJones, self).__init__(
-            latency, name, pars, dopbc=dopbc, threaded=threaded
+            latency, offset, name, pars, dopbc=dopbc, threaded=threaded
         )
         self.epsfour = float(self.pars["eps"]) * 4
         self.sixepsfour = 6 * self.epsfour
         self.sigma2 = float(self.pars["sigma"]) * float(self.pars["sigma"])
 
-    def poll(self):
-        """Polls the forcefield checking if there are requests that should
-        be answered, and if necessary evaluates the associated forces and energy."""
-
-        # We have to be thread-safe, as in multi-system mode this might get
-        # called by many threads at once.
-        with self._threadlock:
-            for r in self.requests:
-                if r["status"] == "Queued":
-                    r["status"] = "Running"
-                    r["t_dispatched"] = time.time()
-                    self.evaluate(r)
-
     def evaluate(self, r):
         """Just a silly function evaluating a non-cutoffed, non-pbc and
         non-neighbour list LJ potential."""
 
         q = r["pos"].reshape((-1, 3))
         nat = len(q)
 
@@ -444,16 +460,15 @@
 
         v *= self.epsfour
 
         r["result"] = [v, f.reshape(nat * 3), np.zeros((3, 3), float), {"raw": ""}]
         r["status"] = "Done"
 
 
-class FFdmd(ForceField):
-
+class FFdmd(FFEval):
     """Pythonic force provider.
 
     Computes DMD forces as in Bowman, .., Brown JCP 2003 DOI: 10.1063/1.1578475. It is a time dependent potential.
     Here extended for periodic systems and for virial term calculation.
 
     Attributes:
         parameters: A dictionary of the parameters used by the driver. Of the
@@ -464,14 +479,15 @@
                          'status': status, 'result': result, 'id': bead id,
                          'start': starting time}.
     """
 
     def __init__(
         self,
         latency=1.0e-3,
+        offset=0.0,
         name="",
         coupling=None,
         freq=0.0,
         dtdmd=0.0,
         dmdstep=0,
         pars=None,
         dopbc=False,
@@ -480,15 +496,17 @@
         """Initialises FFdmd.
 
         Args:
            pars: Optional dictionary, giving the parameters needed by the driver.
         """
 
         # a socket to the communication library is created or linked
-        super(FFdmd, self).__init__(latency, name, pars, dopbc=dopbc, threaded=threaded)
+        super(FFdmd, self).__init__(
+            latency, offset, name, pars, dopbc=dopbc, threaded=threaded
+        )
 
         if coupling is None:
             raise ValueError("Must provide the couplings for DMD.")
         if freq is None:
             raise ValueError(
                 "Must provide a frequency for the periodically oscillating potential."
             )
@@ -497,27 +515,14 @@
                 "Must provide a time step for the periodically oscillating potential."
             )
         self.coupling = coupling
         self.freq = freq
         self.dtdmd = dtdmd
         self.dmdstep = dmdstep
 
-    def poll(self):
-        """Polls the forcefield checking if there are requests that should
-        be answered, and if necessary evaluates the associated forces and energy."""
-
-        # We have to be thread-safe, as in multi-system mode this might get
-        # called by many threads at once.
-        with self._threadlock:
-            for r in self.requests:
-                if r["status"] == "Queued":
-                    r["status"] = "Running"
-                    r["t_dispatched"] = time.time()
-                    self.evaluate(r)  # MR BAD
-
     def evaluate(self, r):
         """Evaluating dmd: pbc: YES,
         cutoff: NO, neighbour list: NO."""
 
         q = r["pos"].reshape((-1, 3))
         nat = len(q)
         cell_h, cell_ih = r["cell"]
@@ -559,16 +564,15 @@
         r["status"] = "Done"
 
     def dmd_update(self):
         """Updates time step when a full step is done. Can only be called after implementation goes into smotion mode..."""
         self.dmdstep += 1
 
 
-class FFDebye(ForceField):
-
+class FFDebye(FFEval):
     """Debye crystal harmonic reference potential
 
     Computes a harmonic forcefield.
 
     Attributes:
        parameters: A dictionary of the parameters used by the driver. Of the
           form {'name': value}.
@@ -578,14 +582,15 @@
                        'status': status, 'result': result, 'id': bead id,
                        'start': starting time}.
     """
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         H=None,
         xref=None,
         vref=0.0,
         pars=None,
         dopbc=False,
         threaded=False,
@@ -594,15 +599,15 @@
 
         Args:
            pars: Optional dictionary, giving the parameters needed by the driver.
         """
 
         # a socket to the communication library is created or linked
         # NEVER DO PBC -- forces here are computed without.
-        super(FFDebye, self).__init__(latency, name, pars, dopbc=False)
+        super(FFDebye, self).__init__(latency, offset, name, pars, dopbc=False)
 
         if H is None:
             raise ValueError("Must provide the Hessian for the Debye crystal.")
         if xref is None:
             raise ValueError(
                 "Must provide a reference configuration for the Debye crystal."
             )
@@ -613,25 +618,14 @@
 
         eigsys = np.linalg.eigh(self.H)
         info(
             " @ForceField: Hamiltonian eigenvalues: " + " ".join(map(str, eigsys[0])),
             verbosity.medium,
         )
 
-    def poll(self):
-        """Polls the forcefield checking if there are requests that should
-        be answered, and if necessary evaluates the associated forces and energy."""
-
-        # we have to be thread-safe, as in multi-system mode this might get called by many threads at once
-        with self._threadlock:
-            for r in self.requests:
-                if r["status"] == "Queued":
-                    r["status"] = "Running"
-                    self.evaluate(r)
-
     def evaluate(self, r):
         """A simple evaluator for a harmonic Debye crystal potential."""
 
         q = r["pos"]
         n3 = len(q)
         if self.H.shape != (n3, n3):
             raise ValueError("Hessian size mismatch")
@@ -647,15 +641,15 @@
             np.zeros((3, 3), float),
             {"raw": ""},
         ]
         r["status"] = "Done"
         r["t_finished"] = time.time()
 
 
-class FFPlumed(ForceField):
+class FFPlumed(FFEval):
     """Direct PLUMED interface
 
     Computes forces from a PLUMED input.
 
     Attributes:
         parameters: A dictionary of the parameters used by the driver. Of the
             form {'name': value}.
@@ -665,14 +659,15 @@
                       'status': status, 'result': result, 'id': bead id,
                       'start': starting time}.
     """
 
     def __init__(
         self,
         latency=1.0e-3,
+        offset=0.0,
         name="",
         pars=None,
         dopbc=False,
         threaded=False,
         init_file="",
         plumeddat="",
         plumedstep=0,
@@ -685,15 +680,15 @@
 
         # a socket to the communication library is created or linked
         if plumed is None:
             raise ImportError(
                 "Cannot find plumed libraries to link to a FFPlumed object/"
             )
         super(FFPlumed, self).__init__(
-            latency, name, pars, dopbc=False, threaded=threaded
+            latency, offset, name, pars, dopbc=False, threaded=threaded
         )
         self.plumed = plumed.Plumed()
         self.plumeddat = plumeddat
         self.plumedstep = plumedstep
         self.init_file = init_file
 
         if self.init_file.mode == "xyz":
@@ -701,16 +696,18 @@
             myframe = read_file(self.init_file.mode, infile)
             myatoms = myframe["atoms"]
             mycell = myframe["cell"]
             myatoms.q *= unit_to_internal("length", self.init_file.units, 1.0)
             mycell.h *= unit_to_internal("length", self.init_file.units, 1.0)
 
         self.natoms = myatoms.natoms
-        self.plumed.cmd("setNatoms", self.natoms)
+        self.plumed.cmd("setRealPrecision", 8)  # i-PI uses double precision
+        self.plumed.cmd("setMDEngine", "i-pi")
         self.plumed.cmd("setPlumedDat", self.plumeddat)
+        self.plumed.cmd("setNatoms", self.natoms)
         self.plumed.cmd("setTimestep", 1.0)
         self.plumed.cmd(
             "setMDEnergyUnits", 2625.4996
         )  # Pass a pointer to the conversion factor between the energy unit used in your code and kJ mol-1
         self.plumed.cmd(
             "setMDLengthUnits", 0.052917721
         )  # Pass a pointer to the conversion factor between the length unit used in your code and nm
@@ -722,28 +719,14 @@
             self.plumed.cmd("setRestart", 1)
         self.plumed.cmd("init")
         self.charges = dstrip(myatoms.q) * 0.0
         self.masses = dstrip(myatoms.m)
         self.lastq = np.zeros(3 * self.natoms)
         self.system_force = None  # reference to physical force calculator
 
-    def poll(self):
-        """Polls the forcefield checking if there are requests that should
-        be answered, and if necessary evaluates the associated forces and energy."""
-
-        # We have to be thread-safe, as in multi-system mode this might get
-        # called by many threads at once.
-        with self._threadlock:
-            for r in self.requests:
-                if r["status"] == "Queued":
-                    r["status"] = "Running"
-                    r["t_dispatched"] = time.time()
-                    self.evaluate(r)
-                    r["t_finished"] = time.time()
-
     def evaluate(self, r):
         """A wrapper function to call the PLUMED evaluation routines
         and return forces."""
 
         if self.natoms != len(r["pos"]) / 3:
             raise ValueError(
                 "Size of atom array changed after initialization of FFPlumed"
@@ -815,21 +798,21 @@
         self.plumed.cmd("prepareCalc")
         self.plumed.cmd("performCalcNoUpdate")
         self.plumed.cmd("update")
 
         return True
 
 
-class FFYaff(ForceField):
-
+class FFYaff(FFEval):
     """Use Yaff as a library to construct a force field"""
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         threaded=False,
         yaffpara=None,
         yaffsys=None,
         yafflog="yaff.log",
         rcut=18.89726133921252,
         alpha_scale=3.5,
@@ -859,15 +842,17 @@
 
         from yaff import System, ForceField, log
         import codecs
         import locale
         import atexit
 
         # a socket to the communication library is created or linked
-        super(FFYaff, self).__init__(latency, name, pars, dopbc, threaded=threaded)
+        super(FFYaff, self).__init__(
+            latency, offset, name, pars, dopbc, threaded=threaded
+        )
 
         # A bit weird to use keyword argument for a required argument, but this
         # is also done in the code above.
         if yaffpara is None:
             raise ValueError("Must provide a Yaff parameter file.")
 
         if yaffsys is None:
@@ -901,25 +886,14 @@
             skin=self.skin,
             smooth_ei=self.smooth_ei,
             reci_ei=self.reci_ei,
         )
 
         log._active = False
 
-    def poll(self):
-        """Polls the forcefield checking if there are requests that should
-        be answered, and if necessary evaluates the associated forces and energy."""
-
-        # we have to be thread-safe, as in multi-system mode this might get called by many threads at once
-        with self._threadlock:
-            for r in self.requests:
-                if r["status"] == "Queued":
-                    r["status"] = "Running"
-                    self.evaluate(r)
-
     def evaluate(self, r):
         """Evaluate the energy and forces with the Yaff force field."""
 
         q = r["pos"]
         nat = len(q) / 3
         rvecs = r["cell"][0]
 
@@ -927,28 +901,27 @@
         self.ff.update_pos(q.reshape((nat, 3)))
         gpos = np.zeros((nat, 3))
         vtens = np.zeros((3, 3))
         e = self.ff.compute(gpos, vtens)
 
         r["result"] = [e, -gpos.ravel(), -vtens, {"raw": ""}]
         r["status"] = "Done"
-        r["t_finished"] = time.time()
 
 
-class FFsGDML(ForceField):
-
+class FFsGDML(FFEval):
     """A symmetric Gradient Domain Machine Learning (sGDML) force field.
     Chmiela et al. Sci. Adv., 3(5), e1603015, 2017; Nat. Commun., 9(1), 3887, 2018.
     http://sgdml.org/doc/
     https://github.com/stefanch/sGDML
     """
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         threaded=False,
         sGDML_model=None,
         pars=None,
         dopbc=False,
     ):
         """Initialises FFsGDML
@@ -956,15 +929,19 @@
         Args:
 
            sGDML_model: Filename contaning the sGDML model
 
         """
 
         # a socket to the communication library is created or linked
-        super(FFsGDML, self).__init__(latency, name, pars, dopbc, threaded=threaded)
+        super(FFsGDML, self).__init__(
+            latency, offset, name, pars, dopbc, threaded=threaded
+        )
+
+        from ipi.utils.units import unit_to_user
 
         # --- Load sGDML package ---
         try:
             from sgdml.predict import GDMLPredict
             from sgdml import __version__
 
             info(" @ForceField: Using sGDML version " + __version__, verbosity.low)
@@ -981,72 +958,79 @@
         if dopbc is True:
             raise ValueError("Must set PBCs to False.")
 
         self.sGDML_model = sGDML_model
 
         # --- Load sGDML model file. ---
         try:
-            self.model = np.load(self.sGDML_model)
+            self.model = dict(np.load(self.sGDML_model, allow_pickle=True))
             info(
                 " @ForceField: sGDML model " + self.sGDML_model + " loaded",
                 verbosity.medium,
             )
         except ValueError:
             raise ValueError(
                 "ERROR: Reading sGDML model " + self.sGDML_model + " file failed."
             )
 
-        if "r_unit" in self.model and "e_unit" in self.model:
-            info(
-                " @ForceField: The units used in your sGDML model are"
-                + self.sGDML_model["r_unit"]
-                + " and "
-                + self.sGDML_model["r_unit"],
-                verbosity.low,
-            )
-
         info(
             " @ForceField: IMPORTANT: It is always assumed that the units in"
             + " the provided model file are in Angstroms and kcal/mol.",
             verbosity.low,
         )
 
+        # --- Units ---
+        transl_units_names = {
+            "Ang": "angstrom",
+            "bohr": "atomic_unit",
+            "millihartree": "milliatomic_unit",
+            "eV": "electronvolt",
+            "kcal/mol": "kilocal/mol",
+        }
+        if "r_unit" in self.model and "e_unit" in self.model:
+            distanceUnits = transl_units_names["{}".format(self.model["r_unit"])]
+            energyUnits = transl_units_names["{}".format(self.model["e_unit"])]
+            info(
+                " @ForceField: The units used in the sGDML model are: "
+                "distance --> {}, energy --> {}".format(distanceUnits, energyUnits),
+                verbosity.low,
+            )
+        else:
+            info(
+                " @ForceField: IMPORTANT: Since the sGDML model doesn't have units for distance and energy it is "
+                "assumed that the units are in Angstroms and kilocal/mol, respectively.",
+                verbosity.low,
+            )
+            distanceUnits = "angstrom"
+            energyUnits = "kilocal/mol"
+
         # --- Constants ---
-        self.bohr_to_ang = 1.0 / UnitMap["length"]["angstrom"]
-        self.kcalmol_to_hartree = UnitMap["energy"]["cal/mol"] * 1000.0
-        self.kcalmolang_to_hartreebohr = self.bohr_to_ang * self.kcalmol_to_hartree
+        self.bohr_to_distanceUnits = unit_to_user("length", distanceUnits, 1)
+        self.energyUnits_to_hartree = unit_to_internal("energy", energyUnits, 1)
+        self.forceUnits_to_hartreebohr = (
+            self.bohr_to_distanceUnits * self.energyUnits_to_hartree
+        )
 
         # --- Creates predictor ---
         self.predictor = GDMLPredict(self.model)
 
         info(
             " @ForceField: Optimizing parallelization settings for sGDML FF.",
             verbosity.medium,
         )
         self.predictor.prepare_parallel(n_bulk=1)
 
-    def poll(self):
-        """Polls the forcefield checking if there are requests that should
-        be answered, and if necessary evaluates the associated forces and energy."""
-
-        # we have to be thread-safe, as in multi-system mode this might get called by many threads at once
-        with self._threadlock:
-            for r in self.requests:
-                if r["status"] == "Queued":
-                    r["status"] = "Running"
-                    self.evaluate(r)
-
     def evaluate(self, r):
         """Evaluate the energy and forces."""
 
-        E, F = self.predictor.predict(r["pos"] * self.bohr_to_ang)
+        E, F = self.predictor.predict(r["pos"] * self.bohr_to_distanceUnits)
 
         r["result"] = [
-            E[0] * self.kcalmol_to_hartree,
-            F.flatten() * self.kcalmolang_to_hartreebohr,
+            E[0] * self.energyUnits_to_hartree,
+            F.flatten() * self.forceUnits_to_hartreebohr,
             np.zeros((3, 3), float),
             {"raw": ""},
         ]
         r["status"] = "Done"
         r["t_finished"] = time.time()
 
 
@@ -1054,30 +1038,33 @@
     """Combines multiple forcefields into a single forcefield object that consolidates
     individual components. Provides the infrastructure to run a simulation based on a
     committee of potentials, and implements the weighted baseline method."""
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         pars=None,
         dopbc=True,
         active=np.array([-1]),
         threaded=True,
         fflist=[],
         ffweights=[],
         alpha=1.0,
         baseline_name="",
         baseline_uncertainty=-1.0,
         active_thresh=0.0,
         active_out=None,
+        parse_json=False,
     ):
         # force threaded mode as otherwise it cannot have threaded children
         super(FFCommittee, self).__init__(
             latency=latency,
+            offset=offset,
             name=name,
             pars=pars,
             dopbc=dopbc,
             active=active,
             threaded=True,
         )
         if len(fflist) == 0:
@@ -1100,14 +1087,15 @@
             raise ValueError(
                 "Name and the uncertainty of the baseline are not simultaneously defined"
             )
         self.ffweights = ffweights
         self.alpha = alpha
         self.active_thresh = active_thresh
         self.active_out = active_out
+        self.parse_json = parse_json
 
     def bind(self, output_maker):
         super(FFCommittee, self).bind(output_maker)
         if self.active_thresh > 0:
             if self.active_out is None:
                 raise ValueError(
                     "Must specify an output file if you want to save structures for active learning"
@@ -1128,28 +1116,34 @@
 
         # creates the request with the help of the base class,
         # making sure it already contains a handle to the list of FF
         # requests
         req = super(FFCommittee, self).queue(
             atoms, cell, reqid, template=dict(ff_handles=ffh)
         )
+        req["t_dispatched"] = time.time()
         return req
 
     def check_finish(self, r):
         """Checks if all sub-requests associated with a given
         request are finished"""
         for ff_r in r["ff_handles"]:
             if ff_r["status"] != "Done":
                 return False
         return True
 
     def gather(self, r):
         """Collects results from all sub-requests, and assemble the committee of models."""
 
-        r["result"] = [0.0, np.zeros(len(r["pos"]), float), np.zeros((3, 3), float), ""]
+        r["result"] = [
+            0.0,
+            np.zeros(len(r["pos"]), float),
+            np.zeros((3, 3), float),
+            "",
+        ]
 
         # list of pointers to the forcefield requests. shallow copy so we can remove stuff
         com_handles = r["ff_handles"].copy()
         if self.baseline_name != "":
             # looks for the baseline potential, store its value and drops it from the list
             names = [ff.name for ff in self.fflist]
 
@@ -1159,18 +1153,45 @@
                     baseline_frc = ff_r["result"][1]
                     baseline_vir = ff_r["result"][2]
                     baseline_xtr = ff_r["result"][3]
                     com_handles.pop(i)
                     break
 
         # Gathers the forcefield energetics and extras
-        pots = [ff_r["result"][0] for ff_r in com_handles]
-        frcs = [ff_r["result"][1] for ff_r in com_handles]
-        virs = [ff_r["result"][2] for ff_r in com_handles]
-        xtrs = [ff_r["result"][3] for ff_r in com_handles]
+        pots = []
+        frcs = []
+        virs = []
+        xtrs = []
+
+        for ff_r in com_handles:
+            # if required, tries to extract multiple committe members from the extras JSON string
+            if "committee_pot" in ff_r["result"][3] and self.parse_json:
+                pots += ff_r["result"][3]["committee_pot"]
+                if "committee_force" not in ff_r["result"][3]:
+                    raise ValueError(
+                        "JSON extras for committe potential misses `committee_force` entry"
+                    )
+                frcs += ff_r["result"][3]["committee_force"]
+                if "committee_virial" not in ff_r["result"][3]:
+                    raise ValueError(
+                        "JSON extras for committe potential misses `committee_virial` entry"
+                    )
+                virs += ff_r["result"][3]["committee_virial"]
+                ff_r["result"][3].pop("committee_pot")
+                ff_r["result"][3].pop("committee_force")
+                ff_r["result"][3].pop("committee_virial")
+                xtrs.append(ff_r["result"][3])
+            else:
+                pots.append(ff_r["result"][0])
+                frcs.append(ff_r["result"][1])
+                virs.append(ff_r["result"][2])
+                xtrs.append(ff_r["result"][3])
+        pots = np.array(pots)
+        frcs = np.array(frcs).reshape(len(pots), -1)
+        virs = np.array(virs).reshape(-1, 3, 3)
 
         # Computes the mean energetics
         mean_pot = np.mean(pots, axis=0)
         mean_frc = np.mean(frcs, axis=0)
         mean_vir = np.mean(virs, axis=0)
 
         # Rescales the committee energetics so that their standard deviation corresponds to the error
@@ -1286,23 +1307,22 @@
             ff.release(ff_r)
 
     def poll(self):
         """Polls the forcefield object to check if it has finished."""
 
         with self._threadlock:
             for r in self.requests:
-                if self.check_finish(r):
-                    r["t_dispatched"] = time.time()
+                if r["status"] != "Done" and self.check_finish(r):
                     r["t_finished"] = time.time()
                     self.gather(r)
+                    r["result"][0] -= self.offset
                     r["status"] = "Done"
 
 
 class PhotonDriver:
-
     """
     Photon driver for a single cavity mode
     """
 
     def __init__(self, apply_photon=True, E0=1e-4, omega_c=0.01, ph_rep="loose"):
         """
         Initialise PhotonDriver
@@ -1487,26 +1507,26 @@
         coeff_y = np.dot(np.transpose(Eky), self.ftilde_ky)
         fx = -np.kron(coeff_x, charge_array_bath)
         fy = -np.kron(coeff_y, charge_array_bath)
         return fx, fy
 
 
 class FFCavPhSocket(FFSocket):
-
     """
     Socket for dealing with cavity photons interacting with molecules by
     Tao E. Li @ 2023-02-25
     Check https://doi.org/10.1073/pnas.2009272117 for details
 
     Independent bath approximation will be made to communicate with many sockets
     """
 
     def __init__(
         self,
         latency=1.0,
+        offset=0.0,
         name="",
         pars=None,
         dopbc=False,
         active=np.array([-1]),
         threaded=True,
         interface=None,
         charge_array=None,
@@ -1538,15 +1558,15 @@
                 'L' atom is coupled to the molecules, and the y dimension of the second 'L' atom is coupled
                 to the molecules. If 'dense', the cavity photons polarized along the x, y directions are
                 represented by one 'L' atom; the x and y dimensions of this 'L' atom are coupled to the molecules.
         """
 
         # a socket to the communication library is created or linked
         super(FFCavPhSocket, self).__init__(
-            latency, name, pars, dopbc, active, threaded, interface
+            latency, offset, name, pars, dopbc, active, threaded, interface
         )
 
         # definition of independent baths
         self.n_independent_bath = 1
         self.charge_array = charge_array
 
         # store photonic variables
@@ -1760,14 +1780,16 @@
             )
             # 8. add cavity effects to our output
             result_tot[0] += e_ph
             result_tot[1][:ndim_tot:3] += fx_cav
             result_tot[1][1:ndim_tot:3] += fy_cav
             result_tot[1][ndim_tot:] = f_ph
 
+        result_tot[0] -= self.offset
+
         # At this moment, we have sucessfully gathered the CavMD forces
         newreq = ForceRequest(
             {
                 "id": reqid,
                 "pos": pbcpos,
                 "active": self.iactive,
                 "cell": (dstrip(cell.h).copy(), dstrip(cell.ih).copy()),
```

### Comparing `ipi-2.6.0/ipi/engine/forces.py` & `ipi-2.6.3/ipi/engine/forces.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 __all__ = ["Forces", "ForceComponent"]
 
 
 fbuid = 0
 
 
-class ForceBead(dobject):
-
+class ForceBead:
     """Base force helper class.
 
     This is the object that computes forces for a single bead. This is the last
     layer before calling a forcefield object.
 
     Attributes:
        atoms: An Atoms object containing all the atom positions.
@@ -68,18 +67,17 @@
        vir: An array containing the components of the virial tensor in upper
           triangular form, not divided by the volume. Depends on ufvx.
        request: a handle to the request that has been filed by the FF object
     """
 
     def __init__(self):
         """Initialises ForceBead."""
-        dself = dd(self)
 
         # ufvx is a list [ u, f, vir, extra ]  which stores the results of the force calculation
-        dself.ufvx = depend_value(name="ufvx", func=self.get_all)
+        self._ufvx = depend_value(name="ufvx", func=self.get_all)
         self._threadlock = threading.Lock()
         self.request = None
         self._getallcount = 0
 
     def bind(self, atoms, cell, ff, output_maker):
         """Binds atoms, cell and a forcefield template to the ForceBead object.
 
@@ -96,61 +94,65 @@
             self.uid = fbuid
             fbuid += 1
 
         # stores a reference to the atoms and cell we are computing forces for
         self.atoms = atoms
         self.cell = cell
         self.ff = ff
-        dself = dd(self)
 
         # ufvx depends on the atomic positions and on the cell
-        dself.ufvx.add_dependency(dd(self.atoms).q)
-        dself.ufvx.add_dependency(dd(self.cell).h)
+        self._ufvx.add_dependency(self.atoms._q)
+        self._ufvx.add_dependency(self.cell._h)
 
         # potential and virial are to be extracted very simply from ufvx
-        dself.pot = depend_value(
-            name="pot", func=self.get_pot, dependencies=[dself.ufvx]
+        self._pot = depend_value(
+            name="pot", func=self.get_pot, dependencies=[self._ufvx]
         )
 
-        dself.vir = depend_array(
+        self._vir = depend_array(
             name="vir",
             value=np.zeros((3, 3), float),
             func=self.get_vir,
-            dependencies=[dself.ufvx],
+            dependencies=[self._ufvx],
         )
 
         # NB: the force requires a bit more work, to define shortcuts to xyz
         # slices without calculating the force at this point.
         fbase = np.zeros(atoms.natoms * 3, float)
-        dself.f = depend_array(
-            name="f", value=fbase, func=self.get_f, dependencies=[dself.ufvx]
+        self._f = depend_array(
+            name="f", value=fbase, func=self.get_f, dependencies=[self._ufvx]
         )
 
-        dself.extra = depend_value(
-            name="extra", func=self.get_extra, dependencies=[dself.ufvx]
+        self._extra = depend_value(
+            name="extra", func=self.get_extra, dependencies=[self._ufvx]
         )
 
-        dself.fx = depend_array(name="fx", value=fbase[0 : 3 * atoms.natoms : 3])
-        dself.fy = depend_array(name="fy", value=fbase[1 : 3 * atoms.natoms : 3])
-        dself.fz = depend_array(name="fz", value=fbase[2 : 3 * atoms.natoms : 3])
-        dcopy(dself.f, dself.fx)
-        dcopy(dself.f, dself.fy)
-        dcopy(dself.f, dself.fz)
+        self._fx = depend_array(name="fx", value=fbase[0 : 3 * atoms.natoms : 3])
+        self._fy = depend_array(name="fy", value=fbase[1 : 3 * atoms.natoms : 3])
+        self._fz = depend_array(name="fz", value=fbase[2 : 3 * atoms.natoms : 3])
+        dcopy(self._f, self._fx)
+        dcopy(self._f, self._fy)
+        dcopy(self._f, self._fz)
 
     def queue(self):
         """Sends the job to the interface queue directly.
 
         Allows the ForceBead object to ask for the ufvx list of each replica
         directly without going through the get_all function. This allows
         all the jobs to be sent at once, allowing them to be parallelized.
+
+        Returns True if a calculation is running
         """
 
+        # only dispatches a request if the forcefield needs it
         with self._threadlock:
-            if self.request is None and dd(self).ufvx.tainted():
+            is_tainted = self._ufvx.tainted()
+            if self.request is None and is_tainted:
                 self.request = self.ff.queue(self.atoms, self.cell, reqid=self.uid)
+        return is_tainted
 
     def get_all(self):
         """Driver routine.
 
         When one of the force, potential or virial are called, this sends the
         atoms and cell to the client code, requesting that it calculates the
         potential, forces and virial tensor. This then waits until the
@@ -163,58 +165,60 @@
         # because we thread over many systems and outputs, we might get called
         # more than once. keep track of how many times we are called so we
         # can make sure to wait until the last call has returned before we release
         with self._threadlock:
             self._getallcount += 1
 
         # this is converting the distribution library requests into [ u, f, v ]  lists
-        # t_start = time.time()
         if self.request is None:
-            self.request = self.queue()
+            self.queue()
 
         # sleeps until the request has been evaluated
-        while self.request["status"] != "Done":
-            if self.request["status"] == "Exit" or softexit.triggered:
+        request = self.request
+        latency = self.ff.latency
+        while request["status"] != "Done":
+            if request["status"] == "Exit" or softexit.triggered:
                 # now, this is tricky. we are stuck here and we cannot return meaningful results.
                 # if we return, we may as well output wrong numbers, or mess up things.
                 # so we can only call soft-exit and wait until that is done. then kill the thread
                 # we are in.
                 softexit.trigger(
                     message=" @ FORCES : cannot return so will die off here"
                 )
                 while softexit.exiting:
-                    time.sleep(self.ff.latency)
+                    time.sleep(latency)
                 sys.exit()
-            time.sleep(self.ff.latency)
+            time.sleep(latency)
+
         # print diagnostics about the elapsed time
         info(
             "# forcefield %s evaluated in %f (queue) and %f (dispatched) sec."
             % (
                 self.ff.name,
-                self.request["t_finished"] - self.request["t_queued"],
-                self.request["t_finished"] - self.request["t_dispatched"],
+                request["t_finished"] - request["t_queued"],
+                request["t_finished"] - request["t_dispatched"],
             ),
             verbosity.debug,
         )
 
         # data has been collected, so the request can be released and a slot
         # freed up for new calculations
-        result = self.request["result"]
+        result = request["result"]
 
         # reduce the reservation count (and wait for all calls to return)
         with self._threadlock:
             self._getallcount -= 1
 
         # releases just once, but wait for all requests to be complete
         if self._getallcount == 0:
-            self.ff.release(self.request)
+            self.ff.release(request)
             self.request = None
         else:
             while self._getallcount > 0:
-                time.sleep(self.ff.latency)
+                time.sleep(latency)
 
         return result
 
     def get_pot(self):
         """Calls get_all routine of forcefield to update the potential.
 
         Returns:
@@ -252,15 +256,18 @@
            A string containing all formatted additional output that the
            client might have produced.
         """
 
         return self.ufvx[3]
 
 
-class ForceComponent(dobject):
+dproperties(ForceBead, ["ufvx", "pot", "vir", "f", "extra", "fx", "fy", "fz"])
+
+
+class ForceComponent:
     """Computes one component (e.g. bonded interactions) of the force.
 
     Deals with splitting the bead representation into
     separate replicas, and collecting the data from each replica.
 
     Attributes:
        natoms: An integer giving the number of atoms.
@@ -314,15 +321,15 @@
               different force components have this field, they will also be summed with
               the respective weight like a forces object.
         """
 
         self.ffield = ffield
         self.name = name
         self.nbeads = nbeads
-        self.weight = depend_value(name="weight", value=weight)
+        self._weight = depend_value(name="weight", value=weight)
         if mts_weights is None:
             self.mts_weights = np.asarray([])
         else:
             self.mts_weights = np.asarray(mts_weights)
         if force_extras is None:
             self.force_extras = []
         else:
@@ -340,15 +347,14 @@
 
         Args:
            beads: Beads object from which the bead positions are taken.
            cell: Cell object from which the system box is taken.
            fflist: A list of forcefield objects to use to calculate the potential,
               forces and virial for each replica.
         """
-        dself = dd(self)
 
         # stores a copy of the number of atoms and of beads
         self.natoms = beads.natoms
         if self.nbeads != beads.nbeads:
             raise ValueError(
                 "Binding together a Beads and a ForceBeads objects with different numbers of beads"
             )
@@ -368,60 +374,66 @@
         self.beads = beads
         for b in range(self.nbeads):
             new_force = ForceBead()
             new_force.bind(beads[b], cell, self.ff, output_maker=output_maker)
             self._forces.append(new_force)
 
         # f is a big array which assembles the forces on individual beads
-        dself.f = depend_array(
+        self._f = depend_array(
             name="f",
             value=np.zeros((self.nbeads, 3 * self.natoms)),
             func=self.f_gather,
-            dependencies=[dd(self._forces[b]).f for b in range(self.nbeads)],
+            dependencies=[self._forces[b]._f for b in range(self.nbeads)],
         )
 
         # collection of pots, virs and extras from individual beads
-        dself.pots = depend_array(
+        self._pots = depend_array(
             name="pots",
             value=np.zeros(self.nbeads, float),
             func=self.pot_gather,
-            dependencies=[dd(self._forces[b]).pot for b in range(self.nbeads)],
+            dependencies=[self._forces[b]._pot for b in range(self.nbeads)],
         )
-        dself.virs = depend_array(
+        self._virs = depend_array(
             name="virs",
             value=np.zeros((self.nbeads, 3, 3), float),
             func=self.vir_gather,
-            dependencies=[dd(self._forces[b]).vir for b in range(self.nbeads)],
+            dependencies=[self._forces[b]._vir for b in range(self.nbeads)],
         )
-        dself.extras = depend_value(
+        self._extras = depend_value(
             name="extras",
             value=np.zeros(self.nbeads, float),
             func=self.extra_gather,
-            dependencies=[dd(self._forces[b]).extra for b in range(self.nbeads)],
+            dependencies=[self._forces[b]._extra for b in range(self.nbeads)],
         )
 
         # total potential and total virial
-        dself.pot = depend_value(
-            name="pot", func=(lambda: self.pots.sum()), dependencies=[dself.pots]
+        self._pot = depend_value(
+            name="pot", func=(lambda: self.pots.sum()), dependencies=[self._pots]
         )
-        dself.vir = depend_array(
+        self._vir = depend_array(
             name="vir",
             func=self.get_vir,
             value=np.zeros((3, 3)),
-            dependencies=[dself.virs],
+            dependencies=[self._virs],
         )
 
     def queue(self):
-        """Submits all the required force calculations to the interface."""
+        """Submits all the required force calculations to the interface.
+
+        Returns True if calculations are running, False if nothing is tainted
+        """
 
         # this should be called in functions which access u,v,f for ALL the beads,
         # before accessing them. it is basically pre-queueing so that the
         # distributed-computing magic can work
+
+        is_tainted = False
         for b in range(self.nbeads):
-            self._forces[b].queue()
+            is_tainted = is_tainted or self._forces[b].queue()
+        return is_tainted
 
     def pot_gather(self):
         """Obtains the potential energy for each replica.
 
         Returns:
            A list of the potential energy of each replica of the system.
         """
@@ -507,67 +519,76 @@
 
         vir = np.zeros((3, 3))
         for v in dstrip(self.virs):
             vir += v
         return vir
 
 
-class ScaledForceComponent(dobject):
+dproperties(ForceComponent, ["weight", "f", "pots", "pot", "virs", "vir", "extras"])
+
+
+class ScaledForceComponent:
     def __init__(self, baseforce, scaling=1):
         self.bf = baseforce
         self.name = baseforce.name
         self.ffield = baseforce.ffield
-        dself = dd(self)
-        dself.scaling = depend_value(name="scaling", value=scaling)
-        dself.f = depend_array(
+        self._scaling = depend_value(name="scaling", value=scaling)
+        self._f = depend_array(
             name="f",
-            func=lambda: self.scaling * self.bf.f
-            if scaling != 0
-            else np.zeros((self.bf.nbeads, 3 * self.bf.natoms)),
+            func=lambda: (
+                self.scaling * self.bf.f
+                if self.scaling != 0
+                else np.zeros((self.bf.nbeads, 3 * self.bf.natoms))
+            ),
             value=np.zeros((self.bf.nbeads, 3 * self.bf.natoms)),
-            dependencies=[dd(self.bf).f, dself.scaling],
+            dependencies=[self.bf._f, self._scaling],
         )
-        dself.pots = depend_array(
+        self._pots = depend_array(
             name="pots",
-            func=lambda: self.scaling * self.bf.pots
-            if scaling != 0
-            else np.zeros(self.bf.nbeads),
+            func=self.get_pots,
             value=np.zeros(self.bf.nbeads),
-            dependencies=[dd(self.bf).pots, dself.scaling],
+            dependencies=[self.bf._pots, self._scaling],
         )
-        dself.virs = depend_array(
+        self._virs = depend_array(
             name="virs",
             func=lambda: self.scaling * self.bf.virs,
             value=np.zeros((self.bf.nbeads, 3, 3)),
-            dependencies=[dd(self.bf).virs, dself.scaling],
+            dependencies=[self.bf._virs, self._scaling],
         )
-        dself.extras = depend_array(
+        self._extras = depend_array(
             name="extras",
             func=lambda: self.bf.extras,
             value=np.zeros(self.bf.nbeads),
-            dependencies=[dd(self.bf).extras],
+            dependencies=[self.bf._extras],
         )
 
         # total potential and total virial
-        dself.pot = depend_value(
-            name="pot", func=(lambda: self.pots.sum()), dependencies=[dself.pots]
+        self._pot = depend_value(
+            name="pot", func=(lambda: self.pots.sum()), dependencies=[self._pots]
         )
-        dself.vir = depend_array(
+        self._vir = depend_array(
             name="vir",
             func=self.get_vir,
             value=np.zeros((3, 3)),
-            dependencies=[dself.virs],
+            dependencies=[self._virs],
         )
 
         # pipes weight from the force, since the scaling is applied on top of that
-        self.weight = depend_value(name="weight", value=0)
-        dpipe(dd(self.bf).weight, dself.weight)
+        self._weight = depend_value(name="weight", value=0)
+        dpipe(self.bf._weight, self._weight)
         self.mts_weights = self.bf.mts_weights
         self.force_extras = self.bf.force_extras
 
+    def get_pots(self):
+        return (
+            self.scaling * self.bf.pots
+            if self.scaling != 0
+            else np.zeros(self.bf.nbeads)
+        )
+
     def get_vir(self):
         """Sums the virial of each replica.
 
         Not the actual system virial, as it has not been divided by either the
         number of beads or the cell volume.
 
         Returns:
@@ -579,16 +600,123 @@
             vir += v
         return vir
 
     def queue(self):
         pass  # this should be taken care of when the force/potential/etc is accessed
 
 
-class Forces(dobject):
+dproperties(
+    ScaledForceComponent,
+    ["weight", "scaling", "f", "pots", "pot", "virs", "vir", "extras"],
+)
+
+
+class MTSForces:
+    """Single-purpose class to compute the MTS forces at a given level"""
+
+    def __init__(self, parent, level):
+        self.nbeads = parent.nbeads
+        self.natoms = parent.natoms
+        self.mforces = parent.mforces
+        self.mrpc = parent.mrpc
+        self.level = level
+
+        self._f = depend_array(
+            name="f",
+            value=np.zeros((self.nbeads, 3 * self.natoms)),
+            func=self.get_forces_mts,
+        )
+
+        self._virs = depend_array(
+            name="virs", value=np.zeros((self.nbeads, 3, 3)), func=self.get_virs_mts
+        )
+
+        self._vir = depend_array(
+            name="vir",
+            value=np.zeros((3, 3)),
+            func=self.get_vir_mts,
+            dependencies=[self._virs],
+        )
+
+        for ff in self.mforces:
+            # add dependencies from the forces that actually depend on this
+            mts_weights = ff.mts_weights
+            if (len(mts_weights) == 0 and level == 0) or (
+                len(mts_weights) > level and mts_weights[level] != 0
+            ):
+                self._f.add_dependency(ff._f)
+                self._f.add_dependency(ff._weight)
+                self._virs.add_dependency(ff._virs)
+                self._virs.add_dependency(ff._weight)
+
+    def queue_mts(self):
+        """Submits all the required force calculations to the forcefields."""
+
+        level = self.level
+        for ff in self.mforces:
+            mts_weights = ff.mts_weights
+            # forces with no MTS specification are applied at the outer level
+            if (len(mts_weights) == 0 and level == 0) or (
+                len(mts_weights) > level and mts_weights[level] != 0 and ff.weight != 0
+            ):
+                # do not queue forces which have zero weight
+                ff.queue()
+
+    def get_forces_mts(self):
+        """Fetches ONLY the forces associated with a given MTS level."""
+
+        level = self.level
+        self.queue_mts()
+
+        fk = np.zeros((self.nbeads, 3 * self.natoms))
+
+        mforces = self.mforces
+        mrpc = self.mrpc
+        for index in range(len(mforces)):
+            # forces with no MTS specification are applied at the outer level
+            weight = mforces[index].weight
+            mts_weights = mforces[index].mts_weights
+            if (len(mts_weights) == 0 and level == 0) or (
+                len(mts_weights) > level and mts_weights[level] != 0 and weight != 0
+            ):
+                fk += (
+                    weight
+                    * mts_weights[level]
+                    * mrpc[index].b2tob1(dstrip(mforces[index].f))
+                )
+        return fk
+
+    def get_vir_mts(self):
+        """Fetches ONLY the total virial associated with a given MTS level."""
+        return np.sum(dstrip(self.virs), axis=0)
 
+    def get_virs_mts(self):
+        """Fetches ONLY the total virial associated with a given MTS level."""
+
+        self.queue_mts()
+        level = self.level
+        mforces = self.mforces
+        mrpc = self.mrpc
+        rp = np.zeros((self.nbeads, 3, 3), float)
+        for index in range(len(mforces)):
+            if (
+                len(mforces[index].mts_weights) > level
+                and mforces[index].mts_weights[level] != 0
+                and mforces[index].weight != 0
+            ):
+                dmvirs = dstrip(mforces[index].virs)
+                dv = mrpc[index].b2tob1(dmvirs)
+                rp += mforces[index].weight * mforces[index].mts_weights[level] * dv
+        return rp
+
+
+dproperties(MTSForces, ["f", "vir", "virs"])
+
+
+class Forces:
     """Class that gathers all the forces together.
     Collects many forcefield instances and parallelizes getting the forces
     in a PIMD environment.
 
     Attributes:
        natoms: An integer giving the number of atoms.
        nbeads: An integer giving the number of beads.
@@ -618,20 +746,18 @@
         self.dcell = None
 
     def add_component(self, nbeads, nrpc, nforces):
         self.mrpc.append(nrpc)
         self.mbeads.append(nbeads)
         self.mforces.append(nforces)
         self.nforces += 1
-        dself = dd(self)
-        dforces = dd(nforces)
-        dself.f.add_dependency(dforces.f)
-        dself.pots.add_dependency(dforces.pots)
-        dself.virs.add_dependency(dforces.virs)
-        dself.extras.add_dependency(dforces.extras)
+        self._f.add_dependency(nforces._f)
+        self._pots.add_dependency(nforces._pots)
+        self._virs.add_dependency(nforces._virs)
+        self._extras.add_dependency(nforces._extras)
 
     def bind(self, beads, cell, fcomponents, fflist, open_paths, output_maker):
         """Binds beads, cell and forces to the forcefield.
 
 
         Args:
            beads: Beads object from which the bead positions are taken.
@@ -649,26 +775,27 @@
 
         self.natoms = beads.natoms
         self.nbeads = beads.nbeads
         self.beads = beads
         self.cell = cell
         self.bound = True
         self.nforces = len(fcomponents)
+
+        # prepares force components
         self.fcomp = fcomponents
+
         self.ff = fflist
         self.open_paths = open_paths
         self.output_maker = output_maker
 
         # fflist should be a dictionary of forcefield objects
         self.mforces = []
         self.mbeads = []
         self.mrpc = []
 
-        dself = dd(self)
-
         # a "function factory" to generate functions to automatically update
         # contracted paths
         def make_rpc(rpc, beads):
             return lambda: rpc.b1tob2(dstrip(beads.q))
 
         # creates new force objects, possibly acting on contracted path
         # representations. note that this new object is always created even if no contraction is required.
@@ -689,195 +816,198 @@
                 epsilon=fc.epsilon,
             )
             newbeads = Beads(beads.natoms, newb)
             newrpc = nm_rescale(beads.nbeads, newb, open_paths=self.open_paths)
 
             # the beads positions for this force components are obtained
             # automatically, when needed, as a contraction of the full beads
-            dd(newbeads).q._func = make_rpc(newrpc, beads)
+            newbeads._q._func = make_rpc(newrpc, beads)
             for b in newbeads:
                 # must update also indirect access to the beads coordinates
-                dd(b).q._func = dd(newbeads).q._func
+                b._q._func = newbeads._q._func
 
             # makes newbeads.q depend from beads.q
-            dd(beads).q.add_dependant(dd(newbeads).q)
+            beads._q.add_dependant(newbeads._q)
 
             # now we create a new forcecomponent which is bound to newbeads!
             newforce.bind(newbeads, cell, fflist, output_maker=self.output_maker)
 
             # adds information we will later need to the appropriate lists.
             self.mbeads.append(newbeads)
             self.mforces.append(newforce)
             self.mrpc.append(newrpc)
 
         # now must expose an interface that gives overall forces
-        dself.f = depend_array(
+        self._f = depend_array(
             name="f",
             value=np.zeros((self.nbeads, 3 * self.natoms)),
             func=self.f_combine,
-            dependencies=[dd(ff).f for ff in self.mforces],
+            dependencies=[ff._f for ff in self.mforces],
         )
 
         # collection of pots and virs from individual ff objects
-        dself.pots = depend_array(
+        self._pots = depend_array(
             name="pots",
             value=np.zeros(self.nbeads, float),
             func=self.pot_combine,
-            dependencies=[dd(ff).pots for ff in self.mforces],
+            dependencies=[ff._pots for ff in self.mforces],
         )
 
         # must take care of the virials!
-        dself.virs = depend_array(
+        self._virs = depend_array(
             name="virs",
             value=np.zeros((self.nbeads, 3, 3), float),
             func=self.vir_combine,
-            dependencies=[dd(ff).virs for ff in self.mforces],
+            dependencies=[ff._virs for ff in self.mforces],
         )
 
-        dself.extras = depend_value(
+        self._extras = depend_value(
             name="extras",
             value=np.zeros(self.nbeads, float),
             func=self.extra_combine,
-            dependencies=[dd(ff).extras for ff in self.mforces],
+            dependencies=[ff._extras for ff in self.mforces],
         )
 
         # total potential and total virial
-        dself.pot = depend_value(
-            name="pot", func=(lambda: self.pots.sum()), dependencies=[dself.pots]
+        self._pot = depend_value(
+            name="pot", func=(lambda: self.pots.sum()), dependencies=[self._pots]
         )
 
-        dself.vir = depend_array(
+        self._vir = depend_array(
             name="vir",
             func=self.get_vir,
             value=np.zeros((3, 3)),
-            dependencies=[dself.virs],
+            dependencies=[self._virs],
         )
 
         # SC forces and potential
-        dself.alpha = depend_value(name="alpha", value=0.0)
+        self._alpha = depend_value(name="alpha", value=0.0)
 
         # The number of MTS levels
-        dself.nmtslevels = depend_value(
+        self._nmtslevels = depend_value(
             name="nmtslevels", value=0, func=self.get_nmtslevels
         )
 
+        if len(self.mforces) > 0:
+            self.mts_forces = [MTSForces(self, i) for i in range(self.nmtslevels)]
+
         # This will be piped from normalmodes
-        dself.omegan2 = depend_value(name="omegan2", value=0)
+        self._omegan2 = depend_value(name="omegan2", value=0)
 
         # The Suzuki-Chin difference potential
-        dself.potssc = depend_array(
+        self._potssc = depend_array(
             name="potssc",
             value=np.zeros(self.nbeads, float),
             dependencies=[
-                dd(self.beads).m,
-                dself.f,
-                dself.pots,
-                dself.alpha,
-                dself.omegan2,
+                self.beads._m,
+                self._f,
+                self._pots,
+                self._alpha,
+                self._omegan2,
             ],
             func=self.get_potssc,
         )
 
-        dself.potsc = depend_value(
-            name="potsc", dependencies=[dself.potssc], func=(lambda: self.potssc.sum())
+        self._potsc = depend_value(
+            name="potsc", dependencies=[self._potssc], func=(lambda: self.potssc.sum())
         )
 
         # The coefficients of the physical and the |f|^2 terms
-        dself.coeffsc_part_1 = depend_array(
+        self._coeffsc_part_1 = depend_array(
             name="coeffsc_part_1",
             value=np.zeros((self.nbeads, 1), float),
             func=self.get_coeffsc_part_1,
         )
 
-        dself.coeffsc_part_2 = depend_array(
+        self._coeffsc_part_2 = depend_array(
             name="coeffsc_part_2",
             value=np.zeros((self.nbeads, 1), float),
-            dependencies=[dself.alpha, dself.omegan2],
+            dependencies=[self._alpha, self._omegan2],
             func=self.get_coeffsc_part_2,
         )
 
         # A list that contains the high order component of the force and the virial
-        dself.fvir_4th_order = depend_value(
+        self._fvir_4th_order = depend_value(
             name="fvir_4th_order",
             value=[None, None],
-            dependencies=[dd(self.beads).m, dself.f, dself.pots],
+            dependencies=[self.beads._m, self._f, self._pots],
             func=self.fvir_4th_order_combine,
         )
 
         # The high order component of the Suzuki-Chin force.
-        dself.f_4th_order = depend_array(
+        self._f_4th_order = depend_array(
             name="f_4th_order",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
-            dependencies=[dself.fvir_4th_order],
+            dependencies=[self._fvir_4th_order],
             func=(lambda: self.fvir_4th_order[0]),
         )
 
-        dself.fsc_part_1 = depend_array(
+        self._fsc_part_1 = depend_array(
             name="fsc_part_1",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
-            dependencies=[dself.coeffsc_part_1, dself.f],
+            dependencies=[self._coeffsc_part_1, self._f],
             func=self.get_fsc_part_1,
         )
 
-        dself.fsc_part_2 = depend_array(
+        self._fsc_part_2 = depend_array(
             name="fsc_part_2",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
-            dependencies=[dself.coeffsc_part_2, dself.f_4th_order],
+            dependencies=[self._coeffsc_part_2, self._f_4th_order],
             func=self.get_fsc_part_2,
         )
 
-        dself.fsc = depend_array(
+        self._fsc = depend_array(
             name="fsc",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
-            dependencies=[dself.fsc_part_1, dself.fsc_part_2],
+            dependencies=[self._fsc_part_1, self._fsc_part_2],
             func=self.get_fsc,
         )
 
         # The high order component of the Suzuki-Chin virial.
-        dself.virs_4th_order = depend_array(
+        self._vir_4th_order = depend_array(
             name="vir_4th_order",
             value=np.zeros((self.nbeads, 3, 3), float),
-            dependencies=[dself.fvir_4th_order],
+            dependencies=[self._fvir_4th_order],
             func=(lambda: self.fvir_4th_order[1]),
         )
 
-        dself.virssc_part_1 = depend_array(
+        self._virssc_part_1 = depend_array(
             name="virssc_part_1",
             value=np.zeros((self.nbeads, 3, 3), float),
-            dependencies=[dself.coeffsc_part_1, dself.virs],
+            dependencies=[self._coeffsc_part_1, self._virs],
             func=self.get_virssc_part_1,
         )
 
-        dself.virssc_part_2 = depend_array(
+        self._virssc_part_2 = depend_array(
             name="virssc_part_2",
             value=np.zeros((self.nbeads, 3, 3), float),
-            dependencies=[dself.coeffsc_part_2, dself.virs_4th_order],
+            dependencies=[self._coeffsc_part_2, self._vir_4th_order],
             func=self.get_virssc_part_2,
         )
 
-        dself.virssc = depend_array(
+        self._virssc = depend_array(
             name="virssc",
             value=np.zeros((self.nbeads, 3, 3), float),
-            dependencies=[dself.virssc_part_1, dself.virssc_part_2],
+            dependencies=[self._virssc_part_1, self._virssc_part_2],
             func=self.get_virssc,
         )
 
-        dself.virsc = depend_value(
-            name="potsc",
-            dependencies=[dself.potssc],
+        self._virsc = depend_value(
+            name="virsc",
+            dependencies=[self._potssc],
             func=(lambda: np.sum(self.virssc, axis=0)),
         )
 
         # Add dependencies from the force weights, that are applied here when the total
         # force is assembled from its components
 
         for fc in self.mforces:
-            dself.f.add_dependency(dd(fc).weight)
-            dself.pots.add_dependency(dd(fc).weight)
-            dself.virs.add_dependency(dd(fc).weight)
+            self._f.add_dependency(fc._weight)
+            self._pots.add_dependency(fc._weight)
+            self._virs.add_dependency(fc._weight)
 
     def copy(self, beads=None, cell=None):
         """Returns a copy of this force object that can be used to compute forces,
         e.g. for use in internal loops of geometry optimizers, or for property
         calculation.
 
         Args:
@@ -933,21 +1063,20 @@
             # then we copy the force value, and set the force as untainted.
             # next time we touch the master q, the tainting does not get
             # propagated, because the contracted q is already marked as tainted,
             # so the force does not get updated. we can fix this by copying
             # the value of the contracted bead, so that it's marked as NOT
             # tainted - it should not be as it's an internal of the force and
             # therefore get copied
-            dd(mself.beads).q.set(mreff.beads.q, manual=False)
+            mself.beads._q.set(mreff.beads.q, manual=False)
             for b in range(mself.nbeads):
-                dfkbref = dd(mreff._forces[b])
-                dfkbself = dd(mself._forces[b])
-
-                dfkbself.ufvx.set(deepcopy(dfkbref.ufvx._value), manual=False)
-                dfkbself.ufvx.taint(taintme=False)
+                mself._forces[b]._ufvx.set(
+                    deepcopy(mreff._forces[b]._ufvx._value), manual=False
+                )
+                mself._forces[b]._ufvx.taint(taintme=False)
 
     def transfer_forces_manual(
         self, new_q, new_v, new_forces, new_x=None, vir=np.zeros((3, 3))
     ):
         """Manual (and flexible) version of the transfer forces function.
         Instead of passing a force object, list with vectors are passed
         Expected shape and sizes:
@@ -957,39 +1086,38 @@
           - new_x list of length equal to number of force type, containing the beads extras
         """
         msg = "Unconsistent dimensions inside transfer_forces_manual"
         assert len(self.mforces) == len(new_q), msg
         assert len(self.mforces) == len(new_v), msg
         assert len(self.mforces) == len(new_forces), msg
         if new_x == None:
-            new_x = [[None] * self.nbeads] * len(self.mforces)
+            new_x = [{"raw": [None] * self.nbeads}] * len(self.mforces)
             info("WARNING: No extras information has been passed.", verbosity.debug)
 
         assert len(self.mforces) == len(new_x), msg
 
         for k in range(len(self.mforces)):
             mv = new_v[k]
             mf = new_forces[k]
             mq = new_q[k]
             mextra = new_x[k]
             mself = self.mforces[k]
-
             assert mq.shape == mf.shape, msg
             assert mq.shape[0] == mv.shape[0], msg
             assert mself.nbeads == mv.shape[0], msg
             assert mself.nbeads == mq.shape[0], msg
-            assert mself.nbeads == len(mextra), msg
-            mxlist = mextra[:]
 
-            dd(mself.beads).q.set(mq, manual=False)
+            mself.beads._q.set(mq, manual=False)
             for b in range(mself.nbeads):
-                ufvx = [mv[b], mf[b], vir, mxlist[b]]
-                dfkbself = dd(mself._forces[b])
-                dfkbself.ufvx.set(ufvx, manual=False)
-                dfkbself.ufvx.taint(taintme=False)
+                mx = {}
+                for key in mextra.keys():
+                    mx[key] = mextra[key][b]
+                ufvx = [mv[b], mf[b], vir, mx]
+                mself._forces[b]._ufvx.set(ufvx, manual=False)
+                mself._forces[b]._ufvx.taint(taintme=False)
 
     def run(self):
         """Makes the socket start looking for driver codes.
 
         Tells the interface code to start the thread that looks for
         connection from the driver codes in a loop. Until this point no
         jobs can be queued.
@@ -1008,17 +1136,19 @@
 
         for ff in self.mforces:
             ff.stop()
 
     def queue(self):
         """Submits all the required force calculations to the forcefields."""
 
+        is_tainted = False
         for ff in self.mforces:
             if ff.weight != 0:  # do not compute forces which have zero weight
-                ff.queue()
+                is_tainted = is_tainted or ff.queue()
+        return is_tainted
 
     def get_vir(self):
         """Sums the virial of each forcefield.
 
         Not the actual system virial.
 
         Returns:
@@ -1063,61 +1193,36 @@
             )
         if self.mforces[index].weight == 0:
             raise ValueError(
                 "Cannot fetch extras for a component that has not been computed because of zero weight"
             )
         return self.mforces[index].extras
 
-    def queue_mts(self, level):
-        """Submits all the required force calculations to the forcefields."""
-
-        for ff in self.mforces:
-            # forces with no MTS specification are applied at the outer level
-            if (len(ff.mts_weights) == 0 and level == 0) or (
-                len(ff.mts_weights) > level
-                and ff.mts_weights[level] != 0
-                and ff.weight != 0
-            ):
-                # do not queue forces which have zero weight
-                ff.queue()
-
-    def forces_mts(self, level):
-        """Fetches ONLY the forces associated with a given MTS level."""
-
-        self.queue_mts(level)
-        fk = np.zeros((self.nbeads, 3 * self.natoms))
-        for index in range(len(self.mforces)):
-            # forces with no MTS specification are applied at the outer level
-            if (len(self.mforces[index].mts_weights) == 0 and level == 0) or (
-                len(self.mforces[index].mts_weights) > level
-                and self.mforces[index].mts_weights[level] != 0
-                and self.mforces[index].weight != 0
-            ):
-                fk += (
-                    self.mforces[index].weight
-                    * self.mforces[index].mts_weights[level]
-                    * self.mrpc[index].b2tob1(dstrip(self.mforces[index].f))
-                )
-        return fk
-
     def forcesvirs_4th_order(self, index):
         """Fetches the 4th order |f^2| correction to the force vector and the virial associated with a given component."""
 
         # gives an error is number of beads is not even.
         if self.nbeads % 2 != 0:
             warning("ERROR: Suzuki-Chin factorization requires even number of beads!")
             exit()
 
         # calculates the finite displacement.
         fbase = dstrip(self.f)
         eps = self.mforces[index].epsilon
-        delta = np.abs(eps) / np.sqrt(
+        foverm = np.sqrt(
             (fbase / self.beads.m3 * fbase / self.beads.m3).sum()
             / (self.nbeads * self.natoms)
         )
+        if np.abs(foverm) > 1e-20:
+            delta = np.abs(eps) / np.sqrt(
+                (fbase / self.beads.m3 * fbase / self.beads.m3).sum()
+                / (self.nbeads * self.natoms)
+            )
+        else:  # defaults to eps if otherwise we'd get an 1/0
+            delta = np.abs(eps)
         dq = delta * fbase / self.beads.m3
 
         # stores the force component.
         fbase = self.mrpc[index].b2tob1(dstrip(self.mforces[index].f))
         mvirs = dstrip(self.mforces[index].virs)
         vbase = self.mrpc[index].b2tob1(mvirs)
 
@@ -1127,19 +1232,19 @@
             # The problem is that the finite difference is computed as [f(q + e.f) - f(q)].e^-1,
             # where f(q + e.f) is computed on a smaller rimg polymer of P / 2 beads which is made
             # by displacing the odd beads of the original ring polymer. Upon contraction,  it yields
             # a ring polymer that is different from the contracted one on which f(q) was computed.
             # This makes the FD incorrect. A fix could be to ALWAYS compute the odd and the even
             # beads on two different ring polymers of P / 2 beads, but centered difference + RPC
             # seems to be a neater solution. Anyway, the cost of a CNT-DIFF in comparison to a FWD-DIFF
-            # is marginal in when RPC + MTS is used.
+            # is marginal when RPC + MTS is used.
 
             if self.mforces[index].nbeads != self.nbeads:
                 warning(
-                    "ERROR: high order PIMD + RPC works with a centered finite difference only! (Uness you find an elegant solution :))"
+                    "ERROR: high order PIMD + RPC works with a centered finite difference only! (Unless you find an elegant solution :))"
                 )
                 exit()
 
             # for the case of alpha = 0, only odd beads are displaced.
             if self.alpha == 0:
                 # we use an aux force evaluator with half the number of beads.
                 if self.dforces is None:
@@ -1275,38 +1380,14 @@
                 # calculates the finite difference.
                 f_4th_order = 2.0 * (fminus - fplus) / 2.0 / delta
                 v_4th_order = 2.0 * (vminus - vplus) / 2.0 / delta
 
         # returns the 4th order |f^2| correction.
         return [f_4th_order, v_4th_order]
 
-    def vir_mts(self, level):
-        """Fetches ONLY the total virial associated with a given MTS level."""
-        return np.sum(self.virs_mts(level), axis=0)
-
-    def virs_mts(self, level):
-        """Fetches ONLY the total virial associated with a given MTS level."""
-
-        self.queue_mts(level)
-        rp = np.zeros((self.beads.nbeads, 3, 3), float)
-        for index in range(len(self.mforces)):
-            if (
-                len(self.mforces[index].mts_weights) > level
-                and self.mforces[index].mts_weights[level] != 0
-                and self.mforces[index].weight != 0
-            ):
-                dmvirs = dstrip(self.mforces[index].virs)
-                dv = self.mrpc[index].b2tob1(dmvirs)
-                rp += (
-                    self.mforces[index].weight
-                    * self.mforces[index].mts_weights[level]
-                    * dv
-                )
-        return rp
-
     def get_nmtslevels(self):
         """Returns the total number of mts levels."""
 
         nm = len(self.mforces[0].mts_weights)
         if all(len(x.mts_weights) == nm for x in self.mforces):
             return nm
         else:
@@ -1334,15 +1415,15 @@
         """Obtains the total fourth order |f^2| correction to the force vector and the virial."""
 
         rf = np.zeros((self.nbeads, 3 * self.natoms), float)
         rv = np.zeros((self.nbeads, 3, 3), float)
 
         for k in range(self.nforces):
             if self.mforces[k].weight != 0 and self.mforces[k].mts_weights.sum() != 0:
-                fv = dstrip(self.forcesvirs_4th_order(k))
+                fv = self.forcesvirs_4th_order(k)
                 rf += self.mforces[k].weight * self.mforces[k].mts_weights.sum() * fv[0]
                 rv += self.mforces[k].weight * self.mforces[k].mts_weights.sum() * fv[1]
         return [rf, rv]
 
     def pot_combine(self):
         """Obtains the potential energy for each forcefield."""
 
@@ -1455,15 +1536,15 @@
         return self.coeffsc_part_1.reshape((self.beads.nbeads, 1, 1)) * dstrip(
             self.virs
         )
 
     def get_virssc_part_2(self):
         """Obtains the quadratic component of Suzuki-Chin correction to the virial."""
         return self.coeffsc_part_2.reshape((self.beads.nbeads, 1, 1)) * dstrip(
-            self.virs_4th_order
+            self.vir_4th_order
         )
 
     def get_fsc(self):
         """Obtains the total Suzuki-Chin correction to the force."""
         return dstrip(self.fsc_part_1) + dstrip(self.fsc_part_2)
 
     def get_virssc(self):
@@ -1481,7 +1562,37 @@
     def get_coeffsc_part_2(self):
         """Obtains the coefficients of the linear part of the Suzuki-Chin correction."""
 
         rc = np.zeros(self.beads.nbeads)
         rc[0::2] = self.alpha / self.omegan2 / 9.0
         rc[1::2] = (1.0 - self.alpha) / self.omegan2 / 9.0
         return np.asmatrix(rc).T
+
+
+dproperties(
+    Forces,
+    [
+        "f",
+        "pots",
+        "virs",
+        "extras",
+        "pot",
+        "vir",
+        "alpha",
+        "nmtslevels",
+        "omegan2",
+        "potssc",
+        "potsc",
+        "coeffsc_part_1",
+        "coeffsc_part_2",
+        "fvir_4th_order",
+        "f_4th_order",
+        "fsc_part_1",
+        "fsc_part_2",
+        "fsc",
+        "vir_4th_order",
+        "virssc_part_1",
+        "virssc_part_2",
+        "virssc",
+        "virsc",
+    ],
+)
```

### Comparing `ipi-2.6.0/ipi/engine/initializer.py` & `ipi-2.6.3/ipi/engine/initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 
 from ipi.engine.beads import Beads
 from ipi.engine.normalmodes import NormalModes
 from ipi.engine.ensembles import Ensemble
 from ipi.engine.motion import Motion
 from ipi.utils.io import read_file
 from ipi.utils.io.inputs.io_xml import xml_parse_file
-from ipi.utils.depend import dobject
 from ipi.utils.units import Constants, unit_to_internal
 from ipi.utils.nmtransform import nm_rescale
 from ipi.utils.messages import verbosity, warning, info
 
 
 __all__ = ["Initializer", "InitBase", "InitIndexed", "InitFile"]
 
 
-class InitBase(dobject):
-
+class InitBase:
     """Base class for initializer objects.
 
     Reads data from a string or file.
 
     Attributes:
        value: A duck-typed stored value.
        mode: A string that determines how the value is to be interpreted.
@@ -56,15 +54,14 @@
         self.units = units
 
         for o, v in list(others.items()):
             self.__dict__[o] = v
 
 
 class InitIndexed(InitBase):
-
     """Class to initialize objects which can be set for a particular bead.
 
     The same as init base, but can also optionally hold information about which
     atom or bead to initialize from.
 
     Attributes:
        index: Which atom to initialize the value of.
@@ -297,16 +294,15 @@
     else:  # we are initializing a specific bead
         if iif.index < 0:
             dq[iif.bead] = rq
         else:
             dq[iif.bead, 3 * iif.index : 3 * (iif.index + 1)] = rq
 
 
-class Initializer(dobject):
-
+class Initializer:
     """Class that deals with the initialization of data.
 
     Holds functions that are required to initialize objects in the code.  Data
     can be initialized from a file, or according to a particular parameter. An
     example of the former would be initializing the configurations from a xyz
     file, an example of the latter would be initializing the velocities
     according to the physical temperature.
@@ -360,21 +356,17 @@
         Raises:
            ValueError: Raised if there is a problem with the initialization,
               if something that should have been has not been, or if the objects
               that have been specified are not compatible with each other.
         """
 
         if simul.beads.nbeads == 0:
-            fpos = (
-                fmom
-            ) = (
-                fmass
-            ) = (
-                flab
-            ) = fcell = False  # we don't have an explicitly defined beads object yet
+            fpos = fmom = fmass = flab = fcell = (
+                False  # we don't have an explicitly defined beads object yet
+            )
         else:
             fpos = fmom = fmass = flab = fcell = True
 
         for k, v in self.queue:
             info(
                 " # Initializer (stage 1) parsing " + str(k) + " object.",
                 verbosity.high,
```

### Comparing `ipi-2.6.0/ipi/engine/motion/__init__.py` & `ipi-2.6.3/ipi/engine/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/engine/motion/al6xxx_kmc.py` & `ipi-2.6.3/ipi/engine/motion/al6xxx_kmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pickle
 import threading
 import numpy as np
 import collections
 
 from ipi.engine.motion import Motion, GeopMotion
-from ipi.utils.depend import dstrip, depend_value, dd
+from ipi.utils.depend import dstrip, depend_value
 from ipi.engine.cell import Cell
 from ipi.utils.units import Constants
 import ipi.utils.io as io
 
 
 class AlKMC(Motion):
     """Stepper for a KMC for Al-6xxx alloys.
@@ -160,15 +160,15 @@
                     self.neigh[j, nneigh[j]] = i
                     nneigh[i] += 1
                     nneigh[j] += 1
 
         self.idx = idx
 
         # the KMC step is variable and so it cannot be stored as proper timing
-        dd(self).dt = depend_value(name="dt", value=0.0)
+        self._dt = depend_value(name="dt", value=0.0)
         self.fixatoms = np.asarray([])
         self.fixcom = True
         self.optimizer = [None] * self.neval
         # geop should not trigger exit if there is early convergence, but just carry on.
         # we hard-code this option to avoid early-termination that would be hard to debug for a user
         optimizer["exit_on_convergence"] = False
         for i in range(self.neval):
```

### Comparing `ipi-2.6.0/ipi/engine/motion/alchemy.py` & `ipi-2.6.3/ipi/engine/motion/alchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 
 import numpy as np
 
 from ipi.engine.motion import Motion
-from ipi.utils.depend import *
+from ipi.utils.depend import dproperties, depend_value, dstrip
 from ipi.utils.units import Constants
 
 
 # __all__ = ['AlchemyMC']
 
 
 class AlchemyMC(Motion):
-
     """Monte Carlo alchemical exchanges class.
 
     Attributes:
         names of the isotopes for exchanges
 
     Depend objects:
         The spring potential energy, names of the atoms.
@@ -42,16 +41,15 @@
         """
 
         super(AlchemyMC, self).__init__(fixcom=fixcom, fixatoms=fixatoms)
 
         self.names = names
         self.nxc = nxc
 
-        dself = dd(self)
-        dself.ealc = depend_value(name="ealc")
+        self._ealc = depend_value(name="ealc")
         if ealc is not None:
             self.ealc = ealc
         else:
             self.ealc = 0.0
 
     def bind(self, ens, beads, cell, bforce, nm, prng, omaker):
         """Binds ensemble beads, cell, bforce, and prng to the dynamics.
@@ -66,15 +64,15 @@
         Args:
             beads: The beads object from whcih the bead positions are taken.
             prng: The random number generator object which controls random number
                 generation.
         """
 
         super(AlchemyMC, self).bind(ens, beads, cell, bforce, nm, prng, omaker)
-        self.ensemble.add_econs(dd(self).ealc)
+        self.ensemble.add_econs(self._ealc)
 
     def AXlist(self, atomtype):
         """This compile a list of atoms ready for exchanges."""
 
         # selects the types of atoms for exchange
         atomexchangelist = []
         for i in range(self.beads.natoms):
@@ -154,7 +152,10 @@
                 )
                 self.beads.p[:, 3 * axlist[j] : 3 * (axlist[j] + 1)] *= np.sqrt(
                     massratio
                 )
 
                 # adjusts the conserved quantity counter based on the change in spring energy
                 self.ealc += -difspring
+
+
+dproperties(AlchemyMC, ["ealc"])
```

### Comparing `ipi-2.6.0/ipi/engine/motion/atomswap.py` & `ipi-2.6.3/ipi/engine/motion/atomswap.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from ipi.engine.motion import Motion
 from ipi.utils.depend import *
 from ipi.utils.units import Constants
 
 
 class AtomSwap(Motion):
-
     """Swap atom positions (typically useful to exchange species in
     a way that is compatible with the i-PI encapsulation paradigm.
 
     Attributes:
         names of the species for exchanges
     """
 
@@ -37,16 +36,15 @@
         """
 
         super(AtomSwap, self).__init__(fixcom=fixcom, fixatoms=fixatoms)
 
         self.names = names
         self.nxc = nxc
 
-        dself = dd(self)
-        dself.ealc = depend_value(name="ealc")
+        self._ealc = depend_value(name="ealc")
         if ealc is not None:
             self.ealc = ealc
         else:
             self.ealc = 0.0
 
     def bind(self, ens, beads, cell, bforce, nm, prng, omaker):
         """Binds ensemble beads, cell, bforce, and prng to the dynamics.
@@ -61,15 +59,15 @@
         Args:
             beads: The beads object from whcih the bead positions are taken.
             prng: The random number generator object which controls random number
                 generation.
         """
 
         super(AtomSwap, self).bind(ens, beads, cell, bforce, nm, prng, omaker)
-        self.ensemble.add_econs(dd(self).ealc)
+        self.ensemble.add_econs(self._ealc)
         self.dbeads = self.beads.copy()
         self.dcell = self.cell.copy()
         self.dforces = self.forces.copy(self.dbeads, self.dcell)
 
     def AXlist(self, atomtype):
         """This compile a list of atoms ready for exchanges."""
 
@@ -129,7 +127,10 @@
 
                 # copy the exchanged beads position
                 self.beads.q[:] = self.dbeads.q[:]
                 # transfers the (already computed) status of the force, so we don't need to recompute
                 self.forces.transfer_forces(self.dforces)
 
                 self.ealc += -(new_energy - old_energy)
+
+
+dproperties(AtomSwap, ["ealc"])
```

### Comparing `ipi-2.6.0/ipi/engine/motion/constrained_dynamics.py` & `ipi-2.6.3/ipi/engine/motion/constrained_dynamics.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,25 +75,25 @@
         Args:
             dt: The timestep of the simulation algorithms.
             fixcom: An optional boolean which decides whether the centre of mass
                 motion will be constrained or not. Defaults to False.
         """
 
         super(Dynamics, self).__init__(fixcom=fixcom, fixatoms=fixatoms)
-        dd(self).dt = depend_value(name="dt", value=timestep)
+        self._dt = depend_value(name="dt", value=timestep)
 
         if thermostat is None:
             self.thermostat = Thermostat()
         else:
             self.thermostat = thermostat
 
         if nmts is None or len(nmts) == 0:
-            dd(self).nmts = depend_array(name="nmts", value=np.asarray([1], int))
+            self._nmts = depend_array(name="nmts", value=np.asarray([1], int))
         else:
-            dd(self).nmts = depend_array(name="nmts", value=np.asarray(nmts, int))
+            self._nmts = depend_array(name="nmts", value=np.asarray(nmts, int))
 
         if barostat is None:
             self.barostat = Barostat()
         else:
             self.barostat = barostat
         self.enstype = mode
 
@@ -105,15 +105,15 @@
             ValueError(
                 "{:s} is not a valid ensemble for constrained dynamics".format(
                     self.enstype
                 )
             )
 
         # splitting mode for the integrators
-        dd(self).splitting = depend_value(name="splitting", value=splitting)
+        self._splitting = depend_value(name="splitting", value=splitting)
 
         # The list of constraints coming from the input is an actual list of independent
         # constraints, and should be treated as such
         if constraint_list is not None:
             self.constraint_list = constraint_list
 
         has_eckart = False
@@ -186,24 +186,27 @@
 
         # now binds the constraints
         for c in self.constraint_list:
             c.bind(beads)
         self.csolver.bind(beads)
 
 
-class ConstraintSolverBase(dobject):
+dproperties(ConstrainedDynamics, ["dt", "nmts", "splitting"])
+
+
+class ConstraintSolverBase:
     """Empty base class for the constraint solver. Provides the interface
     that must be used to offer constraint functionalities to an integrator.
     """
 
     def __init__(self, constraint_list, dt=1.0):
         self.constraint_list = constraint_list
 
         # time step - will have to be linked to the dynamics time step
-        dd(self).dt = depend_value(name="dt", value=dt)
+        self._dt = depend_value(name="dt", value=dt)
 
     def bind(self, beads):
         if beads.nbeads > 1:
             raise ValueError(
                 "Constrained dynamics is only implemented for the case of classical MD (nbeads=1)"
             )
 
@@ -225,14 +228,17 @@
         """Enforce the constraints on the positions (project onto the
         constraint manifold using the Gramian matrix).
         """
 
         raise NotImplementedError()
 
 
+dproperties(ConstraintSolverBase, ["dt"])
+
+
 class ConstraintSolver(ConstraintSolverBase):
     """An implementation of a constraint solver that uses M-RATTLE to
     impose constraints onto the momenta and a quasi-Newton method
     to impose constraints onto the positions. The constraint is applied
     sparsely, i.e. on each block of constraints separately.
 
     For implementation details of M-RATTLE see
@@ -260,31 +266,28 @@
         """Set the momenta conjugate to the constrained degrees of freedom
         to zero non-iteratively by inverting the Gram matrix. For further
         details see H. C. Andersen, J. Comput. Phys. 52, 24 (1983). Note
         that independent groups of constraints are treated separately
         (sparsely).
         """
 
-        #        m3 = dstrip(self.beads.m3[0])
         p = dstrip(self.beads.p[0]).copy()
-        self.beads.p.hold()
 
         for constr in self.constraint_list:
             dg = dstrip(constr.Dg)
             ic = constr.i3_unique
             b = np.dot(dg, p[ic] / constr.m3)
 
             if spla is None:
                 x = np.linalg.solve(dstrip(constr.Gram), b)
             else:
                 x = spla.cho_solve(dstrip(constr.GramChol), b)
 
             p[ic] -= np.dot(np.transpose(dg), x)
         self.beads.p[0] = p
-        self.beads.p.resume()
 
     def proj_manifold(self):
         """Iteratively enforce the constraints onto the positions by finding
         the Lagrange multipliers using a quasi-Newton solver. Note
         that independent groups of constraints are treated separately
         (sparsely).
         """
@@ -358,37 +361,39 @@
 
     def bind(self, motion):
         """Creates local references to all the variables for simpler access."""
 
         super(ConstrainedIntegrator, self).bind(motion)
 
         self.constraint_list = motion.constraint_list
-        dself = dd(self)
         if motion.nsteps_geo is None:
-            dself.nsteps_geo = depend_value(name="nsteps_geo", value=1)
+            self._nsteps_geo = depend_value(name="nsteps_geo", value=1)
         else:
-            dself.nsteps_geo = depend_value(name="nsteps_geo", value=motion.nsteps_geo)
-        print(self.nsteps_geo)
-        dself.qdt.add_dependency(dself.nsteps_geo)
+            self._nsteps_geo = depend_value(name="nsteps_geo", value=motion.nsteps_geo)
+
+        self._qdt.add_dependency(self._nsteps_geo)
         if motion.nsteps_o is None:
-            dself.nsteps_o = depend_value(name="nsteps_o", value=1)
+            self._nsteps_o = depend_value(name="nsteps_o", value=1)
         else:
-            dself.nsteps_o = depend_value(name="nsteps_o", value=motion.nsteps_o)
-        print(self.nsteps_o)
-        dself.tdt.add_dependency(dself.nsteps_o)
-        dd(self).csolver = motion.csolver
-        dpipe(dself.qdt, dd(self.csolver).dt)
+            self._nsteps_o = depend_value(name="nsteps_o", value=motion.nsteps_o)
+
+        self._tdt.add_dependency(self._nsteps_o)
+        self.csolver = motion.csolver
+        dpipe(self._qdt, self.csolver._dt)
 
     def proj_cotangent(self):
         self.csolver.proj_cotangent()
 
     def proj_manifold(self):
         self.csolver.proj_manifold()
 
 
+dproperties(ConstrainedIntegrator, ["nsteps_geo", "nsteps_o"])
+
+
 class NVEConstrainedIntegrator(ConstrainedIntegrator):
     """A propagator for constant-energy integration under a set of constraints.
 
     Implementation details:
         B. Leimkuhler, C. Matthews Proc. R. Soc. A 472, 20160138, (2016)
     """
 
@@ -488,15 +493,14 @@
     def step(self, step=None):
         """Does one simulation time step."""
 
         self.mtsprop(0)
 
 
 class NVTConstrainedIntegrator(NVEConstrainedIntegrator):
-
     """Constrained integrator object for constant temperature simulations.
 
     Has the relevant conserved quantity for the constant temperature
     ensemble. Contains a thermostat object that keeps the temperature
     constant.
 
     Implementation details:
```

### Comparing `ipi-2.6.0/ipi/engine/motion/dynamics.py` & `ipi-2.6.3/ipi/engine/motion/dynamics.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from ipi.engine.thermostats import Thermostat
 from ipi.engine.barostats import Barostat
 from ipi.utils.softexit import softexit
 from ipi.utils.messages import warning, verbosity
 
 
 class Dynamics(Motion):
-
     """self (path integral) molecular dynamics class.
 
     Gives the standard methods and attributes needed in all the
     dynamics classes.
 
     Attributes:
         beads: A beads object giving the atoms positions.
@@ -62,35 +61,34 @@
         Args:
             dt: The timestep of the simulation algorithms.
             fixcom: An optional boolean which decides whether the centre of mass
                 motion will be constrained or not. Defaults to False.
         """
 
         super(Dynamics, self).__init__(fixcom=fixcom, fixatoms=fixatoms)
-        dself = dd(self)  # noqa
 
         # initialize time step. this is the master time step that covers a full time step
-        dd(self).dt = depend_value(name="dt", value=timestep)
+        self._dt = depend_value(name="dt", value=timestep)
 
         if thermostat is None:
             self.thermostat = Thermostat()
         else:
             if (
                 thermostat.__class__.__name__ is ("ThermoPILE_G" or "ThermoNMGLEG ")
             ) and (len(fixatoms) > 0):
                 softexit.trigger(
                     status="bad",
                     message="!! Sorry, fixed atoms and global thermostat on the centroid not supported. Use a local thermostat. !!",
                 )
             self.thermostat = thermostat
 
         if nmts is None or len(nmts) == 0:
-            dd(self).nmts = depend_array(name="nmts", value=np.asarray([1], int))
+            self._nmts = depend_array(name="nmts", value=np.asarray([1], int))
         else:
-            dd(self).nmts = depend_array(name="nmts", value=np.asarray(nmts, int))
+            self._nmts = depend_array(name="nmts", value=np.asarray(nmts, int))
 
         if barostat is None:
             self.barostat = Barostat()
         else:
             self.barostat = barostat
         self.enstype = mode
         if self.enstype == "nve":
@@ -107,22 +105,26 @@
             self.integrator = SCIntegrator()
         elif self.enstype == "scnpt":
             self.integrator = SCNPTIntegrator()
         else:
             self.integrator = DummyIntegrator()
 
         # splitting mode for the integrators
-        dd(self).splitting = depend_value(name="splitting", value=splitting)
+        self._splitting = depend_value(name="splitting", value=splitting)
 
         # constraints
         self.fixcom = fixcom
         if fixatoms is None:
             self.fixatoms = np.zeros(0, int)
+            self.fixatoms3 = np.zeros(0, int)
         else:
             self.fixatoms = fixatoms
+            self.fixatoms3 = np.array(
+                [[3 * i, 3 * i + 1, 3 * i + 2] for i in self.fixatoms]
+            ).flatten()
 
     def get_fixdof(self):
         """Calculate the number of fixed degrees of freedom, required for
         temperature and pressure calculations.
         """
 
         fixdof = len(self.fixatoms) * 3 * self.beads.nbeads
@@ -154,60 +156,53 @@
 
         # Checks if the number of mts levels is equal to the dimensionality of the mts weights.
         if len(self.nmts) != self.forces.nmtslevels:
             raise ValueError(
                 "The number of mts levels for the integrator does not agree with the mts_weights of the force components."
             )
 
-        # Strips off depend machinery for easier referencing.
-        dself = dd(self)
-        dthrm = dd(self.thermostat)
-        dbaro = dd(self.barostat)
-        dnm = dd(self.nm)  # noqa
-        dens = dd(self.ensemble)
-
         # n times the temperature (for path integral partition function)
-        dself.ntemp = depend_value(
-            name="ntemp", func=self.get_ntemp, dependencies=[dens.temp]
+        self._ntemp = depend_value(
+            name="ntemp", func=self.get_ntemp, dependencies=[self.ensemble._temp]
         )
 
         # fixed degrees of freedom count
         fixdof = self.get_fixdof()
 
         # first makes sure that the thermostat has the correct temperature and timestep, then proceeds with binding it.
-        dpipe(dself.ntemp, dthrm.temp)
+        dpipe(self._ntemp, self.thermostat._temp)
 
         # depending on the kind, the thermostat might work in the normal mode or the bead representation.
         self.thermostat.bind(beads=self.beads, nm=self.nm, prng=prng, fixdof=fixdof)
 
         # first makes sure that the barostat has the correct stress and timestep, then proceeds with binding it.
-        dpipe(dself.ntemp, dbaro.temp)
-        dpipe(dens.pext, dbaro.pext)
-        dpipe(dens.stressext, dbaro.stressext)
+        dpipe(self._ntemp, self.barostat._temp)
+        dpipe(self.ensemble._pext, self.barostat._pext)
+        dpipe(self.ensemble._stressext, self.barostat._stressext)
         self.barostat.bind(
             beads,
             nm,
             cell,
             bforce,
             bias=self.ensemble.bias,
             prng=prng,
             fixdof=fixdof,
             nmts=len(self.nmts),
         )
 
         # now that the timesteps are decided, we proceed to bind the integrator.
         self.integrator.bind(self)
 
-        self.ensemble.add_econs(dthrm.ethermo)
-        self.ensemble.add_econs(dbaro.ebaro)
+        self.ensemble.add_econs(self.thermostat._ethermo)
+        self.ensemble.add_econs(self.barostat._ebaro)
 
         # adds the potential, kinetic energy and the cell Jacobian to the ensemble
-        self.ensemble.add_xlpot(dbaro.pot)
-        self.ensemble.add_xlpot(dbaro.cell_jacobian)
-        self.ensemble.add_xlkin(dbaro.kin)
+        self.ensemble.add_xlpot(self.barostat._pot)
+        self.ensemble.add_xlpot(self.barostat._cell_jacobian)
+        self.ensemble.add_xlkin(self.barostat._kin)
 
         # applies constraints immediately after initialization.
         self.integrator.pconstraints()
 
         # TODO THOROUGH CLEAN-UP AND CHECK
         if (
             self.enstype == "nvt"
@@ -238,15 +233,18 @@
     def step(self, step=None):
         """Advances the dynamics by one time step"""
 
         self.integrator.step(step)
         self.ensemble.time += self.dt  # increments internal time
 
 
-class DummyIntegrator(dobject):
+dproperties(Dynamics, ["dt", "nmts", "splitting", "ntemp"])
+
+
+class DummyIntegrator:
     """No-op integrator for (PI)MD"""
 
     def __init__(self):
         pass
 
     def get_qdt(self):
         return self.dt * 0.5 / self.inmts
@@ -277,51 +275,54 @@
         self.forces = motion.forces
         self.prng = motion.prng
         self.nm = motion.nm
         self.thermostat = motion.thermostat
         self.barostat = motion.barostat
         self.fixcom = motion.fixcom
         self.fixatoms = motion.fixatoms
+        self.fixatoms3 = motion.fixatoms3
         self.enstype = motion.enstype
 
-        dself = dd(self)
-        dmotion = dd(motion)
-
         # no need to dpipe these are really just references
-        dself.splitting = dmotion.splitting
-        dself.dt = dmotion.dt
-        dself.nmts = dmotion.nmts
+        self._splitting = motion._splitting
+        self._dt = motion._dt
+        self._nmts = motion._nmts
 
         # total number of iteration in the inner-most MTS loop
-        dself.inmts = depend_value(name="inmts", func=lambda: np.prod(self.nmts))
-        dself.nmtslevels = depend_value(name="nmtslevels", func=lambda: len(self.nmts))
+        self._inmts = depend_value(name="inmts", func=lambda: np.prod(self.nmts))
+        self._nmtslevels = depend_value(name="nmtslevels", func=lambda: len(self.nmts))
         # these are the time steps to be used for the different parts of the integrator
-        dself.qdt = depend_value(
+        self._qdt = depend_value(
             name="qdt",
             func=self.get_qdt,
-            dependencies=[dself.splitting, dself.dt, dself.inmts],
+            dependencies=[self._splitting, self._dt, self._inmts],
         )  # positions
-        dself.pdt = depend_array(
+        self._qdt_on_m = depend_array(
+            name="qdt_on_m",
+            value=np.zeros(3 * self.beads.natoms),
+            func=lambda: self.qdt / dstrip(self.beads.m3)[0],
+        )
+        self._pdt = depend_array(
             name="pdt",
             func=self.get_pdt,
             value=np.zeros(len(self.nmts)),
-            dependencies=[dself.splitting, dself.dt, dself.nmts],
+            dependencies=[self._splitting, self._dt, self._nmts],
         )  # momenta
-        dself.tdt = depend_value(
+        self._tdt = depend_value(
             name="tdt",
             func=self.get_tdt,
-            dependencies=[dself.splitting, dself.dt, dself.nmts],
+            dependencies=[self._splitting, self._dt, self._nmts],
         )  # thermostat
 
-        dpipe(dself.qdt, dd(self.nm).dt)
-        dpipe(dself.dt, dd(self.barostat).dt)
-        dpipe(dself.qdt, dd(self.barostat).qdt)
-        dpipe(dself.pdt, dd(self.barostat).pdt)
-        dpipe(dself.tdt, dd(self.barostat).tdt)
-        dpipe(dself.tdt, dd(self.thermostat).dt)
+        dpipe(self._qdt, self.nm._dt)
+        dpipe(self._dt, self.barostat._dt)
+        dpipe(self._qdt, self.barostat._qdt)
+        dpipe(self._pdt, self.barostat._pdt)
+        dpipe(self._tdt, self.barostat._tdt)
+        dpipe(self._tdt, self.thermostat._dt)
 
         if motion.enstype == "sc" or motion.enstype == "scnpt":
             # coefficients to get the (baseline) trotter to sc conversion
             self.coeffsc = np.ones((self.beads.nbeads, 3 * self.beads.natoms), float)
             self.coeffsc[::2] /= -3.0
             self.coeffsc[1::2] /= 3.0
 
@@ -349,52 +350,43 @@
         added to the thermostat heat energy, as it is assumed that the centre of
         mass motion is due to the thermostat.
 
         If there is a choice of thermostats, the thermostat
         connected to the centroid is chosen.
         """
 
+        beads = self.beads
         if self.fixcom:
-            na3 = self.beads.natoms * 3
-            nb = self.beads.nbeads
-            p = dstrip(self.beads.p)
-            m = dstrip(self.beads.m3)[:, 0:na3:3]
-            M = self.beads[0].M
+            nb = beads.nbeads
+            p = dstrip(beads.p)
+            m3 = dstrip(beads.m3).reshape((-1, 3))
+            M = beads[0].M
             Mnb = M * nb
 
-            dens = 0
-            for i in range(3):
-                pcom = p[:, i:na3:3].sum()
-                dens += pcom**2
-                pcom /= Mnb
-                self.beads.p[:, i:na3:3] -= m * pcom
+            vcom = np.sum(p.reshape(-1, 3), axis=0) / Mnb
+            beads.p -= (m3 * vcom).reshape(nb, -1)
 
-            self.ensemble.eens += dens * 0.5 / Mnb
+            self.ensemble.eens += np.sum(vcom**2) * 0.5 * Mnb  # COM kinetic energy
 
         if len(self.fixatoms) > 0:
-            for bp in self.beads.p:
-                m = dstrip(self.beads.m)
-                self.ensemble.eens += 0.5 * np.dot(
-                    bp[self.fixatoms * 3], bp[self.fixatoms * 3] / m[self.fixatoms]
-                )
-                self.ensemble.eens += 0.5 * np.dot(
-                    bp[self.fixatoms * 3 + 1],
-                    bp[self.fixatoms * 3 + 1] / m[self.fixatoms],
-                )
-                self.ensemble.eens += 0.5 * np.dot(
-                    bp[self.fixatoms * 3 + 2],
-                    bp[self.fixatoms * 3 + 2] / m[self.fixatoms],
-                )
-                bp[self.fixatoms * 3] = 0.0
-                bp[self.fixatoms * 3 + 1] = 0.0
-                bp[self.fixatoms * 3 + 2] = 0.0
+            m3 = dstrip(beads.m3)
+            p = dstrip(beads.p)
+            fixatoms3 = self.fixatoms3
+
+            self.ensemble.eens += 0.5 * np.sum(p[:, fixatoms3] ** 2 / m3[:, fixatoms3])
+            beads.p[:, fixatoms3] = 0.0
 
 
-class NVEIntegrator(DummyIntegrator):
+dproperties(
+    DummyIntegrator,
+    ["splitting", "nmts", "dt", "inmts", "nmtslevels", "qdt", "pdt", "tdt", "qdt_on_m"],
+)
 
+
+class NVEIntegrator(DummyIntegrator):
     """Integrator object for constant energy simulations.
 
     Has the relevant conserved quantity and normal mode propagator for the
     constant energy ensemble. Note that a temperature of some kind must be
     defined so that the spring potential can be calculated.
 
     Attributes:
@@ -407,24 +399,22 @@
             potential energy, and the spring potential energy.
     """
 
     def pstep(self, level=0):
         """Velocity Verlet momentum propagator."""
 
         # halfdt/alpha
-        self.beads.p += self.forces.forces_mts(level) * self.pdt[level]
-        if level == 0:  # adds bias in the outer loop
-            self.beads.p += dstrip(self.bias.f) * self.pdt[level]
+        self.beads.p[:] += dstrip(self.forces.mts_forces[level].f) * self.pdt[level]
+        if level == 0 and self.ensemble.has_bias:  # adds bias in the outer loop
+            self.beads.p[:] += dstrip(self.bias.f) * self.pdt[level]
 
     def qcstep(self):
         """Velocity Verlet centroid position propagator."""
         # dt/inmts
-        self.nm.qnm[0, :] += (
-            dstrip(self.nm.pnm)[0, :] / dstrip(self.beads.m3)[0] * self.qdt
-        )
+        self.nm.qnm[0, :] += dstrip(self.nm.pnm)[0, :] * dstrip(self.qdt_on_m)
 
     # now the idea is that for BAOAB the MTS should work as follows:
     # take the BAB MTS, and insert the O in the very middle. This might imply breaking a A step in two, e.g. one could have
     # Bbabb(a/2) O (a/2)bbabB
     def mtsprop_ba(self, index):
         """Recursive MTS step"""
 
@@ -495,15 +485,14 @@
     def step(self, step=None):
         """Does one simulation time step."""
 
         self.mtsprop(0)
 
 
 class NVTIntegrator(NVEIntegrator):
-
     """Integrator object for constant temperature simulations.
 
     Has the relevant conserved quantity and normal mode propagator for the
     constant temperature ensemble. Contains a thermostat object containing the
     algorithms to keep the temperature constant.
 
     Attributes:
@@ -585,15 +574,14 @@
             self.nm.pnm[0], self.nm.pnm[0] / self.nm.dynm3[0]
         )
         self.nm.pnm[0, :] = 0.0
         self.pconstraints()
 
 
 class NPTIntegrator(NVTIntegrator):
-
     """Integrator object for constant pressure simulations.
 
     Has the relevant conserved quantity and normal mode propagator for the
     constant pressure ensemble. Contains a thermostat object containing the
     algorithms to keep the temperature constant, and a barostat to keep the
     pressure constant.
     """
@@ -606,18 +594,18 @@
         if self._stresscheck and np.array_equiv(
             dstrip(self.forces.vir), np.zeros(len(self.forces.vir))
         ):
             warning(
                 "Forcefield returned a zero stress tensor. NPT simulation will likely make no sense",
                 verbosity.low,
             )
-            if verbosity.medium:
-                raise ValueError(
-                    "Zero stress terminates simulation for medium verbosity and above."
-                )
+            # if verbosity.medium: will uncomment one day
+            #    raise ValueError(
+            #        "Zero stress terminates simulation for medium verbosity and above."
+            #    )
 
         self._stresscheck = False
 
         self.barostat.pstep(level)
         super(NPTIntegrator, self).pstep(level)
         # self.pconstraints()
 
@@ -631,15 +619,14 @@
 
         self.thermostat.step()
         self.barostat.thermostat.step()
         # self.pconstraints()
 
 
 class NSTIntegrator(NPTIntegrator):
-
     """Ensemble object for constant pressure simulations.
 
     Has the relevant conserved quantity and normal mode propagator for the
     constant pressure ensemble. Contains a thermostat object containing the
     algorithms to keep the temperature constant, and a barostat to keep the
     pressure constant.
 
@@ -688,26 +675,26 @@
         bforce: The forcefield object from which the force and virial are
             taken.
         prng: The random number generator object which controls random number
             generation.
         """
 
         super(SCIntegrator, self).bind(mover)
-        self.ensemble.add_econs(dd(self.forces).potsc)
-        self.ensemble.add_xlpot(dd(self.forces).potsc)
+        self.ensemble.add_econs(self.forces._potsc)
+        self.ensemble.add_xlpot(self.forces._potsc)
 
     def pstep(self, level=0):
         """Velocity Verlet monemtum propagator."""
 
         if level == 0:
             # bias goes in the outer loop
             self.beads.p += dstrip(self.bias.f) * self.pdt[level]
         # just integrate the Trotter force scaled with the SC coefficients, which is a cheap approx to the SC force
         self.beads.p += (
-            self.forces.forces_mts(level)
+            self.forces.mts_forces[level].f
             * (1.0 + self.forces.coeffsc_part_1)
             * self.pdt[level]
         )
 
     def step(self, step=None):
         # the |f|^2 term is considered to be slowest (for large enough P) and is integrated outside everything.
         # if nmts is not specified, this is just the same as doing the full SC integration
```

### Comparing `ipi-2.6.0/ipi/engine/motion/geop.py` & `ipi-2.6.3/ipi/engine/motion/geop.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # See the "licenses" directory for full license information.
 
 
 import numpy as np
 import time
 
 from ipi.engine.motion import Motion
-from ipi.utils.depend import dstrip, dobject
+from ipi.utils.depend import dstrip
 from ipi.utils.softexit import softexit
 from ipi.utils.mintools import min_brent, BFGS, BFGSTRM, L_BFGS, Damped_BFGS
 from ipi.utils.messages import verbosity, info
 
 
 __all__ = ["GeopMotion"]
 
@@ -178,15 +178,14 @@
                     verbosity.high,
                 )
         else:
             self.optimizer.step(step)
 
 
 class LineMapper(object):
-
     """Creation of the one-dimensional function that will be minimized.
     Used in steepest descent and conjugate gradient minimizers.
 
     Attributes:
         x0: initial position
         d: move direction
     """
@@ -232,15 +231,14 @@
         g = -np.dot(
             dstrip(self.dforces.f[:, self.fixatoms_mask]).flatten(), self.d.flatten()
         )  # Gradient
         return e, g
 
 
 class GradientMapper(object):
-
     """Creation of the multi-dimensional function that will be minimized.
     Used in the BFGS and L-BFGS minimizers.
 
     Attributes:
         dbeads:   copy of the bead object
         dcell:   copy of the cell object
         dforces: copy of the forces object
@@ -269,15 +267,15 @@
         self.fcount += 1
         self.dbeads.q[:, self.fixatoms_mask] = x
         e = self.dforces.pot  # Energy
         g = -self.dforces.f[:, self.fixatoms_mask]  # Gradient
         return e, g
 
 
-class DummyOptimizer(dobject):
+class DummyOptimizer:
     """Dummy class for all optimization classes"""
 
     def __init__(self):
         """initialises object for LineMapper (1-d function)
         and for GradientMapper (multi-dimensional function)
         """
 
@@ -479,17 +477,17 @@
                 self.big_step,
                 self.ls_options["tolerance"] * self.tolerances["energy"],
                 self.ls_options["iter"],
             )
 
             # Restore dimensionality of d and invhessian
             self.d[:, self.gm.fixatoms_mask] = masked_d
-            self.invhessian[
-                np.ix_(self.gm.fixatoms_mask, self.gm.fixatoms_mask)
-            ] = masked_invhessian
+            self.invhessian[np.ix_(self.gm.fixatoms_mask, self.gm.fixatoms_mask)] = (
+                masked_invhessian
+            )
 
         else:
             fdf0 = (self.old_u, -self.old_f)
 
             # Do one iteration of BFGS
             # The invhessian and the directions are updated inside.
             BFGS(
@@ -574,17 +572,17 @@
                 masked_hessian,
                 self.tr,
                 self.gm,
                 self.big_step,
             )
 
             # Restore dimensionality of the hessian
-            self.hessian[
-                np.ix_(self.gm.fixatoms_mask, self.gm.fixatoms_mask)
-            ] = masked_hessian
+            self.hessian[np.ix_(self.gm.fixatoms_mask, self.gm.fixatoms_mask)] = (
+                masked_hessian
+            )
         else:
             # Make one step. ( A step is finished when a movement is accepted)
             BFGSTRM(
                 self.old_x,
                 self.old_u,
                 self.old_f,
                 self.hessian,
@@ -792,17 +790,17 @@
                 self.gm,
                 fdf0,
                 masked_invhessian,
                 self.big_step,
             )
 
             # Restore dimensionality of the invhessian
-            self.invhessian[
-                np.ix_(self.gm.fixatoms_mask, self.gm.fixatoms_mask)
-            ] = masked_invhessian
+            self.invhessian[np.ix_(self.gm.fixatoms_mask, self.gm.fixatoms_mask)] = (
+                masked_invhessian
+            )
 
         else:
             fdf0 = (self.old_u, -self.old_f)
 
             # Do one iteration of Damped_BFGS
             # The invhessian and the directions are updated inside.
             Damped_BFGS(
```

### Comparing `ipi-2.6.0/ipi/engine/motion/instanton.py` & `ipi-2.6.3/ipi/engine/motion/instanton.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,34 +6,41 @@
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 
 import numpy as np
+import warnings
+
+np.set_printoptions(suppress=True, linewidth=1000)
 import time
 import sys
+from importlib import util
 
+from ipi.engine.beads import Beads
+from ipi.engine.normalmodes import NormalModes
 from ipi.engine.motion import Motion
-from ipi.utils.depend import dstrip, dobject
+from ipi.utils.depend import dstrip
 from ipi.utils.softexit import softexit
 from ipi.utils.messages import verbosity, info
 from ipi.utils import units
 from ipi.utils.mintools import nichols, Powell
 from ipi.engine.motion.geop import L_BFGS
 from ipi.utils.instools import (
     banded_hessian,
     invmul_banded,
     red2comp,
     get_imvector,
     print_instanton_geo,
+    Fix,
 )
 from ipi.utils.instools import print_instanton_hess, diag_banded, ms_pathway
 from ipi.utils.hesstools import get_hessian, clean_hessian, get_dynmat
-from ipi.engine.beads import Beads
+
 
 __all__ = ["InstantonMotion"]
 
 
 class InstantonMotion(Motion):
     """Instanton motion class.
 
@@ -88,31 +95,36 @@
         max_ms=0.0,
         discretization=np.zeros(0, float),
         alt_out=1,
         prefix="instanton",
         delta=np.zeros(0, float),
         hessian_init=None,
         hessian=np.eye(0, 0, 0, float),
+        fric_hessian=np.eye(0, 0, 0, float),
         hessian_update=None,
         hessian_asr=None,
         qlist_lbfgs=np.zeros(0, float),
         glist_lbfgs=np.zeros(0, float),
         scale_lbfgs=1,
         corrections_lbfgs=5,
         ls_options={"tolerance": 1e-1, "iter": 100},
         old_direction=np.zeros(0, float),
         hessian_final="False",
         energy_shift=np.zeros(0, float),
+        friction=False,
+        frictionSD=True,
+        eta=np.eye(0, 0, 0, float),
+        fric_spec_dens=np.zeros(0, float),
+        fric_spec_dens_ener=0.0,
     ):
         """Initialises InstantonMotion."""
 
         super(InstantonMotion, self).__init__(fixcom=fixcom, fixatoms=fixatoms)
 
         self.options = {}  # Optimization options
-        self.optarrays = {}  # Optimization arrays
 
         # Optimization mode
         self.options["mode"] = mode
 
         # Generic optimization
         # self.big_step = biggest_step
         # self.tolerances = tolerances
@@ -121,14 +133,24 @@
         self.options["save"] = alt_out
         self.options["prefix"] = prefix
         self.options["hessian_final"] = hessian_final
 
         self.options["max_e"] = max_e
         self.options["max_ms"] = max_ms
         self.options["discretization"] = discretization
+        self.options["friction"] = friction
+        if not friction:
+            self.options["frictionSD"] = False
+        else:
+            self.options["frictionSD"] = frictionSD
+
+        self.options["fric_spec_dens"] = fric_spec_dens
+        self.options["fric_spec_dens_ener"] = fric_spec_dens_ener
+
+        self.optarrays = {}  # Optimization arrays
         self.optarrays["big_step"] = biggest_step
         self.optarrays["energy_shift"] = energy_shift
         self.optarrays["delta"] = delta
         self.optarrays["old_x"] = old_pos
         self.optarrays["old_u"] = old_pot
         self.optarrays["old_f"] = old_force
 
@@ -144,245 +166,162 @@
             self.options["opt"] = opt
 
         if (
             self.options["opt"] == "nichols"
             or self.options["opt"] == "NR"
             or self.options["opt"] == "lanczos"
         ):
+            if self.options["friction"]:  # and not self.options["frictionSD"]:
+                self.options["eta0"] = eta
+
             self.options["hessian_update"] = hessian_update
             self.options["hessian_asr"] = hessian_asr
             self.options["hessian_init"] = hessian_init
             self.optarrays["hessian"] = hessian
+            if self.options["friction"] and self.options["frictionSD"]:
+                self.optarrays["fric_hessian"] = fric_hessian
 
             if self.options["opt"] == "nichols":
                 self.optimizer = NicholsOptimizer()
-            elif self.options["opt"] == "NR":
-                self.optimizer = NROptimizer()
             else:
-                self.optimizer = LanczosOptimizer()
+                if self.options["friction"]:
+                    raise ValueError(
+                        "\nPlease select nichols opt algorithm for an instanton calculation with friction\n"
+                    )
+                if self.options["opt"] == "NR":
+                    self.optimizer = NROptimizer()
+                else:
+                    self.optimizer = LanczosOptimizer()
 
         elif self.options["opt"] == "lbfgs":
             self.optimizer = LBFGSOptimizer()
             self.optarrays["hessian"] = hessian  # Only for initial (to spread) or final
             self.options["hessian_asr"] = hessian_asr
 
             self.options["corrections"] = corrections_lbfgs
             self.options["scale"] = scale_lbfgs
             self.options["ls_options"] = ls_options
 
             self.optarrays["qlist"] = qlist_lbfgs
             self.optarrays["glist"] = glist_lbfgs
             self.optarrays["d"] = old_direction
 
-        if self.options["opt"] == "NR":
+        if self.options["opt"] == "NR" or self.options["opt"] == "lanczos":
             info(
-                "Note that we need scipy to use NR. If storage and diagonalization of the full hessian is not a "
+                "Note that we need scipy to use NR or lanczos. If storage and diagonalization of the full hessian is not a "
                 "problem use nichols even though it may not be as efficient.",
                 verbosity.low,
             )
+            found = util.find_spec("scipy")
+            if found is None:
+                softexit.trigger(
+                    "Scipy is required to use NR or lanczos optimization but could not be found"
+                )
+
+        if self.options["friction"]:
+            found = util.find_spec("scipy")
+            if found is None:
+                softexit.trigger(
+                    "Scipy is required to use friction in a instanton calculation but could not be found"
+                )
 
     def bind(self, ens, beads, nm, cell, bforce, prng, omaker):
         """Binds beads, cell, bforce and prng to InstantonMotion
 
         Args:
         beads: The beads object from which the bead positions are taken.
         nm: A normal modes object used to do the normal modes transformation.
         cell: The cell object from which the system box is taken.
         bforce: The forcefield object from which the force and virial are taken.
         prng: The random number generator object which controls random number generation.
         """
 
         super(InstantonMotion, self).bind(ens, beads, nm, cell, bforce, prng, omaker)
-        # Binds optimizer
+
+        # Redefine normal modes
+        self.nm = NormalModes(
+            transform_method="matrix", open_paths=np.arange(self.beads.natoms)
+        )
+
+        self.nm.bind(self.ensemble, self, Beads(self.beads.natoms, self.beads.nbeads))
+        if self.options["mode"] == "rate":
+            self.rp_factor = 2
+        elif self.options["mode"] == "splitting":
+            self.rp_factor = 1
 
         self.optimizer.bind(self)
 
     def step(self, step=None):
         self.optimizer.step(step)
 
 
-class Fix(object):
-    """Class that applies a fixatoms type constrain"""
-
-    def __init__(self, natoms, fixatoms, nbeads=1):
-        self.natoms = natoms
-        self.nbeads = nbeads
-        self.fixatoms = fixatoms
-
-        self.mask0 = np.delete(np.arange(self.natoms), self.fixatoms)
-
-        mask1 = np.ones(3 * self.natoms, dtype=bool)
-        for i in range(3):
-            mask1[3 * self.fixatoms + i] = False
-        self.mask1 = np.arange(3 * self.natoms)[mask1]
-
-        mask2 = np.tile(mask1, self.nbeads)
-        self.mask2 = np.arange(3 * self.natoms * self.nbeads)[mask2]
-
-    def get_mask(self, m):
-        if m == 0:
-            return self.mask0
-        elif m == 1:
-            return self.mask1
-        elif m == 2:
-            return self.mask2
-        else:
-            raise ValueError("Mask number not valid")
-
-    def get_active_array(self, arrays):
-        """Functions that gets the subarray corresponding to the active degrees-of-freedom of the
-        full dimensional array"""
-
-        activearrays = {}
-        for key in arrays:
-            if (
-                key == "old_u"
-                or key == "big_step"
-                or key == "delta"
-                or key == "energy_shift"
-                or key == "initial_hessian"
-            ):
-                t = -1
-            elif key == "old_x" or key == "old_f" or key == "d":
-                t = 1
-            elif key == "hessian":
-                t = 2
-            elif key == "qlist" or key == "glist":
-                t = 3
-            else:
-                raise ValueError(
-                    "@get_active_array: There is an array that we can't recognize"
-                )
-
-            activearrays[key] = self.get_active_vector(arrays[key], t)
-
-        return activearrays
-
-    def get_full_vector(self, vector, t):
-        """Set 0 the degrees of freedom (dof) corresponding to the fix atoms
-        IN:
-            fixatoms   indexes of the fixed atoms
-            vector     vector to be reduced
-            t          type of array:
-                type=-1 : do nothing
-                type=0 : names (natoms )
-                type=1 : pos , force or m3 (nbeads,dof)
-                type=2 : hessian (dof, nbeads*dof)
-                type=3 : qlist or glist (corrections, nbeads*dof)
-        OUT:
-            clean_vector  reduced vector
-        """
-        if len(self.fixatoms) == 0 or t == -1:
-            return vector
-
-        if t == 1:
-            full_vector = np.zeros((self.nbeads, 3 * self.natoms))
-            full_vector[:, self.get_mask(1)] = vector
-
-            return full_vector
-
-        elif t == 2:
-            full_vector = np.zeros((3 * self.natoms, 3 * self.natoms * self.nbeads))
-
-            ii = 0
-            for i in self.get_mask(1):
-                full_vector[i, self.get_mask(2)] = vector[ii]
-                ii += 1
-
-            return full_vector
-
-        elif t == 3:
-            full_vector = np.zeros((vector.shape[0], 3 * self.natoms * self.nbeads))
-            full_vector[:, self.fix.get_mask(2)] = vector
-
-            return full_vector
-
-        else:
-            raise ValueError("@apply_fix_atoms: type number is not valid")
-
-    def get_active_vector(self, vector, t):
-        """Delete the degrees of freedom (dof) corresponding to the fix atoms
-        IN:
-            fixatoms   indexes of the fixed atoms
-            vector     vector to be reduced
-            t          type of array:
-                type=-1 : do nothing
-                type=0 : names (natoms )
-                type=1 : pos , force or m3 (nbeads,dof)
-                type=2 : hessian (dof, nbeads*dof)
-                type=3 : qlist or glist (corrections, nbeads*dof)
-        OUT:
-            clean_vector  reduced vector
-        """
-        if len(self.fixatoms) == 0 or t == -1:
-            return vector
-        if t == 0:
-            return vector[self.mask0]
-        elif t == 1:
-            return vector[:, self.mask1]
-        elif t == 2:
-            aux = vector[self.mask1]
-            return aux[:, self.mask2]
-        elif t == 3:
-            return vector[:, self.mask2]
-        else:
-            raise ValueError("@apply_fix_atoms: type number is not valid")
-
-
-class GradientMapper(object):
-
+class PesMapper(object):
     """Creation of the multi-dimensional function to compute the physical potential and forces
 
     Attributes:
         dbeads:  copy of the bead object
         dcell:   copy of the cell object
         dforces: copy of the forces object
     """
 
     def __init__(self):
         self.fcount = 0
         pass
 
-    def bind(self, dumop, discretization, max_ms, max_e):
-        self.dbeads = dumop.beads.copy()
-        self.dcell = dumop.cell.copy()
-        self.dforces = dumop.forces.copy(self.dbeads, self.dcell)
-        self.fix = Fix(dumop.beads.natoms, dumop.fixatoms, dumop.beads.nbeads)
-        self.set_coef(discretization)
+    def bind(self, mapper):
+        self.dbeads = mapper.beads.copy()
+        self.dcell = mapper.cell.copy()
+        self.dforces = mapper.forces.copy(self.dbeads, self.dcell)
+
+        # self.nm = mapper.nm
+        # self.rp_factor = mapper.rp_factor
+        if self.dbeads.nbeads > 1:
+            self.C = mapper.nm.transform._b2o_nm
+        else:
+            self.C = 1
+
+        self.omegak = mapper.rp_factor * mapper.nm.get_o_omegak()
+
+        self.fix = mapper.fix
+        self.coef = mapper.coef
+
+        max_ms = mapper.options["max_ms"]
+        max_e = mapper.options["max_e"]
+
         if max_ms > 0 or max_e > 0:
             self.spline = True
 
             if max_ms > 0:
                 self.max_ms = max_ms
             else:
                 self.max_ms = 1000000
             if max_e > 0:
                 self.max_e = max_e
             else:
                 self.max_e = 10000000
         else:
             self.spline = False
 
-    def set_coef(self, coef):
-        self.coef = coef.reshape(-1, 1)
+    def initialize(self, q, forces):
+        """Initialize potential and forces"""
+        self.save(forces.pots, -forces.f)
 
     def set_pos(self, x):
         """Set the positions"""
         self.dbeads.q = x
 
     def save(self, e, g):
+        """Stores potential and forces in this class for convenience"""
         self.pot = e
         self.f = -g
 
-    def __call__(self, x, full=False, new_disc=True):
-        """computes energy and gradient for optimization step"""
-        self.fcount += 1
-        full_q = x.copy()
-        full_mspath = ms_pathway(full_q, self.dbeads.m3)
-
+    def interpolation(self, full_q, full_mspath, get_all_info=False):
+        """Creates the reduced bead object from which energy and forces will be
+        computed and interpolates the results to the full size
+        """
         if self.spline:
             try:
                 from scipy.interpolate import interp1d
             except ImportError:
                 softexit.trigger(
                     status="bad", message="Scipy required to use  max_ms >0"
                 )
@@ -415,111 +354,447 @@
         reduced_b.q[:] = full_q[indexes]
         reduced_b.m[:] = self.dbeads.m
         reduced_b.names[:] = self.dbeads.names
 
         reduced_cell = self.dcell.copy()
         reduced_forces = self.dforces.copy(reduced_b, reduced_cell)
 
+        # Evaluate energy and forces (and maybe friction)
         rpots = reduced_forces.pots  # reduced energy
         rforces = reduced_forces.f  # reduced gradient
 
         # Interpolate if necessary to get full pot and forces
         if self.spline:
             red_mspath = full_mspath[indexes]
             spline = interp1d(red_mspath, rpots.T, kind="cubic")
             full_pot = spline(full_mspath).T
             spline = interp1d(red_mspath, rforces.T, kind="cubic")
             full_forces = spline(full_mspath).T
         else:
             full_pot = rpots
             full_forces = rforces
+        if get_all_info:
+            return full_pot, full_forces, indexes, reduced_forces
+        else:
+            return full_pot, full_forces
 
-        # This forces the update of the forces
+    def __call__(self, x, new_disc=True):
+        """Computes energy and gradient for optimization step"""
+        self.fcount += 1
+        full_q = x.copy()
+        full_mspath = ms_pathway(full_q, self.dbeads.m3)
+        full_pot, full_forces = self.interpolation(full_q, full_mspath)
         self.dbeads.q[:] = x[:]
+
         self.dforces.transfer_forces_manual([full_q], [full_pot], [full_forces])
+        info("UPDATE of forces and extras", verbosity.debug)
 
-        # e = self.dforces.pot   # Energy
-        # g = -self.dforces.f    # Gradient
-        e = np.sum(full_pot)  # Energy
-        g = -full_forces  # Gradient
+        self.save(full_pot, -full_forces)
+        return self.evaluate()
 
-        self.save(full_pot, g)
+    def evaluate(self):
+        """Evaluate the energy and forces including:
+        - non uniform discretization
+        - friction term (if required)
+        """
 
-        if not full:
-            g = self.fix.get_active_vector(g, 1)
+        e = self.pot.copy()
+        g = -self.f.copy()
 
-        # APPLY OTHERS CONSTRAIN?
+        e = e * (self.coef[1:] + self.coef[:-1]) / 2
+        g = g * (self.coef[1:] + self.coef[:-1]) / 2
 
-        # Discretization
-        if new_disc:
-            e = e * (self.coef[1:] + self.coef[:-1]) / 2
-            g = g * (self.coef[1:] + self.coef[:-1]) / 2
+        return e, g
+
+
+class FrictionMapper(PesMapper):
+    """Creation of the multi-dimensional function to compute the physical potential and forces,
+    as well as the friction terms"""
+
+    def __init__(self, frictionSD, eta0):
+        super(FrictionMapper, self).__init__()
+        self.frictionSD = frictionSD
+        self.eta0 = eta0
+
+    def bind(self, mapper):
+        super(FrictionMapper, self).bind(mapper)
+        from scipy.interpolate import interp1d
+        from scipy.linalg import sqrtm
+        from scipy.integrate import quad
+
+        self.sqrtm = sqrtm
+        self.quad = quad
+        self.interp1d = interp1d
+
+    def save(self, e, g, eta=None):
+        """Stores potential and forces in this class for convenience"""
+        super(FrictionMapper, self).save(e, g)
+        self.eta = eta
+
+    def initialize(self, q, forces):
+        """Initialize potential, forces and friction"""
+
+        if self.frictionSD:
+            eta = np.array(forces.extras["friction"]).reshape(
+                (q.shape[0], q.shape[1], q.shape[1])
+            )
+        else:
+            eta = np.zeros((q.shape[0], q.shape[1], q.shape[1]))
+            for i in range(self.dbeads.nbeads):
+                eta[i] = self.eta0
+
+        self.check_eta(eta)
+
+        self.save(forces.pots, -forces.f, eta)
+
+    def check_eta(self, eta):
+        for i in range(self.dbeads.nbeads):
+            assert (
+                eta[i] - eta[i].T
+                == np.zeros((self.dbeads.natoms * 3, self.dbeads.natoms * 3))
+            ).all()
+        with warnings.catch_warnings():
+            warnings.filterwarnings("error")
+            try:
+                self.sqrtm(
+                    eta[i] + np.eye(self.dbeads.natoms * 3) * 0.000000000001
+                )  # dgdq = s ** 0.5 -> won't work for multiD
+            except Warning:
+                print(eta[i])
+                softexit.trigger("The provided friction is not positive definite")
+
+    def set_fric_spec_dens(self, fric_spec_dens_data, fric_spec_dens_ener):
+        """Computes and sets the laplace transform of the friction tensor"""
+        # from ipi.utils.mathtools import LT_friction
+
+        # from scipy.interpolate import interp1d
+        if len(fric_spec_dens_data) == 0:
+            LT_fric_spec_dens = np.ones((1000, 2))
+            LT_fric_spec_dens[:, 0] = np.arange(self.omegak.shape)
+        else:
+            invcm2au = units.unit_to_internal("frequency", "inversecm", 1)
+
+            # We perform the spline in inversecm for numerical reasons
+            freq = fric_spec_dens_data[:, 0] * invcm2au
+            spline = self.interp1d(
+                freq,
+                fric_spec_dens_data[:, 1],
+                kind="cubic",
+                fill_value=0.0,
+                bounds_error=False,
+            )
+
+            if fric_spec_dens_ener == 0 or fric_spec_dens_ener / invcm2au < freq[0]:
+                norm = 1.0  # spline(freq[0])*freq[0]*invcm2au
+            elif fric_spec_dens_ener / invcm2au > freq[-1]:
+                norm = 1.0  # spline(freq[-1])*freq[-10]*invcm2au
+            else:
+                # norm = spline(fric_spec_dens_ener / invcm2au) * fric_spec_dens_ener
+                norm = spline(fric_spec_dens_ener / invcm2au)
+
+            fric_spec_dens = spline(self.omegak)
+            LT_fric_spec_dens = fric_spec_dens / norm
+            # LT_fric_spec_dens = LT_friction(self.omegak / invcm2au, spline) / norm
+
+        self.fric_LTwk = np.multiply(self.omegak, LT_fric_spec_dens)[:, np.newaxis]
+        info(units.unit_to_user("frequency", "inversecm", self.omegak), verbosity.debug)
+
+    def get_fric_rp_hessian(self, fric_hessian, eta, SD):
+        """Creates the friction hessian from the eta derivatives
+        THIS IS ONLY DONE FOR THE ACTIVE MODES"""
+
+        nphys = self.fix.nactive * 3
+        ndof = self.dbeads.nbeads * self.fix.nactive * 3
+        nbeads = self.dbeads.nbeads
+
+        s = eta
+
+        dgdq = np.zeros(s.shape)
+        for i in range(nbeads):
+            dgdq[i] = self.sqrtm(s[i] + np.eye(nphys) * 0.000000000001)
+
+        h_fric = np.zeros((ndof, ndof))
+
+        # Block diag:
+        if SD:
+            gq = self.obtain_g(s)
+            gq_k = np.dot(self.C, gq)
+            prefactor = np.dot(self.C.T, self.fric_LTwk * gq_k)
+            for n in range(self.dbeads.nbeads):
+                for j in range(nphys):
+                    for k in range(nphys):
+                        aux_jk = 0
+                        for i in range(nphys):
+                            if dgdq[n, i, j] != 0:
+                                aux_jk += (
+                                    0.5
+                                    * prefactor[n, i]
+                                    * fric_hessian[n, i, j, k]
+                                    / dgdq[n, i, j]
+                                )
+                        h_fric[nphys * n + j, nphys * n + k] = aux_jk
+        # Cross-terms:
+        for nl in range(nbeads):
+            for ne in range(nbeads):
+                prefactor = 0
+                for alpha in range(nbeads):
+                    prefactor += (
+                        self.C[alpha, nl] * self.C[alpha, ne] * self.fric_LTwk[alpha]
+                    )
+                for j in range(nphys):
+                    for k in range(nphys):
+                        suma = np.sum(dgdq[nl, :, j] * dgdq[ne, :, k])
+                        h_fric[nphys * nl + j, nphys * ne + k] = prefactor * suma
+        return h_fric
+
+    def obtain_g(self, s):
+        """Computes g from s"""
+
+        nphys = self.dbeads.natoms * 3
+
+        ss = np.zeros(s.shape)
+
+        for i in range(self.dbeads.nbeads):
+            ss[i] = self.sqrtm(
+                s[i] + np.eye(nphys) * 0.000000001
+            )  # ss = s ** 0.5 -> won't work for multiD
+
+        q = self.dbeads.q.copy()
+        gq = np.zeros(self.dbeads.q.copy().shape)
+        for nd in range(3 * self.dbeads.natoms):
+            try:
+                spline = self.interp1d(
+                    q[:, nd], ss[:, nd, nd], kind="cubic"
+                )  # spline for each dof
+                for nb in range(1, self.dbeads.nbeads):
+                    gq[nb, nd] = self.quad(spline, q[0, nd], q[nb, nd])[
+                        0
+                    ]  # Cumulative integral along the path for each dof
+                # for i in range(self.dbeads.nbeads):
+                #    print(q[i, nd],q[i,nd],ss[i, nd, nd],gq[i, nd])
+            except ValueError:
+                gq[:, nd] = 0
+
+        return gq
+
+    def compute_friction_terms(self):
+        """Computes friction component of the energy and gradient"""
+
+        s = self.eta
+
+        nphys = self.dbeads.natoms * 3
+
+        dgdq = np.zeros(s.shape)
+        for i in range(self.dbeads.nbeads):
+            with warnings.catch_warnings():
+                warnings.filterwarnings("error")
+                try:
+                    dgdq[i] = self.sqrtm(
+                        s[i] + np.eye(nphys) * 0.00000001
+                    )  # dgdq = s ** 0.5 -> won't work for multiD
+                except Warning:
+                    print(s[i])
+                    softexit.trigger("The provided friction is not positive definite")
+
+        gq = self.obtain_g(s)
+        gq_k = np.dot(self.C, gq)
+        e = 0.5 * np.sum(self.fric_LTwk * gq_k**2)
+
+        f = np.dot(self.C.T, self.fric_LTwk * gq_k)
+        g = np.zeros(f.shape)
+        for i in range(self.dbeads.nbeads):
+            g[i, :] = np.dot(dgdq[i], f[i])
+
+        return e, g
+
+    def get_full_extras(self, reduced_forces, full_mspath, indexes):
+        """Get the full extra strings"""
+        diction = {}
+        for key in reduced_forces.extras.keys():
+            if str(key) != "raw":
+                red_data = np.array(reduced_forces.extras[key])
+                if self.spline:
+                    red_mspath = full_mspath[indexes]
+                    spline = self.interp1d(red_mspath, red_data.T, kind="cubic")
+                    full_data = spline(full_mspath).T
+                else:
+                    full_data = red_data
+            else:
+                full_data = reduced_forces.extras[key]
+            diction[key] = full_data
+
+        return diction
+
+    def __call__(self, x, new_disc=True):
+        """Computes energy and gradient for optimization step"""
+        self.fcount += 1
+        full_q = x.copy()
+        full_mspath = ms_pathway(full_q, self.dbeads.m3)
+        full_pot, full_forces, indexes, reduced_forces = self.interpolation(
+            full_q, full_mspath, get_all_info=True
+        )
+
+        full_extras = self.get_full_extras(reduced_forces, full_mspath, indexes)
+        if self.frictionSD:
+            full_eta = np.zeros(
+                (self.dbeads.nbeads, self.dbeads.natoms * 3, self.dbeads.natoms * 3)
+            )
+            for n in range(self.dbeads.nbeads):
+                full_eta[n] = full_extras["friction"][n].reshape(
+                    self.dbeads.natoms * 3, self.dbeads.natoms * 3
+                )
+        else:
+            full_eta = self.eta
+
+        info(
+            "We expect friction tensor evaluated at the first RP frequency",
+            verbosity.debug,
+        )
+
+        # This forces the update of the forces and the extras
+        self.dbeads.q[:] = x[:]
+        self.dforces.transfer_forces_manual(
+            [full_q], [full_pot], [full_forces], [full_extras]
+        )
+        self.save(full_pot, -full_forces, full_eta)
+        return self.evaluate()
+
+    def evaluate(self):
+        """Evaluate the energy and forces including:
+        - non uniform discretization
+        - friction term
+        """
+
+        e = self.pot.copy()
+        g = -self.f.copy()
+
+        e_friction, g_friction = self.compute_friction_terms()
+        e += e_friction
+        g += g_friction
+
+        e = e * (self.coef[1:] + self.coef[:-1]) / 2
+        g = g * (self.coef[1:] + self.coef[:-1]) / 2
 
         return e, g
 
 
 class SpringMapper(object):
-    """Creation of the multi-dimensional function to compute full or half ring polymer pot
+    """Creation of the multi-dimensional function to compute full or half ring polymer potential
     and forces.
     """
 
     def __init__(self):
         self.pot = None
         self.f = None
-        self.dbeads = None
-        self.fix = None
+        pass
 
-    def bind(self, dumop, discretization):
-        self.temp = dumop.temp
-        self.fix = Fix(dumop.beads.natoms, dumop.fixatoms, dumop.beads.nbeads)
-        self.dbeads = Beads(
-            dumop.beads.natoms - len(dumop.fixatoms), dumop.beads.nbeads
-        )
-        self.dbeads.q[:] = self.fix.get_active_vector(dumop.beads.copy().q, 1)
-        self.dbeads.m[:] = self.fix.get_active_vector(dumop.beads.copy().m, 0)
-        self.dbeads.names[:] = self.fix.get_active_vector(dumop.beads.copy().names, 0)
-        self.set_coef(discretization)
-
-        if dumop.options["mode"] == "rate":
-            self.omega2 = (
-                self.temp
-                * (2 * self.dbeads.nbeads)
-                * units.Constants.kb
-                / units.Constants.hbar
-            ) ** 2
-        elif dumop.options["mode"] == "splitting":
-            self.omega2 = (
-                self.temp
-                * self.dbeads.nbeads
-                * units.Constants.kb
-                / units.Constants.hbar
-            ) ** 2
+    def bind(self, mapper):
+        self.temp = mapper.temp
+        self.fix = mapper.fix
+        self.coef = mapper.coef
+        self.dbeads = mapper.beads.copy()
+        # self.nm = mapper.nm
+        # self.rp_factor = mapper.rp_factor
+        if self.dbeads.nbeads > 1:
+            self.C = mapper.nm.transform._b2o_nm
+        else:
+            self.C = 1
+        self.omegak = mapper.rp_factor * mapper.nm.get_o_omegak()
+        self.omegan = mapper.rp_factor * mapper.nm.omegan
 
+        # Computes the spring hessian if the optimization modes requires it
         if (
-            dumop.options["opt"] == "nichols"
-            or dumop.options["opt"] == "NR"
-            or dumop.options["opt"] == "lanczos"
+            mapper.options["opt"] == "nichols"
+            or mapper.options["opt"] == "NR"
+            or mapper.options["opt"] == "lanczos"
         ):
             self.h = self.spring_hessian(
-                natoms=self.dbeads.natoms,
-                nbeads=self.dbeads.nbeads,
-                m3=self.dbeads.m3[0],
-                omega2=self.omega2,
+                natoms=self.fix.fixbeads.natoms,
+                nbeads=self.fix.fixbeads.nbeads,
+                m3=self.fix.fixbeads.m3[0],
+                omega2=(self.omegan) ** 2,
                 coef=self.coef,
             )
 
     def set_coef(self, coef):
         """Sets coefficients for non-uniform instanton calculation"""
         self.coef = coef.reshape(-1, 1)
 
     def save(self, e, g):
         """Stores potential and forces in this class for convenience"""
         self.pot = e
         self.f = -g
 
+    def __call__(self, x, ret=True, new_disc=True):
+        """Computes spring energy and gradient for instanton optimization step"""
+
+        if new_disc:
+            coef = self.coef
+        elif new_disc == "one":
+            coef = np.ones(self.coef.shape)
+        else:
+            coef = new_disc.reshape(self.coef.shape)
+
+        if x.shape[0] == 1:  # only one bead
+            self.dbeads.q = x
+            e = 0.0
+            g = np.zeros(x.shape[1])
+            self.save(e, g)
+
+        else:
+            self.dbeads.q = x
+            e = 0.00
+            g = np.zeros(self.dbeads.q.shape, float)
+
+            # OLD reference
+            # for i in range(self.dbeads.nbeads - 1):
+            #    dq = self.dbeads.q[i + 1, :] - self.dbeads.q[i, :]
+            #    e += self.omega2 * 0.5 * np.dot(self.dbeads.m3[0] * dq, dq)
+            # for i in range(0, self.dbeads.nbeads - 1):
+            #    #g[i, :] += self.omega2 * (self.dbeads.q[i, :] - self.dbeads.q[i + 1, :])
+            #    g[i, :] += self.dbeads.m3[i, :] * self.omega2 * (self.dbeads.q[i, :] - self.dbeads.q[i + 1, :])
+            # for i in range(1, self.dbeads.nbeads):
+            #    #g[i, :] +=  self.omega2 * (self.dbeads.q[i, :] - self.dbeads.q[i - 1, :])
+            #    g[i, :] += self.dbeads.m3[i, :] * self.omega2 * (self.dbeads.q[i, :] - self.dbeads.q[i - 1, :])
+            gq_k = np.dot(self.C, self.dbeads.q)
+            g = self.dbeads.m3[0] * np.dot(
+                self.C.T, gq_k * (self.omegak**2)[:, np.newaxis]
+            )
+
+            # With new discretization #This can be expressed as matrix multp
+            if False:  # ALBERTO
+                for i in range(self.dbeads.nbeads - 1):
+                    dq = (self.dbeads.q[i + 1, :] - self.dbeads.q[i, :]) / np.sqrt(
+                        coef[i + 1]
+                    )  # coef[0] and coef[-1] do not enter
+                    e += self.omega2 * 0.5 * np.dot(self.dbeads.m3[0] * dq, dq)
+                for i in range(0, self.dbeads.nbeads - 1):
+                    g[i, :] += (
+                        self.dbeads.m3[i, :]
+                        * self.omega2
+                        * (
+                            self.dbeads.q[i, :] / coef[i + 1]
+                            - self.dbeads.q[i + 1, :] / coef[i + 1]
+                        )
+                    )
+                for i in range(1, self.dbeads.nbeads):
+                    g[i, :] += (
+                        self.dbeads.m3[i, :]
+                        * self.omega2
+                        * (
+                            self.dbeads.q[i, :] / coef[i]
+                            - self.dbeads.q[i - 1, :] / coef[i]
+                        )
+                    )
+
+            self.save(e, g)
+
+        if ret:
+            return e, g
+
     @staticmethod
     def spring_hessian(natoms, nbeads, m3, omega2, mode="half", coef=None):
         """Compute the 'spring hessian'
 
         OUT    h       = hessian with only the spring terms ('spring hessian')
         """
         if coef is None:
@@ -573,129 +848,135 @@
         # Corner
         if mode == "full":
             h[0:ii, (nbeads - 1) * ii : (nbeads) * ii] += ndiag / coef[0]
             h[(nbeads - 1) * ii : (nbeads) * ii, 0:ii] += ndiag / coef[0]
 
         return h
 
-    def __call__(self, x, ret=True, new_disc=True):
-        """Computes spring energy and gradient for instanton optimization step"""
+    # def __call__(self, x, ret=True, new_disc=True):
+    #    """Computes spring energy and gradient for instanton optimization step"""
 
-        x = self.fix.get_active_vector(x, 1).copy()
 
-        if new_disc:
-            coef = self.coef
-        elif new_disc == "one":
-            coef = np.ones(self.coef.shape)
-        else:
-            coef = new_disc.reshape(self.coef.shape)
+class Mapper(object):
+    """Creation of the multi-dimensional function that is the proxy between all the energy and force components and the optimization algorithm.
+    It also handles fixatoms"""
 
-        if x.shape[0] == 1:  # only one bead
-            self.dbeads.q = x
-            e = 0.0
-            g = np.zeros(x.shape[1])
-            self.save(e, g)
+    def __init__(self, esum=False):
+        self.sm = SpringMapper()
+        self.gm = PesMapper()
+        self.esum = esum
 
-        else:
-            self.dbeads.q = x
-            e = 0.00
-            g = np.zeros(self.dbeads.q.shape, float)
+    def initialize(self, q, forces):
+        self.gm.initialize(q, forces)
 
-            # OLD reference
-            # for i in range(self.dbeads.nbeads - 1):
-            #    dq = self.dbeads.q[i + 1, :] - self.dbeads.q[i, :]
-            #    e += self.omega2 * 0.5 * np.dot(self.dbeads.m3[0] * dq, dq)
-            # for i in range(0, self.dbeads.nbeads - 1):
-            #    g[i, :] += self.dbeads.m3[i, :] * self.omega2 * (self.dbeads.q[i, :] - self.dbeads.q[i + 1, :])
-            # for i in range(1, self.dbeads.nbeads):
-            #    g[i, :] += self.dbeads.m3[i, :] * self.omega2 * (self.dbeads.q[i, :] - self.dbeads.q[i - 1, :])
+        e1, g1 = self.gm.evaluate()
+        e2, g2 = self.sm(q)
+        g = self.fix.get_active_vector(g1 + g2, 1)
+        e = np.sum(e1 + e2)
 
-            # With new discretization
-            for i in range(self.dbeads.nbeads - 1):
-                dq = (self.dbeads.q[i + 1, :] - self.dbeads.q[i, :]) / np.sqrt(
-                    coef[i + 1]
-                )  # coef[0] and coef[-1] do not enter
-                e += self.omega2 * 0.5 * np.dot(self.dbeads.m3[0] * dq, dq)
-            for i in range(0, self.dbeads.nbeads - 1):
-                g[i, :] += (
-                    self.dbeads.m3[i, :]
-                    * self.omega2
-                    * (
-                        self.dbeads.q[i, :] / coef[i + 1]
-                        - self.dbeads.q[i + 1, :] / coef[i + 1]
-                    )
-                )
-            for i in range(1, self.dbeads.nbeads):
-                g[i, :] += (
-                    self.dbeads.m3[i, :]
-                    * self.omega2
-                    * (
-                        self.dbeads.q[i, :] / coef[i]
-                        - self.dbeads.q[i - 1, :] / coef[i]
-                    )
-                )
+        self.save(e, g)
 
-            self.save(e, g)
+    def save(self, e, g):
+        self.pot = e
+        self.f = -g
 
-        if ret:
-            return e, g
+    def bind(self, dumop):
+        self.temp = dumop.temp
+        self.beads = dumop.beads
+        self.forces = dumop.forces
+        self.cell = dumop.cell
+        self.nm = dumop.nm
+        self.rp_factor = dumop.rp_factor
+
+        self.fixatoms = dumop.fixatoms
+        self.fix = dumop.fix
+        self.fixbeads = self.fix.fixbeads
+
+        self.options = dumop.options
+
+        self.coef = np.ones(self.beads.nbeads + 1).reshape(-1, 1)
+        self.set_coef(self.options["discretization"])
+
+        self.friction = self.options["friction"]
+        if self.friction:
+            self.frictionSD = self.options["frictionSD"]
+            self.gm = FrictionMapper(self.frictionSD, self.options["eta0"])
+            self.gm.bind(self)
+            self.gm.set_fric_spec_dens(
+                dumop.options["fric_spec_dens"], dumop.options["fric_spec_dens_ener"]
+            )
+        else:
+            self.gm.bind(self)
+
+        self.sm.bind(self)
 
+    def set_coef(self, coef):
+        """Sets coeficients for non-uniform instanton calculation"""
+        self.coef[:] = coef.reshape(-1, 1)
 
-class FullMapper(object):
-    """Creation of the multi-dimensional function to compute the physical and the spring forces."""
+    def __call__(self, x, mode="all", apply_fix=True, new_disc=True, ret=True):
+        if mode == "all":
+            e1, g1 = self.sm(x, new_disc)
+            e2, g2 = self.gm(x, new_disc)
+            e = e1 + e2
+            g = np.add(g1, g2)
+
+        elif mode == "physical":
+            e, g = self.gm(x, new_disc)
+        elif mode == "springs":
+            e, g = self.sm(x, new_disc)
+        else:
+            softexit.trigger("Mode not recognized when calling  FullMapper")
 
-    def __init__(self, im, gm, esum=False):
-        self.im = im
-        self.gm = gm
-        self.esum = esum
+        if apply_fix:
+            g = self.fix.get_active_vector(g, 1)
 
-    def __call__(self, x):
-        e1, g1 = self.im(x)
-        e2, g2 = self.gm(x)
-        e = e1 + e2
-        g = np.add(g1, g2)
+        if mode == "all":
+            self.save(np.sum(e), g)
 
         if self.esum:
             e = np.sum(e)
 
-        return e, g
+        if ret:
+            return e, g
 
 
-class DummyOptimizer(dobject):
+class DummyOptimizer:
     """Dummy class for all optimization classes"""
 
     def __init__(self):
-        """Initialises object for GradientMapper (physical potential, forces and Hessian)
-        and SpringMapper (spring potential, forces and Hessian)"""
+        """Initializes object for PesMapper (physical potential, forces and hessian)
+        and SpringMapper ( spring potential,forces and hessian)"""
 
         self.options = {}  # Optimization options
         self.optarrays = {}  # Optimization arrays
 
-        self.gm = GradientMapper()
-        self.im = SpringMapper()
-        self.fm = FullMapper(self.im, self.gm)
-        self.fix = None
+        self.mapper = Mapper()
 
         self.exit = False
         self.init = False
 
     def bind(self, geop):
         """
-        Bind optimization options and call bind function of Mappers (get beads, cell, forces)
-        check whether force size, Hessian size from  match system size
+        Bind optimization options and call bind function of Mappers (get beads, cell,forces)
+        check whether force size,  Hessian size from  match system size
         """
 
         self.beads = geop.beads
         self.cell = geop.cell
         self.forces = geop.forces
         self.fixcom = geop.fixcom
         self.fixatoms = geop.fixatoms
+
+        self.fix = Fix(self.fixatoms, self.beads, self.beads.nbeads)
         self.nm = geop.nm
-        # self.ensemble = geop.ens
+        self.rp_factor = geop.rp_factor
+
         self.output_maker = geop.output_maker
+
         # The resize action must be done before the bind
 
         if geop.optarrays["old_x"].size != self.beads.q.size:
             if geop.optarrays["old_x"].size == 0:
                 geop.optarrays["old_x"] = np.zeros(
                     (self.beads.nbeads, 3 * self.beads.natoms), float
                 )
@@ -732,52 +1013,55 @@
                 geop.options["discretization"] = np.ones(self.beads.nbeads + 1, float)
             else:
                 raise ValueError("Discretization coefficients do not match system size")
 
         self.options["max_ms"] = geop.options["max_ms"]
         self.options["max_e"] = geop.options["max_e"]
         self.options["discretization"] = geop.options["discretization"]
+        self.options["friction"] = geop.options["friction"]
+        self.options["frictionSD"] = geop.options["frictionSD"]
+        if self.options["friction"]:
+            self.options["eta0"] = geop.options["eta0"]
+            self.options["fric_spec_dens"] = geop.options["fric_spec_dens"]
+            self.options["fric_spec_dens_ener"] = geop.options["fric_spec_dens_ener"]
         self.options["tolerances"] = geop.options["tolerances"]
         self.optarrays["big_step"] = geop.optarrays["big_step"]
         self.optarrays["old_x"] = geop.optarrays["old_x"]
         self.optarrays["old_u"] = geop.optarrays["old_u"]
         self.optarrays["old_f"] = geop.optarrays["old_f"]
         self.options["opt"] = geop.options["opt"]  # optimization algorithm
 
         # Generic instanton
         self.options["save"] = geop.options["save"]
         self.options["prefix"] = geop.options["prefix"]
         self.optarrays["delta"] = geop.optarrays["delta"]
         self.options["hessian_final"] = geop.options["hessian_final"]
         self.optarrays["energy_shift"] = geop.optarrays["energy_shift"]
 
-        self.gm.bind(
-            self,
-            self.options["discretization"],
-            self.options["max_ms"],
-            self.options["max_e"],
-        )
-        self.im.bind(self, self.options["discretization"])
-        self.fix = Fix(geop.beads.natoms, geop.fixatoms, geop.beads.nbeads)
+        # self.fix = Fix(geop.beads.natoms, geop.fixatoms, geop.beads.nbeads)
+
+        self.mapper.bind(self)
 
     def initial_geo(self):
-        # TODO : add linear interpolation
+        """Generates the initial instanton geometry by stretching the transitions-state geometry along the mode with imaginary frequency"""
 
         info(
             " @GEOP: We stretch the initial geometry with an 'amplitude' of {:4.2f}".format(
                 self.optarrays["delta"]
             ),
             verbosity.low,
         )
 
-        fix_onebead = Fix(self.beads.natoms, self.fixatoms, 1)
+        fix_onebead = Fix(self.fixatoms, self.beads, 1)
         active_hessian = fix_onebead.get_active_vector(
             self.optarrays["initial_hessian"], 2
         )
-        active_imvector = get_imvector(active_hessian, self.im.dbeads.m3[0].flatten())
+        active_imvector = get_imvector(
+            active_hessian, fix_onebead.fixbeads.m3[0].flatten()
+        )
         imvector = fix_onebead.get_full_vector(active_imvector, 1).flatten()
 
         for i in range(self.beads.nbeads):
             self.beads.q[i, :] += (
                 self.optarrays["delta"]
                 * np.cos(i * np.pi / float(self.beads.nbeads - 1))
                 * imvector[:]
@@ -785,26 +1069,21 @@
 
     def exitstep(self, d_x_max, step):
         """Exits the simulation step. Computes time, checks for convergence."""
         self.qtime += time.time()
 
         tolerances = self.options["tolerances"]
         d_u = self.forces.pot - self.optarrays["old_u"].sum()
-        active_force = self.fix.get_active_vector(self.forces.f, 1) + self.im.f
+        # active_force = self.fix.get_active_vector(self.forces.f, 1) + self.im.f
 
-        fff = (
-            self.fix.get_active_vector(self.forces.f, 1)
-            * (self.im.coef[1:] + self.im.coef[:-1])
-            / 2
-        )
-        active_force = fff + self.im.f
+        active_force = self.mapper.f
 
         info(
             " @Exit step: Energy difference: {:4.2e}, (condition: {:4.2e})".format(
-                np.absolute(d_u / self.im.dbeads.natoms), tolerances["energy"]
+                np.absolute(d_u / self.fix.fixbeads.natoms), tolerances["energy"]
             ),
             verbosity.low,
         )
         info(
             " @Exit step: Maximum force component: {:4.2e}, (condition: {:4.2e})".format(
                 np.amax(np.absolute(active_force)), tolerances["force"]
             ),
@@ -814,15 +1093,15 @@
             " @Exit step: Maximum component step component: {:4.2e}, (condition: {:4.2e})".format(
                 d_x_max, tolerances["position"]
             ),
             verbosity.low,
         )
 
         if (
-            (np.absolute(d_u / self.im.dbeads.natoms) <= tolerances["energy"])
+            (np.absolute(d_u / self.mapper.sm.dbeads.natoms) <= tolerances["energy"])
             and (
                 (np.amax(np.absolute(active_force)) <= tolerances["force"])
                 or (
                     np.linalg.norm(
                         self.forces.f.flatten() - self.optarrays["old_f"].flatten()
                     )
                     <= 1e-08
@@ -839,33 +1118,53 @@
                 self.beads.q,
                 self.forces.f,
                 self.forces.pots,
                 self.cell,
                 self.optarrays["energy_shift"],
                 self.output_maker,
             )
-            if self.options["hessian_final"] != "true":
+            if not self.options["hessian_final"]:
                 info("We are not going to compute the final hessian.", verbosity.low)
                 info(
                     "Warning, The current hessian is not the real hessian is only an approximation .",
                     verbosity.low,
                 )
 
             else:
                 info("We are going to compute the final hessian", verbosity.low)
-                active_hessian = get_hessian(
-                    self.gm,
-                    self.beads.q.copy(),
-                    self.beads.natoms,
-                    self.beads.nbeads,
-                    self.fixatoms,
-                )
-                self.optarrays["hessian"][:] = self.fix.get_full_vector(
-                    active_hessian, 2
+                current_hessian = get_hessian(
+                    gm=self.mapper.gm,
+                    x0=self.beads.q.copy(),
+                    natoms=self.beads.natoms,
+                    nbeads=self.beads.nbeads,
+                    fixatoms=self.fixatoms,
+                    friction=self.options["frictionSD"],
                 )
+
+                if self.options["friction"] and self.options["frictionSD"]:
+                    friction_hessian = current_hessian[1]
+                    self.optarrays["fric_hessian"][:] = self.fix.get_full_vector(
+                        friction_hessian, 4
+                    )
+                    # self.optarrays["fric_hessian"][:] = friction_hessian #ALBERTO
+                    print_instanton_hess(
+                        self.options["prefix"] + "fric_FINAL",
+                        step,
+                        self.optarrays["fric_hessian"],
+                        self.output_maker,
+                    )
+
+                    phys_hessian = current_hessian[0]
+
+                else:
+                    phys_hessian = current_hessian
+
+                # self.optarrays["hessian"][:] = self.fix.get_full_vector(phys_hessian, 2) #ALBERTO
+                self.optarrays["hessian"][:] = phys_hessian  # ALBERTO
+
                 print_instanton_hess(
                     self.options["prefix"] + "_FINAL",
                     step,
                     self.optarrays["hessian"],
                     self.output_maker,
                 )
 
@@ -873,27 +1172,29 @@
             # If we just exit here, the last step (including the last hessian) will not be in the RESTART file
 
         return False
 
     def update_pos_for(self):
         """Update positions and forces"""
 
-        self.beads.q[:] = self.gm.dbeads.q[:]
+        self.beads.q[:] = self.mapper.gm.dbeads.q[:]
 
         # This forces the update of the forces
-        self.forces.transfer_forces(self.gm.dforces)
+        self.forces.transfer_forces(self.mapper.gm.dforces)
 
     def update_old_pos_for(self):
-        # Update "old" positions and forces
+        """Update 'old' positions and forces arrays"""
+
         self.optarrays["old_x"][:] = self.beads.q
         self.optarrays["old_u"][:] = self.forces.pots
         self.optarrays["old_f"][:] = self.forces.f
 
     def print_geo(self, step):
-        # Print current instanton geometry
+        """Small interface to call the function that prints thet instanton geometry"""
+
         if (
             self.options["save"] > 0 and np.mod(step, self.options["save"]) == 0
         ) or self.exit:
             print_instanton_geo(
                 self.options["prefix"],
                 step,
                 self.beads.nbeads,
@@ -921,16 +1222,15 @@
 
         if adaptative:
             softexit.trigger(
                 status="bad",
                 message="Adaptative discretization is not fully implemented",
             )
             # new_coef = <implement_here>
-            # self.im.set_coef(coef)
-            # self.gm.set_coef(coef)
+            # self.mapper.set_coef(coef)
             raise NotImplementedError
 
         self.qtime = -time.time()
         info("\n Instanton optimization STEP {}".format(step), verbosity.low)
 
         activearrays = self.fix.get_active_array(self.optarrays)
 
@@ -943,22 +1243,22 @@
     def opt_coef(self, coef):
         # func = lambda x: 2 * np.sum(x) - x[0] - x[-1]
         def func(x):
             return 2 * np.sum(x) - x[0] - x[-1]
 
         coef = np.absolute(coef)
         s = func(coef)
-        coef *= 2 * self.im.dbeads.nbeads / s
-        # c0   = 2*self.im.dbeads.nbeads - 2*np.sum(coef)
+        coef *= 2 * self.sm.dbeads.nbeads / s
+        # c0   = 2*self.sm.dbeads.nbeads - 2*np.sum(coef)
         # coef = np.insert(coef,0,c0)
 
-        self.im.set_coef(coef)
+        # self.im.set_coef(coef)
 
         fphys = self.gm.dforces.f * ((coef[1:] + coef[:-1]) / 2).reshape(-1, 1)
-        e, gspring = self.im(self.im.dbeads.q)
+        e, gspring = self.sm(self.sm.dbeads.q)
         return np.amax(np.absolute(-gspring + fphys))
 
 
 class HessianOptimizer(DummyOptimizer):
     """Instanton Rate calculation"""
 
     def bind(self, geop):
@@ -970,28 +1270,26 @@
 
         if len(self.fixatoms) > 0:
             info(" 'fixatoms' is enabled. Setting asr to None", verbosity.low)
             self.options["hessian_asr"] = "none"
         #        self.output_maker = geop.output_maker
         self.options["hessian_init"] = geop.options["hessian_init"]
         self.optarrays["initial_hessian"] = None
+        print(geop.optarrays["hessian"].size)
 
         if geop.optarrays["hessian"].size != (
             self.beads.natoms * 3 * self.beads.q.size
         ):
             if geop.optarrays["hessian"].size == (self.beads.natoms * 3) ** 2:
                 self.optarrays["initial_hessian"] = geop.optarrays["hessian"].copy()
                 geop.optarrays["hessian"] = np.zeros(
                     (self.beads.natoms * 3, self.beads.q.size), float
                 )
 
-            elif (
-                geop.optarrays["hessian"].size == 0
-                and geop.options["hessian_init"] == "true"
-            ):
+            elif geop.optarrays["hessian"].size == 0 and geop.options["hessian_init"]:
                 info(
                     " Initial hessian is not provided. We are going to compute it.",
                     verbosity.low,
                 )
                 geop.optarrays["hessian"] = np.zeros(
                     (self.beads.natoms * 3, self.beads.q.size)
                 )
@@ -1006,111 +1304,175 @@
 
             else:
                 raise ValueError(
                     " 'Hessian_init' is false, an initial hessian (of the proper size) must be provided."
                 )
 
         self.optarrays["hessian"] = geop.optarrays["hessian"]
+        if self.options["friction"]:
+            if geop.options["eta0"].shape == (0, 0):
+                geop.options["eta0"] = np.zeros(
+                    (self.beads.natoms * 3, self.beads.natoms * 3)
+                )
+            assert geop.options["eta0"].shape == (
+                self.beads.natoms * 3,
+                self.beads.natoms * 3,
+            ), "Please provide a friction tensor with the appropiate shape"
+            self.options["eta0"] = geop.options["eta0"]
+
+            if self.options["frictionSD"]:
+                if geop.optarrays["fric_hessian"].shape != (
+                    self.beads.nbeads,
+                    self.beads.natoms * 3,
+                    self.beads.natoms * 3,
+                    self.beads.natoms * 3,
+                ):
+                    if geop.options["hessian_init"]:
+                        geop.optarrays["fric_hessian"] = np.zeros(
+                            (
+                                self.beads.nbeads,
+                                self.beads.natoms * 3,
+                                self.beads.natoms * 3,
+                                self.beads.natoms * 3,
+                            )
+                        )
+                    else:
+                        raise ValueError(
+                            """
+              'Hessian_init' is false, 'friction' is true so an initial fric_hessian (of the proper size) must be provided.
+                    """
+                        )
+                self.optarrays["fric_hessian"] = geop.optarrays["fric_hessian"]
 
     def initialize(self, step):
         if step == 0:
             info(" @GEOP: Initializing INSTANTON", verbosity.low)
 
             if self.beads.nbeads == 1:
                 info(" @GEOP: Classical TS search", verbosity.low)
 
             else:
                 # If the coordinates in all the imaginary time slices are the same
                 if ((self.beads.q - self.beads.q[0]) == 0).all():
                     self.initial_geo()
-                    self.options["hessian_init"] = "true"
+                    self.options["hessian_init"] = True
 
                 else:
                     info(
                         " @GEOP: Starting from the provided geometry in the extended phase space",
                         verbosity.low,
                     )
-                    if not (
-                        (self.optarrays["initial_hessian"] is None)
-                        or (
-                            self.optarrays["initial_hessian"].size
-                            == (self.beads.natoms * 3) ** 2
-                        )
-                    ):
+                    if not (self.optarrays["initial_hessian"] is None):
                         raise ValueError(
-                            " You have to provide a hessian with size (3 x natoms)^2 but also geometry in"
+                            " You have to provided a hessian with size (3 x natoms)^2 but also geometry in"
                             " the extended phase space (nbeads>1). Please check the inputs\n"
                         )
 
-        self.gm.save(self.forces.pots, self.forces.f)
+        # Initialize all the mappers
+        self.mapper.initialize(self.beads.q, self.forces)
 
-        if self.options["hessian_init"] == "true":
-            active_hessian = get_hessian(
-                self.gm,
-                self.beads.q.copy(),
-                self.beads.natoms,
-                self.beads.nbeads,
-                self.fixatoms,
-            )
-            self.optarrays["hessian"][:] = self.fix.get_full_vector(active_hessian, 2)
+        if self.options["hessian_init"]:
+            full_hessian = get_hessian(
+                gm=self.mapper.gm,
+                x0=self.beads.q.copy(),
+                natoms=self.beads.natoms,
+                nbeads=self.beads.nbeads,
+                fixatoms=self.fixatoms,
+                friction=self.options["frictionSD"],
+            )
+            if self.options["friction"] and self.options["frictionSD"]:
+                phys_hessian = full_hessian[0]
+                friction_hessian = full_hessian[1]
+                # self.optarrays["fric_hessian"][:] = self.fix.get_full_vector( friction_hessian, 4 ) #ALBERTO
+                self.optarrays["fric_hessian"][:] = friction_hessian[:]
+            else:
+                phys_hessian = full_hessian
 
-        if self.im.f is None:
-            self.im(self.beads.q, ret=False)  # Init instanton mapper
+            # self.optarrays["hessian"][:] = self.fix.get_full_vector(phys_hessian, 2) #ALBERTO
+            self.optarrays["hessian"][:] = phys_hessian
 
-        self.gm.save(self.forces.pots, self.forces.f)
+        #   self.gm.save(self.forces.pots, self.forces.f)
         self.update_old_pos_for()
 
         self.init = True
 
     def update_hessian(self, update, active_hessian, new_x, d_x, d_g):
         """Update hessian"""
 
         if update == "powell":
-            i = self.im.dbeads.natoms * 3
-            for j in range(self.im.dbeads.nbeads):
+            i = self.fix.fixbeads.natoms * 3
+            for j in range(self.fix.fixbeads.nbeads):
                 aux = active_hessian[:, j * i : (j + 1) * i]
                 dg = d_g[j, :]
                 dx = d_x[j, :]
                 Powell(dx, dg, aux)
+            phys_hessian = active_hessian
+            if self.options["friction"]:
+                info(
+                    "Powell update for friction hessian is not implemented. We move on without updating it. In all tested cases this is not a problem",
+                    verbosity.medium,
+                )
 
         elif update == "recompute":
             active_hessian = get_hessian(
-                self.gm, new_x, self.beads.natoms, self.beads.nbeads, self.fixatoms
+                gm=self.mapper.gm,
+                x0=new_x,
+                natoms=self.beads.natoms,
+                nbeads=self.beads.nbeads,
+                fixatoms=self.fixatoms,
+                friction=self.options["frictionSD"],
             )
 
-        self.optarrays["hessian"][:] = self.fix.get_full_vector(active_hessian, 2)
+            if self.options["friction"] and self.options["frictionSD"]:
+                phys_hessian = active_hessian[0]
+                friction_hessian = active_hessian[1]
+                self.optarrays["fric_hessian"][:] = self.fix.get_full_vector(
+                    friction_hessian, 4
+                )
+            else:
+                phys_hessian = active_hessian
+
+        self.optarrays["hessian"][:] = self.fix.get_full_vector(phys_hessian, 2)
 
     def print_hess(self, step):
         if (
             self.options["save"] > 0 and np.mod(step, self.options["save"]) == 0
         ) or self.exit:
             print_instanton_hess(
                 self.options["prefix"],
                 step,
                 self.optarrays["hessian"],
                 self.output_maker,
             )
+            if self.options["friction"]:
+                print_instanton_hess(
+                    self.options["prefix"] + "_fric",
+                    step,
+                    self.optarrays["fric_hessian"],
+                    self.output_maker,
+                )
 
     def post_step(self, step, new_x, d_x, activearrays):
-        """General tasks that have to be performed after the  actual step"""
+        """General tasks that have to be performed after finding the new step"""
 
         d_x_max = np.amax(np.absolute(d_x))
         info("Current step norm = {}".format(d_x_max), verbosity.medium)
 
-        # Get new energy (u)  and forces(f) using mapper
-        self.im(new_x, ret=False, new_disc=True)  # Only to update the mapper
+        # Get energy and forces(f) for the new position
+        self.mapper(new_x, ret=False)
 
-        u, g2 = self.gm(new_x, new_disc=False)
-        f = -g2
+        # Update
+        f = self.fix.get_active_vector(self.mapper.gm.f, t=1)
         d_g = np.subtract(activearrays["old_f"], f)
 
         # Update
         self.update_hessian(
             self.options["hessian_update"], activearrays["hessian"], new_x, d_x, d_g
         )
+
         self.update_pos_for()
 
         #  Print
         self.print_geo(step)
         self.print_hess(step)
 
         # Check Exit and only then update old arrays
@@ -1126,37 +1488,50 @@
         super(NicholsOptimizer, self).bind(geop)
 
     def initialize(self, step):
         # call initialize function from HessianOptimizer
         super(NicholsOptimizer, self).initialize(step)
 
     def step(self, step=None):
-        """Does one simulation time step."""
+        """Does one simulation step."""
 
         activearrays = self.pre_step(step)
 
         # First construct complete hessian from reduced
         h0 = red2comp(
             activearrays["hessian"],
-            self.im.dbeads.nbeads,
-            self.im.dbeads.natoms,
-            self.im.coef,
+            self.fix.fixbeads.nbeads,
+            self.fix.fixbeads.natoms,
+            self.mapper.coef,
         )
 
         # Add spring terms to the physical hessian
-        h1 = np.add(self.im.h, h0)
+        h = np.add(self.mapper.sm.h, h0)
+
+        # Add friction terms to the hessian
+        if self.options["friction"]:
+            eta_active = self.fix.get_active_vector(self.mapper.gm.eta, 5)
+            if self.options["frictionSD"]:
+                h_fric = self.mapper.gm.get_fric_rp_hessian(
+                    activearrays["fric_hessian"], eta_active, self.options["frictionSD"]
+                )
+            else:
+                h_fric = self.mapper.gm.get_fric_rp_hessian(
+                    None, eta_active, self.options["frictionSD"]
+                )
+            h = np.add(h, h_fric)
 
         # Get eigenvalues and eigenvector.
         d, w = clean_hessian(
-            h1,
-            self.im.dbeads.q,
-            self.im.dbeads.natoms,
-            self.im.dbeads.nbeads,
-            self.im.dbeads.m,
-            self.im.dbeads.m3,
+            h,
+            self.fix.fixbeads.q,
+            self.fix.fixbeads.natoms,
+            self.fix.fixbeads.nbeads,
+            self.fix.fixbeads.m,
+            self.fix.fixbeads.m3,
             self.options["hessian_asr"],
         )
 
         # d,w =np.linalg.eigh(h1) #Cartesian
         info(
             "\n@Nichols: 1st freq {} cm^-1".format(
                 units.unit_to_user(
@@ -1182,25 +1557,27 @@
             verbosity.medium,
         )
         # info('@Nichols: 4th freq {} cm^-1'.format(units.unit_to_user('frequency','inversecm',np.sign(d[3])*np.sqrt(np.absolute(d[3])))),verbosity.medium)
         # info('@Nichols: 8th freq {} cm^-1\n'.format(units.unit_to_user('frequency','inversecm',np.sign(d[7])*np.sqrt(np.absolute(d[7])))),verbosity.medium)
 
         # Find new movement direction
         if self.options["mode"] == "rate":
-            f = activearrays["old_f"] * (self.im.coef[1:] + self.im.coef[:-1]) / 2
             d_x = nichols(
-                f, self.im.f, d, w, self.im.dbeads.m3, activearrays["big_step"]
+                self.mapper.f,
+                d,
+                w,
+                self.fix.fixbeads.m3,
+                activearrays["big_step"],
             )
         elif self.options["mode"] == "splitting":
             d_x = nichols(
-                activearrays["old_f"],
-                self.im.f,
+                self.mapper.f,
                 d,
                 w,
-                self.im.dbeads.m3,
+                self.fix.fixbeads.m3,
                 activearrays["big_step"],
                 mode=0,
             )
 
         # Rescale step if necessary
         if np.amax(np.absolute(d_x)) > activearrays["big_step"]:
             info(
@@ -1228,28 +1605,28 @@
         super(NROptimizer, self).initialize(step)
 
     def step(self, step=None):
         """Does one simulation time step."""
         activearrays = self.pre_step(step)
 
         dyn_mat = get_dynmat(
-            activearrays["hessian"], self.im.dbeads.m3, self.im.dbeads.nbeads
+            activearrays["hessian"], self.sm.dbeads.m3, self.sm.dbeads.nbeads
         )
         h_up_band = banded_hessian(
-            dyn_mat, self.im, masses=False, shift=0.0000001
+            dyn_mat, self.sm, masses=False, shift=0.0000001
         )  # create upper band matrix
 
-        fff = activearrays["old_f"] * (self.im.coef[1:] + self.im.coef[:-1]) / 2
-        f = (fff + self.im.f).reshape(
-            self.im.dbeads.natoms * 3 * self.im.dbeads.nbeads, 1
+        fff = activearrays["old_f"] * (self.mapper.coef[1:] + self.mapper.coef[:-1]) / 2
+        f = (fff + self.sm.f).reshape(
+            self.sm.dbeads.natoms * 3 * self.sm.dbeads.nbeads, 1
         )
-        f = np.multiply(f, self.im.dbeads.m3.reshape(f.shape) ** -0.5)
+        f = np.multiply(f, self.sm.dbeads.m3.reshape(f.shape) ** -0.5)
 
-        d_x = invmul_banded(h_up_band, f).reshape(self.im.dbeads.q.shape)
-        d_x = np.multiply(d_x, self.im.dbeads.m3**-0.5)
+        d_x = invmul_banded(h_up_band, f).reshape(self.sm.dbeads.q.shape)
+        d_x = np.multiply(d_x, self.sm.dbeads.m3**-0.5)
 
         # Rescale step if necessary
         if np.amax(np.absolute(d_x)) > activearrays["big_step"]:
             info(
                 "Step norm, scaled down to {}".format(activearrays["big_step"]),
                 verbosity.low,
             )
@@ -1271,55 +1648,55 @@
         super(LanczosOptimizer, self).bind(geop)
 
     def initialize(self, step):
         # call initialize function from HessianOptimizer
         super(LanczosOptimizer, self).initialize(step)
 
     def step(self, step=None):
-        """Does one simulation time step."""
+        """Does one simulation step."""
 
         activearrays = self.pre_step(step)
 
-        fff = activearrays["old_f"] * (self.im.coef[1:] + self.im.coef[:-1]) / 2
-        f = (fff + self.im.f).reshape(
-            self.im.dbeads.natoms * 3 * self.im.dbeads.nbeads, 1
+        f = self.mapper.f.reshape(
+            self.fix.fixbeads.natoms * 3 * self.fix.fixbeads.nbeads, 1
         )
 
         banded = False
         banded = True
         if banded:
             # BANDED Version
             # MASS-scaled
             dyn_mat = get_dynmat(
-                activearrays["hessian"], self.im.dbeads.m3, self.im.dbeads.nbeads
+                activearrays["hessian"], self.fix.fixbeads.m3, self.fix.fixbeads.nbeads
             )
+
             h_up_band = banded_hessian(
-                dyn_mat, self.im, masses=False, shift=0.000000001
+                dyn_mat, self.mapper.sm, masses=False, shift=0.0000001
             )  # create upper band matrix
-            f = np.multiply(f, self.im.dbeads.m3.reshape(f.shape) ** -0.5)
+            f = np.multiply(f, self.fix.fixbeads.m3.reshape(f.shape) ** -0.5)
             # CARTESIAN
-            # h_up_band = banded_hessian(activearrays["hessian"], self.im,masses=True)  # create upper band matrix
+            # h_up_band = banded_hessian(activearrays["hessian"], self.sm.masses=True)  # create upper band matrix
 
             d = diag_banded(h_up_band)
         else:
             # FULL dimensions version
             h_0 = red2comp(
                 activearrays["hessian"],
-                self.im.dbeads.nbeads,
-                self.im.dbeads.natoms,
-                self.im.coef,
+                self.sm.dbeads.nbeads,
+                self.sm.dbeads.natoms,
+                self.mapper.coef,
             )
-            h_test = np.add(self.im.h, h_0)  # add spring terms to the physical hessian
+            h_test = np.add(self.sm.h, h_0)  # add spring terms to the physical hessian
             d, w = clean_hessian(
                 h_test,
-                self.im.dbeads.q,
-                self.im.dbeads.natoms,
-                self.im.dbeads.nbeads,
-                self.im.dbeads.m,
-                self.im.dbeads.m3,
+                self.sm.dbeads.q,
+                self.sm.dbeads.natoms,
+                self.sm.dbeads.nbeads,
+                self.sm.dbeads.m,
+                self.sm.dbeads.m3,
                 None,
             )
             # CARTESIAN
             # d,w =np.linalg.eigh(h_test) #Cartesian
         info(
             "\n@Lanczos: 1st freq {} cm^-1".format(
                 units.unit_to_user(
@@ -1374,18 +1751,18 @@
         if banded:
             h_up_band[-1, :] += -np.ones(h_up_band.shape[1]) * lamb
             d_x = invmul_banded(h_up_band, f)
         else:
             h_test = alpha * (h_test - np.eye(h_test.shape[0]) * lamb)
             d_x = np.linalg.solve(h_test, f)
 
-        d_x.shape = self.im.dbeads.q.shape
+        d_x.shape = self.fix.fixbeads.q.shape
 
         # MASS-scaled
-        d_x = np.multiply(d_x, self.im.dbeads.m3**-0.5)
+        d_x = np.multiply(d_x, self.fix.fixbeads.m3**-0.5)
 
         # Rescale step if necessary
         if np.amax(np.absolute(d_x)) > activearrays["big_step"]:
             info(
                 "Step norm, scaled down to {}".format(activearrays["big_step"]),
                 verbosity.low,
             )
@@ -1405,23 +1782,23 @@
 
         if geop.optarrays["hessian"].size == (self.beads.natoms * 3) ** 2:
             self.optarrays["initial_hessian"] = geop.optarrays["hessian"].copy()
             geop.optarrays["hessian"] = np.zeros(
                 (self.beads.natoms * 3, self.beads.q.size)
             )
 
-        if geop.options["hessian_final"] == "true":
+        if geop.options["hessian_final"]:
             self.options["hessian_asr"] = geop.options["hessian_asr"]
             if geop.optarrays["hessian"].size == 0:
                 geop.optarrays["hessian"] = np.zeros(
                     (self.beads.natoms * 3, self.beads.q.size)
                 )
             self.optarrays["hessian"] = geop.optarrays["hessian"]
 
-        self.im.bind(self, self.options["discretization"])
+        # self.sm.bind(self, self.options["discretization"])
 
         # Specific for LBFGS
         self.options["corrections"] = geop.options["corrections"]
         self.options["ls_options"] = geop.options["ls_options"]
         if geop.optarrays["qlist"].size != (
             self.options["corrections"] * self.beads.q.size
         ):
@@ -1455,15 +1832,15 @@
                     (self.beads.nbeads, 3 * self.beads.natoms), float
                 )
             else:
                 raise ValueError("Initial direction size does not match system size")
 
         self.optarrays["d"] = geop.optarrays["d"]
 
-        self.fm.esum = True
+        self.mapper.esum = True
 
     def initialize(self, step):
         if step == 0:
             info(" @GEOP: Initializing instanton", verbosity.low)
 
             if self.beads.nbeads == 1:
                 raise ValueError(
@@ -1477,26 +1854,29 @@
                 else:
                     info(
                         " @GEOP: Starting from the provided geometry in the extended phase space",
                         verbosity.low,
                     )
 
         # This must be done after the stretching and before the self.d.
-        if self.im.f is None:
-            self.im(self.beads.q, ret=False)  # Init instanton mapper
+        # Initialize all the mapper
+        self.mapper.initialize(self.beads.q, self.forces)
+        # if self.mapper.sm.f is None:
+        #    self.mapper.sm(self.beads.q, ret=False)  # Init instanton mapper
 
         if (
             self.optarrays["old_x"]
             == np.zeros((self.beads.nbeads, 3 * self.beads.natoms), float)
         ).all():
             self.optarrays["old_x"][:] = self.beads.q
 
         # Specific for LBFGS
         if np.linalg.norm(self.optarrays["d"]) == 0.0:
-            f = self.forces.f + self.im.f
+            # f = self.forces.f + self.mapper.sm.f
+            f = self.mapper.f
             self.optarrays["d"] += dstrip(f) / np.sqrt(np.dot(f.flatten(), f.flatten()))
 
         self.update_old_pos_for()
         self.init = True
 
     def post_step(self, step, activearrays):
         """General tasks that have to be performed after the  actual step"""
@@ -1518,26 +1898,36 @@
         d_x_max = np.amax(
             np.absolute(np.subtract(self.beads.q, self.optarrays["old_x"]))
         )
         self.exit = self.exitstep(d_x_max, step)
         self.update_old_pos_for()
 
     def step(self, step=None):
-        """Does one simulation time step."""
+        """Does one simulation step."""
 
         activearrays = self.pre_step(step)
 
-        e, g = self.fm(self.beads.q)
+        e, g = self.mapper(self.beads.q)
         fdf0 = (e, g)
 
         # Do one step. Update the position and force inside the mapper.
+        print(
+            activearrays["big_step"],
+            self.options["ls_options"]["tolerance"],
+            self.options["tolerances"]["energy"],
+            self.options["ls_options"]["iter"],
+            self.options["corrections"],
+            self.options["scale"],
+            step,
+        )
+
         L_BFGS(
             activearrays["old_x"],
             activearrays["d"],
-            self.fm,
+            self.mapper,
             activearrays["qlist"],
             activearrays["glist"],
             fdf0,
             activearrays["big_step"],
             self.options["ls_options"]["tolerance"]
             * self.options["tolerances"]["energy"],
             self.options["ls_options"]["iter"],
```

### Comparing `ipi-2.6.0/ipi/engine/motion/motion.py` & `ipi-2.6.3/ipi/engine/motion/motion.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 import numpy as np
 
-from ipi.utils.depend import depend_value
-from ipi.utils.depend import dd
-from ipi.utils.depend import dobject
+from ipi.utils.depend import depend_value, dproperties
 
 
-class Motion(dobject):
-
+class Motion:
     """Base motion calculation class.
 
     Gives the standard methods and attributes needed in all the
     motion calculation classes.
 
     Attributes:
         beads: A beads object giving the atoms positions.
@@ -39,16 +36,15 @@
         Args:
            fixcom: An optional boolean which decides whether the centre of mass
               motion will be constrained or not. Defaults to False.
            fixatoms: A list of atoms that should be held fixed to their
              initial positions.
         """
 
-        dself = dd(self)
-        dself.dt = depend_value(name="dt", value=0.0)
+        self._dt = depend_value(name="dt", value=0.0)
         self.fixcom = fixcom
         if fixatoms is None:
             self.fixatoms = np.zeros(0, int)
         else:
             self.fixatoms = fixatoms
 
         self.beads = self.cell = self.forces = self.prng = self.nm = None
@@ -81,7 +77,10 @@
         self.ensemble = ens
         self.output_maker = omaker
 
     def step(self, step=None):
         """Dummy simulation time step which does nothing."""
 
         pass
+
+
+dproperties(Motion, "dt")
```

### Comparing `ipi-2.6.0/ipi/engine/motion/multi.py` & `ipi-2.6.3/ipi/engine/motion/multi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """TODO
 """
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
-from ipi.utils.depend import depend_value, dd
+from ipi.utils.depend import depend_value, dproperties
 from ipi.engine.motion import Motion
 
 
 class MultiMotion(Motion):
-
     """A class to hold multiple motion objects to be executed serially."""
 
     def __init__(self, motionlist=None):
         """Initialises MultiMotion.
 
         Args:
            fixcom: An optional boolean which decides whether the centre of mass
               motion will be constrained or not. Defaults to False.
         """
 
-        dself = dd(self)
-        dself.dt = depend_value(name="dt", func=self.get_totdt)
+        self._dt = depend_value(name="dt", func=self.get_totdt)
         self.mlist = motionlist
         for m in self.mlist:
-            dd(m).dt.add_dependant(dself.dt)
+            m._dt.add_dependant(self._dt)
         a = (  # noqa
             self.dt
         )  # DON'T ASK WHY BUT IF YOU DON'T DO THAT WEAKREFS TO SELF.DT WILL BE INVALIDATED
 
         self.fixatoms = set(self.mlist[0].fixatoms)
         for m in self.mlist:
             self.fixatoms = self.fixatoms.intersection(m.fixatoms)
@@ -66,7 +64,10 @@
             bforce: The forcefield object from which the force and virial are taken.
             prng: The random number generator object which controls random number
                 generation.
         """
 
         for m in self.mlist:
             m.bind(ens, beads, nm, cell, bforce, prng, omaker)
+
+
+dproperties(MultiMotion, "dt")
```

### Comparing `ipi-2.6.0/ipi/engine/motion/neb.py` & `ipi-2.6.3/ipi/engine/motion/neb.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/engine/motion/phonons.py` & `ipi-2.6.3/ipi/engine/motion/phonons.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 
 __all__ = ["DynMatrixMover"]
 
 import numpy as np
 
 
 from ipi.engine.motion import Motion
-from ipi.utils.depend import *
+from ipi.utils.depend import dstrip
 from ipi.utils.softexit import softexit
 from ipi.utils.messages import verbosity, info
 
 
 class DynMatrixMover(Motion):
-
     """Dynamic matrix calculation routine by finite difference."""
 
     def __init__(
         self,
         fixcom=False,
         fixatoms=None,
         mode="fd",
@@ -166,28 +165,30 @@
         outfile = self.output_maker.get_output(self.prefix + ".eigval", "w")
         outfile.write("# Eigenvalues (atomic units)" + wstr + "\n")
         outfile.write("\n".join(map(str, eigsys[0])))
         outfile.close_stream()
 
         # prints eigenvectors
         outfile = self.output_maker.get_output(self.prefix + ".eigvec", "w")
-        outfile.write("# Eigenvector  matrix (normalized)" + "\n")
+        outfile.write(
+            "# Eigenvector  matrix from the dynamical matrix (normalized)" + "\n"
+        )
         for i in range(activedof):
             outfile.write(" ".join(map(str, eigsys[1][i])) + "\n")
         outfile.close_stream()
 
         # prints eigenmodes
         eigmode = 1.0 * eigsys[1]
         for i in range(activedof):
             eigmode[i] *= ism[i]
         for i in range(activedof):
             eigmode[:, i] /= np.sqrt(np.dot(eigmode[:, i], eigmode[:, i]))
         outfile = self.output_maker.get_output(self.prefix + ".mode", "w")
 
-        outfile.write("# Phonon modes (mass-scaled)" + "\n")
+        outfile.write("# Phonon modes (cartesian space and normalized)" + "\n")
         for i in range(activedof):
             outfile.write(" ".join(map(str, eigmode[i])) + "\n")
         outfile.close_stream()
 
     def apply_asr(self, dm):
         """
         Removes the translations and/or rotations depending on the asr mode.
@@ -280,16 +281,15 @@
 
             # Computes the transformation matrix.
             transfmatrix = np.eye(3 * self.beads.natoms) - np.dot(D.T, D)
             r = np.dot(transfmatrix.T, np.dot(dm, transfmatrix))
             return r
 
 
-class DummyPhononCalculator(dobject):
-
+class DummyPhononCalculator:
     """No-op PhononCalculator"""
 
     def __init__(self):
         pass
 
     def bind(self, dm):
         """Reference all the variables for simpler access."""
@@ -301,15 +301,14 @@
 
     def transform(self):
         """Dummy transformation step which does nothing."""
         pass
 
 
 class FDPhononCalculator(DummyPhononCalculator):
-
     """Finite difference phonon evaluator."""
 
     def bind(self, dm):
         """Reference all the variables for simpler access."""
         super(FDPhononCalculator, self).bind(dm)
 
         # Initialises a 3*number of atoms X 3*number of atoms dynamic matrix.
@@ -368,15 +367,14 @@
         dm = self.dm.dynmatrix.copy()
         rdm = self.dm.dynmatrix.copy()
         self.dm.dynmatrix = 0.50 * (dm + dm.T)
         self.dm.refdynmatrix = 0.50 * (rdm + rdm.T)
 
 
 class NMFDPhononCalculator(FDPhononCalculator):
-
     """Normal mode finite difference phonon evaluator."""
 
     def bind(self, dm):
         """Reference all the variables for simpler access."""
         super(NMFDPhononCalculator, self).bind(dm)
 
         if np.array_equal(
@@ -421,15 +419,14 @@
             self.dm.U, np.dot(self.dm.refdynmatrix, np.transpose(self.dm.U))
         )
         rdm = self.dm.dynmatrix.copy()
         self.dm.refdynmatrix = 0.50 * (rdm + rdm.T)
 
 
 class ENMFDPhononCalculator(NMFDPhononCalculator):
-
     """Energy scaled normal mode finite difference phonon evaluator."""
 
     def step(self, step=None):
         """Computes one row of the dynamic matrix."""
 
         # initializes the finite deviation
         vknorm = np.sqrt(np.dot(self.dm.V[:, step], self.dm.V[:, step]))
```

### Comparing `ipi-2.6.0/ipi/engine/motion/planetary.py` & `ipi-2.6.3/ipi/engine/motion/planetary.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,17 @@
 
         self.mode = mode
         self.nsamples = nsamples
         self.stride = stride
         self.nbeads = nbeads
         self.screen = screen
 
-        dself = dd(self)
-
         # the planetary step just computes constrained-centroid properties so it
         # should not advance the timer
-        dself.dt = depend_value(name="dt", value=0.0)
-        # dset(self, "dt", depend_value(name="dt", value = 0.0) )
+        self._dt = depend_value(name="dt", value=0.0)
         self.fixatoms = np.asarray([])
         self.fixcom = True
 
         # nvt-cc means contstant-temperature with constrained centroid
         # this basically is a motion class that will be used to make the
         # centroid propagation at each time step
         self.ccdyn = Dynamics(
@@ -275,7 +272,10 @@
 
         self.tsave += time.time()
         info(
             "@ PLANETARY MODEL Average timing: %f s, %f s, %f s\n"
             % (self.tmc / self.neval, self.tmtx / self.neval, self.tsave / self.neval),
             verbosity.high,
         )
+
+
+dproperties(Planetary, "dt")
```

### Comparing `ipi-2.6.0/ipi/engine/motion/ramp.py` & `ipi-2.6.3/ipi/engine/motion/ramp.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/engine/motion/replay.py` & `ipi-2.6.3/ipi/engine/motion/replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from ipi.utils.messages import verbosity, info
 
 
 __all__ = ["Replay"]
 
 
 class Replay(Motion):
-
     """Calculator object that just loads snapshots from an external file in sequence.
 
     Has the relevant conserved quantity and normal mode propagator for the
     constant energy ensemble. Note that a temperature of some kind must be
     defined so that the spring potential can be calculated.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/engine/motion/scphonons.py` & `ipi-2.6.3/ipi/engine/motion/scphonons.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 """
 
 __all__ = ["SCPhononsMover"]
 
 import os
 import numpy as np
 from ipi.engine.motion.motion import Motion
-from ipi.utils.depend import *
 
-# from ipi.utils import units
+from ipi.utils.depend import dstrip
 from ipi.utils.phonontools import apply_asr
 from ipi.utils.softexit import softexit
 from ipi.utils.messages import verbosity, info
 from ipi.utils.mathtools import gaussian_inv
 
 try:
     from pyscenarios.sobol import sobol
@@ -138,15 +137,15 @@
         self.dforces = self.forces.copy(self.dbeads, self.dcell)
 
         # Sets temperature.
         self.temp = self.ensemble.temp
         self.m = dstrip(self.beads.m).copy()
 
         # Initializes mass related arrays.
-        self.m3 = dstrip(self.beads.m3[-1])
+        self.m3 = dstrip(self.beads.m3)[-1]
         self.im3 = np.divide(1.0, self.m3)
         self.sqm3 = np.sqrt(self.m3)
         self.isqm3 = np.sqrt(self.im3)
 
         # Initializes mass related diagonal matrices.
         self.M = np.diag(self.m3)
         self.iM = np.diag(self.im3)
@@ -167,27 +166,27 @@
         self.fginv = np.vectorize(gaussian_inv)
 
         # TODO implement an option to give the file name to fetch the random samples. Also implement check of dimensionality, and raise an error if it runs out of random numbers
         # reads sobol points from file!
         if self.random_type == "file":
             self.random_sequence = np.loadtxt("SOBOL-RNG")
         elif self.random_type == "pseudo":
-            self.random_sequence = self.prng.rng.rand(
-                self.max_steps * self.max_iter, self.dof
+            self.random_sequence = self.prng.rng[0].uniform(
+                size=(self.max_steps * self.max_iter, self.dof)
             )
         elif self.random_type == "sobol":
             self.random_sequence = np.asarray(
                 [
                     sobol(self.dof, i)
                     for i in range(0, self.max_steps * self.max_iter + 1)
                 ]
             )
 
         # Shuffles the
-        self.prng.rng.shuffle(self.random_shuffle)
+        self.prng.rng[0].shuffle(self.random_shuffle)
 
     def step(self, step=None):
         if self.isc == self.max_iter:
             softexit.trigger(
                 status="bad",
                 message=" @SCP: Reached maximum iterations. Terminating the SCP calculation.",
             )
@@ -196,15 +195,15 @@
         elif self.imc >= 1 and self.imc <= self.max_steps:
             self.phononator.step(step)
         elif self.imc > self.max_steps:
             self.phononator.print_energetics()
             self.phononator.displace()
 
 
-class DummyPhononator(dobject):
+class DummyPhononator:
     """No-op phononator"""
 
     def __init__(self):
         pass
 
     def bind(self, dm):
         """Reference all the variables for simpler access."""
@@ -709,16 +708,16 @@
         and the batch weights.
         """
 
         # Creates new variable names for easier referencing.
         qp, Kp, i = self.dm.beads.q, self.dm.K, self.dm.isc - 1
 
         # Takes the set of forces calculated at the previous step for (self.q, self.iD)
-        avg_f = dstrip(self.f[i]).copy()[-1] * 0.0
-        var_f = dstrip(self.f[i]).copy()[-1] * 0.0
+        avg_f = dstrip(self.f[i])[-1] * 0.0
+        var_f = dstrip(self.f[i])[-1] * 0.0
         norm = 0.0
         batch_w = np.zeros(self.dm.isc)
 
         for i in range(self.dm.isc):
             # Calculates the harmonic force.
             f = self.f[i]
             x = self.x[i]
@@ -744,15 +743,15 @@
         Returns the reweighted Hessian.
         """
 
         # Creates new variable names for easier referencing.
         qp, iDp, Kp, i = self.dm.beads.q, self.dm.iD, self.dm.K, self.dm.isc - 1
 
         # Takes the set of forces calculated at the previous step for (self.q, self.iD)
-        avg_K = dstrip(self.dm.iD).copy() * 0.0
+        avg_K = self.dm.iD * 0.0
         norm = 0.0
 
         for i in range(self.dm.isc):
             # Draws the random configurations and forces.
             f = self.f[i]
             x = self.x[i]
```

### Comparing `ipi-2.6.0/ipi/engine/motion/stringmep.py` & `ipi-2.6.3/ipi/engine/motion/stringmep.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         tau = d1 / npnorm(d1) + d2 / npnorm(d2)
         tau /= npnorm(tau)
 
         # Inverting the force component along the path
         rbf -= 2 * np.dot(rbf, tau) * tau
 
         # Return the potential energy and gradient of the climbing bead
-        e = dstrip(self.rforces.pot.copy())
+        e = self.rforces.pot
         g = -rbf
         info("@STRING_CLIMB: StringClimbGrMapper finished.", vrb.debug)
         return e, g
 
 
 class StringMover(Motion):
     """MEP optimization routine for the String method.
```

### Comparing `ipi-2.6.0/ipi/engine/motion/vscf.py` & `ipi-2.6.3/ipi/engine/motion/vscf.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,19 @@
         self.pair_range = pair_range
 
         if self.prefix == "":
             self.prefix = self.mode
 
     def bind(self, ens, beads, nm, cell, bforce, prng, omaker):
         super(NormalModeMover, self).bind(ens, beads, nm, cell, bforce, prng, omaker)
+
+        # TODO - A LOT OF THESE DEFINITIONS ARE NOT USING DEPEND OBJECTS CORRECTLY
+        # MANY OF THESE SHOUD BE LINKED THROUGH DPIPE, NOT DEREFERENCED. THIS WOULD
+        # BREAK IF USED WITH REPLICA EXCHANGE FOR INSTANCE.
+
         self.temp = self.ensemble.temp
 
         # Raises error for nbeads not equal to 1.
         if self.beads.nbeads > 1:
             raise ValueError(
                 "Calculation not possible for number of beads greater than one."
             )
@@ -145,15 +150,15 @@
         self.dforces = self.forces.copy(self.dbeads, self.dcell)
 
     def step(self, step=None):
         """Executes one step of phonon computation."""
         self.calc.step(step)
 
 
-class DummyCalculator(dobject):
+class DummyCalculator:
     """No-op Calculator"""
 
     def __init__(self):
         pass
 
     def bind(self, imm):
         """Reference all the variables for simpler access."""
@@ -199,15 +204,15 @@
         # Sets
         self.imm.w2[np.abs(self.imm.w2) < 1e-15] = 0.0
         self.imm.nz = sum(np.abs(self.imm.w2) < 1e-15)
 
         # Calculates the normal mode frequencies.
         # TODO : Should also handle soft modes.
         self.imm.w = self.imm.w2 * 0
-        self.imm.w[self.imm.nz :] = np.sqrt(dstrip(self.imm.w2[self.imm.nz :]))
+        self.imm.w[self.imm.nz :] = np.sqrt(self.imm.w2[self.imm.nz :])
 
         self.imm.V = self.imm.U.copy()
         for i in range(len(self.imm.V)):
             self.imm.V[:, i] *= self.imm.ism
 
         # Harm ZP RMS displacement along normal mode
         # Not temperature dependent so that sampled potentials can easily be
@@ -315,17 +320,17 @@
             h[i][i] += 0.5 * (i + 0.5) * hw
         h += h.T
 
         # Diagonalise Hamiltonian matrix and evaluate anharmonic free energy and vibrational freq
         evals, evecs = np.linalg.eigh(h)
 
         # Calculates the free and internal energy
-        A = -logsumexp(-1.0 * evals / dstrip(self.imm.temp)) * dstrip(self.imm.temp)
-        E = np.sum(evals * np.exp(-1.0 * evals / dstrip(self.imm.temp))) / np.sum(
-            np.exp(-1.0 * evals / dstrip(self.imm.temp))
+        A = -logsumexp(-1.0 * evals / self.imm.temp) * self.imm.temp
+        E = np.sum(evals * np.exp(-1.0 * evals / self.imm.temp)) / np.sum(
+            np.exp(-1.0 * evals / self.imm.temp)
         )
 
         if return_eigsys:
             return A, E, evals, evecs.T
         else:
             return A, E
 
@@ -624,41 +629,36 @@
                 % (self.imm.prefix + "." + str(step) + ".vfit"),
                 verbosity.medium,
             )
             outfile.close_stream()
 
         # Done converging wrt size of SHO basis.
         # Calculates the harmonic free and internal energy.
-        Ahar = -logsumexp(
-            [
-                -1.0 * np.sqrt(self.imm.w2[step]) * (0.5 + i) / dstrip(self.imm.temp)
-                for i in range(nnbasis)
-            ]
-        ) * dstrip(self.imm.temp)
+        Ahar = (
+            -logsumexp(
+                [
+                    -1.0 * np.sqrt(self.imm.w2[step]) * (0.5 + i) / self.imm.temp
+                    for i in range(nnbasis)
+                ]
+            )
+            * self.imm.temp
+        )
         Zhar = np.sum(
             [
-                np.exp(
-                    -1.0
-                    * np.sqrt(self.imm.w2[step])
-                    * (0.5 + i)
-                    / dstrip(self.imm.temp)
-                )
+                np.exp(-1.0 * np.sqrt(self.imm.w2[step]) * (0.5 + i) / self.imm.temp)
                 for i in range(nnbasis)
             ]
         )
         Ehar = (
             np.sum(
                 [
                     np.sqrt(self.imm.w2[step])
                     * (0.5 + i)
                     * np.exp(
-                        -1.0
-                        * np.sqrt(self.imm.w2[step])
-                        * (0.5 + i)
-                        / dstrip(self.imm.temp)
+                        -1.0 * np.sqrt(self.imm.w2[step]) * (0.5 + i) / self.imm.temp
                     )
                     for i in range(nnbasis)
                 ]
             )
             / Zhar
         )
```

### Comparing `ipi-2.6.0/ipi/engine/normalmodes.py` & `ipi-2.6.3/ipi/engine/normalmodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from ipi.utils import nmtransform
 from ipi.utils.messages import verbosity, warning, info
 from ipi.utils.exchange import *
 
 __all__ = ["NormalModes"]
 
 
-class NormalModes(dobject):
-
+class NormalModes:
     """Handles the path normal modes.
 
     Normal-modes transformation, determination of path frequencies,
     dynamical mass matrix change, etc.
 
     Attributes:
        natoms: The number of atoms.
@@ -37,14 +36,15 @@
           be done.
        ensemble: The ensemble object, specifying the temperature to hold the
           system to.
        motion: The motion object that will need normal-mode transformation and propagator
        transform: A nm_trans object that contains the functions that are
           required for the normal mode transformation.
 
+
     Depend objects:
        mode: A string specifying how the bead masses are chosen.
        transform_method: A string specifying how to do the normal mode
           transformation.
        nm_freqs: An array that specifies how the normal mode frequencies
           of the ring polymers are to be calculated, and thus how the
           bead masses should be chosen.
@@ -83,14 +83,16 @@
         transform_method="fft",
         propagator="exact",
         freqs=None,
         open_paths=None,
         bosons=None,
         dt=1.0,
         nmts=1,
+        fft_threads=1,
+        fft_float32=False,
     ):
         """Initializes NormalModes.
 
         Sets the options for the normal mode transform.
 
         Args:
            mode: A string specifying how to calculate the bead masses.
@@ -99,47 +101,50 @@
            freqs: A list of data used to calculate the dynamical mass factors.
         """
 
         if freqs is None:
             freqs = []
         if open_paths is None:
             open_paths = []
-        if bosons is None:
-            bosons = []
         self.open_paths = np.asarray(open_paths, int)
-        self.bosons = np.asarray(bosons, int)
-        dself = dd(self)
-        dself.nmts = depend_value(name="nmts", value=nmts)
-        dself.dt = depend_value(name="dt", value=dt)
-        dself.mode = depend_value(name="mode", value=mode)
-        dself.transform_method = depend_value(
+        if bosons is None:
+            bosons = np.zeros(0, int)
+        self._bosons = depend_value(name="bosons", value=bosons)
+        self._nmts = depend_value(name="nmts", value=nmts)
+        self._dt = depend_value(name="dt", value=dt)
+        self._mode = depend_value(name="mode", value=mode)
+        self._transform_method = depend_value(
             name="transform_method", value=transform_method
         )
-        dself.propagator = depend_value(name="propagator", value=propagator)
-        dself.nm_freqs = depend_array(name="nm_freqs", value=np.asarray(freqs, float))
+        self._propagator = depend_value(name="propagator", value=propagator)
+        self._nm_freqs = depend_array(name="nm_freqs", value=np.asarray(freqs, float))
+        self.fft_threads = fft_threads
+        self.fft_float32 = fft_float32
 
     def copy(self, freqs=None):
-        """Creates a new beads object from the original.
+        """Creates a new NormalModes object from the original.
 
         Returns:
-           A Beads object with the same q, p, m and names arrays as the original.
+           A NormalModes object with the same arrays as the original.
         """
 
         if freqs is None:
             freqs = self.nm_freqs.copy()
 
         newnm = NormalModes(
             self.mode,
             self.transform_method,
             self.propagator,
             freqs,
             self.open_paths,
             self.bosons,
             self.dt,
             self.nmts,
+            self.fft_threads,
+            self.fft_float32,
         )
         return newnm
 
     def bind(self, ensemble, motion, beads=None, forces=None):
         """Initializes the normal modes object and binds to beads and ensemble.
 
         Do all the work down here as we need a full-formed necklace and ensemble
@@ -157,286 +162,281 @@
         else:
             self.beads = beads
 
         self.forces = forces
         self.nbeads = beads.nbeads
         self.natoms = beads.natoms
 
-        # if ( (len(self.bosons) > 0) and (len(self.bosons) < self.natoms) ):
-        # raise(IOError("@NormalModes : Currently, only full bosonic/distinguishable simulations are allowed"))
-        if len(self.bosons) > self.natoms:
-            raise IOError
+        # storage space for the propagator
+        self.pq_buffer = np.zeros((2, self.natoms * 3), float)
 
-        dself = dd(self)
+        self.bosons = self.resolve_bosons()
 
         # stores a reference to the bound beads and ensemble objects
         self.ensemble = ensemble
-        dpipe(dd(motion).dt, dself.dt)
+        dpipe(motion._dt, self._dt)
 
         # sets up what's necessary to perform nm transformation.
         if self.nbeads == 1:  # classical trajectory! don't waste time doing anything!
             self.transform = nmtransform.nm_noop(nbeads=self.nbeads)
         elif self.transform_method == "fft":
             self.transform = nmtransform.nm_fft(
-                nbeads=self.nbeads, natoms=self.natoms, open_paths=self.open_paths
+                nbeads=self.nbeads,
+                natoms=self.natoms,
+                open_paths=self.open_paths,
+                n_threads=self.fft_threads,
+                single_precision=self.fft_float32,
             )
         elif self.transform_method == "matrix":
             self.transform = nmtransform.nm_trans(
                 nbeads=self.nbeads, open_paths=self.open_paths
             )
 
         # creates arrays to store normal modes representation of the path.
         # must do a lot of piping to create "ex post" a synchronization between the beads and the nm
         sync_q = synchronizer()
         sync_p = synchronizer()
-        dself.qnm = depend_array(
+        self._qnm = depend_array(
             name="qnm",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
             func={"q": (lambda: self.transform.b2nm(dstrip(self.beads.q)))},
             synchro=sync_q,
         )
-        dself.pnm = depend_array(
+        self._pnm = depend_array(
             name="pnm",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
             func={"p": (lambda: self.transform.b2nm(dstrip(self.beads.p)))},
             synchro=sync_p,
         )
 
         # must overwrite the functions
-        dd(self.beads).q._func = {
-            "qnm": (lambda: self.transform.nm2b(dstrip(self.qnm)))
-        }
-        dd(self.beads).p._func = {
-            "pnm": (lambda: self.transform.nm2b(dstrip(self.pnm)))
-        }
-        dd(self.beads).q.add_synchro(sync_q)
-        dd(self.beads).p.add_synchro(sync_p)
+        self.beads._q._func = {"qnm": (lambda: self.transform.nm2b(dstrip(self.qnm)))}
+        self.beads._p._func = {"pnm": (lambda: self.transform.nm2b(dstrip(self.pnm)))}
+        self.beads._q.add_synchro(sync_q)
+        self.beads._p.add_synchro(sync_p)
 
         # also within the "atomic" interface to beads
         for b in range(self.nbeads):
-            dd(self.beads._blist[b]).q._func = {
+            self.beads._blist[b]._q._func = {
                 "qnm": (lambda: self.transform.nm2b(dstrip(self.qnm)))
             }
-            dd(self.beads._blist[b]).p._func = {
+            self.beads._blist[b]._p._func = {
                 "pnm": (lambda: self.transform.nm2b(dstrip(self.pnm)))
             }
-            dd(self.beads._blist[b]).q.add_synchro(sync_q)
-            dd(self.beads._blist[b]).p.add_synchro(sync_p)
+            self.beads._blist[b]._q.add_synchro(sync_q)
+            self.beads._blist[b]._p.add_synchro(sync_p)
 
         # finally, we mark the beads as those containing the set positions
-        dd(self.beads).q.update_man()
-        dd(self.beads).p.update_man()
+        self.beads._q.update_man()
+        self.beads._p.update_man()
 
         # forces can be converted in nm representation, but here it makes no sense to set up a sync mechanism,
         # as they always get computed in the bead rep
         if self.forces is not None:
-            dself.fnm = depend_array(
+            self._fnm = depend_array(
                 name="fnm",
                 value=np.zeros((self.nbeads, 3 * self.natoms), float),
                 func=(lambda: self.transform.b2nm(dstrip(self.forces.f))),
-                dependencies=[dd(self.forces).f],
+                dependencies=[self.forces._f],
             )
         else:  # have a fall-back plan when we don't want to initialize a force mechanism, e.g. for ring-polymer initialization
-            dself.fnm = depend_array(
+            self._fnm = depend_array(
                 name="fnm",
                 value=np.zeros((self.nbeads, 3 * self.natoms), float),
                 func=(
                     lambda: depraise(
                         ValueError(
                             "Cannot access NM forces when initializing the NM object without providing a force reference!"
                         )
                     )
                 ),
                 dependencies=[],
             )
 
         # create path-frequencies related properties
-        dself.omegan = depend_value(
-            name="omegan", func=self.get_omegan, dependencies=[dd(self.ensemble).temp]
+        self._omegan = depend_value(
+            name="omegan", func=self.get_omegan, dependencies=[self.ensemble._temp]
         )
-        dself.omegan2 = depend_value(
-            name="omegan2", func=self.get_omegan2, dependencies=[dself.omegan]
+        self._omegan2 = depend_value(
+            name="omegan2", func=self.get_omegan2, dependencies=[self._omegan]
         )
-        dself.omegak = depend_array(
+        self._omegak = depend_array(
             name="omegak",
             value=np.zeros(self.beads.nbeads, float),
             func=self.get_omegak,
-            dependencies=[dself.omegan],
+            dependencies=[self._omegan],
         )
-        dself.omegak2 = depend_array(
+        self._omegak2 = depend_array(
             name="omegak2",
             value=np.zeros(self.beads.nbeads, float),
             func=(lambda: self.omegak**2),
-            dependencies=[dself.omegak],
+            dependencies=[self._omegak],
         )
 
         # Add o_omegak to calculate the freq in the case of open path
-        dself.o_omegak = depend_array(
+        self._o_omegak = depend_array(
             name="o_omegak",
             value=np.zeros(self.beads.nbeads, float),
             func=self.get_o_omegak,
-            dependencies=[dself.omegan],
+            dependencies=[self._omegan],
         )
 
         # sets up "dynamical" masses -- mass-scalings to give the correct RPMD/CMD dynamics
-        dself.nm_factor = depend_array(
+        self._nm_factor = depend_array(
             name="nm_factor",
             value=np.zeros(self.nbeads, float),
             func=self.get_nmm,
-            dependencies=[dself.nm_freqs, dself.mode],
+            dependencies=[self._nm_freqs, self._mode],
         )
         # add o_nm_factor for the dynamical mass in the case of open paths
-        dself.o_nm_factor = depend_array(
+        self._o_nm_factor = depend_array(
             name="nmm",
             value=np.zeros(self.nbeads, float),
             func=self.get_o_nmm,
-            dependencies=[dself.nm_freqs, dself.mode],
+            dependencies=[self._nm_freqs, self._mode],
         )
-        dself.dynm3 = depend_array(
+        self._dynm3 = depend_array(
             name="dynm3",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
             func=self.get_dynm3,
-            dependencies=[dself.nm_factor, dd(self.beads).m3],
+            dependencies=[self._nm_factor, self.beads._m3],
         )
-        dself.dynomegak = depend_array(
+        self._dynomegak = depend_array(
             name="dynomegak",
             value=np.zeros(self.nbeads, float),
             func=self.get_dynwk,
-            dependencies=[dself.nm_factor, dself.omegak],
+            dependencies=[self._nm_factor, self._omegak],
         )
 
-        dself.dt = depend_value(name="dt", value=1.0)
-        dpipe(dd(self.motion).dt, dself.dt)
-        dself.prop_pq = depend_array(
+        self._dt = depend_value(name="dt", value=1.0)
+        dpipe(self.motion._dt, self._dt)
+
+        self._prop_pq = depend_array(
             name="prop_pq",
             value=np.zeros((self.beads.nbeads, 2, 2)),
             func=self.get_prop_pq,
-            dependencies=[dself.omegak, dself.nm_factor, dself.dt, dself.propagator],
+            dependencies=[self._omegak, self._nm_factor, self._dt, self._propagator],
         )
-        dself.o_prop_pq = depend_array(
+
+        # mass-scaled propagator
+        self._prop_pq_ms = depend_array(
+            name="prop_pq_ms",
+            value=np.zeros((2, 2, self.beads.nbeads, 3 * self.beads.natoms)),
+            func=self.get_prop_pq_ms,
+            dependencies=[self._prop_pq, self.beads._m3],
+        )
+
+        self._o_prop_pq = depend_array(
             name="o_prop_pq",
             value=np.zeros((self.beads.nbeads, 2, 2)),
             func=self.get_o_prop_pq,
             dependencies=[
-                dself.o_omegak,
-                dself.o_nm_factor,
-                dself.dt,
-                dself.propagator,
+                self._o_omegak,
+                self._o_nm_factor,
+                self._dt,
+                self._propagator,
             ],
         )
 
+        # mass-scaled propagator
+        self._o_prop_pq_ms = depend_array(
+            name="o_prop_pq_ms",
+            value=np.zeros((2, 2, self.beads.nbeads, 3 * len(self.open_paths))),
+            func=self.get_o_prop_pq_ms,
+            dependencies=[self._o_prop_pq, self.beads._m3],
+        )
+
+        self.open_paths_coords = np.array(
+            [[3 * i, 3 * i + 1, 3 * i + 2] for i in self.open_paths]
+        ).flatten()
+
         # if the mass matrix is not the RPMD one, the MD kinetic energy can't be
         # obtained in the bead representation because the masses are all mixed up
-        dself.kins = depend_array(
+        self._kins = depend_array(
             name="kins",
             value=np.zeros(self.nbeads, float),
             func=self.get_kins,
-            dependencies=[dself.pnm, dd(self.beads).sm3, dself.nm_factor],
+            dependencies=[self._pnm, self.beads._sm3, self._nm_factor],
         )
-        dself.kin = depend_value(
-            name="kin", func=self.get_kin, dependencies=[dself.kins]
+        self._kin = depend_value(
+            name="kin", func=self.get_kin, dependencies=[self._kins]
         )
-        dself.kstress = depend_array(
+        self._kstress = depend_array(
             name="kstress",
             value=np.zeros((3, 3), float),
             func=self.get_kstress,
-            dependencies=[dself.pnm, dd(self.beads).sm3, dself.nm_factor],
+            dependencies=[self._pnm, self.beads._sm3, self._nm_factor],
         )
 
-        # Array that holds both vspring and fspring for bosons
-        dself.vspring_and_fspring_B = depend_value(
-            name="v_and_fs_B",
+        self._vspring_and_fspring = depend_value(
+            name="v_and_fs",
             value=[None, None],
-            func=self.get_vspring_and_fspring_B,
-            dependencies=[dself.beads.q, dself.beads.m3, dself.omegan2],
-        )
-
-        # spring energy, calculated in normal modes
-        dself.vspring = depend_value(
-            name="vspring",
-            value=0.0,
-            func=self.get_vspring,
+            func=self.get_vspring_and_fspring,
             dependencies=[
-                dself.qnm,
-                dself.omegak,
-                dself.o_omegak,
-                dd(self.beads).m3,
-                dself.vspring_and_fspring_B,
+                self._qnm,
+                self._omegak,
+                self._o_omegak,
+                self.beads._m3,
+                self.beads._q,
             ],
         )
 
-        # spring forces on normal modes
-        dself.fspringnm = depend_array(
-            name="fspringnm",
-            value=np.zeros((self.nbeads, 3 * self.natoms), float),
-            func=self.get_fspringnm,
-            dependencies=[dself.qnm, dself.omegak, dd(self.beads).m3],
+        if len(self.bosons) > 0:
+            self.exchange_potential = ExchangePotential(self.nbeads, len(self.bosons))
+            self.exchange_potential.bind(self.beads, self.ensemble, self)
+            self._vspring_and_fspring.add_dependency(
+                self.exchange_potential._vspring_and_fspring
+            )
+        else:
+            self.exchange_potential = None
+
+        # just return split potential and force for ease of access
+        self._vspring = depend_value(
+            name="vspring",
+            value=0.0,
+            func=lambda: self.vspring_and_fspring[0],
+            dependencies=[self._vspring_and_fspring],
         )
 
-        # spring forces on beads, transformed from normal modes
-        dself.fspring = depend_array(
-            name="fs",
+        self._fspring = depend_array(
+            name="fspring",
             value=np.zeros((self.nbeads, 3 * self.natoms), float),
-            # func=(lambda: self.transform.nm2b(dstrip(self.fspringnm))),
-            func=self.get_fspring,
-            dependencies=[dself.fspringnm, dself.vspring_and_fspring_B],
+            func=lambda: self.vspring_and_fspring[1],
+            dependencies=[self._vspring_and_fspring],
         )
 
-    def get_fspringnm(self):
-        """Returns the spring force calculated in NM representation."""
-
-        return -self.beads.m3 * self.omegak[:, np.newaxis] ** 2 * self.qnm
-
-    def get_vspring(self):
-        """Returns the spring energy calculated in NM representation for distinguishable particles.
-        For bosons, get the first element of vspring_and_fspring_B[0]
-        For a mixture of both, calculate separately and combine.
-        """
-
-        if self.nbeads == 1:
-            return 0.0
-
-        if len(self.bosons) == 0:
-            sqnm = dstrip(self.qnm) * dstrip(self.beads.sm3)
-            q2 = (sqnm**2).sum(axis=1)
-
-            vspring = (self.omegak2 * q2).sum()
-
-            for j in self.open_paths:
-                vspring += (
-                    self.beads.m[j]
-                    * (self.o_omegak**2 - self.omegak**2)
-                    * (
-                        self.qnm[:, 3 * j] ** 2
-                        + self.qnm[:, 3 * j + 1] ** 2
-                        + self.qnm[:, 3 * j + 2] ** 2
-                    )
-                ).sum()
-
-            return vspring * 0.5
-
-        elif len(self.bosons) is self.natoms:
-            return self.vspring_and_fspring_B[0]
+    def resolve_bosons(self):
+        if not isinstance(self.bosons, tuple):
+            return self.bosons
+
+        bosons_lst, id_mode = self.bosons
+        if id_mode == "index":
+            bosons_array = bosons_lst.astype(int)
+        elif id_mode == "label":
+            for latom in bosons_lst:
+                if latom not in set(self.beads.names):
+                    raise ValueError("Unknown atom label %s for boson" % latom)
+            bosons_array = np.asarray(
+                [
+                    i
+                    for i in range(self.beads.natoms)
+                    if (self.beads.names[i] in bosons_lst)
+                ]
+            )
         else:
-            # Sum over only those particles who are distinguishable.
-            vspring = 0.0
+            raise ValueError(
+                "Error resolving boson identifies using unknown method %s" % id_mode
+            )
 
-            notbosons = list(set(range(self.natoms)) - set(self.bosons))
-            for j in notbosons:
-                vspring += (
-                    self.beads.m[j]
-                    * self.omegak**2
-                    * (
-                        self.qnm[:, 3 * j] ** 2
-                        + self.qnm[:, 3 * j + 1] ** 2
-                        + self.qnm[:, 3 * j + 2] ** 2
-                    )
-                ).sum()
+        if len(bosons_array) > 0 and (
+            np.min(bosons_array) < 0 or np.max(bosons_array) >= self.beads.natoms
+        ):
+            raise ValueError("Invalid index for boson, got %s" % str(bosons_array))
 
-            return vspring * 0.5 + self.vspring_and_fspring_B[0]
+        return bosons_array
 
     def get_omegan(self):
         """Returns the effective vibrational frequency for the interaction
         between replicas.
         """
 
         return (
@@ -515,14 +515,25 @@
                 s = np.sin(dtomegak)
                 pqk[b, 0, 0] = c
                 pqk[b, 1, 1] = c
                 pqk[b, 0, 1] = -s * self.omegak[b] * sk
                 pqk[b, 1, 0] = s / (self.omegak[b] * sk)
         return pqk
 
+    def get_prop_pq_ms(self):
+        """Combines the propagator with the atom masses to make a single array
+        that can be multiplied to propagate the normal modes dynamics"""
+
+        pq_ms = np.zeros((2, 2, self.nbeads, self.natoms * 3))
+        pq_ms[:] = np.moveaxis(dstrip(self.prop_pq), 0, -1)[:, :, :, np.newaxis]
+        pq_ms[0, 1] *= dstrip(self.beads.m3)
+        pq_ms[1, 0] /= dstrip(self.beads.m3)
+
+        return pq_ms
+
     def get_o_prop_pq(self):
         """Gets the normal mode propagator matrix for the open case.
 
         Note the special treatment for the centroid normal mode, which is
         propagated using the standard velocity Verlet algorithm as required.
         Note that both the normal mode positions and momenta are propagated
         using this matrix.
@@ -554,14 +565,26 @@
                 s = np.sin(dto_omegak)
                 pqk[b, 0, 0] = c
                 pqk[b, 1, 1] = c
                 pqk[b, 0, 1] = -s * self.o_omegak[b] * sk
                 pqk[b, 1, 0] = s / (self.o_omegak[b] * sk)
         return pqk
 
+    def get_o_prop_pq_ms(self):
+        """Combines the propagator with the atom masses to make a single array
+        that can be multiplied to propagate the normal modes dynamics. Open path version
+        """
+
+        pq_ms = np.zeros((2, 2, self.nbeads, len(self.open_paths_coords)))
+        pq_ms[:] = np.moveaxis(dstrip(self.o_prop_pq), 0, -1)[:, :, :, np.newaxis]
+        pq_ms[0, 1] *= dstrip(self.beads.m3[:, self.open_paths_coords])
+        pq_ms[1, 0] /= dstrip(self.beads.m3[:, self.open_paths_coords])
+
+        return pq_ms
+
     def get_nmm(self):
         """Returns dynamical mass factors, i.e. the scaling of normal mode
         masses that determine the path dynamics (but not statics)."""
 
         # also checks that the frequencies and the mode given in init are
         # consistent with the beads and ensemble
 
@@ -701,55 +724,79 @@
         # dynamical masses for the open paths
         for j in self.open_paths:
             for a in range(3 * j, 3 * (j + 1)):
                 for k in range(1, self.nbeads):
                     dm3[k, a] = self.beads.m3[k, a] * self.o_nm_factor[k]
         return dm3
 
-    def get_vspring_and_fspring_B(self):
-        """
-        Calculates spring forces and potential for bosons.
-        Evaluated using recursion relation from arXiv:1905.090.
-        """
+    def get_vspring_and_fspring(self):
+        """Returns the total spring energy and spring force."""
 
-        if len(self.bosons) == 0:
-            pass
-        else:
-            (E_k_N, V) = Evaluate_VB(self)
+        # classical simulation - do nothing!
+        vspring, fspring = 0.0, np.zeros_like(self.qnm)
+        if self.nbeads == 1:
+            return vspring, fspring
+
+        if len(self.bosons) < self.natoms:
+            # computes harmonic potential in normal-modes representation
+            qnm = dstrip(self.qnm)
+            sqnm = qnm * dstrip(self.beads.sm3)
+            q2 = (sqnm**2).sum(axis=1)
+
+            vspring += (self.omegak2 * q2).sum()
+            # spring forces (this is only the closed path version -
+            # open path correction is applied in the propagator)
+            # TODO make it happen here, it'd be probably cleaner
+            fspringnm = -self.beads.m3 * self.omegak[:, np.newaxis] ** 2 * qnm
 
-            P = self.nbeads
+            # correction for open paths
+            for j in self.open_paths:
+                vspring += (
+                    self.beads.m[j]
+                    * (self.o_omegak**2 - self.omegak**2)
+                    * (
+                        self.qnm[:, 3 * j] ** 2
+                        + self.qnm[:, 3 * j + 1] ** 2
+                        + self.qnm[:, 3 * j + 2] ** 2
+                    )
+                ).sum()
 
-            F = np.zeros((P, 3 * self.natoms), float)
+                # overrides open path forces
+                fspringnm[:, 3 * j : 3 * (j + 1)] = (
+                    -self.beads.m3[:, 3 * j : 3 * (j + 1)]
+                    * self.o_omegak[:, np.newaxis] ** 2
+                    * qnm[:, 3 * j : 3 * (j + 1)]
+                )
 
-            for ind, l in enumerate(self.bosons):
-                for j in range(P):
-                    F[j, 3 * l : 3 * (l + 1)] = Evaluate_dVB(self, E_k_N, V, ind, j)
+            # correction for bosons
+            if len(self.bosons) > 0:
+                for j in self.bosons:
+                    vspring -= (
+                        self.beads.m[j]
+                        * self.omegak**2
+                        * (
+                            self.qnm[:, 3 * j] ** 2
+                            + self.qnm[:, 3 * j + 1] ** 2
+                            + self.qnm[:, 3 * j + 2] ** 2
+                        )
+                    ).sum()
 
-            return [V[-1], F]
+            vspring *= 0.5
+            fspring += self.transform.nm2b(fspringnm)
 
-    def get_fspring(self):
-        """
-        Returns the spring force. Required for numerical propagation in free_babstep().
-        For distinguishable particles, simply transform fnm to Cartesian coordinates.
-        For bosons, get the second element of vspring_and_fspring_B
-        For a mixture of both, calculate separately and combine.
-        """
+        if len(self.bosons) > 0:
+            vspring_b, fspring_b = self.exchange_potential.vspring_and_fspring
 
-        if len(self.bosons) == 0:
-            return self.transform.nm2b(dstrip(self.fspringnm))
-        elif len(self.bosons) is self.natoms:
-            return self.vspring_and_fspring_B[1]
-        else:
-            # raise("@NormalModes: Implementing mixtures of B and D")
-            f_distinguish = self.transform.nm2b(dstrip(self.fspringnm))
-            # zero force for bosons
-            for boson in self.bosons:
-                f_distinguish[:, 3 * boson : (3 * boson + 3)] = 0.0
+            vspring += vspring_b
+            # overwrites the spring forces for the bosonic particles
+            fspring.reshape((self.nbeads, self.natoms, 3))[
+                :, self.bosons, :
+            ] = fspring_b
 
-            return f_distinguish + self.vspring_and_fspring_B[1]
+        return vspring, fspring
 
     def free_babstep(self):
         """
         Numerical propagator in Cartesian coordinates.
         So the propagation is done through a velocity verlet step with a time step that is
         self.nmts smaller than the one for the physical forces.
         All beads of all atoms are propagated in one step.
@@ -762,96 +809,117 @@
             # Since the dynamics are done in Cartesian coordinates below (including all modes),
             # I need to revert centroid step done separately in qcstep
             self.qnm[0, :] -= (
                 dstrip(self.pnm)[0, :] / dstrip(self.beads.m3)[0] * self.dt
             )
 
             # Free ring polymer dynamics are done with smaller time step detlat = dt/nmts
-            dt = self.dt / dstrip(self.nmts)
+            dt = self.dt / self.nmts
 
-            for j in range(0, dstrip(self.nmts)):
+            for j in range(0, self.nmts):
                 self.beads.p += 0.5 * dt * self.fspring
                 self.beads.q += dt * self.beads.p / dstrip(self.beads.m3)
                 # The depend machinery will take care of automatically calculating
                 # the forces at the updated positions.
                 self.beads.p += 0.5 * dt * self.fspring
 
     def free_qstep(self):
-        # !BH!: Should we update the comment here that now the propagator is either exact, NM or numerical, Cartesian?
-        """Exact normal mode propagator for the free ring polymer.
+        """Position propagator for the free ring polymer.
 
-        Note that the propagator works in mass scaled coordinates, so that the
-        propagator matrix can be determined independently from the particular
-        atom masses, and so the same propagator will work for all the atoms in
-        the system. All the ring polymers are propagated at the same time by a
-        matrix multiplication.
+        The basic propagator is based on a normal mode transformation, and
+        works for closed and open paths. Note that the propagator works in mass
+        scaled coordinates, so that the propagator matrix can be determined
+        independently from the particular atom masses, and so the same propagator
+        will work for all the atoms in the system. All the ring polymers are
+        propagated at the same time by a matrix multiplication.
+        A special Cartesian propagator is used for bosonic exchange.
 
         Also note that the centroid coordinate is propagated in qcstep, so is
         not altered here.
         """
 
         if self.nbeads == 1:
             pass
 
         elif self.propagator == "bab":
             if len(self.open_paths) > 0:
-                raise (
-                    "@Normalmodes : Open path propagator not implemented for bosons. Feel free to implement it if you want to use it :) "
+                raise NotImplementedError(
+                    """@Normalmodes : Open path propagator not implemented for bosons. 
+                    Feel free to implement it if you want to use it :) """
                 )
 
             self.free_babstep()
 
         else:
             if len(self.bosons) > 0:
-                raise (
+                raise NotImplementedError(
                     "@Normalmodes : Bosonic forces not compatible right now with the exact or Cayley propagators."
                 )
 
-            pq = np.zeros((2, self.natoms * 3), float)
-            sm = dstrip(self.beads.sm3)
-            prop_pq = dstrip(self.prop_pq)
-            o_prop_pq = dstrip(self.o_prop_pq)
-            pnm = dstrip(self.pnm) / sm
-            qnm = dstrip(self.qnm) * sm
+            """
+            if len(self.open_paths) > 0:
+                # if there are open paths, make a copy to preserve the original values
+                pnm = pnm.copy()
+                qnm = qnm.copy()
 
-            for k in range(1, self.nbeads):
-                pq[0, :] = pnm[k]
-                pq[1, :] = qnm[k]
-                pq = np.dot(prop_pq[k], pq)
-                qnm[k] = pq[1, :]
-                pnm[k] = pq[0, :]
+            # uses the buffer to apply the propagator in one go
+            pq_buffer = self.pq_buffer
 
             for k in range(1, self.nbeads):
-                pq[0, :] = pnm[k]
-                pq[1, :] = qnm[k]
-                qnm[k] = pq[1, :]
-                pnm[k] = pq[0, :]
+                # goes in mass-scaled coordinates and then applies
+                pq_buffer[0] = pnm[k] / sm[k]
+                pq_buffer[1] = qnm[k] * sm[k]
+                pnm[k], qnm[k] = noddot(prop_pq[k], pq_buffer)                
+            res1 = dstrip(self.pnm[1:]) * self.prop_pq_ms[0,0,1:] + dstrip(self.qnm[1:]) * self.prop_pq_ms[0,1,1:]
+            res2 = dstrip(self.pnm[1:]) * self.prop_pq_ms[1,0,1:] + dstrip(self.qnm[1:]) * self.prop_pq_ms[1,1,1:]
+            
+            print("check, ", np.linalg.norm( pnm[1:] * sm[1:] - res1), 
+            np.linalg.norm( qnm[1:] / sm[1:] - res2))
+            # back to non-scaled coordinates, and update the actual arrays
+            self.pnm[1:] = pnm[1:] * sm[1:]
+            self.qnm[1:] = qnm[1:] / sm[1:]
+
+            """
+
+            # detach arrays
+            pnm = dstrip(self.pnm)
+            qnm = dstrip(self.qnm)
+
+            prop_pq_ms = dstrip(self.prop_pq_ms)
+            new_pnm = pnm[1:] * prop_pq_ms[0, 0, 1:] + qnm[1:] * prop_pq_ms[0, 1, 1:]
+            new_qnm = pnm[1:] * prop_pq_ms[1, 0, 1:] + qnm[1:] * prop_pq_ms[1, 1, 1:]
 
             # now for open paths we recover the initial conditions (that have not yet been overwritten)
-            # and do open path propagation
-            pq = np.zeros(2)
-            for j in self.open_paths:
-                for a in range(3 * j, 3 * (j + 1)):
-                    for k in range(1, self.nbeads):
-                        pq[0] = self.pnm[k, a] / sm[k, a]
-                        pq[1] = self.qnm[k, a] * sm[k, a]
-                        pq = np.dot(o_prop_pq[k], pq)
-                        qnm[k, a] = pq[1]
-                        pnm[k, a] = pq[0]
-            self.pnm = pnm * sm
-            self.qnm = qnm / sm
-            # pq = np.zeros((2,self.natoms*3),float)
-            # sm = dstrip(self.beads.sm3)[0]
-            # prop_pq = dstrip(self.prop_pq)
-            # for k in range(1,self.nbeads):
-            #   pq[0,:] = dstrip(self.pnm)[k]/sm
-            #   pq[1,:] = dstrip(self.qnm)[k]*sm
-            #   pq = np.dot(prop_pq[k],pq)
-            #   self.qnm[k] = pq[1,:]/sm
-            #   self.pnm[k] = pq[0,:]*sm
+            # and do open path propagation. NB this will be slow, will probably need some optimization
+            # to run large calculations with this
+            if len(self.open_paths) > 0:
+                o_prop_pq_ms = dstrip(self.o_prop_pq_ms)
+                opc = self.open_paths_coords
+                new_pnm[:, opc] = (
+                    pnm[1:, opc] * o_prop_pq_ms[0, 0, 1:]
+                    + qnm[1:, opc] * o_prop_pq_ms[0, 1, 1:]
+                )
+                new_qnm[:, opc] = (
+                    pnm[1:, opc] * o_prop_pq_ms[1, 0, 1:]
+                    + qnm[1:, opc] * o_prop_pq_ms[1, 1, 1:]
+                )
+                """
+                pq = np.zeros(2)
+                for j in self.open_paths:
+                    for a in range(3 * j, 3 * (j + 1)):
+                        for k in range(1, self.nbeads):
+                            pq[0] = self.pnm[k, a] / sm[k, a]
+                            pq[1] = self.qnm[k, a] * sm[k, a]
+                            pq = np.dot(o_prop_pq[k], pq)
+                            new_pnm[k, a] = pq[0] * sm[k,a]
+                            new_qnm[k, a] = pq[1] / sm[k,a]
+                """
+            # updates the "real" vectors
+            self.pnm[1:] = new_pnm
+            self.qnm[1:] = new_qnm
 
     def get_kins(self):
         """Gets the MD kinetic energy for all the normal modes.
 
         Returns:
            A list of the kinetic energy for each NM.
 
@@ -899,7 +967,47 @@
                     # also takes care of the possibility of having non-RPMD masses
                     kmd[i, j] += (
                         np.dot(sp[i : 3 * self.natoms : 3], sp[j : 3 * self.natoms : 3])
                         / nmf[b]
                     )
 
         return kmd
+
+
+dproperties(
+    NormalModes,
+    [
+        "nmts",
+        "dt",
+        "mode",
+        "transform_method",
+        "propagator",
+        "nm_freqs",
+        "bosons",
+        "qnm",
+        "pnm",
+        "fnm",
+        "omegan",
+        "omegan2",
+        "omegak",
+        "omegak2",
+        "o_omegak",
+        "nm_factor",
+        "o_nm_factor",
+        "dynm3",
+        "dynomegak",
+        "prop_pq",
+        "prop_pq_ms",
+        "o_prop_pq",
+        "o_prop_pq_ms",
+        "kins",
+        "kin",
+        "kstress",
+        "exchange",
+        "vspring",
+        "vspring_and_fspring_bosons",
+        "vspring_and_fspring_distinguishables",
+        "vspring_and_fspring",
+        "fspring",
+        "fspringnm",
+    ],
+)
```

### Comparing `ipi-2.6.0/ipi/engine/outputs.py` & `ipi-2.6.3/ipi/engine/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 and the restart files.
 """
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
-
 import os
 
 import numpy as np
 
 from ipi.utils.messages import verbosity, info, warning
 from ipi.utils.units import unit_to_user
 from ipi.utils.softexit import softexit
@@ -39,15 +38,15 @@
     back to the initialization phase of the simulation"""
 
     def __init__(self, prefix, olist):
         super(OutputList, self).__init__(olist)
         self.prefix = prefix
 
 
-class OutputMaker(dobject):
+class OutputMaker:
     """Class to create floating outputs with an appropriate prefix"""
 
     def __init__(self, prefix="", f_start=False):
         self.prefix = prefix
         self.f_start = f_start
 
     def bind(self, system):
@@ -65,17 +64,18 @@
         rout.bind(mode)
         return rout
 
 
 class BaseOutput(object):
     """Base class for outputs. Deals with flushing upon close and little more"""
 
-    def __init__(self, filename="out"):
+    def __init__(self, filename="out", stride=1):
         """Initializes the class"""
 
+        self.stride = stride
         self.filename = filename
         self.out = None
 
     def softexit(self):
         """Emergency call when i-pi must exit quickly"""
 
         self.close_stream()
@@ -89,17 +89,18 @@
     def open_stream(self, mode="w"):
         """Opens the output stream"""
 
         # Only open a new file if this is a new run, otherwise append.
         self.mode = mode
         self.out = open_backup(self.filename, self.mode)
 
-    def bind(self, mode="w"):
+    def bind(self, mode="w", system=None):
         """Stores a reference to system and registers for exiting"""
 
+        self.system = system
         self.open_stream(mode)
         softexit.register_function(self.softexit)
 
     def force_flush(self):
         """Tries hard to flush the output stream"""
 
         if self.out is not None:
@@ -115,17 +116,21 @@
 
     def write(self, data):
         """Writes data to file"""
 
         if self.out is not None:
             return self.out.write(data)
 
+    def active(self):
+        """Whether we will output at this step"""
+
+        return (self.system.simul.step + 1) % self.stride == 0
 
-class PropertyOutput(BaseOutput):
 
+class PropertyOutput(BaseOutput):
     """Class dealing with outputting a set of properties to file.
 
     Does not do any calculation, just manages opening a file, getting data
     from a Properties object and outputting with the desired stride.
 
     Attributes:
        filename: The name of the file to output to.
@@ -148,43 +153,42 @@
            filename: A string giving the name of the file to be output to.
            stride: An integer giving how many steps should be taken between
               outputting the data to file.
            flush: Number of writes to file between flushing data.
            outlist: A list of all the properties that should be output.
         """
 
-        super(PropertyOutput, self).__init__(filename)
+        super(PropertyOutput, self).__init__(filename, stride)
 
         if outlist is None:
             outlist = np.zeros(0, np.dtype("|U1024"))
         self.outlist = np.asarray(outlist, np.dtype("|U1024"))
-        self.stride = stride
         self.flush = flush
         self.nout = 0
 
     def bind(self, system, mode="w"):
         """Binds output proxy to System object.
 
         Args:
            system: A System object to be bound.
         """
 
         # Checks as soon as possible if some asked-for properties are
         # missing or mispelled
-        self.system = system
+
         for what in self.outlist:
             key = getkey(what)
             if key not in list(system.properties.property_dict.keys()):
                 print(
                     "Computable properties list: ",
                     list(system.properties.property_dict.keys()),
                 )
                 raise KeyError(key + " is not a recognized property")
 
-        super(PropertyOutput, self).bind(mode)
+        super(PropertyOutput, self).bind(mode, system)
 
     def print_header(self):
         # print nice header if information is available on the properties
         icol = 1
         for what in self.outlist:
             ohead = "# "
             key = getkey(what)
@@ -215,15 +219,15 @@
            KeyError: Raised if one of the properties specified in the output list
               are not contained in the property_dict member of properties.
         """
 
         if softexit.triggered:
             return  # don't write if we are about to exit!
 
-        if not (self.system.simul.step + 1) % self.stride == 0:
+        if not self.active():
             return
         self.out.write("  ")
         for what in self.outlist:
             try:
                 quantity, dimension, unit = self.system.properties[what]
                 if dimension != "" and unit != "":
                     quantity = unit_to_user(dimension, unit, quantity)
@@ -240,15 +244,14 @@
         self.nout += 1
         if self.flush > 0 and self.nout >= self.flush:
             self.force_flush()
             self.nout = 0
 
 
 class TrajectoryOutput(BaseOutput):
-
     """Class dealing with outputting atom-based properties as a
     trajectory file.
 
     Does not do any calculation, just manages opening a file, getting data
     from a Trajectories object and outputting with the desired stride.
 
     Attributes:
@@ -290,17 +293,16 @@
            format: A string specifying the type of trajectory file to be created.
            cell_units: A string specifying the units that the cell parameters are
               given in.
            ibead: If positive, prints out only the selected bead. If negative, prints out one file per bead.
            extra_type: Specifies the type of extras string that is printed in the file
         """
 
-        self.filename = filename
+        super(TrajectoryOutput, self).__init__(filename, stride)
         self.what = what
-        self.stride = stride
         self.flush = flush
         self.ibead = ibead
         self.format = format
         self.cell_units = cell_units
         self.out = None
         self.nout = 0
         self.extra_type = extra_type
@@ -308,25 +310,24 @@
     def bind(self, system, mode="w"):
         """Binds output proxy to System object.
 
         Args:
            system: A System object to be bound.
         """
 
-        self.system = system
         # Checks as soon as possible if some asked-for trajs are missing or misspelled
         key = getkey(self.what)
-        if key not in list(self.system.trajs.traj_dict.keys()):
+        if key not in list(system.trajs.traj_dict.keys()):
             print(
                 "Computable trajectories list: ",
-                list(self.system.trajs.traj_dict.keys()),
+                list(system.trajs.traj_dict.keys()),
             )
             raise KeyError(key + " is not a recognized output trajectory")
 
-        super(TrajectoryOutput, self).bind(mode)
+        super(TrajectoryOutput, self).bind(mode, system)
 
     def print_header(self):
         """No headers for trajectory files"""
         pass
 
     def open_stream(self, mode):
         """Opens the output stream(s)."""
@@ -371,29 +372,30 @@
 
     def close_stream(self):
         """Closes the output stream."""
 
         try:
             if hasattr(self.out, "__getitem__"):
                 for o in self.out:
-                    o.close()
+                    if o is not None:
+                        o.close()
             else:
                 self.out.close()
         except AttributeError:
             # This gets called on softexit. We want to carry on to shut down as cleanly as possible
             warning(
                 "Exception while closing output stream " + str(self.out), verbosity.low
             )
 
     def write(self):
         """Writes out the required trajectories."""
 
         if softexit.triggered:
             return  # don't write if we are about to exit!
-        if not (self.system.simul.step + 1) % self.stride == 0:
+        if not self.active():
             return
 
         doflush = False
         self.nout += 1
         if self.flush > 0 and self.nout >= self.flush:
             doflush = True
             self.nout = 0
@@ -499,14 +501,16 @@
                     else:
                         raise ValueError(
                             "No specialized writer for arrays of dimension > 2"
                         )
                 except:
                     stream.write("%s" % data[self.extra_type][b])
                 stream.write("\n")
+            elif self.extra_type == "raw":
+                stream.write(str(data))
             else:
                 raise KeyError(
                     "Extra type '"
                     + self.extra_type
                     + "' is not among the quantities returned by any of the forcefields."
                 )
             if flush:
@@ -547,16 +551,15 @@
             cell_units=cell_units,
         )
         if flush:
             stream.flush()
             os.fsync(stream)
 
 
-class CheckpointOutput(dobject):
-
+class CheckpointOutput:
     """Class dealing with outputting checkpoints.
 
     Saves the complete status of the simulation at regular intervals.
 
     Attributes:
        filename: The (base) name of the file to output to.
        step: the number of times a checkpoint has been written out.
@@ -579,16 +582,16 @@
            overwrite: If True, the checkpoint file is overwritten at each output.
               If False, will output to 'filename_step'. Note that no check is done
               on whether 'filename_step' exists already.
            step: The number of checkpoint files that have been created so far.
         """
 
         self.filename = filename
-        self.step = depend_value(name="step", value=step)
         self.stride = stride
+        self._step = depend_value(name="step", value=step)
         self.overwrite = overwrite
         self._storing = False
         self._continued = False
 
     def bind(self, simul):
         """Binds output proxy to simulation object.
 
@@ -598,14 +601,19 @@
 
         self.simul = simul
         import ipi.inputs.simulation as isimulation
 
         self.status = isimulation.InputSimulation()
         self.status.store(simul)
 
+    def active(self):
+        """Whether we will output at this step"""
+
+        return (self.simul.step + 1) % self.stride == 0
+
     def store(self):
         """Stores the current simulation status.
 
         Used so that, if halfway through a step a kill signal is received,
         we can output a checkpoint file corresponding to the beginning of the
         current step, which is the last time that both the velocities and
         positions would have been consistent.
@@ -635,15 +643,15 @@
         if self._storing:
             info(
                 "@ CHECKPOINT: Write called while storing. Force re-storing",
                 verbosity.low,
             )
             self.store()
 
-        if not (self.simul.step + 1) % self.stride == 0:
+        if not self.active():
             return
 
         # function to use to open files
         open_function = open_backup
 
         if self.overwrite:
             filename = self.filename
@@ -659,7 +667,10 @@
             self.status.step.store(self.simul.step + 1)
 
         with open_function(filename, "w") as check_file:
             check_file.write(self.status.write(name="simulation"))
 
         # Do not use backed up file open on subsequent writes.
         self._continued = True
+
+
+dproperties(CheckpointOutput, ["step"])
```

### Comparing `ipi-2.6.0/ipi/engine/properties.py` & `ipi-2.6.3/ipi/engine/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,20 @@
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 
 import numpy as np
 
 from ipi.utils.messages import verbosity, info, warning
-from ipi.utils.depend import *
+from ipi.utils.depend import dstrip
 from ipi.utils.units import Constants, unit_to_internal
 from ipi.utils.mathtools import logsumlog, h2abc_deg
 from ipi.utils.io.inputs import io_xml
-from ipi.engine.atoms import *
-from ipi.engine.cell import *
-from ipi.engine.ensembles import *
-from ipi.engine.forces import *
 
-
-__all__ = ["Properties", "Trajectories", "getkey", "getall", "help_latex"]
+__all__ = ["Properties", "Trajectories", "getkey", "getall", "help_latex", "help_rst"]
 
 
 def getkey(pstring):
     """Strips units and argument lists from a property/trajectory keyword.
 
     Args:
        pstring: The string input by the user that specifies an output,
@@ -196,16 +191,15 @@
 
         if len(xstr) > 0:
             rstr += f"\n\n*{xstr.strip()}*"
         rstr += "\n\n"
     return rstr
 
 
-class Properties(dobject):
-
+class Properties:
     """A proxy to compute and output properties of the system.
 
     Takes the fundamental properties calculated during the simulation, and
     prepares them for output. It also contains simple algorithms to calculate
     other properties not calculated during the simulation itself, so that
     these can also be output.
 
@@ -332,17 +326,19 @@
             #                       "func": (lambda: self.ensemble.bias/(Constants.kb*self.ensemble.temp)) },
             "potential": {
                 "dimension": "energy",
                 "help": "The physical system potential energy.",
                 "longhelp": """The physical system potential energy. With the optional argument 'bead'
                          will print the potential associated with the specified bead.""",
                 "func": (
-                    lambda bead="-1": self.forces.pot / self.beads.nbeads
-                    if int(bead) < 0
-                    else self.forces.pots[int(bead)]
+                    lambda bead="-1": (
+                        self.forces.pot / self.beads.nbeads
+                        if int(bead) < 0
+                        else self.forces.pots[int(bead)]
+                    )
                 ),
             },
             "bead_potentials": {
                 "dimension": "energy",
                 "help": "The physical system potential energy of each bead.",
                 "size": "nbeads",
                 "func": (lambda: self.forces.pots),
@@ -363,48 +359,49 @@
                 "dimension": "energy",
                 "help": "The contribution to the system potential from one of the force components. ",
                 "longhelp": """The contribution to the system potential from one of the force components.
                        Takes one mandatory argument index (zero-based) that indicates which component of the
                        potential must be returned. The optional argument 'bead' will print the potential associated
                        with the specified bead. If the potential is weighed, the weight will be applied. """,
                 "func": (
-                    lambda index, bead="-1": self.forces.pots_component(
-                        int(index)
-                    ).sum()
-                    / self.beads.nbeads
-                    if int(bead) < 0
-                    else self.forces.pots_component(int(index))[int(bead)]
+                    lambda index, bead="-1": (
+                        self.forces.pots_component(int(index)).sum() / self.beads.nbeads
+                        if int(bead) < 0
+                        else self.forces.pots_component(int(index))[int(bead)]
+                    )
                 ),
             },
             "pot_component_raw": {
                 "dimension": "energy",
                 "help": "The contribution to the system potential from one of the force components. ",
                 "longhelp": """The contribution to the system potential from one of the
                        force components. Takes one mandatory argument index (zero-based) that indicates
                        which component of the potential must be returned. The optional argument 'bead'
                        will print the potential associated with the specified bead. Potential weights
                        will not be applied. """,
                 "func": (
-                    lambda index, bead="-1": self.forces.pots_component(
-                        int(index), False
-                    ).sum()
-                    / self.beads.nbeads
-                    if int(bead) < 0
-                    else self.forces.pots_component(int(index), False)[int(bead)]
+                    lambda index, bead="-1": (
+                        self.forces.pots_component(int(index), False).sum()
+                        / self.beads.nbeads
+                        if int(bead) < 0
+                        else self.forces.pots_component(int(index), False)[int(bead)]
+                    )
                 ),
             },
             "forcemod": {
                 "dimension": "force",
                 "help": "The modulus of the force.",
                 "longhelp": """The modulus of the force. With the optional argument 'bead'
                        will print the force associated with the specified bead.""",
                 "func": (
-                    lambda bead="-1": np.linalg.norm(self.forces.f) / self.beads.nbeads
-                    if int(bead) < 0
-                    else np.linalg.norm(self.forces.f[int(bead)])
+                    lambda bead="-1": (
+                        np.linalg.norm(self.forces.f) / self.beads.nbeads
+                        if int(bead) < 0
+                        else np.linalg.norm(self.forces.f[int(bead)])
+                    )
                 ),
             },
             "spring": {
                 "dimension": "energy",
                 "help": "The total spring potential energy between the beads of all the ring polymers in the system.",
                 "func": (lambda: self.nm.vspring / self.beads.nbeads),
             },
@@ -863,14 +860,43 @@
                           fourth-order direct estimator. Takes two arguments, 'alpha' , which gives the scaled
                           mass parameter and default to '1.0', and 'atom', which is the label or index of a type
                           of atoms. The 5 numbers output are 1) the average over the excess potential energy for
                           an isotope atom substitution <sc>, 2) the average of the squares of the excess potential
                           energy <sc**2>, and 3) the average of the exponential of excess potential energy
                           <exp(-beta*sc)>, and 4-5) Suzuki-Chin and Takahashi-Imada 4th-order reweighing term""",
             },
+            "exchange_distinct_prob": {
+                "dimension": "undefined",
+                "size": 1,
+                "func": self.get_exchange_distinct_prob,
+                "help": "Probability of the distinguishable ring polymer configuration.",
+                "longhelp": """Probability of the distinguishable ring polymer configuration, 
+                               where each atom has its own separate ring polymer. 
+                               A number between 0 and 1, tends to 1 in high temperatures, which indicates that 
+                               bosonic exchange is negligible""",
+            },
+            "exchange_all_prob": {
+                "dimension": "undefined",
+                "size": 1,
+                "func": self.get_exchange_longest_prob,
+                "help": "Probability of the bosonic ring polymer configuration where all atoms are connected.",
+                "longhelp": """Probability of the ring polymer exchange configuration where all atoms are connected.
+                               It is divided by 1/N, so the number is between 0 and N,
+                               while the asymptotic value at low temperatures is 1.""",
+            },
+            "fermionic_sign": {
+                "dimension": "undefined",
+                "size": 1,
+                "func": self.get_fermionic_sign,
+                "help": "Estimator for the fermionic sign, also used for reweighting fermionic observables.",
+                "longhelp": """Estimator for the fermionic sign, also used for reweighting fermionic observables.
+                               Decreases exponentially with beta and the number of particles, but if not too large,
+                               can be used to recover fermionic statistics from bosonic simulations,
+                               see doi:10.1063/5.0008720.""",
+            },
         }
 
     def bind(self, system):
         """Binds the necessary objects from the system to calculate the
         required properties.
 
         Args:
@@ -1066,14 +1092,22 @@
                     % iatom
                 )
         except ValueError:
             # here 'atom' is a label rather than an index which is stored in latom
             iatom = -1
             latom = atom
 
+        bosons_included = self._atom_property_distinguishability_well_defined(
+            iatom, latom
+        )
+        if bosons_included:
+            raise IndexError(
+                "Quantum centroid virial kinetic energy estimator not applicable to bosons"
+            )
+
         f = dstrip(self.forces.f)
         # subtracts centroid
         q = dstrip(self.beads.q).copy()
         qc = dstrip(self.beads.qc)
         for b in range(self.beads.nbeads):
             q[b] -= qc
 
@@ -1101,14 +1135,15 @@
         # ~ kcv += q[b,k]* f[b,k] + q[b,k+1]* f[b,k+1] + q[b,k+2]* f[b,k+2]
         # ~ kcv *= -0.5/self.beads.nbeads
         # ~ kcv += 1.5*Constants.kb*self.ensemble.temp
         # ~ acv += kcv
         # ~ ncount += 1
 
         if ncount == 0:
+            # TODO: don't warn if bosons are matched
             warning(
                 "Couldn't find an atom which matched the argument of kinetic energy, setting to zero.",
                 verbosity.medium,
             )
 
         return acv
 
@@ -1266,15 +1301,15 @@
                 "Couldn't find an atom which matched the argument of kinetic energy, setting to zero.",
                 verbosity.medium,
             )
 
         return acv
 
     def get_kintd(self, atom=""):
-        """Calculates the quantum centroid virial kinetic energy estimator.
+        """Calculates the quantum primitive kinetic energy estimator.
 
         Args:
            atom: If given, specifies the atom to give the kinetic energy
               for. If not, the system kinetic energy is given.
         """
 
         try:
@@ -1287,48 +1322,99 @@
                     % iatom
                 )
         except ValueError:
             # here 'atom' is a label rather than an index which is stored in latom
             iatom = -1
             latom = atom
 
+        bosons_included = self._atom_property_distinguishability_well_defined(
+            iatom, latom
+        )
+
+        res, ncount = self._kinetic_td_distinguishables(
+            atom, iatom, latom, skip_atom_indices=set(self.nm.bosons)
+        )
+        if bosons_included:
+            res += self.nm.exchange_potential.kinetic_td
+            ncount += len(bosons_included)
+
+        if ncount == 0:
+            warning(
+                "Couldn't find an atom which matched the argument of kinetic energy, setting to zero.",
+                verbosity.medium,
+            )
+
+        return res
+
+    def _atom_property_distinguishability_well_defined(self, iatom, latom):
+        """
+        Should not ask for a property of a subset of atoms some of which are indistinguishables
+        without including *all* the indistinguishable atoms.
+        Returns the bosons included in the property.
+        """
+        atoms_included = set(range(self.beads.natoms))
+        if iatom != -1:
+            atoms_included = set([iatom])
+        elif latom != "":
+            atoms_included = set(
+                filter(lambda i: latom == self.beads.names[i], range(self.beads.natoms))
+            )
+        bosons = set(self.nm.bosons)
+        bosons_included = bosons & atoms_included
+        if bosons_included and not (bosons <= atoms_included):
+            raise IndexError(
+                "Cannot output property of a proper subset of the bosons: "
+                "bosons %s are included, but %s are missing"
+                % (bosons_included, bosons - bosons_included)
+            )
+        return bosons_included
+
+    def _kinetic_td_distinguishables(self, atom, iatom, latom, skip_atom_indices=None):
+        """
+        The total kinetic energy via the primitive estimator for distinguishable particles.
+
+        Args:
+           atom: If given, specifies the atom to give the kinetic energy
+              for. If not, the system kinetic energy is given.
+           iatom: Index of the atom specified (or -1)
+           latom: Label of the atom specified (or "")
+           skip_atom_indices:
+                atoms not to be considered in the distinguishable estimator (e.g. bosons)
+        """
         q = dstrip(self.beads.q)
         m = dstrip(self.beads.m)
         PkT32 = 1.5 * Constants.kb * self.ensemble.temp * self.beads.nbeads
 
         atd = 0.0
         ncount = 0
         for i in range(self.beads.natoms):
             if atom != "" and iatom != i and latom != self.beads.names[i]:
                 continue
 
+            if i in skip_atom_indices:
+                continue
+
             ktd = 0.0
             for b in range(1, self.beads.nbeads):
                 for j in range(3 * i, 3 * (i + 1)):
                     ktd += (q[b, j] - q[b - 1, j]) ** 2
             for j in range(3 * i, 3 * (i + 1)):
                 ktd += (q[self.beads.nbeads - 1, j] - q[0, j]) ** 2
 
             ktd *= -0.5 * m[i] * self.nm.omegan2 / self.beads.nbeads
             ktd += PkT32
             atd += ktd
             ncount += 1
 
-        if ncount == 0:
-            warning(
-                "Couldn't find an atom which matched the argument of kinetic energy, setting to zero.",
-                verbosity.medium,
-            )
-
-        return atd
+        return atd, ncount
 
     def get_sckinpr(self):
         """Calculates the quantum centroid virial kinetic energy estimator."""
 
-        spring = self.beads.vpath * self.nm.omegan2 / self.beads.nbeads
+        spring = self.nm.vspring / self.beads.nbeads
         PkT32 = (
             1.5
             * Constants.kb
             * self.ensemble.temp
             * self.beads.nbeads
             * self.beads.natoms
         )
@@ -2614,17 +2700,31 @@
             warning(
                 "Couldn't find an atom which matched the argument of TI potential, setting to zero.",
                 verbosity.medium,
             )
 
         return ti
 
+    def get_exchange_distinct_prob(self):
+        if self.nm.exchange_potential is None:
+            raise Exception("No bosons found for exchange_distinct_prob")
+        return self.nm.exchange_potential.distinct_probability
+
+    def get_exchange_longest_prob(self):
+        if self.nm.exchange_potential is None:
+            raise Exception("No bosons found for exchange_all_prob")
+        return self.nm.exchange_potential.longest_probability
+
+    def get_fermionic_sign(self):
+        if self.nm.exchange_potential is None:
+            raise Exception("No bosons found for fermionic_sign")
+        return self.nm.exchange_potential.fermionic_sign
 
-class Trajectories(dobject):
 
+class Trajectories:
     """A simple class to take care of output of trajectory data.
 
     Attributes:
        system: The system object from which the position data will be
           obtained.
        fatom: A dummy beads object used so that individual replica trajectories
           can be output.
```

### Comparing `ipi-2.6.0/ipi/engine/simulation.py` & `ipi-2.6.3/ipi/engine/simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 import tracemalloc
 import os
-import threading
 import time
 from copy import deepcopy
 
-from ipi.utils.depend import depend_value, dobject, dd, dpipe
+from ipi.utils.depend import depend_value, dpipe, dproperties
 from ipi.utils.io.inputs.io_xml import xml_parse_file
 from ipi.utils.messages import verbosity, info, warning, banner
 from ipi.utils.softexit import softexit
 import ipi.engine.outputs as eoutputs
 import ipi.inputs.simulation as isimulation
 
+from concurrent.futures import ThreadPoolExecutor
 
 __all__ = ["Simulation"]
 
 
-class Simulation(dobject):
+class Simulation:
     """Main simulation object.
 
     Contains all the references and the main dynamics loop. Also handles the
     initialisation and output.
 
     Attributes:
         prng: A random number generator object.
@@ -117,14 +117,15 @@
         outputs,
         prng,
         smotion=None,
         step=0,
         tsteps=1000,
         ttime=0,
         threads=False,
+        safe_stride=1,
     ):
         """Initialises Simulation class.
 
         Args:
             mode: What kind of simulation is this
             syslist: A list of system objects
             fflist: A list of forcefield objects
@@ -139,15 +140,15 @@
                 cumulative total.
         """
 
         info(" # Initializing simulation object ", verbosity.low)
         self.prng = prng
         self.mode = mode
         self.threading = threads
-        dself = dd(self)
+        self.safe_stride = safe_stride
 
         self.syslist = syslist
         for s in syslist:
             s.prng = self.prng  # bind the system's prng to self prng
             s.init.init_stage1(s)
 
         # TODO - does this have any meaning now that we introduce the smotion class?
@@ -160,15 +161,15 @@
 
         self.fflist = {}
         for f in fflist:
             self.fflist[f.name] = f
 
         self.outtemplate = outputs
 
-        dself.step = depend_value(name="step", value=step)
+        self._step = depend_value(name="step", value=step)
         self.tsteps = tsteps
         self.ttime = ttime
         self.smotion = smotion
 
         self.chk = None
         self.rollback = True
 
@@ -215,29 +216,34 @@
             if self.outtemplate.prefix != "":
                 dco.filename = self.outtemplate.prefix + "." + o.filename
             if (
                 type(dco) is eoutputs.CheckpointOutput
             ):  # checkpoints are output per simulation
                 dco.bind(self)
                 dpipe(
-                    dd(dco).step, dd(o).step
+                    dco._step, o._step
                 )  # makes sure that the checkpoint step is updated also in the template
                 self.outputs.append(dco)
             else:  # properties and trajectories are output per system
                 isys = 0
                 for s in self.syslist:  # create multiple copies
                     no = deepcopy(dco)
                     if s.prefix != "":
                         no.filename = s.prefix + "_" + no.filename
                     no.bind(s, mode)
                     self.outputs.append(no)
                     if f_start:  # starting of simulation, print headers (if any)
                         no.print_header()
                     isys += 1
 
+        if self.threading:
+            self.executor = ThreadPoolExecutor(
+                max_workers=max(len(self.syslist), len(self.outputs))
+            )
+
         self.chk = eoutputs.CheckpointOutput("RESTART", 1, True, 0)
         self.chk.bind(self)
 
         if self.smotion is not None:
             self.smotion.bind(self.syslist, self.prng, self.output_maker)
 
     def softexit(self):
@@ -274,27 +280,22 @@
         # prints inital configuration -- only if we are not restarting
         if self.step == 0:
             self.step = -1
             # must use multi-threading to avoid blocking in multi-system runs with WTE
             if self.threading:
                 stepthreads = []
                 for o in self.outputs:
-                    st = threading.Thread(target=o.write, name=o.filename)
-                    st.daemon = True
-                    st.start()
+                    st = self.executor.submit(o.write)
                     stepthreads.append(st)
 
                 for st in stepthreads:
-                    while st.is_alive():
-                        # This is necessary as join() without timeout prevents main from receiving signals.
-                        st.join(2.0)
+                    st.result()
             else:
                 for o in self.outputs:
-                    o.write()  # threaded output seems to cause random hang-ups. should make things properly thread-safe
-
+                    o.write()
             self.step = 0
 
         steptime = 0.0
         simtime = time.time()
 
         cstep = 0
         # tptime = 0.0
@@ -307,34 +308,28 @@
             # this is a bit time-consuming but makes sure that we can honor soft
             # exit requests without screwing the trajectory
 
             steptime = -time.time()
             if softexit.triggered:
                 break
 
-            self.chk.store()
+            # save a consistent state of the simulation that will be saved as a RESTART file in case of premature (soft) exit
+            if self.step % self.safe_stride == 0:
+                self.chk.store()
 
-            if self.threading:
+            if len(self.syslist) > 0 and self.threading:
                 stepthreads = []
                 # steps through all the systems
                 for s in self.syslist:
                     # creates separate threads for the different systems
-                    st = threading.Thread(
-                        target=s.motion.step, name=s.prefix, kwargs={"step": self.step}
-                    )
-                    st.daemon = True
+                    st = self.executor.submit(s.motion.step, step=self.step)
                     stepthreads.append(st)
 
                 for st in stepthreads:
-                    st.start()
-
-                for st in stepthreads:
-                    while st.is_alive():
-                        # This is necessary as join() without timeout prevents main from receiving signals.
-                        st.join(2.0)
+                    st.result()
             else:
                 for s in self.syslist:
                     s.motion.step(step=self.step)
 
             if softexit.triggered:
                 # Don't continue if we are about to exit.
                 break
@@ -346,23 +341,20 @@
             if softexit.triggered:
                 # Don't write if we are about to exit.
                 break
 
             if self.threading:
                 stepthreads = []
                 for o in self.outputs:
-                    st = threading.Thread(target=o.write, name=o.filename)
-                    st.daemon = True
-                    st.start()
-                    stepthreads.append(st)
+                    if o.active():  # don't start a thread if it's not needed
+                        st = self.executor.submit(o.write)
+                        stepthreads.append(st)
 
                 for st in stepthreads:
-                    while st.is_alive():
-                        # This is necessary as join() without timeout prevents main from receiving signals.
-                        st.join(2.0)
+                    st.result()
             else:
                 for o in self.outputs:
                     o.write()
 
             steptime += time.time()
             ttot += steptime
             cstep += 1
@@ -396,7 +388,10 @@
                 break
 
             if (self.ttime > 0) and (time.time() - simtime > self.ttime):
                 info(" # Wall clock time expired! Bye bye!", verbosity.low)
                 break
 
         self.rollback = False
+
+
+dproperties(Simulation, ["step"])
```

### Comparing `ipi-2.6.0/ipi/engine/smotion/dmd.py` & `ipi-2.6.3/ipi/engine/smotion/dmd.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/engine/smotion/metad.py` & `ipi-2.6.3/ipi/engine/smotion/metad.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2016 i-PI developers
 # See the "licenses" directory for full license information.
 
 from ipi.engine.smotion import Smotion
-from ipi.utils.depend import *
 
 
 __all__ = ["MetaDyn"]
 
 
 class MetaDyn(Smotion):
     """Metadynamics routine based on a FFPlumed forcefield.
@@ -86,12 +85,12 @@
 
                 fmtd = f.mtd_update(pos=s.beads.qc, cell=s.cell.h)
                 if fmtd:  # if metadyn has updated, then we must recompute forces.
                     # hacky but cannot think of a better way: we must manually taint *just* that component
                     for fc in s.ensemble.bias.mforces:
                         if fc.ffield == k:
                             for fb in fc._forces:
-                                dd(fb).ufvx.taint()
+                                fb._ufvx.taint()
                     meta_pot_after = s.ensemble.bias.pot
                     # updates the conserved quantity with the change in bias so that
                     # we remove the shift due to added hills
                     s.ensemble.eens += meta_pot_before - meta_pot_after
```

### Comparing `ipi-2.6.0/ipi/engine/smotion/multi.py` & `ipi-2.6.3/ipi/engine/smotion/multi.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/engine/smotion/remd.py` & `ipi-2.6.3/ipi/engine/smotion/remd.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
                 pxc = np.exp((newpensi + newpensj) - (pensi + pensj))
                 t_eval += time.time()
 
                 if pxc > self.prng.u:  # really does the exchange
                     info(
                         " @ PT:  SWAPPING replicas % 5d and % 5d." % (i, j),
-                        verbosity.low,
+                        verbosity.high,
                     )
 
                     # if we have GLE thermostats, we also have to exchange rescale the s!!!
                     gle_scale(sl[i], (tj / ti))
                     gle_scale(sl[j], (ti / tj))
 
                     t_eval -= time.time()
@@ -201,15 +201,15 @@
                     except AttributeError:
                         pass
 
                     t_swap += time.time()
                     info(
                         " @ PT:  SWAP REJECTED BETWEEN replicas % 5d and % 5d."
                         % (i, j),
-                        verbosity.low,
+                        verbosity.high,
                     )
 
                 # tempi = copy(self.syslist[i].ensemble.temp)
 
                 # self.syslist[i].ensemble.temp = copy(self.syslist[j].ensemble.temp)
                 # velocities have to be adjusted according to the new temperature
```

### Comparing `ipi-2.6.0/ipi/engine/smotion/smotion.py` & `ipi-2.6.3/ipi/engine/smotion/smotion.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 """
 
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
-from ipi.utils.depend import dobject
 
-
-class Smotion(dobject):
+class Smotion:
     """Base smootion calculation class.
 
     Gives the standard methods and attributes needed in all the
     smootion calculation classes.
 
     Attributes:
         dummy: A dummy object giving dummy information.
```

### Comparing `ipi-2.6.0/ipi/engine/system.py` & `ipi-2.6.3/ipi/engine/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,24 @@
 # This file is part of i-PI.
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 
 import threading
 
-from ipi.utils.depend import *
-from ipi.utils.units import *
-from ipi.utils.prng import *
-from ipi.utils.io import *
-from ipi.utils.io.inputs.io_xml import *
+from ipi.utils.depend import dpipe
 from ipi.utils.messages import verbosity, info
-from ipi.engine.atoms import *
-from ipi.engine.cell import *
 from ipi.engine.forces import Forces
 from ipi.engine.properties import Properties, Trajectories
 
 
 __all__ = ["System"]
 
 
-class System(dobject):
-
+class System:
     """Physical system object.
 
     Contains all the physical information. Also handles stepping and output.
 
     Attributes:
        beads: A beads object giving the atom positions.
        cell: A cell object giving the system box.
@@ -113,15 +106,15 @@
             self.nm,
             self.cell,
             self.forces,
             self.prng,
             simul.output_maker,
         )
 
-        dpipe(dd(self.nm).omegan2, dd(self.forces).omegan2)
+        dpipe(self.nm._omegan2, self.forces._omegan2)
 
         self.init.init_stage2(self)
 
         # binds output management objects
         self._propertylock = threading.Lock()
         self.properties.bind(self)
         self.trajs.bind(self)
```

### Comparing `ipi-2.6.0/ipi/engine/thermostats.py` & `ipi-2.6.3/ipi/engine/thermostats.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     "ThermoNMGLE",
     "ThermoNMGLEG",
     "ThermoCL",
     "MultiThermo",
 ]
 
 
-class Thermostat(dobject):
-
+class Thermostat:
     """Base thermostat class.
 
     Gives the standard methods and attributes needed in all the thermostat
     classes.
 
     Attributes:
        prng: A pseudo random number generator object.
@@ -65,18 +64,17 @@
            temp: The simulation temperature. Defaults to 1.0.
            dt: The simulation time step. Defaults to 1.0.
            ethermo: The initial heat energy transferred to the bath.
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
         """
 
-        dself = dd(self)
-        dself.temp = depend_value(name="temp", value=temp)
-        dself.dt = depend_value(name="dt", value=dt)
-        dself.ethermo = depend_value(name="ethermo", value=ethermo)
+        self._temp = depend_value(name="temp", value=temp)
+        self._dt = depend_value(name="dt", value=dt)
+        self._ethermo = depend_value(name="ethermo", value=ethermo)
 
     def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
         """Binds the appropriate degrees of freedom to the thermostat.
 
         This takes an object with degrees of freedom, and makes their momentum
         and mass vectors members of the thermostat. It also then creates the
         objects that will hold the data needed in the thermostat algorithms
@@ -104,41 +102,40 @@
             warning(
                 "Initializing thermostat from standard random PRNG", verbosity.medium
             )
             self.prng = Random()
         else:
             self.prng = prng
 
-        dself = dd(self)
         if beads is not None:
-            dself.p = beads.p.flatten()
-            dself.m = beads.m3.flatten()
+            self._p = beads.p.flatten()
+            self._m = beads.m3.flatten()
         elif atoms is not None:
-            dself.p = dd(atoms).p
-            dself.m = dd(atoms).m3
+            self._p = atoms._p
+            self._m = atoms._m3
         elif pm is not None:
-            dself.p = pm[
+            self._p = pm[
                 0
             ].flatten()  # MR this should allow to simply pass the cell momenta in the anisotropic barostat
-            dself.m = pm[1].flatten()
+            self._m = pm[1].flatten()
         else:
             raise TypeError(
                 "Thermostat.bind expects either Beads, Atoms, NormalModes, or a (p,m) tuple to bind to"
             )
 
         if fixdof is None:
             self.ndof = len(self.p)
         else:
             self.ndof = float(len(self.p) - fixdof)
 
-        dself.sm = depend_array(
+        self._sm = depend_array(
             name="sm",
-            value=np.zeros(len(dself.m)),
+            value=np.zeros(len(self._m)),
             func=self.get_sm,
-            dependencies=[dself.m],
+            dependencies=[self._m],
         )
 
     def get_sm(self):
         """Retrieves the square root of the mass matrix.
 
         Returns:
            A vector of the square root of the mass matrix with one value for
@@ -149,16 +146,18 @@
 
     def step(self):
         """Dummy thermostat step."""
 
         pass
 
 
-class ThermoLangevin(Thermostat):
+dproperties(Thermostat, ["temp", "dt", "ethermo", "p", "m", "sm", "dt"])
+
 
+class ThermoLangevin(Thermostat):
     """Represents a langevin thermostat.
 
     Depend objects:
        tau: Thermostat damping time scale. Larger values give a less strongly
           coupled thermostat.
        T: Coefficient of the diffusive contribution of the thermostat, i.e. the
           drift back towards equilibrium. Depends on tau and the time step.
@@ -171,60 +170,77 @@
 
         return np.exp(-self.dt / self.tau)
 
     def get_S(self):
         """Calculates the coefficient of the white noise."""
         return np.sqrt(Constants.kb * self.temp * (1 - self.T**2))
 
+    def get_T_on_sm(self):
+        """Calculates the combined mass scaling and thermostat damping."""
+        return self.T / dstrip(self.sm)
+
     def __init__(self, temp=1.0, dt=1.0, tau=1.0, ethermo=0.0):
         """Initialises ThermoLangevin.
 
         Args:
            temp: The simulation temperature. Defaults to 1.0.
            dt: The simulation time step. Defaults to 1.0.
            tau: The thermostat damping timescale. Defaults to 1.0.
            ethermo: The initial heat energy transferred to the bath.
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
         """
 
         super(ThermoLangevin, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
 
-        dself.dt = depend_value(value=dt, name="dt")
-        dself.tau = depend_value(value=tau, name="tau")
-        dself.T = depend_value(
-            name="T", func=self.get_T, dependencies=[dself.tau, dself.dt]
+        self._tau = depend_value(value=tau, name="tau")
+        self._T = depend_value(
+            name="T", func=self.get_T, dependencies=[self._tau, self._dt]
         )
-        dself.S = depend_value(
-            name="S", func=self.get_S, dependencies=[dself.temp, dself.T]
+        self._S = depend_value(
+            name="S", func=self.get_S, dependencies=[self._temp, self._T]
         )
 
-    def step(self):
-        """Updates the bound momentum vector with a langevin thermostat."""
+    def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
+        """Binds the appropriate degrees of freedom to the thermostat."""
 
-        et = dstrip(self.ethermo)
-        p = dstrip(self.p).copy()
-        sm = dstrip(self.sm)
+        super(ThermoLangevin, self).bind(beads, atoms, pm, nm, prng, fixdof)
 
-        p /= sm
+        self._T_on_sm = depend_value(
+            name="T_on_sm", func=self.get_T_on_sm, dependencies=[self._T, self._sm]
+        )
 
-        et += np.dot(p, p) * 0.5
-        p *= self.T
-        p += self.S * self.prng.gvec(len(p))
-        et -= np.dot(p, p) * 0.5
+    def step(self):
+        """Updates the bound momentum vector with a langevin thermostat."""
 
-        p *= sm
+        # This performs the following steps
+        # p <- p*exp(-dt/tau)+xi sqrt(C(1-exp-2dt/tau))
+        # where dt is the thermostat time step (half of the MD step)
+        # and C is the equilibrium fluctuations. to have a single
+        # coefficient (and facilitate computing the kinetic energy)
+        # the change in kinetic energy is computed to accumulate the work made
+        # by the thermostat
+
+        # goes in a single step to mass scaled coordinates and applies damping
+        p = dstrip(self.p) * dstrip(self.T_on_sm)
+
+        deltah = noddot(p, p) / (self.T**2)  # must correct for the "pre-damping"
+        p += self.S * self.prng.gvec(len(p))  # random part (in ms coordinates)
+        deltah -= noddot(p, p)  # new energy
+
+        self.p[:] = p * dstrip(
+            self.sm
+        )  # back to physical momentum and updates actual p
+        self.ethermo += deltah * 0.5
 
-        self.p = p
-        self.ethermo = et
 
+dproperties(ThermoLangevin, ["tau", "T", "S", "T_on_sm"])
 
-class ThermoPILE_L(Thermostat):
 
+class ThermoPILE_L(Thermostat):
     """Represents a PILE thermostat with a local centroid thermostat.
 
     Attributes:
        _thermos: The list of the different thermostats for all the ring polymer
           normal modes.
        nm: A normal modes object to attach the thermostat to.
        prng: Random number generator used in the stochastic integration
@@ -256,20 +272,19 @@
         Raises:
            TypeError: Raised if the thermostat is used with any object other than
               a beads object, so that we make sure that the objects needed for the
               normal mode transformation exist.
         """
 
         super(ThermoPILE_L, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
-        dself.tau = depend_value(value=tau, name="tau")
-        dself.pilescale = depend_value(value=scale, name="pilescale")
-        dself.pilect = depend_value(value=pilect, name="pilect")
-        dself.npilect = depend_value(
-            func=self.get_npilect, name="npilect", dependencies=[dself.pilect]
+        self._tau = depend_value(value=tau, name="tau")
+        self._pilescale = depend_value(value=scale, name="pilescale")
+        self._pilect = depend_value(value=pilect, name="pilect")
+        self._npilect = depend_value(
+            func=self.get_npilect, name="npilect", dependencies=[self._pilect]
         )
 
     def bind(
         self,
         beads=None,
         atoms=None,
         pm=None,
@@ -301,15 +316,14 @@
               applied to the system. Defaults to zero.
 
         Raises:
            TypeError: Raised if no appropriate degree of freedom or object
               containing a momentum vector is specified for
               the thermostat to couple to.
         """
-        dself = dd(self)
 
         if nm is None or not type(nm) is NormalModes:
             raise TypeError(
                 "ThermoPILE_L.bind expects a NormalModes argument to bind to"
             )
         if prng is None:
             self.prng = Random()
@@ -323,69 +337,67 @@
         # optionally does not bind the centroid, so we can re-use all of this
         # in the PILE_G case
         if not bindcentroid:
             self._thermos[0] = None
 
         self.nm = nm
 
-        dself.tauk = depend_array(
+        self._tauk = depend_array(
             name="tauk",
             value=np.zeros(nm.nbeads - 1, float),
             func=self.get_tauk,
-            dependencies=[dself.pilescale, dd(nm).dynomegak],
+            dependencies=[self._pilescale, nm._dynomegak],
         )
 
         # must pipe all the dependencies in such a way that values for the nm thermostats
         # are automatically updated based on the "master" thermostat
         def make_taugetter(k):
             return lambda: self.tauk[k - 1]
 
         it = 0
-        nm.pnm.hold()
         for t in self._thermos:
             if t is None:
                 it += 1
                 continue
             if it > 0:
                 fixdof = None  # only the centroid thermostat may have constraints
 
             # bind thermostat t to the it-th bead
 
             t.bind(pm=(nm.pnm[it, :], nm.dynm3[it, :]), prng=self.prng, fixdof=fixdof)
             if it == 0:
                 # the following lines pipe a different temperature to the centroid, if requested
                 if self.pilect > 0.0:
-                    dpipe(dself.pilect, dd(t).temp)
+                    dpipe(self._npilect, t._temp)
                 else:
-                    dpipe(dself.temp, dd(t).temp)
+                    dpipe(self._temp, t._temp)
             else:
                 # pipes temp
-                dpipe(dself.temp, dd(t).temp)
+                dpipe(self._temp, t._temp)
             # pipes dt
-            dpipe(dself.dt, dd(t).dt)
+            dpipe(self._dt, t._dt)
 
             # for tau it is slightly more complex
             if it == 0:
-                dpipe(dself.tau, dd(t).tau)
+                dpipe(self._tau, t._tau)
             else:
                 # Here we manually connect _thermos[i].tau to tauk[i].
                 # Simple and clear.
-                dd(t).tau.add_dependency(dself.tauk)
-                dd(t).tau._func = make_taugetter(it)
-            dself.ethermo.add_dependency(dd(t).ethermo)
-            dself.ethermo.hold()  # will manually update ethermo when needed!
+                t._tau.add_dependency(self._tauk)
+                t._tau._func = make_taugetter(it)
+            self._ethermo.add_dependency(t._ethermo)
             it += 1
 
         # since the ethermo will be "delegated" to the normal modes thermostats,
         # one has to split
         # any previously-stored value between the sub-thermostats
         if bindcentroid:
             for t in self._thermos:
                 t.ethermo = prev_ethermo / nm.nbeads
-            dself.ethermo._func = self.get_ethermo
+            self._ethermo._func = self.get_ethermo
             # if we are not binding the centroid just yet, this bit of the piping
             # is delegated to the function which is actually calling this
 
     def get_tauk(self):
         """Computes the thermostat damping time scale for the non-centroid
         normal modes.
 
@@ -414,24 +426,23 @@
     def get_npilect(self):
         """Multiplies centroid temperature by nbeads"""
         return self.nm.nbeads * self.pilect
 
     def step(self):
         """Updates the bound momentum vector with a PILE thermostat."""
 
-        self.nm.pnm.hold()
         # super-cool! just loop over the thermostats! it's as easy as that!
         for t in self._thermos:
             t.step()
-        self.nm.pnm.resume()
-        dd(self).ethermo.resume()
 
 
-class ThermoSVR(Thermostat):
+dproperties(ThermoPILE_L, ["tau", "pilescale", "pilect", "npilect", "tauk"])
 
+
+class ThermoSVR(Thermostat):
     """Represents a stochastic velocity rescaling thermostat.
 
     Depend objects:
        tau: Centroid thermostat damping time scale. Larger values give a
           less strongly coupled centroid thermostat.
        K: Scaling factor for the total kinetic energy. Depends on the
           temperature.
@@ -456,21 +467,20 @@
            dt: The simulation time step. Defaults to 1.0.
            tau: The thermostat damping timescale. Defaults to 1.0.
            ethermo: The initial conserved energy quantity. Defaults to 0.0. Will
               be non-zero if the thermostat is initialised from a checkpoint file.
         """
 
         super(ThermoSVR, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
 
-        dself.tau = depend_value(value=tau, name="tau")
-        dself.et = depend_value(
-            name="et", func=self.get_et, dependencies=[dself.tau, dself.dt]
+        self._tau = depend_value(value=tau, name="tau")
+        self._et = depend_value(
+            name="et", func=self.get_et, dependencies=[self._tau, self._dt]
         )
-        dself.K = depend_value(name="K", func=self.get_K, dependencies=[dself.temp])
+        self._K = depend_value(name="K", func=self.get_K, dependencies=[self._temp])
 
     def step(self):
         """Updates the bound momentum vector with a stochastic velocity rescaling
         thermostat. See G Bussi, D Donadio, M Parrinello,
         Journal of Chemical Physics 126, 014101 (2007)
         """
 
@@ -496,16 +506,18 @@
         if (r1 + np.sqrt(2 * K / self.K * self.et / (1 - self.et))) < 0:
             alpha *= -1
 
         self.ethermo += K * (1 - alpha2)
         self.p *= alpha
 
 
-class ThermoPILE_G(ThermoPILE_L):
+dproperties(ThermoSVR, ["tau", "et", "K"])
 
+
+class ThermoPILE_G(ThermoPILE_L):
     """Represents a PILE thermostat with a global centroid thermostat.
 
     Simply replaces the Langevin thermostat for the centroid normal mode with
     a global velocity rescaling thermostat.
     """
 
     def __init__(self, temp=1.0, dt=1.0, tau=1.0, ethermo=0.0, scale=1.0, pilect=0.0):
@@ -520,19 +532,18 @@
            scale: A float used to reduce the intensity of the PILE thermostat if
               required.
            pilect: centroid mode temperature (if different from ensemble and set by input).
               Default of 0.0 means it is not used and all modes have equal temperatures.
         """
 
         super(ThermoPILE_G, self).__init__(temp, dt, tau, ethermo)
-        dself = dd(self)
-        dself.pilescale = depend_value(value=scale, name="pilescale")
-        dself.pilect = depend_value(value=pilect, name="pilect")
-        dself.npilect = depend_value(
-            func=self.get_npilect, name="npilect", dependencies=[dself.pilect]
+        self._pilescale = depend_value(value=scale, name="pilescale")
+        self._pilect = depend_value(value=pilect, name="pilect")
+        self._npilect = depend_value(
+            func=self.get_npilect, name="npilect", dependencies=[self._pilect]
         )
 
     def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
         """Binds the appropriate degrees of freedom to the thermostat.
 
         This takes a beads object with degrees of freedom, and makes its momentum
         and mass vectors members of the thermostat. It also then creates the
@@ -554,39 +565,37 @@
         """
 
         # first binds as a local PILE, then substitutes the thermostat on the centroid
         prev_ethermo = self.ethermo
         super(ThermoPILE_G, self).bind(
             nm=nm, prng=prng, bindcentroid=False, fixdof=fixdof
         )
-        dself = dd(self)
 
         # centroid thermostat
         self._thermos[0] = ThermoSVR(temp=1, dt=1, tau=1)
 
         t = self._thermos[0]
         t.bind(pm=(nm.pnm[0, :], nm.dynm3[0, :]), prng=self.prng, fixdof=fixdof)
         # the next lines pipe a different temperatures to the centroid modes, if requested.
         if self.pilect > 0.0:
-            dpipe(dself.pilect, dd(t).temp)
+            dpipe(self._npilect, t._temp)
         else:
-            dpipe(dself.temp, dd(t).temp)
+            dpipe(self._temp, t._temp)
 
-        dpipe(dself.dt, dd(t).dt)
-        dpipe(dself.tau, dd(t).tau)
-        dself.ethermo.add_dependency(dd(t).ethermo)
+        dpipe(self._dt, t._dt)
+        dpipe(self._tau, t._tau)
+        self._ethermo.add_dependency(t._ethermo)
 
         # splits any previous ethermo between the thermostats, and finishes to bind ethermo to the sum function
         for t in self._thermos:
             t.ethermo = prev_ethermo / nm.nbeads
-        dself.ethermo._func = self.get_ethermo
+        self._ethermo._func = self.get_ethermo
 
 
 class ThermoGLE(Thermostat):
-
     """Represents a generalized Langevin equation thermostat.
 
     This is similar to a langevin thermostat, in that it uses Gaussian random
     numbers to simulate a heat bath acting on the system, but simulates a
     non-Markovian system by using a Markovian formulation in an extended phase
     space. This allows for a much greater degree of flexibility, and this
     thermostat, properly fitted, can give an approximation to the correct
@@ -648,35 +657,34 @@
               total number of degrees of freedom in the system.
            ethermo: The initial heat energy transferred to the bath.
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
         """
 
         super(ThermoGLE, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
 
         if A is None:
             A = np.identity(1, float)
-        dself.A = depend_value(value=A.copy(), name="A")
+        self._A = depend_value(value=A.copy(), name="A")
 
         self.ns = len(self.A) - 1
 
         # now, this is tricky. if C is taken from temp, then we want it to be updated
         # as a depend of temp. Otherwise, we want it to be an independent beast.
         if C is None:
             C = np.identity(self.ns + 1, float) * self.temp
-            dself.C = depend_value(name="C", func=self.get_C, dependencies=[dself.temp])
+            self._C = depend_value(name="C", func=self.get_C, dependencies=[self._temp])
         else:
-            dself.C = depend_value(value=C.copy(), name="C")
+            self._C = depend_value(value=C.copy(), name="C")
 
-        dself.T = depend_value(
-            name="T", func=self.get_T, dependencies=[dself.A, dself.dt]
+        self._T = depend_value(
+            name="T", func=self.get_T, dependencies=[self._A, self._dt]
         )
-        dself.S = depend_value(
-            name="S", func=self.get_S, dependencies=[dself.C, dself.T]
+        self._S = depend_value(
+            name="S", func=self.get_S, dependencies=[self._C, self._T]
         )
 
         self.s = np.zeros(0)
 
     def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
         """Binds the appropriate degrees of freedom to the thermostat.
 
@@ -702,24 +710,23 @@
               containing a momentum vector is specified for
               the thermostat to couple to.
         """
 
         super(ThermoGLE, self).bind(
             beads=beads, atoms=atoms, pm=pm, prng=prng, fixdof=fixdof
         )
-        dself = dd(self)
 
         # allocates, initializes or restarts an array of s's
-        if self.s.shape != (self.ns + 1, len(dself.m)):
+        if self.s.shape != (self.ns + 1, len(self._m)):
             if len(self.s) > 0:
                 warning(
                     "Mismatch in GLE s array size on restart, will reinitialise to free particle.",
                     verbosity.low,
                 )
-            self.s = np.zeros((self.ns + 1, len(dself.m)))
+            self.s = np.zeros((self.ns + 1, len(self._m)))
 
             # Initializes the s vector in the free-particle limit
             info(
                 " GLE additional DOFs initialised to the free-particle limit.",
                 verbosity.low,
             )
             SC = stab_cholesky(self.C * Constants.kb)
@@ -737,16 +744,18 @@
             self.S, self.prng.gvec(self.s.shape)
         )
         self.ethermo -= np.dot(self.s[0], self.s[0]) * 0.5
 
         self.p = self.s[0] * self.sm
 
 
-class ThermoNMGLE(Thermostat):
+dproperties(ThermoGLE, ["A", "C", "T", "S"])
+
 
+class ThermoNMGLE(Thermostat):
     """Represents a 'normal-modes' generalized Langevin equation thermostat.
 
     An extension to the GLE thermostat which is applied in the
     normal modes representation, and which allows to use a different
     GLE for each normal mode
 
     Attributes:
@@ -786,30 +795,29 @@
               total number of degrees of freedom in the system.
            ethermo: The initial heat energy transferred to the bath.
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
         """
 
         super(ThermoNMGLE, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
 
         if A is None:
             A = np.identity(1, float)
-        dself.A = depend_value(value=A.copy(), name="A")
+        self._A = depend_value(value=A.copy(), name="A")
 
         self.nb = len(self.A)
         self.ns = len(self.A[0]) - 1
 
         # now, this is tricky. if C is taken from temp, then we want it to be
         # updated as a depend of temp.
         # Otherwise, we want it to be an independent beast.
         if C is None:
-            dself.C = depend_value(name="C", func=self.get_C, dependencies=[dself.temp])
+            self._C = depend_value(name="C", func=self.get_C, dependencies=[self._temp])
         else:
-            dself.C = depend_value(value=C.copy(), name="C")
+            self._C = depend_value(value=C.copy(), name="C")
 
     def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
         """Binds the appropriate degrees of freedom to the thermostat.
 
         This takes an object with degrees of freedom, and makes their momentum
         and mass vectors members of the thermostat. It also then creates the
         objects that will hold the data needed in the thermostat algorithms
@@ -825,15 +833,14 @@
               applied to the system. Defaults to zero.
 
         Raises:
            TypeError: Raised if no beads object is specified for
               the thermostat to couple to.
         """
 
-        dself = dd(self)
         if nm is None or not type(nm) is NormalModes:
             raise TypeError(
                 "ThermoNMGLE.bind expects a NormalModes argument to bind to"
             )
 
         if prng is None:
             self.prng = Random()
@@ -887,32 +894,32 @@
         for t in self._thermos:
             t.s = self.s[it]  # gets the s's as a slice of self.s
             t.bind(
                 pm=(nm.pnm[it, :], nm.dynm3[it, :]), prng=self.prng
             )  # bind thermostat t to the it-th normal mode
 
             # pipes temp and dt
-            dpipe(dself.temp, dd(t).temp)
-            dpipe(dself.dt, dd(t).dt)
+            dpipe(self._temp, t._temp)
+            dpipe(self._dt, t._dt)
 
             # here we pipe the A and C of individual NM to the "master" arrays
-            dd(t).A.add_dependency(dself.A)
-            dd(t).A._func = make_Agetter(it)
-            dd(t).C.add_dependency(dself.C)
-            dd(t).C._func = make_Cgetter(it)
-            dself.ethermo.add_dependency(dd(t).ethermo)
+            t._A.add_dependency(self._A)
+            t._A._func = make_Agetter(it)
+            t._C.add_dependency(self._C)
+            t._C._func = make_Cgetter(it)
+            self._ethermo.add_dependency(t._ethermo)
             it += 1
 
         # since the ethermo will be "delegated" to the normal modes thermostats,
         # one has to split
         # any previously-stored value between the sub-thermostats
         for t in self._thermos:
             t.ethermo = prev_ethermo / self.nb
 
-        dself.ethermo._func = self.get_ethermo
+        self._ethermo._func = self.get_ethermo
 
     def step(self):
         """Updates the thermostat in NM representation by looping over the
         individual DOFs.
         """
 
         for t in self._thermos:
@@ -925,30 +932,32 @@
 
         et = 0.0
         for t in self._thermos:
             et += t.ethermo
         return et
 
 
-class ThermoNMGLEG(ThermoNMGLE):
+dproperties(ThermoNMGLE, ["A", "C", "T", "S"])
+
 
+class ThermoNMGLEG(ThermoNMGLE):
     """Represents a 'normal-modes' generalized Langevin equation thermostat + SVR.
 
     An extension to the above NMGLE thermostat which also adds a stochastic
     velocity rescaling to the centroid. Allows kinetic energy as well as
     potential energy sampling optimization.
 
     Depend objects:
        tau: Thermostat damping time scale. Larger values give a less strongly
           coupled thermostat.
     """
 
     def __init__(self, temp=1.0, dt=1.0, A=None, C=None, tau=1.0, ethermo=0.0):
         super(ThermoNMGLEG, self).__init__(temp, dt, A, C, ethermo)
-        dself.tau = depend_value(value=tau, name="tau")
+        self._tau = depend_value(value=tau, name="tau")
 
     def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
         """Binds the appropriate degrees of freedom to the thermostat.
 
         This takes an object with degrees of freedom, and makes their momentum
         and mass vectors members of the thermostat. It also then creates the
         objects that will hold the data needed in the thermostat algorithms
@@ -969,24 +978,26 @@
         t = ThermoSVR(self.temp, self.dt, self.tau)
 
         t.bind(
             pm=(nm.pnm[0, :], nm.dynm3[0, :]), prng=self.prng
         )  # bind global thermostat to centroid
 
         # pipes temp and dt
-        dpipe(dself.temp, dd(t).temp)
-        dpipe(dself.dt, dd(t).dt)
-        dpipe(dself.tau, dd(t).tau)
+        dpipe(self._temp, t._temp)
+        dpipe(self._dt, t._dt)
+        dpipe(self._tau, t._tau)
 
-        dd(self).ethermo.add_dependency(dd(t).ethermo)
+        self._ethermo.add_dependency(t._ethermo)
         self._thermos.append(t)
 
 
-class ThermoCL(Thermostat):
+dproperties(ThermoNMGLE, ["tau"])
 
+
+class ThermoCL(Thermostat):
     """Represents a Langevin thermostat for systems driven by forces which are statistical
        in nature, i.e. they contain noise, and/or have an unwanted dissipative effect.
        This thermostat's dissipative term is modified to compensate for the inherent noise.
        Similarly, the noise term is modified to compensate for the inherent dissipation.
        The time scales of inherent diffusion and drift (intau and idtau) must be set
        to adequate values in order to make the system reach the target temperature.
        Alternatively, if the automatic parameter adjustment time scale apat is set > 0
@@ -1056,35 +1067,34 @@
            apat: Automatic parameter adjustment time scale. Defaults to 0 (off).
            ethermo: The initial heat energy transferred to the bath.
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
         """
 
         super(ThermoCL, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
 
         self.idstep = False
-        dself.tau = depend_value(value=tau, name="tau")
-        dself.intau = depend_value(value=intau, name="intau")
-        dself.idtau = depend_value(value=idtau, name="idtau")
-        dself.apat = depend_value(value=apat, name="apat")
-        dself.lgT = depend_value(
-            name="lgT", func=self.get_lgT, dependencies=[dself.tau, dself.dt]
-        )
-        dself.inT = depend_value(
-            name="inT", func=self.get_inT, dependencies=[dself.intau, dself.dt]
+        self._tau = depend_value(value=tau, name="tau")
+        self._intau = depend_value(value=intau, name="intau")
+        self._idtau = depend_value(value=idtau, name="idtau")
+        self._apat = depend_value(value=apat, name="apat")
+        self._lgT = depend_value(
+            name="lgT", func=self.get_lgT, dependencies=[self._tau, self._dt]
+        )
+        self._inT = depend_value(
+            name="inT", func=self.get_inT, dependencies=[self._intau, self._dt]
         )
-        dself.idT = depend_value(
-            name="idT", func=self.get_idT, dependencies=[dself.idtau, dself.dt]
+        self._idT = depend_value(
+            name="idT", func=self.get_idT, dependencies=[self._idtau, self._dt]
         )
-        dself.T = depend_value(
-            name="T", func=self.get_T, dependencies=[dself.lgT, dself.inT]
+        self._T = depend_value(
+            name="T", func=self.get_T, dependencies=[self._lgT, self._inT]
         )
-        dself.S = depend_value(
-            name="S", func=self.get_S, dependencies=[dself.temp, dself.lgT, dself.idT]
+        self._S = depend_value(
+            name="S", func=self.get_S, dependencies=[self._temp, self._lgT, self._idT]
         )
 
     def step(self):
         """Updates the bound momentum vector with a langevin thermostat."""
 
         et = self.ethermo
         p = dstrip(self.p).copy()
@@ -1113,16 +1123,18 @@
             else:
                 self.idtau *= (mytemp / self.temp) ** (self.dt / self.apat)
                 print(("ThermoCL inherent dissipation time scale: " + str(self.idtau)))
 
         self.idstep = not self.idstep
 
 
-class ThermoFFL(Thermostat):
+dproperties(ThermoCL, ["tau", "T", "S", "idtau", "intau", "apat", "lgT", "inT", "idT"])
+
 
+class ThermoFFL(ThermoLangevin):
     """Represents a fast-forward langevin thermostat.
 
     Depend objects:
        tau: Thermostat damping time scale. Larger values give a less strongly
           coupled thermostat.
        T: Coefficient of the diffusive contribution of the thermostat, i.e. the
           drift back towards equilibrium. Depends on tau and the time step.
@@ -1152,25 +1164,24 @@
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
            flip: The flipping type. Defaults to 'rescale'.
               Allowed values are 'soft', 'hard', 'rescale', 'none'.
         """
 
         super(ThermoFFL, self).__init__(temp, dt, ethermo)
-        dself = dd(self)
 
-        dself.dt = depend_value(value=dt, name="dt")
-        dself.tau = depend_value(value=tau, name="tau")
-        dself.T = depend_value(
-            name="T", func=self.get_T, dependencies=[dself.tau, dself.dt]
+        self._dt = depend_value(value=dt, name="dt")
+        self._tau = depend_value(value=tau, name="tau")
+        self._T = depend_value(
+            name="T", func=self.get_T, dependencies=[self._tau, self._dt]
         )
-        dself.S = depend_value(
-            name="S", func=self.get_S, dependencies=[dself.temp, dself.T]
+        self._S = depend_value(
+            name="S", func=self.get_S, dependencies=[self._temp, self._T]
         )
-        dself.flip = depend_value(value=flip, name="flip")
+        self._flip = depend_value(value=flip, name="flip")
 
         allowed_flips = ["soft", "hard", "rescale", "none"]
         if not (self.flip in allowed_flips):
             raise KeyError(
                 "Invalid flip type "
                 + self.flip
                 + '; allowed flip types: "'
@@ -1223,50 +1234,52 @@
 
         p *= sm
 
         self.p = p
         self.ethermo = et
 
 
+dproperties(ThermoFFL, "flip")
+
+
 class MultiThermo(Thermostat):
     def __init__(self, temp=1.0, dt=1.0, ethermo=0.0, thermolist=None):
         """Initialises Thermostat.
 
         Args:
            temp: The simulation temperature. Defaults to 1.0.
            dt: The simulation time step. Defaults to 1.0.
            ethermo: The initial heat energy transferred to the bath.
               Defaults to 0.0. Will be non-zero if the thermostat is
               initialised from a checkpoint file.
         """
-        dself = dd(self)
 
         self.tlist = thermolist
-        dself.temp = depend_value(name="temp", value=temp)
-        dself.dt = depend_value(name="dt", value=dt)
-        dself.ethermo = depend_value(name="ethermo", value=ethermo)
+        self._temp = depend_value(name="temp", value=temp)
+        self._dt = depend_value(name="dt", value=dt)
+        self._ethermo = depend_value(name="ethermo", value=ethermo)
         for t in self.tlist:
-            dpipe(dself.dt, dd(t).dt)
-            dpipe(dself.temp, dd(t).temp)
+            dpipe(self._dt, t._dt)
+            dpipe(self._temp, t._temp)
 
     def get_ethermo(self):
         et = 0.0
         for t in self.tlist:
             et += t.ethermo
         return et
 
     def bind(self, beads=None, atoms=None, pm=None, nm=None, prng=None, fixdof=None):
         """Binds the appropriate degrees of freedom to the thermostat."""
 
         # just binds all the sub-thermostats
         for t in self.tlist:
             t.bind(beads=beads, atoms=atoms, pm=pm, nm=nm, prng=prng, fixdof=fixdof)
-            dd(self).ethermo.add_dependency(dd(t).ethermo)
+            self._ethermo.add_dependency(t._ethermo)
 
-        dd(self).ethermo._func = self.get_ethermo
+        self._ethermo._func = self.get_ethermo
 
     def step(self):
         """Steps through all sub-thermostats."""
 
         for t in self.tlist:
             t.step()
         pass
```

### Comparing `ipi-2.6.0/ipi/external/importlib/bundledimportlib.py` & `ipi-2.6.3/ipi/external/importlib/bundledimportlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Backport of importlib.import_module from 3.x."""
+
 # While not critical (and in no way guaranteed!), it would be nice to keep this
 # code compatible with Python 2.3.
 import sys
 
 
 def _resolve_name(name, package, level):
     """Return the absolute name of the module to be imported."""
```

### Comparing `ipi-2.6.0/ipi/inputs/atoms.py` & `ipi-2.6.3/ipi/inputs/atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from ipi.utils.depend import *
 
 
 __all__ = ["InputAtoms"]
 
 
 class InputAtoms(Input):
-
     """Atoms input class.
 
     Handles generating the appropriate atoms class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/inputs/barostats.py` & `ipi-2.6.3/ipi/inputs/barostats.py`

 * *Files identical despite different names*

```diff
@@ -15,15 +15,14 @@
 from ipi.inputs.cell import *
 
 
 __all__ = ["InputBaro"]
 
 
 class InputBaro(Input):
-
     """Barostat input class.
 
     Handles generating the appropriate barostat class from the xml input file,
     and generating the xml checkpoint tags and data from an
     instance of the object.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/inputs/beads.py` & `ipi-2.6.3/ipi/inputs/beads.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from ipi.inputs.atoms import *
 
 
 __all__ = ["InputBeads"]
 
 
 class InputBeads(Input):
-
     """Beads input class.
 
     Handles generating the appropriate beads class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/inputs/cell.py` & `ipi-2.6.3/ipi/inputs/cell.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 from ipi.utils.inputvalue import *
 
 
 __all__ = ["InputCell"]
 
 
 class InputCell(InputArray):
-
     """Cell input class.
 
     Handles generating the appropriate cell class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
     """
 
     attribs = copy(InputArray.attribs)
 
-    default_help = "Deals with the cell parameters. Takes as array which can be used to initialize the cell vector matrix."
+    default_help = """
+Describes with the cell parameters. Takes as array which can be used to initialize the cell vector matrix.
+N.B.: the cell parameters are stored with the lattice vectors in the columns, and the cell must be oriented
+in such a way that the array is upper-triangular (i.e. with the first vector aligned along x and the second
+vector in the xy plane).     
+"""
     default_label = "CELL"
 
     def __init__(self, help=None, dimension=None, units=None, default=None, dtype=None):
         """Initializes InputCell.
 
         Just calls the parent initialization function with appropriate arguments.
         """
@@ -56,7 +60,17 @@
            properties given the attributes of the InputCell object.
         """
 
         h = super(InputCell, self).fetch()
         h.shape = (3, 3)
 
         return Cell(h=h)
+
+    def check(self):
+        """Checks for optional parameters."""
+
+        super(InputCell, self).check()
+
+        h = self.value.reshape(9)
+
+        if (h[[3, 6, 7]] ** 2).sum() > 1e-20:
+            raise ValueError("The cell matrix must be upper triangular.")
```

### Comparing `ipi-2.6.0/ipi/inputs/ensembles.py` & `ipi-2.6.3/ipi/inputs/ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from ipi.utils.units import *
 
 
 __all__ = ["InputEnsemble"]
 
 
 class InputEnsemble(Input):
-
     """Ensemble input class.
 
     Handles generating the appropriate ensemble class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/inputs/forcefields.py` & `ipi-2.6.3/ipi/inputs/forcefields.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     "InputFFCommittee",
     "InputFFdmd",
     "InputFFCavPhSocket",
 ]
 
 
 class InputForceField(Input):
-
     """ForceField input class.
 
     Handles generating one instance of a particular forcefield class from the xml
     input file, and generating the xml checkpoint tags and data from an
     instance of the object.
 
     Attributes:
@@ -85,18 +84,27 @@
         ),
     }
     fields = {
         "latency": (
             InputValue,
             {
                 "dtype": float,
-                "default": 0.01,
+                "default": 1e-4,
                 "help": "The number of seconds the polling thread will wait between exhamining the list of requests.",
             },
         ),
+        "offset": (
+            InputValue,
+            {
+                "dtype": float,
+                "default": 0.0,
+                "dimension": "energy",
+                "help": "A constant offset that is subtracted from the forcefield energy. Useful when there is a large core energy contribution that is constant throughout a simulation and hides significant changes in the 10th digit.",
+            },
+        ),
         "parameters": (
             InputValue,
             {"dtype": dict, "default": {}, "help": "The parameters of the force field"},
         ),
         "activelist": (
             InputArray,
             {
@@ -117,14 +125,15 @@
         Args:
            forceb: A ForceField object.
         """
 
         Input.store(self, ff)
         self.name.store(ff.name)
         self.latency.store(ff.latency)
+        self.offset.store(ff.offset)
         self.parameters.store(ff.pars)
         self.pbc.store(ff.dopbc)
         self.activelist.store(ff.active)
         self.threaded.store(ff.threaded)
 
     def fetch(self):
         """Creates a ForceField object.
@@ -135,22 +144,22 @@
 
         super(InputForceField, self).fetch()
 
         return ForceField(
             pars=self.parameters.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             active=self.activelist.fetch(),
             threaded=self.threaded.fetch(),
         )
 
 
 class InputFFSocket(InputForceField):
-
     """Creates a ForceField object with a socket interface.
 
     Handles generating one instance of a socket interface forcefield class.
 
     Attributes:
        mode: Describes whether the socket will be a unix or an internet socket.
 
@@ -284,14 +293,15 @@
             )
             self.exit_on_disconnect.store(True)
 
         return FFSocket(
             pars=self.parameters.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             active=self.activelist.fetch(),
             threaded=self.threaded.fetch(),
             interface=InterfaceSocket(
                 address=self.address.fetch(),
                 port=self.port.fetch(),
                 slots=self.slots.fetch(),
@@ -340,14 +350,15 @@
     def fetch(self):
         super(InputFFLennardJones, self).fetch()
 
         return FFLennardJones(
             pars=self.parameters.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             threaded=self.threaded.fetch(),
         )
 
         if self.slots.fetch() < 1 or self.slots.fetch() > 5:
             raise ValueError(
                 "Slot number " + str(self.slots.fetch()) + " out of acceptable range."
@@ -415,14 +426,15 @@
             coupling=self.dmd_coupling.fetch(),
             freq=self.dmd_freq.fetch(),
             dtdmd=self.dmd_dt.fetch(),
             dmdstep=self.dmd_step.fetch(),
             pars=self.parameters.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             threaded=self.threaded.fetch(),
         )
 
 
 class InputFFDebye(InputForceField):
     fields = {
@@ -476,14 +488,15 @@
 
         return FFDebye(
             H=self.hessian.fetch(),
             xref=self.x_reference.fetch(),
             vref=self.v_reference.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             threaded=self.threaded.fetch(),
         )
 
 
 class InputFFPlumed(InputForceField):
     fields = {
@@ -529,14 +542,15 @@
 
     def fetch(self):
         super(InputFFPlumed, self).fetch()
 
         return FFPlumed(
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             threaded=self.threaded.fetch(),
             plumeddat=self.plumeddat.fetch(),
             plumedstep=self.plumedstep.fetch(),
             init_file=self.file.fetch(),
         )
 
@@ -648,14 +662,15 @@
             alpha_scale=self.alpha_scale.fetch(),
             gcut_scale=self.gcut_scale.fetch(),
             skin=self.skin.fetch(),
             smooth_ei=self.smooth_ei.fetch(),
             reci_ei=self.reci_ei.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             threaded=self.threaded.fetch(),
         )
 
 
 class InputFFsGDML(InputForceField):
     fields = {
@@ -684,30 +699,38 @@
     def fetch(self):
         super(InputFFsGDML, self).fetch()
 
         return FFsGDML(
             sGDML_model=self.sGDML_model.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             threaded=self.threaded.fetch(),
         )
 
 
 class InputFFCommittee(InputForceField):
     default_help = """Combines multiple forcefields to build a committee model, that can 
                       be used to compute uncertainty-quantified machine-learning models. 
                       Each forcefield can be any of the other FF objects, and each should
                       be used with a client that generates a slightly different estimation
                       of energy and forces. These are averaged, and the mean used as the 
                       actual forcefield. Statistics about the distribution are also returned
                       as extras fields, and can be printed for further postprocessing. 
+                      It is also possible for a single FF object to return a JSON-formatted
+                      string containing entries `committee_pot`, `committee_force` and 
+                      `committee_virial`, that contain multiple members at once. These
+                      will be unpacked and combined with whatever else is present. 
+
                       Also contains options to use it for uncertainty estimation and for
                       active learning in a ML context, based on a committee model.
-                      Implements the approaches discussed in DOI: 10.1063/5.0036522.
+                      Implements the approaches discussed in 
+                      [Musil et al.](http://doi.org/10.1021/acs.jctc.8b00959)
+                      and [Imbalzano et al.](http://doi.org/10.1063/5.0036522)
                       """
     default_label = "FFCOMMITTEE"
 
     dynamic = {
         "ffsocket": (InputFFSocket, {"help": InputFFSocket.default_help}),
         "fflj": (InputFFLennardJones, {"help": InputFFLennardJones.default_help}),
         "ffdebye": (InputFFDebye, {"help": InputFFDebye.default_help}),
@@ -768,28 +791,37 @@
         InputValue,
         {
             "dtype": str,
             "default": "active_output",
             "help": "Output filename for structures that exceed the accuracy threshold of the model, to be used in active learning.",
         },
     )
+    fields["parse_json"] = (
+        InputValue,
+        {
+            "dtype": bool,
+            "default": False,
+            "help": "Tell the model whether to parse extras string looking for committee values of potential, forces, and virials. Default: false.",
+        },
+    )
 
     def store(self, ff):
         """Store all the sub-forcefields"""
 
         super(InputFFCommittee, self).store(ff)
         _fflist = ff.fflist
         if len(self.extra) != len(_fflist):
             self.extra = [0] * len(_fflist)
         self.weights.store(ff.ffweights)
         self.alpha.store(ff.alpha)
         self.baseline_uncertainty.store(ff.baseline_uncertainty)
         self.baseline_name.store(ff.baseline_name)
         self.active_thresh.store(ff.active_thresh)
         self.active_output.store(ff.active_out)
+        self.parse_json.store(ff.parse_json)
 
         for _ii, _obj in enumerate(_fflist):
             if self.extra[_ii] == 0:
                 if isinstance(_obj, FFSocket):
                     _iobj = InputFFSocket()
                     _iobj.store(_obj)
                     self.extra[_ii] = ("ffsocket", _iobj)
@@ -830,22 +862,24 @@
             fflist.append(v.fetch())
 
         # TODO: will actually need to create a FF object here!
         return FFCommittee(
             pars=self.parameters.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             fflist=fflist,
             ffweights=self.weights.fetch(),
             alpha=self.alpha.fetch(),
             baseline_uncertainty=self.baseline_uncertainty.fetch(),
             baseline_name=self.baseline_name.fetch(),
             active_thresh=self.active_thresh.fetch(),
             active_out=self.active_output.fetch(),
+            parse_json=self.parse_json.fetch(),
         )
 
 
 class InputFFCavPhSocket(InputFFSocket):
     default_help = """A cavity molecular dynamics driver for vibraitonal strong coupling. 
                       In the current implementation, only a single cavity mode polarized along the x and y directions is coupled to the molecules.
                       Check https://doi.org/10.1073/pnas.2009272117 and also examples/lammps/h2o-cavmd/ for details.
@@ -940,14 +974,15 @@
             raise ValueError("FFCavPhFPSockets cannot poll without threaded mode.")
 
         # just use threaded throughout
         return FFCavPhSocket(
             pars=self.parameters.fetch(),
             name=self.name.fetch(),
             latency=self.latency.fetch(),
+            offset=self.offset.fetch(),
             dopbc=self.pbc.fetch(),
             active=self.activelist.fetch(),
             threaded=self.threaded.fetch(),
             interface=InterfaceSocket(
                 address=self.address.fetch(),
                 port=self.port.fetch(),
                 slots=self.slots.fetch(),
```

### Comparing `ipi-2.6.0/ipi/inputs/forces.py` & `ipi-2.6.3/ipi/inputs/forces.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ipi.utils.inputvalue import *
 import numpy as np
 
 __all__ = ["InputForces", "InputForceComponent"]
 
 
 class InputForceComponent(Input):
-
     """ForceComponent input class.
 
     Uses the forcefield object whose name is specified as the value of the
     field (matching one of the forcefields defined in the simulation tag)
     to compute one component of the force acting on the ring polymer.
 
 
@@ -138,15 +137,14 @@
         if self.nbeads.fetch() < 0:
             raise ValueError(
                 "The forces must be evaluated over a positive number of beads."
             )
 
 
 class InputForces(Input):
-
     """Deals with creating all the forcefield objects required in the
     simulation.
 
     Dynamic fields:
        socket: Socket object to create the server socket.
     """
```

### Comparing `ipi-2.6.0/ipi/inputs/initializer.py` & `ipi-2.6.3/ipi/inputs/initializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "InputInitLabels",
     "InputInitCell",
     "InputInitThermo",
 ]
 
 
 class InputInitBase(InputValue):
-
     """Base class to handle initialization.
 
     Attributes:
        mode: The type of data to be initialized from.
        _initclass: Which InputInit class to use to read the data.
        _storageclass: Which data type to use to hold the data.
     """
@@ -122,15 +121,14 @@
         if initclass is None:  # allows for some flexibility in return class
             initclass = self._initclass
 
         return initclass(value=self.getval(), **rdict)
 
 
 class InputInitIndexed(InputInitBase):
-
     """Class to handle initialization of properties which the value of each
     bead and atom can be specified.
 
     Attributes:
        index: Which atom to initialize the value of.
        bead: Which bead to initialize the value of.
     """
@@ -154,15 +152,14 @@
     )
 
     default_label = "INITINDEXED"
     default_help = "This is a helper class to initialize with an index."
 
 
 class InputInitFile(InputInitBase):
-
     """Class to handle initialization from a file."""
 
     attribs = deepcopy(InputInitBase.attribs)
     attribs["mode"][1]["default"] = "chk"
     attribs["mode"][1]["options"] = ["xyz", "pdb", "chk", "ase"]
     attribs["mode"][1][
         "help"
@@ -188,30 +185,28 @@
 
     default_label = "INITFILE"
     default_help = "This is the class to initialize from file."
     _initclass = ei.InitFile
 
 
 class InputInitThermo(InputInitBase):
-
     """Class to handle initialization of the thermostat."""
 
     attribs = deepcopy(InputInitBase.attribs)
     attribs["mode"][1]["default"] = "manual"
     attribs["mode"][1]["options"] = ["chk", "manual"]
     attribs["mode"][1][
         "help"
     ] = "'chk' stands for initialization from a checkpoint file. 'manual' means that the value to initialize from is giving explicitly as a vector."
 
     default_label = "INITTHERMO"
     default_help = "This is the class to initialize the thermostat (ethermo and fictitious momenta)."
 
 
 class InputInitPositions(InputInitIndexed):
-
     """Class to handle initialization of the positions."""
 
     attribs = deepcopy(InputInitIndexed.attribs)
     attribs["mode"][1]["default"] = "chk"
     attribs["mode"][1]["options"] = ["manual", "xyz", "pdb", "ase", "chk"]
     attribs["mode"][1][
         "help"
@@ -220,15 +215,14 @@
 
     default_label = "INITPOSITIONS"
     default_help = "This is the class to initialize positions."
     _initclass = ei.InitIndexed
 
 
 class InputInitMomenta(InputInitPositions):
-
     """Class to handle initialization of the momenta."""
 
     attribs = deepcopy(InputInitPositions.attribs)
     attribs["mode"][1]["options"].append("thermal")
     attribs["mode"][1][
         "help"
     ] = """The input data format. 'xyz' and 'pdb' stand for xyz and pdb input files respectively. 
@@ -254,57 +248,53 @@
                 bead=self.bead.fetch(),
             )
         else:
             return super(InputInitMomenta, self).fetch()
 
 
 class InputInitVelocities(InputInitMomenta):
-
     """Class to handle initialization of the velocities."""
 
     attribs = deepcopy(InputInitMomenta.attribs)
 
     default_label = "INITVELOCITIES"
     default_help = "This is the class to initialize velocities."
 
 
 class InputInitMasses(InputInitPositions):
-
     """Class to handle initialization of the masses."""
 
     attribs = deepcopy(InputInitPositions.attribs)
 
     default_label = "INITMASSES"
     default_help = "This is the class to initialize atomic masses."
 
 
 class InputInitLabels(InputInitPositions):
-
     """Class to handle initialization of the atom labels."""
 
     attribs = deepcopy(InputInitPositions.attribs)
 
     default_label = "INITLABELS"
     default_help = "This is the class to initialize atomic labels."
 
     _storageclass = str
 
 
 class InputInitCell(InputInitBase):
-
     """Class to handle initialization of the cell."""
 
     attribs = deepcopy(InputInitBase.attribs)
     attribs["mode"] = (
         InputAttribute,
         {
             "dtype": str,
             "default": "manual",
             "options": ["manual", "pdb", "chk", "abc", "abcABC"],
-            "help": "This decides whether the system box is created from a cell parameter matrix, or from the side lengths and angles between them. If 'mode' is 'manual', then 'cell' takes a 9-elements vector containing the cell matrix (row-major).  The 1st element define lattice vector a, the 2nd, 5th elements define lattice vector b, and the 3rd, 6th, 9th elements define lattice vector c. The other elements are ignored. If 'mode' is 'abcABC', then 'cell' takes an array of 6 floats, the first three being the length of the sides of the system parallelopiped, and the last three being the angles (in degrees) between those sides. Angle A corresponds to the angle between sides b and c, and so on for B and C. If mode is 'abc', then this is the same as for 'abcABC', but the cell is assumed to be orthorhombic. 'pdb' and 'chk' read the cell from a PDB or a checkpoint file, respectively.",
+            "help": "This decides whether the system box is created from a cell parameter matrix, or from the side lengths and angles between them. If 'mode' is 'manual', then 'cell' takes a 9-elements vector containing the cell matrix (row-major, lattice vectors stored in columns).  The 1st element define lattice vector a, the 2nd, 5th elements define lattice vector b, and the 3rd, 6th, 9th elements define lattice vector c. The other elements are ignored, as the cell must be aligned so that it is upper triangular. If 'mode' is 'abcABC', then 'cell' takes an array of 6 floats, the first three being the length of the sides of the system parallelopiped, and the last three being the angles (in degrees) between those sides. Angle A corresponds to the angle between sides b and c, and so on for B and C. If mode is 'abc', then this is the same as for 'abcABC', but the cell is assumed to be orthorhombic. 'pdb' and 'chk' read the cell from a PDB or a checkpoint file, respectively.",
         },
     )
 
     default_label = "INITCELL"
     default_help = "This is the class to initialize cell."
 
     def fetch(self):
@@ -315,17 +305,15 @@
         'abc' or 'abcABC' modes.
         """
 
         mode = self.mode.fetch()
 
         ibase = super(InputInitCell, self).fetch()
         if mode == "abc" or mode == "abcABC":
-            h = io_xml.read_array(
-                float, ibase.value
-            )  # As of numpy v1.20, numpy.float as well as similar aliases (including numpy.int) were deprecated
+            h = io_xml.read_array(float, ibase.value)
 
             if mode == "abc":
                 if h.size != 3:
                     raise ValueError(
                         "If you are initializing cell from cell side lengths you must pass the 'cell' tag an array of 3 floats."
                     )
                 else:
@@ -354,25 +342,24 @@
             if h.size != 9:
                 raise ValueError(
                     "Cell objects must contain a 3x3 matrix describing the cell vectors."
                 )
 
             if not (h[3] == 0.0 and h[6] == 0.0 and h[7] == 0.0):
                 warning(
-                    "Cell vector matrix must be upper triangular, all elements below the diagonal being set to zero.",
+                    "Cell vector matrix must be upper triangular, all elements below the diagonal will be set to zero.",
                     verbosity.low,
                 )
                 h[3] = h[6] = h[7] = 0
             ibase.value = h
 
         return self._initclass(value=ibase.value, mode=mode, units=self.units.fetch())
 
 
 class InputInitializer(Input):
-
     """Input class to handle initialization.
 
     Attributes:
        nbeads: The number of beads to be used in the simulation.
 
     Dynamic fields:
        positions: An object to initialize the positions from.
```

### Comparing `ipi-2.6.0/ipi/inputs/interface.py` & `ipi-2.6.3/ipi/inputs/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from ipi.interfaces.sockets import *
 
 
 __all__ = ["InputInterfaceSocket"]
 
 
 class InputInterfaceSocket(Input):
-
     """Interface input class.
 
     Handles generating the apporopriate interface class from the xml
     input file, and generating the xml checkpoint tags and data from an
     instance of the object.
 
     Attributes:
@@ -65,14 +64,22 @@
             InputValue,
             {
                 "dtype": float,
                 "default": 1e-3,
                 "help": "This gives the number of seconds between each check for new clients.",
             },
         ),
+        "max_workers": (
+            InputValue,
+            {
+                "dtype": int,
+                "default": 128,
+                "help": "This gives the maximum number of job threads that are active simultaneously.",
+            },
+        ),
         "timeout": (
             InputValue,
             {
                 "dtype": float,
                 "default": 3600.0,
                 "help": "This gives the number of seconds before assuming a calculation has died. If 0 there is no timeout.",
             },
@@ -112,14 +119,15 @@
         self.latency.store(iface.latency)
         self.mode.store(iface.mode)
         self.address.store(iface.address)
         self.port.store(iface.port)
         self.slots.store(iface.slots)
         self.timeout.store(iface.timeout)
         self.pbc.store(iface.dopbc)
+        self.max_workers.store(iface.max_workers)
 
     def fetch(self):
         """Creates an InterfaceSocket object.
 
         Returns:
            An interface object with the appropriate socket given the attributes
            of the InputInterfaceSocket object.
@@ -130,14 +138,15 @@
             address=self.address.fetch(),
             port=self.port.fetch(),
             slots=self.slots.fetch(),
             mode=self.mode.fetch(),
             latency=self.latency.fetch(),
             timeout=self.timeout.fetch(),
             dopbc=self.pbc.fetch(),
+            max_workers=self.max_workers.fetch(),
         )
 
     def check(self):
         """Function that deals with optional arguments."""
 
         super(InputInterfaceSocket, self).check()
         if self.port.fetch() < 1 or self.port.fetch() > 65535:
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/al6xxx_kmc.py` & `ipi-2.6.3/ipi/inputs/motion/al6xxx_kmc.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/motion/alchemy.py` & `ipi-2.6.3/ipi/inputs/motion/alchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 )
 
 
 __all__ = ["InputAlchemy"]
 
 
 class InputAlchemy(InputDictionary):
-
     """Alchemy input class.
 
     Handles generating the appropriate alchemical exchange class from the xml input file.
 
     Fields:
         names: isotopes for exchanges.
         nxc: An optional float giving the number of exchanges that should be tried at each step.
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/atomswap.py` & `ipi-2.6.3/ipi/inputs/motion/atomswap.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 )
 
 
 __all__ = ["InputAtomSwap"]
 
 
 class InputAtomSwap(InputDictionary):
-
     """Atomswap input class.
 
     Monte Carlo swaps of atoms types
 
     Fields:
         names:  labels of the atoms that should be exchanged.
         nxc:    how many swaps should be attempted at each step. defaults to 1.0.
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/constrained_dynamics.py` & `ipi-2.6.3/ipi/inputs/motion/constrained_dynamics.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,14 @@
             robj = ConstraintList(cnstr_list)
         else:
             robj = super(InputConstraint, self).fetch()
         return robj
 
 
 class InputConstrainedDynamics(InputDictionary):
-
     """Dynamics input class.
 
     Handles generating the appropriate ensemble class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/dynamics.py` & `ipi-2.6.3/ipi/inputs/motion/dynamics.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from ipi.inputs.thermostats import InputThermo
 
 
 __all__ = ["InputDynamics"]
 
 
 class InputDynamics(InputDictionary):
-
     """Dynamics input class.
 
     Handles generating the appropriate ensemble class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
@@ -46,16 +45,21 @@
 
     attribs = {
         "mode": (
             InputAttribute,
             {
                 "dtype": str,
                 "default": "nve",
-                "help": "The ensemble that will be sampled during the simulation. ",
-                "options": ["nve", "nvt", "npt", "nst", "sc", "scnpt"],
+                "help": """The ensemble that will be sampled during the simulation.
+                nve: constant-energy-volume; nvt: constant-temperature-volume;
+                npt: constant-temperature-pressure(isotropic); nst: constant-temperature-stress(anisotropic);
+                sc: Suzuki-Chin high-order NVT; scnpt: Suzuki-Chin high-order NpT;
+                nvt-cc: constrained-centroid NVT;
+                 """,
+                "options": ["nve", "nvt", "npt", "nst", "sc", "scnpt", "nvt-cc"],
             },
         ),
         "splitting": (
             InputAttribute,
             {
                 "dtype": str,
                 "default": "obabo",
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/geop.py` & `ipi-2.6.3/ipi/inputs/motion/geop.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from ipi.inputs.initializer import *
 from ipi.utils.units import *
 
 __all__ = ["InputGeop"]
 
 
 class InputGeop(InputDictionary):
-
     """Geometry optimization options.
 
     Contains options related with geometry optimization, such as method,
     thresholds, linear search strategy, etc.
 
     """
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/instanton.py` & `ipi-2.6.3/ipi/inputs/motion/instanton.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from ipi.utils.inputvalue import *
 
 
 __all__ = ["InputInst"]
 
 
 class InputInst(InputDictionary):
-
     """Instanton optimization options.
 
     Contains options related with instanton, such as method,
     thresholds, hessian update strategy, etc.
 
     """
 
@@ -127,14 +126,55 @@
             InputArray,
             {
                 "dtype": float,
                 "default": input_default(factory=np.ones, args=(0,)),
                 "help": "Allows to specified non uniform time discretization as proposed in J. Chem. Phys. 134, 184107 (2011)",
             },
         ),
+        "friction": (
+            InputValue,
+            {
+                "dtype": bool,
+                "default": False,
+                "help": "Activates Friction. Add additional terms to the RP related to a position-independent frictional force. See Eq. 20 in J. Chem. Phys. 156, 194106 (2022)",
+            },
+        ),
+        "frictionSD": (
+            InputValue,
+            {
+                "dtype": bool,
+                "default": True,
+                "help": "Activates SD Friction. Add additional terms to the RP related to a position-dependent frictional force. See Eq. 32 in J. Chem. Phys. 156, 194106 (2022)",
+            },
+        ),
+        "fric_spec_dens": (
+            InputArray,
+            {
+                "dtype": float,
+                "default": input_default(factory=np.ones, args=(0,)),
+                "help": "Laplace Transform (LT) of friction. A two column data is expected. First column: w (cm^-1). Second column: LT(eta)(w). See Eq. 11 in J. Chem. Phys. 156, 194106 (2022). Note that within the separable coupling approximation the frequency dependence of the friction tensor is position independent.",
+            },
+        ),
+        "fric_spec_dens_ener": (
+            InputValue,
+            {
+                "dtype": float,
+                "default": 0.0,
+                "help": "Energy at which the LT of the friction tensor is evaluated in the client code",
+                "dimension": "energy",
+            },
+        ),
+        "eta": (
+            InputArray,
+            {
+                "dtype": float,
+                "default": input_default(factory=np.eye, args=(0,)),
+                "help": "Friction Tensor. Only to be used when frictionSD is disabled.",
+            },
+        ),
         "alt_out": (
             InputValue,
             {
                 "dtype": int,
                 "default": 1,
                 "help": """Alternative output:Prints different formatting of outputs for geometry, hessian and bead potential energies.
                                                All quantities are also accessible from typical i-pi output infrastructure.
@@ -164,17 +204,16 @@
             InputValue,
             {"dtype": float, "default": 0.1, "help": "Initial stretch amplitude."},
         ),
         # Hessian
         "hessian_init": (
             InputValue,
             {
-                "dtype": str,
-                "default": "false",
-                "options": ["true", "false"],
+                "dtype": bool,
+                "default": False,
                 "help": "How to initialize the hessian if it is not fully provided.",
             },
         ),
         "hessian": (
             InputArray,
             {
                 "dtype": float,
@@ -196,14 +235,22 @@
             {
                 "dtype": str,
                 "default": "none",
                 "options": ["none", "poly", "crystal"],
                 "help": "Removes the zero frequency vibrational modes depending on the symmetry of the system.",
             },
         ),
+        "fric_hessian": (
+            InputArray,
+            {
+                "dtype": float,
+                "default": input_default(factory=np.eye, args=(0,)),
+                "help": "(Approximate) friction second derivative from which a friction Hessian can be built.",
+            },
+        ),
         # L-BFGS
         "qlist_lbfgs": (
             InputArray,
             {
                 "dtype": float,
                 "default": input_default(factory=np.zeros, args=(0,)),
                 "help": "List of previous position differences for L-BFGS, if known.",
@@ -268,17 +315,16 @@
                 "help": "Set the zero of energy.",
                 "dimension": "energy",
             },
         ),
         "hessian_final": (
             InputValue,
             {
-                "dtype": str,
-                "default": "false",
-                "options": ["false", "true"],
+                "dtype": bool,
+                "default": False,
                 "help": "Decide if we are going to compute the final big-hessian by finite difference.",
             },
         ),
     }
 
     dynamic = {}
 
@@ -300,14 +346,19 @@
         self.biggest_step.store(optarrays["big_step"])
         self.opt.store(options["opt"])
 
         # Generic instanton
         self.max_e.store(options["max_e"])
         self.max_ms.store(options["max_ms"])
         self.discretization.store(options["discretization"])
+        self.friction.store(options["friction"])
+        self.frictionSD.store(options["frictionSD"])
+        if options["friction"]:
+            self.fric_spec_dens.store(options["fric_spec_dens"])
+            self.fric_spec_dens_ener.store(options["fric_spec_dens_ener"])
         self.alt_out.store(options["save"])
         self.prefix.store(options["prefix"])
         self.delta.store(optarrays["delta"])
         self.hessian_final.store(options["hessian_final"])
         self.old_pot.store(optarrays["old_u"])
         self.old_force.store(optarrays["old_f"])
         self.energy_shift.store(optarrays["energy_shift"])
@@ -317,14 +368,19 @@
             geop.options["opt"] == "nichols"
             or geop.options["opt"] == "NR"
             or geop.options["opt"] == "lanczos"
         ):
             self.hessian.store(optarrays["hessian"])
             self.hessian_update.store(options["hessian_update"])
             self.hessian_asr.store(options["hessian_asr"])
+            if options["friction"]:
+                if options["frictionSD"]:
+                    self.fric_hessian.store(optarrays["fric_hessian"])
+                else:
+                    self.eta.store(options["eta0"])
         elif geop.options["opt"] == "lbfgs":
             self.qlist_lbfgs.store(optarrays["qlist"])
             self.glist_lbfgs.store(optarrays["glist"])
             self.old_direction.store(optarrays["d"])
             self.scale_lbfgs.store(options["scale"])
             self.corrections_lbfgs.store(options["corrections"])
             self.ls_options.store(options["ls_options"])
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/motion.py` & `ipi-2.6.3/ipi/inputs/motion/motion.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 from .al6xxx_kmc import InputAlKMC
 from ipi.utils.units import *
 
 __all__ = ["InputMotion"]
 
 
 class InputMotionBase(Input):
-
     """Motion calculation input class.
 
     A class to encompass the different "motion" calculations.
 
     Attributes:
        mode: An optional string giving the kind of motion calculation to be performed.
 
@@ -420,15 +419,14 @@
             sc = Motion()
             # raise ValueError("'" + self.mode.fetch() + "' is not a supported motion calculation mode.")
 
         return sc
 
 
 class InputMotion(InputMotionBase):
-
     """Extends InputMotionBase to allow the definition of a multimotion"""
 
     attribs = copy(InputMotionBase.attribs)
 
     attribs["mode"][1]["options"].append("multi")
 
     dynamic = {
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/neb.py` & `ipi-2.6.3/ipi/inputs/motion/neb.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from ipi.inputs.initializer import *
 from ipi.utils.units import *
 
 __all__ = ["InputNEB"]
 
 
 class InputNEB(InputDictionary):
-
     """Geometry optimization options for nudged elastic band (NEB) calculations.
 
     Contains options related with geometry optimization, such as method,
     thresholds, linear search strategy, etc.
 
     Also contains options related specifically to NEB, such as spring constants
     and climbing image.
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/phonons.py` & `ipi-2.6.3/ipi/inputs/motion/phonons.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from ipi.inputs.initializer import *
 from ipi.utils.units import *
 
 __all__ = ["InputDynMatrix"]
 
 
 class InputDynMatrix(InputDictionary):
-
     """Dynamic matrix calculation options.
 
     Contains options related with finite difference computation of force constats.
 
     """
 
     attribs = {
@@ -105,15 +104,15 @@
                 "help": "Portion of the refined dynamical matrix known up to now.",
             },
         ),
     }
 
     dynamic = {}
 
-    default_help = "Fill in."
+    default_help = "Dynamical matrix Class. It calculates phonon modes and frequencies in solids as well as normal vibrational modes and frequencies of aperiodic systems."
     default_label = "PHONONS"
 
     def store(self, phonons):
         if phonons == {}:
             return
         self.mode.store(phonons.mode)
         self.pos_shift.store(phonons.deltax)
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/planetary.py` & `ipi-2.6.3/ipi/inputs/motion/planetary.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/motion/ramp.py` & `ipi-2.6.3/ipi/inputs/motion/ramp.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/motion/scphonons.py` & `ipi-2.6.3/ipi/inputs/motion/scphonons.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                 "help": "The exponent used to suppress low batch weights.",
             },
         ),
     }
 
     dynamic = {}
 
-    default_help = "Fill in."
+    default_help = "Self-consistent phonons class. It variationally optimizes the free energy to calculate the best harmonic approximation to a system."
     default_label = "SCPHONONS"
 
     def store(self, phonons):
         if phonons == {}:
             return
         self.mode.store(phonons.mode)
         self.prefix.store(phonons.prefix)
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/stringmep.py` & `ipi-2.6.3/ipi/inputs/motion/stringmep.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from ipi.inputs.initializer import *
 from ipi.utils.units import *
 
 __all__ = ["InputStringMEP"]
 
 
 class InputStringMEP(InputDictionary):
-
     """Options for string minimal energy path calculations.
 
     Contains options related to geometry optimization, such as method,
     thresholds, etc.
     Also contains options related specifically to String method.
     """
```

### Comparing `ipi-2.6.0/ipi/inputs/motion/vscf.py` & `ipi-2.6.3/ipi/inputs/motion/vscf.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
                 "help": "The number of forces evaluations per i-PI step.",
             },
         ),
     }
 
     dynamic = {}
 
-    default_help = "Fill in."
+    default_help = "Vibrational self-consistent field class. Approximates the vibrational eigenstates and eigenvalues of a system by performing a normal mode expansion of the potential energy surface."
     default_label = "PHONONS"
 
     def store(self, nm):
         if nm == {}:
             return
         self.mode.store(nm.mode)
         self.prefix.store(nm.prefix)
```

### Comparing `ipi-2.6.0/ipi/inputs/outputs.py` & `ipi-2.6.3/ipi/inputs/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import ipi.engine.outputs as eoutputs
 
 
 __all__ = ["InputOutputs", "InputProperties", "InputTrajectory", "InputCheckpoint"]
 
 
 class InputProperties(InputArray):
-
     """Simple input class to describe output for properties.
 
     Storage class for PropertyOutput.
 
     Attributes:
        filename: The name of the file to output to.
        stride: The number of steps that should be taken between outputting the
@@ -94,15 +93,14 @@
         if self.stride.fetch() < 0:
             raise ValueError(
                 "The stride length for the properties file output must be positive."
             )
 
 
 class InputTrajectory(InputValue):
-
     """Simple input class to describe output for trajectories.
 
     Storage class for TrajectoryOutput.
 
     Attributes:
        filename: The (base) name of the file to output to.
        stride: The number of steps that should be taken between outputting the
@@ -218,15 +216,14 @@
         if self.stride.fetch() < 0:
             raise ValueError(
                 "The stride length for the trajectory file output must be positive."
             )
 
 
 class InputCheckpoint(InputValue):
-
     """Simple input class to describe output for properties.
 
     Storage class for CheckpointOutput.
 
     Attributes:
        filename: The (base) name of the file to output to.
        stride: The number of steps that should be taken between outputting the
@@ -319,15 +316,14 @@
         if self.stride.fetch() < 0:
             raise ValueError(
                 "The stride length for the checkpoint file output must be positive."
             )
 
 
 class InputOutputs(Input):
-
     """List of outputs input class.
 
     An example of a dynamic input class: a variable number of tags might be
     present, corresponding to different output requests. This allows for
     instance to print multiple property outputs, with different content
     and/or output frequency.
```

### Comparing `ipi-2.6.0/ipi/inputs/simulation.py` & `ipi-2.6.3/ipi/inputs/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from ipi.inputs.smotion import InputSmotion
 
 
 __all__ = ["InputSimulation"]
 
 
 class InputSimulation(Input):
-
     """Simulation input class.
 
     Handles generating the appropriate forcefield class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
@@ -40,15 +39,14 @@
 
     Fields:
        output: A list of the required outputs.
        prng: A random number generator object.
        step: An integer giving the current simulation step. Defaults to 0.
        total_steps: The total number of steps. Defaults to 1000
        total_time:  The wall clock time limit. Defaults to 0 (no limit).
-       paratemp: A helper object for parallel tempering simulations
 
     Dynamic fields:
        system: Holds the data needed to specify the state of a single system.
        ffsocket: Gives a forcefield which will use a socket interface to
           communicate with the driver code.
        fflj: Gives a forcefield which uses the internal Python Lennard-Jones
           script to calculate the potential and forces.
@@ -118,15 +116,26 @@
         ),
         "mode": (
             InputAttribute,
             {
                 "dtype": str,
                 "default": "md",
                 "help": "What kind of simulation should be run.",
-                "options": ["md", "paratemp", "static"],
+                "options": ["md", "static"],
+            },
+        ),
+        "safe_stride": (
+            InputAttribute,
+            {
+                "dtype": int,
+                "default": 1,
+                "help": """Consistent simulation states will be saved every this number of steps. 
+Saving state entails a small overhead, so you may want to set this to the smallest output
+frequency in your simulation to make i-PI faster. Use at your own risk!
+""",
             },
         ),
         "floatformat": (
             InputAttribute,
             {
                 "dtype": str,
                 "default": "%16.8e",
@@ -209,14 +218,15 @@
             self.verbosity.store("low")
         elif verbosity.quiet:
             self.verbosity.store("quiet")
         else:
             raise ValueError("Invalid verbosity level")
 
         self.mode.store(simul.mode)
+        self.safe_stride.store(simul.safe_stride)
 
         _fflist = [v for k, v in sorted(simul.fflist.items())]
         if len(self.extra) != len(_fflist) + len(simul.syslist):
             self.extra = [0] * (len(_fflist) + len(simul.syslist))
 
         for (
             _ii,
@@ -327,10 +337,11 @@
             outputs=self.output.fetch(),
             prng=self.prng.fetch(),
             smotion=self.smotion.fetch(),
             step=self.step.fetch(),
             tsteps=self.total_steps.fetch(),
             ttime=self.total_time.fetch(),
             threads=self.threading.fetch(),
+            safe_stride=self.safe_stride.fetch(),
         )
 
         return rsim
```

### Comparing `ipi-2.6.0/ipi/inputs/smotion/dmd.py` & `ipi-2.6.3/ipi/inputs/smotion/dmd.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/smotion/metad.py` & `ipi-2.6.3/ipi/inputs/smotion/metad.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/smotion/remd.py` & `ipi-2.6.3/ipi/inputs/smotion/remd.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/smotion/smotion.py` & `ipi-2.6.3/ipi/inputs/smotion/smotion.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/inputs/system.py` & `ipi-2.6.3/ipi/inputs/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
                     isys.fetch()
                 )  # fetches the generated System and appends to the list
 
         return lsys
 
 
 class InputSystem(Input):
-
     """Physical system input class.
 
     Handles generating the appropriate forcefield class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
```

### Comparing `ipi-2.6.0/ipi/inputs/thermostats.py` & `ipi-2.6.3/ipi/inputs/thermostats.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from ipi.utils.inputvalue import *
 
 
 __all__ = ["InputThermo"]
 
 
 class InputThermoBase(Input):
-
     """Thermostat input class.
 
     Handles generating the appropriate thermostat class from the xml input file,
     and generating the xml checkpoint tags and data from an instance of the
     object.
 
     Attributes:
@@ -203,28 +202,28 @@
             self.mode.store("pile_g")
             self.tau.store(thermo.tau)
             self.pile_lambda.store(thermo.pilescale)
             self.pile_centroid_t.store(thermo.pilect)
         elif type(thermo) is ethermostats.ThermoGLE:
             self.mode.store("gle")
             self.A.store(thermo.A)
-            if dd(thermo).C._func is None:
+            if thermo._C._func is None:
                 self.C.store(thermo.C)
             self.s.store(thermo.s)
         elif type(thermo) is ethermostats.ThermoNMGLE:
             self.mode.store("nm_gle")
             self.A.store(thermo.A)
-            if dd(thermo).C._func is None:
+            if thermo._C._func is None:
                 self.C.store(thermo.C)
             self.s.store(thermo.s)
         elif type(thermo) is ethermostats.ThermoNMGLEG:
             self.mode.store("nm_gle_g")
             self.A.store(thermo.A)
             self.tau.store(thermo.tau)
-            if dd(thermo).C._func is None:
+            if thermo._C._func is None:
                 self.C.store(thermo.C)
             self.s.store(thermo.s)
         elif type(thermo) is ethermostats.ThermoCL:
             self.mode.store("cl")
             self.tau.store(thermo.tau)
             self.intau.store(thermo.intau)
             self.idtau.store(thermo.idtau)
@@ -337,15 +336,14 @@
                 )
         if mode in ["gle", "nm_gle", "nm_gle_g"]:
             pass  # PERHAPS DO CHECKS THAT MATRICES SATISFY REASONABLE CONDITIONS (POSITIVE-DEFINITENESS, ETC)
         # MR Check that pilect is not less than 0.0
 
 
 class InputThermo(InputThermoBase):
-
     """Extends InputThermoBase to allow the definition of a multithermo"""
 
     attribs = copy(InputThermoBase.attribs)
 
     attribs["mode"][1]["options"].append("multi")
 
     dynamic = {
```

### Comparing `ipi-2.6.0/ipi/interfaces/sockets.py` & `ipi-2.6.3/ipi/interfaces/sockets.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,58 +18,73 @@
 
 import numpy as np
 import json
 
 from ipi.utils.messages import verbosity, warning, info
 from ipi.utils.softexit import softexit
 
+from concurrent.futures import ThreadPoolExecutor
+
 
 __all__ = ["InterfaceSocket"]
 
 
 HDRLEN = 12
 UPDATEFREQ = 10
-TIMEOUT = 0.02
+TIMEOUT = 0.1
 SERVERTIMEOUT = 5.0 * TIMEOUT
 NTIMEOUT = 20
+SELECTTIMEOUT = 60
 
 
 def Message(mystr):
     """Returns a header of standard length HDRLEN."""
 
     # convert to bytestream since we'll be sending this over a socket
     return str.ljust(str.upper(mystr), HDRLEN).encode()
 
 
-class Disconnected(Exception):
+MESSAGE = {
+    msg: Message(msg)
+    for msg in [
+        "exit",
+        "status",
+        "ready",
+        "havedata",
+        "init",
+        "needinit",
+        "posdata",
+        "getforce",
+        "forceready",
+    ]
+}
 
+
+class Disconnected(Exception):
     """Disconnected: Raised if client has been disconnected."""
 
     pass
 
 
 class InvalidSize(Exception):
-
     """Disconnected: Raised if client returns forces with inconsistent number of atoms."""
 
     pass
 
 
 class InvalidStatus(Exception):
-
     """InvalidStatus: Raised if client has the wrong status.
 
     Shouldn't have to be used if the structure of the program is correct.
     """
 
     pass
 
 
 class Status(object):
-
     """Simple class used to keep track of the status of the client.
 
     Uses bitwise or to give combinations of different status options.
     i.e. Status.Up | Status.Ready would be understood to mean that the client
     was connected and ready to receive the position and cell data.
 
     Attributes:
@@ -89,15 +104,14 @@
     NeedsInit = 4
     HasData = 8
     Busy = 16
     Timeout = 32
 
 
 class DriverSocket(socket.socket):
-
     """Deals with communication between the client and driver code.
 
     Deals with sending and receiving the data between the client and the driver
     code. This class holds common functions which are used in the driver code,
     but can also be used to directly implement a python client.
     Basically it's just a wrapper around socket to simplify some of the
     specific needs of i-PI communication pattern.
@@ -113,27 +127,28 @@
            socket: A socket through which the communication should be done.
         """
 
         super(DriverSocket, self).__init__(
             sock.family, sock.type, sock.proto, fileno=socket.dup(sock.fileno())
         )
         self.settimeout(sock.gettimeout())
+
         self._buf = np.zeros(0, np.byte)
         if socket:
             self.peername = self.getpeername()
         else:
             self.peername = "no_socket"
 
     def send_msg(self, msg):
         """Send the next message through the socket.
 
         Args:
            msg: The message to send through the socket.
         """
-        return self.sendall(Message(msg))
+        return self.sendall(MESSAGE[msg])
 
     def recv_msg(self, length=HDRLEN):
         """Get the next message send through the socket.
 
         Args:
            l: Length of the accepted message. Defaults to HDRLEN.
         """
@@ -175,25 +190,24 @@
                         verbosity.low,
                     )
                     raise Disconnected()
                 pass
 
             if not timeout and bpart == 0:
                 raise Disconnected()
-
             bpos += bpart
 
-        if hasattr(dest, "shape"):
-            return np.fromstring(self._buf[0:blen], dest.dtype).reshape(dest.shape)
+        if dest.ndim > 0:
+            dest[:] = np.frombuffer(self._buf[0:blen], dest.dtype).reshape(dest.shape)
+            return dest  # tmp.copy() #np.frombuffer(self._buf[0:blen], dest.dtype).reshape(dest.shape).copy()
         else:
-            return np.fromstring(self._buf[0:blen], dest.dtype)[0]
+            return np.frombuffer(self._buf[0:blen], dest.dtype)[0]
 
 
 class Driver(DriverSocket):
-
     """Deals with communication between the client and driver code.
 
     Deals with sending and receiving the data from the driver code. Keeps track
     of the status of the driver. Initialises the driver forcefield, sends the
     position and cell data, and receives the force data.
 
     Attributes:
@@ -223,63 +237,117 @@
         if self.exit_on_disconnect:
             trd = threading.Thread(
                 target=softexit.trigger, kwargs={"message": "Client shutdown."}
             )
             trd.daemon = True
             trd.start()
 
-        self.sendall(Message("exit"))
+        self.send_msg("exit")
         self.status = Status.Disconnected
 
         super(DriverSocket, self).shutdown(how)
 
-    def _getstatus(self):
-        """Gets driver status.
+    def _getstatus_select(self):
+        """Gets driver status. Uses socket.select to make sure one can read/write on the socket.
 
         Returns:
            An integer labelling the status via bitwise or of the relevant members
            of Status.
         """
 
         if not self.waitstatus:
             try:
                 # This can sometimes hang with no timeout.
-                # Using the recommended 60 s.
-                readable, writable, errored = select.select([], [self], [], 60)
+                readable, writable, errored = select.select(
+                    [], [self], [], SELECTTIMEOUT
+                )
                 if self in writable:
-                    self.sendall(Message("status"))
+                    self.send_msg("status")
                     self.waitstatus = True
             except socket.error:
                 return Status.Disconnected
 
         try:
-            reply = self.recv(HDRLEN)
+            readable, writable, errored = select.select([self], [], [], SELECTTIMEOUT)
+            if self in readable:
+                reply = self.recv_msg(HDRLEN)
+                self.waitstatus = False  # got some kind of reply
+            else:
+                # This is usually due to VERY slow clients.
+                warning(
+                    f" @SOCKET: Couldn't find readable socket in {SELECTTIMEOUT}s, will try again",
+                    verbosity.low,
+                )
+                return Status.Busy
+        except socket.timeout:
+            warning(" @SOCKET:   Timeout in status recv!", verbosity.debug)
+            return Status.Up | Status.Busy | Status.Timeout
+        except:
+            warning(
+                " @SOCKET:   Other socket exception. Disconnecting client and trying to carry on.",
+                verbosity.debug,
+            )
+            return Status.Disconnected
+
+        if not len(reply) == HDRLEN:
+            return Status.Disconnected
+        elif reply == MESSAGE["ready"]:
+            return Status.Up | Status.Ready
+        elif reply == MESSAGE["needinit"]:
+            return Status.Up | Status.NeedsInit
+        elif reply == MESSAGE["havedata"]:
+            return Status.Up | Status.HasData
+        else:
+            warning(" @SOCKET:    Unrecognized reply: " + str(reply), verbosity.low)
+            return Status.Up
+
+    def _getstatus_direct(self):
+        """Gets driver status. Relies on blocking send/recv, which might lead to
+        timeouts with slow networks.
+
+        Returns:
+           An integer labelling the status via bitwise or of the relevant members
+           of Status.
+        """
+
+        if not self.waitstatus:
+            try:
+                self.send_msg("status")
+                self.waitstatus = True
+            except socket.error:
+                return Status.Disconnected
+        try:
+            reply = self.recv_msg(HDRLEN)
             self.waitstatus = False  # got some kind of reply
         except socket.timeout:
             warning(" @SOCKET:   Timeout in status recv!", verbosity.debug)
             return Status.Up | Status.Busy | Status.Timeout
         except:
             warning(
                 " @SOCKET:   Other socket exception. Disconnecting client and trying to carry on.",
                 verbosity.debug,
             )
             return Status.Disconnected
 
         if not len(reply) == HDRLEN:
             return Status.Disconnected
-        elif reply == Message("ready"):
+        elif reply == MESSAGE["ready"]:
             return Status.Up | Status.Ready
-        elif reply == Message("needinit"):
+        elif reply == MESSAGE["needinit"]:
             return Status.Up | Status.NeedsInit
-        elif reply == Message("havedata"):
+        elif reply == MESSAGE["havedata"]:
             return Status.Up | Status.HasData
         else:
             warning(" @SOCKET:    Unrecognized reply: " + str(reply), verbosity.low)
             return Status.Up
 
+    # depending on the system either _select or _direct can be slightly faster
+    # if you're network limited it might be worth experimenting changing this
+    _getstatus = _getstatus_select
+
     def get_status(self):
         """Sets (and returns) the client internal status. Wait for an answer if
         the client is busy."""
         status = self._getstatus()
         while status & Status.Busy:
             status = self._getstatus()
         self.status = status
@@ -297,15 +365,15 @@
            InvalidStatus: Raised if the status is not NeedsInit.
         """
 
         if self.status & Status.NeedsInit:
             try:
                 # combines all messages in one to reduce latency
                 self.sendall(
-                    Message("init")
+                    MESSAGE["init"]
                     + np.int32(rid)
                     + np.int32(len(pars))
                     + pars.encode()
                 )
             except:
                 self.get_status()
                 return
@@ -318,31 +386,40 @@
         Args:
            pos: An array containing the atom positions.
            cell: A cell object giving the system box.
 
         Raises:
            InvalidStatus: Raised if the status is not Ready.
         """
+        global TIMEOUT  # we need to update TIMEOUT in case of sendall failure
 
         if self.status & Status.Ready:
             try:
                 # reduces latency by combining all messages in one
                 self.sendall(
-                    Message("posdata")
-                    + h_ih[0].tobytes()  # header
-                    + h_ih[1].tobytes()  # cell
-                    + np.int32(len(pos) // 3).tobytes()  # inverse cell
-                    + pos.tobytes()  # length of position array  # positions
+                    MESSAGE["posdata"]  # header
+                    + h_ih[0].tobytes()  # cell
+                    + h_ih[1].tobytes()  # inverse cell
+                    + np.int32(len(pos) // 3).tobytes()  # length of position array
+                    + pos.tobytes()  # positions
                 )
-
                 self.status = Status.Up | Status.Busy
-            except:
-                print("Error in sendall, resetting status")
-                self.get_status()
+            except socket.timeout:
+                warning(
+                    f"Timeout in sendall after {TIMEOUT}s: resetting status and increasing timeout",
+                    verbosity.quiet,
+                )
+                self.status = Status.Timeout
+                TIMEOUT *= 2
                 return
+            except Exception as exc:
+                warning(
+                    f"Other exception during posdata receive: {exc}", verbosity.quiet
+                )
+                raise exc
         else:
             raise InvalidStatus("Status in sendpos was " + self.status)
 
     def getforce(self):
         """Gets the potential energy, force and virial from the driver.
 
         Raises:
@@ -350,15 +427,15 @@
            Disconnected: Raised if the driver has disconnected.
 
         Returns:
            A list of the form [potential, force, virial, extra].
         """
 
         if self.status & Status.HasData:
-            self.sendall(Message("getforce"))
+            self.send_msg("getforce")
             reply = ""
             while True:
                 try:
                     reply = self.recv_msg()
                 except socket.timeout:
                     warning(
                         " @SOCKET:   Timeout in getforce, trying again!", verbosity.low
@@ -366,15 +443,15 @@
                     continue
                 except:
                     warning(
                         " @SOCKET:   Error while receiving message: %s" % (reply),
                         verbosity.low,
                     )
                     raise Disconnected()
-                if reply == Message("forceready"):
+                if reply == MESSAGE["forceready"]:
                     break
                 else:
                     warning(
                         " @SOCKET:   Unexpected getforce reply: %s" % (reply),
                         verbosity.low,
                     )
                 if reply == "":
@@ -383,23 +460,24 @@
             raise InvalidStatus("Status in getforce was " + str(self.status))
 
         mu = np.float64()
         mu = self.recvall(mu)
 
         mlen = np.int32()
         mlen = self.recvall(mlen)
+
         mf = np.zeros(3 * mlen, np.float64)
         mf = self.recvall(mf)
 
         mvir = np.zeros((3, 3), np.float64)
         mvir = self.recvall(mvir)
 
         # Machinery to return a string as an "extra" field.
         # Comment if you are using a ancient patched driver that does not return anything!
-        # Actually, you should really update your driver, you're like half a decade behind.
+        # Actually, you should really update your driver, you're like a decade behind.
         mlen = np.int32()
         mlen = self.recvall(mlen)
         if mlen > 0:
             mxtra = np.zeros(mlen, np.character)
             mxtra = self.recvall(mxtra)
             mxtra = bytearray(mxtra).decode("utf-8")
         else:
@@ -419,15 +497,14 @@
                 pass
             if "raw" in mxtradict:
                 raise ValueError(
                     "'raw' cannot be used as a field in a JSON-formatted extra string"
                 )
 
             mxtradict["raw"] = mxtra
-
         return [mu, mf, mvir, mxtradict]
 
     def dispatch(self, r):
         """Dispatches a request r and looks after it setting results
         once it has been evaluated. This is meant to be launched as a
         separate thread, and takes care of all the communication related to
         the request.
@@ -467,33 +544,35 @@
 
         try:
             r["result"] = self.getforce()
         except Disconnected:
             self.status = Status.Disconnected
             return
 
+        r["result"][0] -= r["offset"]
+
         if len(r["result"][1]) != len(r["pos"][r["active"]]):
             raise InvalidSize
 
         # If only a piece of the system is active, resize forces and reassign
-        rftemp = r["result"][1]
-        r["result"][1] = np.zeros(len(r["pos"]), dtype=np.float64)
-        r["result"][1][r["active"]] = rftemp
+        if len(r["active"]) != len(r["pos"]):
+            rftemp = r["result"][1]
+            r["result"][1] = np.zeros(len(r["pos"]), dtype=np.float64)
+            r["result"][1][r["active"]] = rftemp
         r["t_finished"] = time.time()
         self.lastreq = r["id"]  #
 
         # updates the status of the client before leaving
         self.get_status()
 
         # marks the request as done as the very last thing
         r["status"] = "Done"
 
 
 class InterfaceSocket(object):
-
     """Host server class.
 
     Deals with distribution of all the jobs between the different client servers
     and both initially and as clients either finish or are disconnected.
     Deals with cleaning up after all calculations are done. Also deals with the
     threading mechanism, and cleaning up if the interface is killed.
 
@@ -525,28 +604,28 @@
         address="localhost",
         port=31415,
         slots=4,
         mode="unix",
         timeout=1.0,
         match_mode="auto",
         exit_on_disconnect=False,
+        max_workers=128,
     ):
         """Initialises interface.
 
         Args:
            address: An optional string giving the name of the host server.
               Defaults to 'localhost'.
            port: An optional integer giving the port number. Defaults to 31415.
            slots: An optional integer giving the maximum allowed backlog of
               queueing clients. Defaults to 4.
            mode: An optional string giving the type of socket. Defaults to 'unix'.
-           latency: An optional float giving the time in seconds the socket will
-              wait before updating the client list. Defaults to 1e-3.
            timeout: Length of time waiting for data from a client before we assume
               the connection is dead and disconnect the client.
+            max_workers: Maximum number of threads launched concurrently
 
         Raises:
            NameError: Raised if mode is not 'unix' or 'inet'.
         """
 
         self.address = address
         self.port = port
@@ -554,14 +633,16 @@
         self.mode = mode
         self.timeout = timeout
         self.poll_iter = UPDATEFREQ  # triggers pool_update at first poll
         self.prlist = []  # list of pending requests
         self.match_mode = match_mode  # heuristics to match jobs and active clients
         self.requests = None  # these will be linked to the request list of the FFSocket object using the interface
         self.exit_on_disconnect = exit_on_disconnect
+        self.max_workers = max_workers
+        self.offset = 0.0  # a constant energy offset added to the results returned by the driver (hacky but simple)
 
     def open(self):
         """Creates a new socket.
 
         Used so that we can create a interface object without having to also
         create the associated socket object.
         """
@@ -578,15 +659,23 @@
                     "Error opening unix socket. Check if a file "
                     + ("/tmp/ipi_" + self.address)
                     + " exists, and remove it if unused."
                 )
 
         elif self.mode == "inet":
             self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+
+            try:
+                self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+                # TCP_NODELAY is set because Nagle's algorithm slows down a lot
+                # the communication pattern of i-PI
+                self.server.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+            except OSError as e:
+                warning(f"Error setting socket options {e}")
+
             self.server.bind((self.address, self.port))
             info(
                 "Created inet socket with address "
                 + self.address
                 + " and port number "
                 + str(self.port),
                 verbosity.medium,
@@ -600,14 +689,15 @@
 
         self.server.listen(self.slots)
         self.server.settimeout(SERVERTIMEOUT)
 
         # these are the two main objects the socket interface should worry about and manage
         self.clients = []  # list of active clients (working or ready to compute)
         self.jobs = []  # list of jobs
+        self.executor = ThreadPoolExecutor(max_workers=self.max_workers)
 
     def close(self):
         """Closes down the socket."""
 
         info(" @SOCKET: Shutting down the driver interface.", verbosity.low)
 
         for c in self.clients:
@@ -675,16 +765,15 @@
                     c.close()
                 except socket.error:
                     pass
                 c.status = Status.Disconnected
                 self.clients.remove(c)
                 # requeue jobs that have been left hanging
                 for [k, j, tc] in self.jobs[:]:
-                    if tc.is_alive():
-                        tc.join(2)
+                    tc.result()
                     if j is c:
                         self.jobs = [
                             w for w in self.jobs if not (w[0] is k and w[1] is j)
                         ]  # removes pair in a robust way
 
                         k["status"] = "Queued"
                         k["start"] = -1
@@ -845,14 +934,19 @@
                 continue
 
             elif match_ids == "free" and fc.locked:
                 continue
 
             # makes sure the request is marked as running and the client included in the jobs list
             fc.locked = fc.lastreq is r["id"]
+
+            r["offset"] = (
+                self.offset
+            )  # transmits with the request an offset value for the energy (typically zero)
+
             r["status"] = "Running"
             self.prlist.remove(r)
             info(
                 " @SOCKET: %s Assigning [%5s] request id %4s to client with last-id %4s (% 3d/% 3d : %s)"
                 % (
                     time.strftime("%y/%m/%d-%H:%M:%S"),
                     match_ids,
@@ -860,32 +954,32 @@
                     str(fc.lastreq),
                     self.clients.index(fc),
                     len(self.clients),
                     str(fc.peername),
                 ),
                 verbosity.high,
             )
-            fc_thread = threading.Thread(
-                target=fc.dispatch, name="DISPATCH", kwargs={"r": r}
-            )
+            # fc_thread = threading.Thread(
+            #    target=fc.dispatch, name="DISPATCH", kwargs={"r": r}
+            # )
+            fc_thread = self.executor.submit(fc.dispatch, r=r)
             self.jobs.append([r, fc, fc_thread])
-            fc_thread.daemon = True
-            fc_thread.start()
+            # fc_thread.daemon = True
+            # fc_thread.start()
             return True
 
         return False
 
     def check_job_finished(self, r, c, ct):
         """
         Checks if a job has been completed, and retrieves the results
         """
 
         if r["status"] == "Done":
-            while ct.is_alive():  # we can wait for end of thread
-                ct.join()
+            ct.result()
             self.jobs = [
                 w for w in self.jobs if not (w[0] is r and w[1] is c)
             ]  # removes pair in a robust way
             return 1
 
         if (
             self.timeout > 0
```

### Comparing `ipi-2.6.0/ipi/utils/constrtools.py` & `ipi-2.6.3/ipi/utils/constrtools.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "ConstraintList",
     "AngleConstraint",
     "RigidBondConstraint",
     "EckartConstraint",
 ]
 
 
-class ConstraintBase(dobject):
+class ConstraintBase:
     """Base constraint class for MD. Takes care of indexing of
     the atoms that are affected by the constraint, and creates
     depend objects to store the constraint function and gradient."""
 
     def __init__(self, constrained_indices, ncons=0):
         """Initialize the constraint.
 
@@ -66,65 +66,64 @@
             self.i3_indirect[ri] = [3 * rri, 3 * rri + 1, 3 * rri + 2]
 
     def bind(self, beads):
         """Binds the constraint to a beads object - so that all of the
         necessary quantities are easily and depend-ably accessable"""
 
         self.beads = beads
-        dself = dd(self)
 
         # masses of the atoms involved in the constraint - repeated 4
         # times to vectorize operations on 3-vectors
-        dself.m3 = depend_array(
+        self._m3 = depend_array(
             name="m3",
             value=np.zeros(self.n_unique * 3),
             func=(lambda: self.beads.m3[0, self.i3_unique]),
-            dependencies=[dd(self.beads).m3],
+            dependencies=[self.beads._m3],
         )
 
         # The constraint function is computed at iteratively updated
         # coordinates during geodesic integration; this array holds such
         # updates. this is useful to avoid messing with the beads q
         # until they can be updated
-        dself.q = depend_array(name="q", value=np.zeros(self.n_unique * 3))
-        dself.g = depend_array(
+        self._q = depend_array(name="q", value=np.zeros(self.n_unique * 3))
+        self._g = depend_array(
             name="g",
             value=np.zeros(self.ncons),
             func=self.gfunc,
-            dependencies=[dself.q],
+            dependencies=[self._q],
         )
 
         # The gradient of the constraint function is computed at the configuration
         # obtained from the previous converged SHAKE step; this array holds
         # a local copy of that configuration
-        dself.qprev = depend_array(name="qprev", value=np.zeros(self.n_unique * 3))
+        self._qprev = depend_array(name="qprev", value=np.zeros(self.n_unique * 3))
 
-        dself.Dg = depend_array(
+        self._Dg = depend_array(
             name="Dg",
             value=np.zeros((self.ncons, self.n_unique * 3)),
             func=self.Dgfunc,
-            dependencies=[dself.qprev],
+            dependencies=[self._qprev],
         )
-        dself.Gram = depend_array(
+        self._Gram = depend_array(
             name="Gram",
             value=np.zeros((self.ncons, self.ncons)),
             func=self.Gfunc,
-            dependencies=[dself.Dg],
+            dependencies=[self._Dg],
         )
         if spla is None:
-            dself.GramChol = depend_array(
+            self._GramChol = depend_array(
                 name="GramChol",
                 value=np.zeros((self.ncons, self.ncons)),
                 func=self.GCfunc,
-                dependencies=[dself.Gram],
+                dependencies=[self._Gram],
             )
         else:
             # scipy cho_factor returns both c and lower, so we need to have a depend tuple
-            dself.GramChol = depend_value(
-                name="GramChol", value=(), func=self.GCfunc, dependencies=[dself.Gram]
+            self._GramChol = depend_value(
+                name="GramChol", value=(), func=self.GCfunc, dependencies=[self._Gram]
             )
 
     def gfunc(self):
         """Calculates the value of the constraint(s)"""
         raise NotImplementedError()
 
     def Dgfunc(self):
@@ -154,14 +153,17 @@
         def GCfunc(self):
             """Computes a cholesky decomposition of the mass-scaled Jacobian,
             used in a few places"""
 
             return spla.cho_factor(self.Gram)
 
 
+dproperties(ConstraintBase, ["m3", "q", "g", "qprev", "Dg", "Gram", "GramChol"])
+
+
 class ValueConstraintBase(ConstraintBase):
     """Base class for a constraint that contains target values."""
 
     def __init__(self, constrained_indices, constraint_values, ncons):
         """Initialize the constraint.
 
         constrained_indices: Indices of the atoms that are involved in the constraint
@@ -171,34 +173,36 @@
         """
 
         # NB: if constraint_values are not provided, it will
         #     use the *initial* values of the constraints to initialize values
         if len(constraint_values) != 0:
             self.ncons = len(constraint_values)
             self._calc_cons = False
-            dd(self).constraint_values = depend_array(
+            self._constraint_values = depend_array(
                 name="constraint_values", value=np.asarray(constraint_values).copy()
             )
         elif ncons != 0:
             self.ncons = ncons
             self._calc_cons = True
-            dd(self).constraint_values = depend_array(
+            self._constraint_values = depend_array(
                 name="constraint_values", value=np.zeros(ncons)
             )
         else:
             raise ValueError("cannot determine the number of constraints in list")
 
         super(ValueConstraintBase, self).__init__(constrained_indices, ncons)
 
     def bind(self, beads):
         super(ValueConstraintBase, self).bind(beads)
 
-        dself = dd(self)
-        dself.g.add_dependency(dself.constraint_values)
-        dself.Dg.add_dependency(dself.constraint_values)
+        self._g.add_dependency(self._constraint_values)
+        self._Dg.add_dependency(self._constraint_values)
+
+
+dproperties(ValueConstraintBase, ["constraint_values"])
 
 
 class RigidBondConstraint(ValueConstraintBase):
     """Constraint class for MD.
     Specialized for rigid bonds. This can actually hold a *list*
     of rigid bonds, i.e. there will be a list of pairs of atoms and
     a list of bond lengths."""
@@ -329,81 +333,80 @@
     Unlike the constraints above, a single instance of this class can only
     describe one set of Eckart conditions.
     """
 
     def __init__(self, constrained_indices, constraint_values):
         super(EckartConstraint, self).__init__(constrained_indices, 6)
         self.constrained_indices.shape = -1
-        dd(self).constraint_values = depend_array(
+        self._constraint_values = depend_array(
             name="constraint_values", value=np.zeros(self.ncons)
         )
 
         # Check that there are no repeats
         if np.any(self.constrained_indices != self.i_unique):
             raise ValueError("repeated atom indices in EckartConstraint")
         self.i3_indirect.shape = (-1, 3)
         if len(constraint_values) == 0:
             self._calc_cons = True
-            dd(self).qref = depend_array(
+            self._qref = depend_array(
                 name="qref", value=np.zeros_like(self.i3_indirect, float)
             )
         else:
             self._calc_cons = False
-            dd(self).qref = depend_array(
+            self._qref = depend_array(
                 name="qref",
                 value=np.reshape(constraint_values, self.i3_indirect.shape).copy(),
             )
 
     def bind(self, beads):
         super(EckartConstraint, self).bind(beads)
         if self._calc_cons:
             self.qref[:] = dstrip(beads.q[0])[self.i3_unique].reshape((-1, 3))
-        dself = dd(self)
-        dself.g.add_dependency(dself.constraint_values)
-        dself.Dg.add_dependency(dself.constraint_values)
+        self._g.add_dependency(self._constraint_values)
+        self._Dg.add_dependency(self._constraint_values)
 
         # Total mass of the group of atoms
-        dself.mtot = depend_value(
+        self._mtot = depend_value(
             name="mtot",
             value=1.0,
             func=(lambda: dstrip(self.m3)[::3].sum()),
-            dependencies=[dself.m3],
+            dependencies=[self._m3],
         )
 
         # Coords of reference centre of mass
-        dself.qref_com = depend_array(
+        self._qref_com = depend_array(
             name="qref_com",
             value=np.zeros(3, float),
             func=(
                 lambda: np.sum(
                     dstrip(self.qref) * dstrip(self.m3).reshape((-1, 3)), axis=0
                 )
                 / self.mtot
             ),
-            dependencies=[dself.m3, dself.qref],
+            dependencies=[self._m3, self._qref],
         )
         # qref in its centre of mass frame
-        dself.qref_rel = depend_array(
+        self._qref_rel = depend_array(
             name="qref_rel",
             value=np.zeros_like(dstrip(self.qref)),
             func=(lambda: dstrip(self.qref) - dstrip(self.qref_com)),
-            dependencies=[dself.qref, dself.qref_com],
+            dependencies=[self._qref, self._qref_com],
         )
         # qref in the CoM frame, mass-weighted
-        dself.mqref_rel = depend_array(
+        self._mqref_rel = depend_array(
             name="mqref_rel",
             value=np.zeros_like(dstrip(self.qref)),
             func=(lambda: dstrip(self.qref_rel) * dstrip(self.m3).reshape((-1, 3))),
-            dependencies=[dself.qref_rel, dself.m3],
+            dependencies=[self._qref_rel, self._m3],
         )
         # Make constraint function and gradient depend on the parameters
-        dself.g.add_dependency(dself.qref)
-        dself.g.add_dependency(dself.m3)
-        dself.Dg.add_dependency(dself.qref)
-        dself.Dg.add_dependency(dself.m3)
+        self._g.add_dependency(self._qref)
+        self._g.add_dependency(self._m3)
+        self._Dg.add_dependency(self._qref)
+        self._Dg.add_dependency(self._m3)
 
     def gfunc(self):
         """
         Calculates the constraint.
         """
 
         q = dstrip(self.q).reshape((-1, 3))
@@ -435,14 +438,17 @@
         r[5, :, 0] = -mqref_rel[:, 1]
         r[5, :, 1] = mqref_rel[:, 0]
         r /= self.mtot
         r.shape = (self.ncons, -1)
         return r
 
 
+dproperties(EckartConstraint, ["mtot", "qref", "qref_com", "qref_rel", "mqref_rel"])
+
+
 class ConstraintList(ConstraintBase):
     """Class to hold a list of constraints to be treated
     simultaneously by the solver."""
 
     def __init__(self, constraint_list):
         """Initialize the constraint list.
         Contains a list of constraint objects, that will
@@ -475,34 +481,33 @@
     def bind(self, beads):
         super(ConstraintList, self).bind(beads)
 
         # we link all of the sub-constraints to the lists of unique q and qprev,
         # so that each constraint gets automatically updated. This involves
         # defining a function that transfer q and qprev to the individual
         # constraints, and setting dependencies appropriately
-        dself = dd(self)
 
         def make_qgetter(k):
             return lambda: self.q[self.ic3_map[k]]
 
         def make_qprevgetter(k):
             return lambda: self.qprev[self.ic3_map[k]]
 
         for ic, c in enumerate(self.constraint_list):
             c.bind(beads)
             # deal with constraint functions
-            dq = dd(c).q
-            dq.add_dependency(dself.q)
+            dq = c._q
+            dq.add_dependency(self._q)
             dq._func = make_qgetter(ic)
-            dself.g.add_dependency(dd(c).g)
+            self._g.add_dependency(c._g)
             # ...and their gradients
-            dqprev = dd(c).qprev
-            dqprev.add_dependency(dself.qprev)
+            dqprev = c._qprev
+            dqprev.add_dependency(self._qprev)
             dqprev._func = make_qprevgetter(ic)
-            dself.Dg.add_dependency(dd(c).Dg)
+            self._Dg.add_dependency(c._Dg)
 
     def gfunc(self):
         """
         Compute the constraint function.
         """
         r = np.zeros(self.ncons)
         si = 0
@@ -524,7 +529,10 @@
         return r
 
     def get_iai(self):
         iai = []
         for constr in self.constraint_list:
             iai += list(constr.get_iai())
         return np.unique(iai)
+
+
+dproperties(ConstraintList, ["dq", "dqprev"])
```

### Comparing `ipi-2.6.0/ipi/utils/depend.py` & `ipi-2.6.3/ipi/utils/depend.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 from ipi.utils.messages import verbosity, warning
 
 
 __all__ = [
     "depend_value",
     "depend_array",
     "synchronizer",
-    "dobject",
-    "dd",
     "dpipe",
     "dcopy",
     "dstrip",
     "depraise",
+    "dproperties",
+    "ddot",
+    "noddot",
 ]
 
 
 class synchronizer(object):
-
     """Class to implement synched objects.
 
     Holds the objects used to keep two or more objects in step with each other.
     This is shared between all the synched objects.
 
     Attributes:
         synched: A dictionary containing all the synched objects, of the form
@@ -75,15 +75,14 @@
             self.synced = deps
 
         self.manual = None
 
 
 # TODO put some error checks in the init to make sure that the object is initialized from consistent synchro and func states
 class depend_base(object):
-
     """Base class for dependency handling.
 
     Builds the majority of the machinery required for the different depend
     objects. Contains functions to add and remove dependencies, the tainting
     mechanism by which information about which objects have been updated is
     passed around the dependency network, and the manual and automatic update
     functions to check that depend objects with functions are not manually
@@ -106,15 +105,14 @@
         self,
         name,
         synchro=None,
         func=None,
         dependants=None,
         dependencies=None,
         tainted=None,
-        active=None,
     ):
         """Initialises depend_base.
 
         An unusual initialisation routine, as it has to be able to deal with
         the depend array mechanism for returning slices as new depend arrays.
 
         This is the reason for the penultimate if statement; it automatically
@@ -134,31 +132,26 @@
                 form {"name": function name}; where "name" is one of the other
                 synched objects and function name is the name of a function to
                 get the object "name" from self.
             synchro: An optional synchronizer object.
             dependants: An optional list containing objects that depend on self.
             dependencies: An optional list containing objects that self
                 depends upon.
-            active: An optional boolean to indicate if this object is evaluated
-                (is active) or on hold.
         """
 
         if tainted is None:
             tainted = np.array([True], bool)
-        if active is None:
-            active = np.array([True], bool)
         if dependants is None:
             dependants = []
         if dependencies is None:
             dependencies = []
 
         self._tainted = tainted
         self._func = func
         self._name = name
-        self._active = active
         self._threadlock = threading.RLock()
         self._dependants = []
         self._synchro = None
 
         self.add_synchro(synchro)
 
         for item in dependencies:
@@ -187,26 +180,14 @@
         for member in newone.__dict__:
             if member == "_threadlock":
                 continue
             setattr(newone, member, deepcopy(getattr(self, member), memo))
 
         return newone
 
-    def hold(self):
-        """Sets depend object as on hold."""
-        self._active[:] = False
-
-    def resume(self):
-        """Sets depend object as active again."""
-        self._active[:] = True
-        if self._func is None:
-            self.taint(taintme=False)
-        else:
-            self.taint(taintme=True)
-
     def add_synchro(self, synchro=None):
         """Links depend object to a synchronizer."""
 
         assert (
             self._synchro is None
         ), "This object must not have a previous synchronizer!"
 
@@ -253,29 +234,34 @@
         other.
 
         Args:
            taintme: A boolean giving whether self should be tainted at the end.
               True by default.
         """
 
-        if not self._active:
-            return
-
-        self._tainted[:] = True
+        # propagates dependency
         for item in self._dependants:
             item = item()
             if not item._tainted[0]:
                 item.taint()
-        if self._synchro is not None:
-            for v in list(self._synchro.synced.values()):
-                if (not v._tainted[0]) and (v is not self):
-                    v.taint(taintme=True)
-            self._tainted[:] = taintme and (not self._name == self._synchro.manual)
+
+        if self._synchro is None:
+            self._tainted[0] = taintme
         else:
-            self._tainted[:] = taintme
+            self._tainted[0] = False
+            for v in self._synchro.synced.values():
+                if not v._tainted[0]:
+                    v._tainted[0] = v._name != self._synchro.manual
+                    # do the propagation on the dependants here
+                    # so we don't iterate multiple times over synchro
+                    for item in v._dependants:
+                        item = item()
+                        if not item._tainted[0]:
+                            item.taint()
+            self._tainted[0] = taintme and (not self._name == self._synchro.manual)
 
     def tainted(self):
         """Returns tainted flag."""
 
         return self._tainted[0]
 
     def update_auto(self):
@@ -328,15 +314,14 @@
     def get(self):
         """Dummy getting routine."""
 
         raise ValueError("Undefined get function for base depend class")
 
 
 class depend_value(depend_base):
-
     """Depend class for scalar values.
 
     Attributes:
         _value: The value associated with self.
     """
 
     def __init__(
@@ -344,15 +329,14 @@
         name,
         value=None,
         synchro=None,
         func=None,
         dependants=None,
         dependencies=None,
         tainted=None,
-        active=None,
     ):
         """Initialises depend_value.
 
         Args:
             name: A string giving the name of self.
             value: The value of the object. Optional.
             tainted: An optional array giving the tainted flag. Default is [True].
@@ -365,58 +349,55 @@
             dependants: An optional list containing objects that depend on self.
             dependencies: An optional list containing objects that self
                 depends upon.
         """
 
         self._value = value
         super(depend_value, self).__init__(
-            name, synchro, func, dependants, dependencies, tainted, active
+            name, synchro, func, dependants, dependencies, tainted
         )
 
     def get(self):
-        """Returns value, after recalculating if necessary.
+        """Returns value, after recalculating if necessary."""
 
-        Overwrites the standard method of getting value, so that value
-        is recalculated if tainted.
+        return self.__get__(self, self.__class__)
+
+    def __get__(self, instance=None, owner=None):
+        """Overwrites standard get function
+
+        Returns a cached value, recomputing only if the value is tainted.
         """
 
-        with self._threadlock:
-            if self._tainted[0]:
+        if self._tainted[0]:
+            with self._threadlock:
                 self.update_auto()
                 self.taint(taintme=False)
 
         return self._value
 
-    def __get__(self, instance, owner):
-        """Overwrites standard get function."""
-
-        return self.get()
-
     def set(self, value, manual=True):
         """Alters value and taints dependencies.
 
         Overwrites the standard method of setting value, so that dependent
         quantities are tainted, and so we check that computed quantities are not
         manually updated.
         """
 
         with self._threadlock:
             self._value = value
-            # self.taint(taintme=False)
             if manual:
                 self.update_man()
 
     def __set__(self, instance, value):
         """Overwrites standard set function."""
 
         self.set(value)
 
 
 class depend_array(np.ndarray, depend_base):
-
     """Depend class for arrays.
 
     Differs from depend_value as arrays handle getting items in a different
     way to scalar quantities, and as there needs to be support for slicing an
     array. Initialisation is also done in a different way for ndarrays.
 
     Attributes:
@@ -430,15 +411,14 @@
         name,
         synchro=None,
         func=None,
         dependants=None,
         dependencies=None,
         tainted=None,
         base=None,
-        active=None,
     ):
         """Creates a new array from a template.
 
         Called whenever a new instance of depend_array is created. Casts the
         array base into an appropriate form before passing it to
         __array_finalize__().
 
@@ -455,15 +435,14 @@
         name,
         synchro=None,
         func=None,
         dependants=None,
         dependencies=None,
         tainted=None,
         base=None,
-        active=None,
     ):
         """Initialises depend_array.
 
         Note that this is only called when a new array is created by an
         explicit constructor.
 
         Args:
@@ -478,15 +457,15 @@
             synchro: An optional synchronizer object.
             dependants: An optional list containing objects that depend on self.
             dependencies: An optional list containing objects that self
                 depends upon.
         """
 
         super(depend_array, self).__init__(
-            name, synchro, func, dependants, dependencies, tainted, active
+            name, synchro, func, dependants, dependencies, tainted
         )
 
         if base is None:
             self._bval = value
         else:
             self._bval = base
 
@@ -524,15 +503,14 @@
                 super(depend_array, self).__init__(
                     obj._name,
                     obj._synchro,
                     obj._func,
                     obj._dependants,
                     None,
                     obj._tainted,
-                    obj._active,
                 )
                 self._bval = obj._bval
         else:
             # Most likely we came here on the way to init.
             # Just sets a defaults for safety
             self._bval = dstrip(self)
 
@@ -598,15 +576,14 @@
             dstrip(self).reshape(newshape),
             name=self._name,
             synchro=self._synchro,
             func=self._func,
             dependants=self._dependants,
             tainted=self._tainted,
             base=self._bval,
-            active=self._active,
         )
 
     def flatten(self):
         """Makes the base array one dimensional.
 
         Returns:
             A flattened array.
@@ -653,51 +630,42 @@
         so without depend machinery. If you need a "scalar depend" which
         behaves as a slice, just create a 1x1 matrix, e.g b=a(7,1:2)
 
         Args:
            index: A slice variable giving the appropriate slice to be read.
         """
 
-        with self._threadlock:
-            if self._tainted[0]:
+        if self._tainted[0]:
+            with self._threadlock:
                 self.update_auto()
                 self.taint(taintme=False)
 
         if self.__scalarindex(index, self.ndim):
-            return dstrip(self)[index]
+            return self.view(np.ndarray)[index]
         else:
-            return depend_array(
-                dstrip(self)[index],
-                name=self._name,
-                synchro=self._synchro,
-                func=self._func,
-                dependants=self._dependants,
-                tainted=self._tainted,
-                base=self._bval,
-                active=self._active,
-            )
+            return super(depend_array, self).__getitem__(index)
 
     def __getslice__(self, i, j):
         """Overwrites standard get function."""
 
         return self.__getitem__(slice(i, j, None))
 
     def get(self):
         """Alternative to standard get function."""
 
         return self.__getitem__(slice(None, None, None))
 
-    def __get__(self, instance, owner):
+    def __get__(self, instance=None, owner=None):
         """Overwrites standard get function."""
 
         # It is worth duplicating this code that is also used in __getitem__ as this
         # is called most of the time, and we avoid creating a load of copies pointing to the same depend_array
 
-        with self._threadlock:
-            if self._tainted[0]:
+        if self._tainted[0]:
+            with self._threadlock:
                 self.update_auto()
                 self.taint(taintme=False)
 
         return self
 
     def __setitem__(self, index, value, manual=True):
         """Alters value[index] and taints dependencies.
@@ -749,25 +717,28 @@
 # np.dot and other numpy.linalg functions have the nasty habit to
 # view cast to generate the output. Since we don't want to pass on
 # dependencies to the result of these functions, and we can't use
 # the ufunc mechanism to demote the class type to ndarray, we must
 # overwrite np.dot and other similar functions.
 
 # ** np.dot
-__dp_dot = np.dot
+noddot = np.dot
 
 
-def dep_dot(da, db):
+def ddot(da, db):
     a = dstrip(da)
     b = dstrip(db)
 
-    return __dp_dot(a, b)
+    return noddot(a, b)
 
 
-np.dot = dep_dot
+# activate this to have safe dstripping
+# np.dot = ddot
+# activate this if you want to assume dot will almost always be applied on dstripped vectors
+np.dot = noddot
 
 # ENDS NUMPY FUNCTIONS OVERRIDE
 
 
 def dstrip(da):
     """Removes dependencies from a depend_array.
 
@@ -779,18 +750,18 @@
     Args:
         deparray: A depend_array.
 
     Returns:
         A ndarray with the same value as deparray.
     """
 
-    # only bother to strip dependencies if the array actually IS a depend_array
-    if isinstance(da, depend_array):
+    try:
         return da.view(np.ndarray)
-    else:
+    except:  # TODO: remove all remaining stray dstrip so we don't need to check here
+        warning("dstrip should only be called on `depend_array`s", verbosity.low)
         return da
 
 
 def dpipe(dfrom, dto, item=-1):
     """Synchonizes two depend objects.
 
     Takes two depend objects, and makes one of them depend on the other in such
@@ -800,15 +771,15 @@
 
     Args:
         dfrom: The object that is depend on.
         dto: The object that depends on the former one.
     """
 
     if item < 0:
-        dto._func = lambda: dfrom.get()
+        dto._func = lambda: dfrom.__get__(dfrom, dfrom.__class__)
     else:
         dto._func = lambda i=item: dfrom.__getitem__(i)
     dto.add_dependency(dfrom)
 
 
 def dcopy(dfrom, dto):
     """Copies the dependencies of one depend object to another.
@@ -825,98 +796,33 @@
         dto._bval = dfrom._bval
 
 
 def depraise(exception):
     raise exception
 
 
-class dobject(object):
-
-    """Class that allows standard notation to be used for depend objects.
-
-    An extension of the standard library object that overloads __getattribute__
-    and __setattribute__, so that we can use the standard syntax for setting
-    and getting the depend object, i.e. foo = value, not foo.set(value).
-    """
-
-    def __new__(cls, *args, **kwds):
-        """Initialize the object using __new__, because we do not want
-        to impose to derived classes to call the super __init__"""
-
-        obj = object.__new__(cls)
-        obj._direct = ddirect(obj)
-        return obj
-
-    def __getattribute__(self, name):
-        """Overrides standard __getattribute__().
+def _inject_depend_property(cls, attr_name):
+    private_name = f"_{attr_name}"
 
-        This changes the standard __getattribute__() function of any class that
-        subclasses dobject such that depend objects are called with their own
-        __get__() function rather than the standard one.
-        """
+    def getter(self):
+        return getattr(self, private_name).__get__(self, cls)
 
-        value = super(dobject, self).__getattribute__(name)
-        if isinstance(value, depend_base):
-            value = value.__get__(self, self.__class__)
-        return value
+    def setter(self, value):
+        return getattr(self, private_name).__set__(self, value)
 
-    def __setattr__(self, name, value):
-        """Overrides standard __setattribute__().
+    setattr(cls, attr_name, property(getter, setter))
 
-        This changes the standard __setattribute__() function of any class that
-        subclasses dobject such that depend objects are called with their own
-        __set__() function rather than the standard one.
-        """
-
-        try:
-            obj = super(dobject, self).__getattribute__(name)
-        except AttributeError:
-            pass
-        else:
-            if isinstance(obj, depend_base):
-                return obj.__set__(self, value)
-        return super(dobject, self).__setattr__(name, value)
 
-    def __deepcopy__(self, memo):
-        """Overrides deepcopy behavior, so that _direct is not actually copied
-        but linked to a ddirect object"""
-
-        newone = type(self)()
-
-        for member in newone._direct.__dict__:
-            if member == "_direct":  # do not overwrite direct accessor
-                continue
-            setattr(
-                newone._direct, member, deepcopy(getattr(self._direct, member), memo)
-            )
-        return newone
-
-
-def dd(dobj):
-    if not isinstance(dobj, dobject):
-        raise ValueError(
-            "Cannot access a ddirect view of an object which is not a subclass of dobject"
-        )
-    return dobj._direct
-
-
-class ddirect(object):
-
-    """Gives a "view" of a depend object where one can directly access its
-    depend_base members."""
-
-    def __init__(self, dobj):
-        """Just stores a reference to the dobject we want to access"""
-
-        object.__setattr__(self, "dobj", dobj)
-
-    def __getattribute__(self, name):
-        """Overrides the dobject value access mechanism and returns the actual
-        member objects."""
-
-        return object.__getattribute__(object.__getattribute__(self, "dobj"), name)
+def dproperties(cls, attr_names):
+    """
+    Adds to a class property wrappers to access its depend members.
+    Assumes that depend objects are named with an underscore prefix, and
+    creates getters and setters with the given names.
 
-    def __setattr__(self, name, value):
-        """Overrides the dobject value access mechanism and returns the actual
-        member objects."""
+    If a class `A` contains a `_val` depend object, one should use
+    `dproperties(A, ["val"])`.
+    """
+    if not isinstance(attr_names, list):
+        attr_names = [attr_names]
 
-        return object.__setattr__(object.__getattribute__(self, "dobj"), name, value)
+    for attr_name in attr_names:
+        _inject_depend_property(cls, attr_name)
```

### Comparing `ipi-2.6.0/ipi/utils/distance.py` & `ipi-2.6.3/ipi/utils/distance.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/hesstools.py` & `ipi-2.6.3/ipi/utils/hesstools.py`

 * *Files 21% similar despite different names*

```diff
@@ -172,38 +172,45 @@
             return d, w, np.prod(I)
         else:
             return d, w, 1.0
     else:
         return d, w
 
 
-def get_hessian(gm, x0, natoms, nbeads=1, fixatoms=[], d=0.001):
+def get_hessian(
+    gm, x0, natoms, nbeads=1, fixatoms=[], d=0.001, new_disc=False, friction=False
+):
     """Compute the physical hessian given a function to evaluate energy and forces (gm).
     The intermediate steps are written as a temporary files so the full hessian calculations is only ONE step.
 
     IN     gm       = gradient mapper
            x0       = position vector
            natoms   = number of atoms
            nbeads   = number of beads
            fixatoms = indexes of fixed atoms
            d        = displacement
 
     OUT    h       = physical hessian ( (natoms-len(fixatoms) )*3 , nbeads*( natoms-len(fixatoms) )*3)
     """
 
-    # TODO What about the case you have numerical gradients?
-
     info(" @get_hessian: Computing hessian", verbosity.low)
-    ii = (natoms - len(fixatoms)) * 3
+    fixdofs = list()
+    for i in fixatoms:
+        fixdofs.extend([3 * i, 3 * i + 1, 3 * i + 2])
+    ii = natoms * 3
+    activedof = np.delete(np.arange(ii), fixdofs)
+    ncalc = ii - len(fixdofs)
     if x0.size != natoms * 3 * nbeads:
         raise ValueError(
             "The position vector is not consistent with the number of atoms/beads."
         )
 
     h = np.zeros((ii, ii * nbeads), float)
+    if friction:
+        eta_h = np.zeros((nbeads, ii, ii, ii), float)
 
     # Check if there is a temporary file:
     i0 = -1
 
     for i in range(ii, -1, -1):
         try:
             b = np.loadtxt("hessian_" + str(i) + ".tmp")
@@ -215,36 +222,84 @@
             print(("We have found a temporary file ( hessian_" + str(i) + ".tmp). "))
             if (
                 b.shape == h.shape
             ):  # Check that the last temporary file was properly written
                 break
             else:
                 continue
+    if friction:
+        for i in range(ii, -1, -1):
+            try:
+                b = np.loadtxt("hessianEta_" + str(i) + ".tmp")
+            except IOError:
+                pass
+            else:
+                eta_h[:] = b.reshape((nbeads, ii, ii, ii))
+                i0 = i
+                print(
+                    (
+                        "We have found a temporary file ( hessianEta_"
+                        + str(i)
+                        + ".tmp). "
+                    )
+                )
+                if (
+                    b.shape == eta_h.shape
+                ):  # Check that the last temporary file was properly written
+                    break
+                else:
+                    continue
 
     # Start calculation:
     for j in range(i0 + 1, ii):
-        info(
-            " @get_hessian: Computing hessian: %d of %d" % ((j + 1), ii), verbosity.low
-        )
-        x = x0.copy()
-
-        x[:, j] = x0[:, j] + d
-        e, f1 = gm(x, new_disc=False)
-        x[:, j] = x0[:, j] - d
-        e, f2 = gm(x, new_disc=False)
-        g = (f1 - f2) / (2 * d)
-
-        h[j, :] = g.flatten()
-
-        f = open("hessian_" + str(j) + ".tmp", "w")
-        np.savetxt(f, h)
-        f.close()
+        if j in fixdofs:
+            continue
+        else:
+            ndone = len(activedof[activedof < j])
+            info(
+                " @get_hessian: Computing hessian: %d of %d" % (ndone + 1, ncalc),
+                verbosity.low,
+            )
+            x = x0.copy()
+
+            # PLUS
+            x[:, j] = x0[:, j] + d
+            e, f1 = gm(x, new_disc)
+            if friction:
+                eta1 = gm.eta
+
+            # Minus
+            x[:, j] = x0[:, j] - d
+            e, f2 = gm(x, new_disc)
+            if friction:
+                eta2 = gm.eta
+
+            # COMBINE
+            g = (f1 - f2) / (2 * d)
+            h[j, :] = g.flatten()
+            f = open("hessian_" + str(j) + ".tmp", "w")
+            np.savetxt(f, h)
+            f.close()
+
+            if friction:
+                eta_h[:, :, :, j] = (eta1 - eta2) / (2 * d)
+                f = open("hessianEta_" + str(j) + ".tmp", "w")
+                np.savetxt(f, eta_h.flatten())
+                f.close()
 
     u, g = gm(x0)  # Keep the mapper updated
 
     for i in range(ii):
         try:
+            os.remove("hessianEta_" + str(i) + ".tmp")
+        except OSError:
+            pass
+
+        try:
             os.remove("hessian_" + str(i) + ".tmp")
         except OSError:
             pass
 
-    return h
+    if not friction:
+        return h
+    else:
+        return h, eta_h
```

### Comparing `ipi-2.6.0/ipi/utils/inputvalue.py` & `ipi-2.6.3/ipi/utils/inputvalue.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     "InputAttribute",
     "InputArray",
     "input_default",
 ]
 
 
 class input_default(object):
-
     """Contains information required to dynamically create objects.
 
     Used so that we can define mutable default input values to various tags
     without the usual trouble with having a class object that is also mutable,
     namely that all members of that class share the same mutable object, so that
     changing it for one instance of that class changes it for all others. It
     does this by not holding the mutable default value, but instead the
@@ -77,15 +76,14 @@
         # **kwargs unpacks the dictionary, and is used for keyword arguments
         self.factory = factory
         self.args = args
         self.kwargs = kwargs
 
 
 class Input(object):
-
     """Base class for input handling.
 
     Has the generic methods for dealing with the xml input file. Parses the input
     data, outputs the output data, and deals with storing and returning the
     data obtained during the simulation for the restart files.
 
     Attributes:
@@ -871,15 +869,14 @@
                 rstr += dummy_obj.help_rst(f, lindent + indent, level + 1, stop_level)
 
         rstr += "\n"
         return rstr
 
 
 class InputDictionary(Input):
-
     """Class that returns the value of all the fields as a dictionary."""
 
     def __init__(
         self, help=None, default=None, dtype=str, options=None, dimension=None
     ):
         """Allows one to introduce additional (homogeneous) fields during initialization"""
 
@@ -938,15 +935,14 @@
         rdic = {}
         for f, v in self.instancefields.items():
             rdic[f] = self.__dict__[f].fetch()
         return rdic
 
 
 class InputAttribute(Input):
-
     """Class for handling attribute data.
 
     Has the methods for dealing with attribute data of the form:
     <tag_name attrib='data'> ..., where data is just a value. Takes the data and
     converts it to the required data_type, so that it can be used in the
     simulation.
 
@@ -1041,15 +1037,14 @@
            A string giving the stored value in the appropriate format.
         """
 
         return name + "='" + write_type(self.type, self.value) + "'"
 
 
 class InputValue(InputAttribute):
-
     """Class for handling scalar input.
 
     Has the methods for dealing with simple data tags of the form:
     <tag_name> data </tag_name>, where data is just a value. Takes the data and
     converts it to the required data_type, so that it can be used in the
     simulation.
 
@@ -1178,15 +1173,14 @@
         self.value = xml_write(xml, text=text)
 
 
 ELPERLINE = 5
 
 
 class InputArray(InputValue):
-
     """Class for handling array input.
 
     Has the methods for dealing with simple data tags of the form:
     <tag_name shape="(shape)"> data </tag_name>, where data is an array
     of the form [data[0], data[1], ... , data[length]].
 
     Takes the data and converts it to the required data type,
```

### Comparing `ipi-2.6.0/ipi/utils/io/__init__.py` & `ipi-2.6.3/ipi/utils/io/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 
 import sys
 import os
 import io
+import json
 import numpy as np
 
 from ipi.utils.messages import info, verbosity
 from ipi.utils.units import unit_to_user
 from ipi.external import importlib
 from ipi.utils.decorators import cached
 
@@ -25,14 +26,15 @@
     "io_units",
     "iter_file",
     "print_file_path",
     "print_file",
     "read_file",
     "netstring_encoded_savez",
     "netstring_encoded_loadz",
+    "NumpyEncoder",
 ]
 
 mode_map = {
     "bin": "binary",
 }
 
 
@@ -40,14 +42,27 @@
     "print_path": "print_%s_path",
     "print": "print_%s",
     "read": "read_%s",
     "iter": "iter_%s",
 }
 
 
+class NumpyEncoder(json.JSONEncoder):
+    """Special json encoder for numpy types"""
+
+    def default(self, obj):
+        if isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        elif isinstance(obj, np.ndarray):
+            return obj.tolist()
+        return json.JSONEncoder.default(self, obj)
+
+
 @cached
 def _get_io_function(mode, io):
     """Returns io function with specified mode.
 
     This will be determined on the fly based on file name extension and
     available ipi/utils/io/backends/io_*.py backends.
```

### Comparing `ipi-2.6.0/ipi/utils/io/backends/io_ase.py` & `ipi-2.6.3/ipi/utils/io/backends/io_ase.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/io/backends/io_binary.py` & `ipi-2.6.3/ipi/utils/io/backends/io_binary.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/io/backends/io_json.py` & `ipi-2.6.3/ipi/utils/io/backends/io_json.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/io/backends/io_pdb.py` & `ipi-2.6.3/ipi/utils/io/backends/io_pdb.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/io/backends/io_xyz.py` & `ipi-2.6.3/ipi/utils/io/backends/io_xyz.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/io/inputs/io_xml.py` & `ipi-2.6.3/ipi/utils/io/inputs/io_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     "write_float",
     "write_bool",
     "write_dict",
 ]
 
 
 class xml_node(object):
-
     """Class to handle a particular xml tag.
 
     Tags are generally written in the form
     <tag_name attribs="attrib_data"> main_data </tag_name>. This class holds
     tag_name, attrib_data and main_data separately so they can be used to
     create the objects with the appropriate names and data.
 
@@ -69,15 +68,14 @@
 
         self.attribs = attribs
         self.name = name
         self.fields = fields
 
 
 class xml_handler(ContentHandler):
-
     """Class giving general xml_reading methods.
 
     Uses the standard python xml_reader to read the different kinds of data.
     Keeps track of the heirarchial nature of an xml file by recording the level
     of nesting, so that the correct data and attributes can be associated with
     the correct tag name.
```

### Comparing `ipi-2.6.0/ipi/utils/io/io_units.py` & `ipi-2.6.3/ipi/utils/io/io_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,11 +121,8 @@
     # Return data as i-PI structures
     cell = Cell(cell)
     atoms = Atoms(natoms)
     atoms.q[:] = data
     atoms.names[:] = names
     atoms.m[:] = masses
 
-    return {
-        "atoms": atoms,
-        "cell": cell,
-    }
+    return {"atoms": atoms, "cell": cell, "comment": comment}
```

### Comparing `ipi-2.6.0/ipi/utils/mathtools.py` & `ipi-2.6.3/ipi/utils/mathtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import math
 
 import numpy as np
 
 from ipi.utils.messages import verbosity, warning
 
-
 __all__ = [
     "matrix_exp",
     "stab_cholesky",
     "h2abc",
     "h2abc_deg",
     "abc2h",
     "invert_ut3x3",
@@ -488,7 +487,37 @@
     if x <= 0.08 or x >= 0.92:
         if y > 0:
             z = 1 - x
         else:
             z = x
         k = np.log(-np.log(z))
         return np.sign(y) * np.polyval([c8, c7, c6, c5, c4, c3, c2, c1, c0], k)
+
+
+def LT_friction(freqs, spectral_density_over_w, forceit=False):
+    """Computes laplace transform of an harmonic bath spectral density.
+    spectral_density_over_w ( J(w)/w ) is a provided as a function (spline)
+    For numerical reasons the  spline  expects frequencies in invcm"""
+    import scipy.integrate as integrate
+
+    if freqs[1] < 1e-4 or np.amax(freqs) > 1e4:  # assumes invcm units
+        if not forceit:
+            raise ValueError(
+                "Problem computing laplace transform. freq outside tested region {} {}".format(
+                    freqs[1], np.amax(freqs)
+                )
+            )
+
+    integral = np.zeros(freqs.size)
+    for n, wk in enumerate(freqs):
+        if wk != 0:
+
+            def f(w):
+                return spectral_density_over_w(w) * (wk / (wk**2 + w**2))
+
+            # if np.mod(n,100)==0:
+            #        print('{} over {}'.format(n,freqs.size))
+            integral[n] = integrate.quad(
+                f, 0, np.inf, limit=100000, epsrel=1e-4, epsabs=1e-7
+            )[0]
+
+    return 2 * integral / np.pi
```

### Comparing `ipi-2.6.0/ipi/utils/messages.py` & `ipi-2.6.3/ipi/utils/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 VERB_MEDIUM = 2
 VERB_HIGH = 3
 VERB_DEBUG = 4
 VERB_TRACE = 5
 
 
 class Verbosity(object):
-
     """Class used to determine what to print to standard output.
 
     Attributes:
         level: Determines what level of output to print.
     """
 
     lock = False
@@ -104,15 +103,15 @@
     print(
         r"""
  ____       ____       ____       ____
 /    \     /    \     /    \     /    \
 |  #################################  |
 \__#_/     \____/     \____/     \_#__/
    #    _        _______  _____    #
-   #   (_)      |_   __ \|_   _|   #      -*-     v 2.6.0  -*-
+   #   (_)      |_   __ \|_   _|   #      -*-     v 2.6.3  -*-
    #   __  ______ | |__) | | |     #
    Y  [  ||______||  ___/  | |     #      A Universal Force Engine
   0 0  | |       _| |_    _| |_    #
    #  [___]     |_____|  |_____|   #
  __#_       ____       ____       _#__
 /  # \     /    \     /    \     / #  \
 |  #################################  |
```

### Comparing `ipi-2.6.0/ipi/utils/mintools.py` & `ipi-2.6.3/ipi/utils/mintools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1528,18 +1528,17 @@
 
     info(" @MINIMIZE: Second L-BFGS loop recursion completed", verbosity.debug)
     info(" @MINIMIZE: Updated search direction", verbosity.debug)
 
     return (x, fx, xi, qlist, glist)
 
 
-def nichols(f0, f1, d, dynmax, m3, big_step, mode=1):
+def nichols(f0, d, dynmax, m3, big_step, mode=1):
     """Find new movement direction. JCP 92,340 (1990)
-    IN    f0      = physical forces        (n,)
-          f1      = spring forces
+    IN    f       = physical + spring forces        (n,)
           d       = dynmax eigenvalues
           dynmax  = dynmax       (n x n-m) with m = # external modes
           m3      = mass vector
     OUT   DX      = displacement in cartesian basis
 
     INTERNAL
           ndim = dimension
@@ -1551,17 +1550,17 @@
           DX   = displacement in cartesian basis
           DXE  = displacement in eigenvector basis
     """
 
     # Resize
     ndim = f0.size
     shape = f0.shape
-    f = (f0 + f1).reshape((1, ndim)) / m3.reshape(
-        (1, ndim)
-    ) ** 0.5  # From cartesian base to mass-weighted base
+    f = (
+        f0.reshape((1, ndim)) / m3.reshape((1, ndim)) ** 0.5
+    )  # From cartesian base to mass-weighted base
 
     # Change of basis to eigenvector space
     d = d[:, np.newaxis]  # dimension nx1
     gEt = -np.dot(f, dynmax)  # Change of basis  #
     gE = gEt.T  # dimension (n-m)x1
     # The step has the general form:
     # d_x[j] =  alpha *( gE[j] )  / ( lambda-d[j] )
```

### Comparing `ipi-2.6.0/ipi/utils/nmtransform.py` & `ipi-2.6.3/ipi/utils/nmtransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # i-PI Copyright (C) 2014-2015 i-PI developers
 # See the "licenses" directory for full license information.
 
 
 import numpy as np
 
 from ipi.utils.depend import dstrip
-from ipi.utils.messages import verbosity, info
+from ipi.utils.messages import verbosity, info, warning
 
 
 __all__ = [
     "nm_noop",
     "nm_trans",
     "nm_rescale",
     "nm_fft",
@@ -154,15 +154,14 @@
         return q
 
     def nm2b(self, qnm):
         return qnm
 
 
 class nm_trans(object):
-
     """Uses matrix multiplication to do normal mode transformations.
 
     Attributes:
        _b2nm: The matrix to transform between the bead and normal mode
           representations.
        _nm2b: The matrix to transform between the normal mode and bead
           representations.
@@ -226,15 +225,14 @@
                     self._o_nm2b, qnm[:, 3 * io + 2], axes=(1, 0)
                 )
 
         return q
 
 
 class nm_rescale(object):
-
     """Uses matrix multiplication to do ring polymer contraction or expansion
     between different numbers of beads.
 
     Attributes:
        _b1tob2: The matrix to transform between a ring polymer with 'nbeads1'
           beads and another with 'nbeads2' beads.
        _b2tob1: The matrix to transform between a ring polymer with 'nbeads2'
@@ -327,15 +325,14 @@
                         q_scal = np.tensordot(self._o_b2tob1, q, axes=(1, 0))
         return q_scal
 
 
 class nm_fft(
     object
 ):  # ! TODO add (matrix-version) of the open path transformation here
-
     """Uses Fast Fourier transforms to do normal mode transformations.
 
     Attributes:
        fft: The fast-Fourier transform function to transform between the
           bead and normal mode representations.
        ifft: The inverse fast-Fourier transform function to transform
           between the normal mode and bead representations.
@@ -343,52 +340,95 @@
           them to the normal mode representation.
        qnmdummy: A matrix to hold a copy of the normal modes to transform
           them to the bead representation.
        nbeads: The number of beads.
        natoms: The number of atoms.
     """
 
-    def __init__(self, nbeads, natoms, open_paths=None):
+    def __init__(
+        self, nbeads, natoms, open_paths=None, n_threads=1, single_precision=False
+    ):
         """Initializes nm_trans.
 
         Args:
            nbeads: The number of beads.
            natoms: The number of atoms.
         """
 
         self.nbeads = nbeads
         self.natoms = natoms
+        self.n_threads = n_threads
+        self.single_precision = single_precision
         if open_paths is None:
             open_paths = []
         self._open = open_paths
         # for atoms with open path we still use the matrix transformation
         self._b2o_nm = mk_o_nm_matrix(nbeads)
         self._o_nm2b = self._b2o_nm.T
         try:
             import pyfftw
 
             info("Import of PyFFTW successful", verbosity.medium)
-            self.qdummy = pyfftw.n_byte_align_empty((nbeads, 3 * natoms), 16, "float32")
+            self.qdummy = pyfftw.n_byte_align_empty(
+                (nbeads, 3 * natoms),
+                16,
+                "float32" if self.single_precision else "float64",
+            )
             self.qnmdummy = pyfftw.n_byte_align_empty(
-                (nbeads // 2 + 1, 3 * natoms), 16, "complex64"
+                (nbeads // 2 + 1, 3 * natoms),
+                16,
+                "complex64" if self.single_precision else "complex128",
             )
-            self.fft = pyfftw.FFTW(
-                self.qdummy, self.qnmdummy, axes=(0,), direction="FFTW_FORWARD"
+
+            pyfftw.config.NUM_THREADS = self.n_threads
+
+            self.pyfftw_fw = pyfftw.FFTW(
+                self.qdummy,
+                self.qnmdummy,
+                axes=(0,),
+                direction="FFTW_FORWARD",
+                threads=self.n_threads,
             )
-            self.ifft = pyfftw.FFTW(
-                self.qnmdummy, self.qdummy, axes=(0,), direction="FFTW_BACKWARD"
+            self.pyfftw_bw = pyfftw.FFTW(
+                self.qnmdummy,
+                self.qdummy,
+                axes=(0,),
+                direction="FFTW_BACKWARD",
+                threads=self.n_threads,
             )
+
+            # wrapping these calls into functions has negligible overhead and makes profiling easier
+            def call_fft(self):
+                self.pyfftw_fw()
+
+            def call_ifft(self):
+                self.pyfftw_bw()
+
+            self.fft = lambda: call_fft(self)
+            self.ifft = lambda: call_ifft(self)
         except ImportError:  # Uses standard numpy fft library if nothing better
             # is available
             info(
-                "Import of PyFFTW unsuccessful, using NumPy library instead",
-                verbosity.medium,
+                "Import of PyFFTW unsuccessful, using NumPy library instead. ",
+                verbosity.low,
+            )
+            if self.nbeads > 1:
+                warning(
+                    "Install PyFFTW to avoid slow normal-modes integration",
+                    verbosity.low,
+                )
+
+            self.qdummy = np.zeros(
+                (nbeads, 3 * natoms),
+                dtype="float32" if self.single_precision else "float64",
+            )
+            self.qnmdummy = np.zeros(
+                (nbeads // 2 + 1, 3 * natoms),
+                dtype="complex64" if self.single_precision else "complex128",
             )
-            self.qdummy = np.zeros((nbeads, 3 * natoms), dtype="float32")
-            self.qnmdummy = np.zeros((nbeads // 2 + 1, 3 * natoms), dtype="complex64")
 
             def dummy_fft(self):
                 self.qnmdummy = np.fft.rfft(self.qdummy, axis=0)
 
             def dummy_ifft(self):
                 self.qdummy = np.fft.irfft(self.qnmdummy, n=self.nbeads, axis=0)
 
@@ -444,44 +484,38 @@
         """Transforms a matrix to the bead representation.
 
         Args:
            qnm: A matrix with nbeads rows and 3*natoms columns,
               in the normal mode representation.
         """
 
-        if self.nbeads == 1:
+        nbeads = self.nbeads
+        if nbeads == 1:
             return qnm
-        if self.nbeads == 2:
+        if nbeads == 2:
             self.qnmdummy[:] = qnm
             self.ifft()
-            return self.qdummy * np.sqrt(self.nbeads)
+            return self.qdummy * np.sqrt(nbeads)
 
-        nmodes = self.nbeads // 2
-        odd = self.nbeads - 2 * nmodes  # 0 if even, 1 if odd
+        nmodes = nbeads // 2
+        odd = nbeads - 2 * nmodes  # 0 if even, 1 if odd
 
-        qnm_complex = np.zeros((nmodes + 1, len(qnm[0, :])), complex)
+        isqrt2 = np.sqrt(0.5)
+        qnm_complex = self.qnmdummy
         qnm_complex[0, :] = qnm[0, :]
         if not odd:
-            (qnm_complex[1:-1, :].real, qnm_complex[1:-1, :].imag) = (
-                qnm[1:nmodes, :],
-                qnm[self.nbeads : nmodes : -1, :],
-            )
-            qnm_complex[1:-1, :] /= np.sqrt(2)
+            qnm_complex[1:-1, :].real = qnm[1:nmodes, :] * isqrt2
+            qnm_complex[1:-1, :].imag = qnm[nbeads:nmodes:-1, :] * isqrt2
             qnm_complex[nmodes, :] = qnm[nmodes, :]
         else:
-            (qnm_complex[1:, :].real, qnm_complex[1:, :].imag) = (
-                qnm[1 : nmodes + 1, :],
-                qnm[self.nbeads : nmodes : -1, :],
-            )
-            qnm_complex[1:, :] /= np.sqrt(2)
+            qnm_complex[1:, :].real = qnm[1 : nmodes + 1, :] * isqrt2
+            qnm_complex[1:, :].imag = qnm[nbeads:nmodes:-1, :] * isqrt2
 
-        self.qnmdummy[:] = qnm_complex
         self.ifft()
-        q = np.zeros(qnm.shape)
-        q = self.qdummy * np.sqrt(self.nbeads)
+        q = self.qdummy * np.sqrt(nbeads)
         for (
             io
         ) in (
             self._open
         ):  # does separately the transformation for the atom that are marked as open paths
             q[:, 3 * io] = np.dot(self._o_nm2b, qnm[:, 3 * io])
             q[:, 3 * io + 1] = np.dot(self._o_nm2b, qnm[:, 3 * io + 1])
```

### Comparing `ipi-2.6.0/ipi/utils/phonontools.py` & `ipi-2.6.3/ipi/utils/phonontools.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/softexit.py` & `ipi-2.6.3/ipi/utils/softexit.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 __all__ = ["Softexit", "softexit"]
 
 
 SOFTEXITLATENCY = 1.0  # seconds to sleep between checking for soft exit
 
 
 class Softexit(object):
-
     """Class to deal with stopping a simulation half way through.
 
     Provides a mechanism to end a simulation from any thread that has
     been properly registered, and to call a series of "emergency" functions
     to try as hard as possible to produce a restartable snapshot of
     the simulation.
     Also, provides a loop to check for soft-exit requests and
```

### Comparing `ipi-2.6.0/ipi/utils/sparse.py` & `ipi-2.6.3/ipi/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/ipi/utils/units.py` & `ipi-2.6.3/ipi/utils/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 from ipi.utils.messages import verbosity, info
 
 
 __all__ = ["Constants", "Elements", "unit_to_internal", "unit_to_user"]
 
 
 class Constants(object):
-
     """Class whose members are fundamental constants.
 
     Attributes:
         kb: Boltzmann constant.
         hbar: Reduced Planck's constant.
         amu: Atomic mass unit.
     """
 
     kb = 1.0
     hbar = 1.0
     amu = 1822.8885
 
 
 class Elements(dict):
-
     """Class which contains the mass of different elements.
 
     Attributes:
         mass_list: A dictionary containing the masses of different elements.
             Has the form {"label": Mass in a.m.u.}. Note that the generic "X"
             label is assumed to be an electron.
     """
```

### Comparing `ipi-2.6.0/ipi.egg-info/PKG-INFO` & `ipi-2.6.3/ipi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipi
-Version: 2.6.0
+Version: 2.6.3
 Summary: A Python interface for ab initio path integral molecular dynamics simulations
 Home-page: http://ipi-code.org
 Author: The i-PI developers
 Author-email: ipi.managers@gmail.com
 Project-URL: Documentation, https://ipi-code.org/i-pi
 Project-URL: Repository, https://github.com/i-pi/i-pi
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,49 +25,45 @@
 License-File: licenses/license_GPL.txt
 License-File: licenses/license_MIT.txt
 Requires-Dist: numpy
 
 i-PI: a Universal Force Engine
 ==============================
 
-A Python interface for ab initio path integral molecular dynamics simulations.
-i-PI is composed of a Python server (i-pi itself, that does not need to be
-compiled but only requires a relatively recent version of Python and Numpy)
-that apply an algorithm that updates the positions of the nuclei, and of an external
-code that acts as a client and computes the electronic energy and forces.
+A Python interface for ab initio path integral molecular dynamics simulations (and more).
+i-PI is a Python server (that does not need to be compiled and only requires a relatively 
+recent version of Python and Numpy) that applies an algorithm to update the positions of 
+the nuclei. One of many compatible external codes acts as client, and computes the 
+electronic energy and forces.
 
 This is typically a patched version of an electronic structure code, but a
 simple self-contained Fortran driver that implements several simple interatomic
 potentials is included for test purposes.
 
 i-PI was originally developed to simulate the quantum mechanical nature of light
 nuclei by performing path integral molecular dynamics simulations,
 and it implements most of the state-of-the-art methods to accelerate this kind of 
 calculations. It has since grown to also provide all sorts of simulation 
 strategies, from replica exchange to geometry optimization. 
 
-Quick Setup and Test
---------------------
+Quick Setup
+-----------
 
-To use i-PI with an existing driver, install and update using Pip:
+To use i-PI with an existing driver, install and update using `pip`:
+
+Last version:
 
-Last version::
 ```bash
 python -m pip install git+https://github.com/i-pi/i-pi.git
 ```
 
-Last Release::
-```bash
-pip install -U i-PI
-```
+Last Release:
 
-Test with Pytest::
 ```bash
-pip install pytest
-pytest --pyargs ipi.tests
+pip install -U ipi
 ```
 
 Full installation
 -----------------
 
 To develop i-PI or test it with the self-contained driver, follow these
 instructions. It is assumed that i-PI will
@@ -82,20 +78,25 @@
 Source the environment settings file `env.sh` as `source env.sh` or `.
 env.sh`.  It is useful to put this in your `.bashrc` or other settings file if
 you always want to have i-PI available.
 
 
 ### Compile the driver code
 
+The built-in driver requires a FORTRAN compiler, and can be built as
+
 ```bash
 cd drivers/f90
 make
 cd ../..
 ```
 
+There is also a Python driver available in `drivers/py`, which however has limited
+functionalities. 
+
 ### Examples and demos
 
 The `examples` and `demos` folders contain inputs for many different types of
 calculations based on i-PI. Examples are typically minimal use-cases of specific
 features, while demos are more structured, tutorial-like examples that show how
 to realize more complex setups, and also provide a brief discussion of the 
 underlying algorithms.
@@ -113,25 +114,26 @@
 i-pi-driver -h localhost -p 31415 -m sg -o 15 &
 i-pi-driver -h localhost -p 31415 -m sg -o 15 &
 tail -f log
 ```
 
 The monitoring can be interrupted with CTRL+C when the run has finished (5000 steps).
 
-
 ### Run the automatic test suite
 
-The automatic test suite can be run by calling the i-pi-test script.
+The automatic test suite can be run by calling the i-pi-tests script.
 You need to have the `pytest` package installed
 
 ```
-i-pi-test
+i-pi-tests
 ```
 
-See more details in the README file inside the ipi_tests folder.
+You may also need to install some dependencies, listed in `requirements.txt`.
+
+See more details in the README file inside the `ipi_tests` folder.
 
 Contributing
 ------------
 
 If you have new features you want to implement into i-PI, your contributions are much welcome.
 See `CONTRIBUTING.md` for a brief set of style guidelines and best practices. Before embarking
 into a substantial project, it might be good to get in touch with the developers, e.g. by opening
```

### Comparing `ipi-2.6.0/ipi.egg-info/SOURCES.txt` & `ipi-2.6.3/ipi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 bin/i-pi
 bin/i-pi-committee-reweight
 bin/i-pi-contract-trajectory
+bin/i-pi-driver-py
 bin/i-pi-get_Ascp
 bin/i-pi-getacf
 bin/i-pi-getproperty
 bin/i-pi-gleacf
 bin/i-pi-kinetic2tag
 bin/i-pi-mergebeadspdb
 bin/i-pi-mux-positions
@@ -19,17 +20,27 @@
 bin/i-pi-remdsort
 bin/i-pi-style
 bin/i-pi-tests
 bin/i-pi-trimsim
 drivers/py/__init__.py
 drivers/py/driver.py
 drivers/py/pes/__init__.py
+drivers/py/pes/ase.py
+drivers/py/pes/bath.py
+drivers/py/pes/doubledoublewell.py
+drivers/py/pes/doublewell.py
+drivers/py/pes/doublewell_with_bath.py
+drivers/py/pes/doublewell_with_friction.py
 drivers/py/pes/dummy.py
 drivers/py/pes/harmonic.py
+drivers/py/pes/mace.py
+drivers/py/pes/metatensor.py
+drivers/py/pes/pet.py
 drivers/py/pes/rascal.py
+drivers/py/pes/spline.py
 ipi/__init__.py
 ipi.egg-info/PKG-INFO
 ipi.egg-info/SOURCES.txt
 ipi.egg-info/dependency_links.txt
 ipi.egg-info/requires.txt
 ipi.egg-info/top_level.txt
 ipi/engine/__init__.py
@@ -122,14 +133,15 @@
 ipi/utils/hesstools.py
 ipi/utils/inputvalue.py
 ipi/utils/instools.py
 ipi/utils/mathtools.py
 ipi/utils/messages.py
 ipi/utils/mintools.py
 ipi/utils/nmtransform.py
+ipi/utils/parsing.py
 ipi/utils/phonontools.py
 ipi/utils/prng.py
 ipi/utils/softexit.py
 ipi/utils/sparse.py
 ipi/utils/units.py
 ipi/utils/io/__init__.py
 ipi/utils/io/io_units.py
@@ -137,23 +149,9 @@
 ipi/utils/io/backends/io_ase.py
 ipi/utils/io/backends/io_binary.py
 ipi/utils/io/backends/io_json.py
 ipi/utils/io/backends/io_pdb.py
 ipi/utils/io/backends/io_xyz.py
 ipi/utils/io/inputs/__init__.py
 ipi/utils/io/inputs/io_xml.py
-ipi_tests/__init__.py
-ipi_tests/test_tools.py
-ipi_tests/regression_tests/__init__.py
-ipi_tests/regression_tests/runstools.py
-ipi_tests/regression_tests/test_run.py
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/files_to_check.txt
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/init.xyz
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/input.xml
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.frc_c.xyz
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.mom_c.xyz
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.out
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.pos_c.xyz
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/ref_simulation.vel_c.xyz
-ipi_tests/regression_tests/tests/NVE/NVE_1/harmonic_python/test_settings.dat
 licenses/license_GPL.txt
 licenses/license_MIT.txt
```

### Comparing `ipi-2.6.0/licenses/license_GPL.txt` & `ipi-2.6.3/licenses/license_GPL.txt`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/licenses/license_MIT.txt` & `ipi-2.6.3/licenses/license_MIT.txt`

 * *Files identical despite different names*

### Comparing `ipi-2.6.0/setup.cfg` & `ipi-2.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ipi
-version = 2.6.0
+version = 2.6.3
 description = A Python interface for ab initio path integral molecular dynamics simulations
 long_description = file: README.md
 long_description_content_type = text/x-rst
 author = The i-PI developers
 author_email = ipi.managers@gmail.com
 url = http://ipi-code.org
 project_urls =
```

