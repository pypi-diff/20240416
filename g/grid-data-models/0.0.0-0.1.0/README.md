# Comparing `tmp/grid_data_models-0.0.0.tar.gz` & `tmp/grid_data_models-0.1.0.tar.gz`

## Comparing `grid_data_models-0.0.0.tar` & `grid_data_models-0.1.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/__init__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/bus.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/capacitor.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/exceptions.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/load.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/quantities.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transformer.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/dataset/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/dataset/cost_model.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/dataset/dataset_system.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/__init__.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/curve.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/distribution_common.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/distribution_enum.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/distribution_graph.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/distribution_system.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/limitset.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/sequence_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/__init__.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_branch.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_bus.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_capacitor.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_component.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_feeder.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_fuse.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_load.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_recloser.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_regulator.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_solar.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_substation.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_switch.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_transformer.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/distribution_vsource.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/geometry_branch.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_branch.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_fuse.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_recloser.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_switch.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/components/sequence_impedance_branch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/controllers/__init__.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_inverter_controller.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_recloser_controller.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_regulator_controller.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_switch_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/bare_conductor_equipment.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/capacitor_equipment.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/concentric_cable_equipment.py
--rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/geometry_branch_equipment.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/inverter_equipment.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/load_equipment.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/phase_load_equipment.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/recloser_controller_equipment.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/distribution/equipment/solar_equipment.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transmission/transmission_branch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transmission/transmission_bus.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transmission/transmission_capacitor.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transmission/transmission_component.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transmission/transmission_load.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/src/gdm/transmission/transmission_substation.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/.gitignore
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/README.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 grid_data_models-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/bus.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/capacitor.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/constants.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/exceptions.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/load.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/quantities.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transformer.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/dataset/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/dataset/cost_model.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/dataset/dataset_system.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/__init__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/curve.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_common.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_enum.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_graph.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/distribution_system.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/limitset.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/sequence_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_branch.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_bus.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_capacitor.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_component.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_feeder.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_fuse.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_load.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_recloser.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_regulator.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_solar.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_substation.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_switch.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_transformer.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/distribution_vsource.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/geometry_branch.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_branch.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_fuse.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_recloser.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_switch.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/components/sequence_impedance_branch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/__init__.py
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_inverter_controller.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_recloser_controller.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_regulator_controller.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_switch_controller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/bare_conductor_equipment.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/capacitor_equipment.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/concentric_cable_equipment.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/geometry_branch_equipment.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/inverter_equipment.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/load_equipment.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_load_equipment.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/recloser_controller_equipment.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/distribution/equipment/solar_equipment.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_branch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_bus.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_capacitor.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_component.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_load.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/src/gdm/transmission/transmission_substation.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/README.md
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 grid_data_models-0.1.0/PKG-INFO
```

### Comparing `grid_data_models-0.0.0/src/gdm/__init__.py` & `grid_data_models-0.1.0/src/gdm/__init__.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/bus.py` & `grid_data_models-0.1.0/src/gdm/bus.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 from typing import Annotated, Optional
 
 from infrasys import Component, Location
 from pydantic import Field
 
 from gdm.quantities import PositiveVoltage
+from gdm.constants import PINT_SCHEMA
 
 
 class PowerSystemBus(Component):
     """Interface for power system bus."""
 
     nominal_voltage: Annotated[
-        PositiveVoltage, Field(..., description="Nominal voltage for this bus.")
+        PositiveVoltage,
+        PINT_SCHEMA,
+        Field(..., description="Nominal voltage for this bus."),
     ]
     coordinate: Annotated[
         Optional[Location],
         Field(None, description="Coordinate for the power system bus."),
     ]
 
     @classmethod
```

### Comparing `grid_data_models-0.0.0/src/gdm/capacitor.py` & `grid_data_models-0.1.0/src/gdm/capacitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 from typing import Annotated
 
 from pydantic import Field, NonNegativeInt, PositiveInt, model_validator
 
 from infrasys import Component
 from gdm.quantities import PositiveReactivePower
+from gdm.constants import PINT_SCHEMA
 
 
 class PowerSystemCapacitor(Component):
     """Interface for power system capacitor."""
 
     rated_capacity: Annotated[
         PositiveReactivePower,
+        PINT_SCHEMA,
         Field(..., description="Capacity of this capacitor."),
     ]
     num_banks_on: Annotated[
         NonNegativeInt, Field(..., description="Number of banks currently on.")
     ]
     num_banks: Annotated[PositiveInt, Field(1, description="Number of banks in the capacitor.")]
```

### Comparing `grid_data_models-0.0.0/src/gdm/load.py` & `grid_data_models-0.1.0/src/gdm/load.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,56 +3,63 @@
 from typing import Annotated
 
 from infrasys import Component
 from infrasys.quantities import ActivePower
 from pydantic import Field
 
 from gdm.quantities import ReactivePower
+from gdm.constants import PINT_SCHEMA
 
 
 class PowerSystemLoad(Component):
     """Interface for power system load."""
 
     z_real: Annotated[
         ActivePower,
+        PINT_SCHEMA,
         Field(
             default=ActivePower(0, "kilowatt"),
             description="Constant impedance load real component.",
         ),
     ]
     z_imag: Annotated[
         ReactivePower,
+        PINT_SCHEMA,
         Field(
             default=ReactivePower(0, "kilovar"),
             description="Constant impedance load imaginary component.",
         ),
     ]
     i_real: Annotated[
         ActivePower,
+        PINT_SCHEMA,
         Field(
             default=ActivePower(0, "kilowatt"),
             description="Constant current load real component.",
         ),
     ]
     i_imag: Annotated[
         ReactivePower,
+        PINT_SCHEMA,
         Field(
             default=ReactivePower(0, "kilovar"),
             description="Constant current load imaginary component.",
         ),
     ]
     p_real: Annotated[
         ActivePower,
+        PINT_SCHEMA,
         Field(
             default=ActivePower(0, "kilowatt"),
             description="Constant power load real component.",
         ),
     ]
     p_imag: Annotated[
         ReactivePower,
+        PINT_SCHEMA,
         Field(
             default=ReactivePower(0, "kilovar"),
             description="Constant power load imaginary component.",
         ),
     ]
 
     @classmethod
