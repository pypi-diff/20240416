# Comparing `tmp/GridCalEngine-5.1.6.tar.gz` & `tmp/GridCalEngine-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCalEngine-5.1.6.tar", last modified: Sat Apr 13 14:14:19 2024, max compression
+gzip compressed data, was "GridCalEngine-5.1.7.tar", last modified: Tue Apr 16 20:42:27 2024, max compression
```

## Comparing `GridCalEngine-5.1.6.tar` & `GridCalEngine-5.1.7.tar`

### file list

```diff
@@ -1,678 +1,678 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-12 12:41:14.135810 GridCalEngine-5.1.6/GridCalEngine/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)    11061 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/data_logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39202 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/enumerations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23740 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/basic_structures.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.6/GridCalEngine/api.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/objects_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/timeseries_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9944 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/results_table_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/iwamoto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/ips.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/powell.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/autodiff.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc_numba.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/selected_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/ortools_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/pulp_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/highs.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Topology/topology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21322 2024-04-11 15:31:05.594472 GridCalEngine-5.1.6/GridCalEngine/Topology/simulation_indices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10513 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Topology/topology_substation_reduction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4490 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Topology/detect_substations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.6/GridCalEngine/Topology/admittance_matrices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21396 2024-04-12 07:37:45.923557 GridCalEngine-5.1.6/GridCalEngine/IO/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/base_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/units.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/base_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/base/base_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/dgs/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/dgs/dgs_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/raw/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/gridcal_to_raw.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/gne_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/switched_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/system_switching_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/facts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/owner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/inter_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/vsc_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/induction_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/fixed_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_storage_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_gen_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_bus_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_branch_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    53833 2024-04-12 14:26:56.903899 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/pack_unpack.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16095 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/zip_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    98239 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/json_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/generic_io_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/h5_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    46676 2024-04-13 08:34:01.782415 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/excel_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/sqlite_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/contingency_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/epc/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/epc/epc_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/IO/others/dpx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/others/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/others/ipa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/others/pypsa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/IO/others/plx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    50379 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2227 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30700 2024-04-12 14:39:07.187909 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/base.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12402 2024-04-12 07:37:45.923557 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_export.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26404 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    82071 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2416 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4230 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_devices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/base_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/psse_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/db_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/Devices/types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8637 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/Devices/sparse_array.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/Devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   195588 2024-04-12 14:26:56.931899 GridCalEngine-5.1.6/GridCalEngine/Devices/multi_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14901 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/Devices/profile.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/municipality.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2579 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3864 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2641 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/emission_gas.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/country.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/modelling_authority.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2536 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2069 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1940 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1864 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investments_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3564 2024-04-12 08:49:11.587616 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/community.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/branch_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_path.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8074 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_turbine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_injection_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_p2x.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10753 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/underground_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10243 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/series_reactance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/wire.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5543 2024-04-12 14:41:25.899911 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line_locations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/sequence_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/overhead_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/vsc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/upfc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20073 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/hvdc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15880 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9392 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/winding.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20777 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11768 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer3w.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/static_generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5947 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/external_grid.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5295 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/current_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/battery.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15440 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator_q_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6879 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/controllable_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6848 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2399 2024-04-12 14:04:34.955880 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/graphic_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1078 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/schematic_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12487 2024-04-12 14:04:34.831880 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/base_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14140 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7381 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/injection_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23830 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/editable_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6781 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/generator_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17133 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/controllable_branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5952 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/load_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17273 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7415 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/shunt_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2339 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_emission.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2392 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2260 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/load_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.6/GridCalEngine/DataStructures/bus_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-11 15:31:05.578472 GridCalEngine-5.1.6/GridCalEngine/DataStructures/branch_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_turbine_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_p2x_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    67032 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/DataStructures/numerical_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-04-11 15:31:05.578472 GridCalEngine-5.1.6/GridCalEngine/DataStructures/generator_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_pump_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/battery_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_path_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/DataStructures/hvdc_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/shunt_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_node_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_newton_pa.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_bentayga.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44207 2024-04-11 15:31:05.578472 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_optimods.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_pgm.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/results_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Simulations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Simulations/results_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_processor_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/node_groups_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/blackout_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.6/GridCalEngine/Simulations/InputsAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29937 2024-04-13 08:56:44.442434 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_estimation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26878 2024-04-12 06:51:51.959518 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    78572 2024-04-12 06:58:44.963524 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/linear_opf_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4258 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44173 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54464 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.6/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-13 14:14:19.882700 GridCalEngine-5.1.6/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-13 14:14:19.882700 GridCalEngine-5.1.6/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11061 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/data_logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39620 2024-04-16 15:44:22.519429 GridCalEngine-5.1.7/GridCalEngine/enumerations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24659 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/basic_structures.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.7/GridCalEngine/api.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Utils/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/objects_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/timeseries_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9944 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/results_table_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/iwamoto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15014 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/ips.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/powell.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/autodiff.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/csc_numba.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/csc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Utils/ThirdParty/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.7/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/selected_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/ortools_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/pulp_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/highs.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Topology/topology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21322 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Topology/simulation_indices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10513 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Topology/topology_substation_reduction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4490 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Topology/detect_substations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.7/GridCalEngine/Topology/admittance_matrices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.7/GridCalEngine/IO/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21772 2024-04-16 15:44:22.527428 GridCalEngine-5.1.7/GridCalEngine/IO/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.7/GridCalEngine/IO/base/base_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.7/GridCalEngine/IO/base/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.7/GridCalEngine/IO/base/units.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.7/GridCalEngine/IO/base/base_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/IO/base/base_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/dgs/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/dgs/dgs_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/raw/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/raw/rawx_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/raw/gridcal_to_raw.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/raw/rawx_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/gne_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/switched_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/system_switching_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/psse_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/facts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/owner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/inter_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/psse_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/psse_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/vsc_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/induction_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/fixed_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_storage_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_gen_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/matpower/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_bus_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_branch_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    53833 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/pack_unpack.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17639 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/zip_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    98239 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/json_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/generic_io_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/h5_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    46676 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/excel_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/sqlite_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/contingency_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/epc/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.7/GridCalEngine/IO/epc/epc_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/IO/others/dpx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.7/GridCalEngine/IO/others/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/IO/others/ipa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.7/GridCalEngine/IO/others/pypsa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/IO/others/plx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    50379 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16191 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2227 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30686 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/base.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12402 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_export.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26404 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    82071 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2416 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4230 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_devices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/base_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/psse_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/db_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.7/GridCalEngine/Devices/types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8637 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/sparse_array.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.7/GridCalEngine/Devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   195588 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/multi_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/Devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14901 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/profile.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/municipality.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/contingency_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2579 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3864 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/contingency.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2641 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/emission_gas.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/country.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/modelling_authority.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2536 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2069 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1940 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1864 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/investments_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3564 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/investment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/community.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/branch_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_path.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8074 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_turbine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_injection_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_p2x.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10753 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/underground_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10243 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/series_reactance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/wire.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5543 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/line_locations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/sequence_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/overhead_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/vsc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/upfc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20071 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/hvdc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15880 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9392 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/winding.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20777 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/transformer_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11768 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/transformer3w.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/static_generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5947 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/external_grid.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5295 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/current_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/battery.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15440 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/generator_q_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6879 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/controllable_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6848 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2399 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/graphic_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/map_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1078 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/map_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/schematic_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12510 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/base_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14140 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7381 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/injection_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23830 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/editable_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6781 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/generator_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17133 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/controllable_branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5952 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/load_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17273 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7415 2024-04-16 11:07:46.038900 GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/shunt_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2339 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/generator_emission.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2392 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/generator_technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2260 2024-04-16 11:07:46.034900 GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/generator_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/load_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.7/GridCalEngine/DataStructures/bus_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/DataStructures/branch_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_turbine_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_p2x_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    67032 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/DataStructures/numerical_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10590 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/DataStructures/generator_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_pump_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/battery_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_path_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.7/GridCalEngine/DataStructures/hvdc_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/DataStructures/shunt_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_node_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_newton_pa.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_bentayga.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/Compilers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44207 2024-04-16 11:07:46.030900 GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_optimods.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_pgm.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12757 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/results_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Simulations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Simulations/results_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.7/GridCalEngine/Simulations/driver_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/driver_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/topology_processor_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/node_groups_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/reliability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1318 2024-04-16 13:44:36.655200 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11640 2024-04-16 13:44:36.655200 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/blackout_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8422 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10982 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.7/GridCalEngine/Simulations/InputsAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.7/GridCalEngine/Simulations/Dynamics/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7749 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14622 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29937 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8864 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8826 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3101 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Simulations/StateEstimation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Simulations/StateEstimation/state_estimation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14827 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27057 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    78856 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/linear_opf_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4258 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44243 2024-04-16 11:07:46.042900 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54464 2024-04-16 11:07:46.046900 GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12951 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.7/GridCalEngine/Simulations/ATC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.7/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.7/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.7/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7091 2024-04-16 12:18:07.019034 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-04-16 10:27:10.402822 GridCalEngine-5.1.7/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-16 20:42:27.134153 GridCalEngine-5.1.7/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-16 20:42:27.134153 GridCalEngine-5.1.7/setup.cfg
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/__version__.py` & `GridCalEngine-5.1.7/GridCalEngine/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCalEngine_VERSION__ = "5.1.6"
+__GridCalEngine_VERSION__ = "5.1.7"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCalEngine_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/LICENSE.txt` & `GridCalEngine-5.1.7/GridCalEngine/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/data_logger.py` & `GridCalEngine-5.1.7/GridCalEngine/data_logger.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/enumerations.py` & `GridCalEngine-5.1.7/GridCalEngine/enumerations.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,14 @@
         """
 
         :return:
         """
         return list(map(lambda c: c.value, cls))
 
 
