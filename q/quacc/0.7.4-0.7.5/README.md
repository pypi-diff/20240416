# Comparing `tmp/quacc-0.7.4.tar.gz` & `tmp/quacc-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.4.tar", last modified: Fri Apr 12 18:24:01 2024, max compression
+gzip compressed data, was "quacc-0.7.5.tar", last modified: Tue Apr 16 16:09:27 2024, max compression
```

## Comparing `quacc-0.7.4.tar` & `quacc-0.7.5.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.500677 quacc-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-12 18:21:59.000000 quacc-0.7.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 18:21:59.000000 quacc-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-12 18:24:01.500677 quacc-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-12 18:21:59.000000 quacc-0.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-12 18:22:00.000000 quacc-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:24:01.500677 quacc-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.464677 quacc-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.468677 quacc-0.7.4/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.476677 quacc-0.7.4/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.476677 quacc-0.7.4/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.476677 quacc-0.7.4/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.492677 quacc-0.7.4/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.492677 quacc-0.7.4/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.492677 quacc-0.7.4/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.496677 quacc-0.7.4/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.496677 quacc-0.7.4/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.496677 quacc-0.7.4/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.515679 quacc-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-16 16:07:28.000000 quacc-0.7.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 16:07:28.000000 quacc-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-16 16:09:27.515679 quacc-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 16:07:28.000000 quacc-0.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-16 16:07:28.000000 quacc-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:09:27.515679 quacc-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.479679 quacc-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.483679 quacc-0.7.5/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17249 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23055 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.511679 quacc-0.7.5/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.511679 quacc-0.7.5/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.4/LICENSE.md` & `quacc-0.7.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/PKG-INFO` & `quacc-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.4
+Version: 0.7.5
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -30,15 +30,16 @@
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
-Requires-Dist: pymatgen>=2024.4.12
+Requires-Dist: pymatgen>=2024.4.13
+Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
 Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