```

### Comparing `grid_data_models-0.0.0/src/gdm/quantities.py` & `grid_data_models-0.1.0/src/gdm/quantities.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     __compatible_unit__ = "ohm/m"
 
 
 class PositiveResistancePULength(ResistancePULength):
     """Quantity representing per unit length positive resistance."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Resistance per unit length ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Resistance per unit length ({value}, {units}) must be positive."
 
 
 class Reactance(Resistance):
     """Quantity representing power system reactance."""
 
 
 class ReactancePULength(BaseQuantity):
@@ -43,22 +45,26 @@
     __compatible_unit__ = "ohm/m"
 
 
 class PositiveReactancePULength(ReactancePULength):
     """Quantity representing per unit length positive power system reactance."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Reactance per unit length ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Reactance per unit length ({value}, {units}) must be positive."
 
 
 class PositiveReactance(PositiveResistance):
     """Quantity representing positive power system reactance."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Reactance ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Reactance ({value}, {units}) must be positive."
 
 
 class Capacitance(BaseQuantity):
     """Quantity representing power system capacitance."""
 
     __compatible_unit__ = "farad"
 
@@ -69,54 +75,67 @@
     __compatible_unit__ = "farad/m"
 
 
 class PositiveCapacitancePULength(CapacitancePULength):
     """Quantity representing per unit length positive capacitance."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Per unit capacitance ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Per unit capacitance ({value}, {units}) must be positive."
 
 
 class PositiveCapacitance(Capacitance):
     """Quantity represening positive capacitance."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Capacitance ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Capacitance ({value}, {units}) must be positive."
 
 
 class ReactivePower(BaseQuantity):
     """Quantity representing reactive power."""
 
     __compatible_unit__ = "var"
 
 
 class PositiveReactivePower(ReactivePower):
     """Quantity representing positive reactive power."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Reactive power ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Reactive power ({value}, {units}) must be positive."
 
 
 class ApparentPower(BaseQuantity):
     """Quantity representing apparent power."""
 
     __compatible_unit__ = "va"
 
 
 class PositiveApparentPower(ApparentPower):
     """Quantity representing positive apparent power."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Apparent power ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Apparent power ({value}, {units}) must be positive."
+
+
+# TODO: Should these get added to infrasys rather than here?
 
-#TODO: Should these get added to infrasys rather than here?
 
 class PositiveActivePower(ActivePower):
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Active power ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Active power ({value}, {units}) must be positive."
+
 
 class PositiveCurrent(Current):
     """Qauntity representing positive current."""
 
     def __init__(self, value, units, **kwargs):
         assert all(np.array(value).flatten() >= 0), f"Current ({value}, {units}) must be positive."
 
@@ -128,19 +147,22 @@
         assert all(np.array(value).flatten() >= 0), f"Voltage ({value}, {units}) must be positive."
 
 
 class PositiveDistance(Distance):
     """Quantity representing positive distance."""
 
     def __init__(self, value, units, **kwargs):
-        assert all(np.array(value).flatten() >= 0), f"Distance ({value}, {units}) must be positive."
+        assert all(
+            np.array(value).flatten() >= 0
+        ), f"Distance ({value}, {units}) must be positive."
+
 
 class ActivePowerPUTime(BaseQuantity):
     """Quantity representing active power per unit of time"""
 
     __compatible_unit__ = "watt/minute"
 
 
 class Irradiance(BaseQuantity):
-    """Quantity representing irradiance in kilowatt per meter**2  """
+    """Quantity representing irradiance in kilowatt per meter**2"""
 
     __compatible_unit__ = "kilowatt/meter**2"
```

### Comparing `grid_data_models-0.0.0/src/gdm/version.py` & `grid_data_models-0.1.0/src/gdm/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import subprocess
 import platform
 import sys
 
-VERSION = "0.0.0"
+VERSION = "0.1.0"
 
 
 def is_git_repo(dir: Path) -> bool:
     """Returns true if it is a git repo."""
     git_path = dir / ".git"
     return git_path.exists()
```

### Comparing `grid_data_models-0.0.0/src/gdm/dataset/cost_model.py` & `grid_data_models-0.1.0/src/gdm/dataset/cost_model.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/dataset/dataset_system.py` & `grid_data_models-0.1.0/src/gdm/dataset/dataset_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/curve.py` & `grid_data_models-0.1.0/src/gdm/distribution/curve.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from typing import Annotated
 
 from pydantic import model_validator, Field
 from infrasys import Component
 from infrasys.quantities import Time, Current
 
+from gdm.constants import PINT_SCHEMA
+
 
 class Curve(Component):
     """An interface for representing a curve using x and y points. e.g for volt-var and volt-watt curves.
 
     Examples
     --------
 
@@ -44,16 +46,16 @@
         )
 
 
 class TimeCurrentCurve(Component):
     """An interface for time current curve."""
 
     name: Annotated[str, Field("", description="Name of the curve.")]
-    curve_x: Annotated[Current, Field(..., description="Array of time values.")]
-    curve_y: Annotated[Time, Field(..., description="Array of current values.")]
+    curve_x: Annotated[Current, PINT_SCHEMA, Field(..., description="Array of time values.")]
+    curve_y: Annotated[Time, PINT_SCHEMA, Field(..., description="Array of current values.")]
 
     @model_validator(mode="after")
     def validate_fields(self) -> "Curve":
         if len(self.curve_x) != len(self.curve_y):
             msg = f"curve_x ({self.curve_x=}) and curve_y ({self.curve_y=}) have different lengths"
             raise ValueError(msg)
         return self
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/distribution_enum.py` & `grid_data_models-0.1.0/src/gdm/distribution/distribution_enum.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/distribution_graph.py` & `grid_data_models-0.1.0/src/gdm/distribution/distribution_graph.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/distribution_system.py` & `grid_data_models-0.1.0/src/gdm/distribution/distribution_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/limitset.py` & `grid_data_models-0.1.0/src/gdm/distribution/limitset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """ This module contains interface for operation limit sets. """
 
 from typing import Annotated
 from infrasys import Component
+from pydantic import Field
 
 from gdm.quantities import PositiveCurrent, PositiveVoltage
 from gdm.distribution.distribution_enum import LimitType
-from pydantic import Field
+from gdm.constants import PINT_SCHEMA
 
 
 class VoltageLimitSet(Component):
     """Interface for voltage limit set."""
-    name: Annotated[str, Field('', description="Name of the voltage limit set.")]
+
+    name: Annotated[str, Field("", description="Name of the voltage limit set.")]
     limit_type: Annotated[LimitType, Field(..., description="Limit type used.")]
-    value: Annotated[PositiveVoltage, Field(..., description="Voltage threshold.")]
+    value: Annotated[
+        PositiveVoltage,
+        PINT_SCHEMA,
+        Field(..., description="Voltage threshold."),
+    ]
 
     @classmethod
     def example(cls) -> "VoltageLimitSet":
         """Example for voltage limit set."""
         return VoltageLimitSet(limit_type=LimitType.MIN, value=PositiveVoltage(400 * 0.9, "volt"))
 
 
 class ThermalLimitSet(Component):
     """Interface for voltage limit set."""
-    name: Annotated[str, Field('', description="Name of the thermal limit set.")]
+
+    name: Annotated[str, Field("", description="Name of the thermal limit set.")]
     limit_type: Annotated[LimitType, Field(..., description="Limit type used.")]
-    value: Annotated[PositiveCurrent, Field(..., description="Current threshold.")]
+    value: Annotated[PositiveCurrent, PINT_SCHEMA, Field(..., description="Current threshold.")]
 
     @classmethod
     def example(cls) -> "ThermalLimitSet":
         """Example for thermal limit set."""
         return ThermalLimitSet(limit_type=LimitType.MAX, value=PositiveCurrent(110, "ampere"))
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_branch.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.distribution.distribution_enum import Phase
 from gdm.quantities import (
     PositiveDistance,
     PositiveVoltage,
 )
