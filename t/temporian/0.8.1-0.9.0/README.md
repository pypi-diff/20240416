# Comparing `tmp/temporian-0.8.1.tar.gz` & `tmp/temporian-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporian-0.8.1.tar", max compression
+gzip compressed data, was "temporian-0.9.0.tar", max compression
```

## Comparing `temporian-0.8.1.tar` & `temporian-0.9.0.tar`

### file list

```diff
@@ -1,376 +1,411 @@
--rw-r--r--   0        0        0    11358 2024-03-27 13:00:13.471235 temporian-0.8.1/LICENSE
--rw-r--r--   0        0        0     5846 2024-03-27 13:00:13.471339 temporian-0.8.1/README.md
--rw-r--r--   0        0        0     3793 2024-03-27 13:00:13.472414 temporian-0.8.1/config/build.py
--rw-r--r--   0        0        0     3110 2024-03-27 13:00:13.527197 temporian-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1507 2024-03-27 13:00:13.527412 temporian-0.8.1/temporian/BUILD
--rw-r--r--   0        0        0     3256 2024-03-27 13:00:13.527517 temporian-0.8.1/temporian/__init__.py
--rw-r--r--   0        0        0      317 2024-03-27 13:00:13.527629 temporian-0.8.1/temporian/api/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.527666 temporian-0.8.1/temporian/api/__init__.py
--rw-r--r--   0        0        0      134 2024-03-27 13:00:13.527761 temporian-0.8.1/temporian/api/duration.py
--rw-r--r--   0        0        0      995 2024-03-27 13:00:13.527855 temporian-0.8.1/temporian/beam/BUILD
--rw-r--r--   0        0        0     1418 2024-03-27 13:00:13.527930 temporian-0.8.1/temporian/beam/__init__.py
--rw-r--r--   0        0        0     5623 2024-03-27 13:00:13.528011 temporian-0.8.1/temporian/beam/evaluation.py
--rw-r--r--   0        0        0     1837 2024-03-27 13:00:13.528107 temporian-0.8.1/temporian/beam/implementation_lib.py
--rw-r--r--   0        0        0     1430 2024-03-27 13:00:13.528193 temporian-0.8.1/temporian/beam/io/BUILD
--rw-r--r--   0        0        0     5670 2024-03-27 13:00:13.528288 temporian-0.8.1/temporian/beam/io/csv.py
--rw-r--r--   0        0        0    16648 2024-03-27 13:00:13.528410 temporian-0.8.1/temporian/beam/io/dict.py
--rw-r--r--   0        0        0     2522 2024-03-27 13:00:13.528519 temporian-0.8.1/temporian/beam/io/np_array_coder.py
--rw-r--r--   0        0        0     9610 2024-03-27 13:00:13.528608 temporian-0.8.1/temporian/beam/io/tensorflow.py
--rw-r--r--   0        0        0     2184 2024-03-27 13:00:13.528744 temporian-0.8.1/temporian/beam/io/test/BUILD
--rw-r--r--   0        0        0     5045 2024-03-27 13:00:13.528833 temporian-0.8.1/temporian/beam/io/test/csv_test.py
--rw-r--r--   0        0        0     8929 2024-03-27 13:00:13.528944 temporian-0.8.1/temporian/beam/io/test/dict_test.py
--rw-r--r--   0        0        0     1959 2024-03-27 13:00:13.529022 temporian-0.8.1/temporian/beam/io/test/np_array_coder_test.py
--rw-r--r--   0        0        0     2316 2024-03-27 13:00:13.529115 temporian-0.8.1/temporian/beam/io/test/tensorflow_test.py
--rw-r--r--   0        0        0     2075 2024-03-27 13:00:13.529216 temporian-0.8.1/temporian/beam/operators/BUILD
--rw-r--r--   0        0        0     1258 2024-03-27 13:00:13.529314 temporian-0.8.1/temporian/beam/operators/__init__.py
--rw-r--r--   0        0        0     4494 2024-03-27 13:00:13.529389 temporian-0.8.1/temporian/beam/operators/add_index.py
--rw-r--r--   0        0        0     3002 2024-03-27 13:00:13.529472 temporian-0.8.1/temporian/beam/operators/base.py
--rw-r--r--   0        0        0     1169 2024-03-27 13:00:13.529554 temporian-0.8.1/temporian/beam/operators/prefix.py
--rw-r--r--   0        0        0     1177 2024-03-27 13:00:13.529640 temporian-0.8.1/temporian/beam/operators/rename.py
--rw-r--r--   0        0        0     1574 2024-03-27 13:00:13.529741 temporian-0.8.1/temporian/beam/operators/select.py
--rw-r--r--   0        0        0     1730 2024-03-27 13:00:13.529839 temporian-0.8.1/temporian/beam/operators/test/BUILD
--rw-r--r--   0        0        0     2252 2024-03-27 13:00:13.529926 temporian-0.8.1/temporian/beam/operators/test/add_index_test.py
--rw-r--r--   0        0        0     1300 2024-03-27 13:00:13.530105 temporian-0.8.1/temporian/beam/operators/test/prefix_test.py
--rw-r--r--   0        0        0     3703 2024-03-27 13:00:13.530222 temporian-0.8.1/temporian/beam/operators/test/rename_test.py
--rw-r--r--   0        0        0     2205 2024-03-27 13:00:13.530350 temporian-0.8.1/temporian/beam/operators/test/select_test.py
--rw-r--r--   0        0        0     2932 2024-03-27 13:00:13.530479 temporian-0.8.1/temporian/beam/operators/window/BUILD
--rw-r--r--   0        0        0     3246 2024-03-27 13:00:13.530581 temporian-0.8.1/temporian/beam/operators/window/base.py
--rw-r--r--   0        0        0     2759 2024-03-27 13:00:13.530664 temporian-0.8.1/temporian/beam/operators/window/moving_count.py
--rw-r--r--   0        0        0     1310 2024-03-27 13:00:13.530747 temporian-0.8.1/temporian/beam/operators/window/moving_max.py
--rw-r--r--   0        0        0     1310 2024-03-27 13:00:13.530840 temporian-0.8.1/temporian/beam/operators/window/moving_min.py
--rw-r--r--   0        0        0     1424 2024-03-27 13:00:13.530919 temporian-0.8.1/temporian/beam/operators/window/moving_standard_deviation.py
--rw-r--r--   0        0        0     1301 2024-03-27 13:00:13.531002 temporian-0.8.1/temporian/beam/operators/window/moving_sum.py
--rw-r--r--   0        0        0     1392 2024-03-27 13:00:13.531093 temporian-0.8.1/temporian/beam/operators/window/simple_moving_average.py
--rw-r--r--   0        0        0      507 2024-03-27 13:00:13.531202 temporian-0.8.1/temporian/beam/operators/window/test/BUILD
--rw-r--r--   0        0        0     3636 2024-03-27 13:00:13.531282 temporian-0.8.1/temporian/beam/operators/window/test/window_test.py
--rw-r--r--   0        0        0     1115 2024-03-27 13:00:13.531396 temporian-0.8.1/temporian/beam/test/BUILD
--rw-r--r--   0        0        0     1713 2024-03-27 13:00:13.531502 temporian-0.8.1/temporian/beam/test/evaluation_test.py
--rw-r--r--   0        0        0     3454 2024-03-27 13:00:13.531593 temporian-0.8.1/temporian/beam/test/utils.py
--rw-r--r--   0        0        0     2915 2024-03-27 13:00:13.531674 temporian-0.8.1/temporian/beam/typing.py
--rw-r--r--   0        0        0     2636 2024-03-27 13:00:13.531814 temporian-0.8.1/temporian/core/BUILD
--rw-r--r--   0        0        0      576 2024-03-27 13:00:13.531904 temporian-0.8.1/temporian/core/__init__.py
--rw-r--r--   0        0        0     6851 2024-03-27 13:00:13.532008 temporian-0.8.1/temporian/core/compilation.py
--rw-r--r--   0        0        0      949 2024-03-27 13:00:13.532129 temporian-0.8.1/temporian/core/data/BUILD
--rw-r--r--   0        0        0      576 2024-03-27 13:00:13.532193 temporian-0.8.1/temporian/core/data/__init__.py
--rw-r--r--   0        0        0     3702 2024-03-27 13:00:13.532277 temporian-0.8.1/temporian/core/data/dtype.py
--rw-r--r--   0        0        0     6484 2024-03-27 13:00:13.532372 temporian-0.8.1/temporian/core/data/duration.py
--rw-r--r--   0        0        0     7878 2024-03-27 13:00:13.532468 temporian-0.8.1/temporian/core/data/duration_utils.py
--rw-r--r--   0        0        0    11434 2024-03-27 13:00:13.532571 temporian-0.8.1/temporian/core/data/node.py
--rw-r--r--   0        0        0     4592 2024-03-27 13:00:13.532669 temporian-0.8.1/temporian/core/data/schema.py
--rw-r--r--   0        0        0      659 2024-03-27 13:00:13.532802 temporian-0.8.1/temporian/core/data/test/BUILD
--rw-r--r--   0        0        0      915 2024-03-27 13:00:13.532902 temporian-0.8.1/temporian/core/data/test/test_dtype.py
--rw-r--r--   0        0        0     1941 2024-03-27 13:00:13.532983 temporian-0.8.1/temporian/core/data/test/test_node.py
--rw-r--r--   0        0        0     1089 2024-03-27 13:00:13.533106 temporian-0.8.1/temporian/core/dataclasses.py
--rw-r--r--   0        0        0    14621 2024-03-27 13:00:13.533249 temporian-0.8.1/temporian/core/evaluation.py
--rw-r--r--   0        0        0   161948 2024-03-27 13:00:13.533704 temporian-0.8.1/temporian/core/event_set_ops.py
--rw-r--r--   0        0        0    12130 2024-03-27 13:00:13.533825 temporian-0.8.1/temporian/core/graph.py
--rw-r--r--   0        0        0     1632 2024-03-27 13:00:13.533899 temporian-0.8.1/temporian/core/operator_lib.py
--rw-r--r--   0        0        0    12402 2024-03-27 13:00:13.534072 temporian-0.8.1/temporian/core/operators/BUILD
--rw-r--r--   0        0        0      594 2024-03-27 13:00:13.534171 temporian-0.8.1/temporian/core/operators/__init__.py
--rw-r--r--   0        0        0     4872 2024-03-27 13:00:13.534275 temporian-0.8.1/temporian/core/operators/add_index.py
--rw-r--r--   0        0        0    13624 2024-03-27 13:00:13.534386 temporian-0.8.1/temporian/core/operators/base.py
--rw-r--r--   0        0        0     1924 2024-03-27 13:00:13.534496 temporian-0.8.1/temporian/core/operators/begin.py
--rw-r--r--   0        0        0     1648 2024-03-27 13:00:13.534623 temporian-0.8.1/temporian/core/operators/binary/BUILD
--rw-r--r--   0        0        0     1373 2024-03-27 13:00:13.534704 temporian-0.8.1/temporian/core/operators/binary/__init__.py
--rw-r--r--   0        0        0     4926 2024-03-27 13:00:13.534820 temporian-0.8.1/temporian/core/operators/binary/arithmetic.py
--rw-r--r--   0        0        0     4067 2024-03-27 13:00:13.534928 temporian-0.8.1/temporian/core/operators/binary/base.py
--rw-r--r--   0        0        0     3177 2024-03-27 13:00:13.535017 temporian-0.8.1/temporian/core/operators/binary/logical.py
--rw-r--r--   0        0        0     4140 2024-03-27 13:00:13.535114 temporian-0.8.1/temporian/core/operators/binary/relational.py
--rw-r--r--   0        0        0     3242 2024-03-27 13:00:13.535228 temporian-0.8.1/temporian/core/operators/calendar/BUILD
--rw-r--r--   0        0        0     1284 2024-03-27 13:00:13.535316 temporian-0.8.1/temporian/core/operators/calendar/__init__.py
--rw-r--r--   0        0        0     2791 2024-03-27 13:00:13.535415 temporian-0.8.1/temporian/core/operators/calendar/base.py
--rw-r--r--   0        0        0     1489 2024-03-27 13:00:13.535527 temporian-0.8.1/temporian/core/operators/calendar/day_of_month.py
--rw-r--r--   0        0        0     1483 2024-03-27 13:00:13.535610 temporian-0.8.1/temporian/core/operators/calendar/day_of_week.py
--rw-r--r--   0        0        0     1483 2024-03-27 13:00:13.535729 temporian-0.8.1/temporian/core/operators/calendar/day_of_year.py
--rw-r--r--   0        0        0     1440 2024-03-27 13:00:13.535814 temporian-0.8.1/temporian/core/operators/calendar/hour.py
--rw-r--r--   0        0        0     1465 2024-03-27 13:00:13.535883 temporian-0.8.1/temporian/core/operators/calendar/iso_week.py
--rw-r--r--   0        0        0     1454 2024-03-27 13:00:13.535971 temporian-0.8.1/temporian/core/operators/calendar/minute.py
--rw-r--r--   0        0        0     1447 2024-03-27 13:00:13.536042 temporian-0.8.1/temporian/core/operators/calendar/month.py
--rw-r--r--   0        0        0     1454 2024-03-27 13:00:13.536157 temporian-0.8.1/temporian/core/operators/calendar/second.py
--rw-r--r--   0        0        0     3612 2024-03-27 13:00:13.536272 temporian-0.8.1/temporian/core/operators/calendar/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.536315 temporian-0.8.1/temporian/core/operators/calendar/test/__init__.py
--rw-r--r--   0        0        0     1941 2024-03-27 13:00:13.536413 temporian-0.8.1/temporian/core/operators/calendar/test/test_base.py
--rw-r--r--   0        0        0     4502 2024-03-27 13:00:13.536510 temporian-0.8.1/temporian/core/operators/calendar/test/test_base_timezone.py
--rw-r--r--   0        0        0     2924 2024-03-27 13:00:13.536629 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_day_of_month.py
--rw-r--r--   0        0        0     1625 2024-03-27 13:00:13.536715 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_day_of_week.py
--rw-r--r--   0        0        0     2141 2024-03-27 13:00:13.536836 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_day_of_year.py
--rw-r--r--   0        0        0     3151 2024-03-27 13:00:13.536964 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_hour.py
--rw-r--r--   0        0        0     1790 2024-03-27 13:00:13.537047 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_iso_week.py
--rw-r--r--   0        0        0     1474 2024-03-27 13:00:13.537128 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_minute.py
--rw-r--r--   0        0        0     2104 2024-03-27 13:00:13.537210 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_month.py
--rw-r--r--   0        0        0     1436 2024-03-27 13:00:13.537312 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_second.py
--rw-r--r--   0        0        0     3346 2024-03-27 13:00:13.537381 temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_year.py
--rw-r--r--   0        0        0     1440 2024-03-27 13:00:13.537465 temporian-0.8.1/temporian/core/operators/calendar/year.py
--rw-r--r--   0        0        0     5886 2024-03-27 13:00:13.537563 temporian-0.8.1/temporian/core/operators/cast.py
--rw-r--r--   0        0        0     7785 2024-03-27 13:00:13.537628 temporian-0.8.1/temporian/core/operators/combine.py
--rw-r--r--   0        0        0     4699 2024-03-27 13:00:13.537676 temporian-0.8.1/temporian/core/operators/drop_index.py
--rw-r--r--   0        0        0     1913 2024-03-27 13:00:13.537772 temporian-0.8.1/temporian/core/operators/end.py
--rw-r--r--   0        0        0     1925 2024-03-27 13:00:13.537879 temporian-0.8.1/temporian/core/operators/enumerate.py
--rw-r--r--   0        0        0     5794 2024-03-27 13:00:13.537950 temporian-0.8.1/temporian/core/operators/fast_fourier_transform.py
--rw-r--r--   0        0        0     1363 2024-03-27 13:00:13.538038 temporian-0.8.1/temporian/core/operators/fillna.py
--rw-r--r--   0        0        0     4286 2024-03-27 13:00:13.538113 temporian-0.8.1/temporian/core/operators/filter.py
--rw-r--r--   0        0        0     2049 2024-03-27 13:00:13.538237 temporian-0.8.1/temporian/core/operators/filter_empty_index.py
--rw-r--r--   0        0        0     2676 2024-03-27 13:00:13.538310 temporian-0.8.1/temporian/core/operators/filter_moving_count.py
--rw-r--r--   0        0        0     6676 2024-03-27 13:00:13.538384 temporian-0.8.1/temporian/core/operators/glue.py
--rw-r--r--   0        0        0     4992 2024-03-27 13:00:13.538477 temporian-0.8.1/temporian/core/operators/join.py
--rw-r--r--   0        0        0     2613 2024-03-27 13:00:13.538559 temporian-0.8.1/temporian/core/operators/lag.py
--rw-r--r--   0        0        0     2709 2024-03-27 13:00:13.538647 temporian-0.8.1/temporian/core/operators/leak.py
--rw-r--r--   0        0        0     5031 2024-03-27 13:00:13.538713 temporian-0.8.1/temporian/core/operators/map.py
--rw-r--r--   0        0        0     2492 2024-03-27 13:00:13.538796 temporian-0.8.1/temporian/core/operators/prefix.py
--rw-r--r--   0        0        0     3965 2024-03-27 13:00:13.538888 temporian-0.8.1/temporian/core/operators/propagate.py
--rw-r--r--   0        0        0     7064 2024-03-27 13:00:13.538951 temporian-0.8.1/temporian/core/operators/rename.py
--rw-r--r--   0        0        0     2298 2024-03-27 13:00:13.539035 temporian-0.8.1/temporian/core/operators/resample.py
--rw-r--r--   0        0        0     1310 2024-03-27 13:00:13.539135 temporian-0.8.1/temporian/core/operators/scalar/BUILD
--rw-r--r--   0        0        0     1378 2024-03-27 13:00:13.539202 temporian-0.8.1/temporian/core/operators/scalar/__init__.py
--rw-r--r--   0        0        0     8001 2024-03-27 13:00:13.539282 temporian-0.8.1/temporian/core/operators/scalar/arithmetic_scalar.py
--rw-r--r--   0        0        0     5219 2024-03-27 13:00:13.539376 temporian-0.8.1/temporian/core/operators/scalar/base.py
--rw-r--r--   0        0        0     4119 2024-03-27 13:00:13.539474 temporian-0.8.1/temporian/core/operators/scalar/relational_scalar.py
--rw-r--r--   0        0        0     4334 2024-03-27 13:00:13.539581 temporian-0.8.1/temporian/core/operators/select.py
--rw-r--r--   0        0        0     4305 2024-03-27 13:00:13.539686 temporian-0.8.1/temporian/core/operators/select_index_values.py
--rw-r--r--   0        0        0     3412 2024-03-27 13:00:13.539774 temporian-0.8.1/temporian/core/operators/since_last.py
--rw-r--r--   0        0        0    12676 2024-03-27 13:00:13.539888 temporian-0.8.1/temporian/core/operators/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.539935 temporian-0.8.1/temporian/core/operators/test/__init__.py
--rw-r--r--   0        0        0     7083 2024-03-27 13:00:13.540034 temporian-0.8.1/temporian/core/operators/test/test_add_index.py
--rw-r--r--   0        0        0     3375 2024-03-27 13:00:13.540124 temporian-0.8.1/temporian/core/operators/test/test_after.py
--rw-r--r--   0        0        0     5805 2024-03-27 13:00:13.540207 temporian-0.8.1/temporian/core/operators/test/test_arithmetic.py
--rw-r--r--   0        0        0     8127 2024-03-27 13:00:13.540313 temporian-0.8.1/temporian/core/operators/test/test_arithmetic_scalar.py
--rw-r--r--   0        0        0     4239 2024-03-27 13:00:13.540716 temporian-0.8.1/temporian/core/operators/test/test_assign.py
--rw-r--r--   0        0        0     3410 2024-03-27 13:00:13.541020 temporian-0.8.1/temporian/core/operators/test/test_before.py
--rw-r--r--   0        0        0     1512 2024-03-27 13:00:13.541270 temporian-0.8.1/temporian/core/operators/test/test_begin.py
--rw-r--r--   0        0        0     4874 2024-03-27 13:00:13.541454 temporian-0.8.1/temporian/core/operators/test/test_cast.py
--rw-r--r--   0        0        0     8436 2024-03-27 13:00:13.541669 temporian-0.8.1/temporian/core/operators/test/test_combine.py
--rw-r--r--   0        0        0     2023 2024-03-27 13:00:13.541875 temporian-0.8.1/temporian/core/operators/test/test_drop.py
--rw-r--r--   0        0        0     4383 2024-03-27 13:00:13.542108 temporian-0.8.1/temporian/core/operators/test/test_drop_index.py
--rw-r--r--   0        0        0     1506 2024-03-27 13:00:13.542355 temporian-0.8.1/temporian/core/operators/test/test_end.py
--rw-r--r--   0        0        0     1794 2024-03-27 13:00:13.542571 temporian-0.8.1/temporian/core/operators/test/test_enumerate.py
--rw-r--r--   0        0        0     4338 2024-03-27 13:00:13.542803 temporian-0.8.1/temporian/core/operators/test/test_fast_fourier_transform.py
--rw-r--r--   0        0        0     1767 2024-03-27 13:00:13.543061 temporian-0.8.1/temporian/core/operators/test/test_fillna.py
--rw-r--r--   0        0        0     2321 2024-03-27 13:00:13.543298 temporian-0.8.1/temporian/core/operators/test/test_filter.py
--rw-r--r--   0        0        0     1443 2024-03-27 13:00:13.543548 temporian-0.8.1/temporian/core/operators/test/test_filter_empty_index.py
--rw-r--r--   0        0        0     2204 2024-03-27 13:00:13.543774 temporian-0.8.1/temporian/core/operators/test/test_filter_moving_count.py
--rw-r--r--   0        0        0     6214 2024-03-27 13:00:13.543954 temporian-0.8.1/temporian/core/operators/test/test_glue.py
--rw-r--r--   0        0        0     4476 2024-03-27 13:00:13.544132 temporian-0.8.1/temporian/core/operators/test/test_join.py
--rw-r--r--   0        0        0     1328 2024-03-27 13:00:13.544365 temporian-0.8.1/temporian/core/operators/test/test_lag.py
--rw-r--r--   0        0        0     1330 2024-03-27 13:00:13.544591 temporian-0.8.1/temporian/core/operators/test/test_leak.py
--rw-r--r--   0        0        0     2204 2024-03-27 13:00:13.544824 temporian-0.8.1/temporian/core/operators/test/test_logical.py
--rw-r--r--   0        0        0     4990 2024-03-27 13:00:13.545047 temporian-0.8.1/temporian/core/operators/test/test_map.py
--rw-r--r--   0        0        0     1503 2024-03-27 13:00:13.545288 temporian-0.8.1/temporian/core/operators/test/test_prefix.py
--rw-r--r--   0        0        0     3763 2024-03-27 13:00:13.545504 temporian-0.8.1/temporian/core/operators/test/test_propagate.py
--rw-r--r--   0        0        0     6025 2024-03-27 13:00:13.545741 temporian-0.8.1/temporian/core/operators/test/test_relational.py
--rw-r--r--   0        0        0     5801 2024-03-27 13:00:13.545936 temporian-0.8.1/temporian/core/operators/test/test_relational_scalar.py
--rw-r--r--   0        0        0     8367 2024-03-27 13:00:13.546060 temporian-0.8.1/temporian/core/operators/test/test_rename.py
--rw-r--r--   0        0        0     1899 2024-03-27 13:00:13.546209 temporian-0.8.1/temporian/core/operators/test/test_resample.py
--rw-r--r--   0        0        0     2080 2024-03-27 13:00:13.546324 temporian-0.8.1/temporian/core/operators/test/test_select.py
--rw-r--r--   0        0        0     6339 2024-03-27 13:00:13.546392 temporian-0.8.1/temporian/core/operators/test/test_select_index_values.py
--rw-r--r--   0        0        0     3203 2024-03-27 13:00:13.546510 temporian-0.8.1/temporian/core/operators/test/test_since_last.py
--rw-r--r--   0        0        0     2369 2024-03-27 13:00:13.546610 temporian-0.8.1/temporian/core/operators/test/test_tick.py
--rw-r--r--   0        0        0     7352 2024-03-27 13:00:13.546743 temporian-0.8.1/temporian/core/operators/test/test_tick_calendar.py
--rw-r--r--   0        0        0     2305 2024-03-27 13:00:13.546810 temporian-0.8.1/temporian/core/operators/test/test_timestamps.py
--rw-r--r--   0        0        0     6093 2024-03-27 13:00:13.546904 temporian-0.8.1/temporian/core/operators/test/test_unary.py
--rw-r--r--   0        0        0     1408 2024-03-27 13:00:13.546984 temporian-0.8.1/temporian/core/operators/test/test_unique_timestamps.py
--rw-r--r--   0        0        0     2302 2024-03-27 13:00:13.547098 temporian-0.8.1/temporian/core/operators/test/test_until_next.py
--rw-r--r--   0        0        0     8807 2024-03-27 13:00:13.547204 temporian-0.8.1/temporian/core/operators/test/test_where.py
--rw-r--r--   0        0        0     2870 2024-03-27 13:00:13.547273 temporian-0.8.1/temporian/core/operators/tick.py
--rw-r--r--   0        0        0     8427 2024-03-27 13:00:13.547382 temporian-0.8.1/temporian/core/operators/tick_calendar.py
--rw-r--r--   0        0        0     1934 2024-03-27 13:00:13.547497 temporian-0.8.1/temporian/core/operators/timestamps.py
--rw-r--r--   0        0        0     9755 2024-03-27 13:00:13.547580 temporian-0.8.1/temporian/core/operators/unary.py
--rw-r--r--   0        0        0     2028 2024-03-27 13:00:13.547650 temporian-0.8.1/temporian/core/operators/unique_timestamps.py
--rw-r--r--   0        0        0     3096 2024-03-27 13:00:13.547870 temporian-0.8.1/temporian/core/operators/until_next.py
--rw-r--r--   0        0        0     6746 2024-03-27 13:00:13.548018 temporian-0.8.1/temporian/core/operators/where.py
--rw-r--r--   0        0        0     3501 2024-03-27 13:00:13.548165 temporian-0.8.1/temporian/core/operators/window/BUILD
--rw-r--r--   0        0        0     1333 2024-03-27 13:00:13.548258 temporian-0.8.1/temporian/core/operators/window/__init__.py
--rw-r--r--   0        0        0     5127 2024-03-27 13:00:13.548364 temporian-0.8.1/temporian/core/operators/window/base.py
--rw-r--r--   0        0        0     1861 2024-03-27 13:00:13.548432 temporian-0.8.1/temporian/core/operators/window/moving_count.py
--rw-r--r--   0        0        0     2021 2024-03-27 13:00:13.548560 temporian-0.8.1/temporian/core/operators/window/moving_max.py
--rw-r--r--   0        0        0     2021 2024-03-27 13:00:13.548637 temporian-0.8.1/temporian/core/operators/window/moving_min.py
--rw-r--r--   0        0        0     2706 2024-03-27 13:00:13.548721 temporian-0.8.1/temporian/core/operators/window/moving_product.py
--rw-r--r--   0        0        0     2270 2024-03-27 13:00:13.548807 temporian-0.8.1/temporian/core/operators/window/moving_standard_deviation.py
--rw-r--r--   0        0        0     2396 2024-03-27 13:00:13.548887 temporian-0.8.1/temporian/core/operators/window/moving_sum.py
--rw-r--r--   0        0        0     2378 2024-03-27 13:00:13.548976 temporian-0.8.1/temporian/core/operators/window/simple_moving_average.py
--rw-r--r--   0        0        0     3581 2024-03-27 13:00:13.549115 temporian-0.8.1/temporian/core/operators/window/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.549173 temporian-0.8.1/temporian/core/operators/window/test/__init__.py
--rw-r--r--   0        0        0     5465 2024-03-27 13:00:13.549282 temporian-0.8.1/temporian/core/operators/window/test/test_base.py
--rw-r--r--   0        0        0     2177 2024-03-27 13:00:13.549366 temporian-0.8.1/temporian/core/operators/window/test/test_cumprod.py
--rw-r--r--   0        0        0     1967 2024-03-27 13:00:13.549454 temporian-0.8.1/temporian/core/operators/window/test/test_cumsum.py
--rw-r--r--   0        0        0     3006 2024-03-27 13:00:13.549548 temporian-0.8.1/temporian/core/operators/window/test/test_moving_count.py
--rw-r--r--   0        0        0     3619 2024-03-27 13:00:13.549622 temporian-0.8.1/temporian/core/operators/window/test/test_moving_max.py
--rw-r--r--   0        0        0     3614 2024-03-27 13:00:13.549725 temporian-0.8.1/temporian/core/operators/window/test/test_moving_min.py
--rw-r--r--   0        0        0     7455 2024-03-27 13:00:13.549893 temporian-0.8.1/temporian/core/operators/window/test/test_moving_product.py
--rw-r--r--   0        0        0     6752 2024-03-27 13:00:13.549969 temporian-0.8.1/temporian/core/operators/window/test/test_moving_standard_deviation.py
--rw-r--r--   0        0        0     6064 2024-03-27 13:00:13.550089 temporian-0.8.1/temporian/core/operators/window/test/test_moving_sum.py
--rw-r--r--   0        0        0     9814 2024-03-27 13:00:13.550230 temporian-0.8.1/temporian/core/operators/window/test/test_simple_moving_average.py
--rw-r--r--   0        0        0     1099 2024-03-27 13:00:13.550397 temporian-0.8.1/temporian/core/schedule.py
--rw-r--r--   0        0        0    24326 2024-03-27 13:00:13.550542 temporian-0.8.1/temporian/core/serialization.py
--rw-r--r--   0        0        0     3160 2024-03-27 13:00:13.550707 temporian-0.8.1/temporian/core/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.550752 temporian-0.8.1/temporian/core/test/__init__.py
--rw-r--r--   0        0        0     6248 2024-03-27 13:00:13.550894 temporian-0.8.1/temporian/core/test/compilation_test.py
--rw-r--r--   0        0        0     7630 2024-03-27 13:00:13.551003 temporian-0.8.1/temporian/core/test/evaluation_test.py
--rw-r--r--   0        0        0     8133 2024-03-27 13:00:13.551086 temporian-0.8.1/temporian/core/test/graph_test.py
--rw-r--r--   0        0        0    23290 2024-03-27 13:00:13.551205 temporian-0.8.1/temporian/core/test/magic_methods_test.py
--rw-r--r--   0        0        0     5213 2024-03-27 13:00:13.551321 temporian-0.8.1/temporian/core/test/operator_test.py
--rw-r--r--   0        0        0     3573 2024-03-27 13:00:13.551419 temporian-0.8.1/temporian/core/test/registered_operators_test.py
--rw-r--r--   0        0        0    20736 2024-03-27 13:00:13.551538 temporian-0.8.1/temporian/core/test/serialization_test.py
--rw-r--r--   0        0        0     9072 2024-03-27 13:00:13.551636 temporian-0.8.1/temporian/core/test/utils.py
--rw-r--r--   0        0        0     1428 2024-03-27 13:00:13.551759 temporian-0.8.1/temporian/core/types.py
--rw-r--r--   0        0        0     5230 2024-03-27 13:00:13.551853 temporian-0.8.1/temporian/core/typing.py
--rw-r--r--   0        0        0      211 2024-03-27 13:00:13.551974 temporian-0.8.1/temporian/implementation/BUILD
--rw-r--r--   0        0        0      576 2024-03-27 13:00:13.552043 temporian-0.8.1/temporian/implementation/__init__.py
--rw-r--r--   0        0        0      649 2024-03-27 13:00:13.552168 temporian-0.8.1/temporian/implementation/numpy/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.552199 temporian-0.8.1/temporian/implementation/numpy/__init__.py
--rw-r--r--   0        0        0     2404 2024-03-27 13:00:13.552278 temporian-0.8.1/temporian/implementation/numpy/data/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.552316 temporian-0.8.1/temporian/implementation/numpy/data/__init__.py
--rw-r--r--   0        0        0    15177 2024-03-27 13:00:13.552437 temporian-0.8.1/temporian/implementation/numpy/data/display_utils.py
--rw-r--r--   0        0        0    11353 2024-03-27 13:00:13.552537 temporian-0.8.1/temporian/implementation/numpy/data/dtype_normalization.py
--rw-r--r--   0        0        0    11481 2024-03-27 13:00:13.552605 temporian-0.8.1/temporian/implementation/numpy/data/event_set.py
--rw-r--r--   0        0        0     7317 2024-03-27 13:00:13.552684 temporian-0.8.1/temporian/implementation/numpy/data/io.py
--rw-r--r--   0        0        0    17076 2024-03-27 13:00:13.552840 temporian-0.8.1/temporian/implementation/numpy/data/plotter.py
--rw-r--r--   0        0        0     2258 2024-03-27 13:00:13.552935 temporian-0.8.1/temporian/implementation/numpy/data/plotter_base.py
--rw-r--r--   0        0        0     6316 2024-03-27 13:00:13.553059 temporian-0.8.1/temporian/implementation/numpy/data/plotter_bokeh.py
--rw-r--r--   0        0        0     4784 2024-03-27 13:00:13.553149 temporian-0.8.1/temporian/implementation/numpy/data/plotter_matplotlib.py
--rw-r--r--   0        0        0     1359 2024-03-27 13:00:13.553325 temporian-0.8.1/temporian/implementation/numpy/data/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.553371 temporian-0.8.1/temporian/implementation/numpy/data/test/__init__.py
--rw-r--r--   0        0        0     5005 2024-03-27 13:00:13.553469 temporian-0.8.1/temporian/implementation/numpy/data/test/event_set_test.py
--rw-r--r--   0        0        0     7121 2024-03-27 13:00:13.553553 temporian-0.8.1/temporian/implementation/numpy/data/test/io_test.py
--rw-r--r--   0        0        0     7143 2024-03-27 13:00:13.553661 temporian-0.8.1/temporian/implementation/numpy/data/test/plotter_test.py
--rw-r--r--   0        0        0      151 2024-03-27 13:00:13.553781 temporian-0.8.1/temporian/implementation/numpy/data/test/test_data/BUILD
--rw-r--r--   0        0        0     2804 2024-03-27 13:00:13.553887 temporian-0.8.1/temporian/implementation/numpy/data/test/test_data/test_html_repr_limits_golden.html
--rw-r--r--   0        0        0     3969 2024-03-27 13:00:13.553963 temporian-0.8.1/temporian/implementation/numpy/data/test/test_data/test_html_repr_no_limits_golden.html
--rw-r--r--   0        0        0     4883 2024-03-27 13:00:13.554100 temporian-0.8.1/temporian/implementation/numpy/evaluation.py
--rw-r--r--   0        0        0     1655 2024-03-27 13:00:13.554197 temporian-0.8.1/temporian/implementation/numpy/implementation_lib.py
--rw-r--r--   0        0        0    13367 2024-03-27 13:00:13.554330 temporian-0.8.1/temporian/implementation/numpy/operators/BUILD
--rw-r--r--   0        0        0     4131 2024-03-27 13:00:13.554404 temporian-0.8.1/temporian/implementation/numpy/operators/__init__.py
--rw-r--r--   0        0        0     2488 2024-03-27 13:00:13.554504 temporian-0.8.1/temporian/implementation/numpy/operators/add_index.py
--rw-r--r--   0        0        0     8088 2024-03-27 13:00:13.554609 temporian-0.8.1/temporian/implementation/numpy/operators/base.py
--rw-r--r--   0        0        0     2175 2024-03-27 13:00:13.554706 temporian-0.8.1/temporian/implementation/numpy/operators/begin.py
--rw-r--r--   0        0        0     1554 2024-03-27 13:00:13.554832 temporian-0.8.1/temporian/implementation/numpy/operators/binary/BUILD
--rw-r--r--   0        0        0      772 2024-03-27 13:00:13.554934 temporian-0.8.1/temporian/implementation/numpy/operators/binary/__init__.py
--rw-r--r--   0        0        0     5385 2024-03-27 13:00:13.555029 temporian-0.8.1/temporian/implementation/numpy/operators/binary/arithmetic.py
--rw-r--r--   0        0        0     3478 2024-03-27 13:00:13.555103 temporian-0.8.1/temporian/implementation/numpy/operators/binary/base.py
--rw-r--r--   0        0        0     2619 2024-03-27 13:00:13.555187 temporian-0.8.1/temporian/implementation/numpy/operators/binary/logical.py
--rw-r--r--   0        0        0     4280 2024-03-27 13:00:13.555279 temporian-0.8.1/temporian/implementation/numpy/operators/binary/relational.py
--rw-r--r--   0        0        0     2578 2024-03-27 13:00:13.555415 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.555456 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/__init__.py
--rw-r--r--   0        0        0     1671 2024-03-27 13:00:13.555537 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/base.py
--rw-r--r--   0        0        0     1240 2024-03-27 13:00:13.555641 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/day_of_month.py
--rw-r--r--   0        0        0     1233 2024-03-27 13:00:13.555722 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/day_of_week.py
--rw-r--r--   0        0        0     1234 2024-03-27 13:00:13.555797 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/day_of_year.py
--rw-r--r--   0        0        0     1191 2024-03-27 13:00:13.555856 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/hour.py
--rw-r--r--   0        0        0     1210 2024-03-27 13:00:13.555954 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/iso_week.py
--rw-r--r--   0        0        0     1203 2024-03-27 13:00:13.556052 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/minute.py
--rw-r--r--   0        0        0     1197 2024-03-27 13:00:13.556131 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/month.py
--rw-r--r--   0        0        0     1203 2024-03-27 13:00:13.556226 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/second.py
--rw-r--r--   0        0        0     1191 2024-03-27 13:00:13.556312 temporian-0.8.1/temporian/implementation/numpy/operators/calendar/year.py
--rw-r--r--   0        0        0     4238 2024-03-27 13:00:13.556391 temporian-0.8.1/temporian/implementation/numpy/operators/cast.py
--rw-r--r--   0        0        0     4140 2024-03-27 13:00:13.556479 temporian-0.8.1/temporian/implementation/numpy/operators/combine.py
--rw-r--r--   0        0        0     3955 2024-03-27 13:00:13.556562 temporian-0.8.1/temporian/implementation/numpy/operators/drop_index.py
--rw-r--r--   0        0        0     2158 2024-03-27 13:00:13.556681 temporian-0.8.1/temporian/implementation/numpy/operators/end.py
--rw-r--r--   0        0        0     1978 2024-03-27 13:00:13.556759 temporian-0.8.1/temporian/implementation/numpy/operators/enumerate.py
--rw-r--r--   0        0        0     3412 2024-03-27 13:00:13.556875 temporian-0.8.1/temporian/implementation/numpy/operators/fast_fourier_transform.py
--rw-r--r--   0        0        0     1639 2024-03-27 13:00:13.556967 temporian-0.8.1/temporian/implementation/numpy/operators/filter.py
--rw-r--r--   0        0        0     2053 2024-03-27 13:00:13.557084 temporian-0.8.1/temporian/implementation/numpy/operators/filter_empty_index.py
--rw-r--r--   0        0        0     2296 2024-03-27 13:00:13.557167 temporian-0.8.1/temporian/implementation/numpy/operators/filter_moving_count.py
--rw-r--r--   0        0        0     2124 2024-03-27 13:00:13.557286 temporian-0.8.1/temporian/implementation/numpy/operators/glue.py
--rw-r--r--   0        0        0     4509 2024-03-27 13:00:13.557723 temporian-0.8.1/temporian/implementation/numpy/operators/join.py
--rw-r--r--   0        0        0     1951 2024-03-27 13:00:13.557844 temporian-0.8.1/temporian/implementation/numpy/operators/lag.py
--rw-r--r--   0        0        0     2070 2024-03-27 13:00:13.557930 temporian-0.8.1/temporian/implementation/numpy/operators/leak.py
--rw-r--r--   0        0        0     3846 2024-03-27 13:00:13.558055 temporian-0.8.1/temporian/implementation/numpy/operators/map.py
--rw-r--r--   0        0        0     1551 2024-03-27 13:00:13.558131 temporian-0.8.1/temporian/implementation/numpy/operators/prefix.py
--rw-r--r--   0        0        0     2745 2024-03-27 13:00:13.558222 temporian-0.8.1/temporian/implementation/numpy/operators/propagate.py
--rw-r--r--   0        0        0     1756 2024-03-27 13:00:13.558298 temporian-0.8.1/temporian/implementation/numpy/operators/rename.py
--rw-r--r--   0        0        0     4157 2024-03-27 13:00:13.558386 temporian-0.8.1/temporian/implementation/numpy/operators/resample.py
--rw-r--r--   0        0        0     1272 2024-03-27 13:00:13.558537 temporian-0.8.1/temporian/implementation/numpy/operators/scalar/BUILD
--rw-r--r--   0        0        0      692 2024-03-27 13:00:13.558644 temporian-0.8.1/temporian/implementation/numpy/operators/scalar/__init__.py
--rw-r--r--   0        0        0     4499 2024-03-27 13:00:13.558731 temporian-0.8.1/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py
--rw-r--r--   0        0        0     2591 2024-03-27 13:00:13.558814 temporian-0.8.1/temporian/implementation/numpy/operators/scalar/base.py
--rw-r--r--   0        0        0     3613 2024-03-27 13:00:13.558889 temporian-0.8.1/temporian/implementation/numpy/operators/scalar/relational_scalar.py
--rw-r--r--   0        0        0     2355 2024-03-27 13:00:13.558972 temporian-0.8.1/temporian/implementation/numpy/operators/select.py
--rw-r--r--   0        0        0     2811 2024-03-27 13:00:13.559055 temporian-0.8.1/temporian/implementation/numpy/operators/select_index_values.py
--rw-r--r--   0        0        0     2981 2024-03-27 13:00:13.559151 temporian-0.8.1/temporian/implementation/numpy/operators/since_last.py
--rw-r--r--   0        0        0     2677 2024-03-27 13:00:13.559232 temporian-0.8.1/temporian/implementation/numpy/operators/tick.py
--rw-r--r--   0        0        0     4486 2024-03-27 13:00:13.559308 temporian-0.8.1/temporian/implementation/numpy/operators/tick_calendar.py
--rw-r--r--   0        0        0     1955 2024-03-27 13:00:13.559386 temporian-0.8.1/temporian/implementation/numpy/operators/timestamps.py
--rw-r--r--   0        0        0     4554 2024-03-27 13:00:13.559469 temporian-0.8.1/temporian/implementation/numpy/operators/unary.py
--rw-r--r--   0        0        0     1937 2024-03-27 13:00:13.559554 temporian-0.8.1/temporian/implementation/numpy/operators/unique_timestamps.py
--rw-r--r--   0        0        0     2486 2024-03-27 13:00:13.559626 temporian-0.8.1/temporian/implementation/numpy/operators/until_next.py
--rw-r--r--   0        0        0     2820 2024-03-27 13:00:13.559728 temporian-0.8.1/temporian/implementation/numpy/operators/where.py
--rw-r--r--   0        0        0     3050 2024-03-27 13:00:13.559846 temporian-0.8.1/temporian/implementation/numpy/operators/window/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.559891 temporian-0.8.1/temporian/implementation/numpy/operators/window/__init__.py
--rw-r--r--   0        0        0     7731 2024-03-27 13:00:13.559987 temporian-0.8.1/temporian/implementation/numpy/operators/window/base.py
--rw-r--r--   0        0        0     3694 2024-03-27 13:00:13.560082 temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_count.py
--rw-r--r--   0        0        0     1203 2024-03-27 13:00:13.560182 temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_max.py
--rw-r--r--   0        0        0     1203 2024-03-27 13:00:13.560281 temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_min.py
--rw-r--r--   0        0        0     1231 2024-03-27 13:00:13.560366 temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_product.py
--rw-r--r--   0        0        0     1304 2024-03-27 13:00:13.560449 temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_standard_deviation.py
--rw-r--r--   0        0        0     1203 2024-03-27 13:00:13.560517 temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_sum.py
--rw-r--r--   0        0        0     1276 2024-03-27 13:00:13.560597 temporian-0.8.1/temporian/implementation/numpy/operators/window/simple_moving_average.py
--rw-r--r--   0        0        0      481 2024-03-27 13:00:13.560722 temporian-0.8.1/temporian/implementation/numpy/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.560773 temporian-0.8.1/temporian/implementation/numpy/test/__init__.py
--rw-r--r--   0        0        0     3650 2024-03-27 13:00:13.560839 temporian-0.8.1/temporian/implementation/numpy/test/registered_operators_test.py
--rw-r--r--   0        0        0       92 2024-03-27 13:00:13.560959 temporian-0.8.1/temporian/implementation/numpy_cc/BUILD
--rw-r--r--   0        0        0      576 2024-03-27 13:00:13.561052 temporian-0.8.1/temporian/implementation/numpy_cc/__init__.py
--rw-r--r--   0        0        0     2368 2024-03-27 13:00:13.561161 temporian-0.8.1/temporian/implementation/numpy_cc/operators/BUILD
--rw-r--r--   0        0        0      576 2024-03-27 13:00:13.561246 temporian-0.8.1/temporian/implementation/numpy_cc/operators/__init__.py
--rw-r--r--   0        0        0     8633 2024-03-27 13:00:13.561343 temporian-0.8.1/temporian/implementation/numpy_cc/operators/add_index.cc
--rw-r--r--   0        0        0      102 2024-03-27 13:00:13.561428 temporian-0.8.1/temporian/implementation/numpy_cc/operators/add_index.h
--rw-r--r--   0        0        0     8100 2024-03-27 13:00:13.561541 temporian-0.8.1/temporian/implementation/numpy_cc/operators/calendar.cc
--rw-r--r--   0        0        0      104 2024-03-27 13:00:13.561634 temporian-0.8.1/temporian/implementation/numpy_cc/operators/calendar.h
--rw-r--r--   0        0        0      674 2024-03-27 13:00:13.561712 temporian-0.8.1/temporian/implementation/numpy_cc/operators/common.h
--rw-r--r--   0        0        0     1195 2024-03-27 13:00:13.561800 temporian-0.8.1/temporian/implementation/numpy_cc/operators/filter_moving_count.cc
--rw-r--r--   0        0        0      112 2024-03-27 13:00:13.561892 temporian-0.8.1/temporian/implementation/numpy_cc/operators/filter_moving_count.h
--rw-r--r--   0        0        0     2996 2024-03-27 13:00:13.561976 temporian-0.8.1/temporian/implementation/numpy_cc/operators/join.cc
--rw-r--r--   0        0        0       97 2024-03-27 13:00:13.562042 temporian-0.8.1/temporian/implementation/numpy_cc/operators/join.h
--rw-r--r--   0        0        0      988 2024-03-27 13:00:13.562117 temporian-0.8.1/temporian/implementation/numpy_cc/operators/pyinit.cc
--rw-r--r--   0        0        0     1615 2024-03-27 13:00:13.562195 temporian-0.8.1/temporian/implementation/numpy_cc/operators/resample.cc
--rw-r--r--   0        0        0      105 2024-03-27 13:00:13.562275 temporian-0.8.1/temporian/implementation/numpy_cc/operators/resample.h
--rw-r--r--   0        0        0     1671 2024-03-27 13:00:13.562369 temporian-0.8.1/temporian/implementation/numpy_cc/operators/since_last.cc
--rw-r--r--   0        0        0      107 2024-03-27 13:00:13.562436 temporian-0.8.1/temporian/implementation/numpy_cc/operators/since_last.h
--rw-r--r--   0        0        0     4145 2024-03-27 13:00:13.562527 temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar.cc
--rw-r--r--   0        0        0      106 2024-03-27 13:00:13.562603 temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar.h
--rw-r--r--   0        0        0     2280 2024-03-27 13:00:13.562669 temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar_utils.cc
--rw-r--r--   0        0        0      542 2024-03-27 13:00:13.562746 temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar_utils.h
--rw-r--r--   0        0        0     2406 2024-03-27 13:00:13.562824 temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar_utils_test.cc
--rw-r--r--   0        0        0     1884 2024-03-27 13:00:13.562916 temporian-0.8.1/temporian/implementation/numpy_cc/operators/until_next.cc
--rw-r--r--   0        0        0      103 2024-03-27 13:00:13.562994 temporian-0.8.1/temporian/implementation/numpy_cc/operators/until_next.h
--rw-r--r--   0        0        0    29444 2024-03-27 13:00:13.563141 temporian-0.8.1/temporian/implementation/numpy_cc/operators/window.cc
--rw-r--r--   0        0        0      103 2024-03-27 13:00:13.563226 temporian-0.8.1/temporian/implementation/numpy_cc/operators/window.h
--rw-r--r--   0        0        0     1803 2024-03-27 13:00:13.563332 temporian-0.8.1/temporian/io/BUILD
--rw-r--r--   0        0        0      810 2024-03-27 13:00:13.563414 temporian-0.8.1/temporian/io/__init__.py
--rw-r--r--   0        0        0     3175 2024-03-27 13:00:13.563490 temporian-0.8.1/temporian/io/csv.py
--rw-r--r--   0        0        0     3307 2024-03-27 13:00:13.563570 temporian-0.8.1/temporian/io/format.py
--rw-r--r--   0        0        0     3218 2024-03-27 13:00:13.563636 temporian-0.8.1/temporian/io/numpy.py
--rw-r--r--   0        0        0     6405 2024-03-27 13:00:13.563727 temporian-0.8.1/temporian/io/pandas.py
--rw-r--r--   0        0        0     2647 2024-03-27 13:00:13.563807 temporian-0.8.1/temporian/io/parquet.py
--rw-r--r--   0        0        0    10580 2024-03-27 13:00:13.563908 temporian-0.8.1/temporian/io/tensorflow.py
--rw-r--r--   0        0        0     1606 2024-03-27 13:00:13.564015 temporian-0.8.1/temporian/io/test/BUILD
--rw-r--r--   0        0        0     3141 2024-03-27 13:00:13.564093 temporian-0.8.1/temporian/io/test/numpy_test.py
--rw-r--r--   0        0        0    17987 2024-03-27 13:00:13.564203 temporian-0.8.1/temporian/io/test/pandas_test.py
--rw-r--r--   0        0        0     1457 2024-03-27 13:00:13.564311 temporian-0.8.1/temporian/io/test/parquet_test.py
--rw-r--r--   0        0        0     7388 2024-03-27 13:00:13.564384 temporian-0.8.1/temporian/io/test/tensorflow_test.py
--rw-r--r--   0        0        0      257 2024-03-27 13:00:13.564479 temporian-0.8.1/temporian/proto/BUILD
--rw-r--r--   0        0        0      576 2024-03-27 13:00:13.564568 temporian-0.8.1/temporian/proto/__init__.py
--rw-r--r--   0        0        0     5549 2024-03-27 13:00:13.564658 temporian-0.8.1/temporian/proto/core.proto
--rw-r--r--   0        0        0     2097 2024-03-27 13:00:13.564764 temporian-0.8.1/temporian/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.564805 temporian-0.8.1/temporian/test/__init__.py
--rw-r--r--   0        0        0     4349 2024-03-27 13:00:13.564892 temporian-0.8.1/temporian/test/api_beam_test.py
--rw-r--r--   0        0        0     6535 2024-03-27 13:00:13.564980 temporian-0.8.1/temporian/test/api_test.py
--rw-r--r--   0        0        0     3625 2024-03-27 13:00:13.565059 temporian-0.8.1/temporian/test/doc_test.py
--rw-r--r--   0        0        0     1701 2024-03-27 13:00:13.565160 temporian-0.8.1/temporian/test/io_test.py
--rw-r--r--   0        0        0      151 2024-03-27 13:00:13.565271 temporian-0.8.1/temporian/test/test_data/BUILD
--rw-r--r--   0        0        0       78 2024-03-27 13:00:13.565370 temporian-0.8.1/temporian/test/test_data/io/input.csv
--rw-r--r--   0        0        0      100 2024-03-27 13:00:13.565478 temporian-0.8.1/temporian/test/test_data/prototype/left_event.csv
--rw-r--r--   0        0        0      124 2024-03-27 13:00:13.565556 temporian-0.8.1/temporian/test/test_data/prototype/output_event.csv
--rw-r--r--   0        0        0       99 2024-03-27 13:00:13.565636 temporian-0.8.1/temporian/test/test_data/prototype/right_event.csv
--rw-r--r--   0        0        0     4185 2024-03-27 13:00:13.565730 temporian-0.8.1/temporian/test/utils.py
--rw-r--r--   0        0        0      843 2024-03-27 13:00:13.565872 temporian-0.8.1/temporian/utils/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.565925 temporian-0.8.1/temporian/utils/__init__.py
--rw-r--r--   0        0        0     1615 2024-03-27 13:00:13.566012 temporian-0.8.1/temporian/utils/compile.bzl
--rw-r--r--   0        0        0     3433 2024-03-27 13:00:13.566095 temporian-0.8.1/temporian/utils/config.py
--rw-r--r--   0        0        0      678 2024-03-27 13:00:13.566182 temporian-0.8.1/temporian/utils/golden.py
--rw-r--r--   0        0        0      587 2024-03-27 13:00:13.566249 temporian-0.8.1/temporian/utils/string.py
--rw-r--r--   0        0        0      737 2024-03-27 13:00:13.566370 temporian-0.8.1/temporian/utils/test/BUILD
--rw-r--r--   0        0        0        0 2024-03-27 13:00:13.566409 temporian-0.8.1/temporian/utils/test/__init__.py
--rw-r--r--   0        0        0     1089 2024-03-27 13:00:13.566486 temporian-0.8.1/temporian/utils/test/string_test.py
--rw-r--r--   0        0        0     6279 2024-03-27 13:00:13.566566 temporian-0.8.1/temporian/utils/test/typecheck_test.py
--rw-r--r--   0        0        0    11569 2024-03-27 13:00:13.566666 temporian-0.8.1/temporian/utils/typecheck.py
--rw-r--r--   0        0        0     8782 1970-01-01 00:00:00.000000 temporian-0.8.1/setup.py
--rw-r--r--   0        0        0     7894 1970-01-01 00:00:00.000000 temporian-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-16 14:54:44.935942 temporian-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5846 2024-04-16 14:54:44.936023 temporian-0.9.0/README.md
+-rw-r--r--   0        0        0     3793 2024-04-16 14:54:44.936968 temporian-0.9.0/config/build.py
+-rw-r--r--   0        0        0     3371 2024-04-16 14:54:44.990392 temporian-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1540 2024-04-16 14:54:44.990508 temporian-0.9.0/temporian/BUILD
+-rw-r--r--   0        0        0     3379 2024-04-16 14:54:44.990594 temporian-0.9.0/temporian/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-16 14:54:44.990698 temporian-0.9.0/temporian/api/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:44.990725 temporian-0.9.0/temporian/api/__init__.py
+-rw-r--r--   0        0        0      134 2024-04-16 14:54:44.990805 temporian-0.9.0/temporian/api/duration.py
+-rw-r--r--   0        0        0      995 2024-04-16 14:54:44.990903 temporian-0.9.0/temporian/beam/BUILD
+-rw-r--r--   0        0        0     1418 2024-04-16 14:54:44.990980 temporian-0.9.0/temporian/beam/__init__.py
+-rw-r--r--   0        0        0     5896 2024-04-16 14:54:44.991110 temporian-0.9.0/temporian/beam/evaluation.py
+-rw-r--r--   0        0        0     2381 2024-04-16 14:54:44.991213 temporian-0.9.0/temporian/beam/implementation_lib.py
+-rw-r--r--   0        0        0     1430 2024-04-16 14:54:44.991300 temporian-0.9.0/temporian/beam/io/BUILD
+-rw-r--r--   0        0        0     5670 2024-04-16 14:54:44.991393 temporian-0.9.0/temporian/beam/io/csv.py
+-rw-r--r--   0        0        0    16648 2024-04-16 14:54:44.991510 temporian-0.9.0/temporian/beam/io/dict.py
+-rw-r--r--   0        0        0     2522 2024-04-16 14:54:44.991620 temporian-0.9.0/temporian/beam/io/np_array_coder.py
+-rw-r--r--   0        0        0     9389 2024-04-16 14:54:44.991707 temporian-0.9.0/temporian/beam/io/tensorflow.py
+-rw-r--r--   0        0        0     2184 2024-04-16 14:54:44.991797 temporian-0.9.0/temporian/beam/io/test/BUILD
+-rw-r--r--   0        0        0     5045 2024-04-16 14:54:44.991880 temporian-0.9.0/temporian/beam/io/test/csv_test.py
+-rw-r--r--   0        0        0     8929 2024-04-16 14:54:44.991994 temporian-0.9.0/temporian/beam/io/test/dict_test.py
+-rw-r--r--   0        0        0     1959 2024-04-16 14:54:44.992066 temporian-0.9.0/temporian/beam/io/test/np_array_coder_test.py
+-rw-r--r--   0        0        0     2316 2024-04-16 14:54:44.992173 temporian-0.9.0/temporian/beam/io/test/tensorflow_test.py
+-rw-r--r--   0        0        0     5896 2024-04-16 14:54:44.992291 temporian-0.9.0/temporian/beam/operators/BUILD
+-rw-r--r--   0        0        0     1928 2024-04-16 14:54:44.992398 temporian-0.9.0/temporian/beam/operators/__init__.py
+-rw-r--r--   0        0        0     4494 2024-04-16 14:54:44.992482 temporian-0.9.0/temporian/beam/operators/add_index.py
+-rw-r--r--   0        0        0     3406 2024-04-16 14:54:44.992591 temporian-0.9.0/temporian/beam/operators/base.py
+-rw-r--r--   0        0        0      415 2024-04-16 14:54:44.992678 temporian-0.9.0/temporian/beam/operators/binary/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:44.992721 temporian-0.9.0/temporian/beam/operators/binary/__init__.py
+-rw-r--r--   0        0        0     5380 2024-04-16 14:54:44.992796 temporian-0.9.0/temporian/beam/operators/binary/binary.py
+-rw-r--r--   0        0        0     1909 2024-04-16 14:54:44.992961 temporian-0.9.0/temporian/beam/operators/cast.py
+-rw-r--r--   0        0        0     6881 2024-04-16 14:54:44.993090 temporian-0.9.0/temporian/beam/operators/drop_index.py
+-rw-r--r--   0        0        0     2167 2024-04-16 14:54:44.993189 temporian-0.9.0/temporian/beam/operators/filter.py
+-rw-r--r--   0        0        0     1664 2024-04-16 14:54:44.993301 temporian-0.9.0/temporian/beam/operators/filter_empty_index.py
+-rw-r--r--   0        0        0     2042 2024-04-16 14:54:44.993419 temporian-0.9.0/temporian/beam/operators/filter_moving_count.py
+-rw-r--r--   0        0        0     1357 2024-04-16 14:54:44.993512 temporian-0.9.0/temporian/beam/operators/glue.py
+-rw-r--r--   0        0        0     1598 2024-04-16 14:54:44.993603 temporian-0.9.0/temporian/beam/operators/lag.py
+-rw-r--r--   0        0        0     1602 2024-04-16 14:54:44.993693 temporian-0.9.0/temporian/beam/operators/leak.py
+-rw-r--r--   0        0        0     1169 2024-04-16 14:54:44.993757 temporian-0.9.0/temporian/beam/operators/prefix.py
+-rw-r--r--   0        0        0     3895 2024-04-16 14:54:44.993835 temporian-0.9.0/temporian/beam/operators/propagate.py
+-rw-r--r--   0        0        0     1177 2024-04-16 14:54:44.993906 temporian-0.9.0/temporian/beam/operators/rename.py
+-rw-r--r--   0        0        0     3580 2024-04-16 14:54:44.993981 temporian-0.9.0/temporian/beam/operators/resample.py
+-rw-r--r--   0        0        0      415 2024-04-16 14:54:44.994076 temporian-0.9.0/temporian/beam/operators/scalar/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:44.994111 temporian-0.9.0/temporian/beam/operators/scalar/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-16 14:54:44.994217 temporian-0.9.0/temporian/beam/operators/scalar/scalar.py
+-rw-r--r--   0        0        0     1574 2024-04-16 14:54:44.994306 temporian-0.9.0/temporian/beam/operators/select.py
+-rw-r--r--   0        0        0     7710 2024-04-16 14:54:44.994391 temporian-0.9.0/temporian/beam/operators/test/BUILD
+-rw-r--r--   0        0        0     2252 2024-04-16 14:54:44.994469 temporian-0.9.0/temporian/beam/operators/test/add_index_test.py
+-rw-r--r--   0        0        0     2943 2024-04-16 14:54:44.994557 temporian-0.9.0/temporian/beam/operators/test/binary_test.py
+-rw-r--r--   0        0        0     2910 2024-04-16 14:54:44.994630 temporian-0.9.0/temporian/beam/operators/test/cast_test.py
+-rw-r--r--   0        0        0     3122 2024-04-16 14:54:44.994721 temporian-0.9.0/temporian/beam/operators/test/drop_index_test.py
+-rw-r--r--   0        0        0     1378 2024-04-16 14:54:44.994789 temporian-0.9.0/temporian/beam/operators/test/filter_empty_index_test.py
+-rw-r--r--   0        0        0     1445 2024-04-16 14:54:44.994858 temporian-0.9.0/temporian/beam/operators/test/filter_moving_count_test.py
+-rw-r--r--   0        0        0     1791 2024-04-16 14:54:44.995000 temporian-0.9.0/temporian/beam/operators/test/filter_test.py
+-rw-r--r--   0        0        0     1977 2024-04-16 14:54:44.995074 temporian-0.9.0/temporian/beam/operators/test/glue_test.py
+-rw-r--r--   0        0        0     1221 2024-04-16 14:54:44.995136 temporian-0.9.0/temporian/beam/operators/test/lag_test.py
+-rw-r--r--   0        0        0     1227 2024-04-16 14:54:44.995242 temporian-0.9.0/temporian/beam/operators/test/leak_test.py
+-rw-r--r--   0        0        0     1300 2024-04-16 14:54:44.995312 temporian-0.9.0/temporian/beam/operators/test/prefix_test.py
+-rw-r--r--   0        0        0     3076 2024-04-16 14:54:44.995376 temporian-0.9.0/temporian/beam/operators/test/propagate_test.py
+-rw-r--r--   0        0        0     3703 2024-04-16 14:54:44.995440 temporian-0.9.0/temporian/beam/operators/test/rename_test.py
+-rw-r--r--   0        0        0     1590 2024-04-16 14:54:44.995519 temporian-0.9.0/temporian/beam/operators/test/resample_test.py
+-rw-r--r--   0        0        0     2510 2024-04-16 14:54:44.995587 temporian-0.9.0/temporian/beam/operators/test/scalar_test.py
+-rw-r--r--   0        0        0     2205 2024-04-16 14:54:44.995653 temporian-0.9.0/temporian/beam/operators/test/select_test.py
+-rw-r--r--   0        0        0     1347 2024-04-16 14:54:44.995742 temporian-0.9.0/temporian/beam/operators/test/timestamps_test.py
+-rw-r--r--   0        0        0     1341 2024-04-16 14:54:44.995816 temporian-0.9.0/temporian/beam/operators/test/unique_timestamps_test.py
+-rw-r--r--   0        0        0     1568 2024-04-16 14:54:44.995887 temporian-0.9.0/temporian/beam/operators/timestamps.py
+-rw-r--r--   0        0        0     1616 2024-04-16 14:54:44.995952 temporian-0.9.0/temporian/beam/operators/unique_timestamps.py
+-rw-r--r--   0        0        0     2931 2024-04-16 14:54:44.996050 temporian-0.9.0/temporian/beam/operators/window/BUILD
+-rw-r--r--   0        0        0     3246 2024-04-16 14:54:44.996133 temporian-0.9.0/temporian/beam/operators/window/base.py
+-rw-r--r--   0        0        0     2759 2024-04-16 14:54:44.996183 temporian-0.9.0/temporian/beam/operators/window/moving_count.py
+-rw-r--r--   0        0        0     1310 2024-04-16 14:54:44.996252 temporian-0.9.0/temporian/beam/operators/window/moving_max.py
+-rw-r--r--   0        0        0     1310 2024-04-16 14:54:44.996329 temporian-0.9.0/temporian/beam/operators/window/moving_min.py
+-rw-r--r--   0        0        0     1424 2024-04-16 14:54:44.996397 temporian-0.9.0/temporian/beam/operators/window/moving_standard_deviation.py
+-rw-r--r--   0        0        0     1301 2024-04-16 14:54:44.996457 temporian-0.9.0/temporian/beam/operators/window/moving_sum.py
+-rw-r--r--   0        0        0     1392 2024-04-16 14:54:44.996544 temporian-0.9.0/temporian/beam/operators/window/simple_moving_average.py
+-rw-r--r--   0        0        0      507 2024-04-16 14:54:44.996645 temporian-0.9.0/temporian/beam/operators/window/test/BUILD
+-rw-r--r--   0        0        0     3636 2024-04-16 14:54:44.996725 temporian-0.9.0/temporian/beam/operators/window/test/window_test.py
+-rw-r--r--   0        0        0     1194 2024-04-16 14:54:44.996833 temporian-0.9.0/temporian/beam/test/BUILD
+-rw-r--r--   0        0        0     1713 2024-04-16 14:54:44.996939 temporian-0.9.0/temporian/beam/test/evaluation_test.py
+-rw-r--r--   0        0        0     3789 2024-04-16 14:54:44.997012 temporian-0.9.0/temporian/beam/test/utils.py
+-rw-r--r--   0        0        0     2915 2024-04-16 14:54:44.997098 temporian-0.9.0/temporian/beam/typing.py
+-rw-r--r--   0        0        0     2636 2024-04-16 14:54:44.997223 temporian-0.9.0/temporian/core/BUILD
+-rw-r--r--   0        0        0      576 2024-04-16 14:54:44.997299 temporian-0.9.0/temporian/core/__init__.py
+-rw-r--r--   0        0        0     6851 2024-04-16 14:54:44.997377 temporian-0.9.0/temporian/core/compilation.py
+-rw-r--r--   0        0        0      949 2024-04-16 14:54:44.997478 temporian-0.9.0/temporian/core/data/BUILD
+-rw-r--r--   0        0        0      576 2024-04-16 14:54:44.997535 temporian-0.9.0/temporian/core/data/__init__.py
+-rw-r--r--   0        0        0     3702 2024-04-16 14:54:44.997607 temporian-0.9.0/temporian/core/data/dtype.py
+-rw-r--r--   0        0        0     6484 2024-04-16 14:54:44.997700 temporian-0.9.0/temporian/core/data/duration.py
+-rw-r--r--   0        0        0     7878 2024-04-16 14:54:44.997810 temporian-0.9.0/temporian/core/data/duration_utils.py
+-rw-r--r--   0        0        0    12646 2024-04-16 14:54:44.997897 temporian-0.9.0/temporian/core/data/node.py
+-rw-r--r--   0        0        0     6171 2024-04-16 14:54:44.997969 temporian-0.9.0/temporian/core/data/schema.py
+-rw-r--r--   0        0        0      954 2024-04-16 14:54:44.998064 temporian-0.9.0/temporian/core/data/test/BUILD
+-rw-r--r--   0        0        0      985 2024-04-16 14:54:44.998162 temporian-0.9.0/temporian/core/data/test/schema_test.py
+-rw-r--r--   0        0        0      915 2024-04-16 14:54:44.998243 temporian-0.9.0/temporian/core/data/test/test_dtype.py
+-rw-r--r--   0        0        0     2209 2024-04-16 14:54:44.998315 temporian-0.9.0/temporian/core/data/test/test_node.py
+-rw-r--r--   0        0        0     1089 2024-04-16 14:54:44.998420 temporian-0.9.0/temporian/core/dataclasses.py
+-rw-r--r--   0        0        0    14621 2024-04-16 14:54:44.998540 temporian-0.9.0/temporian/core/evaluation.py
+-rw-r--r--   0        0        0   164199 2024-04-16 14:54:44.998901 temporian-0.9.0/temporian/core/event_set_ops.py
+-rw-r--r--   0        0        0    12130 2024-04-16 14:54:44.999007 temporian-0.9.0/temporian/core/graph.py
+-rw-r--r--   0        0        0     1632 2024-04-16 14:54:44.999076 temporian-0.9.0/temporian/core/operator_lib.py
+-rw-r--r--   0        0        0    12402 2024-04-16 14:54:44.999236 temporian-0.9.0/temporian/core/operators/BUILD
+-rw-r--r--   0        0        0      594 2024-04-16 14:54:44.999297 temporian-0.9.0/temporian/core/operators/__init__.py
+-rw-r--r--   0        0        0     4872 2024-04-16 14:54:44.999395 temporian-0.9.0/temporian/core/operators/add_index.py
+-rw-r--r--   0        0        0    13624 2024-04-16 14:54:44.999489 temporian-0.9.0/temporian/core/operators/base.py
+-rw-r--r--   0        0        0     1924 2024-04-16 14:54:44.999578 temporian-0.9.0/temporian/core/operators/begin.py
+-rw-r--r--   0        0        0     1648 2024-04-16 14:54:44.999663 temporian-0.9.0/temporian/core/operators/binary/BUILD
+-rw-r--r--   0        0        0     1373 2024-04-16 14:54:44.999727 temporian-0.9.0/temporian/core/operators/binary/__init__.py
+-rw-r--r--   0        0        0     4926 2024-04-16 14:54:44.999804 temporian-0.9.0/temporian/core/operators/binary/arithmetic.py
+-rw-r--r--   0        0        0     3860 2024-04-16 14:54:44.999896 temporian-0.9.0/temporian/core/operators/binary/base.py
+-rw-r--r--   0        0        0     3177 2024-04-16 14:54:44.999982 temporian-0.9.0/temporian/core/operators/binary/logical.py
+-rw-r--r--   0        0        0     4140 2024-04-16 14:54:45.000036 temporian-0.9.0/temporian/core/operators/binary/relational.py
+-rw-r--r--   0        0        0     3242 2024-04-16 14:54:45.000181 temporian-0.9.0/temporian/core/operators/calendar/BUILD
+-rw-r--r--   0        0        0     1284 2024-04-16 14:54:45.000271 temporian-0.9.0/temporian/core/operators/calendar/__init__.py
+-rw-r--r--   0        0        0     2791 2024-04-16 14:54:45.000363 temporian-0.9.0/temporian/core/operators/calendar/base.py
+-rw-r--r--   0        0        0     1489 2024-04-16 14:54:45.000467 temporian-0.9.0/temporian/core/operators/calendar/day_of_month.py
+-rw-r--r--   0        0        0     1483 2024-04-16 14:54:45.000536 temporian-0.9.0/temporian/core/operators/calendar/day_of_week.py
+-rw-r--r--   0        0        0     1483 2024-04-16 14:54:45.000644 temporian-0.9.0/temporian/core/operators/calendar/day_of_year.py
+-rw-r--r--   0        0        0     1440 2024-04-16 14:54:45.000729 temporian-0.9.0/temporian/core/operators/calendar/hour.py
+-rw-r--r--   0        0        0     1465 2024-04-16 14:54:45.000784 temporian-0.9.0/temporian/core/operators/calendar/iso_week.py
+-rw-r--r--   0        0        0     1454 2024-04-16 14:54:45.000953 temporian-0.9.0/temporian/core/operators/calendar/minute.py
+-rw-r--r--   0        0        0     1447 2024-04-16 14:54:45.001028 temporian-0.9.0/temporian/core/operators/calendar/month.py
+-rw-r--r--   0        0        0     1454 2024-04-16 14:54:45.001134 temporian-0.9.0/temporian/core/operators/calendar/second.py
+-rw-r--r--   0        0        0     3612 2024-04-16 14:54:45.001228 temporian-0.9.0/temporian/core/operators/calendar/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.001255 temporian-0.9.0/temporian/core/operators/calendar/test/__init__.py
+-rw-r--r--   0        0        0     1941 2024-04-16 14:54:45.001351 temporian-0.9.0/temporian/core/operators/calendar/test/test_base.py
+-rw-r--r--   0        0        0     4502 2024-04-16 14:54:45.001427 temporian-0.9.0/temporian/core/operators/calendar/test/test_base_timezone.py
+-rw-r--r--   0        0        0     2924 2024-04-16 14:54:45.001512 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_day_of_month.py
+-rw-r--r--   0        0        0     1625 2024-04-16 14:54:45.001617 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_day_of_week.py
+-rw-r--r--   0        0        0     2141 2024-04-16 14:54:45.001718 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_day_of_year.py
+-rw-r--r--   0        0        0     3151 2024-04-16 14:54:45.001807 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_hour.py
+-rw-r--r--   0        0        0     1790 2024-04-16 14:54:45.001857 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_iso_week.py
+-rw-r--r--   0        0        0     1474 2024-04-16 14:54:45.001916 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_minute.py
+-rw-r--r--   0        0        0     2104 2024-04-16 14:54:45.001995 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_month.py
+-rw-r--r--   0        0        0     1436 2024-04-16 14:54:45.002050 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_second.py
+-rw-r--r--   0        0        0     3346 2024-04-16 14:54:45.002105 temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_year.py
+-rw-r--r--   0        0        0     1440 2024-04-16 14:54:45.002182 temporian-0.9.0/temporian/core/operators/calendar/year.py
+-rw-r--r--   0        0        0     5886 2024-04-16 14:54:45.002264 temporian-0.9.0/temporian/core/operators/cast.py
+-rw-r--r--   0        0        0     7785 2024-04-16 14:54:45.002400 temporian-0.9.0/temporian/core/operators/combine.py
+-rw-r--r--   0        0        0     4699 2024-04-16 14:54:45.002460 temporian-0.9.0/temporian/core/operators/drop_index.py
+-rw-r--r--   0        0        0     1913 2024-04-16 14:54:45.002549 temporian-0.9.0/temporian/core/operators/end.py
+-rw-r--r--   0        0        0     1925 2024-04-16 14:54:45.002655 temporian-0.9.0/temporian/core/operators/enumerate.py
+-rw-r--r--   0        0        0     5794 2024-04-16 14:54:45.002718 temporian-0.9.0/temporian/core/operators/fast_fourier_transform.py
+-rw-r--r--   0        0        0     1363 2024-04-16 14:54:45.002793 temporian-0.9.0/temporian/core/operators/fillna.py
+-rw-r--r--   0        0        0     4286 2024-04-16 14:54:45.002854 temporian-0.9.0/temporian/core/operators/filter.py
+-rw-r--r--   0        0        0     2049 2024-04-16 14:54:45.002954 temporian-0.9.0/temporian/core/operators/filter_empty_index.py
+-rw-r--r--   0        0        0     2695 2024-04-16 14:54:45.003018 temporian-0.9.0/temporian/core/operators/filter_moving_count.py
+-rw-r--r--   0        0        0     6709 2024-04-16 14:54:45.003116 temporian-0.9.0/temporian/core/operators/glue.py
+-rw-r--r--   0        0        0     4992 2024-04-16 14:54:45.003205 temporian-0.9.0/temporian/core/operators/join.py
+-rw-r--r--   0        0        0     2613 2024-04-16 14:54:45.003286 temporian-0.9.0/temporian/core/operators/lag.py
+-rw-r--r--   0        0        0     2709 2024-04-16 14:54:45.003354 temporian-0.9.0/temporian/core/operators/leak.py
+-rw-r--r--   0        0        0     5031 2024-04-16 14:54:45.003398 temporian-0.9.0/temporian/core/operators/map.py
+-rw-r--r--   0        0        0     2492 2024-04-16 14:54:45.003464 temporian-0.9.0/temporian/core/operators/prefix.py
+-rw-r--r--   0        0        0     3965 2024-04-16 14:54:45.003546 temporian-0.9.0/temporian/core/operators/propagate.py
+-rw-r--r--   0        0        0     7064 2024-04-16 14:54:45.003604 temporian-0.9.0/temporian/core/operators/rename.py
+-rw-r--r--   0        0        0     2298 2024-04-16 14:54:45.003668 temporian-0.9.0/temporian/core/operators/resample.py
+-rw-r--r--   0        0        0     1310 2024-04-16 14:54:45.003764 temporian-0.9.0/temporian/core/operators/scalar/BUILD
+-rw-r--r--   0        0        0     1378 2024-04-16 14:54:45.003846 temporian-0.9.0/temporian/core/operators/scalar/__init__.py
+-rw-r--r--   0        0        0     8001 2024-04-16 14:54:45.003934 temporian-0.9.0/temporian/core/operators/scalar/arithmetic_scalar.py
+-rw-r--r--   0        0        0     5219 2024-04-16 14:54:45.004009 temporian-0.9.0/temporian/core/operators/scalar/base.py
+-rw-r--r--   0        0        0     4119 2024-04-16 14:54:45.004086 temporian-0.9.0/temporian/core/operators/scalar/relational_scalar.py
+-rw-r--r--   0        0        0     4334 2024-04-16 14:54:45.004170 temporian-0.9.0/temporian/core/operators/select.py
+-rw-r--r--   0        0        0     4305 2024-04-16 14:54:45.004249 temporian-0.9.0/temporian/core/operators/select_index_values.py
+-rw-r--r--   0        0        0     3412 2024-04-16 14:54:45.004336 temporian-0.9.0/temporian/core/operators/since_last.py
+-rw-r--r--   0        0        0    12676 2024-04-16 14:54:45.004431 temporian-0.9.0/temporian/core/operators/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.004468 temporian-0.9.0/temporian/core/operators/test/__init__.py
+-rw-r--r--   0        0        0     7083 2024-04-16 14:54:45.004544 temporian-0.9.0/temporian/core/operators/test/test_add_index.py
+-rw-r--r--   0        0        0     3375 2024-04-16 14:54:45.004621 temporian-0.9.0/temporian/core/operators/test/test_after.py
+-rw-r--r--   0        0        0     5671 2024-04-16 14:54:45.004696 temporian-0.9.0/temporian/core/operators/test/test_arithmetic.py
+-rw-r--r--   0        0        0     8127 2024-04-16 14:54:45.004780 temporian-0.9.0/temporian/core/operators/test/test_arithmetic_scalar.py
+-rw-r--r--   0        0        0     4239 2024-04-16 14:54:45.004858 temporian-0.9.0/temporian/core/operators/test/test_assign.py
+-rw-r--r--   0        0        0     3410 2024-04-16 14:54:45.004927 temporian-0.9.0/temporian/core/operators/test/test_before.py
+-rw-r--r--   0        0        0     1512 2024-04-16 14:54:45.005029 temporian-0.9.0/temporian/core/operators/test/test_begin.py
+-rw-r--r--   0        0        0     4874 2024-04-16 14:54:45.005098 temporian-0.9.0/temporian/core/operators/test/test_cast.py
+-rw-r--r--   0        0        0     8436 2024-04-16 14:54:45.005188 temporian-0.9.0/temporian/core/operators/test/test_combine.py
+-rw-r--r--   0        0        0     2023 2024-04-16 14:54:45.005250 temporian-0.9.0/temporian/core/operators/test/test_drop.py
+-rw-r--r--   0        0        0     4383 2024-04-16 14:54:45.005329 temporian-0.9.0/temporian/core/operators/test/test_drop_index.py
+-rw-r--r--   0        0        0     1506 2024-04-16 14:54:45.005420 temporian-0.9.0/temporian/core/operators/test/test_end.py
+-rw-r--r--   0        0        0     1794 2024-04-16 14:54:45.005498 temporian-0.9.0/temporian/core/operators/test/test_enumerate.py
+-rw-r--r--   0        0        0     4338 2024-04-16 14:54:45.005580 temporian-0.9.0/temporian/core/operators/test/test_fast_fourier_transform.py
+-rw-r--r--   0        0        0     1767 2024-04-16 14:54:45.005658 temporian-0.9.0/temporian/core/operators/test/test_fillna.py
+-rw-r--r--   0        0        0     2321 2024-04-16 14:54:45.005740 temporian-0.9.0/temporian/core/operators/test/test_filter.py
+-rw-r--r--   0        0        0     1443 2024-04-16 14:54:45.005843 temporian-0.9.0/temporian/core/operators/test/test_filter_empty_index.py
+-rw-r--r--   0        0        0     2538 2024-04-16 14:54:45.005942 temporian-0.9.0/temporian/core/operators/test/test_filter_moving_count.py
+-rw-r--r--   0        0        0     6214 2024-04-16 14:54:45.005992 temporian-0.9.0/temporian/core/operators/test/test_glue.py
+-rw-r--r--   0        0        0     4476 2024-04-16 14:54:45.006069 temporian-0.9.0/temporian/core/operators/test/test_join.py
+-rw-r--r--   0        0        0     1328 2024-04-16 14:54:45.006126 temporian-0.9.0/temporian/core/operators/test/test_lag.py
+-rw-r--r--   0        0        0     1330 2024-04-16 14:54:45.006193 temporian-0.9.0/temporian/core/operators/test/test_leak.py
+-rw-r--r--   0        0        0     2187 2024-04-16 14:54:45.006262 temporian-0.9.0/temporian/core/operators/test/test_logical.py
+-rw-r--r--   0        0        0     4990 2024-04-16 14:54:45.006354 temporian-0.9.0/temporian/core/operators/test/test_map.py
+-rw-r--r--   0        0        0     1503 2024-04-16 14:54:45.006414 temporian-0.9.0/temporian/core/operators/test/test_prefix.py
+-rw-r--r--   0        0        0     3763 2024-04-16 14:54:45.006488 temporian-0.9.0/temporian/core/operators/test/test_propagate.py
+-rw-r--r--   0        0        0     5967 2024-04-16 14:54:45.006533 temporian-0.9.0/temporian/core/operators/test/test_relational.py
+-rw-r--r--   0        0        0     5801 2024-04-16 14:54:45.006611 temporian-0.9.0/temporian/core/operators/test/test_relational_scalar.py
+-rw-r--r--   0        0        0     8367 2024-04-16 14:54:45.006671 temporian-0.9.0/temporian/core/operators/test/test_rename.py
+-rw-r--r--   0        0        0     1899 2024-04-16 14:54:45.006727 temporian-0.9.0/temporian/core/operators/test/test_resample.py
+-rw-r--r--   0        0        0     2080 2024-04-16 14:54:45.006837 temporian-0.9.0/temporian/core/operators/test/test_select.py
+-rw-r--r--   0        0        0     6339 2024-04-16 14:54:45.006907 temporian-0.9.0/temporian/core/operators/test/test_select_index_values.py
+-rw-r--r--   0        0        0     3203 2024-04-16 14:54:45.006991 temporian-0.9.0/temporian/core/operators/test/test_since_last.py
+-rw-r--r--   0        0        0     9156 2024-04-16 14:54:45.007108 temporian-0.9.0/temporian/core/operators/test/test_tick.py
+-rw-r--r--   0        0        0    11962 2024-04-16 14:54:45.007169 temporian-0.9.0/temporian/core/operators/test/test_tick_calendar.py
+-rw-r--r--   0        0        0     2305 2024-04-16 14:54:45.007238 temporian-0.9.0/temporian/core/operators/test/test_timestamps.py
+-rw-r--r--   0        0        0     6093 2024-04-16 14:54:45.007282 temporian-0.9.0/temporian/core/operators/test/test_unary.py
+-rw-r--r--   0        0        0     1408 2024-04-16 14:54:45.007339 temporian-0.9.0/temporian/core/operators/test/test_unique_timestamps.py
+-rw-r--r--   0        0        0     2302 2024-04-16 14:54:45.007409 temporian-0.9.0/temporian/core/operators/test/test_until_next.py
+-rw-r--r--   0        0        0     8807 2024-04-16 14:54:45.007498 temporian-0.9.0/temporian/core/operators/test/test_where.py
+-rw-r--r--   0        0        0     3795 2024-04-16 14:54:45.007599 temporian-0.9.0/temporian/core/operators/tick.py
+-rw-r--r--   0        0        0     9133 2024-04-16 14:54:45.007668 temporian-0.9.0/temporian/core/operators/tick_calendar.py
+-rw-r--r--   0        0        0     1934 2024-04-16 14:54:45.007739 temporian-0.9.0/temporian/core/operators/timestamps.py
+-rw-r--r--   0        0        0     9755 2024-04-16 14:54:45.007812 temporian-0.9.0/temporian/core/operators/unary.py
+-rw-r--r--   0        0        0     2028 2024-04-16 14:54:45.007877 temporian-0.9.0/temporian/core/operators/unique_timestamps.py
+-rw-r--r--   0        0        0     3096 2024-04-16 14:54:45.007952 temporian-0.9.0/temporian/core/operators/until_next.py
+-rw-r--r--   0        0        0     6746 2024-04-16 14:54:45.008026 temporian-0.9.0/temporian/core/operators/where.py
+-rw-r--r--   0        0        0     3501 2024-04-16 14:54:45.008123 temporian-0.9.0/temporian/core/operators/window/BUILD
+-rw-r--r--   0        0        0     1333 2024-04-16 14:54:45.008207 temporian-0.9.0/temporian/core/operators/window/__init__.py
+-rw-r--r--   0        0        0     5127 2024-04-16 14:54:45.008256 temporian-0.9.0/temporian/core/operators/window/base.py
+-rw-r--r--   0        0        0     1861 2024-04-16 14:54:45.008334 temporian-0.9.0/temporian/core/operators/window/moving_count.py
+-rw-r--r--   0        0        0     2021 2024-04-16 14:54:45.008401 temporian-0.9.0/temporian/core/operators/window/moving_max.py
+-rw-r--r--   0        0        0     2021 2024-04-16 14:54:45.008465 temporian-0.9.0/temporian/core/operators/window/moving_min.py
+-rw-r--r--   0        0        0     2706 2024-04-16 14:54:45.008533 temporian-0.9.0/temporian/core/operators/window/moving_product.py
+-rw-r--r--   0        0        0     2270 2024-04-16 14:54:45.008610 temporian-0.9.0/temporian/core/operators/window/moving_standard_deviation.py
+-rw-r--r--   0        0        0     2396 2024-04-16 14:54:45.008679 temporian-0.9.0/temporian/core/operators/window/moving_sum.py
+-rw-r--r--   0        0        0     2378 2024-04-16 14:54:45.008734 temporian-0.9.0/temporian/core/operators/window/simple_moving_average.py
+-rw-r--r--   0        0        0     3581 2024-04-16 14:54:45.008852 temporian-0.9.0/temporian/core/operators/window/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.008885 temporian-0.9.0/temporian/core/operators/window/test/__init__.py
+-rw-r--r--   0        0        0     5465 2024-04-16 14:54:45.008958 temporian-0.9.0/temporian/core/operators/window/test/test_base.py
+-rw-r--r--   0        0        0     2177 2024-04-16 14:54:45.009031 temporian-0.9.0/temporian/core/operators/window/test/test_cumprod.py
+-rw-r--r--   0        0        0     1967 2024-04-16 14:54:45.009098 temporian-0.9.0/temporian/core/operators/window/test/test_cumsum.py
+-rw-r--r--   0        0        0     3006 2024-04-16 14:54:45.009163 temporian-0.9.0/temporian/core/operators/window/test/test_moving_count.py
+-rw-r--r--   0        0        0     3619 2024-04-16 14:54:45.009248 temporian-0.9.0/temporian/core/operators/window/test/test_moving_max.py
+-rw-r--r--   0        0        0     3614 2024-04-16 14:54:45.009324 temporian-0.9.0/temporian/core/operators/window/test/test_moving_min.py
+-rw-r--r--   0        0        0     7455 2024-04-16 14:54:45.009395 temporian-0.9.0/temporian/core/operators/window/test/test_moving_product.py
+-rw-r--r--   0        0        0     6752 2024-04-16 14:54:45.009473 temporian-0.9.0/temporian/core/operators/window/test/test_moving_standard_deviation.py
+-rw-r--r--   0        0        0     6064 2024-04-16 14:54:45.009579 temporian-0.9.0/temporian/core/operators/window/test/test_moving_sum.py
+-rw-r--r--   0        0        0     9814 2024-04-16 14:54:45.009683 temporian-0.9.0/temporian/core/operators/window/test/test_simple_moving_average.py
+-rw-r--r--   0        0        0     1099 2024-04-16 14:54:45.009758 temporian-0.9.0/temporian/core/schedule.py
+-rw-r--r--   0        0        0    24326 2024-04-16 14:54:45.009882 temporian-0.9.0/temporian/core/serialization.py
+-rw-r--r--   0        0        0     3160 2024-04-16 14:54:45.009998 temporian-0.9.0/temporian/core/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.010028 temporian-0.9.0/temporian/core/test/__init__.py
+-rw-r--r--   0        0        0     6248 2024-04-16 14:54:45.010112 temporian-0.9.0/temporian/core/test/compilation_test.py
+-rw-r--r--   0        0        0     7630 2024-04-16 14:54:45.010204 temporian-0.9.0/temporian/core/test/evaluation_test.py
+-rw-r--r--   0        0        0     8133 2024-04-16 14:54:45.010309 temporian-0.9.0/temporian/core/test/graph_test.py
+-rw-r--r--   0        0        0    23120 2024-04-16 14:54:45.010432 temporian-0.9.0/temporian/core/test/magic_methods_test.py
+-rw-r--r--   0        0        0     5213 2024-04-16 14:54:45.010517 temporian-0.9.0/temporian/core/test/operator_test.py
+-rw-r--r--   0        0        0     3573 2024-04-16 14:54:45.010659 temporian-0.9.0/temporian/core/test/registered_operators_test.py
+-rw-r--r--   0        0        0    20736 2024-04-16 14:54:45.010775 temporian-0.9.0/temporian/core/test/serialization_test.py
+-rw-r--r--   0        0        0     9072 2024-04-16 14:54:45.010889 temporian-0.9.0/temporian/core/test/utils.py
+-rw-r--r--   0        0        0     1428 2024-04-16 14:54:45.010956 temporian-0.9.0/temporian/core/types.py
+-rw-r--r--   0        0        0     5230 2024-04-16 14:54:45.011065 temporian-0.9.0/temporian/core/typing.py
+-rw-r--r--   0        0        0      211 2024-04-16 14:54:45.011172 temporian-0.9.0/temporian/implementation/BUILD
+-rw-r--r--   0        0        0      576 2024-04-16 14:54:45.011225 temporian-0.9.0/temporian/implementation/__init__.py
+-rw-r--r--   0        0        0      649 2024-04-16 14:54:45.011356 temporian-0.9.0/temporian/implementation/numpy/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.011391 temporian-0.9.0/temporian/implementation/numpy/__init__.py
+-rw-r--r--   0        0        0     2404 2024-04-16 14:54:45.011519 temporian-0.9.0/temporian/implementation/numpy/data/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.011549 temporian-0.9.0/temporian/implementation/numpy/data/__init__.py
+-rw-r--r--   0        0        0    15177 2024-04-16 14:54:45.011658 temporian-0.9.0/temporian/implementation/numpy/data/display_utils.py
+-rw-r--r--   0        0        0    11353 2024-04-16 14:54:45.011759 temporian-0.9.0/temporian/implementation/numpy/data/dtype_normalization.py
+-rw-r--r--   0        0        0    11478 2024-04-16 14:54:45.011836 temporian-0.9.0/temporian/implementation/numpy/data/event_set.py
+-rw-r--r--   0        0        0    11129 2024-04-16 14:54:45.011926 temporian-0.9.0/temporian/implementation/numpy/data/io.py
+-rw-r--r--   0        0        0    17286 2024-04-16 14:54:45.012047 temporian-0.9.0/temporian/implementation/numpy/data/plotter.py
+-rw-r--r--   0        0        0     2258 2024-04-16 14:54:45.012130 temporian-0.9.0/temporian/implementation/numpy/data/plotter_base.py
+-rw-r--r--   0        0        0     6672 2024-04-16 14:54:45.012225 temporian-0.9.0/temporian/implementation/numpy/data/plotter_bokeh.py
+-rw-r--r--   0        0        0     4784 2024-04-16 14:54:45.012307 temporian-0.9.0/temporian/implementation/numpy/data/plotter_matplotlib.py
+-rw-r--r--   0        0        0     1359 2024-04-16 14:54:45.012420 temporian-0.9.0/temporian/implementation/numpy/data/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.012448 temporian-0.9.0/temporian/implementation/numpy/data/test/__init__.py
+-rw-r--r--   0        0        0     5005 2024-04-16 14:54:45.012545 temporian-0.9.0/temporian/implementation/numpy/data/test/event_set_test.py
+-rw-r--r--   0        0        0     8293 2024-04-16 14:54:45.012633 temporian-0.9.0/temporian/implementation/numpy/data/test/io_test.py
+-rw-r--r--   0        0        0     7143 2024-04-16 14:54:45.012708 temporian-0.9.0/temporian/implementation/numpy/data/test/plotter_test.py
+-rw-r--r--   0        0        0      151 2024-04-16 14:54:45.012797 temporian-0.9.0/temporian/implementation/numpy/data/test/test_data/BUILD
+-rw-r--r--   0        0        0     2804 2024-04-16 14:54:45.012894 temporian-0.9.0/temporian/implementation/numpy/data/test/test_data/test_html_repr_limits_golden.html
+-rw-r--r--   0        0        0     3969 2024-04-16 14:54:45.012966 temporian-0.9.0/temporian/implementation/numpy/data/test/test_data/test_html_repr_no_limits_golden.html
+-rw-r--r--   0        0        0     4883 2024-04-16 14:54:45.013046 temporian-0.9.0/temporian/implementation/numpy/evaluation.py
+-rw-r--r--   0        0        0     1655 2024-04-16 14:54:45.013121 temporian-0.9.0/temporian/implementation/numpy/implementation_lib.py
+-rw-r--r--   0        0        0    13367 2024-04-16 14:54:45.013221 temporian-0.9.0/temporian/implementation/numpy/operators/BUILD
+-rw-r--r--   0        0        0     4131 2024-04-16 14:54:45.013272 temporian-0.9.0/temporian/implementation/numpy/operators/__init__.py
+-rw-r--r--   0        0        0     2488 2024-04-16 14:54:45.013345 temporian-0.9.0/temporian/implementation/numpy/operators/add_index.py
+-rw-r--r--   0        0        0     8088 2024-04-16 14:54:45.013428 temporian-0.9.0/temporian/implementation/numpy/operators/base.py
+-rw-r--r--   0        0        0     2175 2024-04-16 14:54:45.013507 temporian-0.9.0/temporian/implementation/numpy/operators/begin.py
+-rw-r--r--   0        0        0     1554 2024-04-16 14:54:45.013589 temporian-0.9.0/temporian/implementation/numpy/operators/binary/BUILD
+-rw-r--r--   0        0        0      772 2024-04-16 14:54:45.013651 temporian-0.9.0/temporian/implementation/numpy/operators/binary/__init__.py
+-rw-r--r--   0        0        0     5385 2024-04-16 14:54:45.013738 temporian-0.9.0/temporian/implementation/numpy/operators/binary/arithmetic.py
+-rw-r--r--   0        0        0     3478 2024-04-16 14:54:45.013802 temporian-0.9.0/temporian/implementation/numpy/operators/binary/base.py
+-rw-r--r--   0        0        0     2619 2024-04-16 14:54:45.013882 temporian-0.9.0/temporian/implementation/numpy/operators/binary/logical.py
+-rw-r--r--   0        0        0     4280 2024-04-16 14:54:45.013952 temporian-0.9.0/temporian/implementation/numpy/operators/binary/relational.py
+-rw-r--r--   0        0        0     2578 2024-04-16 14:54:45.014043 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.014076 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/__init__.py
+-rw-r--r--   0        0        0     1671 2024-04-16 14:54:45.014155 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/base.py
+-rw-r--r--   0        0        0     1240 2024-04-16 14:54:45.014208 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/day_of_month.py
+-rw-r--r--   0        0        0     1233 2024-04-16 14:54:45.014279 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/day_of_week.py
+-rw-r--r--   0        0        0     1234 2024-04-16 14:54:45.014340 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/day_of_year.py
+-rw-r--r--   0        0        0     1191 2024-04-16 14:54:45.014405 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/hour.py
+-rw-r--r--   0        0        0     1210 2024-04-16 14:54:45.014464 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/iso_week.py
+-rw-r--r--   0        0        0     1203 2024-04-16 14:54:45.014529 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/minute.py
+-rw-r--r--   0        0        0     1197 2024-04-16 14:54:45.014601 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/month.py
+-rw-r--r--   0        0        0     1203 2024-04-16 14:54:45.014666 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/second.py
+-rw-r--r--   0        0        0     1191 2024-04-16 14:54:45.014710 temporian-0.9.0/temporian/implementation/numpy/operators/calendar/year.py
+-rw-r--r--   0        0        0     4238 2024-04-16 14:54:45.014788 temporian-0.9.0/temporian/implementation/numpy/operators/cast.py
+-rw-r--r--   0        0        0     4140 2024-04-16 14:54:45.014873 temporian-0.9.0/temporian/implementation/numpy/operators/combine.py
+-rw-r--r--   0        0        0     3955 2024-04-16 14:54:45.014953 temporian-0.9.0/temporian/implementation/numpy/operators/drop_index.py
+-rw-r--r--   0        0        0     2158 2024-04-16 14:54:45.015027 temporian-0.9.0/temporian/implementation/numpy/operators/end.py
+-rw-r--r--   0        0        0     1978 2024-04-16 14:54:45.015095 temporian-0.9.0/temporian/implementation/numpy/operators/enumerate.py
+-rw-r--r--   0        0        0     3412 2024-04-16 14:54:45.015186 temporian-0.9.0/temporian/implementation/numpy/operators/fast_fourier_transform.py
+-rw-r--r--   0        0        0     1639 2024-04-16 14:54:45.015273 temporian-0.9.0/temporian/implementation/numpy/operators/filter.py
+-rw-r--r--   0        0        0     2053 2024-04-16 14:54:45.015344 temporian-0.9.0/temporian/implementation/numpy/operators/filter_empty_index.py
+-rw-r--r--   0        0        0     2359 2024-04-16 14:54:45.015415 temporian-0.9.0/temporian/implementation/numpy/operators/filter_moving_count.py
+-rw-r--r--   0        0        0     2124 2024-04-16 14:54:45.015492 temporian-0.9.0/temporian/implementation/numpy/operators/glue.py
+-rw-r--r--   0        0        0     4509 2024-04-16 14:54:45.015564 temporian-0.9.0/temporian/implementation/numpy/operators/join.py
+-rw-r--r--   0        0        0     1951 2024-04-16 14:54:45.015638 temporian-0.9.0/temporian/implementation/numpy/operators/lag.py
+-rw-r--r--   0        0        0     2070 2024-04-16 14:54:45.015704 temporian-0.9.0/temporian/implementation/numpy/operators/leak.py
+-rw-r--r--   0        0        0     3846 2024-04-16 14:54:45.015810 temporian-0.9.0/temporian/implementation/numpy/operators/map.py
+-rw-r--r--   0        0        0     1551 2024-04-16 14:54:45.015863 temporian-0.9.0/temporian/implementation/numpy/operators/prefix.py
+-rw-r--r--   0        0        0     2745 2024-04-16 14:54:45.015929 temporian-0.9.0/temporian/implementation/numpy/operators/propagate.py
+-rw-r--r--   0        0        0     1756 2024-04-16 14:54:45.015993 temporian-0.9.0/temporian/implementation/numpy/operators/rename.py
+-rw-r--r--   0        0        0     4157 2024-04-16 14:54:45.016071 temporian-0.9.0/temporian/implementation/numpy/operators/resample.py
+-rw-r--r--   0        0        0     1272 2024-04-16 14:54:45.016153 temporian-0.9.0/temporian/implementation/numpy/operators/scalar/BUILD
+-rw-r--r--   0        0        0      692 2024-04-16 14:54:45.016210 temporian-0.9.0/temporian/implementation/numpy/operators/scalar/__init__.py
+-rw-r--r--   0        0        0     4499 2024-04-16 14:54:45.016269 temporian-0.9.0/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py
+-rw-r--r--   0        0        0     2591 2024-04-16 14:54:45.016356 temporian-0.9.0/temporian/implementation/numpy/operators/scalar/base.py
+-rw-r--r--   0        0        0     3613 2024-04-16 14:54:45.016414 temporian-0.9.0/temporian/implementation/numpy/operators/scalar/relational_scalar.py
+-rw-r--r--   0        0        0     2355 2024-04-16 14:54:45.016486 temporian-0.9.0/temporian/implementation/numpy/operators/select.py
+-rw-r--r--   0        0        0     2811 2024-04-16 14:54:45.016567 temporian-0.9.0/temporian/implementation/numpy/operators/select_index_values.py
+-rw-r--r--   0        0        0     2981 2024-04-16 14:54:45.016649 temporian-0.9.0/temporian/implementation/numpy/operators/since_last.py
+-rw-r--r--   0        0        0     3503 2024-04-16 14:54:45.016733 temporian-0.9.0/temporian/implementation/numpy/operators/tick.py
+-rw-r--r--   0        0        0     4673 2024-04-16 14:54:45.016775 temporian-0.9.0/temporian/implementation/numpy/operators/tick_calendar.py
+-rw-r--r--   0        0        0     1955 2024-04-16 14:54:45.016831 temporian-0.9.0/temporian/implementation/numpy/operators/timestamps.py
+-rw-r--r--   0        0        0     4554 2024-04-16 14:54:45.016908 temporian-0.9.0/temporian/implementation/numpy/operators/unary.py
+-rw-r--r--   0        0        0     1937 2024-04-16 14:54:45.017000 temporian-0.9.0/temporian/implementation/numpy/operators/unique_timestamps.py
+-rw-r--r--   0        0        0     2486 2024-04-16 14:54:45.017054 temporian-0.9.0/temporian/implementation/numpy/operators/until_next.py
+-rw-r--r--   0        0        0     2820 2024-04-16 14:54:45.017117 temporian-0.9.0/temporian/implementation/numpy/operators/where.py
+-rw-r--r--   0        0        0     3050 2024-04-16 14:54:45.017231 temporian-0.9.0/temporian/implementation/numpy/operators/window/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.017258 temporian-0.9.0/temporian/implementation/numpy/operators/window/__init__.py
+-rw-r--r--   0        0        0     7731 2024-04-16 14:54:45.017334 temporian-0.9.0/temporian/implementation/numpy/operators/window/base.py
+-rw-r--r--   0        0        0     3694 2024-04-16 14:54:45.017397 temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_count.py
+-rw-r--r--   0        0        0     1203 2024-04-16 14:54:45.017490 temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_max.py
+-rw-r--r--   0        0        0     1203 2024-04-16 14:54:45.017554 temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_min.py
+-rw-r--r--   0        0        0     1231 2024-04-16 14:54:45.017610 temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_product.py
+-rw-r--r--   0        0        0     1304 2024-04-16 14:54:45.017676 temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_standard_deviation.py
+-rw-r--r--   0        0        0     1203 2024-04-16 14:54:45.017741 temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_sum.py
+-rw-r--r--   0        0        0     1276 2024-04-16 14:54:45.017797 temporian-0.9.0/temporian/implementation/numpy/operators/window/simple_moving_average.py
+-rw-r--r--   0        0        0      481 2024-04-16 14:54:45.017900 temporian-0.9.0/temporian/implementation/numpy/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.017932 temporian-0.9.0/temporian/implementation/numpy/test/__init__.py
+-rw-r--r--   0        0        0     3650 2024-04-16 14:54:45.018015 temporian-0.9.0/temporian/implementation/numpy/test/registered_operators_test.py
+-rw-r--r--   0        0        0       92 2024-04-16 14:54:45.018101 temporian-0.9.0/temporian/implementation/numpy_cc/BUILD
+-rw-r--r--   0        0        0      576 2024-04-16 14:54:45.018162 temporian-0.9.0/temporian/implementation/numpy_cc/__init__.py
+-rw-r--r--   0        0        0     2368 2024-04-16 14:54:45.018262 temporian-0.9.0/temporian/implementation/numpy_cc/operators/BUILD
+-rw-r--r--   0        0        0      576 2024-04-16 14:54:45.018339 temporian-0.9.0/temporian/implementation/numpy_cc/operators/__init__.py
+-rw-r--r--   0        0        0     8633 2024-04-16 14:54:45.018430 temporian-0.9.0/temporian/implementation/numpy_cc/operators/add_index.cc
+-rw-r--r--   0        0        0      102 2024-04-16 14:54:45.018501 temporian-0.9.0/temporian/implementation/numpy_cc/operators/add_index.h
+-rw-r--r--   0        0        0     8100 2024-04-16 14:54:45.018588 temporian-0.9.0/temporian/implementation/numpy_cc/operators/calendar.cc
+-rw-r--r--   0        0        0      104 2024-04-16 14:54:45.018655 temporian-0.9.0/temporian/implementation/numpy_cc/operators/calendar.h
+-rw-r--r--   0        0        0      674 2024-04-16 14:54:45.018716 temporian-0.9.0/temporian/implementation/numpy_cc/operators/common.h
+-rw-r--r--   0        0        0     1197 2024-04-16 14:54:45.018767 temporian-0.9.0/temporian/implementation/numpy_cc/operators/filter_moving_count.cc
+-rw-r--r--   0        0        0      112 2024-04-16 14:54:45.018852 temporian-0.9.0/temporian/implementation/numpy_cc/operators/filter_moving_count.h
+-rw-r--r--   0        0        0     2996 2024-04-16 14:54:45.018934 temporian-0.9.0/temporian/implementation/numpy_cc/operators/join.cc
+-rw-r--r--   0        0        0       97 2024-04-16 14:54:45.019039 temporian-0.9.0/temporian/implementation/numpy_cc/operators/join.h
+-rw-r--r--   0        0        0      988 2024-04-16 14:54:45.019106 temporian-0.9.0/temporian/implementation/numpy_cc/operators/pyinit.cc
+-rw-r--r--   0        0        0     1615 2024-04-16 14:54:45.019176 temporian-0.9.0/temporian/implementation/numpy_cc/operators/resample.cc
+-rw-r--r--   0        0        0      105 2024-04-16 14:54:45.019252 temporian-0.9.0/temporian/implementation/numpy_cc/operators/resample.h
+-rw-r--r--   0        0        0     1671 2024-04-16 14:54:45.019295 temporian-0.9.0/temporian/implementation/numpy_cc/operators/since_last.cc
+-rw-r--r--   0        0        0      107 2024-04-16 14:54:45.019352 temporian-0.9.0/temporian/implementation/numpy_cc/operators/since_last.h
+-rw-r--r--   0        0        0     7207 2024-04-16 14:54:45.019431 temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar.cc
+-rw-r--r--   0        0        0      106 2024-04-16 14:54:45.019484 temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar.h
+-rw-r--r--   0        0        0     2280 2024-04-16 14:54:45.019568 temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar_utils.cc
+-rw-r--r--   0        0        0      542 2024-04-16 14:54:45.019631 temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar_utils.h
+-rw-r--r--   0        0        0     2396 2024-04-16 14:54:45.019702 temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar_utils_test.cc
+-rw-r--r--   0        0        0     1884 2024-04-16 14:54:45.019771 temporian-0.9.0/temporian/implementation/numpy_cc/operators/until_next.cc
+-rw-r--r--   0        0        0      103 2024-04-16 14:54:45.019826 temporian-0.9.0/temporian/implementation/numpy_cc/operators/until_next.h
+-rw-r--r--   0        0        0    29444 2024-04-16 14:54:45.019936 temporian-0.9.0/temporian/implementation/numpy_cc/operators/window.cc
+-rw-r--r--   0        0        0      103 2024-04-16 14:54:45.019987 temporian-0.9.0/temporian/implementation/numpy_cc/operators/window.h
+-rw-r--r--   0        0        0     2016 2024-04-16 14:54:45.020099 temporian-0.9.0/temporian/io/BUILD
+-rw-r--r--   0        0        0      897 2024-04-16 14:54:45.020164 temporian-0.9.0/temporian/io/__init__.py
+-rw-r--r--   0        0        0     3175 2024-04-16 14:54:45.020266 temporian-0.9.0/temporian/io/csv.py
+-rw-r--r--   0        0        0     3307 2024-04-16 14:54:45.020339 temporian-0.9.0/temporian/io/format.py
+-rw-r--r--   0        0        0     3218 2024-04-16 14:54:45.020411 temporian-0.9.0/temporian/io/numpy.py
+-rw-r--r--   0        0        0     6404 2024-04-16 14:54:45.020506 temporian-0.9.0/temporian/io/pandas.py
+-rw-r--r--   0        0        0     2647 2024-04-16 14:54:45.020593 temporian-0.9.0/temporian/io/parquet.py
+-rw-r--r--   0        0        0     7643 2024-04-16 14:54:45.020678 temporian-0.9.0/temporian/io/polars.py
+-rw-r--r--   0        0        0    10580 2024-04-16 14:54:45.020771 temporian-0.9.0/temporian/io/tensorflow.py
+-rw-r--r--   0        0        0     1998 2024-04-16 14:54:45.020855 temporian-0.9.0/temporian/io/test/BUILD
+-rw-r--r--   0        0        0     3141 2024-04-16 14:54:45.020924 temporian-0.9.0/temporian/io/test/numpy_test.py
+-rw-r--r--   0        0        0    18021 2024-04-16 14:54:45.021016 temporian-0.9.0/temporian/io/test/pandas_test.py
+-rw-r--r--   0        0        0     1457 2024-04-16 14:54:45.021090 temporian-0.9.0/temporian/io/test/parquet_test.py
+-rw-r--r--   0        0        0    16018 2024-04-16 14:54:45.021151 temporian-0.9.0/temporian/io/test/polars_test.py
+-rw-r--r--   0        0        0     7388 2024-04-16 14:54:45.021209 temporian-0.9.0/temporian/io/test/tensorflow_test.py
+-rw-r--r--   0        0        0      257 2024-04-16 14:54:45.021293 temporian-0.9.0/temporian/proto/BUILD
+-rw-r--r--   0        0        0      576 2024-04-16 14:54:45.021382 temporian-0.9.0/temporian/proto/__init__.py
+-rw-r--r--   0        0        0     5549 2024-04-16 14:54:45.021464 temporian-0.9.0/temporian/proto/core.proto
+-rw-r--r--   0        0        0     2097 2024-04-16 14:54:45.021623 temporian-0.9.0/temporian/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.021671 temporian-0.9.0/temporian/test/__init__.py
+-rw-r--r--   0        0        0     4349 2024-04-16 14:54:45.021809 temporian-0.9.0/temporian/test/api_beam_test.py
+-rw-r--r--   0        0        0     7466 2024-04-16 14:54:45.021863 temporian-0.9.0/temporian/test/api_test.py
+-rw-r--r--   0        0        0     3683 2024-04-16 14:54:45.021952 temporian-0.9.0/temporian/test/doc_test.py
+-rw-r--r--   0        0        0     1701 2024-04-16 14:54:45.022040 temporian-0.9.0/temporian/test/io_test.py
+-rw-r--r--   0        0        0      151 2024-04-16 14:54:45.022140 temporian-0.9.0/temporian/test/test_data/BUILD
+-rw-r--r--   0        0        0       78 2024-04-16 14:54:45.022237 temporian-0.9.0/temporian/test/test_data/io/input.csv
+-rw-r--r--   0        0        0      100 2024-04-16 14:54:45.022313 temporian-0.9.0/temporian/test/test_data/prototype/left_event.csv
+-rw-r--r--   0        0        0      124 2024-04-16 14:54:45.022381 temporian-0.9.0/temporian/test/test_data/prototype/output_event.csv
+-rw-r--r--   0        0        0       99 2024-04-16 14:54:45.022454 temporian-0.9.0/temporian/test/test_data/prototype/right_event.csv
+-rw-r--r--   0        0        0     4746 2024-04-16 14:54:45.022527 temporian-0.9.0/temporian/test/utils.py
+-rw-r--r--   0        0        0      843 2024-04-16 14:54:45.022609 temporian-0.9.0/temporian/utils/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.022633 temporian-0.9.0/temporian/utils/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-16 14:54:45.022726 temporian-0.9.0/temporian/utils/compile.bzl
+-rw-r--r--   0        0        0     3433 2024-04-16 14:54:45.022803 temporian-0.9.0/temporian/utils/config.py
+-rw-r--r--   0        0        0      678 2024-04-16 14:54:45.022880 temporian-0.9.0/temporian/utils/golden.py
+-rw-r--r--   0        0        0      587 2024-04-16 14:54:45.022941 temporian-0.9.0/temporian/utils/string.py
+-rw-r--r--   0        0        0      737 2024-04-16 14:54:45.023047 temporian-0.9.0/temporian/utils/test/BUILD
+-rw-r--r--   0        0        0        0 2024-04-16 14:54:45.023072 temporian-0.9.0/temporian/utils/test/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-16 14:54:45.023131 temporian-0.9.0/temporian/utils/test/string_test.py
+-rw-r--r--   0        0        0     6279 2024-04-16 14:54:45.023211 temporian-0.9.0/temporian/utils/test/typecheck_test.py
+-rw-r--r--   0        0        0    11569 2024-04-16 14:54:45.023311 temporian-0.9.0/temporian/utils/typecheck.py
+-rw-r--r--   0        0        0     8937 1970-01-01 00:00:00.000000 temporian-0.9.0/setup.py
+-rw-r--r--   0        0        0     7996 1970-01-01 00:00:00.000000 temporian-0.9.0/PKG-INFO
```

### Comparing `temporian-0.8.1/LICENSE` & `temporian-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/README.md` & `temporian-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/config/build.py` & `temporian-0.9.0/config/build.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/pyproject.toml` & `temporian-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "temporian"
-version = "0.8.1"
+version = "0.9.0"
 description = "Temporian is a Python package for feature engineering of temporal data, focusing on preventing common modeling errors and providing a simple and powerful API, a first-class iterative development experience, and efficient and well-tested implementations of common and not-so-common temporal data preprocessing functions."
 authors = [
     "Mathieu Guillame-Bert, Braulio Ríos, Guillermo Etchebarne, Ian Spektor, Richard Stotz <gbm@google.com>",
 ]
 maintainers = ["Mathieu Guillame-Bert <gbm@google.com>"]
 repository = "https://github.com/google/temporian"
 classifiers = [
@@ -37,15 +37,16 @@
 absl-py = "^1.3.0"
 protobuf = ">=3.20.3"
 pandas = ">=1.5.2"
 matplotlib = "^3.7.1"
 
 # Extras (keep versions in sync with dev deps)
 apache-beam = { version = "^2.48.0", optional = true }
-tensorflow = { version = "^2.12.0", optional = true }
+tensorflow = {version = ">=2.12.0,<2.16", optional = true}
+polars = { version = "^0.20.15", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
 toml = "^0.10.2"
 pylint = "^2.14.0"
 memory-profiler = "^0.61.0"
@@ -63,23 +64,27 @@
 bokeh = "^3.1.0"
 ipykernel = "^6.22.0"
 jupyterlab = "^4.0.0"
 apache-beam = "^2.48.0"
 pillow = ">=9.5,<11.0"
 cairosvg = "^2.7.0"
 colorama = "^0.4.6"
-tensorflow = "^2.12.0"
+tensorflow = ">=2.13.0,<2.16"
+# limit this package because versions after 0.35 fail on python 3.8
+tensorflow-io-gcs-filesystem = ">=0.33.0,<0.35"
 selenium = "^4.11.2"
 coverage = "^7.3.1"
 mdx-truly-sane-lists = "^1.3"
+polars = "^0.20.15"
 
 [tool.poetry.extras]
 beam = ["apache-beam"]
-tensorflow = ["tensorflow"]
-all = ["apache-beam", "tensorflow"]
+tensorflow = ["tensorflow", "tensorflow-io-gcs-filesystem"]
+polars = ["polars"]
+all = ["apache-beam", "tensorflow", "polars"]
 
 [tool.black]
 line-length = 80
 preview = true
 
 [tool.pylint]
 max-line-length = 80
```

### Comparing `temporian-0.8.1/temporian/BUILD` & `temporian-0.9.0/temporian/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         "//temporian/core/operators:operators_without_implementation",
         "//temporian/implementation/numpy/data:event_set",
         "//temporian/implementation/numpy/data:io",
         "//temporian/implementation/numpy/data:plotter",
         "//temporian/implementation/numpy/operators",
         "//temporian/io:csv",
         "//temporian/io:pandas",
+        "//temporian/io:polars",
         "//temporian/io:numpy",
         "//temporian/io:parquet",
         "//temporian/io:tensorflow",
         "//temporian/utils:config",
         "//temporian/utils:typecheck",
     ],
 )