-
 class AcOpfMode(Enum):
     """
     AC-OPF problem types
     """
     ACOPFstd = 'ACOPFstd'
     ACOPFslacks = 'ACOPFslacks'
     ACOPFMaxInjections = 'ACOPFMaxInjections'
@@ -1265,14 +1264,40 @@
         """
         try:
             return LogSeverity[s]
         except KeyError:
             return s
 
 
+class CGMESVersions(Enum):
+    """
+    Enumeration of logs severities
+    """
+    v2_4_15 = '2.4.15'
+    v3_0_0 = '3.0.0'
+
+    def __str__(self):
+        return self.value
+
+    def __repr__(self):
+        return str(self)
+
+    @staticmethod
+    def argparse(s):
+        """
+
+        :param s:
+        :return:
+        """
+        try:
+            return CGMESVersions[s]
+        except KeyError:
+            return s
+
+
 class SparseSolver(Enum):
     """
     Sparse solvers to use
     """
     ILU = 'ILU'
     KLU = 'KLU'
     SuperLU = 'SuperLU'
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/basic_structures.py` & `GridCalEngine-5.1.7/GridCalEngine/basic_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,24 +254,28 @@
 
 class LogEntry:
     """
     Logger entry
     """
 
     def __init__(self,
+                 time: Union[str, None] = None,
                  msg="",
                  severity: LogSeverity = LogSeverity.Information,
                  device="",
                  value="",
                  expected_value="",
                  device_class="",
                  device_property="",
                  object_value=None,
                  expected_object_value=None):
-        self.time = "{date:%H:%M:%S}".format(date=datetime.datetime.now())  # might use %Y/%m/%d %H:%M:%S
+        if time is None:
+            self.time = "{date:%H:%M:%S}".format(date=datetime.datetime.now())  # might use %Y/%m/%d %H:%M:%S
+        else:
+            self.time = time
         self.msg = str(msg)
         self.severity = severity
         self.device = device
         self.device_class = device_class
         self.device_property = device_property
         self.value = value
         self.expected_value = str(expected_value)
@@ -492,14 +496,30 @@
         """
         data = [e.to_list() for e in self.entries]
         df = pd.DataFrame(data=data, columns=['Time', 'Severity', 'Message', 'Class',
                                               'Property', 'Device', 'Value', 'Expected value'])
         df.set_index('Time', inplace=True)
         return df
 
+    def parse_df(self, df: pd.DataFrame):
+        """
+        Parse DataFrame
+        :param df: DataFrame
+        """
+        for i, row in df.iterrows():
+            self.entries.append(LogEntry(msg=str(row["Message"]),
+                                         severity=LogSeverity(row["Severity"]),
+                                         device=str(row["Device"]),
+                                         value=str(row["Value"]),
+                                         expected_value=str(row["Expected value"]),
+                                         device_class=str(row["Class"]),
+                                         device_property=str(row["Property"]),
+                                         object_value="",
+                                         expected_object_value=""))
+
     def to_csv(self, fname):
         """
         Save to CSV
         :param fname: file name
         """
         self.to_df().to_csv(fname)
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/api.py` & `GridCalEngine-5.1.7/GridCalEngine/api.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/objects_filtering.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/objects_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/timeseries_filtering.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/timeseries_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/filtering.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/results_table_filtering.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Filtering/results_table_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/common.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/common.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/ips.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/ips.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         lam_norm = np.linalg.norm(lam, np.Inf)
         mu_norm = np.linalg.norm(mu, np.Inf)
         z_norm = np.linalg.norm(z, np.Inf)
 
         lx = ret.fx + Hx_t @ mu + Gx_t @ lam
         feascond = max([g_norm, max(ret.H)]) / (1 + max([np.linalg.norm(x, np.Inf), z_norm]))
         gradcond = np.linalg.norm(lx, np.Inf) / (1 + max([lam_norm, mu_norm]))
-        error = np.max([feascond, gradcond])
+        error = np.max([feascond, gradcond, gamma])
 
         z_inv = diags(1.0 / z)
         mu_diag = diags(mu)
 
         converged = feascond < tol and gradcond < tol and gamma < tol
 
         if verbose > 1:
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/powell.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/powell.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/autodiff.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/autodiff.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/sparse_solve.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/NumericalMethods/sparse_solve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc_numba.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/csc_numba.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/csc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/utils.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/Sparse/utils.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/selected_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/selected_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/ortools_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/ortools_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/pulp_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/pulp_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/highs.py` & `GridCalEngine-5.1.7/GridCalEngine/Utils/MIP/SimpleMip/highs.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Topology/topology.py` & `GridCalEngine-5.1.7/GridCalEngine/Topology/topology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Topology/simulation_indices.py` & `GridCalEngine-5.1.7/GridCalEngine/Topology/simulation_indices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Topology/topology_substation_reduction.py` & `GridCalEngine-5.1.7/GridCalEngine/Topology/topology_substation_reduction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Topology/detect_substations.py` & `GridCalEngine-5.1.7/GridCalEngine/Topology/detect_substations.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Topology/admittance_matrices.py` & `GridCalEngine-5.1.7/GridCalEngine/Topology/admittance_matrices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/file_handler.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/file_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,39 +44,45 @@
 from GridCalEngine.IO.cim.cgmes.cgmes_to_gridcal import cgmes_to_gridcal
 from GridCalEngine.IO.gridcal.zip_interface import save_gridcal_data_to_zip, get_frames_from_zip
 from GridCalEngine.IO.gridcal.sqlite_interface import save_data_frames_to_sqlite, open_data_frames_from_sqlite
 from GridCalEngine.IO.gridcal.h5_interface import save_h5, open_h5
 from GridCalEngine.IO.raw.rawx_parser_writer import parse_rawx, write_rawx
 from GridCalEngine.IO.others.pypsa_parser import parse_netcdf, parse_hdf5
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
+from GridCalEngine.Simulations.results_template import DriverToSave
+from GridCalEngine.enumerations import CGMESVersions
 
 
 class FileSavingOptions:
     """
     This class is to store the extra stuff that needs to be passed to save more complex files
     """
 
     def __init__(self,
                  cgmes_boundary_set: str = "",
                  simulation_drivers: List[DriverTemplate] = None,
-                 sessions: List[Any] = None,
-                 dictionary_of_json_files: Dict[str, Dict[str, Any]] = None):
+                 sessions_data: List[DriverToSave] = None,
+                 dictionary_of_json_files: Dict[str, Dict[str, Any]] = None,
+                 cgmes_version: CGMESVersions = CGMESVersions.v2_4_15):
         """
         Constructor
         :param cgmes_boundary_set: CGMES boundary set zip file path
         :param simulation_drivers: List of Simulation Drivers
-        :param sessions: List of sessions
+        :param sessions_data: List of sessions_data
         :param dictionary_of_json_files: Dictionary of json files
+        :param cgmes_version: Version to use with CGMES
         """
 
+        self.cgmes_vesrion: CGMESVersions = cgmes_version
+
         self.cgmes_boundary_set: str = cgmes_boundary_set
 
         self.simulation_drivers = simulation_drivers if simulation_drivers else list()
 