+from gdm.constants import PINT_SCHEMA
 
 
 class DistributionBranch(Component):
     """Interface for distribution branch."""
 
     belongs_to: BELONG_TO_TYPE
     buses: Annotated[
         list[DistributionBus],
         Field(..., description="List of buses connecting a branch."),
     ]
-    length: Annotated[PositiveDistance, Field(..., description="Length of the branch.")]
+    length: Annotated[
+        PositiveDistance, PINT_SCHEMA, Field(..., description="Length of the branch.")
+    ]
     phases: Annotated[
         list[Phase],
         Field(..., description="List of phases in the same order as conductors."),
     ]
 
     @model_validator(mode="after")
     def validate_fields(self) -> "DistributionBranch":
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_bus.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_bus.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_capacitor.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_capacitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             ),
         ),
     ]
     controllers: Annotated[
         list[CapacitorController],
         Field(
             [],
-            description=("List of the controllers which are used for each phase in order.",),
+            description="List of the controllers which are used for each phase in order.",
         ),
     ]
 
     equipment: Annotated[CapacitorEquipment, Field(..., description="Capacitor model.")]
 
     @model_validator(mode="after")
     def validate_fields(self) -> "DistributionCapacitor":
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_component.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from gdm.distribution.components.distribution_feeder import DistributionFeeder
 from gdm.distribution.components.distribution_substation import DistributionSubstation
 
 
 class DistributionComponent(Component):
     """Interface for simple distribution component."""
-    name: Annotated[str, Field('', description="Name of the component.")]
+
+    name: Annotated[str, Field("", description="Name of the component.")]
     substation: Annotated[
         Optional[DistributionSubstation], Field(None, description="Name of the substation.")
     ]
     feeder: Annotated[Optional[DistributionFeeder], Field(None, description="Name of the feeder.")]
 
     @classmethod
     def example(cls) -> "DistributionComponent":
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_load.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_load.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_regulator.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_regulator.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_solar.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_solar.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             ),
         ),
     ]
     controller: Annotated[
         InverterController,
         Field(
             ...,
-            description=("The controller which is used for the PV array.",),
+            description="The controller which is used for the PV array.",
         ),
     ]
 
     equipment: Annotated[SolarEquipment, Field(..., description="Solar PV model.")]
 
     @classmethod
     def example(cls) -> "DistributionSolar":
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_substation.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_substation.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_transformer.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,42 +52,51 @@
     ]
 
     def _check_if_voltage_is_on_split_side(self, voltage: Voltage) -> bool:
         """Internal method to check if winding is on split side."""
         if not self.equipment.is_center_tapped:
             return False
 
-        all_voltages = [item.nominal_voltage for item in self.equipment.windings]
-        if voltage not in all_voltages:
-            msg = f"{voltage=} not in transformer winding voltages = {all_voltages}"
+        all_voltages = [round(item.nominal_voltage, 2) for item in self.equipment.windings]
+        if round(voltage, 2) not in all_voltages:
+            msg = f"{round(voltage, 2)=} not in transformer winding voltages = {all_voltages}"
             raise ValueError(msg)
         return voltage < max(all_voltages)
 
     @model_validator(mode="after")
     def validate_fields(self) -> "DistributionTransformer":
         """Custom validator for distribution transformer."""
         if len(self.winding_phases) != len(self.equipment.windings):
             msg = (
-                f"Number of windings {len(self.equipment.windings)} must be equal to"
+                f"Number of windings {len(self.equipment.windings)} must be equal to "
                 f"numbe of winding phases {len(self.winding_phases)}"
             )
             raise ValueError(msg)
 
         for wdg, pw_phases in zip(self.equipment.windings, self.winding_phases):
-            if len(pw_phases) > wdg.num_phases:
+            pw_phases_length = len(pw_phases) - 1 if Phase.N in pw_phases else len(pw_phases)
+
+            if pw_phases_length > wdg.num_phases and pw_phases_length != 2:
+                msg = (
+                    f"Number of phases in windings {wdg.num_phases=} must be "
+                    f"less than or equal to phases {pw_phases=}"
+                )
+                raise ValueError(msg)
+            elif pw_phases_length == 2 and wdg.num_phases != 1:
                 msg = (
-                    f"Number of phases in windings {wdg.num_phases=} must be"
-                    f"greater than or equal to phases {pw_phases=}"
+                    f"For a single phase delta connected transformer, {pw_phases=}"
+                    f" inconsistant number of phases provided for winding {wdg.num_phases=}"
                 )
                 raise ValueError(msg)
 
         for bus, pw_phases in zip(self.buses, self.winding_phases):