```

### Comparing `temporian-0.8.1/temporian/__init__.py` & `temporian-0.9.0/temporian/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 """Temporian."""
 
 # NOTE: If you need to import something here that isn't part of the public API,
 # import it with a private name (and delete the symbol if possible):
 # from temporian.module import submodule as _submodule
 # del _submodule
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 # Register all operator implementations
 from temporian.implementation.numpy import operators as _impls
 
 del _impls
 
 
 # ================== #
 # PUBLIC API SYMBOLS #
 # ================== #
 
 # EventSetNodes
 from temporian.core.data.node import EventSetNode
-from temporian.core.data.node import input_node
+from temporian.core.data.node import input_node, input_node_from_schema
 
 # Dtypes
 from temporian.core.data.dtype import float64
 from temporian.core.data.dtype import float32
 from temporian.core.data.dtype import int32
 from temporian.core.data.dtype import int64
 from temporian.core.data.dtype import bool_
@@ -54,15 +54,15 @@
 from temporian.core.data.schema import Schema, FeatureSchema, IndexSchema
 
 # Durations
 from temporian.api import duration
 
 # EventSets
 from temporian.implementation.numpy.data.event_set import EventSet, IndexData
-from temporian.implementation.numpy.data.io import event_set
+from temporian.implementation.numpy.data.io import event_set, from_struct
 
 # Serialization
 from temporian.core.serialization import save
 from temporian.core.serialization import load
 from temporian.core.serialization import save_graph
 from temporian.core.serialization import load_graph
 