-        self.sessions = sessions if sessions else list()
+        self.sessions_data: List[DriverToSave] = sessions_data if sessions_data else list()
 
         self.dictionary_of_json_files = dictionary_of_json_files if dictionary_of_json_files else dict()
 
 
 class FileOpen:
     """
     File open interface
@@ -394,15 +400,15 @@
                                           legacy=False)
 
         model_data = gather_model_as_jsons(self.circuit)
 
         save_gridcal_data_to_zip(dfs=dfs,
                                  filename_zip=self.file_name,
                                  model_data=model_data,
-                                 sessions=self.options.sessions,
+                                 sessions_data=self.options.sessions_data,
                                  diagrams=self.circuit.diagrams,
                                  json_files=self.options.dictionary_of_json_files,
                                  text_func=self.text_func,
                                  progress_func=self.progress_func,
                                  logger=logger)
 
         return logger
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/base/units.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/base/units.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/base/base_property.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/base/base_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/dgs/dgs_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/dgs/dgs_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_legacy.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_functions.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_writer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/rawx_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_writer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_to_gridcal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/raw_to_gridcal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_legacy.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/rawx_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/gne_device.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/gne_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/switched_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/switched_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/system_switching_device.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/system_switching_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_object.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/psse_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/transformer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/facts.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/facts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/owner.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/owner.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/inter_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/inter_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_property.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/psse_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/generator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_circuit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/psse_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/bus.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/vsc_dc_line.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/vsc_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/induction_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/induction_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/fixed_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/fixed_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/load.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/zone.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/branch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/substation.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/raw/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_storage_definitions.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_storage_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_gen_definitions.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_gen_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_bus_definitions.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_bus_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_branch_definitions.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/matpower/matpower_branch_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/pack_unpack.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/pack_unpack.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/zip_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/zip_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,36 @@
 from io import StringIO, TextIOWrapper, BytesIO
 import os
 import numpy as np
 import chardet
 import pandas as pd
 import zipfile
 from warnings import warn
-from typing import List, Dict, Any, Union, Callable
+from typing import List, Dict, Union, Callable
 from GridCalEngine.basic_structures import Logger
 from GridCalEngine.IO.gridcal.generic_io_functions import parse_config_df, CustomJSONizer
+from GridCalEngine.Simulations.results_template import DriverToSave
 import GridCalEngine.Devices as dev
 
 
 def save_gridcal_data_to_zip(dfs: Dict[str, pd.DataFrame],
                              filename_zip: str,
                              model_data: Dict[str, Dict[str, str]],
-                             sessions: List[Any],
+                             sessions_data: List[DriverToSave],
                              diagrams: List[Union[dev.MapDiagram, dev.SchematicDiagram]],
                              json_files: Dict[str, dict],
                              text_func: Union[None, Callable[[str], None]] = None,
                              progress_func: Union[None, Callable[[float], None]] = None,
                              logger=Logger()):
     """
     Save a list of DataFrames to a zip file without saving to disk the csv files
     :param dfs: dictionary of pandas dataFrames {name: DataFrame}
     :param filename_zip: file name where to save all
     :param model_data: dictionary of json data opposed to the dataframes collection
-    :param sessions: SimulationSession instance
+    :param sessions_data: List of DriverToSave instances, representing the results drivers data
     :param diagrams: List of Diagram objects
     :param json_files: List of configuration json files to save Dict[file_name, dictionary to save]
     :param text_func: pointer to function that prints the names
     :param progress_func: pointer to function that prints the progress 0~100
     :param logger: Logger object
     """
 
@@ -62,15 +63,15 @@
 
         # save the GridCal object as json data
         for object_type_name, object_data in model_data.items():
             filename = "model_data/" + object_type_name + ".model"
             try:
                 f_zip_ptr.writestr(filename, json.dumps(object_data, indent=4, cls=CustomJSONizer))
             except TypeError as e:
-                logger.add_error(msg=e, device_class=object_type_name)
+                logger.add_error(msg=str(e), device_class=object_type_name)
                 warn(f"{object_type_name}: {e}")
 
         # save diagrams
         for diagram in diagrams:
             filename = "diagrams/" + diagram.idtag + ".diagram"
             f_zip_ptr.writestr(filename, json.dumps(diagram.get_properties_dict(), indent=4))
 
@@ -111,50 +112,70 @@
                 with StringIO() as buffer:
                     df.to_csv(buffer, index=False)  # save the DataFrame to the buffer
                     f_zip_ptr.writestr(filename, buffer.getvalue())  # save the buffer to the zip file
 
             i += 1
 
         # pre-count the sessions
-        n_items = 0
-        for session in sessions:
-            for drv_name, drv in session.drivers.items():
-                if hasattr(drv, 'results'):
-                    if drv.results is not None:
-                        for arr_name, arr in drv.results.get_arrays().items():
-                            n_items += 1
+        n_items = len(sessions_data)
 
         # save sessions
         i = 0
-        for session in sessions:
-            for drv_name, drv in session.drivers.items():
-                if hasattr(drv, 'results'):
-                    if drv.results is not None:
-                        for arr_name, arr in drv.results.get_arrays().items():
-                            filename = 'sessions/' + session.name + '/' + drv.tpe.value + '/' + arr_name
-
-                            if text_func is not None:
-                                text_func('Flushing ' + filename + ' to ' + filename_zip + '...')
-
-                            with BytesIO() as buffer:
-                                # save the DataFrame to the buffer, protocol4 is to be compatible with python 3.6
-                                np.save(buffer, np.array(arr))  # save the DataFrame to the buffer
-                                f_zip_ptr.writestr(filename + '.npy',
-                                                   buffer.getvalue())  # save the buffer to the zip file
+        for session_data in sessions_data:
 
-                            if progress_func is not None:
-                                progress_func((i + 1) / n_items * 100)
+            if session_data.results is not None:
 
-                            i += 1
+                # traverse the registered results
+                for arr_name, arr_prop in session_data.results.data_variables.items():
+
+                    filename = 'sessions/' + session_data.name + '/' + session_data.tpe.value + '/' + arr_name
+
+                    if text_func is not None:
+                        text_func('Flushing ' + filename + ' to ' + filename_zip + '...')
+
+                    # get the array
+                    arr = getattr(session_data.results, arr_name)
+
+                    with BytesIO() as buffer:
+                        # pack the array into a DataFrame
+
+                        try:
+                            if np.iscomplexobj(arr):
+                                filename += "__complex__"
+                                pd.DataFrame(data=np.c_[arr.real, arr.imag]).to_parquet(buffer)
+                            else:
+                                pd.DataFrame(data=arr).to_parquet(buffer)
+
+                            # save the buffer to the zip file
+                            f_zip_ptr.writestr(filename + ".parquet", buffer.getvalue())
+
+                        except ValueError as e:
+                            warn(str(e))
+
+                    if progress_func is not None:
+                        progress_func((i + 1) / n_items * 100)
+
+                    i += 1
+
+            # save logger
+            if session_data.logger is not None:
+                filename = 'sessions/' + session_data.name + '/' + session_data.tpe.value + '/logger.parquet'
+                with BytesIO() as buffer:
+                    # save the DataFrame to the buffer, protocol4 is to be compatible with python 3.6
+                    session_data.logger.to_df().to_parquet(buffer)
+                    # save the buffer to the zip file
+                    f_zip_ptr.writestr(filename, buffer.getvalue())
 
     if n_failed:
         print('Failed to pickle several profiles, but saved them as csv.\nFor improved speed install Pandas >= 1.2')
 
 
-def read_data_frame_from_zip(file_pointer, extension: str, index_col=None, logger=Logger()):
+def read_data_frame_from_zip(file_pointer,
+                             extension: str,
+                             index_col=None, logger=Logger()) -> Union[None, pd.DataFrame]:
     """
     read DataFrame
     :param file_pointer: Pointer to the file within the zip file
     :param extension: Extension, just to determine the reader method
     :param index_col: Index col (only for config file)
     :param logger:
     :return: Data
@@ -185,14 +206,34 @@
             except ValueError as e:
                 logger.add_error(str(e), device=file_pointer.name)
                 return None
             except AttributeError as e:
                 logger.add_error(str(e) + ' Upgrading pandas might help.', device=file_pointer.name)
                 return None
 
+        elif extension == '.feather':
+            try:
+                return pd.read_feather(file_pointer)
+            except ValueError as e:
+                logger.add_error(str(e), device=file_pointer.name)
+                return None
+            except AttributeError as e:
+                logger.add_error(str(e) + ' Upgrading pandas might help.', device=file_pointer.name)
+                return None
+
+        elif extension == '.hdf':
+            try:
+                return pd.read_hdf(file_pointer, key='array')
+            except ValueError as e:
+                logger.add_error(str(e), device=file_pointer.name)
+                return None
+            except AttributeError as e:
+                logger.add_error(str(e) + ' Upgrading pandas might help.', device=file_pointer.name)
+                return None
+
     except EOFError:
         logger.add_error("EOF error", device=file_pointer.name)
         return None
     except zipfile.BadZipFile:
         logger.add_error("Bad zip file error", device=file_pointer.name)
         return None
 