@@ -90,15 +91,14 @@
 <div align="center">
   <img src=https://github.com/Quantum-Accelerators/quacc/blob/main/docs/images/quacc_logo_wide.png width="300"><br>
 </div>
 
 # `quacc` – The Quantum Accelerator 🦆
 
 [![codecov](https://codecov.io/gh/Quantum-Accelerators/quacc/branch/main/graph/badge.svg?token=OJaOZAH30u&precision=1)](https://codecov.io/gh/Quantum-Accelerators/quacc)
-[![DeepSource](https://app.deepsource.com/gh/Quantum-Accelerators/quacc.svg/?label=active+issues&token=Y1NxOLIuFFEqWdjawIYnJNde)](https://app.deepsource.com/gh/Quantum-Accelerators/quacc/?ref=repository-badge)
 ![Python - Version](https://img.shields.io/pypi/pyversions/quacc)
 ![PyPI - Version](https://img.shields.io/pypi/v/quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/10.5281/zenodo.7720998)
 
 `quacc` is a flexible platform for computational materials science 💎 and quantum chemistry 🧪 that is built for the big data era 🔥. It is maintained by the [Rosen Research Group](https://rosen.cbe.princeton.edu/) at Princeton University.
 
 - `quacc` makes it possible to easily run pre-made [computational materials science workflows](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination thereof.
```

### Comparing `quacc-0.7.4/README.md` & `quacc-0.7.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 <div align="center">
   <img src=https://github.com/Quantum-Accelerators/quacc/blob/main/docs/images/quacc_logo_wide.png width="300"><br>
 </div>
 
 # `quacc` – The Quantum Accelerator 🦆
 
 [![codecov](https://codecov.io/gh/Quantum-Accelerators/quacc/branch/main/graph/badge.svg?token=OJaOZAH30u&precision=1)](https://codecov.io/gh/Quantum-Accelerators/quacc)
-[![DeepSource](https://app.deepsource.com/gh/Quantum-Accelerators/quacc.svg/?label=active+issues&token=Y1NxOLIuFFEqWdjawIYnJNde)](https://app.deepsource.com/gh/Quantum-Accelerators/quacc/?ref=repository-badge)
 ![Python - Version](https://img.shields.io/pypi/pyversions/quacc)
 ![PyPI - Version](https://img.shields.io/pypi/v/quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/10.5281/zenodo.7720998)
 
 `quacc` is a flexible platform for computational materials science 💎 and quantum chemistry 🧪 that is built for the big data era 🔥. It is maintained by the [Rosen Research Group](https://rosen.cbe.princeton.edu/) at Princeton University.
 
 - `quacc` makes it possible to easily run pre-made [computational materials science workflows](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination thereof.
```

#### html2text {}

```diff
@@ -1,17 +1,14 @@
      [https://github.com/Quantum-Accelerators/quacc/blob/main/docs/images/
                              quacc_logo_wide.png]
 # `quacc` â The Quantum Accelerator ð¦ [![codecov](https://codecov.io/gh/
 Quantum-Accelerators/quacc/branch/main/graph/
 badge.svg?token=OJaOZAH30u&precision=1)](https://codecov.io/gh/Quantum-
-Accelerators/quacc) [![DeepSource](https://app.deepsource.com/gh/Quantum-
-Accelerators/quacc.svg/?label=active+issues&token=Y1NxOLIuFFEqWdjawIYnJNde)]
-(https://app.deepsource.com/gh/Quantum-Accelerators/quacc/?ref=repository-
-badge) ![Python - Version](https://img.shields.io/pypi/pyversions/quacc) ![PyPI
-- Version](https://img.shields.io/pypi/v/
+Accelerators/quacc) ![Python - Version](https://img.shields.io/pypi/pyversions/
+quacc) ![PyPI - Version](https://img.shields.io/pypi/v/
 quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F) [![DOI]
 (https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/
 10.5281/zenodo.7720998) `quacc` is a flexible platform for computational
 materials science ð and quantum chemistry ð§ª that is built for the big
 data era ð¥. It is maintained by the [Rosen Research Group](https://
 rosen.cbe.princeton.edu/) at Princeton University. - `quacc` makes it possible
 to easily run pre-made [computational materials science workflows](https://
```

### Comparing `quacc-0.7.4/pyproject.toml` & `quacc-0.7.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.4"
+version = "0.7.5"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -33,15 +33,16 @@
     "emmet-core>=0.80.0", # for pre-made schemas
     "maggma>=0.64.0", # for database handling
     "monty>=2024.2.26", # miscellaneous Python utilities
     "numpy>=1.25.0", # for array handling
     "psutil", # for getting compute architecture details
     "pydantic>=2.0.1", # for settings management
     "pydantic-settings>=2.2.0", # for settings management
-    "pymatgen>=2024.4.12", # for structure manipulation
+    "pymatgen>=2024.4.13", # for structure manipulation
+    "ruamel.yaml>=0.17.40", # for YAML
     "typer>=0.12.1", # for the CLI
 ]
 
 [project.optional-dependencies]
 covalent = ["covalent>=0.234.0rc0", "covalent-cloud>=0.39.0"]
 dask = ["dask[distributed]>=2023.12.1", "dask-jobqueue>=0.8.2"]
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
@@ -115,69 +116,71 @@
   "if TYPE_CHECKING:",
   "if __name__ == .__main__.:",
   "except ImportError:",
 ]
 
 [tool.ruff]
 lint.select = [
+  "A",      # flake8-builtins
+  "ARG",    # flake8-unused-arguments
+  "ASYNC",  # flake8-async
   "B",      # flake8-bugbear
   "C4",     # flake8-comprehensions
+  "DTZ",    # flake8-datetimez
   "E",      # pycodestyle error
   "EXE",    # flake8-executable
   "F",      # pyflakes
   "FA",     # flake8-future-annotations
-  "FBT003", # boolean-positional-value-in-call
   "FLY",    # flynt
   "I",      # isort
   "ICN",    # flake8-import-conventions
+  "INT",    # flake8-gettext
+  "ISC",    # flake8-implicit-str-concat
+  "LOG",    # flake8-logging
+  "NPY",    # numpy-specific rules
   "PD",     # pandas-vet
   "PERF",   # perflint
   "PIE",    # flake8-pie
   "PL",     # pylint
   "PT",     # flake8-pytest-style
-  "PYI",    # flakes8-pyi
+  "PTH",    # flake8-use-pathlib
+  "PYI",    # flake8-pyi
   "Q",      # flake8-quotes
   "RET",    # flake8-return
   "RSE",    # flake8-raise
   "RUF",    # Ruff-specific rules
   "SIM",    # flake8-simplify
   "SLOT",   # flake8-slots
+  "T20",    # flake8-print
   "TCH",    # flake8-type-checking
   "TID",    # flake8-tidy-imports
+  "TRIO",   # flake8-trio
   "UP",     # pyupgrade
   "W",      # pycodestyle warning
   "YTT",    # flake8-2020
 ]
 lint.ignore = [
-  "PLR",    # Design related pylint codes
   "E501",   # Line too long
-  "B028",   # No explicit stacklevel
-  "EM101",  # Exception must not use a string literal
-  "EM102",  # Exception must not use an f-string literal
-  "G004",   # f-string in Logging statement
-  "RUF015", # Prefer next(iter())
-  "RET505", # Unnecessary `elif` after `return`
-  "PT004",  # Fixture does not return anthing
-  "B017",   # pytest.raises
+  "ISC001",   # single-line-implicit-string-concatenation
+  "PLR",    # Design related pylint codes
+  "PERF203",  # try-except-in-loop
+  "PT004",  # Fixture does not return anything
   "PT011",  # pytest.raises
   "PT012",  # pytest.raises
+  "RET505", # Unnecessary `elif` after `return`
 ]
-lint.typing-modules = ["mypackage._compat.typing"]
 src = ["src"]
-lint.unfixable = [
-  "T20",  # Removes print statements
-  "F841", # Removes unused variables
-]
 lint.pydocstyle.convention = "numpy"
 lint.isort.known-first-party = ["quacc"]
 lint.isort.required-imports = ["from __future__ import annotations"]
+extend-include = ["*.ipynb"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
-"tests/**" = ["ANN201", "D", "E402", "S101"]
+"tests/**" = ["ANN", "ARG", "D", "E402", "PTH", "S101"]
 "src/quacc/settings.py" = ["FBT003", "TCH002", "UP007"]
 
 [tool.docformatter]
 pre-summary-newline = true
 black = true
 
 [tool.mypy]
```

### Comparing `quacc-0.7.4/src/quacc/__init__.py` & `quacc-0.7.5/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/_cli/quacc.py` & `quacc-0.7.5/src/quacc/_cli/quacc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     if value:
         rich_print(f"quacc v{__version__}")
         raise typer.Exit
 
 
 @app.callback()
 def main(
-    version: Optional[bool] = typer.Option(  # noqa: UP007
+    version: Optional[bool] = typer.Option(  # noqa: ARG001, UP007
         None,
         "--version",
         "-v",
         help="Show the application's version and exit.",
         callback=callback,
         is_eager=True,
     ),
@@ -77,23 +77,23 @@
     Returns
     -------
     None
     """
     from quacc import SETTINGS
     from quacc.settings import _DEFAULT_CONFIG_FILE_PATH
 
-    CONFIG_FILE = SETTINGS.CONFIG_FILE or _DEFAULT_CONFIG_FILE_PATH
+    config_file = SETTINGS.CONFIG_FILE or _DEFAULT_CONFIG_FILE_PATH
     parameter = parameter.upper()
 
     settings = _type_handler({parameter: new_value})
     new_value = settings[parameter]
     _parameter_handler(parameter, SETTINGS.model_dump(), value=new_value)
 
-    rich_print(f"Setting `{parameter}` to `{new_value}` in {CONFIG_FILE}")
-    _update_setting(parameter, new_value, CONFIG_FILE)
+    rich_print(f"Setting `{parameter}` to `{new_value}` in {config_file}")
+    _update_setting(parameter, new_value, config_file)
 
 
 @app.command()
 def unset(parameter: str) -> None:
     """
     Unset the specified quacc parameter in the quacc configuration file. This command
     will not override any environment variables.
@@ -186,17 +186,17 @@
     config_file
         The path to the configuration file.
 
     Returns
     -------
     None
     """
-    import ruamel.yaml
+    from ruamel.yaml import YAML
 
-    yaml = ruamel.yaml.YAML()
+    yaml = YAML()
     if config_file.exists():
         with config_file.open() as yaml_file:
             yaml_content = yaml.load(yaml_file)
 
         if yaml_content:
             yaml_content.pop(key, None)
             with config_file.open(mode="w") as yaml_file:
```

### Comparing `quacc-0.7.4/src/quacc/atoms/core.py` & `quacc-0.7.5/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/atoms/defects.py` & `quacc-0.7.5/src/quacc/atoms/defects.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,19 +108,19 @@
         defect_entry = _get_defect_entry_from_defect(
             defect=defect,
             defect_supercell=defect_supercell,
             defect_charge=defect_charge,
         )
 
         # Instantiate class to apply rattle and bond distortion to all defects
-        Dist = Distortions([defect_entry])
+        dist = Distortions([defect_entry])
 
         # Apply rattle and bond distortion to all defects
-        defect_dict, distortion_metadata = Dist.apply_distortions()
-        defect_symbol = list(distortion_metadata["defects"].keys())[0]
+        defect_dict, distortion_metadata = dist.apply_distortions()
+        defect_symbol = next(iter(distortion_metadata["defects"].keys()))
         distortion_dict = defect_dict[defect_symbol]["charges"][defect_charge][
             "structures"
         ]["distortions"]
 
         # Make atoms objects and store defect stats
         for distortions, defect_struct in distortion_dict.items():
             final_defect = defect_struct.to_ase_atoms()
```

### Comparing `quacc-0.7.4/src/quacc/atoms/deformation.py` & `quacc-0.7.5/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/atoms/phonons.py` & `quacc-0.7.5/src/quacc/atoms/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/atoms/slabs.py` & `quacc-0.7.5/src/quacc/atoms/slabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,9 +390,9 @@
     Returns
     -------
     np.floating
         The surface energy in eV/A^2.
     """
     alpha = len(slab) / len(bulk)
     cell = slab.get_cell()
-    A = np.linalg.norm(np.cross(cell[0], cell[1]))
-    return (slab_energy - alpha * bulk_energy) / (2 * A)
+    area = np.linalg.norm(np.cross(cell[0], cell[1]))
+    return (slab_energy - alpha * bulk_energy) / (2 * area)
```

### Comparing `quacc-0.7.4/src/quacc/calculators/espresso/espresso.py` & `quacc-0.7.5/src/quacc/calculators/espresso/espresso.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,14 @@
             The `directory` kwarg from the calculator.
 
         Returns
         -------
         dict[str, Any]
             The merged kwargs
         """
-
         os.environ.pop("ESPRESSO_TMPDIR", None)
         os.environ.pop("ESPRESSO_FILDVSCF_DIR", None)
         os.environ.pop("ESPRESSO_FILDRHO_DIR", None)
 
         espresso_outdir = Path(directory).expanduser().resolve()
         outkeys = espresso_prepare_dir(espresso_outdir, self.binary)
```

### Comparing `quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.7.5/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/espresso/utils.py` & `quacc-0.7.5/src/quacc/calculators/espresso/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         The q-point coordinates in QE units
 
     Returns
     -------
     dict
         The dictionary of files to copy
     """
-
     lqdir = ph_input_data["inputph"].get("lqdir", False)
 
     files_to_copy = {
         directory: [
             Path("_ph0", "pwscf.phsave", "control_ph.xml*"),
             Path("_ph0", "pwscf.phsave", "status_run.xml*"),
             Path("_ph0", "pwscf.phsave", "patterns.*.xml*"),
@@ -148,15 +147,14 @@
         The binary to be used for the espresso calculation
 
     Returns
     -------
     dict
         Input data for the espresso calculation
     """
-
     outkeys = {
         "pw": {"control": {"prefix": "pwscf", "outdir": outdir, "wfcdir": Remove}},
         "ph": {
             "inputph": {
                 "prefix": "pwscf",
                 "fildyn": "matdyn",
                 "outdir": outdir,
@@ -213,19 +211,19 @@
 
     Parameters
     ----------
     parameters
         The input data for the espresso calculation
     binary
         The binary to use for the espresso calculation
+
     Returns
     -------
         The modified dictionary
     """
-
     to_copy = []
 
     pw_base = [
         Path("pwscf.save", "charge-density.*"),
         Path("pwscf.save", "data-file-schema.*"),
         Path("pwscf.save", "paw.*"),
     ]
@@ -351,14 +349,13 @@
         The reference dictionary that will remain intact
 
     Returns
     -------
     dict
         The modified dictionary
     """
-
     if "kpts" in reference_dict:
         to_change_dict.pop("kspacing", None)
     if "kspacing" in reference_dict:
         to_change_dict.pop("kpts", None)
 
     return to_change_dict
```

### Comparing `quacc-0.7.4/src/quacc/calculators/qchem/io.py` & `quacc-0.7.5/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/qchem/params.py` & `quacc-0.7.5/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/qchem/qchem.py` & `quacc-0.7.5/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.7.5/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/io.py` & `quacc-0.7.5/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/params.py` & `quacc-0.7.5/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/vasp.py` & `quacc-0.7.5/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.7.5/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/common/defects.py` & `quacc-0.7.5/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/common/elastic.py` & `quacc-0.7.5/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/common/phonons.py` & `quacc-0.7.5/src/quacc/recipes/common/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/common/slabs.py` & `quacc-0.7.5/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/dftb/_base.py` & `quacc-0.7.5/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/dftb/core.py` & `quacc-0.7.5/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/emt/core.py` & `quacc-0.7.5/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/emt/defects.py` & `quacc-0.7.5/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/emt/elastic.py` & `quacc-0.7.5/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/emt/phonons.py` & `quacc-0.7.5/src/quacc/recipes/emt/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/emt/slabs.py` & `quacc-0.7.5/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/espresso/_base.py` & `quacc-0.7.5/src/quacc/recipes/espresso/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,14 @@
         The binary to use.
 
     Returns
     -------
     dict
         Dictionary of files to copy.
     """
-
     if isinstance(copy_files, (str, Path)):
         copy_files = [copy_files]
 
     if isinstance(copy_files, list):
         exact_files_to_copy = prepare_copy_files(calc_params, binary=binary)
         return {source: exact_files_to_copy for source in copy_files}
```

### Comparing `quacc-0.7.4/src/quacc/recipes/espresso/bands.py` & `quacc-0.7.5/src/quacc/recipes/espresso/bands.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/espresso/core.py` & `quacc-0.7.5/src/quacc/recipes/espresso/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     is_metal = check_is_metal(atoms)
 
     calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
     calc_defaults["input_data"]["control"] = {"calculation": "scf"}
 
     return run_and_summarize(
         atoms,
@@ -149,15 +148,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     is_metal = check_is_metal(atoms)
 
     calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
     calc_defaults["input_data"]["control"] = {
         "calculation": "vc-relax" if relax_cell else "relax"
     }
 
@@ -226,15 +224,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     is_metal = check_is_metal(atoms)
 
     calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
     calc_defaults["input_data"]["control"] = {
         "calculation": "scf",
         "tstress": relax_cell,
         "tprnfor": True,
```

### Comparing `quacc-0.7.4/src/quacc/recipes/espresso/dos.py` & `quacc-0.7.5/src/quacc/recipes/espresso/dos.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/espresso/phonons.py` & `quacc-0.7.5/src/quacc/recipes/espresso/phonons.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     return run_and_summarize(
         template=EspressoTemplate("q2r"),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "q2r.x Phonon"},
         copy_files=copy_files,
@@ -187,15 +186,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     return run_and_summarize(
         template=EspressoTemplate("matdyn"),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "matdyn Phonon"},
         copy_files=copy_files,
@@ -532,15 +530,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     return run_and_summarize(
         template=EspressoTemplate("dvscf_q2r"),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "dvscf_q2r Phonon"},
         copy_files=copy_files,
@@ -589,15 +586,14 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-
     return run_and_summarize(
         template=EspressoTemplate("postahc"),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "postahc Phonon"},
         copy_files=copy_files,
```

### Comparing `quacc-0.7.4/src/quacc/recipes/gaussian/_base.py` & `quacc-0.7.5/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/gaussian/core.py` & `quacc-0.7.5/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/gulp/_base.py` & `quacc-0.7.5/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/gulp/core.py` & `quacc-0.7.5/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/lj/core.py` & `quacc-0.7.5/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/mlp/_base.py` & `quacc-0.7.5/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/mlp/core.py` & `quacc-0.7.5/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/mlp/phonons.py` & `quacc-0.7.5/src/quacc/recipes/mlp/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/newtonnet/core.py` & `quacc-0.7.5/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.7.5/src/quacc/recipes/newtonnet/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/onetep/_base.py` & `quacc-0.7.5/src/quacc/recipes/onetep/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/onetep/core.py` & `quacc-0.7.5/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/orca/_base.py` & `quacc-0.7.5/src/quacc/recipes/orca/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/orca/core.py` & `quacc-0.7.5/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/psi4/_base.py` & `quacc-0.7.5/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/psi4/core.py` & `quacc-0.7.5/src/quacc/recipes/psi4/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/qchem/_base.py` & `quacc-0.7.5/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/qchem/core.py` & `quacc-0.7.5/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/qchem/ts.py` & `quacc-0.7.5/src/quacc/recipes/qchem/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/tblite/core.py` & `quacc-0.7.5/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/tblite/phonons.py` & `quacc-0.7.5/src/quacc/recipes/tblite/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/vasp/_base.py` & `quacc-0.7.5/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/vasp/core.py` & `quacc-0.7.5/src/quacc/recipes/vasp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/vasp/mp.py` & `quacc-0.7.5/src/quacc/recipes/vasp/mp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/vasp/qmof.py` & `quacc-0.7.5/src/quacc/recipes/vasp/qmof.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/recipes/vasp/slabs.py` & `quacc-0.7.5/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/runners/ase.py` & `quacc-0.7.5/src/quacc/runners/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     # Perform staging operations
     tmpdir, job_results_dir = calc_setup(atoms, copy_files=copy_files)
 
     # Set defaults
     optimizer_kwargs = recursive_dict_merge(
         {
             "logfile": "-" if SETTINGS.DEBUG else tmpdir / "opt.log",
-            "restart": tmpdir / "opt.pckl",
+            "restart": tmpdir / "opt.json",
         },
         optimizer_kwargs,
     )
     run_kwargs = run_kwargs or {}
 
     # Check if trajectory kwarg is specified
     if "trajectory" in optimizer_kwargs:
```

### Comparing `quacc-0.7.4/src/quacc/runners/phonons.py` & `quacc-0.7.5/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/runners/prep.py` & `quacc-0.7.5/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/runners/thermo.py` & `quacc-0.7.5/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/_aliases/ase.py` & `quacc-0.7.5/src/quacc/schemas/_aliases/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.7.5/src/quacc/schemas/_aliases/atoms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Aliases for type hinting `quacc.schemas.atoms`"""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from quacc.schemas._aliases.emmet import MoleculeMetadata, StructureMetadata
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
     from pymatgen.core.structure import Molecule, Structure
 
 
 class AtomsSchema(StructureMetadata, MoleculeMetadata):
     """Type hint associated with [quacc.schemas.atoms.atoms_to_metadata][]"""
 
     atoms: Atoms
-    atoms_info: dict[str, Any]  # from atoms.info
     structure: Structure  # if atoms.pbc.any()
     molecule: Molecule  # if not atoms.pbc.any()
```

### Comparing `quacc-0.7.4/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.7.5/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.7.5/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.7.5/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.7.5/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/ase.py` & `quacc-0.7.5/src/quacc/schemas/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/atoms.py` & `quacc-0.7.5/src/quacc/schemas/atoms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Schemas for storing metadata about Atoms objects."""
 
 from __future__ import annotations
 
-from copy import deepcopy
 from typing import TYPE_CHECKING
 
 from emmet.core.structure import MoleculeMetadata, StructureMetadata
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from quacc.atoms.core import (
     copy_atoms,
@@ -78,17 +77,14 @@
             mol = AseAtomsAdaptor().get_molecule(atoms, charge_spin_check=False)
             metadata = MoleculeMetadata().from_molecule(mol).model_dump()
             if store_pmg:
                 results["molecule"] = mol
     else:
         metadata = {}
 
-    # Copy the info flags as a separate entry in the DB for easy querying
-    results["atoms_info"] = deepcopy(atoms.info)
-
     # Store Atoms object
     results["atoms"] = atoms
 
     # Combine the metadata and results dictionaries
     atoms_doc_unsorted = metadata | results | additional_fields
 
     return clean_task_doc(atoms_doc_unsorted)
```

### Comparing `quacc-0.7.4/src/quacc/schemas/cclib.py` & `quacc-0.7.5/src/quacc/schemas/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/phonons.py` & `quacc-0.7.5/src/quacc/schemas/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/prep.py` & `quacc-0.7.5/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/schemas/vasp.py` & `quacc-0.7.5/src/quacc/schemas/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/settings.py` & `quacc-0.7.5/src/quacc/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,20 +447,21 @@
             if not v.is_absolute():
                 raise ValueError(f"{v} must be an absolute path.")
             if not v.exists():
                 v.mkdir(parents=True)
         return v
 
     @field_validator("STORE")
+    @classmethod
     def generate_store(cls, v: Union[dict[str, dict[str, Any]], Store]) -> Store:
         """Generate the Maggma store."""
         from maggma import stores
 
         if isinstance(v, dict):
-            store_name = list(v.keys())[0]
+            store_name = next(iter(v.keys()))
             store = getattr(stores, store_name)
 
             return store(**v[store_name])
         else:
             return v
 
     @model_validator(mode="before")
```

### Comparing `quacc-0.7.4/src/quacc/utils/dicts.py` & `quacc-0.7.5/src/quacc/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/utils/files.py` & `quacc-0.7.5/src/quacc/utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from copy import deepcopy
 from datetime import datetime, timezone
 from pathlib import Path
 from random import randint
 from shutil import copy
 from typing import TYPE_CHECKING
 
-import yaml
 from monty.io import zopen
 from monty.os.path import zpath
 from monty.shutil import copy_r, decompress_dir, decompress_file
+from ruamel.yaml import YAML
 
 if TYPE_CHECKING:
     from typing import Any
 
     Filenames = str | Path | list[str | Path]
     SourceDirectory = str | Path
 
@@ -207,16 +207,15 @@
         yaml_path = yaml_path.with_suffix(f"{yaml_path.suffix}.yaml")
 
     if not yaml_path.exists():
         msg = f"Cannot find {yaml_path}"
         raise FileNotFoundError(msg)
 
     # Load YAML file
-    with yaml_path.open() as stream:
-        config = yaml.safe_load(stream)
+    config = YAML().load(yaml_path)
 
     # Inherit arguments from any parent YAML files but do not overwrite those in
     # the child file.
     for config_arg in deepcopy(config):
         if "parent" in config_arg.lower():
             yaml_parent_path = Path(yaml_path).parent / Path(config[config_arg])
             parent_config = load_yaml_calc(yaml_parent_path)
```

### Comparing `quacc-0.7.4/src/quacc/utils/kpts.py` & `quacc-0.7.5/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/utils/lists.py` & `quacc-0.7.5/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/wflow_tools/customizers.py` & `quacc-0.7.5/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/wflow_tools/db.py` & `quacc-0.7.5/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc/wflow_tools/decorators.py` & `quacc-0.7.5/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc.egg-info/PKG-INFO` & `quacc-0.7.5/src/quacc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.4
+Version: 0.7.5
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -30,15 +30,16 @@
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
-Requires-Dist: pymatgen>=2024.4.12
+Requires-Dist: pymatgen>=2024.4.13
+Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
 Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
@@ -90,15 +91,14 @@
 <div align="center">
   <img src=https://github.com/Quantum-Accelerators/quacc/blob/main/docs/images/quacc_logo_wide.png width="300"><br>
 </div>
 
 # `quacc` – The Quantum Accelerator 🦆
 
 [![codecov](https://codecov.io/gh/Quantum-Accelerators/quacc/branch/main/graph/badge.svg?token=OJaOZAH30u&precision=1)](https://codecov.io/gh/Quantum-Accelerators/quacc)
-[![DeepSource](https://app.deepsource.com/gh/Quantum-Accelerators/quacc.svg/?label=active+issues&token=Y1NxOLIuFFEqWdjawIYnJNde)](https://app.deepsource.com/gh/Quantum-Accelerators/quacc/?ref=repository-badge)
 ![Python - Version](https://img.shields.io/pypi/pyversions/quacc)
 ![PyPI - Version](https://img.shields.io/pypi/v/quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/10.5281/zenodo.7720998)
 
 `quacc` is a flexible platform for computational materials science 💎 and quantum chemistry 🧪 that is built for the big data era 🔥. It is maintained by the [Rosen Research Group](https://rosen.cbe.princeton.edu/) at Princeton University.
 
 - `quacc` makes it possible to easily run pre-made [computational materials science workflows](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination thereof.
```

### Comparing `quacc-0.7.4/src/quacc.egg-info/SOURCES.txt` & `quacc-0.7.5/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.7.4/src/quacc.egg-info/requires.txt` & `quacc-0.7.5/src/quacc.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 emmet-core>=0.80.0
 maggma>=0.64.0
 monty>=2024.2.26
 numpy>=1.25.0
 psutil
 pydantic>=2.0.1
 pydantic-settings>=2.2.0
-pymatgen>=2024.4.12
+pymatgen>=2024.4.13
+ruamel.yaml>=0.17.40
 typer>=0.12.1
 
 [covalent]
 covalent>=0.234.0rc0
 covalent-cloud>=0.39.0
 
 [dask]
```