@@ -74,14 +74,16 @@
 from temporian.io.csv import to_csv
 from temporian.io.csv import from_csv
 from temporian.io.pandas import to_pandas
 from temporian.io.numpy import to_numpy
 from temporian.io.pandas import from_pandas
 from temporian.io.parquet import from_parquet
 from temporian.io.parquet import to_parquet
+from temporian.io.polars import to_polars
+from temporian.io.polars import from_polars
 from temporian.io.tensorflow import to_tensorflow_dataset
 from temporian.io.tensorflow import from_tensorflow_record
 from temporian.io.tensorflow import to_tensorflow_record
 
 # Plotting
 from temporian.implementation.numpy.data.plotter import plot
```

### Comparing `temporian-0.8.1/temporian/beam/BUILD` & `temporian-0.9.0/temporian/beam/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/__init__.py` & `temporian-0.9.0/temporian/beam/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/evaluation.py` & `temporian-0.9.0/temporian/beam/evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,14 +133,22 @@
 
     schedule = build_schedule(
         inputs=set(inputs.keys()), outputs=set(outputs), verbose=verbose
     )
 
     data = {**inputs}
 
+    # Check that operators implementations are available
+    needed_operators = set()
+    for step in schedule.steps:
+        needed_operators.add(step.op.definition.key)
+    implementation_lib.check_operators_implementations_are_available(
+        needed_operators
+    )
+
     num_steps = len(schedule.steps)
     for step_idx, step in enumerate(schedule.steps):
         operator_def = step.op.definition
 
         if verbose > 0:
             print("=============================", file=sys.stderr)
             print(
```

### Comparing `temporian-0.8.1/temporian/beam/implementation_lib.py` & `temporian-0.9.0/temporian/beam/implementation_lib.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Registering mechanism for operator implementation classes."""
 
-from typing import Any, Dict
+from typing import Any, Dict, Set
 
 _OPERATOR_IMPLEMENTATIONS = {}
 
 # TODO: Create a "registration" module to handle in-process and beam operator
 # registration.
 
 
+def check_operators_implementations_are_available(needed: Set[str]):
+    """Checks if operator implementations are available."""
+    missing = set(needed) - set(_OPERATOR_IMPLEMENTATIONS.keys())
+    if missing:
+        raise ValueError(
+            f"Unknown operator implementations '{missing}' for Beam backend. It"
+            " seems this operator is only available for the in-process"
+            " Temporian backend. Available Beam operator implementations are:"
+            f" {list(_OPERATOR_IMPLEMENTATIONS.keys())}."
+        )
+
+
 def register_operator_implementation(
     operator_class, operator_implementation_class
 ):
     """Registers an operator implementation."""
     op_key = operator_class.operator_key()
     if op_key in _OPERATOR_IMPLEMENTATIONS:
         raise ValueError("Operator implementation already registered")
```

### Comparing `temporian-0.8.1/temporian/beam/io/BUILD` & `temporian-0.9.0/temporian/beam/io/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/csv.py` & `temporian-0.9.0/temporian/beam/io/csv.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/dict.py` & `temporian-0.9.0/temporian/beam/io/dict.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/np_array_coder.py` & `temporian-0.9.0/temporian/beam/io/np_array_coder.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/tensorflow.py` & `temporian-0.9.0/temporian/beam/io/tensorflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,35 +89,30 @@
         f(ex, self._timestamp_key).float_list.value[:] = dict_example[
             self._timestamp_key
         ]
 
         # Features
         for feature_schema in self._schema.features:
             src_value = dict_example[feature_schema.name]
+
             if feature_schema.dtype in [
                 DType.BOOLEAN,
                 DType.INT32,
                 DType.INT64,
             ]:
-                f(ex, feature_schema.name).int64_list.value[
-                    :
-                ] = src_value = dict_example[feature_schema.name]
+                f(ex, feature_schema.name).int64_list.value[:] = src_value
 
             elif feature_schema.dtype in [
                 DType.FLOAT32,
                 DType.FLOAT64,
             ]:
-                f(ex, feature_schema.name).float_list.value[
-                    :
-                ] = src_value = dict_example[feature_schema.name]
+                f(ex, feature_schema.name).float_list.value[:] = src_value
 
             elif feature_schema.dtype == DType.STRING:
-                f(ex, feature_schema.name).bytes_list.value[
-                    :
-                ] = src_value = dict_example[feature_schema.name]
+                f(ex, feature_schema.name).bytes_list.value[:] = src_value
 
             else:
                 raise ValueError("Non supported feature dtype")
 
         # Indexes
         for index_schema in self._schema.indexes:
             src_value = dict_example[index_schema.name]
```

### Comparing `temporian-0.8.1/temporian/beam/io/test/BUILD` & `temporian-0.9.0/temporian/beam/io/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/test/csv_test.py` & `temporian-0.9.0/temporian/beam/io/test/csv_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/test/dict_test.py` & `temporian-0.9.0/temporian/beam/io/test/dict_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/test/np_array_coder_test.py` & `temporian-0.9.0/temporian/beam/io/test/np_array_coder_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/io/test/tensorflow_test.py` & `temporian-0.9.0/temporian/beam/io/test/tensorflow_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/BUILD` & `temporian-0.9.0/temporian/core/BUILD`

 * *Files 17% similar despite different names*

```diff
@@ -3,85 +3,120 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "base",
-    srcs = ["base.py"],
+    name = "evaluation",
+    srcs = ["evaluation.py"],
     srcs_version = "PY3",
     deps = [
-        # already_there/apache_beam
+        ":graph",
+        ":schedule",
+        ":typing",
+        "//temporian/core/data:node",
         "//temporian/core/operators:base",
-        "//temporian/beam:typing",
+        "//temporian/core/operators:leak",
+        "//temporian/implementation/numpy:evaluation",
+        "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
-    name = "operators",
-    srcs = ["__init__.py"],
+    name = "operator_lib",
+    srcs = ["operator_lib.py"],
     srcs_version = "PY3",
     deps = [
-        ":add_index",
-        ":select",
-        ":rename",
-        ":prefix",
-        "//temporian/beam/operators/window:moving_count",
-        "//temporian/beam/operators/window:moving_max",
-        "//temporian/beam/operators/window:moving_min",
-        "//temporian/beam/operators/window:moving_standard_deviation",
-        "//temporian/beam/operators/window:moving_sum",
-        "//temporian/beam/operators/window:simple_moving_average",
+        "//temporian/core/operators:base",
+    ],
+)
+
+py_library(
+    name = "schedule",
+    srcs = ["schedule.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//temporian/core/data:node",
+        "//temporian/core/operators:base",
+    ],
+)
+
+py_library(
+    name = "graph",
+    srcs = ["graph.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//temporian/core/data:node",
+        "//temporian/core/operators:base",
     ],
 )
 
 py_library(
-    name = "select",
-    srcs = ["select.py"],
+    name = "serialization",
+    srcs = ["serialization.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/beam:implementation_lib",
-        "//temporian/beam:typing",
-        "//temporian/beam/operators:base",
-        "//temporian/core/operators:select",
+        ":typing",
+        "//temporian/core:compilation",
+        "//temporian/core:graph",
+        "//temporian/core:operator_lib",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:node",
+        "//temporian/core/data:schema",
+        "//temporian/core/operators:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/proto:core_py_proto",
     ],
 )
 
 py_library(
-    name = "add_index",
-    srcs = ["add_index.py"],
+    name = "compilation",
+    srcs = ["compilation.py"],
     srcs_version = "PY3",
     deps = [
-        # already_there/apache_beam
-        # already_there/numpy
-        "//temporian/beam:typing",
-        "//temporian/beam:implementation_lib",
-        "//temporian/beam/operators:base",
-        "//temporian/core/operators:add_index",
+        "//temporian/core/data:node",
+        "//temporian/implementation/numpy/data:event_set",
     ],
 )
 
 py_library(
-    name = "rename",
-    srcs = ["rename.py"],
+    name = "event_set_ops",
+    srcs = ["event_set_ops.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/beam:implementation_lib",
-        "//temporian/beam:typing",
-        "//temporian/beam/operators:base",
-        "//temporian/core/operators:rename",
+        "//temporian/core/data:duration",
     ],
 )
 
+py_library(
+    name = "typing",
+    srcs = ["typing.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//temporian/core:event_set_ops",
+        "//temporian/core/data:dtype",
+        "//temporian/core/data:duration",
+        "//temporian/core/data:node",
+        "//temporian/implementation/numpy/data:event_set",
+    ],
+)
+
+py_library(
+    name = "dataclasses",
+    srcs = ["dataclasses.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//temporian/core:typing",
+    ]
+)
 
 py_library(
-    name = "prefix",
-    srcs = ["prefix.py"],
+    name = "types",
+    srcs = ["types.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/beam:implementation_lib",
-        "//temporian/beam:typing",
-        "//temporian/beam/operators:base",
-        "//temporian/core/operators:prefix",
+        ":dataclasses",
+        ":typing",
+        "//temporian/core/operators:map",
     ],
 )
```

### Comparing `temporian-0.8.1/temporian/beam/operators/__init__.py` & `temporian-0.9.0/temporian/core/operators/window/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Imports all the packages containing operator implementations."""
+"""Window operators."""
 
 # pylint: disable=unused-import
 # pylint: disable=line-too-long
 # fmt: off
-from temporian.beam.operators.window import moving_count
-from temporian.beam.operators.window import moving_max
-from temporian.beam.operators.window import moving_min
-from temporian.beam.operators.window import moving_standard_deviation
-from temporian.beam.operators.window import moving_sum
-from temporian.beam.operators.window import simple_moving_average
-from temporian.beam.operators import select
-from temporian.beam.operators import add_index
-from temporian.beam.operators import rename
-from temporian.beam.operators import prefix
+
+from temporian.core.operators.window.simple_moving_average import simple_moving_average
+from temporian.core.operators.window.moving_standard_deviation import moving_standard_deviation
+from temporian.core.operators.window.moving_sum import cumsum
+from temporian.core.operators.window.moving_sum import moving_sum
+from temporian.core.operators.window.moving_count import moving_count
+from temporian.core.operators.window.moving_min import moving_min
+from temporian.core.operators.window.moving_max import moving_max
+from temporian.core.operators.window.moving_product import cumprod
+from temporian.core.operators.window.moving_product import moving_product
```

### Comparing `temporian-0.8.1/temporian/beam/operators/add_index.py` & `temporian-0.9.0/temporian/beam/operators/add_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/base.py` & `temporian-0.9.0/temporian/beam/operators/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,25 +42,40 @@
 
     def __call__(self, **inputs: BeamEventSet) -> Dict[str, BeamEventSet]:
         outputs = self.call(**inputs)
         return outputs
 
 
 def beam_eventset_map(
-    src: BeamEventSet, name: str, fn: Callable[[FeatureItem, int], FeatureItem]
+    src: BeamEventSet,
+    name: str,
+    fn: Callable[[FeatureItem, int], Iterable[FeatureItem]],
 ) -> BeamEventSet:
     """Applies a function on each feature of a Beam eventset."""
 
     def apply(idx, item):
         return item | f"Map on feature #{idx} {name}" >> beam.Map(fn, idx)
 
     return tuple([apply(idx, item) for idx, item in enumerate(src)])
 
 
-def _extract_from_iterable(
+def beam_eventset_flatmap(
+    src: BeamEventSet,
+    name: str,
+    fn: Callable[[FeatureItem, int], Iterable[FeatureItem]],
+) -> BeamEventSet:
+    """Applies a function on each feature of a Beam eventset."""
+
+    def apply(idx, item):
+        return item | f"Map on feature #{idx} {name}" >> beam.FlatMap(fn, idx)
+
+    return tuple([apply(idx, item) for idx, item in enumerate(src)])
+
+
+def extract_from_iterable(
     src: Iterable[FeatureItemValue],
 ) -> Optional[FeatureItemValue]:
     for x in src:
         return x
     return None
 
 
@@ -81,16 +96,16 @@
         item: Tuple[
             BeamIndexKey,
             Tuple[Iterable[FeatureItemValue], Iterable[FeatureItemValue]],
         ],
         idx: int,
     ) -> Iterator[FeatureItem]:
         index, (it_feature, it_sampling) = item
-        feature = _extract_from_iterable(it_feature)
-        sampling = _extract_from_iterable(it_sampling)
+        feature = extract_from_iterable(it_feature)
+        sampling = extract_from_iterable(it_sampling)
         if sampling is not None:
             yield fn(index, feature, sampling, idx)
 
     def apply(idx, item):
         return (
             (item, sampling[0])
             | f"Join feature and sampling on feature #{idx} {name}"
```

### Comparing `temporian-0.8.1/temporian/beam/operators/prefix.py` & `temporian-0.9.0/temporian/beam/operators/prefix.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/rename.py` & `temporian-0.9.0/temporian/beam/operators/rename.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/select.py` & `temporian-0.9.0/temporian/beam/operators/select.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/test/BUILD` & `temporian-0.9.0/temporian/io/test/BUILD`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,79 @@
 package(
     default_visibility = ["//visibility:public"],
     licenses = ["notice"],
 )
 
+# Tests
+# =====
 py_test(
-    name = "select_test",
-    srcs = ["select_test.py"],
+    name = "pandas_test",
+    srcs = ["pandas_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
+        # already_there/numpy
         # already_there/absl/testing:parameterized
-        # already_there/google/protobuf:use_fast_cpp_protos
+        # already_there/pandas
+        "//temporian/test:utils",
         "//temporian/implementation/numpy/data:io",
-        "//temporian/beam/test:utils",
-        "//temporian/core/operators:select",
+        "//temporian/io:pandas",
     ],
 )
 
 py_test(
-    name = "add_index_test",
-    srcs = ["add_index_test.py"],
+    name = "polars_test",
+    srcs = ["polars_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
+        # already_there/numpy
         # already_there/absl/testing:parameterized
-        # already_there/google/protobuf:use_fast_cpp_protos
+        # already_there/polars
+        "//temporian/test:utils",
         "//temporian/implementation/numpy/data:io",
-        "//temporian/beam/test:utils",
-        "//temporian/core/operators:add_index",
+        "//temporian/io:polars",
     ],
 )
 
 py_test(
-    name = "rename_test",
-    srcs = ["rename_test.py"],
+    name = "numpy_test",
+    srcs = ["numpy_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
+        # already_there/numpy
         # already_there/absl/testing:parameterized
-        # already_there/google/protobuf:use_fast_cpp_protos
+        "//temporian/test:utils",
         "//temporian/implementation/numpy/data:io",
-        "//temporian/beam/test:utils",
-        "//temporian/core/operators:rename",
+        "//temporian/io:numpy",
     ],
 )
 
-
 py_test(
-    name = "prefix_test",
-    srcs = ["prefix_test.py"],
+    name = "tensorflow_test",
+    srcs = ["tensorflow_test.py"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/absl/testing:parameterized
-        # already_there/google/protobuf:use_fast_cpp_protos
+        # already_there/numpy
+        # already_there/tensorflow
+        "//temporian/test:utils",
         "//temporian/implementation/numpy/data:io",
-        "//temporian/beam/test:utils",
-        "//temporian/core/operators:prefix",
+        "//temporian/io:tensorflow",
     ],
 )
+
+py_test(
+    name = "parquet_test",
+    srcs = ["parquet_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        # already_there/numpy
+        # already_there/pyarrow
+        "//temporian/test:utils",
+        "//temporian/implementation/numpy/data:io",
+        "//temporian/io:parquet",
+    ],
+)
```

### Comparing `temporian-0.8.1/temporian/beam/operators/test/add_index_test.py` & `temporian-0.9.0/temporian/beam/operators/test/add_index_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/test/prefix_test.py` & `temporian-0.9.0/temporian/beam/operators/test/prefix_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/test/rename_test.py` & `temporian-0.9.0/temporian/beam/operators/test/rename_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/test/select_test.py` & `temporian-0.9.0/temporian/beam/operators/test/select_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/BUILD` & `temporian-0.9.0/temporian/beam/operators/window/BUILD`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # =========
 
 py_library(
     name = "base",
     srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-
         "//temporian/beam:typing",
         "//temporian/beam/operators:base",
         "//temporian/core/operators/window:base",
         "//temporian/implementation/numpy/operators/window:base",
     ],
 )
```

### Comparing `temporian-0.8.1/temporian/beam/operators/window/base.py` & `temporian-0.9.0/temporian/beam/operators/window/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/moving_count.py` & `temporian-0.9.0/temporian/beam/operators/window/moving_count.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/moving_max.py` & `temporian-0.9.0/temporian/beam/operators/window/moving_max.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/moving_min.py` & `temporian-0.9.0/temporian/beam/operators/window/moving_min.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/moving_standard_deviation.py` & `temporian-0.9.0/temporian/beam/operators/window/moving_standard_deviation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/moving_sum.py` & `temporian-0.9.0/temporian/beam/operators/window/moving_sum.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/simple_moving_average.py` & `temporian-0.9.0/temporian/beam/operators/window/simple_moving_average.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/operators/window/test/window_test.py` & `temporian-0.9.0/temporian/beam/operators/window/test/window_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/test/BUILD` & `temporian-0.9.0/temporian/beam/test/BUILD`

 * *Files 9% similar despite different names*

```diff
@@ -31,13 +31,15 @@
     deps = [
         "//temporian/core/data:dtype",
         # already_there/absl/testing:absltest
         # already_there/absl/testing:parameterized
         # already_there/apache_beam
         "//temporian/test:utils",
         "//temporian/beam/io:csv",
+        "//temporian/beam/io:tensorflow",
         "//temporian/beam:evaluation",
         "//temporian/io:csv",
+        "//temporian/io:tensorflow",
         "//temporian/core/data:node",
         "//temporian/implementation/numpy/data:event_set",
     ],
 )