@@ -205,27 +246,27 @@
     Open the csv files from a zip file
     :param file_name_zip: name of the zip file
     :param text_func: pointer to function that prints the names
     :param progress_func: pointer to function that prints the progress 0~100
     :param logger:
     :return: list of DataFrames
     """
+    data = {'diagrams': list(),
+            'model_data': dict()}
+    json_files = dict()
 
     # open the zip file
     try:
         zip_file_pointer = zipfile.ZipFile(file_name_zip)
     except zipfile.BadZipFile:
-        return None
+        return data, json_files
 
     names = zip_file_pointer.namelist()
 
     n = len(names)
-    data = {'diagrams': list(),
-            'model_data': dict()}
-    json_files = dict()
 
     # for each file in the zip file...
     for i, file_name in enumerate(names):
 
         # split the file name into name and extension
         name, extension = os.path.splitext(file_name)
 
@@ -325,30 +366,32 @@
                     data[session_name][study_name] = list()
 
                 data[session_name][study_name].append(array_name)
 
     return data
 
 
-def load_session_driver_objects(file_name_zip: str, session_name: str, study_name: str):
+def load_session_driver_objects(file_name_zip: str,
+                                session_name: str,
+                                study_name: str) -> Dict[str, Union[None, pd.DataFrame]]:
     """
     Get the sessions structure
     :param file_name_zip:
     :param session_name:
     :param study_name:
-    :return:
+    :return: Dict[str, Union[None, pd.DataFrame]]
     """
     try:
         zip_file_pointer = zipfile.ZipFile(file_name_zip)
     except zipfile.BadZipFile:
         return dict()
 
     data = dict()
 
-    # traverse the zip names and pick all those that start with sessions/session_name/study_name
+    # traverse the zip names and pick all those that start with sessions_data/session_name/study_name
     for name in zip_file_pointer.namelist():
         if '/' in name:
             path = name.split('/')
             if len(path) > 3:
                 if path[0].lower() == 'sessions' and session_name == path[1] and study_name == path[2]:
                     # create a buffer to read the file
                     file_pointer = zip_file_pointer.open(name)
@@ -356,53 +399,48 @@
                     # split the file name into name and extension
                     _, extension = os.path.splitext(name)
                     arr_name = path[3].replace(extension, '')
 
                     # read the data
                     data[arr_name] = read_data_frame_from_zip(file_pointer, extension)
 
-                    # try:
-                    #     data[arr_name] = np.load(file_pointer)
-                    # except ValueError:
-                    #     data[arr_name] = np.load(file_pointer, allow_pickle=True)
-
     return data
 
 
-def get_xml_content(file_ptr):
+def get_xml_content(file_ptr: zipfile.ZipExtFile) -> List[str]:
     """
     Reads the content of a file
     :param file_ptr: File pointer (from file or zip file)
     :return: list of text lines
     """
     # xml files always have the encoding declared, find it out
     first_line = file_ptr.readline()
 
     if b'encoding' in first_line:
         encoding = first_line.split()[2].split(b'=')[1].replace(b'"', b'').replace(b'?>', b'').decode()
     else:
         try:
             detection = chardet.detect(first_line)
             encoding = detection['encoding']
-        except:
+        except TypeError:
             encoding = 'utf-8'
 
     # sequential back to the start
     file_ptr.seek(0)
 
     # read all the lines
     with TextIOWrapper(file_ptr, encoding=encoding) as fle:
         text_lines = [l for l in fle]
 
     return text_lines
 
 
 def get_xml_from_zip(file_name_zip: str,
                      text_func: Union[None, Callable[[str], None]] = None,
-                     progress_func: Union[None, Callable[[float], None]] = None,):
+                     progress_func: Union[None, Callable[[float], None]] = None, ):
     """
     Get the .xml files from a zip file
     :param file_name_zip: name of the zip file
     :param text_func: pointer to function that prints the names
     :param progress_func: pointer to function that prints the progress 0~100
     :return: list of xml file contents
     """
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/json_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/json_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/generic_io_functions.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/generic_io_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/h5_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/h5_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/excel_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/excel_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/sqlite_interface.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/sqlite_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/contingency_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/gridcal/contingency_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/epc/epc_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/epc/epc_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/others/dpx_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/others/dpx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/others/ipa_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/others/ipa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/others/pypsa_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/others/pypsa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/others/plx_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/others/plx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_enums.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,26 +352,31 @@
                 model_keys = list(file_cgmes_data['FullModel'])
 
                 if len(model_keys) == 1:  # there must be exacly one FullModel
                     model_info = file_cgmes_data['FullModel'][model_keys[0]]
                     self.parsed_data[file_name] = file_cgmes_data
                     profile = model_info.get('profile', '')
 
-                    for prof in profile:
-                        if prof in cgmes2_4_15_uri:
-                            self.cgmes_version = "2.4.15"
-                        elif prof in cgmes3_0_0_uri:
-                            self.cgmes_version = "3.0.0"
-
                     if isinstance(profile, list):
+                        for prof in profile:
+                            if prof in cgmes2_4_15_uri:
+                                self.cgmes_version = "2.4.15"
+                            elif prof in cgmes3_0_0_uri:
+                                self.cgmes_version = "3.0.0"
+
                         if 'Boundary' in profile[0]:
                             merge(self.boudary_set, file_cgmes_data, self.logger)
                         else:
                             merge(self.data, file_cgmes_data, self.logger)
                     else:
+                        if profile in cgmes2_4_15_uri:
+                            self.cgmes_version = "2.4.15"
+                        elif profile in cgmes3_0_0_uri:
+                            self.cgmes_version = "3.0.0"
+
                         if 'Boundary' in profile:
                             merge(self.boudary_set, file_cgmes_data, self.logger)
                         else:
                             merge(self.data, file_cgmes_data, self.logger)
 
                 else:
                     self.logger.add_error("File does not contain exactly one FullModel",
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_writer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
             else:
                 logger.add_error(msg='No TopologinalNode found',
                                  device=cn.name,
                                  device_class=cn.tpe)
         else:
             logger.add_error(msg='Connectivity Node has no default bus',
                              device=mc_elm.name,
-                             device_class=gcdev.ConnectivityNode.type_name)
+                             device_class=mc_elm.device_type)
             # print(f'Topological node not found for cn: {cn.name}')
 
         cgmes_model.add(cn)
 
     return
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/base.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/base.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_export.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_export.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_utils.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_utils.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_circuit.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_devices.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_devices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_enums.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_data_parser.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/cim16/cim_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/base_db.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/base_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/cgmes_lookup_db.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/cgmes_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/file_system.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/file_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/psse_lookup_db.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/psse_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/db_handler.py` & `GridCalEngine-5.1.7/GridCalEngine/IO/cim/db/db_handler.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/types.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/sparse_array.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/sparse_array.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/multi_circuit.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/multi_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/measurement.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/profile.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/profile.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/municipality.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/municipality.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency_group.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/contingency_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/fuel.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/contingency.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/emission_gas.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/emission_gas.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/country.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/country.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/modelling_authority.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/modelling_authority.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/region.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/area.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/technology.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/technology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/zone.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investments_group.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/investments_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investment.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/investment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/community.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/community.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/branch_group.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Aggregation/branch_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_path.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_path.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_pump.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_node.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_turbine.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_turbine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_injection_template.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_injection_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_p2x.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Fluid/fluid_p2x.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/dc_line.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/underground_line_type.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/underground_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/series_reactance.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/series_reactance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/wire.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/wire.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line_locations.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/line_locations.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/sequence_line_type.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/sequence_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/overhead_line_type.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/overhead_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/switch.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/vsc.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/vsc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/upfc.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/upfc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/hvdc_line.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/hvdc_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 class HvdcLine(BranchParent):
     """
     HvdcLine
     """
 
     def __init__(self, bus_from: Bus = None, bus_to: Bus = None, name='HVDC Line', idtag=None, active=True, code='',
                  rate=1.0, Pset=0.0, r=1e-20, loss_factor=0.0, Vset_f=1.0, Vset_t=1.0, length=1.0, mttf=0.0, mttr=0.0,
-                 overload_cost=1000.0,   min_firing_angle_f=-1.0, max_firing_angle_f=1.0, min_firing_angle_t=-1.0,
+                 overload_cost=1000.0, min_firing_angle_f=-1.0, max_firing_angle_f=1.0, min_firing_angle_t=-1.0,
                  max_firing_angle_t=1.0, contingency_factor=1.0, protection_rating_factor: float = 1.4,
                  control_mode: HvdcControlType = HvdcControlType.type_1_Pset, dispatchable=True, angle_droop=0,
                  capex=0, opex=0, build_status: BuildStatus = BuildStatus.Commissioned, n_lines: int = 1):
         """
         HVDC Line model
         :param bus_from: Bus from
         :param bus_to: Bus to
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/tap_changer.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/winding.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/winding.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/branch.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer_type.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/transformer_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer3w.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Branches/transformer3w.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/static_generator.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/static_generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/external_grid.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/external_grid.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/current_injection.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/current_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/battery.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/battery.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator_q_curve.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/generator_q_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/controllable_shunt.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/controllable_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/load.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Injections/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/graphic_location.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/graphic_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_diagram.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/map_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_location.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/map_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/schematic_diagram.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/schematic_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/base_diagram.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Diagrams/base_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,26 +85,27 @@
                    data: Dict[str, Dict[str, Union[int, float, bool, List[Tuple[float, float]]]]],
                    obj_dict: Dict[str, ALL_DEV_TYPES],
                    logger: Logger,
                    category: str = "") -> None:
         """
         Parse file data ito this class
         :param data: json dictionary
-        :param obj_dict: dicrtionary of relevant objects (idtag, object)
+        :param obj_dict: dictionary of relevant objects (idtag, object)
         :param logger: Logger
         :param category: category
         """
         self.locations = dict()
 
         for idtag, location in data.items():
 
             api_object = obj_dict.get(idtag, None)
 
             if api_object is None:
                 # locations with no API object are not created