-            if not set(pw_phases).issubset(bus.phases):
+            if not (set(pw_phases) - set(Phase.N)).issubset(bus.phases):
                 msg = (
-                    f"Winding phases {pw_phases=}" f"must be subset of bus phases ({bus.phases=})."
+                    f"Winding phases {pw_phases=}"
+                    f" must be subset of bus phases ({bus.phases=})."
                 )
                 raise ValueError(msg)
 
         for bus, wdg in zip(self.buses, self.equipment.windings):
             bus_phase_voltage = get_phase_voltage_in_kv(
                 bus.nominal_voltage,
                 bus.voltage_type,
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/distribution_vsource.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/distribution_vsource.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 from infrasys.quantities import Angle, Resistance, Voltage
 from pydantic import Field
 
 from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.quantities import Reactance, PositiveVoltage
 from gdm.distribution.distribution_enum import Phase
+from gdm.constants import PINT_SCHEMA
 
 
 class PhaseVoltageSourceEquipment(Component):
     """Interface for phase voltage source."""
-    r0: Annotated[Resistance, Field(..., description="Zero sequence resistance.")]
-    r1: Annotated[Resistance, Field(..., description="Positive sequence resistance.")]
-    x0: Annotated[Reactance, Field(..., description="Zero sequence reactance.")]
-    x1: Annotated[Reactance, Field(..., description="Positive sequence reactane.")]
-    voltage: Annotated[Voltage, Field(..., description="Voltage for this substation.")]
-    angle: Annotated[Angle, Field(..., description="Angle for the voltage")]
+
+    r0: Annotated[Resistance, PINT_SCHEMA, Field(..., description="Zero sequence resistance.")]
+    r1: Annotated[Resistance, PINT_SCHEMA, Field(..., description="Positive sequence resistance.")]
+    x0: Annotated[Reactance, PINT_SCHEMA, Field(..., description="Zero sequence reactance.")]
+    x1: Annotated[Reactance, PINT_SCHEMA, Field(..., description="Positive sequence reactane.")]
+    voltage: Annotated[
+        Voltage, PINT_SCHEMA, Field(..., description="Voltage for this substation.")
+    ]
+    angle: Annotated[Angle, PINT_SCHEMA, Field(..., description="Angle for the voltage")]
 
     @classmethod
     def example(cls) -> "PhaseVoltageSourceEquipment":
         """Example for phase voltage source."""
         return PhaseVoltageSourceEquipment(
             name="phase-source-1",
             r0=Resistance(0.001, "ohm"),
@@ -33,26 +37,29 @@
             voltage=PositiveVoltage(132.0, "kilovolt"),
             angle=Angle(180, "degree"),
         )
 
 
 class VoltageSourceEquipment(Component):
     """Interface for voltage source model."""
+
     sources: Annotated[
         list[PhaseVoltageSourceEquipment],
         Field(
             ...,
             description="list of single phase voltage sources",
         ),
     ]
 
     @classmethod
     def example(cls) -> "VoltageSourceEquipment":
         """Example for voltage source model."""
-        return VoltageSourceEquipment(name="Voltage Source 1", sources=[PhaseVoltageSourceEquipment.example()] * 3)
+        return VoltageSourceEquipment(
+            name="Voltage Source 1", sources=[PhaseVoltageSourceEquipment.example()] * 3
+        )
 
 
 class DistributionVoltageSource(Component):
     """Interface for distribution substation."""
 
     belongs_to: BELONG_TO_TYPE
     bus: Annotated[
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/geometry_branch.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/geometry_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_branch.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_fuse.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_fuse.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_recloser.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_recloser.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/matrix_impedance_switch.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/matrix_impedance_switch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/components/sequence_impedance_branch.py` & `grid_data_models-0.1.0/src/gdm/distribution/components/sequence_impedance_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py` & `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,35 +9,40 @@
 
 from gdm.quantities import (
     PositiveActivePower,
     PositiveReactivePower,
     PositiveVoltage,
     PositiveCurrent,
 )
+from gdm.constants import PINT_SCHEMA
 
 
 class CapacitorController(Component):
     """Interface for capacitor controllers. Phase connection specified in the capacitor."""
-    name: Annotated[str, Field('', description="Name of the capacitor controller.")]
+
+    name: Annotated[str, Field("", description="Name of the capacitor controller.")]
     delay_on: Annotated[
         Optional[Time],
+        PINT_SCHEMA,
         Field(
             None,
             description="The time that the capacitor needs to connect or disconnect when switching on",
         ),
     ]
     delay_off: Annotated[
         Optional[Time],
+        PINT_SCHEMA,
         Field(
             None,
             description="The time that the capacitor needs to connect or disconnect when switching off",
         ),
     ]
     dead_time: Annotated[
         Optional[Time],
+        PINT_SCHEMA,
         Field(
             None,
             description="The time that the capacitor must remain off before turning back on again",
         ),
     ]
 
     @classmethod
@@ -47,22 +52,24 @@
 
 
 class VoltageCapacitorController(CapacitorController):
     """Interface for a Capacitor Controller which uses voltage."""
 
     on_voltage: Annotated[
         PositiveVoltage,
+        PINT_SCHEMA,
         Field(
             ...,
             description="Value of the controller voltage, above which the capacitor switches on.",
         ),
     ]
 
     off_voltage: Annotated[
         PositiveVoltage,
+        PINT_SCHEMA,
         Field(..., description="Value of the voltage, below which the capacitors switches off."),
     ]
 
     pt_ratio: Annotated[
         float,
         Field(
             ...,
@@ -83,21 +90,23 @@
 
 
 class ActivePowerCapacitorController(CapacitorController):
     """Interface for a Capacitor Controller which uses active power."""
 
     on_power: Annotated[
         PositiveActivePower,
+        PINT_SCHEMA,
         Field(
             ..., description="Value of the active power, above which the capacitor switches on."
         ),
     ]
 
     off_power: Annotated[
         PositiveActivePower,
+        PINT_SCHEMA,
         Field(
             ..., description="Value of the active power, below which the capacitor switches off."
         ),
     ]
 
     @classmethod
     def example(cls) -> "ActivePowerCapacitorController":
@@ -110,21 +119,23 @@
 
 
 class ReactivePowerCapacitorController(CapacitorController):
     """Interface for a Capacitor Controller which uses reactive power."""
 
     on_power: Annotated[
         PositiveReactivePower,
+        PINT_SCHEMA,
         Field(
             ..., description="Value of the reactive power, above which the capacitor switches on."
         ),
     ]
 
     off_power: Annotated[
         PositiveReactivePower,
+        PINT_SCHEMA,
         Field(
             ..., description="Value of the reactive power, below which the capacitor switches off."
         ),
     ]
 
     @classmethod
     def example(cls) -> "ReactivePowerCapacitorController":
@@ -137,22 +148,24 @@
 
 
 class CurrentCapacitorController(CapacitorController):
     """Interface for a Capacitor Controller which uses current."""
 
     on_current: Annotated[
         PositiveCurrent,
+        PINT_SCHEMA,
         Field(
             ...,
             description="Value of the controller current, above which the capacitor switches on.",
         ),
     ]
 
     off_current: Annotated[
         PositiveCurrent,
+        PINT_SCHEMA,
         Field(
             ...,
             description="Value of the controller current, below which the capacitor switches off.",
         ),
     ]
 
     ct_ratio: Annotated[
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_inverter_controller.py` & `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_inverter_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_recloser_controller.py` & `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_recloser_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 
 from pydantic import Field, model_validator
 from infrasys.quantities import Time
 from infrasys import Component
 
 from gdm.distribution.equipment.recloser_controller_equipment import RecloserControllerEquipment
 from gdm.distribution.curve import TimeCurrentCurve
+from gdm.constants import PINT_SCHEMA
 
 
 class DistributionRecloserController(Component):
     """Interface for distribution recloser controller."""
-    name: Annotated[str, Field('', description="Name of the recloser controller.")]
-    delay: Annotated[Time, Field(description="Fixed delay added to the recloser trip time.")]
+
+    name: Annotated[str, Field("", description="Name of the recloser controller.")]
+
+    delay: Annotated[
+        Time, PINT_SCHEMA, Field(description="Fixed delay added to the recloser trip time.")
+    ]
     ground_delayed: Annotated[
         TimeCurrentCurve, Field(description="TCC curve related to ground delayed trip.")
     ]
     ground_fast: Annotated[
         TimeCurrentCurve, Field(description="TCC curve related to ground fast trip.")
     ]
     phase_delayed: Annotated[
@@ -28,16 +33,18 @@
     ]
     num_fast_ops: Annotated[
         int, Field(ge=0, description="Number of fast operations (fuse savings).")
     ]
     num_shots: Annotated[
         int, Field(ge=1, description="Number of fast and delayed shots before lockout.")
     ]
-    reclose_intervals: Annotated[Time, Field(..., description="Array of reclose intervals.")]
-    reset_time: Annotated[Time, Field(..., description="Reset time for recloser.")]
+    reclose_intervals: Annotated[
+        Time, PINT_SCHEMA, Field(..., description="Array of reclose intervals.")
+    ]
+    reset_time: Annotated[Time, PINT_SCHEMA, Field(..., description="Reset time for recloser.")]
     equipment: Annotated[
         RecloserControllerEquipment, Field(..., description="Recloser controller equipment.")
     ]
 
     @model_validator(mode="after")
     def validate_fields(self) -> "DistributionRecloserController":
         """Validate fields for DistributionRecloserController."""
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_regulator_controller.py` & `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_regulator_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,69 @@
 """ This module contains interface for distribution controllers."""
+
 from typing import Annotated, Optional
 
 from infrasys import Component
 from infrasys.quantities import Time
 from pydantic import Field
 
 from gdm.quantities import (
     PositiveVoltage,
     PositiveCurrent,
 )
+
+from gdm.constants import PINT_SCHEMA
+
+
 class RegulatorController(Component):
     """Interface for a Regulator Controller."""
-    name: Annotated[str, Field('', description="Name of the regulator controller.")]
+
+    name: Annotated[str, Field("", description="Name of the regulator controller.")]
     delay: Annotated[
-        Optional[Time], Field(..., description="Delay for the first tap change operation")
+        Optional[Time],
+        PINT_SCHEMA,
+        Field(..., description="Delay for the first tap change operation"),
     ]
     regulator_setting: Annotated[
-        PositiveVoltage, Field(..., description="The target control voltage for regulator controller.")
+        PositiveVoltage,
+        PINT_SCHEMA,
+        Field(..., description="The target control voltage for regulator controller."),
     ]
     pt_ratio: Annotated[
-        float, Field(..., ge=0, description="Value of the voltage (potential) transformer ratio used to step down the voltage for the controller.")
+        float,
+        Field(
+            ...,
+            ge=0,
+            description="Value of the voltage (potential) transformer ratio used to step down the voltage for the controller.",
+        ),
     ]
     ldc_R: Annotated[
-        Optional[PositiveVoltage], Field(None, description="R setting on the line drop compensator of the regulator in Volts.")
+        Optional[PositiveVoltage],
+        PINT_SCHEMA,
+        Field(
+            None, description="R setting on the line drop compensator of the regulator in Volts."
+        ),
     ]
     ldc_X: Annotated[
-        Optional[PositiveVoltage], Field(None, description="X setting on the line drop compensator of the regulator in Volts.")
+        Optional[PositiveVoltage],
+        PINT_SCHEMA,
+        Field(
+            None, description="X setting on the line drop compensator of the regulator in Volts."
+        ),
     ]
     ct_primary: Annotated[
-        Optional[PositiveCurrent], Field(None, description="Current at which the line drop compensator voltages match the R and X settings.")
+        Optional[PositiveCurrent],
+        PINT_SCHEMA,
+        Field(
+            None,
+            description="Current at which the line drop compensator voltages match the R and X settings.",
+        ),
     ]
 
     @classmethod
     def example(cls) -> "RegulatorController":
         """Example for a Regulator Controller."""
         return RegulatorController(
-            delay = Time(10, "seconds"),
-            regulator_setting = PositiveVoltage(120,"volts"),
-            pt_ratio = 60,
+            delay=Time(10, "seconds"),
+            regulator_setting=PositiveVoltage(120, "volts"),
+            pt_ratio=60,
         )
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/controllers/distribution_switch_controller.py` & `grid_data_models-0.1.0/src/gdm/distribution/controllers/distribution_switch_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,26 @@
 from typing import Annotated, Literal
 
 from pydantic import Field
 
 from infrasys.quantities import Time
 from infrasys import Component
 
+from gdm.constants import PINT_SCHEMA
+
 
 class DistributionSwitchController(Component):
     """Interface for distribution switch controller."""
-    name: Annotated[str, Field('', description="Name of the switch controller.")]
-    delay: Annotated[Time, Field(description="Fixed delay added to the recloser trip time.")]
+
+    name: Annotated[str, Field("", description="Name of the switch controller.")]
+
+    delay: Annotated[
+        Time, PINT_SCHEMA, Field(description="Fixed delay added to the recloser trip time.")
+    ]
+
     normal_state: Annotated[
         Literal["open", "close"],
         Field(..., description="Action to open or close the switch after delay time."),
     ]
     is_locked: Annotated[
         bool, Field(description="Boolean value representing whether the switch is locked or not.")
     ]
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/bare_conductor_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/bare_conductor_equipment.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,40 +7,47 @@
 
 from gdm.distribution.limitset import ThermalLimitSet
 from gdm.quantities import (
     PositiveResistancePULength,
     PositiveDistance,
     PositiveCurrent,
 )
+from gdm.constants import PINT_SCHEMA
 
 
 class BareConductorEquipment(Component):
     """Interface for conductor catalaog."""
 
     conductor_diameter: Annotated[
-        PositiveDistance, Field(..., description="Diameter of the conductor.")
+        PositiveDistance, PINT_SCHEMA, Field(..., description="Diameter of the conductor.")
     ]
     conductor_gmr: Annotated[
         PositiveDistance,
+        PINT_SCHEMA,
         Field(..., description="Geometric mean radius of the conductor."),
     ]
-    ampacity: Annotated[PositiveCurrent, Field(..., description="Ampacity of the conductor.")]
+    ampacity: Annotated[
+        PositiveCurrent, PINT_SCHEMA, Field(..., description="Ampacity of the conductor.")
+    ]
     ac_resistance: Annotated[
         PositiveResistancePULength,
+        PINT_SCHEMA,
         Field(
             ...,
             description="Per unit length positive alternating current resistance of the conductor.",
         ),
     ]
     emergency_ampacity: Annotated[
         PositiveCurrent,
+        PINT_SCHEMA,
         Field(..., description="Emergency ampacity for this conductor."),
     ]
     dc_resistance: Annotated[
         PositiveResistancePULength,
+        PINT_SCHEMA,
         Field(
             ...,
             description="Per unit length positive direct current resistance of the conductor.",
         ),
     ]
     loading_limit: Annotated[
         Optional[ThermalLimitSet],
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/capacitor_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/capacitor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/concentric_cable_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/concentric_cable_equipment.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,57 +8,70 @@
 from gdm.quantities import (
     PositiveDistance,
     PositiveCurrent,
     PositiveResistancePULength,
     PositiveVoltage,
 )
 from gdm.distribution.limitset import ThermalLimitSet
+from gdm.constants import PINT_SCHEMA
 
 
 class ConcentricCableEquipment(Component):
     """Interface for cable catalog."""
 
     strand_diameter: Annotated[
-        PositiveDistance, Field(..., description="Diameter of the cable strand.")
+        PositiveDistance, PINT_SCHEMA, Field(..., description="Diameter of the cable strand.")
     ]
     conductor_diameter: Annotated[
         PositiveDistance,
+        PINT_SCHEMA,
         Field(..., description="Diameter of the conductor inside cable."),
     ]
-    cable_diameter: Annotated[PositiveDistance, Field(..., description="Diameter of the cable.")]
+    cable_diameter: Annotated[
+        PositiveDistance, PINT_SCHEMA, Field(..., description="Diameter of the cable.")
+    ]
     insulation_thickness: Annotated[
-        PositiveDistance, Field(..., description="Thickness of insulation.")
+        PositiveDistance, PINT_SCHEMA, Field(..., description="Thickness of insulation.")
     ]
     insulation_diameter: Annotated[
-        PositiveDistance, Field(..., description="Diameter of the insulation.")
+        PositiveDistance, PINT_SCHEMA, Field(..., description="Diameter of the insulation.")
+    ]
+    ampacity: Annotated[
+        PositiveCurrent, PINT_SCHEMA, Field(..., description="Ampacity of the conductor.")
     ]
-    ampacity: Annotated[PositiveCurrent, Field(..., description="Ampacity of the conductor.")]
     emergency_ampacity: Annotated[
-        PositiveCurrent, Field(..., description="Emergency ampacity of the conductor.")
+        PositiveCurrent,
+        PINT_SCHEMA,
+        Field(..., description="Emergency ampacity of the conductor."),
     ]
     conductor_gmr: Annotated[
         PositiveDistance,
+        PINT_SCHEMA,
         Field(..., description="Geometric mean radius of the conductor."),
     ]
     strand_gmr: Annotated[
-        PositiveDistance, Field(..., description="Geometric mean radius of the strand.")
+        PositiveDistance,
+        PINT_SCHEMA,
+        Field(..., description="Geometric mean radius of the strand."),
     ]
     phase_ac_resistance: Annotated[
         PositiveResistancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length conductor ac resistance."),
     ]
     strand_ac_resistance: Annotated[
         PositiveResistancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length ac resistance of the strand."),
     ]
     num_neutral_strands: Annotated[
         PositiveInt, Field(..., description="Number of neutral strands in the cable.")
     ]
     rated_voltage: Annotated[
-        PositiveVoltage, Field(..., description="Rated voltage for the cable.")
+        PositiveVoltage, PINT_SCHEMA, Field(..., description="Rated voltage for the cable.")
     ]
     loading_limit: Annotated[
         Optional[ThermalLimitSet],
         Field(None, description="Loading limit set for this conductor."),
     ]
 
     @model_validator(mode="after")
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from infrasys import Component
 from pydantic import Field, model_validator
 
 from gdm.distribution.sequence_pair import SequencePair
 from gdm.distribution.distribution_enum import ConnectionType, VoltageTypes
 from gdm.quantities import PositiveApparentPower, PositiveVoltage
+from gdm.constants import PINT_SCHEMA
 
 
 class WindingEquipment(Component):
     """Interface for winding."""
 
     name: Annotated[str, Field("", description="Name of the winding.")]
     resistance: Annotated[
@@ -20,21 +21,23 @@
         Field(
             ..., strict=True, ge=0, le=100, description="Percentage resistance for this winding."
         ),
     ]
     is_grounded: Annotated[bool, Field(..., description="Is this winding grounded or not.")]
     nominal_voltage: Annotated[
         PositiveVoltage,
+        PINT_SCHEMA,
         Field(..., description="Nominal voltage rating for this winding."),
     ]
     voltage_type: Annotated[
         VoltageTypes, Field(..., description="Set voltage type for nominal voltage.")
     ]
     rated_power: Annotated[
         PositiveApparentPower,
+        PINT_SCHEMA,
         Field(..., description="Rated power for this winding."),
     ]
     num_phases: Annotated[
         int, Field(..., ge=1, le=3, description="Number of phases for this winding.")
     ]
     connection_type: Annotated[
         ConnectionType,
@@ -63,18 +66,22 @@
     tap_positions: Annotated[
         list[int], Field(..., description="List of tap positions for each phase. Centered at 0.")
     ]
     total_taps: Annotated[
         int, Field(default=32, description="Total number of taps along the bandwidth.")
     ]
     bandwidth: Annotated[
-        PositiveVoltage, Field(..., description="The total voltage bandwidth for the controller")
+        PositiveVoltage,
+        PINT_SCHEMA,
+        Field(..., description="The total voltage bandwidth for the controller"),
     ]
     band_center: Annotated[
-        PositiveVoltage, Field(..., description="The voltage bandcenter on the controller.")
+        PositiveVoltage,
+        PINT_SCHEMA,
+        Field(..., description="The voltage bandcenter on the controller."),
     ]
     max_step: Annotated[
         int,
         Field(
             ge=0,
             description="Maximum number of steps upwards or downwards that can be made per control iteration.",
         ),
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/geometry_branch_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/geometry_branch_equipment.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 
 from pydantic import Field, model_validator
 from infrasys import Component
 
 from gdm.distribution.equipment.bare_conductor_equipment import BareConductorEquipment
 from gdm.distribution.equipment.concentric_cable_equipment import ConcentricCableEquipment
 from gdm.quantities import Distance
+from gdm.constants import PINT_SCHEMA
 
 
 class GeometryBranchEquipment(Component):
     """Interface for geometry branch info."""
 
     conductors: Annotated[
         list[BareConductorEquipment | ConcentricCableEquipment],
         Field(..., description="List of overhead wires or cables."),
     ]
     horizontal_positions: Annotated[
         Distance,
+        PINT_SCHEMA,
         Field(..., description="Horizontal position of the conductor."),
     ]
     vertical_positions: Annotated[
         Distance,
+        PINT_SCHEMA,
         Field(
             ...,
             description="""Vertical position of the conductor.""",
         ),
     ]
 
     @model_validator(mode="after")
@@ -48,10 +51,10 @@
 
     @classmethod
     def example(cls) -> "GeometryBranchEquipment":
         """Example for geometry branch equipment."""
         return GeometryBranchEquipment(
             name="geometry-branch-1",
             conductors=[BareConductorEquipment.example()] * 3,
-            horizontal_positions= Distance([5.6, 6.0, 6.4], "m") * 3,
-            vertical_positions=Distance([5.6, 6.0, 6.4], "m") ,
+            horizontal_positions=Distance([5.6, 6.0, 6.4], "m") * 3,
+            vertical_positions=Distance([5.6, 6.0, 6.4], "m"),
         )
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/inverter_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/inverter_equipment.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,35 @@
 from typing import Annotated, Optional
 
 from infrasys import Component
 from pydantic import Field
 
 from gdm.quantities import PositiveApparentPower, ActivePowerPUTime
 from gdm.distribution.curve import Curve
+from gdm.constants import PINT_SCHEMA
 
 
 class InverterEquipment(Component):
     """Interface for inverter equipment."""
 
     name: Annotated[str, Field("", description="Name of the inverter controller.")]
     capacity: Annotated[
-        PositiveApparentPower, Field(..., description="Apparent power rating for the inverter.")
+        PositiveApparentPower,
+        PINT_SCHEMA,
+        Field(..., description="Apparent power rating for the inverter."),
     ]
     rise_limit: Annotated[
         Optional[ActivePowerPUTime],
+        PINT_SCHEMA,
         Field(..., description="The rise in power output allowed per unit of time"),
     ]
 
     fall_limit: Annotated[
         Optional[ActivePowerPUTime],
+        PINT_SCHEMA,
         Field(..., description="The fall in power output allowed per unit of time"),
     ]
     eff_curve: Annotated[Optional[Curve], Field(None, description="Efficency curve for inverter.")]
 
     @classmethod
     def example(cls) -> "InverterEquipment":
         """Example for load model."""
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/load_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,38 @@
 from gdm.quantities import (
     PositiveResistancePULength,
     ReactancePULength,
     CapacitancePULength,
     PositiveCurrent,
 )
 from gdm.distribution.limitset import ThermalLimitSet
+from gdm.constants import PINT_SCHEMA
 
 
 class MatrixImpedanceBranchEquipment(Component):
     """Interface for impedance based branch."""
 
     r_matrix: Annotated[
         PositiveResistancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length resistance matrix."),
     ]
     x_matrix: Annotated[
         ReactancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length reactance matrix."),
     ]
     c_matrix: Annotated[
         CapacitancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length capacitance matrix."),
     ]
-    ampacity: Annotated[PositiveCurrent, Field(..., description="Ampacity of the conducotr.")]
+    ampacity: Annotated[
+        PositiveCurrent, PINT_SCHEMA, Field(..., description="Ampacity of the conducotr.")
+    ]
     loading_limit: Annotated[
         Optional[ThermalLimitSet],
         Field(None, description="Loading limit set for this conductor."),
     ]
 
     @model_validator(mode="after")
     def validate_fields(self) -> "MatrixImpedanceBranchEquipment":
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from infrasys.quantities import Time
 
 
 from gdm.distribution.equipment.matrix_impedance_branch_equipment import (
     MatrixImpedanceBranchEquipment,
 )
 from gdm.distribution.curve import TimeCurrentCurve
+from gdm.constants import PINT_SCHEMA
 
 
 class MatrixImpedanceFuseEquipment(MatrixImpedanceBranchEquipment):
     """Interface for impedance based fuse equipment."""
 
-    delay: Annotated[Time, Field(description="Delay time before blowing the fuse.")]
+    delay: Annotated[Time, PINT_SCHEMA, Field(description="Delay time before blowing the fuse.")]
     tcc_curve: Annotated[TimeCurrentCurve, Field(description="Time current curve")]
 
     @classmethod
     def example(cls) -> "MatrixImpedanceFuseEquipment":
         """Example for matrix impedance model."""
         return MatrixImpedanceFuseEquipment(
             **MatrixImpedanceBranchEquipment.example().model_dump(exclude_none=True),
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 from typing import Annotated
 
 from pydantic import Field
 
 from gdm.capacitor import PowerSystemCapacitor
 from gdm.quantities import PositiveResistance, PositiveReactance
+from gdm.constants import PINT_SCHEMA
 
 
 class PhaseCapacitorEquipment(PowerSystemCapacitor):
     """Interface for phase capacitor."""
 
     resistance: Annotated[
         PositiveResistance,
+        PINT_SCHEMA,
         Field(
             PositiveResistance(0, "ohm"),
             description="Positive resistance for the capacitor.",
         ),
     ]
     reactance: Annotated[
         PositiveReactance,
+        PINT_SCHEMA,
         Field(
             PositiveReactance(0, "ohm"),
             description="Positive reactance for the capacitor.",
         ),
     ]
 
     @classmethod
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/phase_load_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/phase_load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,44 +8,53 @@
 from gdm.quantities import (
     PositiveCurrent,
     ResistancePULength,
     ReactancePULength,
     CapacitancePULength,
 )
 from gdm.distribution.limitset import ThermalLimitSet
+from gdm.constants import PINT_SCHEMA
 
 
 class SequenceImpedanceBranchEquipment(Component):
     """Interface for sequence impedance branch."""
 
     pos_seq_resistance: Annotated[
         ResistancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length positive sequence resistance."),
     ]
     zero_seq_resistance: Annotated[
         ResistancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length zero sequence impedance."),
     ]
     pos_seq_reactance: Annotated[
         ReactancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length positive sequence impedance."),
     ]
     zero_seq_reactance: Annotated[
         ReactancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length zero sequence impedance."),
     ]
     pos_seq_capacitance: Annotated[
         CapacitancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length positive sequence capacitance."),
     ]
     zero_seq_capacitance: Annotated[
         CapacitancePULength,
+        PINT_SCHEMA,
         Field(..., description="Per unit length zero sequence capacitance."),
     ]
-    ampacity: Annotated[PositiveCurrent, Field(..., description="Ampacity of the conductor.")]
+    ampacity: Annotated[
+        PositiveCurrent, PINT_SCHEMA, Field(..., description="Ampacity of the conductor.")
+    ]
     loading_limit: Annotated[
         Optional[ThermalLimitSet],
         Field(None, description="Loading limit set for this conductor."),
     ]
 
     @classmethod
     def example(cls) -> "SequenceImpedanceBranchEquipment":
```

### Comparing `grid_data_models-0.0.0/src/gdm/distribution/equipment/solar_equipment.py` & `grid_data_models-0.1.0/src/gdm/distribution/equipment/solar_equipment.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 from typing import Annotated
 
 from infrasys import Component
 from pydantic import Field
 
 from gdm.quantities import PositiveActivePower
+from gdm.constants import PINT_SCHEMA
 
 
 class SolarEquipment(Component):
     """Interface for Solar Model."""
 
     rated_capacity: Annotated[
-        PositiveActivePower, Field(..., description="Active power rating of the Solar PV array.")
+        PositiveActivePower,
+        PINT_SCHEMA,
+        Field(..., description="Active power rating of the Solar PV array."),
     ]
 
     solar_power: Annotated[
         PositiveActivePower,
+        PINT_SCHEMA,
         Field(..., description="The DC active power that is generated by the solar equipment."),
     ]
     resistance: Annotated[
         float,
         Field(
             ...,
             strict=True,
```

### Comparing `grid_data_models-0.0.0/.gitignore` & `grid_data_models-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/LICENSE.txt` & `grid_data_models-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.0.0/README.md` & `grid_data_models-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # Grid Data Models (GDM)
 
-GDM is a python package containing [pydantic](https://docs.pydantic.dev/latest/) data models for power system assets and datasets. This package is actively being developed at [National Renewable Energy Laboratory (NREL)](https://www.nrel.gov/).
+GDM is a python package containing data models for power system assets and datasets. This package is actively being developed at [National Renewable Energy Laboratory (NREL)](https://www.nrel.gov/).
+
+## Installation
+
+You can install latest version of `grid-data-models` from PyPi.
+
+```bash
+pip install grid-data-models
+```
+
 
 ## Why Grid Data Models ?
 
-In an effort to reduce code duplication and provide client packages a standard interface to interact with power system data, a group of 
-research engineers at NREL is working on developing standard data models. Features:
+In an effort to reduce code duplication and provide client packages a standard interface to interact with power system data, a group of research engineers at NREL is working on developing standard data models. Features:
 
-- **Builtin validation layer:** Use of [pydantic](https://docs.pydantic.dev/latest/) in creating data models allows us to check for fields during the time of construction and update.
-- **Timeseries data management:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) package which enables attaching time series data to fields in the data model. For example, we can attach time series power consumption data to a load profile.
-- **Builtin unit conversion:** GDM leverages [pint](https://pint.readthedocs.io/en/stable/) for unit conversion for power system quantities. For e.g power, voltage, time etc.
-- **JSON serialization/deserializatin:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) to serialize and deserialize distribution system containing power system components and time series data attached to components.
+- **Built-in validation layer:** Use of [pydantic](https://docs.pydantic.dev/latest/) allows us to validate model fields.
+- **Time series data management:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) package which enables [efficient time series data management](https://nrel.github.io/infrasys/explanation/time_series.html) by sharing arrays across components and offloading system memory. For example, we can attach time series power consumption data to a load profile.
+- **Built-in unit conversion:** GDM leverages [pint](https://pint.readthedocs.io/en/stable/) for unit conversion for power system quantities. For e.g power, voltage, time etc.
+- **JSON serialization/deserialization:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) to serialize and deserialize distribution system components to/from JSON.
 
 ## How to get started ?
 
 To get started, you can clone and pip install this library from [here](https://github.nrel.gov/CADET/grid-data-models).
 
 
 ## Contributors
 
 - **Kapil Duwadi**
 - **Tarek Elgindy**
 - **Aadil Latif**
 - **Pedro Andres Sanchez Perez**
-- **Daniel Thompson**
-- **Jeremy Keen**
+- **Daniel Thom**
+- **Jeremy Keen**
```

### Comparing `grid_data_models-0.0.0/pyproject.toml` & `grid_data_models-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,21 @@
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
 ]
 dependencies = ["networkx", "infrasys"]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "pytest", "pytest-cov", "ruff"]
-doc = ["sphinx", "sphinx-immaterial", "myst-parser", "sphinxcontrib-mermaid"]
+doc = [
+  "sphinx",
+  "pydata-sphinx-theme",
+  "myst-parser",
+  "autodoc_pydantic",
+  "sphinxcontrib-mermaid",
+]
 
 [project.urls]
 Documentation = "https://github.com/NREL-Distribution-Suites/grid-data-models#readme"
 Issues = "https://github.com/NREL-Distribution-Suites/grid-data-models/issues"
 Source = "https://github.com/NREL-Distribution-Suites/grid-data-models"
 
 [tool.ruff]
@@ -38,14 +44,17 @@
 line-length = 99
 indent-width = 4
 target-version = "py311"
 
 [tool.hatch.version]
 path = 'src/gdm/version.py'
 
+[tool.pytest.ini_options]
+pythonpath = "src"
+testpaths = ["tests"]
 
 [tool.ruff.lint]
 # Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
 select = [
   "C901", # McCabe complexity
   "E4",   # Subset of pycodestyle (E)
   "E7",
```

### Comparing `grid_data_models-0.0.0/PKG-INFO` & `grid_data_models-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grid-data-models
-Version: 0.0.0
+Version: 0.1.0
 Project-URL: Documentation, https://github.com/NREL-Distribution-Suites/grid-data-models#readme
 Project-URL: Issues, https://github.com/NREL-Distribution-Suites/grid-data-models/issues
 Project-URL: Source, https://github.com/NREL-Distribution-Suites/grid-data-models
 Author-email: Kapil Duwadi <Kapil.Duwadi@nrel.gov>, Aadil Latif <Aadil.Latif@nrel.gov>, Tarek Elgindy <tarek.elgindy@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: BSD License
@@ -15,40 +15,49 @@
 Requires-Dist: networkx
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: doc
+Requires-Dist: autodoc-pydantic; extra == 'doc'
 Requires-Dist: myst-parser; extra == 'doc'
+Requires-Dist: pydata-sphinx-theme; extra == 'doc'
 Requires-Dist: sphinx; extra == 'doc'
-Requires-Dist: sphinx-immaterial; extra == 'doc'
 Requires-Dist: sphinxcontrib-mermaid; extra == 'doc'
 Description-Content-Type: text/markdown
 
 # Grid Data Models (GDM)
 
-GDM is a python package containing [pydantic](https://docs.pydantic.dev/latest/) data models for power system assets and datasets. This package is actively being developed at [National Renewable Energy Laboratory (NREL)](https://www.nrel.gov/).
+GDM is a python package containing data models for power system assets and datasets. This package is actively being developed at [National Renewable Energy Laboratory (NREL)](https://www.nrel.gov/).
+
+## Installation
+
+You can install latest version of `grid-data-models` from PyPi.
+
+```bash
+pip install grid-data-models
+```
+
 
 ## Why Grid Data Models ?
 
-In an effort to reduce code duplication and provide client packages a standard interface to interact with power system data, a group of 
-research engineers at NREL is working on developing standard data models. Features:
+In an effort to reduce code duplication and provide client packages a standard interface to interact with power system data, a group of research engineers at NREL is working on developing standard data models. Features:
 
-- **Builtin validation layer:** Use of [pydantic](https://docs.pydantic.dev/latest/) in creating data models allows us to check for fields during the time of construction and update.
-- **Timeseries data management:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) package which enables attaching time series data to fields in the data model. For example, we can attach time series power consumption data to a load profile.
-- **Builtin unit conversion:** GDM leverages [pint](https://pint.readthedocs.io/en/stable/) for unit conversion for power system quantities. For e.g power, voltage, time etc.
-- **JSON serialization/deserializatin:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) to serialize and deserialize distribution system containing power system components and time series data attached to components.
+- **Built-in validation layer:** Use of [pydantic](https://docs.pydantic.dev/latest/) allows us to validate model fields.
+- **Time series data management:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) package which enables [efficient time series data management](https://nrel.github.io/infrasys/explanation/time_series.html) by sharing arrays across components and offloading system memory. For example, we can attach time series power consumption data to a load profile.
+- **Built-in unit conversion:** GDM leverages [pint](https://pint.readthedocs.io/en/stable/) for unit conversion for power system quantities. For e.g power, voltage, time etc.
+- **JSON serialization/deserialization:** GDM uses [infrasys](https://github.nrel.gov/CADET/infrastructure_systems) to serialize and deserialize distribution system components to/from JSON.
 
 ## How to get started ?
 
 To get started, you can clone and pip install this library from [here](https://github.nrel.gov/CADET/grid-data-models).
 
 
 ## Contributors
 
 - **Kapil Duwadi**
 - **Tarek Elgindy**
 - **Aadil Latif**
 - **Pedro Andres Sanchez Perez**
-- **Daniel Thompson**
-- **Jeremy Keen**
+- **Daniel Thom**
+- **Jeremy Keen**
```