```

### Comparing `temporian-0.8.1/temporian/beam/test/evaluation_test.py` & `temporian-0.9.0/temporian/beam/test/evaluation_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/beam/test/utils.py` & `temporian-0.9.0/temporian/beam/test/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,23 @@
 from temporian.core.data.dtype import DType
 
 from temporian.test.utils import assertEqualEventSet
 from temporian.beam.io.csv import from_csv as beam_from_csv
 from temporian.beam.io.csv import to_csv as beam_to_csv
 from temporian.beam.evaluation import run_multi_io
 from temporian.io.csv import to_csv, from_csv
+from temporian.io.tensorflow import to_tensorflow_record, from_tensorflow_record
 from temporian.core.data.node import EventSetNode
 from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.beam.io.tensorflow import (
+    from_tensorflow_record as beam_from_tensorflow_record,
+)
+from temporian.beam.io.tensorflow import (
+    to_tensorflow_record as beam_to_tensorflow_record,
+)
 
 
 def check_beam_implementation(
     test: absltest.TestCase,
     input_data: Union[EventSet, List[EventSet]],
     output_node: EventSetNode,
     cast: Optional[DType] = None,
@@ -57,42 +64,42 @@
     output_path = os.path.join(tmp_dir, "output.csv")
     input_paths = []
 
     # Export input data to csv
     for input_idx, input_evset in enumerate(input_data):
         input_path = os.path.join(tmp_dir, f"input_{input_idx}.csv")
         input_paths.append(input_path)
-        to_csv(input_evset, path=input_path)
+        to_tensorflow_record(input_evset, path=input_path)
 
     # Run the Temporian program using the Beam backend
     with TestPipeline() as p:
         input_pcollection = {}
         for input_path, input_evset in zip(input_paths, input_data):
-            input_pcollection[input_evset.node()] = p | beam_from_csv(
+            input_pcollection[
+                input_evset.node()
+            ] = p | beam_from_tensorflow_record(
                 input_path, input_evset.node().schema
             )
 
         output_pcollection = run_multi_io(
             inputs=input_pcollection, outputs=[output_node]
         )
 
         assert len(output_pcollection) == 1
 
-        output = output_pcollection[output_node] | beam_to_csv(
+        output = output_pcollection[output_node] | beam_to_tensorflow_record(
             output_path, output_node.schema, shard_name_template=""
         )
 
         assert_that(
             output,
             equal_to([output_path]),
         )
 
-    beam_output = from_csv(
-        output_path, indexes=output_node.schema.index_names()
-    )
+    beam_output = from_tensorflow_record(output_path, output_node.schema)
 
     if cast:
         beam_output = beam_output.cast(cast)
 
     # Run the Temporian program using the numpy backend
     expected_output = output_node.run(input_data)
```

### Comparing `temporian-0.8.1/temporian/beam/typing.py` & `temporian-0.9.0/temporian/beam/typing.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/BUILD`

 * *Files 20% similar despite different names*

```diff
@@ -3,120 +3,119 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "evaluation",
-    srcs = ["evaluation.py"],
+    name = "calendar",
+    srcs = ["__init__.py"],
+    srcs_version = "PY3",
+)
+
+py_library(
+    name = "base",
+    srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        ":graph",
-        ":schedule",
-        ":typing",
-        "//temporian/core/data:node",
-        "//temporian/core/operators:base",
-        "//temporian/core/operators:leak",
-        "//temporian/implementation/numpy:evaluation",
-        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/core/operators/calendar:base",
     ],
 )
 
 py_library(
-    name = "operator_lib",
-    srcs = ["operator_lib.py"],
+    name = "day_of_month",
+    srcs = ["day_of_month.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/operators:base",
+        ":base",
+        "//temporian/core/operators/calendar:day_of_month",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "schedule",
-    srcs = ["schedule.py"],
+    name = "day_of_week",
+    srcs = ["day_of_week.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/core/operators:base",
+        ":base",
+        "//temporian/core/operators/calendar:day_of_week",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "graph",
-    srcs = ["graph.py"],
+    name = "day_of_year",
+    srcs = ["day_of_year.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/core/operators:base",
+        ":base",
+        "//temporian/core/operators/calendar:day_of_year",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "serialization",
-    srcs = ["serialization.py"],
+    name = "hour",
+    srcs = ["hour.py"],
     srcs_version = "PY3",
     deps = [
-        ":typing",
-        "//temporian/core:compilation",
-        "//temporian/core:graph",
-        "//temporian/core:operator_lib",
-        "//temporian/core/data:dtype",
-        "//temporian/core/data:node",
-        "//temporian/core/data:schema",
-        "//temporian/core/operators:base",
-        "//temporian/implementation/numpy/data:event_set",
-        "//temporian/proto:core_py_proto",
+        ":base",
+        "//temporian/core/operators/calendar:hour",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "compilation",
-    srcs = ["compilation.py"],
+    name = "iso_week",
+    srcs = ["iso_week.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:node",
-        "//temporian/implementation/numpy/data:event_set",
+        ":base",
+        "//temporian/core/operators/calendar:iso_week",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "event_set_ops",
-    srcs = ["event_set_ops.py"],
+    name = "minute",
+    srcs = ["minute.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/data:duration",
+        ":base",
+        "//temporian/core/operators/calendar:minute",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "typing",
-    srcs = ["typing.py"],
+    name = "month",
+    srcs = ["month.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core:event_set_ops",
-        "//temporian/core/data:dtype",
-        "//temporian/core/data:duration",
-        "//temporian/core/data:node",
-        "//temporian/implementation/numpy/data:event_set",
+        ":base",
+        "//temporian/core/operators/calendar:month",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
 
 py_library(
-    name = "dataclasses",
-    srcs = ["dataclasses.py"],
+    name = "second",
+    srcs = ["second.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core:typing",
-    ]
+        ":base",
+        "//temporian/core/operators/calendar:second",
+        "//temporian/implementation/numpy:implementation_lib",
+    ],
 )
 
 py_library(
-    name = "types",
-    srcs = ["types.py"],
+    name = "year",
+    srcs = ["year.py"],
     srcs_version = "PY3",
     deps = [
-        ":dataclasses",
-        ":typing",
-        "//temporian/core/operators:map",
+        ":base",
+        "//temporian/core/operators/calendar:year",
+        "//temporian/implementation/numpy:implementation_lib",
     ],
 )
```

### Comparing `temporian-0.8.1/temporian/core/__init__.py` & `temporian-0.9.0/temporian/core/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/compilation.py` & `temporian-0.9.0/temporian/core/compilation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/BUILD` & `temporian-0.9.0/temporian/core/data/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/__init__.py` & `temporian-0.9.0/temporian/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/dtype.py` & `temporian-0.9.0/temporian/core/data/dtype.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/duration.py` & `temporian-0.9.0/temporian/core/data/duration.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/duration_utils.py` & `temporian-0.9.0/temporian/core/data/duration_utils.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/node.py` & `temporian-0.9.0/temporian/core/data/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -172,16 +172,18 @@
             f"name: {self._name}\n"
             f"creator: {self._creator}\n"
             f"id:{id(self)}\n"
         )
 
 
 def input_node(
-    features: List[Tuple[str, DType]],
-    indexes: Optional[List[Tuple[str, IndexDType]]] = None,
+    features: Union[List[FeatureSchema], List[Tuple[str, DType]]],
+    indexes: Optional[
+        Union[List[IndexSchema], List[Tuple[str, IndexDType]]]
+    ] = None,
     is_unix_timestamp: bool = False,
     same_sampling_as: Optional[EventSetNode] = None,
     name: Optional[str] = None,
 ) -> EventSetNode:
     """Creates an input [`EventSetNode`][temporian.EventSetNode].
 
     An input EventSetNode can be used to feed data into a graph.
@@ -241,14 +243,51 @@
             indexes=indexes,
             is_unix_timestamp=is_unix_timestamp,
             name=name,
             creator=None,
         )
 
 
+def input_node_from_schema(
+    schema: Schema,
+    same_sampling_as: Optional[EventSetNode] = None,
+    name: Optional[str] = None,
+) -> EventSetNode:
+    """Creates an input [`EventSetNode`][temporian.EventSetNode] from a schema.
+
+    Usage example:
+
+        ```python
+        >>> # Create two nodes with the same schema.
+        >>> a = tp.input_node(features=[("f1", tp.float64), ("f2", tp.str_)])
+        >>> b = tp.input_node_from_schema(a.schema)
+
+        ```
+
+    Args:
+        schema: Schema of the node.
+        same_sampling_as: If set, the created EventSetNode is guaranteed to have the
+            same sampling as same_sampling_as`. In this case, `indexes` and
+            `is_unix_timestamp` should not be provided. Some operators require
+            for input EventSetNodes to have the same sampling.
+        name: Name for the EventSetNode.
+
+    Returns:
+        EventSetNode with the given specifications.
+    """
+
+    return input_node(
+        features=schema.features,
+        indexes=schema.indexes,
+        is_unix_timestamp=schema.is_unix_timestamp,
+        same_sampling_as=same_sampling_as,
+        name=name,
+    )
+
+
 @dataclass
 class Sampling:
     """A sampling is a reference to the way data is sampled."""
 
     creator: Optional[Operator] = None
 
     def __hash__(self):
```

### Comparing `temporian-0.8.1/temporian/core/data/schema.py` & `temporian-0.9.0/temporian/core/operators/add_index.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,142 +8,158 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Schema and related classes."""
+"""Add and set index operators classes and public API function definitions."""
 
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import List, Tuple, Dict, Union
+from typing import List, Union
 
-from temporian.core.data.dtype import DType, IndexDType
+from temporian.core import operator_lib
+from temporian.core.compilation import compile
+from temporian.core.data.node import (
+    EventSetNode,
+    create_node_new_features_new_sampling,
+)
+from temporian.core.data.schema import FeatureSchema, IndexSchema
+from temporian.core.operators.base import Operator
+from temporian.core.typing import EventSetOrNode
+from temporian.proto import core_pb2 as pb
+from temporian.core.operators.drop_index import drop_index
 
 
-@dataclass(frozen=True)
-class FeatureSchema:
-    name: str
-    dtype: DType
-
-    def __repr__(self) -> str:
-        return f"({self.name!r}, {self.dtype})"
-
+class AddIndexOperator(Operator):
+    def __init__(
+        self,
+        input: EventSetNode,
+        indexes: List[str],
+    ) -> None:
+        super().__init__()
 
-@dataclass(frozen=True)
-class IndexSchema:
-    name: str
-    dtype: IndexDType
+        output_feature_schemas = self._get_output_feature_schemas(
+            input, indexes
+        )
+        output_indexes = self._get_output_indexes(input, indexes)
+        self._indexes = indexes
 
-    def __repr__(self) -> str:
-        return f"({self.name!r}, {self.dtype})"
+        self.add_input("input", input)
 
+        self.add_attribute("indexes", indexes)
 
-class Schema:
-    """A schema defines the type of data in an
-    [`EventSetNode`][temporian.EventSetNode] or
-    [`EventSet`][temporian.EventSet].
+        self.add_output(
+            "output",
+            create_node_new_features_new_sampling(
+                features=output_feature_schemas,
+                indexes=output_indexes,
+                is_unix_timestamp=input.schema.is_unix_timestamp,
+                creator=self,
+            ),
+        )
+        self.check()
 
-    A schema does not contain any actual data.
+    def _get_output_feature_schemas(
+        self, input: EventSetNode, indexes: List[str]
+    ) -> List[FeatureSchema]:
+        return [
+            feature
+            for feature in input.schema.features
+            if feature.name not in indexes
+        ]
+
+    def _get_output_indexes(
+        self, input: EventSetNode, indexes: List[str]
+    ) -> List[IndexSchema]:
+        index_dict = input.schema.index_name_to_dtype()
+        feature_dict = input.schema.feature_name_to_dtype()
+
+        new_indexes: List[IndexSchema] = []
+        for index in indexes:
+            if index in index_dict:
+                raise ValueError(f"{index} is already an index in input.")
 
-    A schema can be shared by multiple EventSetNodes.
+            if index not in feature_dict:
+                raise ValueError(f"{index} is not a feature in input.")
 
-    Attributes:
-        features: List of feature names and types.
-        indexes: List of index names and types.
-        is_unix_timestamp: Whether values correspond to Unix timestamps.
-    """
+            new_indexes.append(
+                IndexSchema(name=index, dtype=feature_dict[index])
+            )
+        # Note: The new indexes are added after the existing ones.
+        return input.schema.indexes + new_indexes
 
-    def __init__(
-        self,
-        features: Union[List[FeatureSchema], List[Tuple[str, DType]]],
-        indexes: Union[List[IndexSchema], List[Tuple[str, IndexDType]]] = [],
-        is_unix_timestamp: bool = False,
-    ):
-        self._features = list(map(_normalize_feature, features))
-        self._indexes = list(map(_normalize_index, indexes))
-        self._is_unix_timestamp = is_unix_timestamp
-
-    def __eq__(self, other):
-        if not isinstance(other, Schema):
-            return False
-        return (
-            self._features == other._features
-            and self._indexes == other._indexes
-            and self._is_unix_timestamp == other._is_unix_timestamp
+    @classmethod
+    def build_op_definition(cls) -> pb.OperatorDef:
+        return pb.OperatorDef(
+            key="ADD_INDEX",
+            attributes=[
+                pb.OperatorDef.Attribute(
+                    key="indexes",
+                    type=pb.OperatorDef.Attribute.Type.LIST_STRING,
+                ),
+            ],
+            inputs=[pb.OperatorDef.Input(key="input")],
+            outputs=[pb.OperatorDef.Output(key="output")],
         )
 
     @property
-    def features(self) -> List[FeatureSchema]:
-        return self._features
-
-    @property
-    def indexes(self) -> List[IndexSchema]:
+    def indexes(self) -> List[str]:
         return self._indexes
 
-    @property
-    def is_unix_timestamp(self) -> bool:
-        return self._is_unix_timestamp
 
-    @is_unix_timestamp.setter
-    def is_unix_timestamp(self, value):
-        self._is_unix_timestamp = value
+operator_lib.register_operator(AddIndexOperator)
 
-    def feature_names(self) -> List[str]:
-        return [feature.name for feature in self._features]
 
-    def index_names(self) -> List[str]:
-        return [index.name for index in self._indexes]
+def _normalize_indexes(
+    indexes: Union[str, List[str]],
+) -> List[str]:
+    if isinstance(indexes, str):
+        return [indexes]
 
-    def feature_dtypes(self) -> List[DType]:
-        return [feature.dtype for feature in self._features]
+    if len(indexes) == 0:
+        raise ValueError("Cannot specify empty list as `indexes` argument.")
 
-    def index_dtypes(self) -> List[IndexDType]:
-        return [index.dtype for index in self._indexes]
+    return indexes
 
-    def feature_name_to_dtype(self) -> Dict[str, DType]:
-        return {feature.name: feature.dtype for feature in self._features}
 
-    def index_name_to_dtype(self) -> Dict[str, IndexDType]:
-        return {index.name: index.dtype for index in self._indexes}
+def _normalize_indexes_to_set(
+    indexes: Union[str, List[str]],
+) -> List[str]:
+    if isinstance(indexes, str):
+        return [indexes]
 
-    def __repr__(self) -> str:
-        r = (
-            f"features: {self._features}\n"
-            f"indexes: {self._indexes}\n"
-            f"is_unix_timestamp: {self._is_unix_timestamp}\n"
-        )
-        return r
+    if len(indexes) == 0:
+        raise ValueError("Cannot specify empty list as `indexes` argument.")
 
-    def check_compatible_index(self, other: Schema):
-        if self.indexes != other.indexes:
-            raise ValueError(
-                f"Arguments don't have the same index. {self.indexes} !="
-                f" {other.indexes}"
-            )
+    return indexes
 
-    def check_compatible_features(self, other: Schema, check_order: bool):
-        if set(self.features) != set(other.features):
-            raise ValueError(
-                "Some features are different between inputs: "
-                f"{set(self.features) ^ set(other.features)}."
-            )
-        if check_order and (self.features != other.features):
-            raise ValueError(
-                "Features should be in the same order, but got:"
-                f"{self.feature_names} and {other.feature_names}."
-            )
 
+@compile
+def add_index(
+    input: EventSetOrNode, indexes: Union[str, List[str]]
+) -> EventSetOrNode:
+    assert isinstance(input, EventSetNode)
+
+    indexes = _normalize_indexes(indexes)
+    return AddIndexOperator(input, indexes).outputs["output"]
+
+
+@compile
+def set_index(
+    input: EventSetOrNode, indexes: Union[str, List[str]]
+) -> EventSetOrNode:
+    assert isinstance(input, EventSetNode)
+
+    indexes = _normalize_indexes_to_set(indexes)
+
+    # Note
+    # The set_index is implemented as a drop_index + add_index.
+    # The implementation could be improved (simpler, faster) with a new
+    # operator to re-order the indexes.
 
-def _normalize_feature(x):
-    if isinstance(x, FeatureSchema):
-        return x
-    assert len(x) == 2
-    return FeatureSchema(x[0], x[1])
+    if len(input.schema.indexes) != 0:
+        input = drop_index(input)
 
+    if len(indexes) != 0:
+        input = add_index(input, indexes)
 
-def _normalize_index(x):
-    if isinstance(x, IndexSchema):
-        return x
-    assert len(x) == 2
-    return IndexSchema(x[0], x[1])
+    return input
```

### Comparing `temporian-0.8.1/temporian/core/data/test/BUILD` & `temporian-0.9.0/temporian/core/data/test/BUILD`

 * *Files 12% similar despite different names*

```diff
@@ -23,7 +23,20 @@
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
         # already_there/absl/testing:parameterized
         "//temporian/core/data:dtype",
     ],
 )
+
+
+py_test(
+    name = "schema_test",
+    srcs = ["schema_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/absl/testing:absltest
+        # already_there/absl/testing:parameterized
+        "//temporian/core/data:schema",
+        "//temporian/core:serialization",
+    ],
+)
```

### Comparing `temporian-0.8.1/temporian/core/data/test/test_dtype.py` & `temporian-0.9.0/temporian/core/data/test/test_dtype.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/data/test/test_node.py` & `temporian-0.9.0/temporian/core/data/test/test_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,24 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from absl.testing import absltest
 
 from temporian.core.test import utils
 from temporian.implementation.numpy.data.event_set import EventSet
+from temporian.core.data.node import (
+    input_node_from_schema,
+)
 
 
 class EventSetNodeTest(absltest.TestCase):
     def test_run_input(self):
         node = utils.create_input_node()
         evset = utils.create_input_event_set()
         result = node.run({node: evset})
         self.assertIsInstance(result, EventSet)
         self.assertTrue(result is evset)
 
+    def test_input_node_from_schema(self):
+        node = utils.create_input_node()
+        other_node = input_node_from_schema(node.schema)
+        self.assertEqual(node.schema, other_node.schema)
+
     def test_run_single_operator(self):
         evset = utils.create_input_event_set()
         result = evset.node().simple_moving_average(10)
         result = result.run(evset)
         self.assertIsInstance(result, EventSet)
 
     def test_hash_map(self):
```

### Comparing `temporian-0.8.1/temporian/core/dataclasses.py` & `temporian-0.9.0/temporian/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/evaluation.py` & `temporian-0.9.0/temporian/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/event_set_ops.py` & `temporian-0.9.0/temporian/core/event_set_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,19 +115,19 @@
             ...     features={"f2": [-10, 100, 5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a != b
             >>> c
             indexes: []
-            features: [('ne_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'ne_f1_f2': [ True False True]
+                    'f1': [ True False True]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -189,20 +189,20 @@
             ...     features={"f3": [-1, 1, 2], "f4": [1, -1, 5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a + b
             >>> c
             indexes: []
-            features: [('add_f1_f3', int64), ('add_f2_f4', int64)]
+            features: [('f1', int64), ('f2', int64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'add_f1_f3': [ -1 101 202]
-                    'add_f2_f4': [ 11 -11 10]
+                    'f1': [ -1 101 202]
+                    'f2': [ 11 -11 10]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -241,19 +241,19 @@
                 ...
             ValueError: ... corresponding features should have the same dtype. ...
 
             >>> # Cast f1 to float
             >>> c = a["f1"].cast(tp.float64) + a["f2"]
             >>> c
             indexes: []
-            features: [('add_f1_f2', float64)]
+            features: [('f1', float64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'add_f1_f2': [ 10. 90. 205.]
+                    'f1': [ 10. 90. 205.]
             ...
 
             ```
 
         Resample example:
             ```python
             >>> a = tp.event_set(
@@ -271,19 +271,19 @@
                 ...
             ValueError: ... should have the same sampling. ...
 
             >>> # Resample a to match b timestamps
             >>> c = a.resample(b) + b
             >>> c
             indexes: []
-            features: [('add_fa_fb', int64)]
+            features: [('fa', int64)]
             events:
                 (4 events):
                     timestamps: [-1. 1.5 3. 5. ]
-                    'add_fa_fb': [-10 16 33 53]
+                    'fa': [-10 16 33 53]
             ...
 
             ```
 
         Reindex example:
             ```python
             >>> a = tp.event_set(
@@ -310,22 +310,22 @@
 
             >>> # Add index 'cat' to b
             >>> b = b.add_index("cat")
             >>> # Make explicit same samplings and add
             >>> c = a + b.resample(a)
             >>> c
             indexes: [('cat', int64)]
-            features: [('add_M_N', int64)]
+            features: [('M', int64)]
             events:
                 cat=1 (2 events):
                     timestamps: [1. 2.]
-                    'add_M_N': [20 40]
+                    'M': [20 40]
                 cat=2 (2 events):
                     timestamps: [3. 4.]
-                    'add_M_N': [60 80]
+                    'M': [60 80]
             ...
 
             ```
 
         Args:
             other: EventSet or scalar value.
 
@@ -378,19 +378,19 @@
             ...     features={"f2": [10, 20, -5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a - b
             >>> c
             indexes: []
-            features: [('sub_f1_f2', int64)]
+            features: [('f1', int64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'sub_f1_f2': [-10 80 205]
+                    'f1': [-10 80 205]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -471,19 +471,19 @@
             ...     features={"f2": [10, 3, 2]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a * b
             >>> c
             indexes: []
-            features: [('mult_f1_f2', int64)]
+            features: [('f1', int64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'mult_f1_f2': [ 0 300 400]
+                    'f1': [ 0 300 400]
             ...
 
             ```
 
         Example with scalar value:
              ```python
             >>> a = tp.event_set(
@@ -630,19 +630,19 @@
             ...     features={"f2": [10.0, 20.0, 50.0]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a / b
             >>> c
             indexes: []
-            features: [('div_f1_f2', float64)]
+            features: [('f1', float64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'div_f1_f2': [0. 5. 4.]
+                    'f1': [0. 5. 4.]
             ...
 
             ```
 
         Example casting integer features:
             ```python
             >>> a = tp.event_set(
@@ -661,19 +661,19 @@
                 ...
             ValueError: Cannot use the divide operator on feature f1 of type int64. ...
 
             >>> # Cast to tp.float64 or tp.float32 before
             >>> c = a.cast(tp.float64) / b.cast(tp.float64)
             >>> c
             indexes: []
-            features: [('div_f1_f2', float64)]
+            features: [('f1', float64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'div_f1_f2': [0. 5. 4.]
+                    'f1': [0. 5. 4.]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -753,19 +753,19 @@
             ...     features={"f2": [10, 3, 150]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a // b
             >>> c
             indexes: []
-            features: [('floordiv_f1_f2', int64)]
+            features: [('f1', int64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'floordiv_f1_f2': [ 0 33 1]
+                    'f1': [ 0 33 1]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -846,19 +846,19 @@
             ...     features={"f2": [0, 3, 2]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a ** b
             >>> c
             indexes: []
-            features: [('pow_f1_f2', int64)]
+            features: [('f1', int64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'pow_f1_f2': [ 1 8 16]
+                    'f1': [ 1 8 16]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -939,19 +939,19 @@
             ...     features={"f2": [10, 5, 150]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a % b
             >>> c
             indexes: []
-            features: [('mod_f1_f2', int64)]
+            features: [('f1', int64)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'mod_f1_f2': [ 0 2 50]
+                    'f1': [ 0 2 50]
             ...
 
             ```
 
         Example with scalar value:
             ```python
             >>> a = tp.event_set(
@@ -1029,19 +1029,19 @@
             ...     features={"f2": [-10, 100, 5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a > b
             >>> c
             indexes: []
-            features: [('gt_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'gt_f1_f2': [ True False True]
+                    'f1': [ True False True]
             ...
 
             ```
 
         Example with scalar:
             ```python
             >>> a = tp.event_set(
@@ -1105,19 +1105,19 @@
             ...     features={"f2": [-10, 100, 5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a >= b
             >>> c
             indexes: []
-            features: [('ge_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'ge_f1_f2': [ True True True]
+                    'f1': [ True True True]
             ...
 
             ```
 
         Example with scalar:
             ```python
             >>> a = tp.event_set(
@@ -1181,19 +1181,19 @@
             ...     features={"f2": [-10, 100, 5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a < b
             >>> c
             indexes: []
-            features: [('lt_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'lt_f1_f2': [False False False]
+                    'f1': [False False False]
             ...
 
             ```
 
         Example with scalar:
             ```python
             >>> a = tp.event_set(
@@ -1257,19 +1257,19 @@
             ...     features={"f2": [-10, 100, 5]},
             ...     same_sampling_as=a
             ... )
 
             >>> c = a <= b
             >>> c
             indexes: []
-            features: [('le_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'le_f1_f2': [False True False]
+                    'f1': [False True False]
             ...
 
             ```
 
         Example with scalar:
             ```python
             >>> a = tp.event_set(
@@ -1332,38 +1332,38 @@
             >>> # Sample boolean features
             >>> b = a > 100
             >>> c = a < 200
 
             >>> d = b & c
             >>> d
             indexes: []
-            features: [('and_f1_f1', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'and_f1_f1': [False True False]
+                    'f1': [False True False]
             ...
 
             ```
 
         Example casting integer to boolean:
             ```python
             >>> a = tp.event_set(
             ...     timestamps=[1, 2, 3],
             ...     features={"f1": [0, 1, 1], "f2": [1, 1, 0]}
             ... )
             >>> b = a.cast(bool)
             >>> c = b["f1"] & b["f2"]
             >>> c
             indexes: []
-            features: [('and_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'and_f1_f2': [False True False]
+                    'f1': [False True False]
             ...
 
             ```
 
         Args:
             other: EventSet with only boolean features.
 
@@ -1397,19 +1397,19 @@
             >>> # Sample boolean features
             >>> b = a <= 100
             >>> c = a >= 200
 
             >>> d = b | c
             >>> d
             indexes: []
-            features: [('or_f1_f1', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'or_f1_f1': [ True False True]
+                    'f1': [ True False True]
             ...
 
             ```
 
         Args:
             other: EventSet with only boolean features.
 
@@ -1443,19 +1443,19 @@
             >>> # Sample boolean features
             >>> b = a > 100
             >>> c = a < 200
 
             >>> d = b ^ c
             >>> d
             indexes: []
-            features: [('xor_f1_f1', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'xor_f1_f1': [ True False True]
+                    'f1': [ True False True]
             ...
 
             ```
 
         Args:
             other: EventSet with only boolean features.
 
@@ -2473,19 +2473,19 @@
                     'f1': [False True False]
             ...
 
             >>> # Element-wise comparison between two EventSets
             >>> c = a.equal(b)
             >>> c
             indexes: []
-            features: [('eq_f1_f2', bool_)]
+            features: [('f1', bool_)]
             events:
                 (3 events):
                     timestamps: [1. 2. 3.]
-                    'eq_f1_f2': [False True False]
+                    'f1': [False True False]
             ...
 
             ```
 
         Args:
             other: Second EventSet or single value to compare.
 
@@ -3525,22 +3525,22 @@
             ValueError: Arguments should have the same sampling. ...
 
             >>> # Third attempt: propagate + resample
             >>> store_resample = store.propagate(products, resample=True)
             >>> div = products / store_resample
             >>> div
             indexes: [('product', int64)]
-            features: [('div_sales_sales', float64)]
+            features: [('sales', float64)]
             events:
                 product=1 (3 events):
                     timestamps: [1. 2. 3.]
-                    'div_sales_sales': [0.01   0.01   0.0167]
+                    'sales': [0.01   0.01   0.0167]
                 product=2 (3 events):
                     timestamps: [1. 2. 3.]
-                    'div_sales_sales': [0.1    0.1    0.1667]
+                    'sales': [0.1    0.1    0.1667]
             ...
 
             ```
 
         Args:
             sampling: EventSet with the indexes to propagate to.
             resample: If true, apply a [`EventSet.resample()`][temporian.EventSet.resample]
@@ -4083,63 +4083,98 @@
                 the input if not.
         """
         from temporian.core.operators.since_last import since_last
 
         return since_last(self, steps=steps, sampling=sampling)
 
     def tick(
-        self: EventSetOrNode, interval: Duration, align: bool = True
+        self: EventSetOrNode,
+        interval: Duration,
+        align: bool = True,
+        after_last: bool = True,
+        before_first: bool = False,
     ) -> EventSetOrNode:
         """Generates timestamps at regular intervals in the range of a guide
         [`EventSet`][temporian.EventSet].
 
         Example with align:
             ```python
             >>> a = tp.event_set(timestamps=[5, 9, 16])
             >>> b = a.tick(interval=tp.duration.seconds(3), align=True)
             >>> b
             indexes: ...
-                    timestamps: [ 6. 9. 12. 15.]
+                    timestamps: [ 6. 9. 12. 15. 18.]
             ...
 
             ```
 
         Example without align:
             ```python
             >>> a = tp.event_set(timestamps=[5, 9, 16])
             >>> b = a.tick(interval=tp.duration.seconds(3), align=False)
             >>> b
             indexes: ...
-                    timestamps: [ 5. 8. 11. 14.]
+                    timestamps: [ 5. 8. 11. 14. 17.]
             ...
 
             ```
 
+        Example with before_first:
+            ```python
+            >>> a = tp.event_set(timestamps=[5, 9, 16])
+            >>> b = a.tick(interval=tp.duration.seconds(3), align=True, before_first=True)
+            >>> b
+            indexes: ...
+                    timestamps: [ 3. 6. 9. 12. 15. 18.]
+            ...
+
+            ```
+
+        Example without after_last:
+            ```python
+            >>> a = tp.event_set(timestamps=[5, 9, 16])
+            >>> b = a.tick(interval=tp.duration.seconds(3), align=True, after_last=False)
+            >>> b
+            indexes: ...
+                    timestamps: [ 6. 9. 12. 15.]
+            ...
+
+            ```
         Args:
             interval: Tick interval.
             align: If false, the first tick is generated at the first timestamp
                 (similar to [`EventSet.begin()`][temporian.EventSet.begin]).
                 If true (default), ticks are generated on timestamps that are
                 multiple of `interval`.
+            after_last: If True, a tick after the last timestamp is included.
+            before_first: If True, a tick before the first timestamp is included.
 
         Returns:
             A feature-less EventSet with regular timestamps.
         """
         from temporian.core.operators.tick import tick
 
-        return tick(self, interval=interval, align=align)
+        return tick(
+            self,
+            interval=interval,
+            align=align,
+            after_last=after_last,
+            before_first=before_first,
+        )
 
     def tick_calendar(
         self: EventSetOrNode,
         second: Optional[Union[int, Literal["*"]]] = None,
         minute: Optional[Union[int, Literal["*"]]] = None,
         hour: Optional[Union[int, Literal["*"]]] = None,
         mday: Optional[Union[int, Literal["*"]]] = None,
         month: Optional[Union[int, Literal["*"]]] = None,
         wday: Optional[Union[int, Literal["*"]]] = None,
+        after_last: bool = True,
+        before_first: bool = False,
     ) -> EventSetOrNode:
         """Generates events periodically at fixed times or dates e.g. each month.
 
         Events are generated in the range of the input
         [`EventSet`][temporian.EventSet] independently for each index.
 
         The usability is inspired in the crontab format, where arguments can
@@ -4161,52 +4196,52 @@
             ```python
             >>> # Every day (at 00:00:00) in the period (exactly one year)
             >>> a = tp.event_set(timestamps=["2021-01-01", "2021-12-31 23:59:59"])
             >>> b = a.tick_calendar(hour=0)
             >>> b
             indexes: ...
             events:
-                (365 events):
+                (366 events):
                     timestamps: [...]
             ...
 
 
             >>> # Every day at 2:30am
             >>> b = a.tick_calendar(hour=2, minute=30)
             >>> tp.glue(b.calendar_hour(), b.calendar_minute())
             indexes: ...
             events:
-                (365 events):
+                (366 events):
                     timestamps: [...]
                     'calendar_hour': [2 2 2 ... 2 2 2]
                     'calendar_minute': [30 30 30 ... 30 30 30]
             ...
 
 
             >>> # Day 5 of every month (at 00:00)
             >>> b = a.tick_calendar(mday=5)
             >>> b.calendar_day_of_month()
             indexes: ...
             events:
-                (12 events):
+                (13 events):
                     timestamps: [...]
                     'calendar_day_of_month': [5 5 5 ... 5 5 5]
             ...
 
 
             >>> # 1st of February of every year
             >>> a = tp.event_set(timestamps=["2020-01-01", "2021-12-31"])
             >>> b = a.tick_calendar(month=2)
             >>> tp.glue(b.calendar_day_of_month(), b.calendar_month())
             indexes: ...
             events:
-                (2 events):
+                (3 events):
                     timestamps: [...]
-                    'calendar_day_of_month': [1 1]
-                    'calendar_month': [2 2]
+                    'calendar_day_of_month': [1 1 1]
+                    'calendar_month': [2 2 2]
             ...
 
             >>> # Every second in the period  (2 hours -> 7200 seconds)
             >>> a = tp.event_set(timestamps=["2020-01-01 00:00:00",
             ...                              "2020-01-01 01:59:59"])
             >>> b = a.tick_calendar(second='*')
             >>> b
@@ -4219,25 +4254,49 @@
             >>> # Every second of the minute 30 of every hour (00:30 and 01:30)
             >>> a = tp.event_set(timestamps=["2020-01-01 00:00",
             ...                              "2020-01-01 02:00"])
             >>> b = a.tick_calendar(second='*', minute=30)
             >>> b
             indexes: ...
             events:
-                (120 events):
+                (121 events):
                     timestamps: [...]
             ...
 
             >>> # Not allowed: intermediate arguments (minute, hour) not specified
             >>> b = a.tick_calendar(second=1, mday=1)  # ambiguous meaning
             Traceback (most recent call last):
                 ...
             ValueError: Can't set argument to None because previous and
             following arguments were specified. Set to '*' or an integer ...
 
+            >>> # not after_last
+            >>> a = tp.event_set(timestamps=["2020-02-01", "2020-04-01"])
+            >>> b = a.tick_calendar(mday=10, after_last=False)
+            >>> tp.glue(b.calendar_day_of_month(), b.calendar_month())
+            indexes: ...
+            events:
+                (2 events):
+                    timestamps: [...]
+                    'calendar_day_of_month': [10 10]
+                    'calendar_month': [2 3]
+            ...
+
+            >>> # before_first
+            >>> a = tp.event_set(timestamps=["2020-02-01", "2020-04-01"])
+            >>> b = a.tick_calendar(mday=10, before_first=True)
+            >>> tp.glue(b.calendar_day_of_month(), b.calendar_month())
+            indexes: ...
+            events:
+                (4 events):
+                    timestamps: [...]
+                    'calendar_day_of_month': [10 10 10 10]
+                    'calendar_month': [1 2 3 4]
+            ...
+
             ```
 
         Args:
             second: '*' (any second), None (auto) or number in range `[0-59]`
                     to tick at specific second of each minute.
             minute: '*' (any minute), None (auto) or number in range `[0-59]`
                     to tick at specific minute of each hour.
@@ -4248,28 +4307,37 @@
                         without some particular day may not have any tick
                         (e.g: day 31 on February).
             month: '*' (any month), None (auto) or number in range `[1-12]` to
                     tick at one particular month of each year.
             wday: '*' (any day), None (auto) or number in range `[0-6]`
                     (Sun-Sat) to tick at particular day of week. Can only be
                     specified if `day_of_month` is `None`.
+            after_last: If True, a tick after the last timestamp is included.
+                    Useful for window operations where you want the timestamps
+                    to be included in the range of the ticks.
+            before_first: If True, a tick before the first timestamp is
+                    included.
+                    Useful for window operations where you want the timestamps
+                    to be included in the range of the ticks.
 
         Returns:
             A feature-less EventSet with timestamps at specified interval.
         """
         from temporian.core.operators.tick_calendar import tick_calendar
 
         return tick_calendar(
             self,
             second=second,
             minute=minute,
             hour=hour,
             mday=mday,
             month=month,
             wday=wday,
+            after_last=after_last,
+            before_first=before_first,
         )
 
     def timestamps(self: EventSetOrNode) -> EventSetOrNode:
         """Converts an [`EventSet`][temporian.EventSet]'s timestamps into a
         `float64` feature.
 
         Features in the input EventSet are ignored, only the timestamps are used.
```

### Comparing `temporian-0.8.1/temporian/core/graph.py` & `temporian-0.9.0/temporian/core/graph.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operator_lib.py` & `temporian-0.9.0/temporian/core/operator_lib.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/BUILD` & `temporian-0.9.0/temporian/core/operators/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/__init__.py` & `temporian-0.9.0/temporian/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/add_index.py` & `temporian-0.9.0/temporian/core/operators/join.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,158 +8,152 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Add and set index operators classes and public API function definitions."""
 
-from typing import List, Union
+"""Join operator class and public API function definitions."""
+
+from typing import Optional
 
-from temporian.core import operator_lib
 from temporian.core.compilation import compile
+from temporian.core.data.dtype import DType
+from temporian.core import operator_lib
 from temporian.core.data.node import (
     EventSetNode,
-    create_node_new_features_new_sampling,
+    create_node_with_new_reference,
+    Feature,
 )
-from temporian.core.data.schema import FeatureSchema, IndexSchema
 from temporian.core.operators.base import Operator
 from temporian.core.typing import EventSetOrNode
 from temporian.proto import core_pb2 as pb
-from temporian.core.operators.drop_index import drop_index
+from temporian.core.data.schema import Schema
 
+JOIN_LEFT = "left"
+# TODO: Add support for outer and inner joins.
 
-class AddIndexOperator(Operator):
+
+class Join(Operator):
     def __init__(
         self,
-        input: EventSetNode,
-        indexes: List[str],
-    ) -> None:
+        left: EventSetNode,
+        right: EventSetNode,
+        how: str = "left",
+        on: Optional[str] = None,
+    ):
         super().__init__()
 
-        output_feature_schemas = self._get_output_feature_schemas(
-            input, indexes
-        )
-        output_indexes = self._get_output_indexes(input, indexes)
-        self._indexes = indexes
-
-        self.add_input("input", input)
+        self.add_input("left", left)
+        self.add_input("right", right)
+        self.add_attribute("how", how)
+        if on is not None:
+            self.add_attribute("on", on)
+        self._on = on
+
+        left.schema.check_compatible_index(right.schema)
+
+        if how not in [JOIN_LEFT]:
+            raise ValueError(
+                f"Non supported join type {how}. Supported join type(s) are:"
+                f" {JOIN_LEFT}"
+            )
 
-        self.add_attribute("indexes", indexes)
+        if on is not None:
+            for node, node_name in [(left, "left"), (right, "right")]:
+                feature_names = node.schema.feature_names()
+                if on not in feature_names:
+                    raise ValueError(
+                        f'Feature "{on}" does not exist in {node_name}'
+                    )
+                on_dtype = node.schema.features[feature_names.index(on)].dtype
+                if on_dtype != DType.INT64:
+                    raise ValueError(
+                        '"on" feature should be of type int64. Got'
+                        f" {on_dtype} instead for {node_name}."
+                    )
+
+        output_features = []
+        output_feature_schemas = []
+        output_features.extend(left.feature_nodes)
+        output_feature_schemas.extend(left.schema.features)
+
+        left_feature_names = left.schema.feature_names()
+        for i2_feature in right.schema.features:
+            if on is not None and i2_feature.name == on:
+                continue
+            output_features.append(Feature(creator=self))
+            output_feature_schemas.append(i2_feature)
+            if i2_feature.name in left_feature_names:
+                raise ValueError(
+                    f'Feature "{i2_feature.name}" is defined in both inputs'
+                )
 
         self.add_output(
             "output",
-            create_node_new_features_new_sampling(
-                features=output_feature_schemas,
-                indexes=output_indexes,
-                is_unix_timestamp=input.schema.is_unix_timestamp,
+            create_node_with_new_reference(
+                schema=Schema(
+                    features=output_feature_schemas,
+                    indexes=left.schema.indexes,
+                    is_unix_timestamp=left.schema.is_unix_timestamp,
+                ),
+                sampling=left.sampling_node,
+                features=output_features,
                 creator=self,
             ),
         )
-        self.check()
 
-    def _get_output_feature_schemas(
-        self, input: EventSetNode, indexes: List[str]
-    ) -> List[FeatureSchema]:
-        return [
-            feature
-            for feature in input.schema.features
-            if feature.name not in indexes
-        ]
-
-    def _get_output_indexes(
-        self, input: EventSetNode, indexes: List[str]
-    ) -> List[IndexSchema]:
-        index_dict = input.schema.index_name_to_dtype()
-        feature_dict = input.schema.feature_name_to_dtype()
-
-        new_indexes: List[IndexSchema] = []
-        for index in indexes:
-            if index in index_dict:
-                raise ValueError(f"{index} is already an index in input.")
-
-            if index not in feature_dict:
-                raise ValueError(f"{index} is not a feature in input.")
+        self.check()
 
-            new_indexes.append(
-                IndexSchema(name=index, dtype=feature_dict[index])
-            )
-        # Note: The new indexes are added after the existing ones.
-        return input.schema.indexes + new_indexes
+    @property
+    def on(self) -> Optional[str]:
+        return self._on
 
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="ADD_INDEX",
+            key="JOIN",
             attributes=[
                 pb.OperatorDef.Attribute(
-                    key="indexes",
-                    type=pb.OperatorDef.Attribute.Type.LIST_STRING,
+                    key="how",
+                    type=pb.OperatorDef.Attribute.Type.STRING,
                 ),
+                pb.OperatorDef.Attribute(
+                    key="on",
+                    type=pb.OperatorDef.Attribute.Type.STRING,
+                    is_optional=True,
+                ),
+            ],
+            inputs=[
+                pb.OperatorDef.Input(key="left"),
+                pb.OperatorDef.Input(key="right"),
             ],
-            inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
-    @property
-    def indexes(self) -> List[str]:
-        return self._indexes
-
 
-operator_lib.register_operator(AddIndexOperator)
-
-
-def _normalize_indexes(
-    indexes: Union[str, List[str]],
-) -> List[str]:
-    if isinstance(indexes, str):
-        return [indexes]
-
-    if len(indexes) == 0:
-        raise ValueError("Cannot specify empty list as `indexes` argument.")
-
-    return indexes
-
-
-def _normalize_indexes_to_set(
-    indexes: Union[str, List[str]],
-) -> List[str]:
-    if isinstance(indexes, str):
-        return [indexes]
-
-    if len(indexes) == 0:
-        raise ValueError("Cannot specify empty list as `indexes` argument.")
-
-    return indexes
+operator_lib.register_operator(Join)
 
 
 @compile
-def add_index(
-    input: EventSetOrNode, indexes: Union[str, List[str]]
+def join(
+    left: EventSetOrNode,
+    right: EventSetOrNode,
+    how: str = "left",
+    on: Optional[str] = None,
 ) -> EventSetOrNode:
-    assert isinstance(input, EventSetNode)
-
-    indexes = _normalize_indexes(indexes)
-    return AddIndexOperator(input, indexes).outputs["output"]
+    assert isinstance(left, EventSetNode)
+    assert isinstance(right, EventSetNode)
 
+    if left.sampling_node is right.sampling_node:
+        raise ValueError(
+            "Both inputs have the same sampling. Use `tp.glue()` instead of"
+            " `EventSet.join()`."
+        )
 
-@compile
-def set_index(
-    input: EventSetOrNode, indexes: Union[str, List[str]]
-) -> EventSetOrNode:
-    assert isinstance(input, EventSetNode)
-
-    indexes = _normalize_indexes_to_set(indexes)
-
-    # Note
-    # The set_index is implemented as a drop_index + add_index.
-    # The implementation could be improved (simpler, faster) with a new
-    # operator to re-order the indexes.
-
-    if len(input.schema.indexes) != 0:
-        input = drop_index(input)
-
-    if len(indexes) != 0:
-        input = add_index(input, indexes)
-
-    return input
+    return Join(
+        left=left,
+        right=right,
+        how=how,
+        on=on,
+    ).outputs["output"]
```

### Comparing `temporian-0.8.1/temporian/core/operators/base.py` & `temporian-0.9.0/temporian/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/begin.py` & `temporian-0.9.0/temporian/core/operators/begin.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/binary/BUILD` & `temporian-0.9.0/temporian/core/operators/binary/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/binary/__init__.py` & `temporian-0.9.0/temporian/core/operators/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/binary/arithmetic.py` & `temporian-0.9.0/temporian/core/operators/binary/arithmetic.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/binary/base.py` & `temporian-0.9.0/temporian/core/operators/binary/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     f" {feature_idx}-th features don't match. Left argument ="
                     f" {feature_1}, right argument = {feature_2}."
                 )
 
         # outputs
         output_features = [  # pylint: disable=g-complex-comprehension
             FeatureSchema(
-                name=self.output_feature_name(feature_1, feature_2),
+                name=feature_1.name,
                 dtype=self.output_feature_dtype(feature_1, feature_2),
             )
             for feature_1, feature_2 in zip(
                 input_1.schema.features, input_2.schema.features
             )
         ]
 
@@ -103,17 +103,12 @@
         """Gets the key of the operator definition."""
 
     @property
     @abstractmethod
     def prefix(self) -> str:
         """Gets the prefix to use for the output features."""
 
-    def output_feature_name(
-        self, feature_1: FeatureSchema, feature_2: FeatureSchema
-    ) -> str:
-        return f"{self.prefix}_{feature_1.name}_{feature_2.name}"
-
     def output_feature_dtype(
         self, feature_1: FeatureSchema, feature_2: FeatureSchema
     ) -> DType:
         del feature_2
         return feature_1.dtype
```

### Comparing `temporian-0.8.1/temporian/core/operators/binary/logical.py` & `temporian-0.9.0/temporian/core/operators/binary/logical.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/binary/relational.py` & `temporian-0.9.0/temporian/core/operators/binary/relational.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/BUILD` & `temporian-0.9.0/temporian/core/operators/calendar/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/__init__.py` & `temporian-0.9.0/temporian/core/operators/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/base.py` & `temporian-0.9.0/temporian/core/operators/calendar/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/day_of_month.py` & `temporian-0.9.0/temporian/core/operators/calendar/day_of_month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/day_of_week.py` & `temporian-0.9.0/temporian/core/operators/calendar/day_of_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/day_of_year.py` & `temporian-0.9.0/temporian/core/operators/calendar/day_of_year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/hour.py` & `temporian-0.9.0/temporian/core/operators/calendar/hour.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/iso_week.py` & `temporian-0.9.0/temporian/core/operators/calendar/iso_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/minute.py` & `temporian-0.9.0/temporian/core/operators/calendar/minute.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/month.py` & `temporian-0.9.0/temporian/core/operators/calendar/month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/second.py` & `temporian-0.9.0/temporian/core/operators/calendar/second.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/BUILD` & `temporian-0.9.0/temporian/core/operators/calendar/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_base.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_base_timezone.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_base_timezone.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_day_of_month.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_day_of_month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_day_of_week.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_day_of_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_day_of_year.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_day_of_year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_hour.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_hour.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_iso_week.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_iso_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_minute.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_minute.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_month.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_second.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_second.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/test/test_calendar_year.py` & `temporian-0.9.0/temporian/core/operators/calendar/test/test_calendar_year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/calendar/year.py` & `temporian-0.9.0/temporian/core/operators/calendar/year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/cast.py` & `temporian-0.9.0/temporian/core/operators/cast.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/combine.py` & `temporian-0.9.0/temporian/core/operators/combine.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/drop_index.py` & `temporian-0.9.0/temporian/core/operators/drop_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/end.py` & `temporian-0.9.0/temporian/core/operators/end.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/enumerate.py` & `temporian-0.9.0/temporian/core/operators/enumerate.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/fast_fourier_transform.py` & `temporian-0.9.0/temporian/core/operators/fast_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/fillna.py` & `temporian-0.9.0/temporian/core/operators/fillna.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/filter.py` & `temporian-0.9.0/temporian/core/operators/filter.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/filter_empty_index.py` & `temporian-0.9.0/temporian/core/operators/filter_empty_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/filter_moving_count.py` & `temporian-0.9.0/temporian/core/operators/filter_moving_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.add_attribute("window_length", window_length)
 
         self._window_length = window_length
 
         self.add_output(
             "output",
             create_node_new_features_new_sampling(
-                features=[],
+                features=input.schema.features,
                 indexes=input.schema.indexes,
                 is_unix_timestamp=input.schema.is_unix_timestamp,
                 creator=self,
             ),
         )
 
         self.check()
```

### Comparing `temporian-0.8.1/temporian/core/operators/glue.py` & `temporian-0.9.0/temporian/core/operators/glue.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,25 +117,25 @@
         ...     timestamps=[0, 1, 5],
         ...     features={"M": [0, 10, 50], "N": [50, 100, 500]},
         ... )
         >>> b = a["M"] + a["N"]
         >>> c = a["M"] - a["N"]
 
         # Glue all features from a,b,c
-        >>> d = tp.glue(a, b, c)
+        >>> d = tp.glue(a, b.rename("plus_N"), c.rename("minus_N"))
         >>> d
         indexes: []
-        features: [('M', int64), ('N', int64), ('add_M_N', int64), ('sub_M_N', int64)]
+        features: [('M', int64), ('N', int64), ('plus_N', int64), ('minus_N', int64)]
         events:
             (3 events):
                 timestamps: [0. 1. 5.]
                 'M': [ 0 10 50]
                 'N': [ 50 100 500]
-                'add_M_N': [ 50 110 550]
-                'sub_M_N': [ -50  -90 -450]
+                'plus_N': [ 50 110 550]
+                'minus_N': [ -50  -90 -450]
         ...
 
         ```
 
     To glue EventSets with duplicated feature names, add a prefix or rename them
     before.
```

### Comparing `temporian-0.8.1/temporian/core/operators/lag.py` & `temporian-0.9.0/temporian/core/operators/lag.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/leak.py` & `temporian-0.9.0/temporian/core/operators/leak.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/map.py` & `temporian-0.9.0/temporian/core/operators/map.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/prefix.py` & `temporian-0.9.0/temporian/core/operators/prefix.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/propagate.py` & `temporian-0.9.0/temporian/core/operators/propagate.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/rename.py` & `temporian-0.9.0/temporian/core/operators/rename.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/resample.py` & `temporian-0.9.0/temporian/core/operators/resample.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/scalar/BUILD` & `temporian-0.9.0/temporian/core/operators/scalar/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/scalar/__init__.py` & `temporian-0.9.0/temporian/core/operators/scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/scalar/arithmetic_scalar.py` & `temporian-0.9.0/temporian/core/operators/scalar/arithmetic_scalar.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/scalar/base.py` & `temporian-0.9.0/temporian/core/operators/scalar/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/scalar/relational_scalar.py` & `temporian-0.9.0/temporian/core/operators/scalar/relational_scalar.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/select.py` & `temporian-0.9.0/temporian/core/operators/select.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/select_index_values.py` & `temporian-0.9.0/temporian/core/operators/select_index_values.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/since_last.py` & `temporian-0.9.0/temporian/core/operators/since_last.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/BUILD` & `temporian-0.9.0/temporian/core/operators/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_add_index.py` & `temporian-0.9.0/temporian/core/operators/test/test_add_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_after.py` & `temporian-0.9.0/temporian/core/operators/test/test_after.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_arithmetic.py` & `temporian-0.9.0/temporian/core/operators/test/test_arithmetic.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,74 +53,72 @@
     def test_addition(self) -> None:
         # Expected result after addition
         expected_evset = event_set(
             timestamps=[0, 1, 2, 1, 1, 2, 0, 1],
             features={
                 "store_id": [1, 1, 1, 1, 2, 2, 2, 2],
                 "product_id": [1, 1, 1, 2, 2, 2, 3, 3],
-                "add_f1_f3": f64([-9.5, 9.5, 32, 10, 3, 0, 6, 9]),
-                "add_f2_f4": f32([6, 5, 4, 6, -3, 8, 11, 11]),
+                "f1": f64([-9.5, 9.5, 32, 10, 3, 0, 6, 9]),
+                "f2": f32([6, 5, 4, 6, -3, 8, 11, 11]),
             },
             indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 + self.evset_2, expected_evset)
 
     def test_subtraction(self) -> None:
         expected_evset = event_set(
             timestamps=[0, 1, 2, 1, 1, 2, 0, 1],
             features={
                 "store_id": [1, 1, 1, 1, 2, 2, 2, 2],
                 "product_id": [1, 1, 1, 2, 2, 2, 3, 3],
-                "sub_f1_f3": f64([-18.5, 20.5, 0, 10, -3, 16, 0, -1]),
-                "sub_f2_f4": f32([-4, -1, 2, 2, 13, 4, 3, 5]),
+                "f1": f64([-18.5, 20.5, 0, 10, -3, 16, 0, -1]),
+                "f2": f32([-4, -1, 2, 2, 13, 4, 3, 5]),
             },
             indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 - self.evset_2, expected_evset)
 
     def test_multiplication(self) -> None:
         expected_evset = event_set(
             timestamps=[0, 1, 2, 1, 1, 2, 0, 1],
             features={
                 "store_id": [1, 1, 1, 1, 2, 2, 2, 2],
                 "product_id": [1, 1, 1, 2, 2, 2, 3, 3],
-                "mult_f1_f3": f64([-63, -82.5, 256, 0, 0, -64, 9, 20]),
-                "mult_f2_f4": f32([5, 6, 3, 8, -40, 12, 28, 24]),
+                "f1": f64([-63, -82.5, 256, 0, 0, -64, 9, 20]),
+                "f2": f32([5, 6, 3, 8, -40, 12, 28, 24]),
             },
             indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 * self.evset_2, expected_evset)
 
     def test_division(self) -> None:
         expected_evset = event_set(
             timestamps=[0, 1, 2, 1, 1, 2, 0, 1],
             features={
                 "store_id": [1, 1, 1, 1, 2, 2, 2, 2],
                 "product_id": [1, 1, 1, 2, 2, 2, 3, 3],
-                "div_f1_f3": f64(
-                    [-14 / 4.5, -15 / 5.5, 1, np.inf, 0, -1, 1, 0.8]
-                ),
-                "div_f2_f4": f32([0.2, 2 / 3, 3, 2, -0.625, 3, 1.75, 8 / 3]),
+                "f1": f64([-14 / 4.5, -15 / 5.5, 1, np.inf, 0, -1, 1, 0.8]),
+                "f2": f32([0.2, 2 / 3, 3, 2, -0.625, 3, 1.75, 8 / 3]),
             },
             indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 / self.evset_2, expected_evset)
 
     def test_floordiv(self) -> None:
         expected_evset = event_set(
             timestamps=[0, 1, 2, 1, 1, 2, 0, 1],
             features={
                 "store_id": [1, 1, 1, 1, 2, 2, 2, 2],
                 "product_id": [1, 1, 1, 2, 2, 2, 3, 3],
-                "floordiv_f1_f3": f64([-4, -3, 1, np.inf, 0, -1, 1, 0]),
-                "floordiv_f2_f4": f32([0, 0, 3, 2, -1, 3, 1, 2]),
+                "f1": f64([-4, -3, 1, np.inf, 0, -1, 1, 0]),
+                "f2": f32([0, 0, 3, 2, -1, 3, 1, 2]),
             },
             indexes=["store_id", "product_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 // self.evset_2, expected_evset)
 
     def test_noindex_unsorted(self) -> None:
@@ -138,16 +136,16 @@
                 "f1": [-3, -2, -1, 0],
             },
             same_sampling_as=evset_1,
         )
         expected = event_set(
             timestamps=[0, 1, 2, 3],
             features={
-                "add_f1_f2": [0, 11, 22, 33],
-                "add_f2_f1": [0, 9, 18, 27],
+                "f1": [0, 11, 22, 33],
+                "f2": [0, 9, 18, 27],
             },
             same_sampling_as=evset_1,
         )
         assertOperatorResult(self, evset_1 + evset_2, expected)
 
 
 if __name__ == "__main__":
```

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_arithmetic_scalar.py` & `temporian-0.9.0/temporian/core/operators/test/test_arithmetic_scalar.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_assign.py` & `temporian-0.9.0/temporian/core/operators/test/test_assign.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_before.py` & `temporian-0.9.0/temporian/core/operators/test/test_before.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_begin.py` & `temporian-0.9.0/temporian/core/operators/test/test_begin.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_cast.py` & `temporian-0.9.0/temporian/core/operators/test/test_cast.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_combine.py` & `temporian-0.9.0/temporian/core/operators/test/test_combine.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_drop.py` & `temporian-0.9.0/temporian/core/operators/test/test_drop.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_drop_index.py` & `temporian-0.9.0/temporian/core/operators/test/test_drop_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_end.py` & `temporian-0.9.0/temporian/core/operators/test/test_end.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_enumerate.py` & `temporian-0.9.0/temporian/core/operators/test/test_enumerate.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_fast_fourier_transform.py` & `temporian-0.9.0/temporian/core/operators/test/test_fast_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_fillna.py` & `temporian-0.9.0/temporian/core/operators/test/test_fillna.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_filter.py` & `temporian-0.9.0/temporian/core/operators/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_filter_empty_index.py` & `temporian-0.9.0/temporian/core/operators/test/test_filter_empty_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_filter_moving_count.py` & `temporian-0.9.0/temporian/core/operators/test/test_filter_moving_count.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,10 +57,20 @@
         result = evset.filter_moving_count(window_length=win_length)
 
         # NOTE: check_sampling=False still checks timestamps
         assertOperatorResult(
             self, result, expected_output, check_sampling=False
         )
 
+    def test_with_feature(
+        self,
+    ):
+        evset = event_set([1, 2, 4], {"f": [10, 11, 14]})
+        expected_output = event_set([1, 4], {"f": [10, 14]})
+        result = evset.filter_moving_count(window_length=1.5)
+        assertOperatorResult(
+            self, result, expected_output, check_sampling=False
+        )
+
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_glue.py` & `temporian-0.9.0/temporian/core/operators/test/test_glue.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_join.py` & `temporian-0.9.0/temporian/core/operators/test/test_join.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_lag.py` & `temporian-0.9.0/temporian/core/operators/test/test_lag.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_leak.py` & `temporian-0.9.0/temporian/core/operators/test/test_leak.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_logical.py` & `temporian-0.9.0/temporian/core/operators/test/test_logical.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,33 +31,33 @@
             same_sampling_as=self.evset_1,
         )
 
     def test_correct_and(self) -> None:
         """Test correct AND operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4],
-            features={"and_x_x": [True, False, False, False]},
+            features={"x": [True, False, False, False]},
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 & self.evset_2, expected)
 
     def test_correct_or(self) -> None:
         """Test correct OR operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4],
-            features={"or_x_x": [True, False, True, True]},
+            features={"x": [True, False, True, True]},
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 | self.evset_2, expected)
 
     def test_correct_xor(self) -> None:
         """Test correct XOR operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4],
-            features={"xor_x_x": [False, False, True, True]},
+            features={"x": [False, False, True, True]},
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 ^ self.evset_2, expected)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_map.py` & `temporian-0.9.0/temporian/core/operators/test/test_map.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_prefix.py` & `temporian-0.9.0/temporian/core/operators/test/test_prefix.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_propagate.py` & `temporian-0.9.0/temporian/core/operators/test/test_propagate.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_relational.py` & `temporian-0.9.0/temporian/core/operators/test/test_relational.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def test_correct_equal(self) -> None:
         """Test correct equal operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4, 5, 6],
             features={
                 "store_id": [0, 0, 1, 1, 2, 2],
                 # NOTE: nan == nan is False
-                "eq_sales_cost": [True, False, False, False, True, False],
+                "sales": [True, False, False, False, True, False],
             },
             indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1.equal(self.evset_2), expected)
 
     def test_equal_str(self) -> None:
@@ -64,15 +64,15 @@
             timestamps=timestamps,
             features={"b": ["A", "B", "A", "B"]},
             same_sampling_as=evset_1,
         )
 
         expected = event_set(
             timestamps=timestamps,
-            features={"eq_a_b": [True, False, False, True]},
+            features={"a": [True, False, False, True]},
             same_sampling_as=evset_1,
         )
         # NOTE: evset_1 == evset_2 is not overloaded for event-wise comparison
         assertOperatorResult(self, evset_1.equal(evset_2), expected)
 
     def test_notequal_str(self) -> None:
         timestamps = [1, 2, 3, 4]
@@ -84,84 +84,84 @@
             timestamps=timestamps,
             features={"b": ["A", "B", "A", "B"]},
             same_sampling_as=evset_1,
         )
 
         expected = event_set(
             timestamps=timestamps,
-            features={"ne_a_b": [False, True, True, False]},
+            features={"a": [False, True, True, False]},
             same_sampling_as=evset_1,
         )
 
         assertOperatorResult(self, evset_1 != evset_2, expected)
 
     def test_correct_not_equal(self) -> None:
         """Test correct not-equal operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4, 5, 6],
             features={
                 "store_id": [0, 0, 1, 1, 2, 2],
                 # NOTE: nan != nan is True
-                "ne_sales_cost": [False, True, True, True, False, True],
+                "sales": [False, True, True, True, False, True],
             },
             indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 != self.evset_2, expected)
 
     def test_correct_greater(self) -> None:
         """Test '>' operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4, 5, 6],
             features={
                 "store_id": [0, 0, 1, 1, 2, 2],
                 # NOTE: any comparison to nan is always False
-                "gt_sales_cost": [False, True, False, False, False, False],
+                "sales": [False, True, False, False, False, False],
             },
             indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 > self.evset_2, expected)
 
     def test_correct_greater_equal(self) -> None:
         """Test '>=' operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4, 5, 6],
             features={
                 "store_id": [0, 0, 1, 1, 2, 2],
                 # NOTE: any comparison to nan is always False
-                "ge_sales_cost": [True, True, False, False, True, False],
+                "sales": [True, True, False, False, True, False],
             },
             indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 >= self.evset_2, expected)
 
     def test_correct_less(self) -> None:
         """Test '<' operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4, 5, 6],
             features={
                 "store_id": [0, 0, 1, 1, 2, 2],
                 # NOTE: any comparison to nan is always False
-                "lt_sales_cost": [False, False, True, False, False, False],
+                "sales": [False, False, True, False, False, False],
             },
             indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 < self.evset_2, expected)
 
     def test_correct_less_equal(self) -> None:
         """Test '<=' operator."""
         expected = event_set(
             timestamps=[1, 2, 3, 4, 5, 6],
             features={
                 "store_id": [0, 0, 1, 1, 2, 2],
                 # NOTE: any comparison to nan is always False
-                "le_sales_cost": [True, False, True, False, True, False],
+                "sales": [True, False, True, False, True, False],
             },
             indexes=["store_id"],
             same_sampling_as=self.evset_1,
         )
         assertOperatorResult(self, self.evset_1 <= self.evset_2, expected)
```

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_relational_scalar.py` & `temporian-0.9.0/temporian/core/operators/test/test_relational_scalar.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_rename.py` & `temporian-0.9.0/temporian/core/operators/test/test_rename.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_resample.py` & `temporian-0.9.0/temporian/core/operators/test/test_resample.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_select.py` & `temporian-0.9.0/temporian/core/operators/test/test_select.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_select_index_values.py` & `temporian-0.9.0/temporian/core/operators/test/test_select_index_values.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_since_last.py` & `temporian-0.9.0/temporian/core/operators/test/test_since_last.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_tick_calendar.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_moving_product.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,200 +8,224 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from datetime import datetime, timedelta, timezone
-from absl.testing import absltest, parameterized
+from math import nan
+
+import numpy as np
+from absl.testing import absltest
+from absl.testing.parameterized import TestCase, parameters
 
 from temporian.implementation.numpy.data.io import event_set
-from temporian.test.utils import assertOperatorResult, SetTimezone
+from temporian.test.utils import f32, f64, assertOperatorResult
 
 
-class TickCalendarOperatorTest(parameterized.TestCase):
-    @parameterized.parameters(
-        {
-            # Test: specify only mday, all days at 00:00
-            "span": ["2020-01-01 00:00", "2020-03-01 00:00"],
-            "calendar_args": dict(mday=1),
-            "expected": [
-                "2020-01-01 00:00",
-                "2020-02-01 00:00",
-                "2020-03-01 00:00",
-            ],
-        },
-        {
-            # Test: mday=31, February should be ignored
-            "span": ["2020-01-01 00:00", "2020-03-31 00:00"],
-            "calendar_args": dict(mday=31),
-            "expected": [
-                "2020-01-31 00:00",
-                "2020-03-31 00:00",
-            ],
-        },
-        {
-            # Test: offsets in hours at beginning and end
-            "span": ["2020-01-01 13:04", "2020-03-06 19:35"],
-            "calendar_args": dict(mday=1),
-            "expected": ["2020-02-01 00:00", "2020-03-01 00:00"],
-        },
-        {
-            # Test: 3 days in the span, should only consider start/end
-            "span": ["2020-01-01", "2020-01-02", "2020-01-03"],
-            "calendar_args": dict(mday="*"),
-            "expected": ["2020-01-01", "2020-01-02", "2020-01-03"],
-        },
-        {
-            # Test: specific mday/hour and offsets
-            "span": ["2020-01-02 13:04", "2020-03-05 19:35"],
-            "calendar_args": dict(hour=3, mday=5),
-            "expected": ["2020-02-05 03:00", "2020-03-05 03:00"],
-        },
-        {
-            # Test: Edge cases for range
-            "span": ["2020-01-10 13:00", "2020-03-10 12:59:59.99"],
-            "calendar_args": dict(hour=13, mday=10),
-            "expected": ["2020-01-10 13:00", "2020-02-10 13:00"],
+class MovingProductTest(TestCase):
+    def test_without_sampling(self):
+        timestamps = f64([1, 2, 3, 5, 6])
+        evset = event_set(
+            timestamps=timestamps, features={"a": f32([2, nan, 3, 0, 5])}
+        )
+
+        expected = event_set(
+            timestamps=timestamps,
+            features={"a": f32([2.0, 2.0, 3.0, 0.0, 0.0])},
+            same_sampling_as=evset,
+        )
+
+        result = evset.moving_product(window_length=2.0)
+        assertOperatorResult(self, result, expected)
+
+    def test_with_zeros_and_nans(self):
+        timestamps = f64([1, 2, 3, 4])
+        evset = event_set(
+            timestamps=timestamps, features={"a": f32([2.0, 0.0, nan, 3.0])}
+        )
+
+        expected = event_set(
+            timestamps=timestamps,
+            features={"a": f32([2.0, 0.0, 0.0, 3.0])},
+            same_sampling_as=evset,
+        )
+
+        result = evset.moving_product(window_length=2.0)
+        assertOperatorResult(self, result, expected)
+
+    def test_empty_event_set(self):
+        timestamps = f64([])
+        evset = event_set(timestamps=timestamps, features={"a": f32([])})
+
+        expected = event_set(
+            timestamps=timestamps,
+            features={"a": f32([])},
+            same_sampling_as=evset,
+        )
+
+        result = evset.moving_product(window_length=2.0)
+        assertOperatorResult(self, result, expected)
+
+    def test_without_sampling_many_features(self):
+        timestamps = [1, 2, 3, 5, 20]
+        evset = event_set(
+            timestamps=timestamps,
+            features={
+                "a": [10.0, 11.0, 12.0, 13.0, 14.0],
+                "b": [20.0, 21.0, 22.0, 23.0, 24.0],
+            },
+        )
+
+        expected = event_set(
+            timestamps=timestamps,
+            features={
+                "a": [10.0, 110.0, 132.0, 13.0, 14.0],
+                "b": [20.0, 420.0, 462.0, 23.0, 24.0],
+            },
+            same_sampling_as=evset,
+        )
+
+        result = evset.moving_product(window_length=2.0)
+        assertOperatorResult(self, result, expected)
+
+    def test_without_sampling_with_index(self):
+        timestamps = [1, 2, 3, 1.1, 2.1, 3.1, 1.2, 2.2, 3.2]
+        evset = event_set(
+            timestamps=timestamps,
+            features={
+                "x": ["X1", "X1", "X1", "X2", "X2", "X2", "X2", "X2", "X2"],
+                "y": ["Y1", "Y1", "Y1", "Y1", "Y1", "Y1", "Y2", "Y2", "Y2"],
+                "a": [10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0, 18.0],
+            },
+            indexes=["x", "y"],
+        )
+
+        expected = event_set(
+            timestamps=timestamps,
+            features={
+                "x": ["X1", "X1", "X1", "X2", "X2", "X2", "X2", "X2", "X2"],
+                "y": ["Y1", "Y1", "Y1", "Y1", "Y1", "Y1", "Y2", "Y2", "Y2"],
+                "a": [
+                    10.0,
+                    110.0,
+                    1320.0,
+                    13.0,
+                    182.0,
+                    2730.0,
+                    16.0,
+                    272.0,
+                    4896.0,
+                ],
+            },
+            indexes=["x", "y"],
+            same_sampling_as=evset,
+        )
+
+        result = evset.moving_product(window_length=5.0)
+        assertOperatorResult(self, result, expected)
+
+    @parameters(
+        {  # normal
+            "timestamps": f64([1, 2, 3, 5, 6]),
+            "feature": [10.0, 11.0, 12.0, 13.0, 14.0],
+            "window_length": 3.1,
+            "sampling_timestamps": [-1.0, 1.0, 1.1, 3.0, 3.5, 6.0, 10.0],
+            "output_feature": [nan, 10.0, 10.0, 1320.0, 1320.0, 2184.0, nan],
+        },
+        {  # w nan
+            "timestamps": f64([1, 2, 3, 5, 6]),
+            "feature": [nan, 11.0, nan, 13.0, 14.0],
+            "window_length": 1.1,
+            "sampling_timestamps": [1, 2, 2.5, 3, 3.5, 4, 5, 6],
+            "output_feature": [nan, 11.0, 11.0, 11.0, nan, nan, 13.0, 182.0],
         },
     )
-    def test_base(self, span, expected, calendar_args):
-        evset = event_set(timestamps=span)
-        expected_evset = event_set(timestamps=expected)
-        result = evset.tick_calendar(**calendar_args)
-
-        # NOTE: check_sampling=False still checks timestamps
-        assertOperatorResult(self, result, expected_evset, check_sampling=False)
-
-        # Check that it's exactly the same with env TZ!=UTC defined
-        with SetTimezone():
-            result = evset.tick_calendar(**calendar_args)
-            assertOperatorResult(
-                self, result, expected_evset, check_sampling=False
-            )
-
-    def test_end_of_month_seconds(self):
-        # All seconds at mday=31, should only be valid for months 1, 3, 5
-
-        evset = event_set(timestamps=["2020-01-01", "2020-06-01"])
-
-        # Expected output
-        def seconds_at_01_01(day, month):
-            return [datetime(2020, day, month, 1, 1, sec) for sec in range(60)]
-
-        expected_evset = event_set(
-            timestamps=seconds_at_01_01(1, 31)
-            + seconds_at_01_01(3, 31)
-            + seconds_at_01_01(5, 31),
-        )
-        result = evset.tick_calendar(second="*", minute=1, hour=1, mday=31)
-        assertOperatorResult(self, result, expected_evset, check_sampling=False)
-
-    def test_end_of_year_minutes(self):
-        # All hours/minutes from 30/12/2019 to 2/1/2020
-        evset = event_set(
-            timestamps=[
-                "2019-12-30 00:00:00",
-                "2020-01-02 23:59:59",
-            ],
-        )
-
-        # Expected timestamps: all hours/minutes in 4 days
-        timestamps = []
-        for day, month, year in [
-            (30, 12, 2019),
-            (31, 12, 2019),
-            (1, 1, 2020),
-            (2, 1, 2020),
-        ]:
-            for hour in range(24):
-                for minute in range(60):
-                    timestamps += [datetime(year, month, day, hour, minute, 0)]
-        expected_evset = event_set(
-            timestamps=timestamps,
-        )
-        result = evset.tick_calendar(minute="*")
-        assertOperatorResult(self, result, expected_evset, check_sampling=False)
-
-    def test_weekdays(self):
-        # All exact hours from all saturdays in 2023
-
-        evset = event_set(
-            timestamps=[
-                "2023-01-01",
-                "2023-12-31 23:00:00",
-            ],
-        )
-
-        # Expected timestamps: all hours on Saturdays
-        timestamps = []
-        day = datetime(2023, 1, 7, tzinfo=timezone.utc)  # First saturday
-        one_week = timedelta(days=7)
-        while day.year < 2024:
-            for hour in range(24):
-                timestamps += [day + timedelta(hours=hour)]
-            day += one_week
-        expected_evset = event_set(
-            timestamps=timestamps,
-        )
-
-        result = evset.tick_calendar(hour="*", wday=5)
-        assertOperatorResult(self, result, expected_evset, check_sampling=False)
-
-    def test_invalid_ranges(self):
-        evset = event_set(timestamps=["2020-01-01", "2020-06-01"])
-        for kwargs in (
-            {"second": -1},
-            {"second": 60},
-            {"minute": -1},
-            {"minute": 60},
-            {"hour": -1},
-            {"hour": 24},
-            {"mday": 0},
-            {"mday": 32},
-            {"mday": -1},  # may be supported in the future
-            {"month": -1},
-            {"month": 13},
-            {"wday": -1},
-            {"wday": 7},
-        ):
-            with self.assertRaisesRegex(
-                ValueError, "Value should be '\*' or integer in range"
-            ):
-                evset.tick_calendar(**kwargs)
-
-    def test_invalid_types(self):
-        evset = event_set(timestamps=["2020-01-01", "2020-06-01"])
-        for kwargs in (
-            {"second": "1"},
-            {"minute": "00"},
-            {"hour": "00:00"},
-            {"month": "January"},
-            {"wday": "Sat"},
-        ):
-            with self.assertRaisesRegex(ValueError, "Non matching type"):
-                evset.tick_calendar(**kwargs)  # type: ignore
+    def test_with_sampling(
+        self,
+        timestamps,
+        feature,
+        window_length,
+        sampling_timestamps,
+        output_feature,
+    ):
+        evset = event_set(
+            timestamps=timestamps,
+            features={"a": feature},
+        )
+        sampling = event_set(timestamps=sampling_timestamps)
 
-    def test_undefined_args(self):
-        evset = event_set(timestamps=["2020-01-01", "2020-06-01"])
-        with self.assertRaisesRegex(
-            ValueError,
-            "Can't set argument to None because previous and following",
-        ):
-            evset.tick_calendar(second=1, hour=1)  # undefined min
+        expected = event_set(
+            timestamps=sampling_timestamps,
+            features={"a": output_feature},
+            same_sampling_as=sampling,
+        )
+
+        result = evset.moving_product(
+            window_length=window_length, sampling=sampling
+        )
+        assertOperatorResult(self, result, expected)
+
+    def test_with_variable_winlen_same_sampling(self):
+        timestamps = f64([0, 1, 2, 3, 5, 20])
+        evset = event_set(
+            timestamps=timestamps,
+            features={"a": f32([nan, 10, 11, 12, 13, 14])},
+        )
+
+        window = event_set(
+            timestamps=timestamps,
+            features={"a": f64([1, 1, 1.5, 0.5, 3.5, 20])},
+            same_sampling_as=evset,
+        )
+
+        expected = event_set(
+            timestamps=timestamps,
+            features={"a": f32([nan, 10, 110, 12, nan, nan])},
+            same_sampling_as=evset,
+        )
+
+        result = evset.moving_product(window_length=window)
+        assertOperatorResult(self, result, expected)
+
+    def test_with_variable_winlen_diff_sampling(self):
+        window_timestamps = f64([-1, 1, 4, 19, 20, 20])
+        window_length = f64([10, 0.5, 2.5, 19, 16, np.inf])
+
+        evset = event_set(
+            timestamps=f64([0, 1, 2, 3, 5, 20]),
+            features={"a": f32([nan, 10, 11, 12, 13, 14])},
+        )
+
+        window = event_set(
+            timestamps=window_timestamps,
+            features={"a": window_length},
+        )
+
+        expected = event_set(
+            timestamps=window_timestamps,
+            features={"a": f32([nan, 10.0, 132.0, nan, 182.0, nan])},
+            same_sampling_as=window,
+        )
+
+        result = evset.moving_product(window_length=window)
+        assertOperatorResult(self, result, expected)
 
+    def test_error_input_int(self):
+        evset = event_set([1, 2], {"f": [1, 2]})
         with self.assertRaisesRegex(
             ValueError,
-            "Can't set argument to None because previous and following",
+            "moving_product requires the input EventSet to contain",
         ):
-            evset.tick_calendar(second=1, month=1)
+            _ = evset.moving_product(1)
 
+    def test_error_input_bytes(self):
+        evset = event_set([1, 2], {"f": ["A", "B"]})
         with self.assertRaisesRegex(
             ValueError,
-            "Can't set argument to None because previous and following",
+            "moving_product requires the input EventSet to contain",
         ):
-            evset.tick_calendar(hour=0, month=1)
+            _ = evset.moving_product(1)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_timestamps.py` & `temporian-0.9.0/temporian/core/operators/test/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_unary.py` & `temporian-0.9.0/temporian/core/operators/test/test_unary.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_unique_timestamps.py` & `temporian-0.9.0/temporian/core/operators/test/test_unique_timestamps.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_until_next.py` & `temporian-0.9.0/temporian/core/operators/test/test_until_next.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/test/test_where.py` & `temporian-0.9.0/temporian/core/operators/test/test_where.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/tick.py` & `temporian-0.9.0/temporian/core/operators/timestamps.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,90 +9,56 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Tick operator class and public API function definitions."""
+"""Timestamps operator class and public API function definitions."""
 
 from temporian.core import operator_lib
-from temporian.core.compilation import compile
 from temporian.core.data.node import (
     EventSetNode,
-    create_node_new_features_new_sampling,
+    create_node_new_features_existing_sampling,
 )
+from temporian.core.compilation import compile
 from temporian.core.operators.base import Operator
 from temporian.core.typing import EventSetOrNode
 from temporian.proto import core_pb2 as pb
-from temporian.core.data.duration_utils import (
-    Duration,
-    NormalizedDuration,
-    normalize_duration,
-)
+from temporian.core.data import dtype
 
 
-class Tick(Operator):
-    def __init__(
-        self, input: EventSetNode, interval: NormalizedDuration, align: bool
-    ):
+class Timestamps(Operator):
+    def __init__(self, input: EventSetNode):
         super().__init__()
 
-        self._interval = interval
-        self._align = align
-
         self.add_input("input", input)
-        self.add_attribute("interval", interval)
-        self.add_attribute("align", align)
 
         self.add_output(
             "output",
-            create_node_new_features_new_sampling(
-                features=[],
-                indexes=input.schema.indexes,
-                is_unix_timestamp=input.schema.is_unix_timestamp,
+            create_node_new_features_existing_sampling(
+                features=[("timestamps", dtype.float64)],
+                sampling_node=input,
                 creator=self,
             ),
         )
 
         self.check()
 
-    @property
-    def interval(self) -> NormalizedDuration:
-        return self._interval
-
-    @property
-    def align(self) -> bool:
-        return self._align
-
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="TICK",
-            attributes=[
-                pb.OperatorDef.Attribute(
-                    key="interval",
-                    type=pb.OperatorDef.Attribute.Type.FLOAT_64,
-                ),
-                pb.OperatorDef.Attribute(
-                    key="align",
-                    type=pb.OperatorDef.Attribute.Type.BOOL,
-                ),
-            ],
+            key="TIMESTAMPS",
+            attributes=[],
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
-operator_lib.register_operator(Tick)
+operator_lib.register_operator(Timestamps)
 
 
-# TODO: Add support for begin/end arguments.
 @compile
-def tick(
-    input: EventSetOrNode, interval: Duration, align: bool = True
-) -> EventSetOrNode:
+def timestamps(input: EventSetOrNode) -> EventSetOrNode:
     assert isinstance(input, EventSetNode)
 
-    return Tick(
-        input=input, interval=normalize_duration(interval), align=align
-    ).outputs["output"]
+    return Timestamps(input=input).outputs["output"]
```

### Comparing `temporian-0.8.1/temporian/core/operators/tick_calendar.py` & `temporian-0.9.0/temporian/core/operators/tick_calendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """TickCalendar operator class and public API function definitions."""
-from typing import Literal, Tuple, Optional, Union
+from typing import Literal, Optional, Tuple, Union
 
 import numpy as np
 
 from temporian.core import operator_lib
 from temporian.core.compilation import compile
 from temporian.core.data.node import (
     EventSetNode,
@@ -38,34 +38,40 @@
         input: EventSetNode,
         second: Union[int, TypeWildCard],
         minute: Union[int, TypeWildCard],
         hour: Union[int, TypeWildCard],
         mday: Union[int, TypeWildCard],
         month: Union[int, TypeWildCard],
         wday: Union[int, TypeWildCard],
+        after_last: bool = True,
+        before_first: bool = False,
     ):
         super().__init__()
         if not input.schema.is_unix_timestamp:
             raise ValueError(
                 "Can only use tick_calendar on unix timestamp samplings"
             )
 
         # Attributes
         self._second = self._check_arg(second, self.seconds_max_range())
         self._minute = self._check_arg(minute, self.minutes_max_range())
         self._hour = self._check_arg(hour, self.hours_max_range())
         self._mday = self._check_arg(mday, self.mday_max_range())
         self._month = self._check_arg(month, self.month_max_range())
         self._wday = self._check_arg(wday, self.wday_max_range())
+        self.after_last = after_last
+        self.before_first = before_first
         self.add_attribute("second", second)
         self.add_attribute("minute", minute)
         self.add_attribute("hour", hour)
         self.add_attribute("mday", mday)
         self.add_attribute("month", month)
         self.add_attribute("wday", wday)
+        self.add_attribute("after_last", after_last)
+        self.add_attribute("before_first", before_first)
 
         self.add_input("input", input)
 
         self.add_output(
             "output",
             create_node_new_features_new_sampling(
                 features=[],
@@ -174,14 +180,22 @@
                     key="month",
                     type=pb.OperatorDef.Attribute.Type.ANY,
                 ),
                 pb.OperatorDef.Attribute(
                     key="wday",
                     type=pb.OperatorDef.Attribute.Type.ANY,
                 ),
+                pb.OperatorDef.Attribute(
+                    key="after_last",
+                    type=pb.OperatorDef.Attribute.Type.BOOL,
+                ),
+                pb.OperatorDef.Attribute(
+                    key="before_first",
+                    type=pb.OperatorDef.Attribute.Type.BOOL,
+                ),
             ],
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
 operator_lib.register_operator(TickCalendar)
@@ -193,14 +207,16 @@
     input: EventSetOrNode,
     second: Optional[Union[int, TypeWildCard]] = None,
     minute: Optional[Union[int, TypeWildCard]] = None,
     hour: Optional[Union[int, TypeWildCard]] = None,
     mday: Optional[Union[int, TypeWildCard]] = None,
     month: Optional[Union[int, TypeWildCard]] = None,
     wday: Optional[Union[int, TypeWildCard]] = None,
+    after_last: bool = True,
+    before_first: bool = False,
 ) -> EventSetOrNode:
     # Don't allow empty args
     if all(arg is None for arg in (second, minute, hour, mday, month, wday)):
         raise ValueError("At least one argument must be provided (not None).")
 
     # All defined values must be consecutive (no gaps with None)
     if wday is not None:
@@ -252,8 +268,10 @@
         input=input,  # type: ignore
         second=second,
         minute=minute,
         hour=hour,
         mday=mday,
         month=month,
         wday=wday,
+        after_last=after_last,
+        before_first=before_first,
     ).outputs["output"]
```

### Comparing `temporian-0.8.1/temporian/core/operators/timestamps.py` & `temporian-0.9.0/temporian/core/operators/unique_timestamps.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,56 +9,56 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Timestamps operator class and public API function definitions."""
-
+"""Unique timestamps operator class and public API function definitions."""
 from temporian.core import operator_lib
+from temporian.core.compilation import compile
 from temporian.core.data.node import (
     EventSetNode,
-    create_node_new_features_existing_sampling,
+    create_node_new_features_new_sampling,
 )
-from temporian.core.compilation import compile
 from temporian.core.operators.base import Operator
 from temporian.core.typing import EventSetOrNode
+from temporian.utils.typecheck import typecheck
 from temporian.proto import core_pb2 as pb
-from temporian.core.data import dtype
 
 
-class Timestamps(Operator):
+class UniqueTimestamps(Operator):
     def __init__(self, input: EventSetNode):
         super().__init__()
 
         self.add_input("input", input)
 
         self.add_output(
             "output",
-            create_node_new_features_existing_sampling(
-                features=[("timestamps", dtype.float64)],
-                sampling_node=input,
+            create_node_new_features_new_sampling(
+                features=[],
+                indexes=input.schema.indexes,
+                is_unix_timestamp=input.schema.is_unix_timestamp,
                 creator=self,
             ),
         )
-
         self.check()
 
     @classmethod
     def build_op_definition(cls) -> pb.OperatorDef:
         return pb.OperatorDef(
-            key="TIMESTAMPS",
+            key="UNIQUE_TIMESTAMPS",
             attributes=[],
             inputs=[pb.OperatorDef.Input(key="input")],
             outputs=[pb.OperatorDef.Output(key="output")],
         )
 
 
-operator_lib.register_operator(Timestamps)
+operator_lib.register_operator(UniqueTimestamps)
 
 
+@typecheck
 @compile
-def timestamps(input: EventSetOrNode) -> EventSetOrNode:
+def unique_timestamps(input: EventSetOrNode) -> EventSetOrNode:
     assert isinstance(input, EventSetNode)
 
-    return Timestamps(input=input).outputs["output"]
+    return UniqueTimestamps(input=input).outputs["output"]
```

### Comparing `temporian-0.8.1/temporian/core/operators/unary.py` & `temporian-0.9.0/temporian/core/operators/unary.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/unique_timestamps.py` & `temporian-0.9.0/temporian/beam/operators/unique_timestamps.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,56 +9,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Unique timestamps operator class and public API function definitions."""
-from temporian.core import operator_lib
-from temporian.core.compilation import compile
-from temporian.core.data.node import (
-    EventSetNode,
-    create_node_new_features_new_sampling,
-)
-from temporian.core.operators.base import Operator
-from temporian.core.typing import EventSetOrNode
-from temporian.utils.typecheck import typecheck
-from temporian.proto import core_pb2 as pb
-
-
-class UniqueTimestamps(Operator):
-    def __init__(self, input: EventSetNode):
-        super().__init__()
-
-        self.add_input("input", input)
-
-        self.add_output(
-            "output",
-            create_node_new_features_new_sampling(
-                features=[],
-                indexes=input.schema.indexes,
-                is_unix_timestamp=input.schema.is_unix_timestamp,
-                creator=self,
-            ),
-        )
-        self.check()
+from typing import Dict
+import numpy as np
 
-    @classmethod
-    def build_op_definition(cls) -> pb.OperatorDef:
-        return pb.OperatorDef(
-            key="UNIQUE_TIMESTAMPS",
-            attributes=[],
-            inputs=[pb.OperatorDef.Input(key="input")],
-            outputs=[pb.OperatorDef.Output(key="output")],
-        )
+from temporian.core.operators.unique_timestamps import (
+    UniqueTimestamps as CurrentOperator,
+)
+from temporian.beam import implementation_lib
+from temporian.beam.operators.base import (
+    BeamOperatorImplementation,
+    beam_eventset_flatmap,
+)
+from temporian.beam.typing import (
+    BeamEventSet,
+    FeatureItem,
+)
 
 
-operator_lib.register_operator(UniqueTimestamps)
+class UniqueTimestampsBeamImplementation(BeamOperatorImplementation):
+    def call(self, input: BeamEventSet) -> Dict[str, BeamEventSet]:
+        assert isinstance(self.operator, CurrentOperator)
+
+        def fun(item: FeatureItem, feature_idx: int):
+            if feature_idx == 0:
+                indexes, (timestamps, _) = item
+                yield indexes, (np.unique(timestamps), None)
+
+        output = beam_eventset_flatmap(
+            input,
+            name=f"{self.operator}",
+            fn=fun,
+        )
 
+        return {"output": output}
 
-@typecheck
-@compile
-def unique_timestamps(input: EventSetOrNode) -> EventSetOrNode:
-    assert isinstance(input, EventSetNode)
 
-    return UniqueTimestamps(input=input).outputs["output"]
+implementation_lib.register_operator_implementation(
+    CurrentOperator, UniqueTimestampsBeamImplementation
+)
```

### Comparing `temporian-0.8.1/temporian/core/operators/until_next.py` & `temporian-0.9.0/temporian/core/operators/until_next.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/where.py` & `temporian-0.9.0/temporian/core/operators/where.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/BUILD` & `temporian-0.9.0/temporian/core/operators/window/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/__init__.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_sum.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,22 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Window operators."""
 
-# pylint: disable=unused-import
-# pylint: disable=line-too-long
-# fmt: off
-
-from temporian.core.operators.window.simple_moving_average import simple_moving_average
-from temporian.core.operators.window.moving_standard_deviation import moving_standard_deviation
-from temporian.core.operators.window.moving_sum import cumsum
-from temporian.core.operators.window.moving_sum import moving_sum
-from temporian.core.operators.window.moving_count import moving_count
-from temporian.core.operators.window.moving_min import moving_min
-from temporian.core.operators.window.moving_max import moving_max
-from temporian.core.operators.window.moving_product import cumprod
-from temporian.core.operators.window.moving_product import moving_product
+from temporian.core.operators.window.moving_sum import (
+    MovingSumOperator,
+)
+from temporian.implementation.numpy import implementation_lib
+from temporian.implementation.numpy.operators.window.base import (
+    BaseWindowNumpyImplementation,
+)
+from temporian.implementation.numpy_cc.operators import operators_cc
+
+
+class MovingSumNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the moving sum operator."""
+
+    def _implementation(self):
+        return operators_cc.moving_sum
+
+
+implementation_lib.register_operator_implementation(
+    MovingSumOperator, MovingSumNumpyImplementation
+)
```

### Comparing `temporian-0.8.1/temporian/core/operators/window/base.py` & `temporian-0.9.0/temporian/core/operators/window/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/moving_count.py` & `temporian-0.9.0/temporian/core/operators/window/moving_count.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/moving_max.py` & `temporian-0.9.0/temporian/core/operators/window/moving_max.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/moving_min.py` & `temporian-0.9.0/temporian/core/operators/window/moving_min.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/moving_product.py` & `temporian-0.9.0/temporian/core/operators/window/moving_product.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/moving_standard_deviation.py` & `temporian-0.9.0/temporian/core/operators/window/moving_standard_deviation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/moving_sum.py` & `temporian-0.9.0/temporian/core/operators/window/moving_sum.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/simple_moving_average.py` & `temporian-0.9.0/temporian/core/operators/window/simple_moving_average.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/BUILD` & `temporian-0.9.0/temporian/core/operators/window/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_base.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_cumprod.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_cumprod.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_cumsum.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_moving_count.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_moving_count.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_moving_max.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_moving_max.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_moving_min.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_moving_min.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_moving_product.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_moving_sum.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,56 +18,28 @@
 from absl.testing import absltest
 from absl.testing.parameterized import TestCase, parameters
 
 from temporian.implementation.numpy.data.io import event_set
 from temporian.test.utils import f32, f64, assertOperatorResult
 
 
-class MovingProductTest(TestCase):
+class MovingSumTest(TestCase):
     def test_without_sampling(self):
-        timestamps = f64([1, 2, 3, 5, 6])
+        timestamps = f64([1, 2, 3, 5, 20])
         evset = event_set(
-            timestamps=timestamps, features={"a": f32([2, nan, 3, 0, 5])}
+            timestamps=timestamps, features={"a": f32([10, nan, 12, 13, 14])}
         )
 
         expected = event_set(
             timestamps=timestamps,
-            features={"a": f32([2.0, 2.0, 3.0, 0.0, 0.0])},
+            features={"a": f32([10.0, 10.0, 22.0, 35.0, 14.0])},
             same_sampling_as=evset,
         )
 
-        result = evset.moving_product(window_length=2.0)
-        assertOperatorResult(self, result, expected)
-
-    def test_with_zeros_and_nans(self):
-        timestamps = f64([1, 2, 3, 4])
-        evset = event_set(
-            timestamps=timestamps, features={"a": f32([2.0, 0.0, nan, 3.0])}
-        )
-
-        expected = event_set(
-            timestamps=timestamps,
-            features={"a": f32([2.0, 0.0, 0.0, 3.0])},
-            same_sampling_as=evset,
-        )
-
-        result = evset.moving_product(window_length=2.0)
-        assertOperatorResult(self, result, expected)
-
-    def test_empty_event_set(self):
-        timestamps = f64([])
-        evset = event_set(timestamps=timestamps, features={"a": f32([])})
-
-        expected = event_set(
-            timestamps=timestamps,
-            features={"a": f32([])},
-            same_sampling_as=evset,
-        )
-
-        result = evset.moving_product(window_length=2.0)
+        result = evset.moving_sum(window_length=5.0)
         assertOperatorResult(self, result, expected)
 
     def test_without_sampling_many_features(self):
         timestamps = [1, 2, 3, 5, 20]
         evset = event_set(
             timestamps=timestamps,
             features={
@@ -75,21 +47,21 @@
                 "b": [20.0, 21.0, 22.0, 23.0, 24.0],
             },
         )
 
         expected = event_set(
             timestamps=timestamps,
             features={
-                "a": [10.0, 110.0, 132.0, 13.0, 14.0],
-                "b": [20.0, 420.0, 462.0, 23.0, 24.0],
+                "a": [10.0, 21.0, 33.0, 46.0, 14.0],
+                "b": [20.0, 41.0, 63.0, 86.0, 24.0],
             },
             same_sampling_as=evset,
         )
 
-        result = evset.moving_product(window_length=2.0)
+        result = evset.moving_sum(window_length=5.0)
         assertOperatorResult(self, result, expected)
 
     def test_without_sampling_with_index(self):
         timestamps = [1, 2, 3, 1.1, 2.1, 3.1, 1.2, 2.2, 3.2]
         evset = event_set(
             timestamps=timestamps,
             features={
@@ -101,47 +73,37 @@
         )
 
         expected = event_set(
             timestamps=timestamps,
             features={
                 "x": ["X1", "X1", "X1", "X2", "X2", "X2", "X2", "X2", "X2"],
                 "y": ["Y1", "Y1", "Y1", "Y1", "Y1", "Y1", "Y2", "Y2", "Y2"],
-                "a": [
-                    10.0,
-                    110.0,
-                    1320.0,
-                    13.0,
-                    182.0,
-                    2730.0,
-                    16.0,
-                    272.0,
-                    4896.0,
-                ],
+                "a": [10.0, 21.0, 33.0, 13.0, 27.0, 42.0, 16.0, 33.0, 51.0],
             },
             indexes=["x", "y"],
             same_sampling_as=evset,
         )
 
-        result = evset.moving_product(window_length=5.0)
+        result = evset.moving_sum(window_length=5.0)
         assertOperatorResult(self, result, expected)
 
     @parameters(
         {  # normal
             "timestamps": f64([1, 2, 3, 5, 6]),
             "feature": [10.0, 11.0, 12.0, 13.0, 14.0],
             "window_length": 3.1,
             "sampling_timestamps": [-1.0, 1.0, 1.1, 3.0, 3.5, 6.0, 10.0],
-            "output_feature": [nan, 10.0, 10.0, 1320.0, 1320.0, 2184.0, nan],
+            "output_feature": [0.0, 10.0, 10.0, 33.0, 33.0, 39.0, 0.0],
         },
         {  # w nan
             "timestamps": f64([1, 2, 3, 5, 6]),
             "feature": [nan, 11.0, nan, 13.0, 14.0],
             "window_length": 1.1,
             "sampling_timestamps": [1, 2, 2.5, 3, 3.5, 4, 5, 6],
-            "output_feature": [nan, 11.0, 11.0, 11.0, nan, nan, 13.0, 182.0],
+            "output_feature": [0.0, 11.0, 11.0, 11.0, 0.0, 0.0, 13.0, 27.0],
         },
     )
     def test_with_sampling(
         self,
         timestamps,
         feature,
         window_length,
@@ -156,15 +118,15 @@
 
         expected = event_set(
             timestamps=sampling_timestamps,
             features={"a": output_feature},
             same_sampling_as=sampling,
         )
 
-        result = evset.moving_product(
+        result = evset.moving_sum(
             window_length=window_length, sampling=sampling
         )
         assertOperatorResult(self, result, expected)
 
     def test_with_variable_winlen_same_sampling(self):
         timestamps = f64([0, 1, 2, 3, 5, 20])
         evset = event_set(
@@ -176,19 +138,19 @@
             timestamps=timestamps,
             features={"a": f64([1, 1, 1.5, 0.5, 3.5, 20])},
             same_sampling_as=evset,
         )
 
         expected = event_set(
             timestamps=timestamps,
-            features={"a": f32([nan, 10, 110, 12, nan, nan])},
+            features={"a": f32([0, 10, 21, 12, 36, 60])},
             same_sampling_as=evset,
         )
 
-        result = evset.moving_product(window_length=window)
+        result = evset.moving_sum(window_length=window)
         assertOperatorResult(self, result, expected)
 
     def test_with_variable_winlen_diff_sampling(self):
         window_timestamps = f64([-1, 1, 4, 19, 20, 20])
         window_length = f64([10, 0.5, 2.5, 19, 16, np.inf])
 
         evset = event_set(
@@ -199,33 +161,25 @@
         window = event_set(
             timestamps=window_timestamps,
             features={"a": window_length},
         )
 
         expected = event_set(
             timestamps=window_timestamps,
-            features={"a": f32([nan, 10.0, 132.0, nan, 182.0, nan])},
+            features={"a": f32([0, 10, 23, 46, 27, 60])},
             same_sampling_as=window,
         )
 
-        result = evset.moving_product(window_length=window)
+        result = evset.moving_sum(window_length=window)
         assertOperatorResult(self, result, expected)
 
-    def test_error_input_int(self):
-        evset = event_set([1, 2], {"f": [1, 2]})
-        with self.assertRaisesRegex(
-            ValueError,
-            "moving_product requires the input EventSet to contain",
-        ):
-            _ = evset.moving_product(1)
-
     def test_error_input_bytes(self):
         evset = event_set([1, 2], {"f": ["A", "B"]})
         with self.assertRaisesRegex(
             ValueError,
-            "moving_product requires the input EventSet to contain",
+            "moving_sum requires the input EventSet to contain numerical",
         ):
-            _ = evset.moving_product(1)
+            _ = evset.moving_sum(1)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_moving_standard_deviation.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_moving_standard_deviation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/operators/window/test/test_simple_moving_average.py` & `temporian-0.9.0/temporian/core/operators/window/test/test_simple_moving_average.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/schedule.py` & `temporian-0.9.0/temporian/core/schedule.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/serialization.py` & `temporian-0.9.0/temporian/core/serialization.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/BUILD` & `temporian-0.9.0/temporian/core/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/compilation_test.py` & `temporian-0.9.0/temporian/core/test/compilation_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/evaluation_test.py` & `temporian-0.9.0/temporian/core/test/evaluation_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/graph_test.py` & `temporian-0.9.0/temporian/core/test/graph_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/magic_methods_test.py` & `temporian-0.9.0/temporian/core/test/magic_methods_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,64 +275,64 @@
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 != float_2
         self.assertTrue(isinstance(out.creator, NotEqualOperator))
-        self.assertTrue(out.schema.features[0].name == "ne_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "ne_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_boolean(out, float_1)
 
     def test_greater(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 > float_2
         self.assertTrue(isinstance(out.creator, GreaterOperator))
-        self.assertTrue(out.schema.features[0].name == "gt_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "gt_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_boolean(out, float_1)
 
     def test_less(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 < float_2
         self.assertTrue(isinstance(out.creator, LessOperator))
-        self.assertTrue(out.schema.features[0].name == "lt_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "lt_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_boolean(out, float_1)
 
     def test_greater_equal(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 >= float_2
         self.assertTrue(isinstance(out.creator, GreaterEqualOperator))
-        self.assertTrue(out.schema.features[0].name == "ge_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "ge_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_boolean(out, float_1)
 
     def test_less_equal(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 <= float_2
         self.assertTrue(isinstance(out.creator, LessEqualOperator))
-        self.assertTrue(out.schema.features[0].name == "le_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "le_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_boolean(out, float_1)
 
     # ###################################
     # ### Relational scalar operators ###
     # ###################################
 
     def test_not_equal_scalar(self, float_1: EventSetNodeOrEvset, **kwargs):
@@ -424,90 +424,90 @@
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 + float_2
         self.assertTrue(isinstance(out.creator, AddOperator))
-        self.assertTrue(out.schema.features[0].name == "add_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "add_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_node_same_dtype(float_1, out)
 
     def test_subtraction(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 - float_2
         self.assertTrue(isinstance(out.creator, SubtractOperator))
-        self.assertTrue(out.schema.features[0].name == "sub_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "sub_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_node_same_dtype(float_1, out)
 
     def test_multiplication(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 * float_2
         self.assertTrue(isinstance(out.creator, MultiplyOperator))
-        self.assertTrue(out.schema.features[0].name == "mult_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "mult_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_node_same_dtype(float_1, out)
 
     def test_division(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 / float_2
         self.assertTrue(isinstance(out.creator, DivideOperator))
-        self.assertTrue(out.schema.features[0].name == "div_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "div_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_node_same_dtype(float_1, out)
 
     def test_floordiv(
         self, int_1: EventSetNodeOrEvset, int_2: EventSetNodeOrEvset, **kwargs
     ):
         # First, check that truediv is not supported for integer types
         with self.assertRaises(ValueError):
             out = int_1 / int_2
 
         # Check floordiv operator instead
         out = int_1 // int_2
         self.assertTrue(isinstance(out.creator, FloorDivOperator))
-        self.assertTrue(out.schema.features[0].name == "floordiv_f5_f7")
-        self.assertTrue(out.schema.features[1].name == "floordiv_f6_f8")
+        self.assertTrue(out.schema.features[0].name == "f5")
+        self.assertTrue(out.schema.features[1].name == "f6")
         self._check_node_same_dtype(int_1, out)
 
     def test_modulo(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1 % float_2
         self.assertTrue(isinstance(out.creator, ModuloOperator))
-        self.assertTrue(out.schema.features[0].name == "mod_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "mod_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_node_same_dtype(float_1, out)
 
     def test_power(
         self,
         float_1: EventSetNodeOrEvset,
         float_2: EventSetNodeOrEvset,
         **kwargs,
     ):
         out = float_1**float_2
         self.assertTrue(isinstance(out.creator, PowerOperator))
-        self.assertTrue(out.schema.features[0].name == "pow_f1_f3")
-        self.assertTrue(out.schema.features[1].name == "pow_f2_f4")
+        self.assertTrue(out.schema.features[0].name == "f1")
+        self.assertTrue(out.schema.features[1].name == "f2")
         self._check_node_same_dtype(float_1, out)
 
     # ###################################
     # ### Arithmetic scalar operators ###
     # ###################################
 
     def test_addition_scalar(
```

### Comparing `temporian-0.8.1/temporian/core/test/operator_test.py` & `temporian-0.9.0/temporian/core/test/operator_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/registered_operators_test.py` & `temporian-0.9.0/temporian/core/test/registered_operators_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/serialization_test.py` & `temporian-0.9.0/temporian/core/test/serialization_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/test/utils.py` & `temporian-0.9.0/temporian/core/test/utils.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/types.py` & `temporian-0.9.0/temporian/core/types.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/core/typing.py` & `temporian-0.9.0/temporian/core/typing.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/__init__.py` & `temporian-0.9.0/temporian/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/data/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/display_utils.py` & `temporian-0.9.0/temporian/implementation/numpy/data/display_utils.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/dtype_normalization.py` & `temporian-0.9.0/temporian/implementation/numpy/data/dtype_normalization.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/event_set.py` & `temporian-0.9.0/temporian/implementation/numpy/data/event_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                     f" ({len(self.timestamps)})."
                 )
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, IndexData):
             return False
 
-        if not np.array_equal(self.timestamps, other.timestamps):
+        if not np.allclose(self.timestamps, other.timestamps):
             return False
 
         for f1, f2 in zip(self.features, other.features):
             if f1.dtype.kind == "f":
                 if not np.allclose(f1, f2, equal_nan=True):
                     return False
             else:
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/io.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,201 +1,205 @@
-from typing import Any, List, Optional, Union, Dict
+# Copyright 2021 Google LLC.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+from abc import abstractmethod
 import logging
+from typing import Dict, Optional, List, Any, Union
+
 import numpy as np
+from temporian.core.data.duration_utils import NormalizedDuration
+
+from temporian.core.operators.window.base import BaseWindowOperator
+from temporian.implementation.numpy.data.event_set import IndexData
+from temporian.implementation.numpy.data.event_set import (
+    EventSet,
+)
+from temporian.implementation.numpy.operators.base import OperatorImplementation
 from temporian.implementation.numpy.data.dtype_normalization import (
-    normalize_features,
-    normalize_timestamps,
-    numpy_array_to_tp_dtype,
+    tp_dtype_to_np_dtype,
 )
 
-from temporian.utils.typecheck import typecheck
-from temporian.implementation.numpy.data.event_set import EventSet, IndexData
-from temporian.core.evaluation import run
-from temporian.core.operators.add_index import add_index
-from temporian.core.data.schema import Schema
-
-# Array of values as feed by the user.
-DataArray = Union[List[Any], np.ndarray, "pandas.Series"]
-
-
-# Note: Keep the documentation about supported types in sync with
-# "normalize_timestamp" and "normalize_features".
-@typecheck
-def event_set(
-    timestamps: DataArray,
-    features: Optional[Dict[str, DataArray]] = None,
-    indexes: Optional[List[str]] = None,
-    name: Optional[str] = None,
-    is_unix_timestamp: Optional[bool] = None,
-    same_sampling_as: Optional[EventSet] = None,
-) -> EventSet:
-    """Creates an [`EventSet`][temporian.EventSet] from arrays (lists, NumPy
-    arrays, Pandas Series.)
-
-    Usage examples:
-
-        ```python
-        >>> # Creates an EventSet with 4 timestamps and 3 features.
-        >>> evset = tp.event_set(
-        ...     timestamps=[1, 2, 3, 4],
-        ...     features={
-        ...         "feature_1": [0.5, 0.6, np.nan, 0.9],
-        ...         "feature_2": ["red", "blue", "red", "blue"],
-        ...         "feature_3": [10, -1, 5, 5],
-        ...     },
-        ... )
-
-        >>> # Creates an EventSet with an index.
-        >>> evset = tp.event_set(
-        ...     timestamps=[1, 2, 3, 4],
-        ...     features={
-        ...         "feature_1": [0.5, 0.6, np.nan, 0.9],
-        ...         "feature_2": ["red", "blue", "red", "blue"],
-        ...     },
-        ...     indexes=["feature_2"],
-        ... )
-
-        >>> # Create an EventSet with datetimes.
-        >>> from datetime import datetime
-        >>> evset = tp.event_set(
-        ...     timestamps=[datetime(2015, 1, 1), datetime(2015, 1, 2)],
-        ...     features={
-        ...         "feature_1": [0.5, 0.6],
-        ...         "feature_2": ["red", "blue"],
-        ...     },
-        ...     indexes=["feature_2"],
-        ... )
-
-        ```
-
-    Supported values for `timestamps`:
-
-    - List of int, float, str, bytes and datetime.
-    - Numpy arrays of int{32, 64}, float{32, 64}, str_, string_ / bytes_,
-        Numpy datetime64, and object containing "str".
-    - Pandas series of int{32, 64}, float{32, 64}, Pandas Timestamp.
-
-    String timestamps are interpreted as ISO 8601 datetime.
-
-    Supported values for `features`:
-
-    - List of int, float, str, bytes, bool, and datetime.
-    - Numpy arrays of int{32, 64}, float{32, 64}, str_, string_ / bytes_,
-        Numpy datetime64, or object containing "str".
-    - Pandas series of int{32, 64}, float{32, 64}, Pandas Timestamp.
-
-    Date / datetime features are converted to int64 unix times.
-    NaN for float-like features are interpreted as missing values.
-
-    Args:
-        timestamps: Array of timestamps values.
-        features: Dictionary of feature names to feature values. Feature
-            and timestamp arrays must be of the same length.
-        indexes: Names of the features to use as indexes. If empty
-            (default), the data is not indexed. Only integer and string features
-            can be used as indexes.
-        name: Optional name of the EventSet. Used for debugging, and
-            graph serialization.
-        is_unix_timestamp: Whether the timestamps correspond to unix time. Unix
-            times are required for calendar operators. If `None` (default),
-            timestamps are interpreted as unix times if the `timestamps`
-            argument is an array of date or date-like object.
-        same_sampling_as: If set, the new EventSet is checked and tagged as
-            having the same sampling as `same_sampling_as`. Some operators,
-            such as [`EventSet.filter()`][temporian.EventSet.filter], require
-            their inputs to have the same sampling.
-
-    Returns:
-        An EventSet.
-    """
-    if features is None:
-        features = {}
-
-    logging.debug("Normalizing features")
-    features = {
-        name: normalize_features(value, name)
-        for name, value in features.items()
-    }
-
-    # Check timestamps and all features are of same length
-    if not all(len(f) == len(timestamps) for f in features.values()):
-        raise ValueError(
-            "Timestamps and all features must have the same length."
+
+class BaseWindowNumpyImplementation(OperatorImplementation):
+    """Interface definition and common logic for numpy implementation of
+    window operators."""
+
+    def __init__(self, operator: BaseWindowOperator) -> None:
+        super().__init__(operator)
+        assert isinstance(operator, BaseWindowOperator)
+
+    def __call__(
+        self,
+        input: EventSet,
+        sampling: Optional[EventSet] = None,
+        window_length: Optional[EventSet] = None,
+    ) -> Dict[str, EventSet]:
+        assert isinstance(self.operator, BaseWindowOperator)
+
+        # pick effective sampling
+        effective_sampling = input
+        if self.operator.has_variable_winlen:
+            assert window_length is not None
+            effective_sampling = window_length
+        elif self.operator.has_sampling:
+            assert sampling is not None
+            effective_sampling = sampling
+
+        # check that sampling isn't the input's, in which case we don't pass it
+        # to cpp impl to use the more efficient sampling-less version
+        has_sampling = (
+            effective_sampling.node().sampling_node
+            is not input.node().sampling_node
         )
 
-    # Convert timestamps to expected type.
-    logging.debug("Normalizing timestamps")
-    timestamps, auto_is_unix_timestamp = normalize_timestamps(timestamps)
-
-    if not np.all(timestamps[:-1] <= timestamps[1:]):
-        logging.debug("Sorting timestamps")
-        order = np.argsort(timestamps, kind="mergesort")
-        timestamps = timestamps[order]
-        features = {name: value[order] for name, value in features.items()}
-
-    if is_unix_timestamp is None:
-        is_unix_timestamp = auto_is_unix_timestamp
-    assert isinstance(is_unix_timestamp, bool)
-
-    # Infer the schema
-    logging.debug("Assembling schema")
-    schema = Schema(
-        features=[
-            (feature_key, numpy_array_to_tp_dtype(feature_key, feature_data))
-            for feature_key, feature_data in features.items()
-        ],
-        indexes=[],
-        is_unix_timestamp=is_unix_timestamp,
-    )
-
-    # Shallow copy the data to temporian format
-    logging.debug("Assembling data")
-    index_data = IndexData(
-        features=[
-            features[feature_name] for feature_name in schema.feature_names()
-        ],
-        timestamps=timestamps,
-        schema=schema,
-    )
-    evset = EventSet(
-        schema=schema,
-        data={(): index_data},
-    )
-
-    if indexes:
-        # Index the data
-        logging.debug("Indexing events")
-        input_node = evset.node()
-        output_node = add_index(input_node, indexes=indexes)
-        evset = run(output_node, {input_node: evset})
-        assert isinstance(evset, EventSet)
-
-    evset.name = name
-
-    if same_sampling_as is not None:
-        logging.debug("Setting same sampling")
-        evset.schema.check_compatible_index(same_sampling_as.schema)
-
-        if evset.data.keys() != same_sampling_as.data.keys():
-            raise ValueError(
-                "The new EventSet and `same_sampling_as` have the same"
-                " indexes, but different index keys. They should have the"
-                " same index keys to have the same sampling."
+        # create destination evset
+        output_schema = self.operator.outputs["output"].schema
+        output_evset = EventSet(data={}, schema=output_schema)
+
+        # For each index
+        for index_key, sampling_data in effective_sampling.data.items():
+            output_data = IndexData(
+                features=[],
+                timestamps=sampling_data.timestamps,
+                schema=None,  # Checking is done later
             )
 
-        for key, same_sampling_as_value in same_sampling_as.data.items():
-            if not np.all(
-                evset.data[key].timestamps == same_sampling_as_value.timestamps
-            ):
-                raise ValueError(
-                    "The new EventSet and `same_sampling_as` have different"
-                    f" timestamps values for the index={key!r}. The timestamps"
-                    " should be equal for both to have the same sampling."
+            if window_length is not None:
+                effective_window_length = window_length.data[
+                    index_key
+                ].features[0]
+                # Warn if not all window length values are positive
+                if not np.all(effective_window_length > 0):
+                    logging.warning(
+                        "`window_length`'s values should be strictly"
+                        " positive. 0, NaN and negative window lengths will"
+                        " output missing values."
+                    )
+            else:
+                assert self.operator.window_length is not None
+                effective_window_length = self.operator.window_length
+
+            sampling_timestamps = (
+                sampling_data.timestamps if has_sampling else None
+            )
+
+            if index_key in input.data:
+                input_data = input.data[index_key]
+
+                self._compute(
+                    src_timestamps=input_data.timestamps,
+                    src_features=input_data.features,
+                    sampling_timestamps=sampling_timestamps,
+                    dst_features=output_data.features,
+                    window_length=effective_window_length,
+                )
+            else:
+                # Sets the feature data as missing.
+                empty_features = [
+                    np.empty((0,), dtype=tp_dtype_to_np_dtype(f.dtype))
+                    for f in output_schema.features
+                ]
+                empty_timestamps = np.empty((0,), dtype=np.float64)
+                self._compute(
+                    src_timestamps=empty_timestamps,
+                    src_features=empty_features,
+                    sampling_timestamps=sampling_timestamps,
+                    dst_features=output_data.features,
+                    window_length=effective_window_length,
                 )
 
-            # Discard the new timestamps arrays.
-            evset.data[key].timestamps = same_sampling_as_value.timestamps
+            output_data.check_schema(output_schema)
+            output_evset.set_index_value(
+                index_key, output_data, normalize=False
+            )
 
-        evset.node()._sampling = same_sampling_as.node().sampling_node
+        return {"output": output_evset}
 
-    return evset
+    @abstractmethod
+    def _implementation(self) -> Any:
+        pass
+
+    def _compute(
+        self,
+        src_timestamps: np.ndarray,
+        src_features: List[np.ndarray],
+        sampling_timestamps: Optional[np.ndarray],
+        dst_features: List[np.ndarray],
+        window_length: Union[NormalizedDuration, np.ndarray],
+    ) -> None:
+        assert isinstance(self.operator, BaseWindowOperator)
+
+        implementation = self._implementation()
+        for src_ts in src_features:
+            kwargs = {
+                "evset_timestamps": src_timestamps,
+                "evset_values": src_ts,
+                "window_length": window_length,
+            }
+            if sampling_timestamps is not None:
+                kwargs["sampling_timestamps"] = sampling_timestamps
+            dst_feature = implementation(**kwargs)
+            dst_features.append(dst_feature)
+
+    def apply_feature_wise(
+        self,
+        src_timestamps: np.ndarray,
+        src_feature: np.ndarray,
+        feature_idx: int,
+    ) -> np.ndarray:
+        """Applies the operator on a single feature."""
+        assert isinstance(self.operator, BaseWindowOperator)
+
+        implementation = self._implementation()
+        kwargs = {
+            "evset_timestamps": src_timestamps,
+            "evset_values": src_feature,
+            "window_length": self.operator.window_length,
+        }
+        return implementation(**kwargs)
+
+    def apply_feature_wise_with_sampling(
+        self,
+        src_timestamps: Optional[np.ndarray],
+        src_feature: Optional[np.ndarray],
+        sampling_timestamps: np.ndarray,
+        feature_idx: int,
+    ) -> np.ndarray:
+        """Applies the operator on a single feature with a sampling."""
+
+        assert isinstance(self.operator, BaseWindowOperator)
+        implementation = self._implementation()
+
+        if src_feature is not None:
+            kwargs = {
+                "evset_timestamps": src_timestamps,
+                "evset_values": src_feature,
+                "window_length": self.operator.window_length,
+                "sampling_timestamps": sampling_timestamps,
+            }
+            return implementation(**kwargs)
+        else:
+            # Sets the feature data as missing.
+            output_schema = self.operator.outputs["output"].schema
+            output_dtype = output_schema.features[feature_idx].dtype
+            empty_features = np.empty(
+                (0,), dtype=tp_dtype_to_np_dtype(output_dtype)
+            )
+            empty_timestamps = np.empty((0,), dtype=np.float64)
+            kwargs = {
+                "evset_timestamps": empty_timestamps,
+                "evset_values": empty_features,
+                "window_length": self.operator.window_length,
+                "sampling_timestamps": sampling_timestamps,
+            }
+            return implementation(**kwargs)
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/plotter.py` & `temporian-0.9.0/temporian/implementation/numpy/data/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,24 @@
 
 def bokeh_backend():
     from temporian.implementation.numpy.data import plotter_bokeh
 
     return plotter_bokeh.Plotter
 
 
+def bokeh_webgl_backend():
+    from temporian.implementation.numpy.data import plotter_bokeh
+
+    return plotter_bokeh.PlotterWebGL
+
+
 BACKENDS: Dict[str, Callable] = {
     "matplotlib": matplotlib_backend,
     "bokeh": bokeh_backend,
+    "bokeh_webgl": bokeh_webgl_backend,
 }
 
 
 def error_message_import_backend(backend: str) -> str:
     return (
         f"Cannot plot with selected backend={backend}. Solutions: (1) Install"
         f" {backend} e.g. 'pip install {backend}', or (2) use a different"
@@ -177,22 +184,22 @@
 
 def _list_index_values(
     indexes: Optional[IndexKeyList], evsets: InputEventSet, max_values: int
 ) -> List[NormalizedIndexKey]:
     """Lists all the index values to plot."""
 
     flat_indexes = set(normalize_index_key_list(indexes, None))
-    index_values = []
+    index_values = set()
     for evtset in _unroll_evsets(evsets):
         for index_value in evtset.data:
             if indexes is None or index_value in flat_indexes:
-                index_values.append(index_value)
+                index_values.add(index_value)
                 if len(index_values) >= max_values:
-                    return index_values
-    return index_values
+                    return list(index_values)
+    return list(index_values)
 
 
 def plot(
     evsets: InputEventSet,
     indexes: Optional[IndexKeyList] = None,
     features: InputFeatures = None,
     width_px: int = 1024,
@@ -275,15 +282,15 @@
         style: A `Style` or equivalent string like: `line`, `marker` or `vline`.
         return_fig: If true, returns the figure object. The figure object
             depends on the backend.
         interactive: If true, creates an interactive plotting. interactive=True
             effectively selects a backend that support interactive plotting.
             Ignored if "backend" is set.
         backend: Plotting library to use. Possible values are: matplotlib,
-            bokeh. If set, overrides the "interactive" argument.
+            bokeh, and bokeh_webgl. If set, overrides the "interactive" argument.
         merge: If true, plots all features in the same plots. If false, plots
             features in separate plots. merge=True on event-sets [e1, e2] is
             equivalent to plotting (e1, e2).
         font_scale: Scaling factor for all the fonts.
     """
 
     if merge:
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/plotter_base.py` & `temporian-0.9.0/temporian/implementation/numpy/data/plotter_base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/plotter_bokeh.py` & `temporian-0.9.0/temporian/implementation/numpy/data/plotter_bokeh.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     Options,
     Style,
     PlotterBackend,
 )
 
 
 class Plotter(PlotterBackend):
+    output_backend = "canvas"
+
     def __init__(self, num_plots: int, options: Options):
         super().__init__(num_plots, options)
 
         self.figs = []
         self.options = options
 
     def new_subplot(
@@ -42,15 +44,15 @@
         self,
     ):
         if self.cur_fig is not None:
             self.figs.append(self.cur_fig)
 
     def ensure_cur_is_available(self, categorical_values: Optional[List[str]]):
         if self.cur_fig is None:
-            self.cur_fig = create_fig(
+            self.cur_fig = self.create_fig(
                 self.cur_title,
                 self.cur_is_unix_timestamp,
                 self.options,
                 categorical_values,
             )
             self.has_categorical_values = categorical_values is not None
         else:
@@ -148,61 +150,66 @@
             figure_set = self.figs[0]
             figure_set.toolbar.logo = None
 
         output_notebook(hide_banner=True)
         show(figure_set)
         return figure_set
 
+    def create_fig(
+        self,
+        title: Optional[str],
+        is_unix_timestamp: bool,
+        options: Options,
+        categorical_values: Optional[List[str]],
+    ):
+        tools = [
+            "xpan",
+            "pan",
+            "xwheel_zoom",
+            "ywheel_zoom",
+            "box_zoom",
+            "reset",
+            "undo",
+            "save",
+            "hover",
+        ]
+
+        fig_args = {}
+        if is_unix_timestamp:
+            fig_args["x_axis_type"] = "datetime"
+        if title:
+            fig_args["title"] = title
+
+        if options.min_time is not None or options.max_time is not None:
+            args = {}
+            if options.min_time is not None:
+                args["start"] = (
+                    convert_timestamp_to_datetime(options.min_time)
+                    if is_unix_timestamp
+                    else options.min_time
+                )
+            if options.max_time is not None:
+                args["end"] = (
+                    convert_timestamp_to_datetime(options.max_time)
+                    if is_unix_timestamp
+                    else options.max_time
+                )
+            fig_args["x_range"] = Range1d(**args)
+
+        if categorical_values is not None:
+            fig_args["y_range"] = categorical_values
 
-def create_fig(
-    title: Optional[str],
-    is_unix_timestamp: bool,
-    options: Options,
-    categorical_values: Optional[List[str]],
-):
-    tools = [
-        "xpan",
-        "pan",
-        "xwheel_zoom",
-        "ywheel_zoom",
-        "box_zoom",
-        "reset",
-        "undo",
-        "save",
-        "hover",
-    ]
-
-    fig_args = {}
-    if is_unix_timestamp:
-        fig_args["x_axis_type"] = "datetime"
-    if title:
-        fig_args["title"] = title
-
-    if options.min_time is not None or options.max_time is not None:
-        args = {}
-        if options.min_time is not None:
-            args["start"] = (
-                convert_timestamp_to_datetime(options.min_time)
-                if is_unix_timestamp
-                else options.min_time
-            )
-        if options.max_time is not None:
-            args["end"] = (
-                convert_timestamp_to_datetime(options.max_time)
-                if is_unix_timestamp
-                else options.max_time
-            )
-        fig_args["x_range"] = Range1d(**args)
+        # Note: Ranges cannot be set after the figure is created see:
+        # https://discourse.bokeh.org/t/updating-y-range-to-categorical/2397/3
+        fig = figure(
+            width=options.width_px,
+            height=options.height_per_plot_px,
+            tools=tools,
+            output_backend=self.output_backend,
+            **fig_args,
+        )
 
-    if categorical_values is not None:
-        fig_args["y_range"] = categorical_values
+        return fig
 
-    # Note: Ranges cannot be set after the figure is created see:
-    # https://discourse.bokeh.org/t/updating-y-range-to-categorical/2397/3
-    fig = figure(
-        width=options.width_px,
-        height=options.height_per_plot_px,
-        tools=tools,
-        **fig_args,
-    )
 
-    return fig
+class PlotterWebGL(Plotter):
+    output_backend = "webgl"
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/plotter_matplotlib.py` & `temporian-0.9.0/temporian/implementation/numpy/data/plotter_matplotlib.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/test/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/data/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/test/event_set_test.py` & `temporian-0.9.0/temporian/implementation/numpy/data/test/event_set_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/test/io_test.py` & `temporian-0.9.0/temporian/implementation/numpy/data/test/io_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from absl import logging
 import numpy as np
 import math
 import pandas as pd
 from numpy.testing import assert_array_equal
 from datetime import datetime
 
-from temporian.implementation.numpy.data.io import event_set
+from temporian.implementation.numpy.data.io import event_set, from_struct
 from temporian.implementation.numpy.data.event_set import IndexData, EventSet
 from temporian.core.data.schema import Schema
 from temporian.core.data.dtype import DType
 
 
 class IOTest(absltest.TestCase):
     def test_event_set(self):
@@ -195,10 +195,43 @@
                 timestamps=[1, 2],
                 features={
                     # np.array({1, 2}) would produce a single-item value
                     "y": {1, 2},
                 },
             )
 
+    def test_from_struct(self):
+        evset = from_struct(
+            [
+                (
+                    {"i1": 1, "i2": "A"},
+                    {"timestamp": [1, 2], "f1": [10, 11], "f2": ["X", "Y"]},
+                ),
+                (
+                    {"i1": 1, "i2": "B"},
+                    {"timestamp": [3, 4], "f1": [12, 13], "f2": ["X", "X"]},
+                ),
+                (
+                    {"i1": 2, "i2": "A"},
+                    {"timestamp": [5, 6], "f1": [14, 15], "f2": ["Y", "Y"]},
+                ),
+                (
+                    {"i1": 2, "i2": "B"},
+                    {"timestamp": [7, 8], "f1": [16, 17], "f2": ["Y", "Z"]},
+                ),
+            ]
+        )
+        expected = event_set(
+            timestamps=[1, 2, 3, 4, 5, 6, 7, 8],
+            features={
+                "f1": [10, 11, 12, 13, 14, 15, 16, 17],
+                "f2": ["X", "Y", "X", "X", "Y", "Y", "Y", "Z"],
+                "i1": [1, 1, 1, 1, 2, 2, 2, 2],
+                "i2": ["A", "A", "B", "B", "A", "A", "B", "B"],
+            },
+            indexes=["i1", "i2"],
+        )
+        self.assertEqual(evset, expected)
+
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/test/plotter_test.py` & `temporian-0.9.0/temporian/implementation/numpy/data/test/plotter_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/test/test_data/test_html_repr_limits_golden.html` & `temporian-0.9.0/temporian/implementation/numpy/data/test/test_data/test_html_repr_limits_golden.html`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/data/test/test_data/test_html_repr_no_limits_golden.html` & `temporian-0.9.0/temporian/implementation/numpy/data/test/test_data/test_html_repr_no_limits_golden.html`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/evaluation.py` & `temporian-0.9.0/temporian/implementation/numpy/evaluation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/implementation_lib.py` & `temporian-0.9.0/temporian/implementation/numpy/implementation_lib.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/operators/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/__init__.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/add_index.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/add_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/base.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/begin.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/begin.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/binary/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/operators/binary/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/binary/__init__.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/binary/arithmetic.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/binary/arithmetic.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/binary/base.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/binary/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/binary/logical.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/binary/logical.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/binary/relational.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/binary/relational.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/BUILD`

 * *Files 14% similar despite different names*

```diff
@@ -3,119 +3,111 @@
     licenses = ["notice"],
 )
 
 # Libraries
 # =========
 
 py_library(
-    name = "calendar",
+    name = "window",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
 )
 
 py_library(
     name = "base",
     srcs = ["base.py"],
     srcs_version = "PY3",
     deps = [
-        "//temporian/core/operators/calendar:base",
+        # already_there/numpy
+        "//temporian/core/operators/window:base",
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/implementation/numpy/operators:base",
+        "//temporian/core/data:duration_utils",
+        "//temporian/implementation/numpy/data:dtype_normalization",
     ],
 )
 
 py_library(
-    name = "day_of_month",
-    srcs = ["day_of_month.py"],
+    name = "simple_moving_average",
+    srcs = ["simple_moving_average.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/operators/calendar:day_of_month",
+        "//temporian/core/operators/window:simple_moving_average",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "day_of_week",
-    srcs = ["day_of_week.py"],
+    name = "moving_standard_deviation",
+    srcs = ["moving_standard_deviation.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/operators/calendar:day_of_week",
+        "//temporian/core/operators/window:moving_standard_deviation",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "day_of_year",
-    srcs = ["day_of_year.py"],
+    name = "moving_product",
+    srcs = ["moving_product.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/operators/calendar:day_of_year",
+        "//temporian/core/operators/window:moving_product",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "hour",
-    srcs = ["hour.py"],
+    name = "moving_sum",
+    srcs = ["moving_sum.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/operators/calendar:hour",
+        "//temporian/core/operators/window:moving_sum",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "iso_week",
-    srcs = ["iso_week.py"],
+    name = "moving_count",
+    srcs = ["moving_count.py"],
     srcs_version = "PY3",
     deps = [
+        # already_there/numpy
         ":base",
-        "//temporian/core/operators/calendar:iso_week",
+        "//temporian/core/operators/window:moving_count",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
+        "//temporian/core/data:duration_utils",
     ],
 )
 
 py_library(
-    name = "minute",
-    srcs = ["minute.py"],
+    name = "moving_max",
+    srcs = ["moving_max.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/operators/calendar:minute",
+        "//temporian/core/operators/window:moving_max",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
 
 py_library(
-    name = "month",
-    srcs = ["month.py"],
+    name = "moving_min",
+    srcs = ["moving_min.py"],
     srcs_version = "PY3",
     deps = [
         ":base",
-        "//temporian/core/operators/calendar:month",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "second",
-    srcs = ["second.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:second",
-        "//temporian/implementation/numpy:implementation_lib",
-    ],
-)
-
-py_library(
-    name = "year",
-    srcs = ["year.py"],
-    srcs_version = "PY3",
-    deps = [
-        ":base",
-        "//temporian/core/operators/calendar:year",
+        "//temporian/core/operators/window:moving_min",
         "//temporian/implementation/numpy:implementation_lib",
+        "//temporian/implementation/numpy_cc/operators:operators_cc",
     ],
 )
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/base.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/day_of_month.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/day_of_month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/day_of_week.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/day_of_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/day_of_year.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/day_of_year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/hour.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/hour.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/iso_week.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/iso_week.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/minute.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/minute.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/month.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/month.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/second.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/second.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/calendar/year.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/calendar/year.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/cast.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/cast.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/combine.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/combine.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/drop_index.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/drop_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/end.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/end.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/enumerate.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/enumerate.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/fast_fourier_transform.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/fast_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/filter.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/filter.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/filter_empty_index.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/filter_empty_index.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/filter_moving_count.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/filter_moving_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,24 +41,24 @@
         # Create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
 
         window_length = self.operator.window_length
 
         # Fill output EventSet's data
         for index_key, index_data in input.data.items():
-            dst_timestamps = operators_cc.filter_moving_count(
+            sampling_idx = operators_cc.filter_moving_count(
                 index_data.timestamps,
                 window_length=window_length,
             )
 
             output_evset.set_index_value(
                 index_key,
                 IndexData(
-                    features=[],
-                    timestamps=dst_timestamps,
+                    features=[f[sampling_idx] for f in index_data.features],
+                    timestamps=index_data.timestamps[sampling_idx],
                     schema=output_schema,
                 ),
             )
 
         return {"output": output_evset}
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/glue.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/glue.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/join.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/join.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/lag.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/lag.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/leak.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/leak.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/map.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/map.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/prefix.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/prefix.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/propagate.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/propagate.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/rename.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/rename.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/resample.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/resample.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/scalar/BUILD` & `temporian-0.9.0/temporian/implementation/numpy/operators/scalar/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/scalar/__init__.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/scalar/arithmetic_scalar.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/scalar/base.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/scalar/base.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/scalar/relational_scalar.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/scalar/relational_scalar.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/select.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/select.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/select_index_values.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/select_index_values.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/since_last.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/since_last.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/tick.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/tick.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Implementation for the Tick operator."""
 
 
+import math
 from typing import Dict
 
-import math
 import numpy as np
-from temporian.implementation.numpy.data.event_set import IndexData, EventSet
+
 from temporian.core.operators.tick import Tick
 from temporian.implementation.numpy import implementation_lib
+from temporian.implementation.numpy.data.event_set import EventSet, IndexData
 from temporian.implementation.numpy.operators.base import OperatorImplementation
 
 
 class TickNumpyImplementation(OperatorImplementation):
     def __init__(self, operator: Tick) -> None:
         assert isinstance(operator, Tick)
         super().__init__(operator)
@@ -37,34 +38,52 @@
         output_schema = self.output_schema("output")
 
         # create output EventSet
         output_evset = EventSet(data={}, schema=output_schema)
 
         # fill output EventSet data
         for index_key, index_data in input.data.items():
-            if len(index_data.timestamps) == 0:
+            if len(index_data.timestamps) < 1:
                 dst_timestamps = np.array([], dtype=np.float64)
             else:
                 begin = index_data.timestamps[0]
                 end = index_data.timestamps[-1]
 
+                save_begin = begin
+                save_end = end
                 if self.operator.align:
-                    save_begin = begin
                     begin = (
                         float(begin // self.operator.interval)
                         * self.operator.interval
                     )
 
                     if save_begin != begin:
                         begin += self.operator.interval
 
+                # adjust begin if before_first and the first tick is not going
+                # to be equal to the begin
+                if self.operator.before_first and (
+                    (save_begin - begin) % self.operator.interval != 0
+                ):
+                    begin -= self.operator.interval
+                # adjust end if after_last and the final tick is not going
+                # to be equal to the end
+                if self.operator.after_last and (
+                    (save_end - begin) % self.operator.interval != 0
+                ):
+                    end += self.operator.interval
+
+                interval = np.float64(self.operator.interval)
+                # arange doesn't include the end so we move it to the next tick
+                end = begin + ((end - begin) // interval + 1) * interval
+
                 dst_timestamps = np.arange(
                     begin,
-                    np.nextafter(end, math.inf),
-                    self.operator.interval,
+                    end,
+                    interval,
                     dtype=np.float64,
                 )
 
             output_evset.set_index_value(
                 index_key,
                 IndexData(
                     [],
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/tick_calendar.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/tick_calendar.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Implementation for the TickCalendar operator."""
 
-from typing import Dict, Literal, Union, Tuple
+from typing import Dict, Literal, Tuple, Union
 
 import numpy as np
 
-from temporian.implementation.numpy.data.event_set import IndexData, EventSet
 from temporian.core.operators.tick_calendar import TickCalendar
 from temporian.implementation.numpy import implementation_lib
+from temporian.implementation.numpy.data.event_set import EventSet, IndexData
 from temporian.implementation.numpy.operators.base import OperatorImplementation
 from temporian.implementation.numpy_cc.operators import operators_cc
 
 
 class TickCalendarNumpyImplementation(OperatorImplementation):
     def __init__(self, operator: TickCalendar) -> None:
         assert isinstance(operator, TickCalendar)
@@ -77,14 +77,17 @@
 
         # Weekday: convert python (wday=0 for Mon) to C++ (wday=0 for Sun)
         wday = self.operator.wday
         if wday != "*":
             wday = self._wday_py_to_cpp(wday)
         wday_range = self._get_arg_range(wday, self.operator.wday_max_range())
 
+        after_last = self.operator.after_last
+        before_first = self.operator.before_first
+
         # Fill output EventSet's data
         for index_key, index_data in input.data.items():
             if len(index_data.timestamps) == 0:
                 dst_timestamps = np.array([], dtype=np.float64)
             else:
                 dst_timestamps = operators_cc.tick_calendar(
                     start_timestamp=index_data.timestamps[0],
@@ -97,14 +100,16 @@
                     max_hour=hour_range[1],
                     min_mday=mday_range[0],
                     max_mday=mday_range[1],
                     min_month=month_range[0],
                     max_month=month_range[1],
                     min_wday=wday_range[0],
                     max_wday=wday_range[1],
+                    after_last=after_last,
+                    before_first=before_first,
                 )
             output_evset.set_index_value(
                 index_key,
                 IndexData(
                     features=[],
                     timestamps=dst_timestamps,
                     schema=output_schema,
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/timestamps.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/timestamps.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/unary.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/unary.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/unique_timestamps.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/unique_timestamps.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/until_next.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/until_next.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/where.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/where.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_count.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_count.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_max.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_max.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_min.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_min.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_product.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_product.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_standard_deviation.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/moving_standard_deviation.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy/operators/window/moving_sum.py` & `temporian-0.9.0/temporian/implementation/numpy/operators/window/simple_moving_average.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from temporian.core.operators.window.moving_sum import (
-    MovingSumOperator,
+from temporian.core.operators.window.simple_moving_average import (
+    SimpleMovingAverageOperator,
 )
 from temporian.implementation.numpy import implementation_lib
 from temporian.implementation.numpy.operators.window.base import (
     BaseWindowNumpyImplementation,
 )
 from temporian.implementation.numpy_cc.operators import operators_cc
 
 
-class MovingSumNumpyImplementation(BaseWindowNumpyImplementation):
-    """Numpy implementation of the moving sum operator."""
+class SimpleMovingAverageNumpyImplementation(BaseWindowNumpyImplementation):
+    """Numpy implementation of the simple moving average operator."""
 
     def _implementation(self):
-        return operators_cc.moving_sum
+        return operators_cc.simple_moving_average
 
 
 implementation_lib.register_operator_implementation(
-    MovingSumOperator, MovingSumNumpyImplementation
+    SimpleMovingAverageOperator, SimpleMovingAverageNumpyImplementation
 )
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy/test/registered_operators_test.py` & `temporian-0.9.0/temporian/implementation/numpy/test/registered_operators_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/__init__.py` & `temporian-0.9.0/temporian/implementation/numpy_cc/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/BUILD` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/__init__.py` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/add_index.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/add_index.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/calendar.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/calendar.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/common.h` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/common.h`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/filter_moving_count.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/filter_moving_count.cc`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 #include <vector>
 
 #include "temporian/implementation/numpy_cc/operators/common.h"
 
 namespace {
 namespace py = pybind11;
 
-py::array_t<double> filter_moving_count(
+py::array_t<Idx> filter_moving_count(
     const py::array_t<double> &event_timestamps, const double window_length) {
   // Input size
   const Idx n_event = event_timestamps.shape(0);
 
   // Access raw input / output data
   auto v_event = event_timestamps.unchecked<1>();
 
-  std::vector<double> output;
+  std::vector<Idx> output;
 
   // Index of the last emitted event. If -1, no event was emitted so far.
   Idx last_emitted_idx = -1;
 
   for (Idx event_idx = 0; event_idx < n_event; event_idx++) {
     const auto t = v_event[event_idx];
     if (last_emitted_idx == -1 ||
         (t - v_event[last_emitted_idx]) >= window_length) {
       // Emitting event.
       last_emitted_idx = event_idx;
-      output.push_back(t);
+      output.push_back(event_idx);
     }
   }
 
   return vector_to_np_array(output);
 }
 
 }  // namespace
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/join.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/join.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/pyinit.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/pyinit.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/resample.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/resample.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/since_last.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/since_last.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar_utils.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar_utils.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar_utils.h` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar_utils.h`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/tick_calendar_utils_test.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/tick_calendar_utils_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 TEST_P(UTCMkTimeTest, MatchExpected) {
   const UTCMkTimeTestCase& test_case = GetParam();
   const auto result =
       UTCMkTime(test_case.year, test_case.month, test_case.day, test_case.hour,
                 test_case.minute, test_case.second);
   EXPECT_TRUE(result.has_value());
-  EXPECT_EQ(result.value().seconds_since_epoch,
+  EXPECT_EQ((*result).seconds_since_epoch,
             test_case.expected_seconds_since_epoch);
-  EXPECT_EQ(result.value().wday, test_case.expected_wday);
+  EXPECT_EQ((*result).wday, test_case.expected_wday);
 }
 
 INSTANTIATE_TEST_SUITE_P(UTCMkTimeTestBase, UTCMkTimeTest,
                          testing::ValuesIn<UTCMkTimeTestCase>({
                              {1900, 1, 1, 0, 0, 0, -2208988800, 1 /*Monday*/},
 
                              {1963, 1, 1, 0, 0, 0, -220924800, 2},
```

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/until_next.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/until_next.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/implementation/numpy_cc/operators/window.cc` & `temporian-0.9.0/temporian/implementation/numpy_cc/operators/window.cc`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/__init__.py` & `temporian-0.9.0/temporian/io/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 from temporian.io.csv import to_csv
 from temporian.io.csv import from_csv
 
 from temporian.io.pandas import to_pandas
 from temporian.io.pandas import from_pandas
 
 from temporian.io.numpy import to_numpy
+
+from temporian.io.polars import to_polars
+from temporian.io.polars import from_polars
```

### Comparing `temporian-0.8.1/temporian/io/csv.py` & `temporian-0.9.0/temporian/io/csv.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/format.py` & `temporian-0.9.0/temporian/io/format.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/numpy.py` & `temporian-0.9.0/temporian/io/numpy.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/pandas.py` & `temporian-0.9.0/temporian/io/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         my_index
         red         0.5     2015-01-01
         red         0.6     2015-01-02
 
         ```
 
     Args:
-        evset: Input event set.
+        evset: Input EventSet.
         tp_string_to_pd_string: If true, cast Temporian strings (equivalent to
             np.string_ or np.bytes) to Pandas strings (equivalent to np.str_).
         timestamp_to_datetime: If true, cast Temporian timestamps to datetime64
             when is_unix_timestamp is set to True.
         timestamps: If true, the timestamps are included as a column.
 
     Returns:
```

### Comparing `temporian-0.8.1/temporian/io/parquet.py` & `temporian-0.9.0/temporian/io/parquet.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/tensorflow.py` & `temporian-0.9.0/temporian/io/tensorflow.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/test/BUILD` & `temporian-0.9.0/temporian/test/BUILD`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 package(
     default_visibility = ["//visibility:public"],
     licenses = ["notice"],
 )
 
 # Tests
 # =====
+
+py_library(
+    name = "utils",
+    srcs = ["utils.py"],
+    srcs_version = "PY3",
+    deps = [
+        # already_there/numpy
+        # already_there/absl/logging
+        # already_there/absl/testing:absltest
+        # already_there/absl/testing:parameterized
+        # already_there/google/protobuf:use_fast_cpp_protos
+        "//temporian/implementation/numpy/data:event_set",
+        "//temporian/core:serialization",
+    ],
+)
+
 py_test(
-    name = "pandas_test",
-    srcs = ["pandas_test.py"],
+    name = "api_test",
+    srcs = ["api_test.py"],
     srcs_version = "PY3",
     deps = [
+        # already_there/absl/logging
         # already_there/absl/testing:absltest
-        # already_there/numpy
         # already_there/absl/testing:parameterized
-        # already_there/pandas
-        "//temporian/test:utils",
-        "//temporian/implementation/numpy/data:io",
-        "//temporian/io:pandas",
+        # already_there/bokeh
+        # already_there/google/protobuf:use_fast_cpp_protos
+        # already_there/matplotlib
+        "//temporian",
     ],
 )
 
 py_test(
-    name = "numpy_test",
-    srcs = ["numpy_test.py"],
+    name = "api_beam_test",
+    srcs = ["api_beam_test.py"],
+    data = ["//temporian/test/test_data"],
     srcs_version = "PY3",
     deps = [
+        # already_there/absl/logging
         # already_there/absl/testing:absltest
-        # already_there/numpy
         # already_there/absl/testing:parameterized
-        "//temporian/test:utils",
-        "//temporian/implementation/numpy/data:io",
-        "//temporian/io:numpy",
+        # already_there/bokeh
+        # already_there/google/protobuf:use_fast_cpp_protos
+        # already_there/matplotlib
+        "//temporian",
+        "//temporian/beam",
     ],
 )
 
 py_test(
-    name = "tensorflow_test",
-    srcs = ["tensorflow_test.py"],
+    name = "doc_test",
+    srcs = ["doc_test.py"],
+    data = glob(["**/*.md"]),
     srcs_version = "PY3",
     deps = [
+        "//temporian",
         # already_there/absl/testing:absltest
         # already_there/absl/testing:parameterized
-        # already_there/numpy
-        # already_there/tensorflow
-        "//temporian/test:utils",
-        "//temporian/implementation/numpy/data:io",
-        "//temporian/io:tensorflow",
+        # already_there/google/protobuf:use_fast_cpp_protos
     ],
 )
 
 py_test(
-    name = "parquet_test",
-    srcs = ["parquet_test.py"],
+    name = "io_test",
+    srcs = ["io_test.py"],
+    data = ["//temporian/test/test_data"],
     srcs_version = "PY3",
     deps = [
         # already_there/absl/testing:absltest
-        # already_there/numpy
-        # already_there/pyarrow
-        "//temporian/test:utils",
-        "//temporian/implementation/numpy/data:io",
-        "//temporian/io:parquet",
+        # already_there/absl/testing:parameterized
+        # already_there/google/protobuf:use_fast_cpp_protos
+        # already_there/pandas
+        "//temporian",
+        ":utils",
     ],
-)
+)
```

### Comparing `temporian-0.8.1/temporian/io/test/numpy_test.py` & `temporian-0.9.0/temporian/io/test/numpy_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/test/pandas_test.py` & `temporian-0.9.0/temporian/io/test/pandas_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from absl.testing import absltest
 
 from temporian.implementation.numpy.data.io import event_set
 from temporian.io.pandas import from_pandas, to_pandas
 from temporian.test.utils import assertEqualDFRandomRowOrder
 
 
-class DataFrameToEventTest(absltest.TestCase):
+class FromPandasTest(absltest.TestCase):
     def test_correct(self) -> None:
         df = pd.DataFrame(
             [
                 [666964, 1.0, 740.0],
                 [666964, 2.0, 508.0],
                 [574016, 3.0, 573.0],
             ],
@@ -415,14 +415,16 @@
                 "x": ["a", "nan", "b"],
                 "y": [1, 2, 3],
             },
         )
 
         self.assertEqual(evset, expected_evset)
 
+
+class ToPandasTest(absltest.TestCase):
     def test_evset_to_df(self) -> None:
         evset = event_set(
             timestamps=[1.0, 2.0, 3.0],
             features={
                 "product_id": [666964, 666964, 574016],
                 "costs": [740.0, 508.0, 573.0],
             },
```

### Comparing `temporian-0.8.1/temporian/io/test/parquet_test.py` & `temporian-0.9.0/temporian/io/test/parquet_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/io/test/tensorflow_test.py` & `temporian-0.9.0/temporian/io/test/tensorflow_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/proto/__init__.py` & `temporian-0.9.0/temporian/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/proto/core.proto` & `temporian-0.9.0/temporian/proto/core.proto`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/test/api_beam_test.py` & `temporian-0.9.0/temporian/test/api_beam_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/test/api_test.py` & `temporian-0.9.0/temporian/test/api_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,14 +105,27 @@
             },
         )
 
         df = tp.to_pandas(evset)
         reconstructed_evset = tp.from_pandas(df)
         self.assertEqual(evset, reconstructed_evset)
 
+    def test_polars(self):
+        evset = tp.event_set(
+            timestamps=[0.0, 2.0, 4.0, 6.0],
+            features={
+                "f1": [1.0, 2.0, 3.0, 4.0],
+                "f2": [5.0, 6.0, 7.0, 8.0],
+            },
+        )
+
+        df = tp.to_polars(evset)
+        reconstructed_evset = tp.from_polars(df)
+        self.assertEqual(evset, reconstructed_evset)
+
     def test_serialization(self):
         a = tp.input_node([("f1", tp.float32), ("f2", tp.float32)])
         b = a.simple_moving_average(window_length=7)
 
         with tempfile.TemporaryDirectory() as tempdir:
             path = os.path.join(tempdir, "my_graph.tem")
             tp.save_graph(inputs={"a": a}, outputs={"b": b}, path=path)
@@ -200,10 +213,24 @@
 
     def test_duration_to_string(self):
         self.assertEqual(
             tp.duration.to_string(tp.duration.days(2) + tp.duration.hours(3)),
             "2d3h",
         )
 
+    def test_schema_to_from_proto(self):
+        a = tp.Schema(features=[("f1", tp.int32), ("f2", tp.float64)])
+        p = a.to_proto()
+        b = tp.Schema.from_proto(p)
+        self.assertEqual(a, b)
+
+    def test_schema_to_from_proto_file(self):
+        with tempfile.TemporaryDirectory() as tempdir:
+            path = os.path.join(tempdir, "schema.pbtxt")
+            a = tp.Schema(features=[("f1", tp.int32), ("f2", tp.float64)])
+            a.to_proto_file(path)
+            b = tp.Schema.from_proto_file(path)
+            self.assertEqual(a, b)
+
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `temporian-0.8.1/temporian/test/doc_test.py` & `temporian-0.9.0/temporian/test/doc_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import doctest
 import tempfile
 from pathlib import Path
 from typing import List
 
 import numpy as np
 import pandas as pd
+import polars as pl
 from absl.testing import absltest
 
 import temporian as tp
 
 
 class DocTest(absltest.TestCase):
     """
@@ -58,14 +59,15 @@
                     doctest.testfile(
                         str(path),
                         module_relative=False,
                         raise_on_error=True,
                         globs={
                             "np": np,
                             "pd": pd,
+                            "pl": pl,
                             "tp": tp,
                             "tmp_dir": tmp_dir,
                         },
                         # Use ... to match anything and ignore different whitespaces
                         optionflags=doctest.ELLIPSIS
                         | doctest.NORMALIZE_WHITESPACE,
                         verbose=False,
```

### Comparing `temporian-0.8.1/temporian/test/io_test.py` & `temporian-0.9.0/temporian/test/io_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/test/utils.py` & `temporian-0.9.0/temporian/test/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -130,14 +130,35 @@
             f"{real}"
             "\n==========\nEXPECTED:\n==========\n"
             f"{expected}"
         ),
     )
 
 
+def assertEqualDFRandomRowOrderPolars(
+    test: absltest.TestCase, real: "pl.DataFrame", expected: "pl.DataFrame"
+):
+    list_real = real.to_dicts()
+    list_expected = expected.to_dicts()
+
+    sorted_real = sorted(list_real, key=lambda x: str(x))
+    sorted_expected = sorted(list_expected, key=lambda x: str(x))
+
+    test.assertEqual(
+        sorted_real,
+        sorted_expected,
+        (
+            "\n==========\nREAL:\n==========\n"
+            f"{real}"
+            "\n==========\nEXPECTED:\n==========\n"
+            f"{expected}"
+        ),
+    )
+
+
 class SetTimezone:
     def __init__(self, timezone: str = "America/Montevideo"):
         self._tz = timezone
         self._restore_tz = ""
 
     def __enter__(self):
         self._restore_tz = os.environ.get("TZ", "")
```

### Comparing `temporian-0.8.1/temporian/utils/BUILD` & `temporian-0.9.0/temporian/utils/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/compile.bzl` & `temporian-0.9.0/temporian/utils/compile.bzl`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/config.py` & `temporian-0.9.0/temporian/utils/config.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/golden.py` & `temporian-0.9.0/temporian/utils/golden.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/string.py` & `temporian-0.9.0/temporian/utils/string.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/test/BUILD` & `temporian-0.9.0/temporian/utils/test/BUILD`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/test/string_test.py` & `temporian-0.9.0/temporian/utils/test/string_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/test/typecheck_test.py` & `temporian-0.9.0/temporian/utils/test/typecheck_test.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/temporian/utils/typecheck.py` & `temporian-0.9.0/temporian/utils/typecheck.py`

 * *Files identical despite different names*

### Comparing `temporian-0.8.1/setup.py` & `temporian-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 packages = \
 ['temporian',
  'temporian.api',
  'temporian.beam',
  'temporian.beam.io',
  'temporian.beam.io.test',
  'temporian.beam.operators',
+ 'temporian.beam.operators.binary',
+ 'temporian.beam.operators.scalar',
  'temporian.beam.operators.test',
  'temporian.beam.operators.window',
  'temporian.beam.operators.window.test',
  'temporian.beam.test',
  'temporian.core',
  'temporian.core.data',
  'temporian.core.data.test',
@@ -51,21 +53,24 @@
 install_requires = \
 ['absl-py>=1.3.0,<2.0.0',
  'matplotlib>=3.7.1,<4.0.0',
  'pandas>=1.5.2',
  'protobuf>=3.20.3']
 
 extras_require = \
-{'all': ['apache-beam>=2.48.0,<3.0.0', 'tensorflow>=2.12.0,<3.0.0'],
+{'all': ['apache-beam>=2.48.0,<3.0.0',
+         'tensorflow>=2.12.0,<2.16',
+         'polars>=0.20.15,<0.21.0'],
  'beam': ['apache-beam>=2.48.0,<3.0.0'],
- 'tensorflow': ['tensorflow>=2.12.0,<3.0.0']}
+ 'polars': ['polars>=0.20.15,<0.21.0'],
+ 'tensorflow': ['tensorflow>=2.12.0,<2.16']}
 
 setup_kwargs = {
     'name': 'temporian',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Temporian is a Python package for feature engineering of temporal data, focusing on preventing common modeling errors and providing a simple and powerful API, a first-class iterative development experience, and efficient and well-tested implementations of common and not-so-common temporal data preprocessing functions.',
     'long_description': '<img src="https://github.com/google/temporian/raw/main/docs/src/assets/banner.png" width="100%" alt="Temporian logo">\n\n[![pypi](https://img.shields.io/pypi/v/temporian?color=blue)](https://pypi.org/project/temporian/)\n[![docs](https://readthedocs.org/projects/temporian/badge/?version=stable)](https://temporian.readthedocs.io/en/stable/?badge=stable)\n![tests](https://github.com/google/temporian/actions/workflows/test.yaml/badge.svg)\n![formatting](https://github.com/google/temporian/actions/workflows/formatting.yaml/badge.svg)\n![publish](https://github.com/google/temporian/actions/workflows/publish.yaml/badge.svg)\n\n**Temporian** is a library for **safe**, **simple** and **efficient** preprocessing and feature engineering of temporal data in Python. Temporian supports multivariate time-series, multivariate time-sequences, event logs, and cross-source event streams.\n\nTemporian is to [temporal data](https://temporian.readthedocs.io/en/stable/user_guide/#what-is-temporal-data) what Pandas is to tabular data.\n\n## Key features\n\n- **Supports most types of temporal data** 📈: Handles both uniformly sampled and\n  non-uniformly sampled data, both single-variate and multivariate data, both flat\n  and multi-index data, and both mono-source and multi-source non-synchronized\n  events.\n\n- **Optimized for Temporal data** 🔥: Temporian\'s core computation is\n  implemented in C++ and optimized for temporal data. Temporian can be more than\n  1,000x faster than off-the-shelf data processing libraries when operating on\n  temporal data.\n\n- **Easy to integrate into an existing ML ecosystem**: Temporian does not perform any ML model training - instead it integrates seamlessly with any ML library, such as PyTorch, Scikit-Learn, Jax, TensorFlow, XGBoost, or Yggdrasil Decision Forests.\n\n- **Prevents unwanted future leakage** 😰: Unless explicitly specified with\n  `tp.leak`, feature computation cannot depend on future data, thereby preventing\n  unwanted, hard-to-debug, and potentially costly future leakage.\n\n<!--\n- **Iterative and interactive development** 📊: Users can easily analyze\n  temporal data and visualize results in real-time with iterative tools like\n  notebooks. When prototyping, users can iteratively preprocess, analyze, and\n  visualize temporal data in real-time with notebooks. In production, users\n  can easily reuse, apply, and scale these implementations to larger datasets.\n\n- **Flexible runtime** ☁️: Temporian programs can run seamlessly in-process in\n  Python, on large datasets using [Apache Beam](https://beam.apache.org/).\n-->\n\n## Quickstart\n\n### Installation\n\nInstall Temporian from [PyPI](https://pypi.org/project/temporian/) with `pip`:\n\n```shell\npip install temporian -U\n```\n\nTemporian is currently available for Linux and MacOS (ARM and Intel). Windows support is under development.\n\n### Minimal example\n\nConsider sale records that contain contain the `timestamp`, `store`, and `revenue` of individual sales.\n\n```shell\n$ cat sales.csv\ntimestamp,store,revenue\n2023-12-04 21:21:05,STORE_31,5071\n2023-11-08 17:14:38,STORE_4,1571\n2023-11-29 21:44:46,STORE_49,6101\n2023-12-20 18:17:14,STORE_18,4499\n2023-12-15 10:55:09,STORE_2,6666\n...\n```\n\nOur goal is to compute the sum of revenue for each store at 11 pm every weekday (excluding weekends).\n\nFirst, we load the data and list the workdays.\n\n```python\nimport temporian as tp\n\n# Load sale transactions\nsales = tp.from_csv("sales.csv")\n\n# Index sales per store\nsales_per_store = sales.add_index("store")\n\n# List work days\ndays = sales_per_store.tick_calendar(hour=22)\nwork_days = (days.calendar_day_of_week() <= 5).filter()\n\nwork_days.plot(max_num_plots=1)\n```\n\n![](https://github.com/google/temporian/raw/main/docs/src/assets/frontpage_workdays.png)\n\nThen, we sum the daily revenue for each workday and each store.\n\n```python\n# Aggregate revenue per store and per work day\ndaily_revenue = sales_per_store["revenue"].moving_sum(tp.duration.days(1), sampling=work_days).rename("daily_revenue")\n\n# Plot the results\ndaily_revenue.plot(max_num_plots=3)\n```\n\n![](https://github.com/google/temporian/raw/main/docs/src/assets/frontpage_aggregated_revenue.png)\n\nFinally, we can export the result as a Pandas DataFrame for further processing or for consumption by other libraries.\n\n```python\ntp.to_pandas(daily_revenue)\n```\n\n![](https://github.com/google/temporian/raw/main/docs/src/assets/frontpage_pandas.png)\n\nCheck the [Getting Started tutorial](https://temporian.readthedocs.io/en/stable/tutorials/getting_started/) to find out more!\n\n## Next steps\n\nNew users should refer to the [Getting Started](https://temporian.readthedocs.io/en/stable/getting_started/) guide, which provides a\nquick overview of the key concepts and operations of Temporian.\n\nAfter that, visit the [User Guide](https://temporian.readthedocs.io/en/stable/user_guide/) for a deep dive into\nthe major concepts, operators, conventions, and practices of Temporian. For a\nhands-on learning experience, work through the [Tutorials](https://temporian.readthedocs.io/en/stable/tutorials/) or refer to the [API\nreference](https://temporian.readthedocs.io/en/stable/reference/).\n\nIf you need help, have a question, want to contribute, or just want to be a part of the Temporian community, we encourage you to join our [Discord](https://discord.gg/nT54yATCTy) server! 🤝🏼\n\n## Documentation\n\nThe documentation 📚 is available at [temporian.readthedocs.io](https://temporian.readthedocs.io/en/stable/). The [Getting Started guide](https://temporian.readthedocs.io/en/stable/getting_started/) is the best way to start.\n\n## Contributing\n\nContributions to Temporian are welcome! Check out the [Contributing guide](https://temporian.readthedocs.io/en/stable/contributing/) to get started.\n\n## Credits\n\nTemporian is developed in collaboration between Google and [Tryolabs](https://tryolabs.com/).\n',
     'author': 'Mathieu Guillame-Bert, Braulio Ríos, Guillermo Etchebarne, Ian Spektor, Richard Stotz',
     'author_email': 'gbm@google.com',
     'maintainer': 'Mathieu Guillame-Bert',
     'maintainer_email': 'gbm@google.com',
     'url': 'https://github.com/google/temporian',
```

### Comparing `temporian-0.8.1/PKG-INFO` & `temporian-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temporian
-Version: 0.8.1
+Version: 0.9.0
 Summary: Temporian is a Python package for feature engineering of temporal data, focusing on preventing common modeling errors and providing a simple and powerful API, a first-class iterative development experience, and efficient and well-tested implementations of common and not-so-common temporal data preprocessing functions.
 Home-page: https://github.com/google/temporian
 License: Apache 2.0
 Author: Mathieu Guillame-Bert, Braulio Ríos, Guillermo Etchebarne, Ian Spektor, Richard Stotz
 Author-email: gbm@google.com
 Maintainer: Mathieu Guillame-Bert
 Maintainer-email: gbm@google.com
@@ -24,21 +24,23 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: beam
+Provides-Extra: polars
 Provides-Extra: tensorflow
 Requires-Dist: absl-py (>=1.3.0,<2.0.0)
 Requires-Dist: apache-beam (>=2.48.0,<3.0.0) ; extra == "beam" or extra == "all"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=1.5.2)
+Requires-Dist: polars (>=0.20.15,<0.21.0) ; extra == "polars" or extra == "all"
 Requires-Dist: protobuf (>=3.20.3)
-Requires-Dist: tensorflow (>=2.12.0,<3.0.0) ; extra == "tensorflow" or extra == "all"
+Requires-Dist: tensorflow (>=2.12.0,<2.16) ; extra == "tensorflow" or extra == "all"
 Project-URL: Repository, https://github.com/google/temporian
 Description-Content-Type: text/markdown
 
 <img src="https://github.com/google/temporian/raw/main/docs/src/assets/banner.png" width="100%" alt="Temporian logo">
 
 [![pypi](https://img.shields.io/pypi/v/temporian?color=blue)](https://pypi.org/project/temporian/)
 [![docs](https://readthedocs.org/projects/temporian/badge/?version=stable)](https://temporian.readthedocs.io/en/stable/?badge=stable)
```