+                print()
                 logger.add_error("Diagram location could not find API object",
                                  device_class=category,
                                  device=idtag,)
             else:
                 if 'x' in location:
                     self.locations[idtag] = GraphicLocation(x=location['x'],
                                                             y=location['y'],
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/connectivity_node.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/voltage_level.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/bus.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/busbar.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/substation.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Substation/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/injection_parent.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/injection_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/editable_device.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/editable_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/generator_parent.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/generator_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/controllable_branch_parent.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/controllable_branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/load_parent.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/load_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/branch_parent.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/shunt_parent.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Parents/shunt_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_emission.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/generator_emission.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_technology.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/generator_technology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_fuel.py` & `GridCalEngine-5.1.7/GridCalEngine/Devices/Associations/generator_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/load_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/load_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/bus_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/bus_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/branch_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/branch_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_turbine_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_turbine_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_p2x_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_p2x_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/numerical_circuit.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/numerical_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/generator_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/generator_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -302,7 +302,23 @@
 
     def get_dispatchable_indices(self) -> IntVec:
         """
         Get the indices of dispatchable generators
         :return:
         """
         return np.where(self.dispatchable == 1)[0]
+
+    def get_dispatchable_active_indices(self) -> IntVec:
+        """
+        Get the indices of dispatchable generators
+        :return:
+        """
+        x = (self.dispatchable * self.active).astype(int)
+        return np.where(x == 1)[0]
+
+    def get_non_dispatchable_indices(self) -> IntVec:
+        """
+        Get the indices of dispatchable generators
+        :return:
+        """
+        x = (~self.dispatchable * self.active).astype(int)
+        return np.where(x == 1)[0]
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_pump_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_pump_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/battery_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/battery_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_path_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_path_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/hvdc_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/hvdc_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/shunt_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/shunt_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_node_data.py` & `GridCalEngine-5.1.7/GridCalEngine/DataStructures/fluid_node_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_newton_pa.py` & `GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_newton_pa.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_bentayga.py` & `GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_bentayga.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Compilers/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_data.py` & `GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_optimods.py` & `GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_optimods.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_pgm.py` & `GridCalEngine-5.1.7/GridCalEngine/Compilers/circuit_to_pgm.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/results_template.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/results_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 import json
 import numpy as np
+import pandas as pd
 from typing import List, Dict, Union, TYPE_CHECKING
 
 from GridCalEngine.Simulations.results_table import ResultsTable
-from GridCalEngine.basic_structures import IntVec, Vec, CxVec, StrVec, Mat, DateVec, CxMat
+from GridCalEngine.basic_structures import IntVec, Vec, CxVec, StrVec, Mat, DateVec, CxMat, Logger
 from GridCalEngine.enumerations import StudyResultsType, ResultTypes
+from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
     from GridCalEngine.Simulations.Clustering.clustering_results import ClusteringResults
 
 
 class ResultsProperty:
@@ -69,15 +71,15 @@
         :param clustering_results: ClusteringResults object (optional)
         :param study_results_type: StudyResultsType Instance
         """
         self.name: str = name
 
         self.study_results_type: StudyResultsType = study_results_type
 
-        self.available_results: Dict[ResultTypes: List[ResultTypes]] = available_results
+        self.available_results: Dict[ResultTypes, List[ResultTypes]] = available_results
 
         self.data_variables: Dict[str, ResultsProperty] = dict()
 
         self.time_array: Union[DateVec, None] = time_array
 
         if clustering_results:
             self.clustering_results = clustering_results
@@ -156,22 +158,14 @@
             for key, values in self.available_results.items():
                 d[key.value] = [x.value for x in values]
         if isinstance(self.available_results, list):
             d = [x.value for x in self.available_results]
 
         return d
 
-    def get_arrays(self):
-        """
-        Get a dictionary with the array name and the actual array of the class (it also works with the derived class)
-        :return: {array_name: array}
-        """
-        property_names = [p for p in dir(self) if isinstance(getattr(self, p), np.ndarray)]
-        return {var_name: getattr(self, var_name) for var_name in property_names}
-
     def to_json(self, file_name):
         """
         Export as json
         :param file_name: File name
         """
 
         with open(file_name, "w") as output_file:
@@ -339,7 +333,69 @@
                                 setattr(self, prop, arr)  # overwrite the array
                         else:
                             pass
                             # print(prop, value.ndim, value.dtype)
                     else:
                         pass
                         # print(prop, value.ndim, value.dtype)
+
+    def parse_saved_data(self, grid: MultiCircuit, data_dict: Dict[str, pd.DataFrame]) -> None:
+        """
+
+        :param grid: MultiCircuit
+        :param data_dict: Dictionary with the info loaded from disk
+        :return:
+        """
+        self.time_array = grid.get_time_array()
+
+        for arr_name, df in data_dict.items():
+
+            is_complex = '__complex__' in arr_name
+            arr_name = arr_name.replace('__complex__', '')
+
+            # try to get the property of the saved file
+            res_prop: ResultsProperty = self.data_variables.get(arr_name, None)
+
+            if df is not None and res_prop is not None:
+
+                # it may be complex...
+                if is_complex:
+                    split_pt = int(df.columns.size / 2)
+                    r = df.values[:, :split_pt]
+                    i = df.values[:, split_pt:]
+                    array = r + 1j * i
+                else:
+                    # keep the 2D shape
+                    array = df.values
+
+                if array.shape[1] == 1:
+                    # if there is only one column, convert to array directly
+                    array = array[:, 0]
+
+                # it may be a single number...
+                if res_prop.tpe in [int, float, complex]:
+                    if array.size == 1:
+                        array = array[0]
+
+                setattr(self, res_prop.name, array)
+
+
+class DriverToSave:
+    """
+    Wrapper to save a driver
+    """
+    def __init__(self,
+                 name: str,
+                 tpe: SimulationTypes,
+                 results: ResultsTemplate,
+                 logger: Logger):
+        """
+
+        :param name:
+        :param tpe:
+        :param results:
+        :param logger:
+        """
+        self.name = name
+        self.tpe = tpe
+        self.results = results
+        self.logger = logger
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/results_table.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/results_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_types.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/driver_types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_template.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/driver_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_reduction_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/topology_reduction_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_processor_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/topology_processor_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/node_groups_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Topology/node_groups_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/reliability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # Lesser General Public License for more details.
 # 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from GridCalEngine.Simulations.Stochastic.stochastic_power_flow_driver import StochasticPowerFlowDriver, StochasticPowerFlowResults, StochasticPowerFlowInput, StochasticPowerFlowType
-from GridCalEngine.Simulations.Stochastic.blackout_driver import Cascading, CascadingResults, CascadeType, CascadingReportElement
+from GridCalEngine.Simulations.Stochastic.blackout_driver import CascadingDriver, CascadingResults, CascadeType, CascadingReportElement
 from GridCalEngine.Simulations.Stochastic.reliability_driver import ReliabilityStudy
 from GridCalEngine.Simulations.Stochastic.reliability_iterable import ReliabilityIterable, get_transition_probabilities
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_iterable.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/reliability_iterable.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/blackout_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/blackout_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     def plot(self):
 
         # TODO: implement cascading plot
         pass
 
 
-class Cascading(DriverTemplate):
+class CascadingDriver(DriverTemplate):
     tpe = SimulationTypes.Cascade_run
 
     # TODO: re-make this simulation class
 
     def __init__(self, grid: MultiCircuit, options: PowerFlowOptions, triggering_idx=None, max_additional_islands=1,
                  cascade_type_: CascadeType = CascadeType.LatinHypercube, n_lhs_samples_=1000):
         """
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,20 @@
 
         self.batch_size = batch_size
 
         self.max_sampling_points = sampling_points
 
         self.simulation_type = simulation_type
 
-        self.results = None
+        self.results = StochasticPowerFlowResults(n=0,
+                                                  m=0,
+                                                  p=0,
+                                                  bus_names=np.empty(0),
+                                                  branch_names=np.empty(0),
+                                                  bus_types=np.empty(0))
 
         self.logger = Logger()
 
         self.pool = None
 
         self.returned_results = list()
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,25 @@
             engine=engine
         )
 
         self.options = PowerFlowOptions() if options is None else options
 
         self.opf_time_series_results = opf_time_series_results
 
+        self.results = PowerFlowTimeSeriesResults(n=0,
+                                                  m=0,
+                                                  n_hvdc=0,
+                                                  bus_names=np.empty(0),
+                                                  branch_names=np.empty(0),
+                                                  hvdc_names=np.empty(0),
+                                                  time_array=np.empty(0),
+                                                  bus_types=np.empty(0),
+                                                  area_names=None,
+                                                  clustering_results=None)
+
     def run_single_thread(self, time_indices) -> PowerFlowTimeSeriesResults:
         """
         Run single thread time series
         :param time_indices: array of time indices to consider
         :return: TimeSeriesResults instance
         """
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/grid_analysis.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/grid_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/dynamic_modules.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Dynamics/dynamic_modules.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,53 +26,58 @@
 from GridCalEngine.Simulations.driver_template import DriverTemplate
 
 
 class ContinuationPowerFlowDriver(DriverTemplate):
     name = 'Continuation Power Flow'
     tpe = SimulationTypes.ContinuationPowerFlow_run
 
-    def __init__(self, circuit: MultiCircuit,
+    def __init__(self, grid: MultiCircuit,
                  options: ContinuationPowerFlowOptions,
                  inputs: ContinuationPowerFlowInput,
                  pf_options: PowerFlowOptions,
                  opf_results=None, t=0):
         """
         ContinuationPowerFlowDriver constructor
-        :param circuit: NumericalCircuit instance
+        :param grid: NumericalCircuit instance
         :param options: ContinuationPowerFlowOptions instance
         :param inputs: ContinuationPowerFlowInput instance
         :param pf_options: PowerFlowOptions instance
         :param opf_results:
         """
 
-        DriverTemplate.__init__(self, grid=circuit)
+        DriverTemplate.__init__(self, grid=grid)
 
         # voltage stability options
         self.options = options
 
         self.inputs = inputs
 
         self.pf_options = pf_options
 
         self.opf_results = opf_results
 
         self.t = t
 
-        self.results = None
+        self.results = ContinuationPowerFlowResults(nval=0,
+                                                    nbus=0,
+                                                    nbr=0,
+                                                    bus_names=[],
+                                                    branch_names=[],
+                                                    bus_types=[])
 
     def get_steps(self):
         """
         List of steps
         """
         if self.results.lambdas is not None:
             return ['Lambda:' + str(l) for l in self.results.lambdas]
         else:
             return list()
 
-    def progress_callback(self, lmbda):
+    def progress_callback(self, lmbda: float) -> None:
         """
         Send progress report
         :param lmbda: lambda value
         :return: None
         """
         self.report_text('Running continuation power flow (lambda:' + "{0:.2f}".format(lmbda) + ')...')
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,23 @@
         self.pf_options = pf_options
 
         self.opf_results = opf_results
 
         # Options to use
         self.options = options
 
-        self.results: ShortCircuitResults = None
+        # declare an empty results object
+        self.results: ShortCircuitResults = ShortCircuitResults(n=0,
+                                                                m=0,
+                                                                n_hvdc=0,
+                                                                bus_names=np.empty(0),
+                                                                branch_names=np.empty(0),
+                                                                hvdc_names=np.empty(0),
+                                                                bus_types=np.empty(0),
+                                                                area_names=None)
 
         self.logger = Logger()
 
         self.__cancel__ = False
 
         self._is_running = False
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_opf.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_opf.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/NTC/ntc_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from GridCalEngine.Simulations.ContingencyAnalysis.contingency_analysis_options import ContingencyAnalysisOptions
 from GridCalEngine.Simulations.ContingencyAnalysis.contingency_analysis_driver import ContingencyAnalysisDriver
 from GridCalEngine.Simulations.ContingencyAnalysis.contingency_analysis_results import ContingencyAnalysisResults
-from GridCalEngine.Simulations.ContingencyAnalysis.contingency_analysis_ts_driver import ContingencyAnalysisTimeSeries
+from GridCalEngine.Simulations.ContingencyAnalysis.contingency_analysis_ts_driver import ContingencyAnalysisTimeSeriesDriver
 from GridCalEngine.Simulations.ContingencyAnalysis.contingency_analysis_ts_results import ContingencyAnalysisTimeSeriesResults
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
             msg_srap: str,
             srap_power: float,
             solved_by_srap: bool = False):
 
         """
         Add report data
         :param time_index:
-        :param t_prob_
+        :param t_prob:
         :param area_from:
         :param area_to:
         :param base_name:
         :param contingency_name:
         :param base_rating:
         :param contingency_rating:
         :param srap_rating:
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCalEngine.Simulations.driver_template import TimeSeriesDriverTemplate
 from GridCalEngine.Simulations.Clustering.clustering_results import ClusteringResults
 from GridCalEngine.Compilers.circuit_to_newton_pa import newton_pa_contingencies, translate_contingency_report
 from GridCalEngine.Utils.NumericalMethods.weldorf_online_stddev import WeldorfOnlineStdDevMat
 
 
-class ContingencyAnalysisTimeSeries(TimeSeriesDriverTemplate):
+class ContingencyAnalysisTimeSeriesDriver(TimeSeriesDriverTemplate):
     """
     Contingency Analysis Time Series
     """
     name = 'Contingency analysis time series'
     tpe = SimulationTypes.ContingencyAnalysisTS_run
 
     def __init__(self,
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
                                  ramp_constraints=False,
                                  all_generators_fixed=True,
                                  lodf_threshold=options.lin_options.lodf_threshold,
                                  maximize_inter_area_flow=False,
                                  areas_from=list(),
                                  areas_to=list(),
                                  energy_0=None,
+                                 fluid_level_0=None,
                                  logger=logger,
                                  export_model_fname=None)
 
     # for each contingency group
     for ic, multi_contingency in enumerate(linear_multiple_contingencies.multi_contingencies):
 
         if multi_contingency.has_injection_contingencies():
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/Clustering/clustering_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
+import numpy as np
 from typing import Union
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCalEngine.Simulations.driver_template import DriverTemplate
 from GridCalEngine.Simulations.Clustering.clustering_results import ClusteringResults
 from GridCalEngine.Simulations.Clustering.clustering_options import ClusteringAnalysisOptions
 from GridCalEngine.Simulations.Clustering.clustering import kmeans_sampling
@@ -34,15 +35,18 @@
         :param grid: Multicircuit instance
         :param options: ClusteringAnalysisOptions
         """
         DriverTemplate.__init__(self, grid=grid)
 
         self.options: ClusteringAnalysisOptions = options
 
-        self.results: Union[ClusteringResults, None] = None
+        self.results: Union[ClusteringResults, None] = ClusteringResults(time_indices=np.empty(0, dtype=int),
+                                                                         sampled_probabilities=np.empty(0),
+                                                                         time_array=np.empty(0),
+                                                                         original_sample_idx=np.empty(0, dtype=int))
 
     def run(self):
         """
         Run thread
         """
         self.tic()
         self.report_text("Clustering")
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_estimation.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/StateEstimation/state_estimation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
                                          ramp_constraints=False,
                                          all_generators_fixed=False,
                                          lodf_threshold=self.options.lodf_tolerance,
                                          maximize_inter_area_flow=self.options.maximize_flows,
                                          areas_from=self.options.areas_from,
                                          areas_to=self.options.areas_to,
                                          energy_0=None,
+                                         fluid_level_0=None,
                                          logger=self.logger,
                                          export_model_fname=self.options.export_model_fname)
 
             self.results.voltage = np.ones(opf_vars.nbus) * np.exp(1j * opf_vars.bus_vars.theta[0, :])
             self.results.bus_shadow_prices = opf_vars.bus_vars.shadow_prices[0, :]
             self.results.load_shedding = opf_vars.load_vars.shedding[0, :]
             self.results.battery_power = opf_vars.batt_vars.p[0, :]
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_ts_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,15 @@
             ngen=self.grid.get_generators_number(),
             nbat=self.grid.get_batteries_number(),
             nload=self.grid.get_loads_number(),
             nhvdc=self.grid.get_hvdc_number(),
             n_fluid_node=self.grid.get_fluid_nodes_number(),
             n_fluid_path=self.grid.get_fluid_paths_number(),
             n_fluid_injection=self.grid.get_fluid_injection_number(),
-            time_array=self.grid.time_profile[self.time_indices] if self.time_indices is not None else [
-                datetime.datetime.now()],
+            time_array=self.grid.time_profile[self.time_indices] if self.time_indices is not None else [datetime.datetime.now()],
             bus_types=np.ones(self.grid.get_bus_number(), dtype=int),
             clustering_results=clustering_results)
 
         self.all_solved = True
 
     @property
     def pf_options(self) -> PowerFlowOptions:
@@ -263,14 +262,15 @@
 
         # get the partition points of the time series
         groups = get_time_groups(t_array=self.grid.time_profile[self.time_indices], grouping=self.options.grouping)
 
         n = len(groups)
         i = 1
         energy_0: Union[Vec, None] = None  # at the beginning
+        fluid_level_0: Union[Vec, None] = None
 
         while i < n and not self.__cancel__:
             start_ = groups[i - 1]
             end_ = groups[i]
 
             # Grab the last time index in the last group
             if i == n - 1:
@@ -295,14 +295,15 @@
                                          ramp_constraints=self.options.unit_commitment,
                                          all_generators_fixed=False,
                                          lodf_threshold=self.options.lodf_tolerance,
                                          maximize_inter_area_flow=self.options.maximize_flows,
                                          areas_from=self.options.areas_from,
                                          areas_to=self.options.areas_to,
                                          energy_0=energy_0,
+                                         fluid_level_0=fluid_level_0,
                                          logger=self.logger,
                                          export_model_fname=self.options.export_model_fname)
 
             self.results.voltage[time_indices, :] = (np.ones((opf_vars.nt, opf_vars.nbus))
                                                      * np.exp(1j * opf_vars.bus_vars.theta))
             self.results.bus_shadow_prices[time_indices, :] = opf_vars.bus_vars.shadow_prices
 
@@ -340,14 +341,15 @@
             self.results.system_emissions[time_indices, :] = opf_vars.sys_vars.system_emissions
             self.results.system_energy_cost[time_indices] = opf_vars.sys_vars.system_energy_cost
 
             # set converged for all t to the value of acceptable solution
             self.results.converged[time_indices] = np.array([opf_vars.acceptable_solution] * opf_vars.nt)
 
             energy_0 = self.results.battery_energy[end_ - 1, :]
+            fluid_level_0 = self.results.fluid_node_current_level[end_ - 1, :]
 
             # update progress bar
             self.report_progress2(i, len(groups))
 
             i += 1
 
     def add_report(self, eps: float = 1e-6) -> None:
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/linear_opf_ts.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/linear_opf_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -996,15 +996,15 @@
     Formulate the branches
     :param t: time index
     :param Sbase: base power (100 MVA)
     :param branch_data_t: BranchData
     :param branch_vars: BranchVars
     :param bus_vars: BusVars
     :param prob: OR problem
-    :param inf: number considered infinte
+    :param inf: number considered infinite
     :return objective function
     """
     f_obj = 0.0
 
     # for each branch
     for m in range(branch_data_t.nelm):
         fr = branch_data_t.F[m]
@@ -1281,14 +1281,15 @@
                           node_data: FluidNodeData,
                           path_data: FluidPathData,
                           turbine_data: FluidTurbineData,
                           pump_data: FluidPumpData,
                           p2x_data: FluidP2XData,
                           generator_data: GeneratorData,
                           generator_vars: GenerationVars,
+                          fluid_level_0: Vec,
                           prob: LpModel,
                           logger: Logger):
     """
     Formulate the branches
     :param t: local time index
     :param time_global_tidx: global time index
     :param time_array: list of time indices
@@ -1299,14 +1300,15 @@
     :param node_data: FluidNodeData
     :param path_data: FluidPathData
     :param turbine_data: FluidTurbineData
     :param pump_data: FluidPumpData
     :param p2x_data: FluidP2XData
     :param generator_data: GeneratorData
     :param generator_vars: GeneratorVars
+    :param fluid_level_0: Initial node level
     :param prob: OR problem
     :param logger: log of the LP
     :return objective function
     """
 
     f_obj = 0.0
 
@@ -1406,22 +1408,22 @@
 
         # f_obj -= p2x_flow
 
     if time_global_tidx is not None:
         # constraints for the node level
         for m in range(node_data.nelm):
             if t == 0:
-                # Initialize level at the initial one (from snapshot), akin to dt=0
                 if len(time_array) > time_global_tidx + 1:
                     dt = (time_array[time_global_tidx + 1] - time_array[time_global_tidx]).seconds
                 else:
                     dt = 3600
 
+                # Initialize level at fluid_level_0
                 prob.add_cst(cst=(node_vars.current_level[t, m] ==
-                                  node_data.initial_level[m]
+                                  fluid_level_0[m]
                                   + dt * node_data.inflow[m]
                                   + dt * node_vars.flow_in[t, m]
                                   + dt * node_vars.p2x_flow[t, m]
                                   - dt * node_vars.spillage[t, m]
                                   - dt * node_vars.flow_out[t, m]),
                              name=join("nodal_balance_", [t, m], "_"))
             else:
@@ -1449,14 +1451,15 @@
                       ramp_constraints: bool = False,
                       all_generators_fixed: bool = False,
                       lodf_threshold: float = 0.001,
                       maximize_inter_area_flow: bool = False,
                       areas_from: List[Area] = None,
                       areas_to: List[Area] = None,
                       energy_0: Union[Vec, None] = None,
+                      fluid_level_0: Union[Vec, None] = None,
                       logger: Logger = Logger(),
                       progress_text: Union[None, Callable[[str], None]] = None,
                       progress_func: Union[None, Callable[[float], None]] = None,
                       export_model_fname: Union[None, str] = None) -> OpfVars:
     """
     Run linear optimal power flow
     :param grid: MultiCircuit instance
@@ -1470,14 +1473,15 @@
     :param all_generators_fixed: All generators take their snapshot or profile values
                                  instead of resorting to dispatcheable status
     :param lodf_threshold:
     :param maximize_inter_area_flow:
     :param areas_from:
     :param areas_to:
     :param energy_0:
+    :param fluid_level_0: initial fluid level of the nodes
     :param logger: logger instance
     :param progress_text:
     :param progress_func:
     :param export_model_fname: Export the model into LP and MPS?
     :return: OpfVars
     """
     bus_dict = {bus: i for i, bus in enumerate(grid.buses)}
@@ -1497,17 +1501,14 @@
     nbr = grid.get_branch_number_wo_hvdc()
     ng = grid.get_generators_number()
     nb = grid.get_batteries_number()
     nl = grid.get_load_like_device_number()
     n_hvdc = grid.get_hvdc_number()
     n_fluid_node = grid.get_fluid_nodes_number()
     n_fluid_path = grid.get_fluid_paths_number()
-    n_fluid_turbine = grid.get_fluid_turbines_number()
-    n_fluid_pump = grid.get_fluid_pumps_number()
-    n_fluid_p2x = grid.get_fluid_p2xs_number()
     n_fluid_inj = grid.get_fluid_injection_number()
 
     # gather the fuels and emission rates matrices
     gen_emissions_rates_matrix = grid.get_emission_rates_sparse_matrix()
     gen_fuel_rates_matrix = grid.get_fuel_rates_sparse_matrix()
 
     if maximize_inter_area_flow:
@@ -1661,14 +1662,18 @@
 
                 for branches_list in [inter_area_branches, inter_area_hvdc]:
                     for k, branch, sense in branches_list:
                         # we want to maximize, hence the minus sign
                         f_obj += mip_vars.branch_vars.flows[local_t_idx, k] * (- sense)
 
             # add hydro side -------------------------------------------------------------------------------------------
+            if local_t_idx == 0 and fluid_level_0 is None:
+                # declare the initial level of the fluid nodes
+                fluid_level_0 = nc.fluid_node_data.initial_level
+
             if n_fluid_node > 0:
                 f_obj += add_hydro_formulation(t=local_t_idx,
                                                time_global_tidx=global_t_idx,
                                                time_array=grid.time_profile,
                                                Sbase=nc.Sbase,
                                                node_vars=mip_vars.fluid_node_vars,
                                                path_vars=mip_vars.fluid_path_vars,
@@ -1676,14 +1681,15 @@
                                                node_data=nc.fluid_node_data,
                                                path_data=nc.fluid_path_data,
                                                turbine_data=nc.fluid_turbine_data,
                                                pump_data=nc.fluid_pump_data,
                                                p2x_data=nc.fluid_p2x_data,
                                                generator_data=nc.generator_data,
                                                generator_vars=mip_vars.gen_vars,
+                                               fluid_level_0=fluid_level_0,
                                                prob=lp_model,
                                                logger=logger)
 
         elif zonal_grouping == ZonalGrouping.All:
             # this is the copper plate approach
             pass
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/opf_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,18 +497,18 @@
     # PV buses are identified by those who have the same upper and lower limits for the voltage. Slack obtained from nc
     pv = np.flatnonzero(Vm_max == Vm_min)
     pq = np.flatnonzero(Vm_max != Vm_min)
     slack = nc.vd
 
     # Check the active elements and their operational limits.
     br_mon_idx = nc.branch_data.get_monitor_enabled_indices()
-    gen_disp_idx = nc.generator_data.get_dispatchable_indices()
+    gen_disp_idx = nc.generator_data.get_dispatchable_active_indices()
     ind_gens = np.arange(len(Pg_max))
-    nig = np.where(~np.isin(ind_gens, gen_disp_idx))[0]
-    Sg_undis = (nc.generator_data.get_injections() / nc.Sbase)[nig]
+    gen_nondisp_idx = nc.generator_data.get_non_dispatchable_indices()
+    Sg_undis = (nc.generator_data.get_injections() / nc.Sbase)[gen_nondisp_idx]
     rates = nc.rates / Sbase  # Line loading limits. If the grid is not well conditioned, add constant value (i.e. +100)
     Va_max = nc.bus_data.angle_max  # This limits are not really used as of right now.
     Va_min = nc.bus_data.angle_min
 
     # Transformer control modes and line parameters to calculate the associated derivatives w.r.t the tap variables.
     k_m = nc.k_m
     k_tau = nc.k_tau
@@ -551,16 +551,16 @@
     f_disp_hvdc = nc.hvdc_data.F[hvdc_disp_idx]
     t_disp_hvdc = nc.hvdc_data.T[hvdc_disp_idx]
     P_hvdc_max = nc.hvdc_data.rate[hvdc_disp_idx]
 
     if opf_options.acopf_mode == AcOpfMode.ACOPFslacks:
         nsl = 2 * npq + 2 * n_br_mon
         # Slack relaxations for constraints
-        c_s = 1 * np.power(nc.branch_data.overload_cost[br_mon_idx] + 1e-9, 1.0)  # Cost squared since the slack is also squared
-        c_v = 1 * nc.bus_data.cost_v[pq] + 1e-9
+        c_s = 1 * np.power(nc.branch_data.overload_cost[br_mon_idx] + 0.1, 1.0)  # Cost squared since the slack is also squared
+        c_v = 1 * (nc.bus_data.cost_v[pq] + 0.1)
         sl_sf0 = np.ones(n_br_mon)
         sl_st0 = np.ones(n_br_mon)
         sl_vmax0 = np.ones(npq)
         sl_vmin0 = np.ones(npq)
 
     else:
         nsl = 0
@@ -625,68 +625,68 @@
         # run the solver with the function that checks the derivatives
         # against their finite differences equivalent
         result = interior_point_solver(x0=x0, n_x=NV, n_eq=NE, n_ineq=NI,
                                        func=evaluate_power_flow_debug,
                                        arg=(admittances, Cg, Sd, slack, from_idx, to_idx,
                                             pq, pv, Va_max, Va_min, Vm_max, Vm_min, Pg_max, Pg_min,
                                             Qg_max, Qg_min, tapm_max, tapm_min, tapt_max, tapt_min, alltapm, alltapt,
-                                            k_m, k_tau, k_mtau, c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, nig,
+                                            k_m, k_tau, k_mtau, c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, gen_nondisp_idx,
                                             Sg_undis, pf_options.control_Q, opf_options.acopf_mode),
                                        verbose=opf_options.verbose,
                                        max_iter=opf_options.ips_iterations,
                                        tol=opf_options.ips_tolerance,
                                        trust=opf_options.ips_trust_radius)
 
     else:
         if use_autodiff:
             # run the solver with the autodiff derivatives
             result = interior_point_solver(x0=x0, n_x=NV, n_eq=NE, n_ineq=NI,
                                            func=compute_autodiff_structures,
                                            arg=(admittances, Cg, Sd, slack, from_idx, to_idx, pq, pv,
                                                 Va_max, Va_min, Vm_max, Vm_min, Pg_max, Pg_min, Qg_max, Qg_min,
                                                 tapm_max, tapm_min, tapt_max, tapt_min, k_m, k_tau, k_mtau,
-                                                c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, nig, Sg_undis,
+                                                c0, c1, c2, Sbase, rates, br_mon_idx, gen_disp_idx, gen_nondisp_idx, Sg_undis,
                                                 opf_options.acopf_mode, 1e-5),
                                            verbose=opf_options.verbose,
                                            max_iter=opf_options.ips_iterations,
                                            tol=opf_options.ips_tolerance,
                                            trust=opf_options.ips_trust_radius)
         else:
             # run the solver with the analytic derivatives
             result = interior_point_solver(x0=x0, n_x=NV, n_eq=NE, n_ineq=NI,
                                            func=compute_analytic_structures,
                                            arg=(admittances, Cg, R, X, Sd, slack, from_idx, to_idx, f_nd_hvdc, t_nd_hvdc,
                                                 f_disp_hvdc, t_disp_hvdc, n_disp_hvdc, pq, pv, Pf_nondisp, P_hvdc_max, Vm_max, Vm_min, Pg_max,
                                                 Pg_min, tanmax, Qg_max, Qg_min, tapm_max, tapm_min, tapt_max, tapt_min,
                                                 alltapm, alltapt, k_m, k_tau, c0, c1, c2, c_s, c_v, Sbase, rates, br_mon_idx,
-                                                n_br_mon, gen_disp_idx, nig, Sg_undis, pf_options.control_Q, opf_options.acopf_mode),
+                                                n_br_mon, gen_disp_idx, gen_nondisp_idx, Sg_undis, pf_options.control_Q, opf_options.acopf_mode),
                                            verbose=opf_options.verbose,
                                            max_iter=opf_options.ips_iterations,
                                            tol=opf_options.ips_tolerance,
                                            trust=opf_options.ips_trust_radius)
 
     # convert the solution to the problem variables
     (Va, Vm, Pg_dis, Qg_dis, sl_sf, sl_st,
      sl_vmax, sl_vmin, tapm, tapt, Pfdc) = x2var(result.x, nVa=nbus, nVm=nbus, nPg=n_gen_disp, nQg=n_gen_disp,
                                                  M=n_br_mon, npq=npq, ntapm=ntapm, ntapt=ntapt, ndc=n_disp_hvdc,
                                                  acopf_mode=opf_options.acopf_mode)
 
     # Save Results DataFrame for tests
-    # pd.DataFrame(Va).transpose().to_csv('pegase89resth.csv')
-    # pd.DataFrame(Vm).transpose().to_csv('pegase89resV.csv')
-    # pd.DataFrame(Pg_dis).transpose().to_csv('pegase89resP.csv')
-    # pd.DataFrame(Qg_dis).transpose().to_csv('pegase89resQ.csv')
+    #pd.DataFrame(Va).transpose().to_csv('REEresth.csv')
+    #pd.DataFrame(Vm).transpose().to_csv('REEresV.csv')
+    #pd.DataFrame(Pg_dis).transpose().to_csv('REEresP.csv')
+    #pd.DataFrame(Qg_dis).transpose().to_csv('REEresQ.csv')
 
     Pg = np.zeros(len(ind_gens))
     Qg = np.zeros(len(ind_gens))
 
     Pg[gen_disp_idx] = Pg_dis
     Qg[gen_disp_idx] = Qg_dis
-    Pg[nig] = np.real(Sg_undis)
-    Qg[nig] = np.imag(Sg_undis)
+    Pg[gen_nondisp_idx] = np.real(Sg_undis)
+    Qg[gen_nondisp_idx] = np.imag(Sg_undis)
 
     # convert the lagrange multipliers to significant ones
     lam_p, lam_q = result.lam[:nbus], result.lam[nbus:2 * nbus]
 
     S = result.structs.S
     Sf = result.structs.Sf
     St = result.structs.St
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,25 +196,26 @@
             raise Exception('Result type not understood:' + str(result_type))
 
 
 class AvailableTransferCapacityTimeSeriesDriver(TimeSeriesDriverTemplate):
     tpe = SimulationTypes.NetTransferCapacityTS_run
     name = tpe.value
 
-    def __init__(
-            self, grid: MultiCircuit,
-            options: AvailableTransferCapacityOptions,
-            time_indices: np.ndarray,
-            clustering_results: Union[ClusteringResults, None] = None):
+    def __init__(self,
+                 grid: MultiCircuit,
+                 options: AvailableTransferCapacityOptions,
+                 time_indices: np.ndarray,
+                 clustering_results: Union[ClusteringResults, None] = None):
 
         """
         Power Transfer Distribution Factors class constructor
         :param grid: MultiCircuit Object
         :param options: OPF options
         :param time_indices: array of time indices to simulate
+        :param clustering_results: ClusteringResults (optional)
         """
 
         TimeSeriesDriverTemplate.__init__(
             self,
             grid=grid,
             time_indices=time_indices,
             clustering_results=clustering_results
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ATC/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/__init__.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,19 @@
         self.options: LinearAnalysisOptions = LinearAnalysisOptions() if options is None else options
 
         self.engine: EngineType = engine
 
         self.opf_results = opf_results
 
         # Results
-        self.results: Union[LinearAnalysisResults, None] = None
+        self.results: Union[LinearAnalysisResults, None] = LinearAnalysisResults(n_br=0,
+                                                                                 n_bus=0,
+                                                                                 br_names=(),
+                                                                                 bus_names=(),
+                                                                                 bus_types=())
 
         self.all_solved: bool = True
 
     def run(self):
         """
         Run thread
         """
```

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py` & `GridCalEngine-5.1.7/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/setup.py` & `GridCalEngine-5.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.6/PKG-INFO` & `GridCalEngine-5.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCalEngine
-Version: 5.1.6
+Version: 5.1.7
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

